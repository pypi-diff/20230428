# Comparing `tmp/i3dFeatureExtraction-0.2.8.tar.gz` & `tmp/i3dFeatureExtraction-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.2.8.tar", last modified: Tue Apr 18 07:44:31 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.2.9.tar", last modified: Fri Apr 28 09:11:08 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.2.8.tar` & `i3dFeatureExtraction-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3797 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-04-18 07:16:31.000000 i3dFeatureExtraction-0.2.8/README.md
--rw-rw-rw-   0        0        0     3338 2023-04-18 07:44:02.000000 i3dFeatureExtraction-0.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.055423 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.078998 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.081996 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/__init__.py
--rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/convert_weights.py
--rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/pretrained_existed.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.072842 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0     3797 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      677 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-18 07:44:16.000000 i3dFeatureExtraction-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:11:08.099618 i3dFeatureExtraction-0.2.9/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4585 2023-04-28 09:11:08.098613 i3dFeatureExtraction-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3858 2023-04-28 08:54:16.000000 i3dFeatureExtraction-0.2.9/README.md
+-rw-rw-rw-   0        0        0     4126 2023-04-28 09:10:52.000000 i3dFeatureExtraction-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 09:11:08.079616 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4190 2023-04-28 08:33:43.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    11165 2023-04-28 08:13:24.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:11:08.094616 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:11:08.097613 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/__init__.py
+-rw-rw-rw-   0        0        0     2714 2023-04-28 07:48:47.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/convert_weights.py
+-rw-rw-rw-   0        0        0     3227 2023-04-28 07:49:05.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/pretrained_existed.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:11:08.088655 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0     4585 2023-04-28 09:11:07.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-04-28 09:11:08.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:11:07.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:11:07.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-28 09:11:07.000000 i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:11:08.099618 i3dFeatureExtraction-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-28 09:06:45.000000 i3dFeatureExtraction-0.2.9/setup.py
```

### Comparing `i3dFeatureExtraction-0.2.8/LICENSE.txt` & `i3dFeatureExtraction-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/PKG-INFO` & `i3dFeatureExtraction-0.2.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -35,15 +35,14 @@
 Usage
 -----
 
 Installation
 ~~~~~~~~~~~~
 
 Before installing my package, please install these pakages:
-
 \*
 `Opencv-Python==4.5.5 <https://www.lfd.uci.edu/~gohlke/pythonlibs/#opencv>`__
 
 \*
 `torch==1.10.1+cu113 <https://download.pytorch.org/whl/cu113/torch-1.10.1%2Bcu113-cp38-cp38-win_amd64.whl>`__
 
 \*
@@ -61,55 +60,65 @@
 .. code:: commandline
 
    pip install torchvision-0.11.2+cu113-cp38-cp38-win_amd64.whl
    pip install torchaudio-0.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install torch-1.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install opencv_python-4.5.5-cp38-cp38-win_amd64.whl
 
-
 After 4 above packages, to install ``i3dFeatureExtraction`` package into
 your Python environment, run this code on your terminal:
 
 .. code:: commandline
 
    pip install i3dFeatureExtraction
 
-Or install a specific version:
-
-.. code:: commandline
-
-   pip install i3dFeatureExtraction==x.x.x
 
 Implementing
 ~~~~~~~~~~~~
 
 The main function of this package is ``FeatureExtraction`` which
 converts a directory of videos into numpy feature files.
 
 .. code:: python
 
    from i3dFeatureExtraction import FeatureExtraction
    FeatureExtraction.generate(
-       outputpath = "directory/to/store/output/numpy/files",
        datasetpath="directory/of/input/videos",
+       outputpath = "directory/to/store/output/numpy/files",
        pretrainedpath = "path/to/i3D/pretrained/weight",
        sample_mode = "oversample/center_crop"
+       multiplefiles = True/False
    )
 
+-  **datasetpath** (REQUIRED): path to videos.
+-  If **multiplefiles** is *True* (default), the **datasetpath** is the
+   path to a directory which contains 1 or more videos.
+-  If **multiplefiles** is *False*, the **datasetpath** is the path to a
+   video.
+-  **outputpath** (optional, default: *“output/”*): the proccessed numpy
+   feature files would be stored in this directory.
+-  **pretrainedpath** (optional, default: *“pretrained/”*): the path of
+   the pretrained i3d weight. If the weight is not existed, it will be
+   downloaded and created manually.
+-  **sample_mode** (optional, default: *“oversample/”*) receive
+   “oversample” or “center_crop”. If *oversample*, each frame will be
+   cropped and flipped to be turned into 10 frames.
+
+
 --------------
