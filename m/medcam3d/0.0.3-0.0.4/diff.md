# Comparing `tmp/medcam3d-0.0.3.tar.gz` & `tmp/medcam3d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medcam3d-0.0.3.tar", last modified: Wed Apr 26 17:36:57 2023, max compression
+gzip compressed data, was "medcam3d-0.0.4.tar", last modified: Fri Apr 28 11:36:36 2023, max compression
```

## Comparing `medcam3d-0.0.3.tar` & `medcam3d-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1072 2023-04-23 14:18:38.000000 medcam3d-0.0.3/LICENSE
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-26 17:36:57.000000 medcam3d-0.0.3/PKG-INFO
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     3607 2023-04-26 17:34:19.000000 medcam3d-0.0.3/README.md
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       39 2023-04-23 21:52:28.000000 medcam3d-0.0.3/medcam3d/__init__.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     1932 2023-04-24 16:43:09.000000 medcam3d-0.0.3/medcam3d/activations_and_gradients.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)    12375 2023-04-26 16:52:13.000000 medcam3d-0.0.3/medcam3d/base_medcam3d.py
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      927 2023-04-26 16:18:10.000000 medcam3d-0.0.3/medcam3d/grad_cam3d.py
-drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d.egg-info/
--rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/PKG-INFO
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      293 2023-04-26 17:36:57.000000 medcam3d-0.0.3/medcam3d.egg-info/SOURCES.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)        1 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/dependency_links.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       94 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/requires.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)        9 2023-04-26 17:36:56.000000 medcam3d-0.0.3/medcam3d.egg-info/top_level.txt
--rw-r--r--   0 jjia      (1592) afd_b     (1487)       38 2023-04-26 17:36:57.000000 medcam3d-0.0.3/setup.cfg
--rw-r--r--   0 jjia      (1592) afd_b     (1487)      914 2023-04-26 17:36:01.000000 medcam3d-0.0.3/setup.py
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-28 11:36:36.000000 medcam3d-0.0.4/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     1072 2023-04-23 14:18:38.000000 medcam3d-0.0.4/LICENSE
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-28 11:36:36.000000 medcam3d-0.0.4/PKG-INFO
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     3607 2023-04-26 17:34:19.000000 medcam3d-0.0.4/README.md
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       39 2023-04-23 21:52:28.000000 medcam3d-0.0.4/medcam3d/__init__.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     1932 2023-04-24 16:43:09.000000 medcam3d-0.0.4/medcam3d/activations_and_gradients.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)    12375 2023-04-28 11:34:44.000000 medcam3d-0.0.4/medcam3d/base_medcam3d.py
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      927 2023-04-26 16:18:10.000000 medcam3d-0.0.4/medcam3d/grad_cam3d.py
+drwxr-xr-x   0 jjia      (1592) afd_b     (1487)        0 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)     4117 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/PKG-INFO
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      293 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/SOURCES.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)        1 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/dependency_links.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       94 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/requires.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)        9 2023-04-28 11:36:36.000000 medcam3d-0.0.4/medcam3d.egg-info/top_level.txt
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)       38 2023-04-28 11:36:36.000000 medcam3d-0.0.4/setup.cfg
+-rw-r--r--   0 jjia      (1592) afd_b     (1487)      914 2023-04-28 11:36:15.000000 medcam3d-0.0.4/setup.py
```

### Comparing `medcam3d-0.0.3/LICENSE` & `medcam3d-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.3/PKG-INFO` & `medcam3d-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medcam3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: CAM for 3D medical image networks
 Home-page: https://github.com/Jingnan-Jia/medcam3d
 Author: Jingnan Jia
 Author-email: jiajingnan2222@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jingnan-Jia/medcam3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medcam3d-0.0.3/README.md` & `medcam3d-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.3/medcam3d/activations_and_gradients.py` & `medcam3d-0.0.4/medcam3d/activations_and_gradients.py`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.3/medcam3d/base_medcam3d.py` & `medcam3d-0.0.4/medcam3d/base_medcam3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         cam_per_layer: list = self.compute_cam_per_layer(input_tensor,
                                                    targets,
                                                    eigen_smooth)
         return self.aggregate_multi_layers(cam_per_layer)
 
     def get_target_length_width_height(self,
                                 input_tensor: torch.Tensor) -> Tuple[int, int]:
-        length, width, height = input_tensor.size(-1), input_tensor.size(-2), input_tensor.size(-3)
+        length, width, height = input_tensor.size(-3), input_tensor.size(-2), input_tensor.size(-1)
         return length, width, height
 
     def compute_cam_per_layer(
             self,
             input_tensor: torch.Tensor,
             targets: List[torch.nn.Module],
             eigen_smooth: bool) -> list:
```

### Comparing `medcam3d-0.0.3/medcam3d/grad_cam3d.py` & `medcam3d-0.0.4/medcam3d/grad_cam3d.py`

 * *Files identical despite different names*

### Comparing `medcam3d-0.0.3/medcam3d.egg-info/PKG-INFO` & `medcam3d-0.0.4/medcam3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medcam3d
-Version: 0.0.3
+Version: 0.0.4
 Summary: CAM for 3D medical image networks
 Home-page: https://github.com/Jingnan-Jia/medcam3d
 Author: Jingnan Jia
 Author-email: jiajingnan2222@gmail.com
 Project-URL: Bug Tracker, https://github.com/Jingnan-Jia/medcam3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medcam3d-0.0.3/setup.py` & `medcam3d-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name='medcam3d',
-    version='0.0.3',
+    version='0.0.4',
     author='Jingnan Jia',
     author_email='jiajingnan2222@gmail.com',
     description='CAM for 3D medical image networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Jingnan-Jia/medcam3d',
     project_urls={
```

