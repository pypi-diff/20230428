# Comparing `tmp/brucelee-1.0.2.tar.gz` & `tmp/brucelee-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brucelee-1.0.2.tar", last modified: Thu Apr 27 07:15:26 2023, max compression
+gzip compressed data, was "brucelee-1.0.3.tar", last modified: Fri Apr 28 08:31:14 2023, max compression
```

## Comparing `brucelee-1.0.2.tar` & `brucelee-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.851922 brucelee-1.0.2/
--rw-rw-rw-   0        0        0       41 2023-04-26 10:26:22.000000 brucelee-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6930 2023-04-27 07:15:26.850925 brucelee-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6145 2023-04-27 07:15:26.000000 brucelee-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.806045 brucelee-1.0.2/brucelee/
--rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 brucelee-1.0.2/brucelee/__init__.py
--rw-rw-rw-   0        0        0      926 2023-04-26 08:44:44.000000 brucelee-1.0.2/brucelee/_loader.py
--rw-rw-rw-   0        0        0     2098 2023-04-26 07:57:34.000000 brucelee-1.0.2/brucelee/_utils.py
--rw-rw-rw-   0        0        0    10334 2023-04-23 10:09:38.000000 brucelee-1.0.2/brucelee/auth.py
--rw-rw-rw-   0        0        0    10919 2023-04-26 08:29:10.000000 brucelee-1.0.2/brucelee/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 brucelee-1.0.2/brucelee/cbv.py
--rw-rw-rw-   0        0        0     5273 2023-04-27 07:09:11.000000 brucelee-1.0.2/brucelee/config.py
--rw-rw-rw-   0        0        0     4201 2023-04-23 15:52:12.000000 brucelee-1.0.2/brucelee/controller.py
--rw-rw-rw-   0        0        0    12683 2023-04-23 11:33:03.000000 brucelee-1.0.2/brucelee/controller_utils.py
--rw-rw-rw-   0        0        0    12634 2023-04-25 05:16:51.000000 brucelee-1.0.2/brucelee/core.py
--rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 brucelee-1.0.2/brucelee/database.py
--rw-rw-rw-   0        0        0     6516 2023-04-26 08:48:08.000000 brucelee-1.0.2/brucelee/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 brucelee-1.0.2/brucelee/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 brucelee-1.0.2/brucelee/midware_session.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.821004 brucelee-1.0.2/brucelee/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 brucelee-1.0.2/brucelee/scripts/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-04-27 07:10:31.000000 brucelee-1.0.2/brucelee/scripts/_app.py
--rw-rw-rw-   0        0        0     2041 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/_project.py
--rw-rw-rw-   0        0        0      601 2023-04-27 07:11:40.000000 brucelee-1.0.2/brucelee/scripts/_run.py
--rw-rw-rw-   0        0        0     1481 2023-04-27 07:02:02.000000 brucelee-1.0.2/brucelee/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.777122 brucelee-1.0.2/brucelee/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.831974 brucelee-1.0.2/brucelee/scripts/tpls/app/
--rw-rw-rw-   0        0        0     1637 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 brucelee-1.0.2/brucelee/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.833970 brucelee-1.0.2/brucelee/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.834968 brucelee-1.0.2/brucelee/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.844941 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      146 2023-04-26 10:26:22.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.849928 brucelee-1.0.2/brucelee/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_500.html
--rw-rw-rw-   0        0        0     1645 2023-04-24 14:18:26.000000 brucelee-1.0.2/brucelee/view.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:15:26.816021 brucelee-1.0.2/brucelee.egg-info/
--rw-rw-rw-   0        0        0     6930 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      767 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 07:15:26.000000 brucelee-1.0.2/brucelee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 07:15:26.851922 brucelee-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2935 2023-04-27 07:14:58.000000 brucelee-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.726941 brucelee-1.0.3/
+-rw-rw-rw-   0        0        0       41 2023-04-26 10:26:22.000000 brucelee-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6930 2023-04-28 08:31:14.725942 brucelee-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6145 2023-04-28 08:31:14.000000 brucelee-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.643818 brucelee-1.0.3/brucelee/
+-rw-rw-rw-   0        0        0      295 2023-04-24 10:22:01.000000 brucelee-1.0.3/brucelee/__init__.py
+-rw-rw-rw-   0        0        0      926 2023-04-26 08:44:44.000000 brucelee-1.0.3/brucelee/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 brucelee-1.0.3/brucelee/_utils.py
+-rw-rw-rw-   0        0        0    10334 2023-04-23 10:09:38.000000 brucelee-1.0.3/brucelee/auth.py
+-rw-rw-rw-   0        0        0    10919 2023-04-26 08:29:10.000000 brucelee-1.0.3/brucelee/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 brucelee-1.0.3/brucelee/cbv.py
+-rw-rw-rw-   0        0        0     5273 2023-04-27 07:09:11.000000 brucelee-1.0.3/brucelee/config.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 brucelee-1.0.3/brucelee/controller.py
+-rw-rw-rw-   0        0        0    12619 2023-04-27 14:24:00.000000 brucelee-1.0.3/brucelee/controller_utils.py
+-rw-rw-rw-   0        0        0    13375 2023-04-27 14:25:22.000000 brucelee-1.0.3/brucelee/core.py
+-rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 brucelee-1.0.3/brucelee/database.py
+-rw-rw-rw-   0        0        0     6516 2023-04-26 08:48:08.000000 brucelee-1.0.3/brucelee/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 brucelee-1.0.3/brucelee/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 brucelee-1.0.3/brucelee/midware_session.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.676730 brucelee-1.0.3/brucelee/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 brucelee-1.0.3/brucelee/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8312 2023-04-28 08:30:22.000000 brucelee-1.0.3/brucelee/scripts/_app.py
+-rw-rw-rw-   0        0        0     6543 2023-04-28 08:15:07.000000 brucelee-1.0.3/brucelee/scripts/_controller.py
+-rw-rw-rw-   0        0        0     2041 2023-04-26 10:26:22.000000 brucelee-1.0.3/brucelee/scripts/_project.py
+-rw-rw-rw-   0        0        0      601 2023-04-27 07:11:40.000000 brucelee-1.0.3/brucelee/scripts/_run.py
+-rw-rw-rw-   0        0        0     1506 2023-04-28 06:21:34.000000 brucelee-1.0.3/brucelee/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.614894 brucelee-1.0.3/brucelee/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.700666 brucelee-1.0.3/brucelee/scripts/tpls/app/
+-rw-rw-rw-   0        0        0     1379 2023-04-28 08:29:29.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1263 2023-04-25 10:41:46.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       19 2023-04-28 05:57:01.000000 brucelee-1.0.3/brucelee/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.705653 brucelee-1.0.3/brucelee/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.707647 brucelee-1.0.3/brucelee/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.720615 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-04-18 14:10:48.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      342 2023-04-22 11:06:16.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      300 2023-04-03 07:47:20.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      839 2023-04-19 05:59:11.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      831 2023-04-26 09:58:29.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      146 2023-04-26 10:26:22.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.723622 brucelee-1.0.3/brucelee/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1234 2023-04-07 11:12:30.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1056 2023-04-07 11:24:23.000000 brucelee-1.0.3/brucelee/scripts/tpls/project/public/error_500.html
+-rw-rw-rw-   0        0        0     1645 2023-04-24 14:18:26.000000 brucelee-1.0.3/brucelee/view.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:31:14.650800 brucelee-1.0.3/brucelee.egg-info/
+-rw-rw-rw-   0        0        0     6930 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1625 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      767 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 08:31:14.000000 brucelee-1.0.3/brucelee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 08:31:14.726941 brucelee-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2935 2023-04-28 08:30:55.000000 brucelee-1.0.3/setup.py
```

### Comparing `brucelee-1.0.2/PKG-INFO` & `brucelee-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brucelee
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/brucelee
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brucelee-1.0.2/README.md` & `brucelee-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/_loader.py` & `brucelee-1.0.3/brucelee/_loader.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/_utils.py` & `brucelee-1.0.3/brucelee/_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import json
 from datetime import datetime, date
 from json import JSONEncoder
 import re
 import os