-Structure
---------------
+
+Structure of this package
+--------------------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
-   :alt: i3dFeatureExtraction - UML Diagram
+![i3dFeatureExtraction - UML Diagram](https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png)
 
 Credits
------------
+-------
 
 This code is based on the following repositories:
 
 \*
 `pytorch-resnet3d <https://github.com/Tushar-N/pytorch-resnet3d>`__
 
 \*
@@ -118,8 +127,8 @@
 \*
 `E2E-Action-Segmentation/feature_extraction/ <https://github.com/nguyenphwork/E2E-Action-Segmentation/tree/main/feature_extraction>`__
 
 I would like to extend a special thank-you to the original authors of
 these repositories for providing the foundation on which this
 implementation is built.
 
-
+.. |i3dFeatureExtraction - UML Diagram| image:: UML/i3dExtract.png
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `i3dFeatureExtraction-0.2.8/README.rst` & `i3dFeatureExtraction-0.2.9/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 Usage
 -----
 
 Installation
 ~~~~~~~~~~~~
 
 Before installing my package, please install these pakages:
-
 \*
 `Opencv-Python==4.5.5 <https://www.lfd.uci.edu/~gohlke/pythonlibs/#opencv>`__
 
 \*
 `torch==1.10.1+cu113 <https://download.pytorch.org/whl/cu113/torch-1.10.1%2Bcu113-cp38-cp38-win_amd64.whl>`__
 
 \*
@@ -48,55 +47,65 @@
 .. code:: commandline
 
    pip install torchvision-0.11.2+cu113-cp38-cp38-win_amd64.whl
    pip install torchaudio-0.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install torch-1.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install opencv_python-4.5.5-cp38-cp38-win_amd64.whl
 
-
 After 4 above packages, to install ``i3dFeatureExtraction`` package into
 your Python environment, run this code on your terminal:
 
 .. code:: commandline
 
    pip install i3dFeatureExtraction
 
-Or install a specific version:
-
-.. code:: commandline
-
-   pip install i3dFeatureExtraction==x.x.x
 
 Implementing
 ~~~~~~~~~~~~
 
 The main function of this package is ``FeatureExtraction`` which
 converts a directory of videos into numpy feature files.
 
 .. code:: python
 
    from i3dFeatureExtraction import FeatureExtraction
    FeatureExtraction.generate(
-       outputpath = "directory/to/store/output/numpy/files",
        datasetpath="directory/of/input/videos",
+       outputpath = "directory/to/store/output/numpy/files",
        pretrainedpath = "path/to/i3D/pretrained/weight",
        sample_mode = "oversample/center_crop"
+       multiplefiles = True/False
    )
 
+-  **datasetpath** (REQUIRED): path to videos.
+-  If **multiplefiles** is *True* (default), the **datasetpath** is the
+   path to a directory which contains 1 or more videos.
+-  If **multiplefiles** is *False*, the **datasetpath** is the path to a
+   video.
+-  **outputpath** (optional, default: *“output/”*): the proccessed numpy
+   feature files would be stored in this directory.
+-  **pretrainedpath** (optional, default: *“pretrained/”*): the path of
+   the pretrained i3d weight. If the weight is not existed, it will be
+   downloaded and created manually.
+-  **sample_mode** (optional, default: *“oversample/”*) receive
+   “oversample” or “center_crop”. If *oversample*, each frame will be
+   cropped and flipped to be turned into 10 frames.
+
+
 --------------
-Structure
---------------
+
+Structure of this package
+--------------------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
-   :alt: i3dFeatureExtraction - UML Diagram
+![i3dFeatureExtraction - UML Diagram](https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png)
 
 Credits
------------
+-------
 
 This code is based on the following repositories:
 
 \*
 `pytorch-resnet3d <https://github.com/Tushar-N/pytorch-resnet3d>`__
 
 \*
@@ -105,8 +114,8 @@
 \*
 `E2E-Action-Segmentation/feature_extraction/ <https://github.com/nguyenphwork/E2E-Action-Segmentation/tree/main/feature_extraction>`__
 
 I would like to extend a special thank-you to the original authors of
 these repositories for providing the foundation on which this
 implementation is built.
 
-
+.. |i3dFeatureExtraction - UML Diagram| image:: UML/i3dExtract.png
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 import torch.nn.functional as F
 import torch.optim as optim
 from torch.optim import lr_scheduler
 from torch.autograd import Variable
 import torchvision
 import os
 
