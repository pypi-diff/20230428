# Comparing `tmp/pdt_extract-0.1.3-py3-none-any.whl.zip` & `tmp/pdt_extract-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 8573 bytes, number of entries: 7
+Zip file size: 10635 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    11413 b- defN 23-Apr-25 23:53 pdt_canny.py
 -rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-26 19:26 pdt_extract/__init__.py
--rw-rw-rw-  2.0 fat    11416 b- defN 23-Apr-26 19:26 pdt_extract/pdt_extract.py
--rw-rw-rw-  2.0 fat      640 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      545 b- defN 23-Apr-26 19:27 pdt_extract-0.1.3.dist-info/RECORD
-7 files, 24192 bytes uncompressed, 7609 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat     5714 b- defN 23-Apr-28 19:45 pdt_extract/feature_extract.py
+-rw-rw-rw-  2.0 fat    11582 b- defN 23-Apr-28 15:55 pdt_extract/pdt_extract.py
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      632 b- defN 23-Apr-28 19:48 pdt_extract-0.1.4.dist-info/RECORD
+8 files, 30181 bytes uncompressed, 9535 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: pdt_canny.py
 Comment: 
 
 Filename: pdt_extract/__init__.py
 Comment: 
 
+Filename: pdt_extract/feature_extract.py
+Comment: 
+
 Filename: pdt_extract/pdt_extract.py
 Comment: 
 
-Filename: pdt_extract-0.1.3.dist-info/METADATA
+Filename: pdt_extract-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pdt_extract-0.1.3.dist-info/WHEEL
+Filename: pdt_extract-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pdt_extract-0.1.3.dist-info/top_level.txt
+Filename: pdt_extract-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pdt_extract-0.1.3.dist-info/RECORD
+Filename: pdt_extract-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdt_extract/pdt_extract.py

```diff
@@ -1,106 +1,103 @@
 """
-Author: Dmitri Lyalikov-Dlyalikov01@manhattan.edu
+Author: Dmitri Lyalikov
+Email:  Dlyalikov01@manhattan.edu
+Date of last revision: 04/28/2023
+
+Status:
+    in development / validating
+
+pdt-extract.py
+    This module is the entry point and controller of the profile and feature extraction sequence
+    implemented by the pdt-extract project.
+    It can be used as a standalone script or imported with DropProfile class to:
+        - process one or more image files from the folder: path, or from a single .png file or image (ndarray)
+        - output the extracted canny generated drop profile to the subdirectory: dest
+        - extract and generate a .csv file of characteristic features to file: dest/feature_set.csv
 
-Canny Edge Detection Processor
-This module will process all image files from the folder: pendant_drops
-and output the extracted canny generated drop profile to the subdirectory: drop_profiles
-
-TODO: Implement Feature extraction from apex radius and:
-    - generate CSV of features from all profiles with extract_from_dir
-    - return dictionary of features {Drop Height, Capillary Radius, Rs, Re} with extract_from_file, extract_from_img
 """
 
 import imageio
 import os
 from scipy import ndimage
+from feature_extract import FeatureExtract
 
 import numpy as np
 from numpy import fft
 import matplotlib.pyplot as plt
-from circle_fit import taubinSVD
+import pandas as pd
 
 
 class DropProfile:
-    def __init__(self, path="Pendant Drops", dest="Drop Profiles"):
+    def __init__(self, path: str = "../Pendant Drops", dest: str = "Drop Profiles", feature_set: str = "features.csv"):
+        """
+        :param path: poth to directory to access input images.
+        :param dest: path to subdir to save output images. It is assumed destination dir is a subdirectory in path: (path/dest)
+        :param feature_set: file name to save feature set as csv to (should include .csv)
+        """
         self.path = path
         self.destination = dest
+        self.feature_set = feature_set
         self.max_height = 0
         self.max_width = 0
+        self.feature_list = []
 
     # Perform bulk profile and feature extraction on all files in self.path
     # generate drop profile .jpg and save to self.destination
     def extract_from_dir(self):
+        os.chdir("../pdt_extract")
         os.chdir(self.path)
         for filename in os.listdir():
             if not os.path.isdir(filename):
                 print(f"Extracting profile from: {filename}...")
                 profile = extract_profile_from_image(os.path.join(filename))
                 os.chdir(self.destination)
-                get_profile(profile, filename)
-                os.chdir("../..")
+                self.get_profile(profile, filename)
+                os.chdir("..")
             else:
                 print(f"not file: {filename}")
+        df = pd.DataFrame(self.feature_list)
+        df.to_csv(self.destination + '/' + self.feature_set, index=False)
+        os.chdir("../pdt_extract")
 
         print(f"Done Extracting Profiles")
 
     # perform extraction of profile and feature set given a path to an image with respect to self.path
     def extract_from_file(self, fname: str) -> (ndimage, list):
         os.chdir(self.path)
         profile = extract_profile_from_image(os.path.join(fname))
-        return get_profile(profile)
+        return self.get_profile(profile)
 
     # perform extraction of profile and feature set given a ndimage
     def extract_from_img(self, img: ndimage) -> (ndimage, list):
         profile = extract_profile_from_image(img, load=False, path_to_file=None)
 
-
-# label connected components as edge profiles
-def get_profile(final_image, filename=None, save=True):
-    labeled_image, num_features = ndimage.label(final_image)
-    # Remove feature 2 which is the internal noise from light
-    final_image[labeled_image == 2] = 0
-    final_image[labeled_image == 1] = 255
-    final_image = split_profile(final_image)
-    R0 = find_apex_radius(final_image, 0.15, 0.005)
-    print(f"Apex_Radius (cm): {R0}")  # 0.05 /44
-    show_image(final_image)
-
-    fft_profile(final_image)
-    if save:
-        imageio.imwrite(filename, np.uint8(final_image))
-    else:
-        return final_image, {"Apex Radius": R0}
-
-
-# Use Circle fit to approximate apex radius of edge profile
-# ratio_drop_length: 1 >= float value > 0 representing number points along profile to approximate with
-# change_ro: float value representing minimum value of change in circle radius before stopping approximation
-def find_apex_radius(profile: ndimage, ratio_drop_length: float, change_ro: float) -> float:
-    indices = np.where(profile == 255)
-    x = np.flip(indices[1])
-    y = np.flip(indices[0])
-
-    num_point_ro_circlefit = round(len(x) * ratio_drop_length) + 1
-
-    percent_drop_ro = 0.1
-    i = 0
-    diff = 0
-    r0 = 0
-    r_0 = []
-    while diff >= change_ro*r0 or num_point_ro_circlefit <= percent_drop_ro * len(x):
-        points_ro_circlefit = np.stack((x[:num_point_ro_circlefit], y[:num_point_ro_circlefit]), axis=1)
-        xc, yc, r0, sigma = taubinSVD(points_ro_circlefit)
-        r_0.append(r0)
-        if i > 1:
-            diff = abs(r_0[i] - r_0[i-1])
-        i += 1
-        num_point_ro_circlefit += 1
-
-    return r_0[-1]
+    # label connected components as edge profiles
+    def get_profile(self, final_image, filename=None, save=True):
+        labeled_image, num_features = ndimage.label(final_image)
+        # Remove feature 2 which is the internal noise from light
+        final_image[labeled_image == 2] = 0
+        final_image[labeled_image == 1] = 255
+        final_image = split_profile(final_image)
+
+        # Create ordered set of X and Y coordinates along edge profile
+        indices = np.where(final_image == 255)
+        x = np.flip(indices[1])
+        y = np.flip(indices[0])
+        # Extract and save profile features to feature list
+        features = FeatureExtract(x, y)
+        features.feature_set["image"] = filename
+        self.feature_list.append(features.feature_set)
+        show_image(final_image)
+
+        fft_profile(final_image)
+        if save:
+            imageio.imwrite(filename, np.uint8(final_image))
+        else:
+            return final_image, features.feature_set
 
 
 #    Execute the Canny Sequence on the image
 #    gaussian_blur_sigma value = 1.2
 #    high_threshold_ratio = 0.2
 #    low_threshold_ratio = 0.15
 def extract_profile_from_image(path_to_file: str, img: ndimage = None, load=True):
```

