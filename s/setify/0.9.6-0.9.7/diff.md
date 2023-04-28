# Comparing `tmp/setify-0.9.6.tar.gz` & `tmp/setify-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setify-0.9.6.tar", last modified: Wed Nov 16 20:13:14 2022, max compression
+gzip compressed data, was "setify-0.9.7.tar", last modified: Fri Apr 28 17:03:03 2023, max compression
```

## Comparing `setify-0.9.6.tar` & `setify-0.9.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2022-11-16 20:13:14.257316 setify-0.9.6/
--rw-r--r--   0 mina       (501) staff       (20)      933 2022-11-16 20:13:14.257487 setify-0.9.6/PKG-INFO
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2022-11-16 20:13:14.257267 setify-0.9.6/setify/
--rw-r--r--   0 mina       (501) staff       (20)       66 2022-11-16 20:12:46.859077 setify-0.9.6/setify/__init__.py
--rw-r--r--   0 mina       (501) staff       (20)     3586 2022-11-16 19:57:00.090915 setify-0.9.6/setify/datasets.py
--rw-r--r--   0 mina       (501) staff       (20)     3334 2022-11-16 18:07:25.365047 setify-0.9.6/setify/utils.py
--rw-r--r--   0 mina       (501) staff       (20)       61 2022-11-16 18:07:25.365130 setify-0.9.6/setup.cfg
--rw-r--r--   0 mina       (501) staff       (20)     1244 2022-11-16 20:12:56.625043 setify-0.9.6/setup.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2023-04-28 17:03:03.631495 setify-0.9.7/
+-rw-r--r--   0 mina       (501) staff       (20)      933 2023-04-28 17:03:03.631605 setify-0.9.7/PKG-INFO
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2023-04-28 17:03:03.631445 setify-0.9.7/setify/
+-rw-r--r--   0 mina       (501) staff       (20)       66 2023-04-28 17:00:49.030141 setify-0.9.7/setify/__init__.py
+-rw-r--r--   0 mina       (501) staff       (20)     3628 2023-04-28 16:54:07.590625 setify-0.9.7/setify/datasets.py
+-rw-r--r--   0 mina       (501) staff       (20)     3334 2023-04-28 16:53:21.208739 setify-0.9.7/setify/utils.py
+-rw-r--r--   0 mina       (501) staff       (20)       61 2023-04-28 16:53:21.208820 setify-0.9.7/setup.cfg
+-rw-r--r--   0 mina       (501) staff       (20)     1244 2023-04-28 17:02:07.190902 setify-0.9.7/setup.py
```

### Comparing `setify-0.9.6/PKG-INFO` & `setify-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: setify
-Version: 0.9.6
+Version: 0.9.7
 Summary: Dataset packages
 Home-page: https://github.com/MinaGabriel/setify.git
 Author: Mina Gabriel
 Author-email: developer.mina@gmail.com
 License: MIT
-Download-URL: https://github.com/MinaGabriel/setify/archive/refs/tags/v0.9.6.tar.gz
+Download-URL: https://github.com/MinaGabriel/setify/archive/refs/tags/v0.9.7.tar.gz
 Description: Setify is an open-source dataset package manager written in Python and designed to enable fast experimentation for Machine Learning, Setify allows you to reach hundreds of datasets with one command.
 Keywords: Dataset,Data
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `setify-0.9.6/setify/datasets.py` & `setify-0.9.7/setify/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import urllib.request
 import pandas as pd
 from setify import utils
 
 
 
 def _get_server():
-    return 'https://setify-server.herokuapp.com'
+    #return 'https://setify-server.herokuapp.com'
+    return 'http://159.223.176.152:5000'
 
 
 def hazardous_materials():
     fpath = utils.load_data(
         _get_server() + "/hazardous_materials", 'hazardous_materials.h5')
     return pd.read_hdf(fpath)
```

### Comparing `setify-0.9.6/setify/utils.py` & `setify-0.9.7/setify/utils.py`

 * *Files identical despite different names*

### Comparing `setify-0.9.6/setup.py` & `setify-0.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
     name='setify',
     packages=['setify'],
-    version='0.9.6',
+    version='0.9.7',
     license='MIT',
     description='Dataset packages',
     author='Mina Gabriel',
     author_email='developer.mina@gmail.com',
     url='https://github.com/MinaGabriel/setify.git',
-    download_url='https://github.com/MinaGabriel/setify/archive/refs/tags/v0.9.6.tar.gz',
+    download_url='https://github.com/MinaGabriel/setify/archive/refs/tags/v0.9.7.tar.gz',
     keywords=['Dataset', 'Data'],
     install_requires=[
         'pandas',
         'numpy',
         'tqdm',
         'colorama',
         'tables'
```