-from .extract_features import I3DFeaturesExtractor
+from extract_features import I3DFeaturesExtractor
 
 class FeatureExtraction:
     def __init__(self, datasetpath="samplevideos/", outputpath="output", 
                  pretrainedpath="pretrained/i3d_r50_kinetics.pth",
                  frequency=16, batch_size=20, sample_mode="oversample"):
         self.datasetpath = datasetpath
         self.outputpath = outputpath
         self.pretrainedpath = pretrainedpath
         self.frequency = frequency
         self.batch_size = batch_size
         self.sample_mode = sample_mode
     @staticmethod
-    def generate(outputpath="output", datasetpath="samplevideos/", 
+    def generate(datasetpath="samplevideos/", outputpath="output",
                  pretrainedpath="pretrained/i3d_r50_kinetics.pth", 
-                 frequency=16, batch_size=20, sample_mode="oversample"):        
+                 frequency=16, batch_size=20, sample_mode="oversample", multiplefiles = True):
         '''
         Processing to turn an input video into a i3d features numpy file.
         Arg:
           outputpath (str): path to the directory saving the i3d generated output feature files.
           datasetpath (str): path to the directory placing the videos that need to be converted.
           pretrainedpath (str): path to the Resnet-50 i3d pretrained model.
             If the pretrained file is not existed, the file will be downloaded online and converted.
@@ -43,15 +43,19 @@
         Return:
           A set of .npy files in the outputpath.
         '''
         assert os.path.exists(datasetpath), f"Dataset path {datasetpath} does not exist. Please check."
         Path(outputpath).mkdir(parents=True, exist_ok=True)
         temppath = outputpath + "/temp/"
         rootdir = Path(datasetpath)
-        videos = [str(f) for f in rootdir.glob('**/*.avi')]
+        if multiplefiles:
+            videos = [str(f) for f in rootdir.glob('**/*.avi')]
+        else:
+            videos = [str(rootdir)]
+
 
         with torch.no_grad():
             for video in videos:
                 outfilename = Path(outputpath) / (Path(video).stem + ".npy")
                 video = Path(video).absolute()
                 video = r"{}".format(video).replace('\\', '/')
 
@@ -61,25 +65,25 @@
                     Path(temppath).mkdir(parents=True, exist_ok=True)
                     i3d_extractor = I3DFeaturesExtractor(
                         freq=frequency,
                         sample_mode=sample_mode,
                         batch_size=batch_size,
                         pretrainedpath=pretrainedpath
                     )
-                    features = i3d_extractor.run(video_path=video, frames_dir=temppath)
+                    features = i3d_extractor.run(video_path=video, frames_dir=temppath, sample_mode=sample_mode)
 
                     # Save features
                     np.save(outfilename, features)
                     print("Obtained features of size: ", features.shape)
                     shutil.rmtree(temppath)
                 print("done in {0}.".format(time.time() - startime))
 
-# if __name__ == '__main__':
-# 	parser = argparse.ArgumentParser()
-# 	parser.add_argument('--datasetpath', type=str, default="samplevideos/")
-# 	parser.add_argument('--outputpath', type=str, default="output")
-# 	parser.add_argument('--pretrainedpath', type=str, default="pretrained/i3d_r50_kinetics.pth")
-# 	parser.add_argument('--frequency', type=int, default=16)
-# 	parser.add_argument('--batch_size', type=int, default=20)
-# 	parser.add_argument('--sample_mode', type=str, default="oversample", help='center_crop or oversample')
-# 	args = parser.parse_args()
-# 	FeatureExtraction.generate(str(args.outputpath), args.datasetpath, args.pretrainedpath, args.frequency, args.batch_size, args.sample_mode)
+if __name__ == '__main__':
+	parser = argparse.ArgumentParser()
+	parser.add_argument('--datasetpath', type=str, default="samplevideos/")
+	parser.add_argument('--outputpath', type=str, default="output")
+	parser.add_argument('--pretrainedpath', type=str, default="pretrained/i3d_r50_kinetics.pth")
+	parser.add_argument('--frequency', type=int, default=16)
+	parser.add_argument('--batch_size', type=int, default=20)
+	parser.add_argument('--sample_mode', type=str, default="oversample", help='center_crop or oversample')
+	args = parser.parse_args()
+	FeatureExtraction.generate(args.datasetpath, str(args.outputpath), args.pretrainedpath, args.frequency, args.batch_size, args.sample_mode)
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/extract_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,79 @@
-import os
+import os, cv2
 import numpy as np
 import torch
 from natsort import natsorted
 from PIL import Image