## Comparing `pdt_extract-0.1.3.dist-info/METADATA` & `pdt_extract-0.1.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pdt-extract
-Version: 0.1.3
+Version: 0.1.4
 Summary: Perform edge profile and characteristic feature extraction from images of pendant drops
 Home-page: https://github.com/DmitriLyalikov/pdt-canny-edge-detector
 Author: Dmitri Lyalikov
 Author-email: Dlyalikov01@manhattan.edu
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 Requires-Dist: imageio
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: circle-fit
+Requires-Dist: pandas
 
 This package provides modules and automation to perform edge profile extraction and characteristic feature approximation from pendant drop images.
```

## Comparing `pdt_extract-0.1.3.dist-info/RECORD` & `pdt_extract-0.1.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 pdt_canny.py,sha256=H9B7o4vPiWQoMjiu6J8d5uIk2FHaCQNmWz0NMTOuF3Y,11413
 pdt_extract/__init__.py,sha256=4lNIpyPWiCe7y_Ksf3ZEb9qB0D7WJ1FMJGDwY0Qywjg,74
-pdt_extract/pdt_extract.py,sha256=zhqg5hvnJmjXQkpitGbR_VMiVb-4-rgTCoZ1XML8PXY,11416
-pdt_extract-0.1.3.dist-info/METADATA,sha256=7qpBd_9JUcq2Dl2W7v2pVW3-uFGo8C8NlDq3fL9_RVw,640
-pdt_extract-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pdt_extract-0.1.3.dist-info/top_level.txt,sha256=QCEOHNPwd72hz8668WATwVkOuYdskgLisqco3A-kRSQ,12
-pdt_extract-0.1.3.dist-info/RECORD,,
+pdt_extract/feature_extract.py,sha256=w-aKaQ2Mm0U3ITQ8Ygro1IlrSDxi2n_2Zyy5FVea0b8,5714
+pdt_extract/pdt_extract.py,sha256=nPiGN4Y8G8Mm2nJghk2qdeQ5mpi3bQzWPinW2KjBHbo,11582
+pdt_extract-0.1.4.dist-info/METADATA,sha256=1DaEGpF6olHaFsXi-IeRWS9GudNz27eVoobf6blndRI,662
+pdt_extract-0.1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pdt_extract-0.1.4.dist-info/top_level.txt,sha256=QCEOHNPwd72hz8668WATwVkOuYdskgLisqco3A-kRSQ,12
+pdt_extract-0.1.4.dist-info/RECORD,,
```

