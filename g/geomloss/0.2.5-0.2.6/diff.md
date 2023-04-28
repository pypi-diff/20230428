# Comparing `tmp/geomloss-0.2.5.tar.gz` & `tmp/geomloss-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomloss-0.2.5.tar", last modified: Tue Mar 29 16:11:52 2022, max compression
+gzip compressed data, was "geomloss-0.2.6.tar", last modified: Fri Apr 28 17:23:35 2023, max compression
```

## Comparing `geomloss-0.2.5.tar` & `geomloss-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jfeydy    (1902) lai       (1610)        0 2022-03-29 16:11:52.966733 geomloss-0.2.5/
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     1067 2020-10-29 19:29:02.000000 geomloss-0.2.5/LICENSE.txt
--rw-r--r--   0 jfeydy    (1902) lai       (1610)      940 2022-03-29 16:11:52.966733 geomloss-0.2.5/PKG-INFO
--rw-r--r--   0 jfeydy    (1902) lai       (1610)      140 2020-10-29 19:29:02.000000 geomloss-0.2.5/README.md
-drwxr-xr-x   0 jfeydy    (1902) lai       (1610)        0 2022-03-29 16:11:52.966733 geomloss-0.2.5/geomloss/
--rw-r--r--   0 jfeydy    (1902) lai       (1610)      244 2022-03-29 10:16:06.000000 geomloss-0.2.5/geomloss/__init__.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     8228 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/kernel_samples.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)    19849 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/samples_loss.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)    28449 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/sinkhorn_divergence.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     6833 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/sinkhorn_images.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)    22666 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/sinkhorn_samples.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     8209 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/utils.py
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     3713 2022-03-29 10:09:32.000000 geomloss-0.2.5/geomloss/wasserstein_barycenter_images.py
-drwxr-xr-x   0 jfeydy    (1902) lai       (1610)        0 2022-03-29 16:11:52.966733 geomloss-0.2.5/geomloss.egg-info/
--rw-r--r--   0 jfeydy    (1902) lai       (1610)      940 2022-03-29 16:11:52.000000 geomloss-0.2.5/geomloss.egg-info/PKG-INFO
--rw-r--r--   0 jfeydy    (1902) lai       (1610)      411 2022-03-29 16:11:52.000000 geomloss-0.2.5/geomloss.egg-info/SOURCES.txt
--rw-r--r--   0 jfeydy    (1902) lai       (1610)        1 2022-03-29 16:11:52.000000 geomloss-0.2.5/geomloss.egg-info/dependency_links.txt
--rw-r--r--   0 jfeydy    (1902) lai       (1610)       22 2022-03-29 16:11:52.000000 geomloss-0.2.5/geomloss.egg-info/requires.txt
--rw-r--r--   0 jfeydy    (1902) lai       (1610)        9 2022-03-29 16:11:52.000000 geomloss-0.2.5/geomloss.egg-info/top_level.txt
--rw-r--r--   0 jfeydy    (1902) lai       (1610)       38 2022-03-29 16:11:52.966733 geomloss-0.2.5/setup.cfg
--rw-r--r--   0 jfeydy    (1902) lai       (1610)     1419 2022-03-29 10:15:32.000000 geomloss-0.2.5/setup.py
+drwxr-xr-x   0 jfeydy   (668235) heka     (201783)        0 2023-04-28 17:23:35.876101 geomloss-0.2.6/
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     1067 2022-09-21 09:55:10.000000 geomloss-0.2.6/LICENSE.txt
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)      913 2023-04-28 17:23:35.876101 geomloss-0.2.6/PKG-INFO
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)      140 2022-09-21 09:55:10.000000 geomloss-0.2.6/README.md
+drwxr-xr-x   0 jfeydy   (668235) heka     (201783)        0 2023-04-28 17:23:35.876101 geomloss-0.2.6/geomloss/
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)      258 2023-04-28 14:59:29.000000 geomloss-0.2.6/geomloss/__init__.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)       22 2023-04-28 14:59:29.000000 geomloss-0.2.6/geomloss/__version__.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     8228 2022-09-21 09:55:10.000000 geomloss-0.2.6/geomloss/kernel_samples.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)    19849 2023-04-28 14:59:26.000000 geomloss-0.2.6/geomloss/samples_loss.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)    28449 2023-04-28 14:59:26.000000 geomloss-0.2.6/geomloss/sinkhorn_divergence.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     6833 2023-04-28 14:59:26.000000 geomloss-0.2.6/geomloss/sinkhorn_images.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)    22666 2023-04-28 14:59:26.000000 geomloss-0.2.6/geomloss/sinkhorn_samples.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     8209 2022-09-21 09:55:10.000000 geomloss-0.2.6/geomloss/utils.py
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     3713 2023-04-28 14:59:26.000000 geomloss-0.2.6/geomloss/wasserstein_barycenter_images.py
+drwxr-xr-x   0 jfeydy   (668235) heka     (201783)        0 2023-04-28 17:23:35.876101 geomloss-0.2.6/geomloss.egg-info/
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)      913 2023-04-28 17:23:35.000000 geomloss-0.2.6/geomloss.egg-info/PKG-INFO
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)      435 2023-04-28 17:23:35.000000 geomloss-0.2.6/geomloss.egg-info/SOURCES.txt
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)        1 2023-04-28 17:23:35.000000 geomloss-0.2.6/geomloss.egg-info/dependency_links.txt
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)       28 2023-04-28 17:23:35.000000 geomloss-0.2.6/geomloss.egg-info/requires.txt
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)        9 2023-04-28 17:23:35.000000 geomloss-0.2.6/geomloss.egg-info/top_level.txt
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)       38 2023-04-28 17:23:35.876101 geomloss-0.2.6/setup.cfg
+-rw-r--r--   0 jfeydy   (668235) heka     (201783)     1534 2023-04-28 14:59:29.000000 geomloss-0.2.6/setup.py
```

### Comparing `geomloss-0.2.5/LICENSE.txt` & `geomloss-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/PKG-INFO` & `geomloss-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: geomloss
-Version: 0.2.5
+Version: 0.2.6
 Summary: Geometric loss functions between point clouds, images and volumes.