-from .models.resnet import i3_res50
+from models.resnet import i3_res50
 from torch.autograd import Variable
 import ffmpeg
-from .utils.pretrained_existed import get_pth_weight
+from utils.pretrained_existed import get_pth_weight
 
 
+def extract_frames(video_path, temppath, width=640, height=480):
+    if not os.path.exists(temppath):
+        os.makedirs(temppath)
+
+    # Open the video file
+    cap = cv2.VideoCapture(video_path)
+    # Initialize the frame counter
+    frame_count = 0
+    # Loop over all frames
+    while cap.isOpened():
+        # Read a new frame
+        ret, frame = cap.read()
+
+        # If the frame was not successfully read, break the loop
+        if not ret:
+            break
+
+        # Resize the frame to desired width and height
+        frame = cv2.resize(frame, (width, height))
+
+        # Save the frame as image
+        filename = os.path.join(temppath, f"{frame_count:06d}.jpg")
+        cv2.imwrite(filename, frame)
+
+        # Increment the frame counter
+        frame_count += 1
+
+    # Release the video capture object
+    print("Frames extraction completed!")
+    cap.release()
+
 class I3DFeaturesExtractor:
     def __init__(self, freq=16, sample_mode='oversample',
                  batch_size=20, 
                  pretrainedpath = "pretrained/i3d_r50_kinetics.pth"):
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.frequency = freq  # default value, can be adjusted
         self.batch_size = batch_size  # default value, can be adjusted
         self.pretrainedpath = pretrainedpath
         self.model = self._load_i3d_model()
+
+        import cv2
+
+
     
     @staticmethod
     def resize_input(video_path, size=None, temppath='temp/'):
         if not size:
             size = (256, 256)
         
         print("... video path: ", video_path)
         print("... resizing frames to size {} ...".format(size))
 
         width, height = size[0], size[1] 
 
-        return ffmpeg.input(video_path). \
-          filter('scale', width, height).\
-          output('{}%d.jpg'.format(temppath),start_number=0, format='image2', vcodec='mjpeg').\
-            global_args('-loglevel', 'quiet').run()
-
-        # return ffmpeg.input("pipe:"). \
-        #     filter('scale', width, height). \
-        #     output("pipe:", format='rawvideo',
-        #            pix_fmt='rgb24').run_async(pipe_stdin=True, pipe_stdout=True, pipe_stderr=True)
+        return extract_frames(video_path, temppath, width, height)
+        # return ffmpeg.input(video_path). \
+        #   filter('scale', width, height).\
+        #   output('{}%d.jpg'.format(temppath),start_number=0, format='image2', vcodec='mjpeg').\
+        #     global_args('-loglevel', 'quiet').run()
 
 
     def _load_i3d_model(self):
         # code to load the I3D model
         print("-"*50)
         print("... Loading i3d model ...")
         weight_file_path = get_pth_weight(os.path.dirname(self.pretrainedpath))
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/convert_weights.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/convert_weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import torch
 import re, os
 import sys, numpy
-from ..models.resnet import I3Res50
+from models.resnet import I3Res50
 
 def convert_weights(pkl_weight:str):
 	if not pkl_weight:
 		print("Error pkl weight input.")
 		return None
 	c2_weights = pkl_weight # 'pretrained/i3d_baseline_32x2_IN_pretrain_400k.pkl'
 	pth_weights_out = os.path.dirname(pkl_weight) + '/i3d_r50_kinetics.pth'
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/pretrained_existed.py` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction/utils/pretrained_existed.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,9 +61,9 @@
             weight_found = glob.glob(os.path.dirname(pkl_weight) + '/*.pth')
             weight_file_path = os.path.join(os.path.dirname(pkl_weight), weight_found[0])
             return os.path.abspath(weight_file_path)
         weight_found = glob.glob(path_to_pretrained + '/*.pth')[0]
         weight_file_path = os.path.abspath(weight_found)
         return weight_file_path
 
-if __name__=='__main__':
-      print("--",get_pth_weight())
+# if __name__=='__main__':
+#       print("--",get_pth_weight())
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/PKG-INFO` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.2.8
+Version: 0.2.9
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -35,15 +35,14 @@
 Usage
 -----
 
 Installation
 ~~~~~~~~~~~~
 
 Before installing my package, please install these pakages:
