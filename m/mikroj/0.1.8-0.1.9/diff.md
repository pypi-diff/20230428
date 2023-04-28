# Comparing `tmp/mikroj-0.1.8.tar.gz` & `tmp/mikroj-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikroj-0.1.8.tar", max compression
+gzip compressed data, was "mikroj-0.1.9.tar", max compression
```

## Comparing `mikroj-0.1.8.tar` & `mikroj-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,29 @@
--rw-r--r--   0        0        0        0 2021-09-22 12:00:55.199463 mikroj-0.1.8/mikroj/__init__.py
--rw-r--r--   0        0        0      711 2021-09-22 12:07:00.158609 mikroj-0.1.8/mikroj/helper.py
--rw-r--r--   0        0        0        0 2021-09-22 12:02:36.459207 mikroj-0.1.8/mikroj/implementations/__init__.py
--rw-r--r--   0        0        0     4732 2021-09-22 12:07:37.490531 mikroj-0.1.8/mikroj/implementations/temp_color_code.py
--rw-r--r--   0        0        0        0 2021-09-22 12:02:36.475207 mikroj-0.1.8/mikroj/macros/__init__.py
--rw-r--r--   0        0        0      930 2021-09-22 12:07:56.930491 mikroj-0.1.8/mikroj/macros/base.py
--rw-r--r--   0        0        0      265 2021-09-22 12:07:56.930491 mikroj-0.1.8/mikroj/macros/filter.py
--rw-r--r--   0        0        0      930 2021-09-22 12:07:56.930491 mikroj-0.1.8/mikroj/macros/image_acting.py
--rw-r--r--   0        0        0        0 2021-09-22 12:02:36.487207 mikroj-0.1.8/mikroj/registries/__init__.py
--rw-r--r--   0        0        0     1095 2021-09-22 12:02:36.491207 mikroj-0.1.8/mikroj/registries/helper.py
--rw-r--r--   0        0        0     1862 2021-09-28 12:27:24.102189 mikroj-0.1.8/mikroj/run.py
--rw-r--r--   0        0        0      547 2021-09-29 08:59:35.416962 mikroj-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      853 2021-09-29 08:59:35.878220 mikroj-0.1.8/setup.py
--rw-r--r--   0        0        0      563 2021-09-29 08:59:35.878384 mikroj-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-09-22 12:00:55.199463 mikroj-0.1.9/mikroj/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-12 13:38:23.702032 mikroj-0.1.9/mikroj/actors/__init__.py
+-rw-r--r--   0        0        0     1284 2021-10-12 14:12:04.343370 mikroj-0.1.9/mikroj/actors/base.py
+-rw-r--r--   0        0        0     1093 2021-10-12 13:41:57.125735 mikroj-0.1.9/mikroj/actors/stack.py
+-rw-r--r--   0        0        0      818 2021-10-12 14:40:01.869523 mikroj-0.1.9/mikroj/agent.py
+-rw-r--r--   0        0        0      146 2021-10-13 12:21:40.654855 mikroj-0.1.9/mikroj/env.py
+-rw-r--r--   0        0        0      997 2021-10-06 07:34:51.528776 mikroj-0.1.9/mikroj/helper.py
+-rw-r--r--   0        0        0     4812 2021-10-13 12:57:08.596000 mikroj-0.1.9/mikroj/main.py
+-rw-r--r--   0        0        0        0 2021-10-12 07:25:10.514296 mikroj-0.1.9/mikroj/parsers/__init__.py
+-rw-r--r--   0        0        0      988 2021-10-12 12:57:32.834332 mikroj-0.1.9/mikroj/parsers/base.py
+-rw-r--r--   0        0        0        0 2021-10-12 12:50:24.307330 mikroj-0.1.9/mikroj/parsers/code/__init__.py
+-rw-r--r--   0        0        0      317 2021-10-12 12:57:16.118380 mikroj-0.1.9/mikroj/parsers/code/base.py
+-rw-r--r--   0        0        0      496 2021-10-12 13:00:13.553903 mikroj-0.1.9/mikroj/parsers/code/groovy.py
+-rw-r--r--   0        0        0        0 2021-10-12 12:50:26.311328 mikroj-0.1.9/mikroj/parsers/definition/__init__.py
+-rw-r--r--   0        0        0      142 2021-10-12 13:01:29.781717 mikroj-0.1.9/mikroj/parsers/definition/base.py
+-rw-r--r--   0        0        0      677 2021-10-12 14:07:52.087642 mikroj-0.1.9/mikroj/parsers/definition/meta.py
+-rw-r--r--   0        0        0      596 2021-10-13 07:31:50.522470 mikroj-0.1.9/mikroj/parsers/definition/python.py
+-rw-r--r--   0        0        0      571 2021-10-12 13:01:48.365673 mikroj-0.1.9/mikroj/parsers/definition/yaml.py
+-rw-r--r--   0        0        0      716 2021-10-12 14:04:34.867822 mikroj-0.1.9/mikroj/parsers/meta.py
+-rw-r--r--   0        0        0     3538 2021-10-12 14:32:17.241791 mikroj-0.1.9/mikroj/plugins/show.md
+-rw-r--r--   0        0        0     3939 2021-10-12 14:36:33.849475 mikroj-0.1.9/mikroj/plugins/time_lapse.md
+-rw-r--r--   0        0        0        0 2021-09-22 12:02:36.487207 mikroj-0.1.9/mikroj/registries/__init__.py
+-rw-r--r--   0        0        0     1144 2021-10-12 13:43:20.801616 mikroj-0.1.9/mikroj/registries/actor.py
+-rw-r--r--   0        0        0     1095 2021-09-22 12:02:36.491207 mikroj-0.1.9/mikroj/registries/helper.py
+-rw-r--r--   0        0        0     3974 2021-10-12 14:22:09.082613 mikroj-0.1.9/mikroj/registries/macro.py
+-rw-r--r--   0        0        0        0 2021-10-07 11:17:45.567896 mikroj-0.1.9/mikroj/ui/__init__.py
+-rw-r--r--   0        0        0      588 2021-10-13 13:22:14.887229 mikroj-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      954 2021-10-13 13:22:15.241823 mikroj-0.1.9/setup.py
+-rw-r--r--   0        0        0      590 2021-10-13 13:22:15.241995 mikroj-0.1.9/PKG-INFO
```

### Comparing `mikroj-0.1.8/mikroj/helper.py` & `mikroj-0.1.9/mikroj/helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from mikro.schema import Representation
 from mikroj.registries.helper import BaseImageJHelper, set_running_helper
 import dask