+snake_case_re = re.compile("(?<!^)(?=[A-Z][a-z])")
+controller_re = re.compile("([\\w]+)Controller")
+
+
+def get_controller_name(controller_name):
+    return controller_re.match(controller_name).group(1)
+
+def get_snaked_name(_name:str):
+    return snake_case_re.sub("_", _name).lower()
 def is_valid_filename(filename):
     if filename is None or len(filename) == 0:
         return False
     if len(filename) > 200:
         return False
     illegal_chars = set('/\\?%*:|"<>')
     if any(char in illegal_chars for char in filename):
```

### Comparing `brucelee-1.0.2/brucelee/auth.py` & `brucelee-1.0.3/brucelee/auth.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/base_controller.py` & `brucelee-1.0.3/brucelee/base_controller.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/cbv.py` & `brucelee-1.0.3/brucelee/cbv.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/config.py` & `brucelee-1.0.3/brucelee/config.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/controller.py` & `brucelee-1.0.3/brucelee/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     @staticmethod
     def http(path,methods=['GET'],*args,**kwargs):
         return _route_method(path,method=methods,*args,**kwargs)
     @staticmethod
     def get(path: str, *args, **kwargs): 
         """if path eq application._public_auth_url,the auth agr must set to 'none' """
-        if MvcRouter.app and path == MvcRouter.app._public_auth_url:
+        if MvcRouter.app and path == MvcRouter.app.public_auth_url:
             if 'auth' in kwargs and kwargs['auth']!='none':
                 raise RuntimeError('the public auth path must set to "none" on auth arguments') 
             elif not 'auth' in kwargs:
                  kwargs['auth'] = 'none'
         return _route_method(path, "get", *args, **kwargs)
 
     @staticmethod