-
 \*
 `Opencv-Python==4.5.5 <https://www.lfd.uci.edu/~gohlke/pythonlibs/#opencv>`__
 
 \*
 `torch==1.10.1+cu113 <https://download.pytorch.org/whl/cu113/torch-1.10.1%2Bcu113-cp38-cp38-win_amd64.whl>`__
 
 \*
@@ -61,55 +60,65 @@
 .. code:: commandline
 
    pip install torchvision-0.11.2+cu113-cp38-cp38-win_amd64.whl
    pip install torchaudio-0.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install torch-1.10.1+cu113-cp38-cp38-win_amd64.whl
    pip install opencv_python-4.5.5-cp38-cp38-win_amd64.whl
 
-
 After 4 above packages, to install ``i3dFeatureExtraction`` package into
 your Python environment, run this code on your terminal:
 
 .. code:: commandline
 
    pip install i3dFeatureExtraction
 
-Or install a specific version:
-
-.. code:: commandline
-
-   pip install i3dFeatureExtraction==x.x.x
 
 Implementing
 ~~~~~~~~~~~~
 
 The main function of this package is ``FeatureExtraction`` which
 converts a directory of videos into numpy feature files.
 
 .. code:: python
 
    from i3dFeatureExtraction import FeatureExtraction
    FeatureExtraction.generate(
-       outputpath = "directory/to/store/output/numpy/files",
        datasetpath="directory/of/input/videos",
+       outputpath = "directory/to/store/output/numpy/files",
        pretrainedpath = "path/to/i3D/pretrained/weight",
        sample_mode = "oversample/center_crop"
+       multiplefiles = True/False
    )
 
+-  **datasetpath** (REQUIRED): path to videos.
+-  If **multiplefiles** is *True* (default), the **datasetpath** is the
+   path to a directory which contains 1 or more videos.
+-  If **multiplefiles** is *False*, the **datasetpath** is the path to a
+   video.
+-  **outputpath** (optional, default: *“output/”*): the proccessed numpy
+   feature files would be stored in this directory.
+-  **pretrainedpath** (optional, default: *“pretrained/”*): the path of
+   the pretrained i3d weight. If the weight is not existed, it will be
+   downloaded and created manually.
+-  **sample_mode** (optional, default: *“oversample/”*) receive
+   “oversample” or “center_crop”. If *oversample*, each frame will be
+   cropped and flipped to be turned into 10 frames.
+
+
 --------------
-Structure
---------------
+
+Structure of this package
+--------------------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
-   :alt: i3dFeatureExtraction - UML Diagram
+![i3dFeatureExtraction - UML Diagram](https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png)
 
 Credits
------------
+-------
 
 This code is based on the following repositories:
 
 \*
 `pytorch-resnet3d <https://github.com/Tushar-N/pytorch-resnet3d>`__
 
 \*
@@ -118,8 +127,8 @@
 \*
 `E2E-Action-Segmentation/feature_extraction/ <https://github.com/nguyenphwork/E2E-Action-Segmentation/tree/main/feature_extraction>`__
 
 I would like to extend a special thank-you to the original authors of
 these repositories for providing the foundation on which this
 implementation is built.
 
-
+.. |i3dFeatureExtraction - UML Diagram| image:: UML/i3dExtract.png
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.2.9/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 certifi==2022.12.7
 charset-normalizer==2.1.1
 click==8.1.3
 colorama==0.4.6
 contourpy==1.0.7
 cycler==0.11.0
 einops==0.6.0
+ffmpeg==1.4
 ffmpeg-python==0.2.0
 Flask==2.2.2
 Flask-SQLAlchemy==2.5.1
 fonttools==4.39.3
 future==0.18.3
 greenlet==2.0.2
 idna==3.4
```

### Comparing `i3dFeatureExtraction-0.2.8/setup.py` & `i3dFeatureExtraction-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 DESCRIPTION = "This package helps extract i3D features with ResNet-50 backbone given a folder of videos"
 REQUIREMENTS = [i for i in open("requirements.txt").readlines()]
 setuptools.setup(
     name="i3dFeatureExtraction",
-    version="0.2.8",
+    version="0.2.9",
     author="Hao Vy Phan",
     author_email="vyhao03@gmail.com",
     description=DESCRIPTION,
-    long_description = open('README.rst').read(),
+    long_description = open('README.rst', encoding='utf-8').read(),
     long_description_content_type='text/x-rst',
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: Freely Distributable",
         "Operating System :: Microsoft :: Windows"
```

