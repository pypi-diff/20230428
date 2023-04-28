# Comparing `tmp/i3dFeatureExtraction-0.3.0.tar.gz` & `tmp/i3dFeatureExtraction-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.3.0.tar", last modified: Fri Apr 28 09:28:51 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.3.1.tar", last modified: Fri Apr 28 09:41:30 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.3.0.tar` & `i3dFeatureExtraction-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:28:51.472257 i3dFeatureExtraction-0.3.0/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4768 2023-04-28 09:28:51.471258 i3dFeatureExtraction-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3858 2023-04-28 08:54:16.000000 i3dFeatureExtraction-0.3.0/README.md
--rw-rw-rw-   0        0        0     4309 2023-04-28 09:28:24.000000 i3dFeatureExtraction-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 09:28:51.451259 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4211 2023-04-28 09:20:37.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    11168 2023-04-28 09:20:37.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/extract_features_org.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:28:51.467258 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:28:51.470257 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/__init__.py
--rw-rw-rw-   0        0        0     2716 2023-04-28 09:20:37.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/convert_weights.py
--rw-rw-rw-   0        0        0     3227 2023-04-28 07:49:05.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/pretrained_existed.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:28:51.460258 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0     4768 2023-04-28 09:28:51.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-04-28 09:28:51.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:28:51.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      689 2023-04-28 09:28:51.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-28 09:28:51.000000 i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 09:28:51.472257 i3dFeatureExtraction-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-28 09:28:24.000000 i3dFeatureExtraction-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:41:30.819178 i3dFeatureExtraction-0.3.1/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4768 2023-04-28 09:41:30.818177 i3dFeatureExtraction-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3858 2023-04-28 08:54:16.000000 i3dFeatureExtraction-0.3.1/README.md
+-rw-rw-rw-   0        0        0     4309 2023-04-28 09:28:24.000000 i3dFeatureExtraction-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 09:41:30.795199 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4211 2023-04-28 09:20:37.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    11170 2023-04-28 09:40:41.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:41:30.814176 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:41:30.817180 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/__init__.py
+-rw-rw-rw-   0        0        0     2716 2023-04-28 09:20:37.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/convert_weights.py
+-rw-rw-rw-   0        0        0     3227 2023-04-28 07:49:05.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/pretrained_existed.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:41:30.807178 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0     4768 2023-04-28 09:41:30.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-04-28 09:41:30.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:41:30.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:41:30.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-28 09:41:30.000000 i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:41:30.819178 i3dFeatureExtraction-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-28 09:41:03.000000 i3dFeatureExtraction-0.3.1/setup.py
```

### Comparing `i3dFeatureExtraction-0.3.0/LICENSE.txt` & `i3dFeatureExtraction-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/PKG-INFO` & `i3dFeatureExtraction-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
```

### Comparing `i3dFeatureExtraction-0.3.0/README.md` & `i3dFeatureExtraction-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/README.rst` & `i3dFeatureExtraction-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/__init__.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/extract_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, cv2
 import numpy as np
 import torch
 from natsort import natsorted
 from PIL import Image
-from models.resnet import i3_res50
+from ..models.resnet import i3_res50
 from torch.autograd import Variable
 # import ffmpeg
 from .utils.pretrained_existed import get_pth_weight
 
 
 def extract_frames(video_path, temppath, width=640, height=480):
     if not os.path.exists(temppath):
```

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/convert_weights.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/convert_weights.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction/utils/pretrained_existed.py` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction/utils/pretrained_existed.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/PKG-INFO` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.3.0
+Version: 0.3.1
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
```

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.3.0/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.3.1/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files identical despite different names*