```

### Comparing `brucelee-1.0.2/brucelee/controller_utils.py` & `brucelee-1.0.3/brucelee/controller_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from functools import wraps, update_wrapper
 from typing import Callable, Dict, Set, Type
 import copy
 import typing_inspect
 from fastapi import APIRouter,Request,Response,HTTPException,Form,Depends
 from .cbv import cbv
 from fastapi.openapi import  utils as fastapi_dependencies_utils
- 
+from ._utils import get_snaked_name,get_controller_name
+
 def _get_flat_params(dependant )  :
     flat_dependant =fastapi_dependencies_utils.get_flat_dependant(dependant, skip_repeats=True)
     new_params_query = []
     for _item in flat_dependant.query_params:
         if not (_item.name.startswith("__") and _item.name.endswith("__")):
             new_params_query.append(_item)
     return (
@@ -21,16 +22,16 @@
         + new_params_query
         + flat_dependant.header_params
         + flat_dependant.cookie_params
     )
 # _old_get_flat_params = fastapi_dependencies_utils.get_flat_params
 fastapi_dependencies_utils.get_flat_params = _get_flat_params 
 
-controller_re = re.compile("([\\w]+)Controller")
-snake_case_re = re.compile("(?<!^)(?=[A-Z][a-z])")
+
+
 
 TEMPLATE_PATH_KEY = "__template_path__"
 VER_KEY = "__custom_version__"
 PATH_KEY = "__custom_path__"
 METHOD_KEY = "__custom_method__"
 KWARGS_KEY = "__custom_kwargs__"
 SIGNATURE_KEY = "__saved_signature__"