+import xarray as xr
 
 class ImageJHelper(BaseImageJHelper):
 
     def __init__(self, headless=False, bind=True, version="sc.fiji:fiji:2.1.0", plugins = []) -> None:
         if bind: set_running_helper(self)
         super().__init__(headless=headless, version=version, plugins= plugins)
 
 
+    def show_xarray(self, xarray: xr.DataArray):
+        if dask.is_dask_collection(xarray.data):
+            jimage = self.py.to_java(xarray.compute())
+        else:
+            jimage = self.py.to_java(xarray)
+        
+        self.ui.show(xarray.name, jimage)
+
+
+
     def displayRep(self, rep: Representation):
         image = rep.data.squeeze()
 
         if dask.is_dask_collection(image.data):
             jimage = self.py.to_java(image.compute())
         else:
             jimage = self.py.to_java(image)
```

### Comparing `mikroj-0.1.8/mikroj/registries/helper.py` & `mikroj-0.1.9/mikroj/registries/helper.py`

 * *Files identical despite different names*

### Comparing `mikroj-0.1.8/setup.py` & `mikroj-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mikroj', 'mikroj.implementations', 'mikroj.macros', 'mikroj.registries']
+['mikroj',
+ 'mikroj.actors',
+ 'mikroj.parsers',
+ 'mikroj.parsers.code',
+ 'mikroj.parsers.definition',
+ 'mikroj.registries',
+ 'mikroj.ui']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'mikroj': ['plugins/*']}
 
 install_requires = \
-['PyQt5>=5.15.4,<6.0.0',
+['Markdown>=3.3.4,<4.0.0',
+ 'PyQt5>=5.15.4,<6.0.0',
  'PyQtWebEngine>=5.15.4,<6.0.0',
- 'arkitekt>=0.1.17,<0.2.0',
- 'mikro>=0.1.13,<0.2.0',
+ 'arkitekt==0.1.38',
+ 'mikro==0.1.25',
  'pyimagej>=1.0.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['mikroj = mikroj.run:main']}
 
 setup_kwargs = {
     'name': 'mikroj',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `mikroj-0.1.8/PKG-INFO` & `mikroj-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mikroj
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: Markdown (>=3.3.4,<4.0.0)
 Requires-Dist: PyQt5 (>=5.15.4,<6.0.0)
 Requires-Dist: PyQtWebEngine (>=5.15.4,<6.0.0)
-Requires-Dist: arkitekt (>=0.1.17,<0.2.0)
-Requires-Dist: mikro (>=0.1.13,<0.2.0)
+Requires-Dist: arkitekt (==0.1.38)
+Requires-Dist: mikro (==0.1.25)
 Requires-Dist: pyimagej (>=1.0.1,<2.0.0)
```