-Home-page: UNKNOWN
+Home-page: 
 Author: Jean Feydy
 Author-email: jean.feydy@inria.fr
 License: LICENSE.txt
 Keywords: kernels optimal transport measure loss geometry
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -20,9 +19,7 @@
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE.txt
 
 # Geometric loss functions between point clouds, images and volumes
 
 Please check our [website](https://www.kernel-operations.io/geomloss)!
-
-
```

### Comparing `geomloss-0.2.5/geomloss/kernel_samples.py` & `geomloss-0.2.6/geomloss/kernel_samples.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/samples_loss.py` & `geomloss-0.2.6/geomloss/samples_loss.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/sinkhorn_divergence.py` & `geomloss-0.2.6/geomloss/sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/sinkhorn_images.py` & `geomloss-0.2.6/geomloss/sinkhorn_images.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/sinkhorn_samples.py` & `geomloss-0.2.6/geomloss/sinkhorn_samples.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/utils.py` & `geomloss-0.2.6/geomloss/utils.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss/wasserstein_barycenter_images.py` & `geomloss-0.2.6/geomloss/wasserstein_barycenter_images.py`

 * *Files identical despite different names*

### Comparing `geomloss-0.2.5/geomloss.egg-info/PKG-INFO` & `geomloss-0.2.6/geomloss.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: geomloss
-Version: 0.2.5
+Version: 0.2.6
 Summary: Geometric loss functions between point clouds, images and volumes.
-Home-page: UNKNOWN
+Home-page: 
 Author: Jean Feydy
 Author-email: jean.feydy@inria.fr
 License: LICENSE.txt
 Keywords: kernels optimal transport measure loss geometry
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -20,9 +19,7 @@
 Description-Content-Type: text/markdown
 Provides-Extra: full
 License-File: LICENSE.txt
 
 # Geometric loss functions between point clouds, images and volumes
 
 Please check our [website](https://www.kernel-operations.io/geomloss)!
-
-
```

### Comparing `geomloss-0.2.5/setup.py` & `geomloss-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
+# Get the current version
+version = {}
+with open("geomloss/__version__.py") as fp:
+    exec(fp.read(), version)
+
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-import geomloss
-
 setup(
     name="geomloss",
-    version=geomloss.__version__,
+    version=version["__version__"],
     description="Geometric loss functions between point clouds, images and volumes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jean Feydy",
     author_email="jean.feydy@inria.fr",
     python_requires=">=3",
     classifiers=[
@@ -36,14 +39,15 @@
     packages=["geomloss"],
     package_data={"geomloss": []},
     scripts=[],
     url="",
     license="LICENSE.txt",
     install_requires=[
         "numpy",
+        "torch",
     ],
     extras_require={
         "full": [
             "pykeops",
         ],
     },
 )
```