@@ -44,14 +45,15 @@
     pass
 
 
 CBType = Type[ControllerBase]
 CBTypeSet = Set[CBType]
 
 
+
 def _get_leaf_controllers(controller_base: CBType) -> CBTypeSet:
     """
 
     Args:
       controller_base: Type[ControllerBase]:
 
     Returns:
@@ -81,19 +83,19 @@
       controller_name: str:
       path_template_prefix: str:
       version: str:
 
     Returns:
 
     """
-    controller_name = controller_re.match(controller_name).group(1)
-    snake_case_controller_name = snake_case_re.sub("_", controller_name)
+    controller_name = get_controller_name(controller_name)
+    snake_case_controller_name = get_snaked_name(controller_name)
 
     return f"{path_template_prefix}{route_path}" \
-        .replace("{controller}", snake_case_controller_name.lower()) \
+        .replace("{controller}", snake_case_controller_name) \
         .replace("{version}", version)
 
 
 def _get_routes_in_controller(controller: Type[ControllerBase]):
     """
 
     Args:
```

### Comparing `brucelee-1.0.2/brucelee/core.py` & `brucelee-1.0.3/brucelee/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,56 @@
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
+from ._utils import get_controller_name,get_snaked_name
 
 __is_debug=config.get('debug',False)
 
 
 class MvcApp(FastAPI):
     def __init__(self,  **kwargs):
         self._authObj:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
-        self._user_auth_url=""
-        self._public_auth_url=""
+        self.__user_auth_url=""
+        self.__public_auth_url=""
         self._app_views_dirs = {} 
         self.routers_map = {}
         super().__init__(**kwargs)
     @property
+    def public_auth_url(self):
+        """public user auth url"""
+        return self.__public_auth_url
+    @public_auth_url.setter
+    def public_auth_url(self,url):
+        if self.__public_auth_url:
+            raise RuntimeError(f"public_auth_url only can be setting once time,current is:{self.__public_auth_url}")
+        self.__public_auth_url = url
+        
+    @property
+    def user_auth_url(self):
+        """internal user auth url"""
+        return self.__user_auth_url
+    @user_auth_url.setter
+    def user_auth_url(self,url):
+        if self.__user_auth_url:
+            raise RuntimeError(f"user_auth_url only can be setting once time,current is:{self.__user_auth_url}")
+        self.__user_auth_url = url
+
+    @property
     def authObj(self)->auth.AuthenticationBackend_:
         return self._authObj
     
     @authObj.setter
     def authObj(self,value:auth.AuthenticationBackend_):
         self._authObj = value
-    pass
+     
     @property 
     def data_engine(self)->database.Engine:
         return self._data_engine
     @data_engine.setter
     def data_engine(self,value):
         self._data_engine = value
 
@@ -174,15 +195,15 @@
                         application.authObj.create_access_token(user=user, expires_delta=None,request=request)
                 #
                 if not ret and not user: 
                     _log.debug(f'Failed Auth[type:{auth_type}] url:'+str(request.url))
                     if accept_header == "application/json":
                         return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
-                    _auth_url = getattr(application,f"_{auth_type}_auth_url") if hasattr(application,f"_{auth_type}_auth_url") else None
+                    _auth_url = getattr(application,f"{auth_type}_auth_url") 
 
                     if _auth_url: 
                         if 'flash' not in request.session:
                             request.session['flash']=''
                         if request.session['flash']=="":
                             request.session['flash']  = "you are not authenticated,please login!"  
                         _auth_url = add_redirect_param(_auth_url,str(request.url))
@@ -191,15 +212,15 @@
                         return RedirectResponse('/',status_code=StateCodes.HTTP_303_SEE_OTHER),None
                 else:
                     _log.debug(f'Successed Auth[type:{auth_type}] Url:'+str(request.url)+',User:'+str(user))
                     return ret,user
 
         setattr(puppetController,AUTH_KEY,allargs['auth'])         
         setattr(puppetController,"__name__",targetController.__name__)  
-        controller_name = targetController.__name__.lower().replace("controller","")
+        controller_name = get_controller_name(targetController.__name__)
         setattr(puppetController,"__controller_name__",controller_name)  
         
         setattr(puppetController,"__version__",version)  
         setattr(puppetController,"__location__",relative_path)  
         setattr(puppetController,"__appdir__",app_dir)  
 
         setattr(puppetController,"__controler_url__",controller_name)
```

### Comparing `brucelee-1.0.2/brucelee/database.py` & `brucelee-1.0.3/brucelee/database.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/midware.py` & `brucelee-1.0.3/brucelee/midware.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/midware_casbin.py` & `brucelee-1.0.3/brucelee/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/midware_session.py` & `brucelee-1.0.3/brucelee/midware_session.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/_app.py` & `brucelee-1.0.3/brucelee/scripts/_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,164 @@
 import argparse
-import sys,os
+import sys,os,re
 from typing import Any
 from jinja2 import Template
-from brucelee._utils import is_valid_filename
-from  brucelee.config import IS_IN_BRUCELEE
+from brucelee._utils import is_valid_filename,get_controller_name,get_snaked_name
+from  brucelee.config import is_in_brucelee
 
 class Generator():
-    def __init__(self,args) -> None:
-        self.args=args
+    def __init__(self,args,dir) -> None:
+        self.args = args
+        self.dir = dir
         pass
     def gen_common(self):
         '''#todo: check configs dir
                   check data dir
 
         '''
         pass
-    def gen_tpl(self,tpl_file,dest,context={}, use_micro=True):
+    def gen_tpl(self,tpl_file,dest,context={}, use_micro=True,dir_only=False):
         tpl_dir = os.path.dirname(__file__)+"/tpls/app"
         tpl_file = os.path.join(tpl_dir,tpl_file)
+        dest = os.path.normpath(dest)
         if not os.path.exists(tpl_file):
             raise Exception(f"{tpl_file} does not exists!")
-        with open(tpl_file,'r') as f:
-            content = f.read()
-        dest_content = content
-        if use_micro:
-            template = Template(content)
-            dest_content = template.render(context)
+        if os.path.exists(dest):
+            print(f"{dest} is exists! skip..")
+            return True
         dir = os.path.dirname(dest) 
         os.makedirs(dir,exist_ok=True)
-        with open(dest,'w') as f:
-            f.write(dest_content)
+        if not dir_only:
+            with open(tpl_file,'r') as f:
+                content = f.read()
+            dest_content = content
+            if use_micro:
+                template = Template(content)
+                dest_content = template.render(context)
+            
+            
+            with open(dest,'w') as f:
+                f.write(dest_content)
+        print(f"create {dest}")
         return True
-    def add_enabled_to_app(self,app_name):
-        import yaml
-        try:
-            file = './configs/general.yaml'
- 
-            with open(file, "r") as f:
-                data = yaml.load(f, Loader=yaml.FullLoader)
- 
-            data['app']['enabled'] = data['app']['enabled'].append(app_name)
- 
-            with open(file, "w") as f:
-                yaml.dump(data, f)
-        except Exception as e:
-            print(f'an error raised {e.args}')
-            print(f"now please open configs/general.yaml to modify app.enabled to add {app_name}!")
-            return
-        print(f"configs/general.yaml app.enabled has been added {app_name}!")
+    def str_to_upper(self,name):
+        new_name = name.title().replace("_", "")
+        return new_name
+    def is_valid_class_name(self,name):
+        if not isinstance(name, str):
+            return False 
+        if not re.match(r'^[a-zA-Z_]', name):
+            return False 
+        if not re.match(r'^\w+$', name):
+            return False 
+        import keyword
+        if keyword.iskeyword(name):
+            return False 
+        return True
+    def ensure_line(self,filepath, line_to_add):
+        found = False
+        lines = []
+        if os.path.exists(filepath):
+            # Read in the file
+            with open(filepath, 'r') as file:
+                lines = file.readlines()
+
+                # Check if the line is already in the file
+                for line in lines:
+                    if line.strip() == line_to_add.strip():
+                        found = True
+                        break
+
+        # If the line is not in the file, add it
+        if not found:
+            lines.append('\n' + line_to_add.strip() + '\n')
+            with open(filepath, 'w') as file:
+                file.writelines(lines)
+
     def __call__(self) -> Any:
-        if not self.args.dir:
-            self.args.dir = input("please input dir to store app[default=apps]:")
-            if not self.args.dir:
-                self.args.dir = 'apps'
-        assert is_valid_filename(self.args.dir)
-        if not self.args.name:
-            self.args.name = input("please input app name:")
+         
         if not self.args.name:
-            print(f'app name is empty,exit!')
+            print(f'controller name is empty,exit!')
             exit()
-        assert is_valid_filename(self.args.name)    
+        for name in self.args.name:
+            if not is_valid_filename(name) :
+                print(f'{name} is not avalided!')
+                exit() 
 
-        store_dir = self.args.dir
-        app_name = self.args.name
-        store_dir = os.path.join(store_dir,app_name)
-        if os.path.exists(store_dir):
-            if os.path.isdir(store_dir):
-                if bool(os.listdir(store_dir)):
-                    print(f"directory {store_dir} is exists and is not empty!")
-                    exit()
-        
-        
-        dirs_items =  {
-            'controllers':{'tpl':'controller.tpl','dest':f'{app_name}_controller.py','micro':True} , 
-            'models': {'tpl':'model.tpl','dest' : f'{app_name}_model.py','micro':True},
-            'services':{'tpl':'service.tpl','dest': f'{app_name}_service.py','micro':True },
-            'views': [
-                {'tpl' : 'view.tpl','dest': f'{app_name}/home.html','micro':False},
-                {'tpl' : 'css.tpl','dest': f'{app_name}/home.css','micro':False}
-                ] ,
+            store_dir = self.dir
+            controller_name = name
+            controler_path_name = get_snaked_name(controller_name)
+            # store_dir = os.path.join(store_dir,controler_path_name )
             
-            'tests': {'tpl':'test.tpl','dest': f'test_{app_name}.py','micro':True}
-        }
-        context = {'app':app_name}
-        for dir in dirs_items:
-            _current_dir = os.path.join(store_dir,dir)
-            os.makedirs(_current_dir,exist_ok=True)
-            items = dirs_items[dir]
-            if isinstance(items,list):
-                _item = items
-            else:
-                _item = [items]
-            for item in _item:
-                tpl = item['tpl']
-                dest = os.path.join(_current_dir , item['dest'])
-                micro = item['micro']
-                self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro) 
-        with open(os.path.join(store_dir,'__init__.py'),'w') as f:
-            f.write(f"from .controllers import *")
-        with open(os.path.join(store_dir,'controllers','__init__.py'),'w') as f:
-            f.write(f"from . import {app_name}_controller")
-        
-        self.add_enabled_to_app(app_name)
+            # controller_name = self.str_to_upper(name)
+            if not self.is_valid_class_name(controller_name):
+                print(f"{controller_name} is a not valided class name,exit...")
+                exit() 
+            
+            dirs_items =  {
+                'controllers':{'tpl':'controller.tpl','dest':f'controllers/{controler_path_name}_controller.py','micro':True} , 
+                'models': {'tpl':'model.tpl','dest' : f'models/{controler_path_name}_model.py','micro':True},
+                'services':{'tpl':'service.tpl','dest': f'services/{controler_path_name}_service.py','micro':True },
+                'views': [
+                    {'tpl' : 'view.tpl','dest': f'views/{controler_path_name}/index.html','micro':False},
+                    {'tpl' : 'css.tpl','dest': f'views/{controler_path_name}/index.css','micro':False}
+                    ] ,
+                
+                'tests': {'tpl':'test.tpl','dest': f'tests/test_{controler_path_name}.py','micro':True}
+            }
+            context = {'ctrl_name':controller_name,'ctrl_path':controler_path_name}
+            for dir in dirs_items:
+                _current_dir = store_dir#os.path.join(store_dir,dir)
+                os.makedirs(_current_dir,exist_ok=True)
+                items = dirs_items[dir]
+                if isinstance(items,list):
+                    _item = items
+                else:
+                    _item = [items]
+                for item in _item:
+                    tpl = item['tpl']
+                    dest = os.path.join(_current_dir , item['dest'])
+                    micro = item['micro']
+                    self.gen_tpl(tpl_file=tpl,dest=dest,context=context,use_micro=micro,dir_only=False) 
+            __init_file = os.path.join(_current_dir,'controllers','__init__.py')
+            self.ensure_line(__init_file,f"from . import {controler_path_name}_controller")
+             
         
         print("Done!")
     pass
 
+def is_in_app(directory):
+    """
+    check exists configs dir, apps dir, main.py and configs/general.yaml 
+    """
+    
+    controller_dir = os.path.join(directory, 'controllers')
+    views_dir = os.path.join(directory, 'views')  
+    if not os.path.exists(controller_dir) or not os.path.exists(views_dir) :
+        return False  
+    initfile = os.path.join(controller_dir, '__init__.py') 
+    if not os.path.exists(initfile):
+        return False
+    
+    return True
 def main():
-    if not IS_IN_BRUCELEE:
-        print(f"Please exec in brucelee dir")
-        exit()
+     
+    cur_dir = os.path.abspath(os.curdir)
+    root_path = os.path.abspath(os.path.join(cur_dir,"../.."))
+    if os.path.exists(root_path) and  os.path.isdir(root_path): 
+        if not is_in_brucelee(root_path) or not is_in_app(cur_dir):
+            print(f"Please exec in brucelee project's app dir ,like `apps/app`")
+            exit()
     self_file = __file__.lstrip("_").replace(".py",'')
-    parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name NAME] [-d DIR]", description='new app')
-    parser.add_argument('--name',help="name to create app")
-    parser.add_argument('-d','--dir',help="dir to store app files")
+    parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [--name] `controller name` ...", description='create new controller')
+    parser.add_argument('--name',help="controller name to create")
+    parser.add_argument('args', nargs=argparse.REMAINDER)
+     
     args = parser.parse_args()
     if not any(args.__dict__.values()):
         parser.print_help()
-
-    _gen = Generator(args)
+    if not args.name:
+        args.name = args.args
+    else:
+        args.name = [args.name]
+    _gen = Generator(args,cur_dir)
     _gen()
```

### Comparing `brucelee-1.0.2/brucelee/scripts/_project.py` & `brucelee-1.0.3/brucelee/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/_run.py` & `brucelee-1.0.3/brucelee/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/main.py` & `brucelee-1.0.3/brucelee/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import sys
 import importlib.util
 import os.path
  
 import os
 import re
-
+ 
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
     """
     
     dir_path = os.path.dirname(os.path.abspath(__file__))  
     py_files = []
@@ -33,15 +33,15 @@
      
     args = parser.parse_args()
     
     args.feature = '_' +args.feature
     
     module_path = os.path.join(module_dir, args.feature + '.py')
 
-    
+    sys.argv[0] = 'brucelee'
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(args.feature, module_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         sys.argv.pop(1)
         module.main()
     else:
```

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/app/controller.tpl` & `brucelee-1.0.3/brucelee/scripts/tpls/app/controller.tpl`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 # -*- coding: utf-8 -*- 
 from brucelee import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect,UploadFile,File
 
 from typing import Any, Dict ,List
-from pydantic import conlist
+from pydantic import conlist 
 
-application._public_auth_url = '/{{app}}/login'
-application._user_auth_url = '/{{app}}/login'
- 
-@api_router(auth='none')
-class {{app}}Controller(BaseController): 
-    @api.get("/{{app}}/login" )
+@api_router(path='{{ctrl_path}}',auth='none')
+class {{ctrl_name}}Controller(BaseController): 
+    @api.get("/login" )
     def login(self):
         """:title Login"""  
         redirect = self.get_param('redirect') if self.get_param('redirect') else '/' 
         return self.view() 
-    @api.post("/{{app}}/verity_user",auth="none")
+    @api.post("/verity_user",auth="none")
     async def verity_user(self):  
         username = self['username']
         password = self['password']
         redirect = self['redirect']
         if username and password:
             #do veritied
             if username in ['bruce','alice'] and password:
                 return self._verity_successed(username,redirect)
             else:
                 return self._verity_error() 
         return self._verity_error()
     
-    @api.get("/{{app}}/logout")
+    @api.get("/logout")
     def logout(self):
         return self._user_logout()
     
-    @api.post("/{{app}}/upload")
+    @api.post("/upload")
     async def upload_test(self, files: List[UploadFile] = File(...) ): 
         p = {}
         for file in files:
             path,url = await self._save_upload_file(file)
             p[file.filename] = [path,url]
         return {"files":p} 
     
-    
-    @api.get("/",auth='none' )
-    def home(self,request:Request): 
-        '''
-        :title Home
-        '''
-   
-        return self.view()
-    
+
```

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/app/css.tpl` & `brucelee-1.0.3/brucelee/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/app/view.tpl` & `brucelee-1.0.3/brucelee/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/alembic.ini` & `brucelee-1.0.3/brucelee/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/database.yaml` & `brucelee-1.0.3/brucelee/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/project/configs/general.yaml` & `brucelee-1.0.3/brucelee/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_404.html` & `brucelee-1.0.3/brucelee/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/scripts/tpls/project/public/error_500.html` & `brucelee-1.0.3/brucelee/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee/view.py` & `brucelee-1.0.3/brucelee/view.py`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/brucelee.egg-info/PKG-INFO` & `brucelee-1.0.3/brucelee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brucelee
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/brucelee
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `brucelee-1.0.2/brucelee.egg-info/SOURCES.txt` & `brucelee-1.0.3/brucelee.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 brucelee.egg-info/dependency_links.txt
 brucelee.egg-info/entry_points.txt
 brucelee.egg-info/requires.txt
 brucelee.egg-info/top_level.txt
 brucelee/scripts/main.py
 brucelee/scripts/__init__.py
 brucelee/scripts/_app.py
+brucelee/scripts/_controller.py
 brucelee/scripts/_project.py
 brucelee/scripts/_run.py
 brucelee/scripts/main.py
 brucelee/scripts/tpls/app/controller.tpl
 brucelee/scripts/tpls/app/css.tpl
+brucelee/scripts/tpls/app/home.css.tpl
+brucelee/scripts/tpls/app/home.tpl
 brucelee/scripts/tpls/app/model.tpl
 brucelee/scripts/tpls/app/service.tpl
 brucelee/scripts/tpls/app/test.tpl
 brucelee/scripts/tpls/app/view.tpl
 brucelee/scripts/tpls/project/.gitignore
 brucelee/scripts/tpls/project/main.py
 brucelee/scripts/tpls/project/apps/__init__.py
```

### Comparing `brucelee-1.0.2/brucelee.egg-info/requires.txt` & `brucelee-1.0.3/brucelee.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `brucelee-1.0.2/setup.py` & `brucelee-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 import chardet
 
-version = "1.0.2"
+version = "1.0.3"
 def update_readme(source,spec,content=""):
     assert source or content
 
     if not content:
         with open(source, 'r') as file:
             content = file.read()
     with open('README.md', 'r') as file:
```

