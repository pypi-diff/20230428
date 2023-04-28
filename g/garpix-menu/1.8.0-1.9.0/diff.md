# Comparing `tmp/garpix_menu-1.8.0.tar.gz` & `tmp/garpix_menu-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_menu-1.8.0.tar", last modified: Fri Apr 22 07:50:42 2022, max compression
+gzip compressed data, was "garpix_menu-1.9.0.tar", last modified: Wed Jun 29 08:25:32 2022, max compression
```

## Comparing `garpix_menu-1.8.0.tar` & `garpix_menu-1.9.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.021542 garpix_menu-1.8.0/
--rw-r--r--   0 crusat     (501) staff       (20)       73 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     5932 2022-04-22 07:50:42.021402 garpix_menu-1.8.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.018442 garpix_menu-1.8.0/garpix_menu/
--rw-r--r--   0 crusat     (501) staff       (20)       73 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     5305 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/README.rst
--rw-r--r--   0 crusat     (501) staff       (20)       57 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.019549 garpix_menu-1.8.0/garpix_menu/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      213 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      419 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1560 2021-09-19 16:06:48.000000 garpix_menu-1.8.0/garpix_menu/__pycache__/context_processors.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      198 2021-09-08 12:08:50.000000 garpix_menu-1.8.0/garpix_menu/__pycache__/tests.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      992 2021-10-29 06:54:36.000000 garpix_menu-1.8.0/garpix_menu/__pycache__/validators.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.019760 garpix_menu-1.8.0/garpix_menu/admin/
--rw-r--r--   0 crusat     (501) staff       (20)       45 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/admin/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.019972 garpix_menu-1.8.0/garpix_menu/admin/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      210 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1780 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/admin/__pycache__/menu_item.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1364 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/admin/menu_item.py
--rw-r--r--   0 crusat     (501) staff       (20)      126 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/apps.py
--rw-r--r--   0 crusat     (501) staff       (20)      533 2021-09-19 16:19:40.000000 garpix_menu-1.8.0/garpix_menu/context_processors.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.020170 garpix_menu-1.8.0/garpix_menu/mixins/
--rw-r--r--   0 crusat     (501) staff       (20)       42 2021-09-18 13:24:06.000000 garpix_menu-1.8.0/garpix_menu/mixins/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.020389 garpix_menu-1.8.0/garpix_menu/mixins/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      208 2021-09-18 13:24:07.000000 garpix_menu-1.8.0/garpix_menu/mixins/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1837 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu/mixins/__pycache__/link_mixin.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1664 2022-04-22 07:49:09.000000 garpix_menu-1.8.0/garpix_menu/mixins/link_mixin.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.020604 garpix_menu-1.8.0/garpix_menu/models/
--rw-r--r--   0 crusat     (501) staff       (20)       39 2022-01-12 12:38:27.000000 garpix_menu-1.8.0/garpix_menu/models/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.020822 garpix_menu-1.8.0/garpix_menu/models/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      206 2022-01-12 12:38:36.000000 garpix_menu-1.8.0/garpix_menu/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2491 2021-11-08 13:58:31.000000 garpix_menu-1.8.0/garpix_menu/models/__pycache__/menu_item.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2108 2021-11-08 13:58:13.000000 garpix_menu-1.8.0/garpix_menu/models/menu_item.py
--rw-r--r--   0 crusat     (501) staff       (20)      198 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/serializers.py
--rw-r--r--   0 crusat     (501) staff       (20)     1141 2022-04-22 07:50:34.000000 garpix_menu-1.8.0/garpix_menu/setup.py
--rw-r--r--   0 crusat     (501) staff       (20)       68 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/tests.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.021037 garpix_menu-1.8.0/garpix_menu/translation/
--rw-r--r--   0 crusat     (501) staff       (20)       53 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/translation/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.021245 garpix_menu-1.8.0/garpix_menu/translation/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      224 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      504 2021-07-20 10:21:37.000000 garpix_menu-1.8.0/garpix_menu/translation/__pycache__/menu.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      200 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/translation/menu.py
--rw-r--r--   0 crusat     (501) staff       (20)      176 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/urls.py
--rw-r--r--   0 crusat     (501) staff       (20)     1822 2022-01-12 12:39:11.000000 garpix_menu-1.8.0/garpix_menu/utils.py
--rw-r--r--   0 crusat     (501) staff       (20)      838 2021-10-29 06:53:19.000000 garpix_menu-1.8.0/garpix_menu/validators.py
--rw-r--r--   0 crusat     (501) staff       (20)      503 2021-07-20 10:19:22.000000 garpix_menu-1.8.0/garpix_menu/views.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-04-22 07:50:42.019044 garpix_menu-1.8.0/garpix_menu.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     5932 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)     1459 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)       83 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       12 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/garpix_menu.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2022-04-22 07:50:42.021588 garpix_menu-1.8.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1141 2022-04-22 07:50:41.000000 garpix_menu-1.8.0/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.576898 garpix_menu-1.9.0/
+-rw-r--r--   0 crusat     (501) staff       (20)       73 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     5932 2022-06-29 08:25:32.576696 garpix_menu-1.9.0/PKG-INFO
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.570698 garpix_menu-1.9.0/garpix_menu/
+-rw-r--r--   0 crusat     (501) staff       (20)       73 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     5305 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/README.rst
+-rw-r--r--   0 crusat     (501) staff       (20)       57 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.574272 garpix_menu-1.9.0/garpix_menu/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      213 2021-07-20 10:21:37.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      419 2021-07-20 10:21:37.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      749 2022-06-29 07:53:33.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/context_processors.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      198 2021-09-08 12:08:50.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/tests.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1411 2022-06-29 07:53:33.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      992 2021-10-29 06:54:36.000000 garpix_menu-1.9.0/garpix_menu/__pycache__/validators.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.574484 garpix_menu-1.9.0/garpix_menu/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)       45 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/admin/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.574718 garpix_menu-1.9.0/garpix_menu/admin/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      210 2021-07-20 10:21:37.000000 garpix_menu-1.9.0/garpix_menu/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1814 2022-06-29 07:52:56.000000 garpix_menu-1.9.0/garpix_menu/admin/__pycache__/menu_item.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1399 2022-06-29 07:44:03.000000 garpix_menu-1.9.0/garpix_menu/admin/menu_item.py
+-rw-r--r--   0 crusat     (501) staff       (20)      126 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/apps.py
+-rw-r--r--   0 crusat     (501) staff       (20)      533 2021-09-19 16:19:40.000000 garpix_menu-1.9.0/garpix_menu/context_processors.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.574935 garpix_menu-1.9.0/garpix_menu/mixins/
+-rw-r--r--   0 crusat     (501) staff       (20)       42 2021-09-18 13:24:06.000000 garpix_menu-1.9.0/garpix_menu/mixins/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.575147 garpix_menu-1.9.0/garpix_menu/mixins/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      208 2021-09-18 13:24:07.000000 garpix_menu-1.9.0/garpix_menu/mixins/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1837 2022-04-22 07:50:41.000000 garpix_menu-1.9.0/garpix_menu/mixins/__pycache__/link_mixin.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1664 2022-04-22 07:49:09.000000 garpix_menu-1.9.0/garpix_menu/mixins/link_mixin.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.575448 garpix_menu-1.9.0/garpix_menu/models/
+-rw-r--r--   0 crusat     (501) staff       (20)       39 2022-01-12 12:38:27.000000 garpix_menu-1.9.0/garpix_menu/models/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.575883 garpix_menu-1.9.0/garpix_menu/models/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      206 2022-01-12 12:38:36.000000 garpix_menu-1.9.0/garpix_menu/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2773 2022-06-29 07:44:50.000000 garpix_menu-1.9.0/garpix_menu/models/__pycache__/menu_item.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     2418 2022-06-29 07:44:03.000000 garpix_menu-1.9.0/garpix_menu/models/menu_item.py
+-rw-r--r--   0 crusat     (501) staff       (20)      198 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/serializers.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1174 2022-06-29 07:44:40.000000 garpix_menu-1.9.0/garpix_menu/setup.py
+-rw-r--r--   0 crusat     (501) staff       (20)       68 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/tests.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.576193 garpix_menu-1.9.0/garpix_menu/translation/
+-rw-r--r--   0 crusat     (501) staff       (20)       53 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/translation/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.576460 garpix_menu-1.9.0/garpix_menu/translation/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      224 2021-07-20 10:21:37.000000 garpix_menu-1.9.0/garpix_menu/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      504 2021-07-20 10:21:37.000000 garpix_menu-1.9.0/garpix_menu/translation/__pycache__/menu.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      200 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/translation/menu.py
+-rw-r--r--   0 crusat     (501) staff       (20)      176 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/urls.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1832 2022-06-29 07:44:03.000000 garpix_menu-1.9.0/garpix_menu/utils.py
+-rw-r--r--   0 crusat     (501) staff       (20)      838 2021-10-29 06:53:19.000000 garpix_menu-1.9.0/garpix_menu/validators.py
+-rw-r--r--   0 crusat     (501) staff       (20)      503 2021-07-20 10:19:22.000000 garpix_menu-1.9.0/garpix_menu/views.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-06-29 08:25:32.573570 garpix_menu-1.9.0/garpix_menu.egg-info/
+-rw-r--r--   0 crusat     (501) staff       (20)     5932 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/PKG-INFO
+-rw-r--r--   0 crusat     (501) staff       (20)     1504 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/not-zip-safe
+-rw-r--r--   0 crusat     (501) staff       (20)      104 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/requires.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       12 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/garpix_menu.egg-info/top_level.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       38 2022-06-29 08:25:32.576941 garpix_menu-1.9.0/setup.cfg
+-rw-r--r--   0 crusat     (501) staff       (20)     1174 2022-06-29 08:25:32.000000 garpix_menu-1.9.0/setup.py
```

### Comparing `garpix_menu-1.8.0/PKG-INFO` & `garpix_menu-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_menu
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: garpix_menu Version: 1.8.0 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: garpix_menu Version: 1.9.0 Summary: UNKNOWN Home-
 page: UNKNOWN Author: Garpix LTD Author-email: info@garpix.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
 Environment :: Web Environment Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Framework :: Django Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `garpix_menu-1.8.0/garpix_menu/README.rst` & `garpix_menu-1.9.0/garpix_menu/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu/__pycache__/context_processors.cpython-38.pyc` & `garpix_menu-1.9.0/garpix_menu/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Sep 19 16:04:42 2021 UTC, .py size: 1769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,89 @@
-00000000: 550d 0d0a 0000 0000 9a5f 4761 e906 0000  U........_Ga....
+00000000: 550d 0d0a 0000 0000 c302 bc62 2807 0000  U..........b(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6405 6406 8400 5a07 6407  m.Z...d.d...Z.d.
-00000060: 6408 8400 5a08 6409 5300 290a 753c 0000  d...Z.d.S.).u<..
-00000070: 000a d09a d0be d0bd d182 d0b5 d0ba d181  ................
-00000080: d182 d0bd d18b d0b9 20d0 bfd1 80d0 bed1  ........ .......
-00000090: 86d0 b5d1 81d1 81d0 bed1 8020 d0b4 d0bb  ........... ....
-000000a0: d18f 20d0 bcd0 b5d0 bdd1 8e2e 0ae9 0000  .. .............
-000000b0: 0000 2901 da08 7365 7474 696e 6773 2901  ..)...settings).
-000000c0: da08 4d65 6e75 4974 656d 2901 da0d 6d6f  ..MenuItem)...mo
-000000d0: 6465 6c5f 746f 5f64 6963 7463 0100 0000  del_to_dictc....
-000000e0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-000000f0: 4300 0000 7330 0000 0064 0164 0267 027d  C...s0...d.d.g.}
-00000100: 0174 006a 0144 005d 187d 027c 01a0 0264  .t.j.D.].}.|...d
-00000110: 027c 0264 0319 009b 009d 02a1 0101 0071  .|.d...........q
-00000120: 0e7c 007c 016b 0653 0029 044e da00 fa01  .|.|.k.S.).N....
-00000130: 2f72 0100 0000 2903 7202 0000 00da 094c  /r....).r......L
-00000140: 414e 4755 4147 4553 da06 6170 7065 6e64  ANGUAGES..append
-00000150: 2903 da03 7572 6cda 0475 726c 73da 0469  )...url..urls..i
-00000160: 7465 6da9 0072 0c00 0000 fa4c 2f55 7365  tem..r.....L/Use
-00000170: 7273 2f63 7275 7361 742f 7072 6f6a 6563  rs/crusat/projec
-00000180: 7473 2f67 6172 7069 785f 6d65 6e75 2f62  ts/garpix_menu/b
-00000190: 6163 6b65 6e64 2f67 6172 7069 785f 6d65  ackend/garpix_me
-000001a0: 6e75 2f63 6f6e 7465 7874 5f70 726f 6365  nu/context_proce
-000001b0: 7373 6f72 732e 7079 da0d 6368 6563 6b5f  ssors.py..check_
-000001c0: 6973 5f68 6f6d 6509 0000 0073 0800 0000  is_home....s....
-000001d0: 0001 0801 0a01 1601 720e 0000 0063 0100  ........r....c..
-000001e0: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-000001f0: 0000 4300 0000 73ea 0000 007c 006a 007d  ..C...s....|.j.}
-00000200: 017c 017d 027c 0264 0119 0064 026b 0272  .|.}.|.d...d.k.r
-00000210: 227c 0264 0364 0185 0219 007d 0264 0469  "|.d.d.....}.d.i
-00000220: 0069 017d 0374 016a 0244 005d b47d 0474  .i.}.t.j.D.].}.t
-00000230: 036a 046a 0564 057c 0464 0319 0064 0664  .j.j.d.|.d...d.d
-00000240: 078d 037d 057c 05a0 0664 0864 09a1 027c  ...}.|...d.d...|
-00000250: 0364 0419 007c 0464 0319 003c 007c 0364  .d...|.d...<.|.d
-00000260: 0419 007c 0464 0319 0019 0044 005d 707d  ...|.d.....D.]p}
-00000270: 067c 06a0 07a1 007c 017c 0266 026b 0672  .|.....|.|.f.k.r
-00000280: 9464 057c 065f 0864 057c 065f 096e 467c  .d.|._.d.|._.nF|
-00000290: 01a0 0a7c 06a0 07a1 00a1 0172 b674 0b7c  ...|.......r.t.|
-000002a0: 06a0 07a1 0083 0173 da64 057c 065f 086e  .......s.d.|._.n
-000002b0: 247c 066a 0c72 da7c 066a 0ca0 0d7c 01a1  $|.j.r.|.j...|..
-000002c0: 0172 da74 0b7c 06a0 07a1 0083 0173 da64  .r.t.|.......s.d
-000002d0: 057c 065f 0874 0e7c 0683 017d 0671 7271  .|._.t.|...}.qrq
-000002e0: 307c 0353 0029 0a75 1801 0000 0a20 2020  0|.S.).u.....   
-000002f0: 20d0 9ad0 bed0 bdd1 82d0 b5d0 bad1 81d1   ...............
-00000300: 82d0 bdd1 8bd0 b920 d0bf d180 d0be d186  ....... ........
-00000310: d0b5 d181 d181 d0be d180 20d0 b4d0 bbd1  .......... .....
-00000320: 8f20 d0b2 d0be d0b7 d0bc d0be d0b6 d0bd  . ..............
-00000330: d0be d181 d182 d0b8 20d0 bed1 82d0 bed0  ........ .......
-00000340: b1d1 80d0 b0d0 b6d0 b5d0 bdd0 b8d1 8f20  ............... 
-00000350: d0b2 d181 d0b5 d185 20d0 bcd0 b5d0 bdd1  ........ .......
-00000360: 8e20 d0bd d0b0 20d1 81d0 b0d0 b9d1 82d0  . .... .........
-00000370: b52e 0a20 2020 20d0 9cd0 b5d0 bdd1 8e20  ...    ........ 
-00000380: d0be d0b1 d18b d187 d0bd d0be 20d1 80d0  ............ ...
-00000390: b0d1 81d0 bfd0 bed0 bbd0 bed0 b3d0 b0d1  ................
-000003a0: 8ed1 82d1 81d1 8f20 d0bd d0b0 20d0 bdd0  ....... .... ...
-000003b0: b5d1 81d0 bad0 bed0 bbd1 8cd0 bad0 b8d1  ................
-000003c0: 8520 d181 d182 d180 d0b0 d0bd d0b8 d186  . ..............
-000003d0: d0b0 d185 2c20 d0bf d0be d18d d182 d0be  ...., ..........
-000003e0: d0bc d183 20d0 b2d1 8bd0 bdd0 b5d1 81d0  .... ...........
-000003f0: b5d0 bdd0 be20 d181 d18e d0b4 d0b0 2e0a  ..... ..........
-00000400: 2020 2020 e9ff ffff ff72 0600 0000 7201      .....r....r.
-00000410: 0000 005a 056d 656e 7573 544e 2903 da09  ...Z.menusTN)...
-00000420: 6973 5f61 6374 6976 65da 096d 656e 755f  is_active..menu_
-00000430: 7479 7065 da06 7061 7265 6e74 da04 736f  type..parent..so
-00000440: 7274 da05 7469 746c 6529 0fda 0470 6174  rt..title)...pat
-00000450: 6872 0200 0000 da11 4348 4f49 4345 5f4d  hr......CHOICE_M
-00000460: 454e 555f 5459 5045 5372 0300 0000 da07  ENU_TYPESr......
-00000470: 6f62 6a65 6374 73da 0666 696c 7465 72da  objects..filter.
-00000480: 086f 7264 6572 5f62 79da 0867 6574 5f6c  .order_by..get_l
-00000490: 696e 6bda 0a69 735f 6375 7272 656e 74da  ink..is_current.
-000004a0: 0f69 735f 6375 7272 656e 745f 6675 6c6c  .is_current_full
-000004b0: da0a 7374 6172 7473 7769 7468 720e 0000  ..startswithr...
-000004c0: 0072 0900 0000 da08 656e 6473 7769 7468  .r......endswith
-000004d0: 7204 0000 0029 07da 0772 6571 7565 7374  r....)...request
-000004e0: da0c 6375 7272 656e 745f 7061 7468 5a1a  ..current_pathZ.
-000004f0: 6375 7272 656e 745f 7061 7468 5f77 6974  current_path_wit
-00000500: 686f 7574 5f73 6c61 7368 da07 636f 6e74  hout_slash..cont
-00000510: 6578 745a 0d6d 656e 755f 7479 7065 5f61  extZ.menu_type_a
-00000520: 7272 da04 6d65 6e75 da09 6d65 6e75 5f69  rr..menu..menu_i
-00000530: 7465 6d72 0c00 0000 720c 0000 0072 0d00  temr....r....r..
-00000540: 0000 da0e 6d65 6e75 5f70 726f 6365 7373  ....menu_process
-00000550: 6f72 1000 0000 732c 0000 0000 0506 0104  or....s,........
-00000560: 010c 010c 0302 0002 ff04 030a 0116 0118  ................
-00000570: 0114 0110 0106 0108 010e 010c 0108 0112  ................
-00000580: 010c 0106 010c 0172 2400 0000 4e29 09da  .......r$...N)..
-00000590: 075f 5f64 6f63 5f5f da0b 646a 616e 676f  .__doc__..django
-000005a0: 2e63 6f6e 6672 0200 0000 5a12 6761 7270  .confr....Z.garp
-000005b0: 6978 5f6d 656e 752e 6d6f 6465 6c73 7203  ix_menu.modelsr.
-000005c0: 0000 00da 1364 6a61 6e67 6f2e 666f 726d  .....django.form
-000005d0: 732e 6d6f 6465 6c73 7204 0000 0072 0e00  s.modelsr....r..
-000005e0: 0000 7224 0000 0072 0c00 0000 720c 0000  ..r$...r....r...
-000005f0: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
-00000600: 6475 6c65 3e01 0000 0073 0a00 0000 0403  dule>....s......
-00000610: 0c01 0c01 0c03 0807                      ........
+00000020: 0002 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6404 6405 8400 5a06 6406 6407 8400  ..d.d...Z.d.d...
+00000060: 5a07 6408 5300 2909 e900 0000 0029 01da  Z.d.S.)......)..
+00000070: 0873 6574 7469 6e67 7329 01da 0d6d 6f64  .settings)...mod
+00000080: 656c 5f74 6f5f 6469 6374 2901 da08 4d65  el_to_dict)...Me
+00000090: 6e75 4974 656d 6301 0000 0000 0000 0000  nuItemc.........
+000000a0: 0000 0003 0000 0006 0000 0043 0000 0073  ...........C...s
+000000b0: 3000 0000 6401 6402 6702 7d01 7400 6a01  0...d.d.g.}.t.j.
+000000c0: 4400 5d18 7d02 7c01 a002 6402 7c02 6403  D.].}.|...d.|.d.
+000000d0: 1900 9b00 9d02 a101 0100 710e 7c00 7c01  ..........q.|.|.
+000000e0: 6b06 5300 2904 4eda 00fa 012f 7201 0000  k.S.).N..../r...
+000000f0: 0029 0372 0200 0000 da09 4c41 4e47 5541  .).r......LANGUA
+00000100: 4745 53da 0661 7070 656e 6429 03da 0375  GES..append)...u
+00000110: 726c da04 7572 6c73 da04 6974 656d a900  rl..urls..item..
+00000120: 720c 0000 00fa 3f2f 5573 6572 732f 6372  r.....?/Users/cr
+00000130: 7573 6174 2f70 726f 6a65 6374 732f 6761  usat/projects/ga
+00000140: 7270 6978 5f6d 656e 752f 6261 636b 656e  rpix_menu/backen
+00000150: 642f 6761 7270 6978 5f6d 656e 752f 7574  d/garpix_menu/ut
+00000160: 696c 732e 7079 da0d 6368 6563 6b5f 6973  ils.py..check_is
+00000170: 5f68 6f6d 6506 0000 0073 0800 0000 0001  _home....s......
+00000180: 0801 0a01 1601 720e 0000 0063 0100 0000  ......r....c....
+00000190: 0000 0000 0000 0000 0700 0000 0a00 0000  ................
+000001a0: 4300 0000 7392 0100 007c 007d 017c 0164  C...s....|.}.|.d
+000001b0: 0119 0064 026b 0272 1c7c 0164 0364 0185  ...d.k.r.|.d.d..
+000001c0: 0219 007d 0169 007d 0274 006a 0144 0090  ...}.i.}.t.j.D..
+000001d0: 015d 647d 0374 026a 036a 0464 047c 0364  .]d}.t.j.j.d.|.d
+000001e0: 0319 0064 0064 058d 037d 0467 007c 027c  ...d.d...}.g.|.|
+000001f0: 0364 0319 003c 007c 04a0 0564 0664 07a1  .d...<.|...d.d..
+00000200: 0244 0090 015d 2e7d 057c 05a0 06a1 007d  .D...].}.|.....}
+00000210: 067c 067c 007c 0166 026b 0672 8264 047c  .|.|.|.f.k.r.d.|
+00000220: 055f 0764 047c 055f 086e 3a7c 00a0 097c  ._.d.|._.n:|...|
+00000230: 06a1 0172 9c74 0a7c 0683 0173 bc64 047c  ...r.t.|...s.d.|
+00000240: 055f 076e 207c 056a 0b72 bc7c 056a 0ba0  ._.n |.j.r.|.j..
+00000250: 0c7c 00a1 0172 bc74 0a7c 0683 0173 bc64  .|...r.t.|...s.d
+00000260: 047c 055f 077c 027c 0364 0319 0019 00a0  .|._.|.|.d......
+00000270: 0d74 0e7c 0583 01a1 0101 007c 067c 027c  .t.|.......|.|.|
+00000280: 0364 0319 0019 0064 0119 0064 083c 007c  .d.....d...d.<.|
+00000290: 056a 077c 027c 0364 0319 0019 0064 0119  .j.|.|.d.....d..
+000002a0: 0064 093c 007c 056a 087c 027c 0364 0319  .d.<.|.j.|.|.d..
+000002b0: 0019 0064 0119 0064 0a3c 007a 1c7c 056a  ...d...d.<.z.|.j
+000002c0: 0f6a 0b7c 027c 0364 0319 0019 0064 0119  .j.|.|.d.....d..
+000002d0: 0064 0b3c 0057 006e 2a04 0074 106b 0a90  .d.<.W.n*..t.k..
+000002e0: 0172 5801 0001 0001 0064 007c 027c 0364  .rX......d.|.|.d
+000002f0: 0319 0019 0064 0119 0064 0b3c 0059 006e  .....d...d.<.Y.n
+00000300: 0258 007c 027c 0364 0319 0019 0064 0119  .X.|.|.d.....d..
+00000310: 00a0 1164 0c64 00a1 0201 007c 027c 0364  ...d.d.....|.|.d
+00000320: 0319 0019 0064 0119 00a0 1164 0d64 00a1  .....d.....d.d..
+00000330: 0201 0071 5a71 267c 0253 0029 0e4e e9ff  ...qZq&|.S.).N..
+00000340: ffff ff72 0600 0000 7201 0000 0054 2903  ...r....r....T).
+00000350: da09 6973 5f61 6374 6976 65da 096d 656e  ..is_active..men
+00000360: 755f 7479 7065 da06 7061 7265 6e74 da04  u_type..parent..
+00000370: 736f 7274 da05 7469 746c 65da 0867 6574  sort..title..get
+00000380: 5f6c 696e 6bda 0a69 735f 6375 7272 656e  _link..is_curren
+00000390: 74da 0f69 735f 6375 7272 656e 745f 6675  t..is_current_fu
+000003a0: 6c6c da04 6963 6f6e da04 7061 6765 da0f  ll..icon..page..
+000003b0: 7469 746c 655f 666f 725f 6164 6d69 6e29  title_for_admin)
+000003c0: 1272 0200 0000 da11 4348 4f49 4345 5f4d  .r......CHOICE_M
+000003d0: 454e 555f 5459 5045 5372 0400 0000 da07  ENU_TYPESr......
+000003e0: 6f62 6a65 6374 73da 0666 696c 7465 72da  objects..filter.
+000003f0: 086f 7264 6572 5f62 7972 1500 0000 7216  .order_byr....r.
+00000400: 0000 0072 1700 0000 da0a 7374 6172 7473  ...r......starts
+00000410: 7769 7468 720e 0000 0072 0900 0000 da08  withr....r......
+00000420: 656e 6473 7769 7468 7208 0000 0072 0300  endswithr....r..
+00000430: 0000 7218 0000 00da 0945 7863 6570 7469  ..r......Excepti
+00000440: 6f6e da03 706f 7029 07da 0c63 7572 7265  on..pop)...curre
+00000450: 6e74 5f70 6174 685a 1a63 7572 7265 6e74  nt_pathZ.current
+00000460: 5f70 6174 685f 7769 7468 6f75 745f 736c  _path_without_sl
+00000470: 6173 68da 056d 656e 7573 5a0d 6d65 6e75  ash..menusZ.menu
+00000480: 5f74 7970 655f 6172 72da 046d 656e 75da  _type_arr..menu.
+00000490: 096d 656e 755f 6974 656d da04 6c69 6e6b  .menu_item..link
+000004a0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+000004b0: 0967 6574 5f6d 656e 7573 0d00 0000 733a  .get_menus....s:
+000004c0: 0000 0000 0104 010c 010c 0204 010c 0116  ................
+000004d0: 010c 0112 0108 010c 0106 0108 010a 0108  ................
+000004e0: 0108 0112 0108 0106 0116 0114 0116 0116  ................
+000004f0: 0102 011c 0110 011a 0118 011c 0172 2800  .............r(.
+00000500: 0000 4e29 08da 0b64 6a61 6e67 6f2e 636f  ..N)...django.co
+00000510: 6e66 7202 0000 00da 1364 6a61 6e67 6f2e  nfr......django.
+00000520: 666f 726d 732e 6d6f 6465 6c73 7203 0000  forms.modelsr...
+00000530: 005a 1267 6172 7069 785f 6d65 6e75 2e6d  .Z.garpix_menu.m
+00000540: 6f64 656c 7372 0400 0000 720e 0000 0072  odelsr....r....r
+00000550: 2800 0000 720c 0000 0072 0c00 0000 720c  (...r....r....r.
+00000560: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000570: 653e 0100 0000 7308 0000 000c 010c 010c  e>....s.........
+00000580: 0308 07                                  ...
```

### Comparing `garpix_menu-1.8.0/garpix_menu/__pycache__/validators.cpython-38.pyc` & `garpix_menu-1.9.0/garpix_menu/__pycache__/validators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu/admin/__pycache__/menu_item.cpython-38.pyc` & `garpix_menu-1.9.0/garpix_menu/admin/__pycache__/menu_item.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jul 20 10:19:22 2021 UTC, .py size: 1364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2aa3 f660 5405 0000  U.......*..`T...
+00000000: 550d 0d0a 0000 0000 c302 bc62 7705 0000  U..........bw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6501 a00c 6509 a101 4700  m.Z...e...e...G.
@@ -12,101 +12,103 @@
 000000b0: 2901 da16 4368 6563 6b62 6f78 5365 6c65  )...CheckboxSele
 000000c0: 6374 4d75 6c74 6970 6c65 2901 da12 4472  ctMultiple)...Dr
 000000d0: 6167 6761 626c 654d 5054 5441 646d 696e  aggableMPTTAdmin
 000000e0: 2901 da08 4d65 6e75 4974 656d 2901 da16  )...MenuItem)...
 000000f0: 5461 6262 6564 5472 616e 736c 6174 696f  TabbedTranslatio
 00000100: 6e41 646d 696e 6300 0000 0000 0000 0000  nAdminc.........
 00000110: 0000 0000 0000 0003 0000 0000 0000 0073  ...............s
-00000120: 5800 0000 6500 5a01 6400 5a02 6401 5a03  X...e.Z.d.Z.d.Z.
+00000120: 5e00 0000 6500 5a01 6400 5a02 6401 5a03  ^...e.Z.d.Z.d.Z.
 00000130: 6402 5a04 6403 5a05 6506 6a07 6404 6508  d.Z.d.Z.e.j.d.e.
 00000140: 6901 6901 5a09 6405 5a0a 6406 5a0b 6407  i.i.Z.d.Z.d.Z.d.
-00000150: 5a0c 6408 6409 8400 5a0d 640a 640b 8400  Z.d.d...Z.d.d...
-00000160: 5a0e 640c 650e 5f0f 8700 6601 640d 640e  Z.d.e._...f.d.d.
-00000170: 8408 5a10 8700 0400 5a11 5300 290f da0d  ..Z.....Z.S.)...
-00000180: 4d65 6e75 4974 656d 4164 6d69 6e29 01da  MenuItemAdmin)..
-00000190: 0772 6562 7569 6c64 2902 da06 7061 7265  .rebuild)...pare
-000001a0: 6e74 da09 6973 5f61 6374 6976 6529 08da  nt..is_active)..
-000001b0: 0c74 7265 655f 6163 7469 6f6e 73da 0e69  .tree_actions..i
-000001c0: 6e64 656e 7465 645f 7469 746c 65da 0574  ndented_title..t
-000001d0: 6974 6c65 da09 6d65 6e75 5f74 7970 65da  itle..menu_type.
-000001e0: 0867 6574 5f6c 696e 6bda 0c74 6172 6765  .get_link..targe
-000001f0: 745f 626c 616e 6b72 0b00 0000 da04 736f  t_blankr......so
-00000200: 7274 da06 7769 6467 6574 2901 720e 0000  rt..widget).r...
-00000210: 0029 0172 1200 0000 2901 720d 0000 0063  .).r....).r....c
-00000220: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000230: 0600 0000 4300 0000 7322 0000 007a 107c  ....C...s"...z.|
-00000240: 006a 006a 01a0 02a1 0001 0057 006e 0c01  .j.j.......W.n..
-00000250: 0001 0001 0059 006e 0258 0064 0053 00a9  .....Y.n.X.d.S..
-00000260: 014e 2903 da05 6d6f 6465 6cda 076f 626a  .N)...model..obj
-00000270: 6563 7473 7209 0000 0029 01da 0473 656c  ectsr....)...sel
-00000280: 66a9 0072 1800 0000 fa49 2f55 7365 7273  f..r.....I/Users
-00000290: 2f63 7275 7361 742f 7072 6f6a 6563 7473  /crusat/projects
-000002a0: 2f67 6172 7069 785f 6d65 6e75 2f62 6163  /garpix_menu/bac
-000002b0: 6b65 6e64 2f67 6172 7069 785f 6d65 6e75  kend/garpix_menu
-000002c0: 2f61 646d 696e 2f6d 656e 755f 6974 656d  /admin/menu_item
-000002d0: 2e70 79da 085f 7265 6275 696c 6415 0000  .py.._rebuild...
-000002e0: 0073 0800 0000 0001 0201 1001 0601 7a16  .s............z.
-000002f0: 4d65 6e75 4974 656d 4164 6d69 6e2e 5f72  MenuItemAdmin._r
-00000300: 6562 7569 6c64 6303 0000 0000 0000 0000  ebuildc.........
-00000310: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-00000320: 0c00 0000 7c00 a000 a100 0100 6401 5300  ....|.......d.S.
-00000330: 2902 758d 0000 000a 2020 2020 2020 2020  ).u.....        
-00000340: d09f d0b5 d180 d0b5 d181 d0be d180 d0b1  ................
-00000350: d0b0 d182 d18c 20d0 9cd0 9fd0 a2d0 a220  ...... ........ 
-00000360: d0bc d0be d0b4 d0b5 d0bb d18c 2e20 d098  ............. ..
-00000370: d0bd d0be d0b3 d0b4 d0b0 20d1 82d1 80d0  .......... .....
-00000380: b5d0 b1d1 83d0 b5d1 82d1 81d1 8f20 d0b4  ............. ..
-00000390: d0bb d18f 20d0 bfd0 b5d1 80d0 b5d0 b7d0  .... ...........
-000003a0: b0d0 b3d1 80d1 83d0 b7d0 bad0 b820 d0b4  ............. ..
-000003b0: d0b5 d180 d0b5 d0b2 d0b0 2e0a 2020 2020  ............    
-000003c0: 2020 2020 4e29 0172 1a00 0000 2903 7217      N).r....).r.
-000003d0: 0000 00da 0772 6571 7565 7374 da08 7175  .....request..qu
-000003e0: 6572 7973 6574 7218 0000 0072 1800 0000  erysetr....r....
-000003f0: 7219 0000 0072 0900 0000 1b00 0000 7302  r....r........s.
-00000400: 0000 0000 047a 154d 656e 7549 7465 6d41  .....z.MenuItemA
-00000410: 646d 696e 2e72 6562 7569 6c64 7532 0000  dmin.rebuildu2..
-00000420: 00d0 9fd0 b5d1 80d0 b5d1 81d0 bed0 b1d1  ................
-00000430: 80d0 b0d1 82d1 8c20 d0bf d183 d0bd d0ba  ....... ........
-00000440: d182 d18b 20d1 80d0 b0d0 b7d0 b4d0 b5d0  .... ...........
-00000450: bbd0 b063 0500 0000 0000 0000 0000 0000  ...c............
-00000460: 0500 0000 0600 0000 0300 0000 731e 0000  ............s...
-00000470: 007c 00a0 00a1 0001 0074 0183 00a0 027c  .|.......t.....|
-00000480: 017c 027c 037c 04a1 0401 0064 0053 0072  .|.|.|.....d.S.r
-00000490: 1400 0000 2903 721a 0000 00da 0573 7570  ....).r......sup
-000004a0: 6572 da0a 7361 7665 5f6d 6f64 656c 2905  er..save_model).
-000004b0: 7217 0000 0072 1b00 0000 da03 6f62 6ada  r....r......obj.
-000004c0: 0466 6f72 6dda 0663 6861 6e67 65a9 01da  .form..change...
-000004d0: 095f 5f63 6c61 7373 5f5f 7218 0000 0072  .__class__r....r
-000004e0: 1900 0000 721e 0000 0022 0000 0073 0400  ....r...."...s..
-000004f0: 0000 0002 0801 7a18 4d65 6e75 4974 656d  ......z.MenuItem
-00000500: 4164 6d69 6e2e 7361 7665 5f6d 6f64 656c  Admin.save_model
-00000510: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000520: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000530: 6e61 6d65 5f5f da07 6163 7469 6f6e 73da  name__..actions.
-00000540: 0b6c 6973 745f 6669 6c74 6572 da0c 6c69  .list_filter..li
-00000550: 7374 5f64 6973 706c 6179 7203 0000 00da  st_displayr.....
-00000560: 0f4d 616e 7954 6f4d 616e 7946 6965 6c64  .ManyToManyField
-00000570: 7204 0000 00da 1366 6f72 6d66 6965 6c64  r......formfield
-00000580: 5f6f 7665 7272 6964 6573 da0d 7365 6172  _overrides..sear
-00000590: 6368 5f66 6965 6c64 73da 0d6c 6973 745f  ch_fields..list_
-000005a0: 6564 6974 6162 6c65 da12 6c69 7374 5f64  editable..list_d
-000005b0: 6973 706c 6179 5f6c 696e 6b73 721a 0000  isplay_linksr...
-000005c0: 0072 0900 0000 da11 7368 6f72 745f 6465  .r......short_de
-000005d0: 7363 7269 7074 696f 6e72 1e00 0000 da0d  scriptionr......
-000005e0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1800  __classcell__r..
-000005f0: 0000 7218 0000 0072 2200 0000 7219 0000  ..r....r"...r...
-00000600: 0072 0800 0000 0900 0000 731a 0000 0008  .r........s.....
-00000610: 0204 0104 0104 0204 0006 ff04 0304 0104  ................
-00000620: 0104 0208 0608 0506 0272 0800 0000 4e29  .........r....N)
-00000630: 0e5a 0e64 6a61 6e67 6f2e 636f 6e74 7269  .Z.django.contri
-00000640: 6272 0200 0000 da09 646a 616e 676f 2e64  br......django.d
-00000650: 6272 0300 0000 5a0c 646a 616e 676f 2e66  br....Z.django.f
-00000660: 6f72 6d73 7204 0000 00da 0a6d 7074 742e  ormsr......mptt.
-00000670: 6164 6d69 6e72 0500 0000 5a12 6761 7270  adminr....Z.garp
-00000680: 6978 5f6d 656e 752e 6d6f 6465 6c73 7206  ix_menu.modelsr.
-00000690: 0000 005a 166d 6f64 656c 7472 616e 736c  ...Z.modeltransl
-000006a0: 6174 696f 6e2e 6164 6d69 6e72 0700 0000  ation.adminr....
-000006b0: da08 7265 6769 7374 6572 7208 0000 0072  ..registerr....r
-000006c0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-000006d0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000006e0: 0073 0e00 0000 0c01 0c01 0c01 0c01 0c01  .s..............
-000006f0: 0c03 0801                                ....
+00000150: 5a0c 6408 6701 5a0d 6409 640a 8400 5a0e  Z.d.g.Z.d.d...Z.
+00000160: 640b 640c 8400 5a0f 640d 650f 5f10 8700  d.d...Z.d.e._...
+00000170: 6601 640e 640f 8408 5a11 8700 0400 5a12  f.d.d...Z.....Z.
+00000180: 5300 2910 da0d 4d65 6e75 4974 656d 4164  S.)...MenuItemAd
+00000190: 6d69 6e29 01da 0772 6562 7569 6c64 2902  min)...rebuild).
+000001a0: da06 7061 7265 6e74 da09 6973 5f61 6374  ..parent..is_act
+000001b0: 6976 6529 08da 0c74 7265 655f 6163 7469  ive)...tree_acti
+000001c0: 6f6e 73da 0e69 6e64 656e 7465 645f 7469  ons..indented_ti
+000001d0: 746c 65da 0574 6974 6c65 da09 6d65 6e75  tle..title..menu
+000001e0: 5f74 7970 65da 0867 6574 5f6c 696e 6bda  _type..get_link.
+000001f0: 0c74 6172 6765 745f 626c 616e 6b72 0b00  .target_blankr..
+00000200: 0000 da04 736f 7274 da06 7769 6467 6574  ....sort..widget
+00000210: 2901 720e 0000 0029 0172 1200 0000 2901  ).r....).r....).
+00000220: 720d 0000 00da 0573 6974 6573 6301 0000  r......sitesc...
+00000230: 0000 0000 0000 0000 0001 0000 0006 0000  ................
+00000240: 0043 0000 0073 2200 0000 7a10 7c00 6a00  .C...s"...z.|.j.
+00000250: 6a01 a002 a100 0100 5700 6e0c 0100 0100  j.......W.n.....
+00000260: 0100 5900 6e02 5800 6400 5300 a901 4e29  ..Y.n.X.d.S...N)
+00000270: 03da 056d 6f64 656c da07 6f62 6a65 6374  ...model..object
+00000280: 7372 0900 0000 2901 da04 7365 6c66 a900  sr....)...self..
+00000290: 7219 0000 00fa 492f 5573 6572 732f 6372  r.....I/Users/cr
+000002a0: 7573 6174 2f70 726f 6a65 6374 732f 6761  usat/projects/ga
+000002b0: 7270 6978 5f6d 656e 752f 6261 636b 656e  rpix_menu/backen
+000002c0: 642f 6761 7270 6978 5f6d 656e 752f 6164  d/garpix_menu/ad
+000002d0: 6d69 6e2f 6d65 6e75 5f69 7465 6d2e 7079  min/menu_item.py
+000002e0: da08 5f72 6562 7569 6c64 1700 0000 7308  .._rebuild....s.
+000002f0: 0000 0000 0102 0110 0106 017a 164d 656e  ...........z.Men
+00000300: 7549 7465 6d41 646d 696e 2e5f 7265 6275  uItemAdmin._rebu
+00000310: 696c 6463 0300 0000 0000 0000 0000 0000  ildc............
+00000320: 0300 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00000330: 007c 00a0 00a1 0001 0064 0153 0029 0275  .|.......d.S.).u
+00000340: 8d00 0000 0a20 2020 2020 2020 20d0 9fd0  .....        ...
+00000350: b5d1 80d0 b5d1 81d0 bed1 80d0 b1d0 b0d1  ................
+00000360: 82d1 8c20 d09c d09f d0a2 d0a2 20d0 bcd0  ... ........ ...
+00000370: bed0 b4d0 b5d0 bbd1 8c2e 20d0 98d0 bdd0  .......... .....
+00000380: bed0 b3d0 b4d0 b020 d182 d180 d0b5 d0b1  ....... ........
+00000390: d183 d0b5 d182 d181 d18f 20d0 b4d0 bbd1  .......... .....
+000003a0: 8f20 d0bf d0b5 d180 d0b5 d0b7 d0b0 d0b3  . ..............
+000003b0: d180 d183 d0b7 d0ba d0b8 20d0 b4d0 b5d1  .......... .....
+000003c0: 80d0 b5d0 b2d0 b02e 0a20 2020 2020 2020  .........       
+000003d0: 204e 2901 721b 0000 0029 0372 1800 0000   N).r....).r....
+000003e0: da07 7265 7175 6573 74da 0871 7565 7279  ..request..query
+000003f0: 7365 7472 1900 0000 7219 0000 0072 1a00  setr....r....r..
+00000400: 0000 7209 0000 001d 0000 0073 0200 0000  ..r........s....
+00000410: 0004 7a15 4d65 6e75 4974 656d 4164 6d69  ..z.MenuItemAdmi
+00000420: 6e2e 7265 6275 696c 6475 3200 0000 d09f  n.rebuildu2.....
+00000430: d0b5 d180 d0b5 d181 d0be d0b1 d180 d0b0  ................
+00000440: d182 d18c 20d0 bfd1 83d0 bdd0 bad1 82d1  .... ...........
+00000450: 8b20 d180 d0b0 d0b7 d0b4 d0b5 d0bb d0b0  . ..............
+00000460: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00000470: 0006 0000 0003 0000 0073 1e00 0000 7c00  .........s....|.
+00000480: a000 a100 0100 7401 8300 a002 7c01 7c02  ......t.....|.|.
+00000490: 7c03 7c04 a104 0100 6400 5300 7215 0000  |.|.....d.S.r...
+000004a0: 0029 0372 1b00 0000 da05 7375 7065 72da  .).r......super.
+000004b0: 0a73 6176 655f 6d6f 6465 6c29 0572 1800  .save_model).r..
+000004c0: 0000 721c 0000 00da 036f 626a da04 666f  ..r......obj..fo
+000004d0: 726d da06 6368 616e 6765 a901 da09 5f5f  rm..change....__
+000004e0: 636c 6173 735f 5f72 1900 0000 721a 0000  class__r....r...
+000004f0: 0072 1f00 0000 2400 0000 7304 0000 0000  .r....$...s.....
+00000500: 0208 017a 184d 656e 7549 7465 6d41 646d  ...z.MenuItemAdm
+00000510: 696e 2e73 6176 655f 6d6f 6465 6c29 13da  in.save_model)..
+00000520: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000530: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000540: 655f 5fda 0761 6374 696f 6e73 da0b 6c69  e__..actions..li
+00000550: 7374 5f66 696c 7465 72da 0c6c 6973 745f  st_filter..list_
+00000560: 6469 7370 6c61 7972 0300 0000 da0f 4d61  displayr......Ma
+00000570: 6e79 546f 4d61 6e79 4669 656c 6472 0400  nyToManyFieldr..
+00000580: 0000 da13 666f 726d 6669 656c 645f 6f76  ....formfield_ov
+00000590: 6572 7269 6465 73da 0d73 6561 7263 685f  errides..search_
+000005a0: 6669 656c 6473 da0d 6c69 7374 5f65 6469  fields..list_edi
+000005b0: 7461 626c 65da 126c 6973 745f 6469 7370  table..list_disp
+000005c0: 6c61 795f 6c69 6e6b 73da 1166 696c 7465  lay_links..filte
+000005d0: 725f 686f 7269 7a6f 6e74 616c 721b 0000  r_horizontalr...
+000005e0: 0072 0900 0000 da11 7368 6f72 745f 6465  .r......short_de
+000005f0: 7363 7269 7074 696f 6e72 1f00 0000 da0d  scriptionr......
+00000600: 5f5f 636c 6173 7363 656c 6c5f 5f72 1900  __classcell__r..
+00000610: 0000 7219 0000 0072 2300 0000 721a 0000  ..r....r#...r...
+00000620: 0072 0800 0000 0900 0000 731c 0000 0008  .r........s.....
+00000630: 0204 0104 0104 0204 0006 ff04 0304 0104  ................
+00000640: 0104 0206 0208 0608 0506 0272 0800 0000  ...........r....
+00000650: 4e29 0e5a 0e64 6a61 6e67 6f2e 636f 6e74  N).Z.django.cont
+00000660: 7269 6272 0200 0000 da09 646a 616e 676f  ribr......django
+00000670: 2e64 6272 0300 0000 5a0c 646a 616e 676f  .dbr....Z.django
+00000680: 2e66 6f72 6d73 7204 0000 00da 0a6d 7074  .formsr......mpt
+00000690: 742e 6164 6d69 6e72 0500 0000 5a12 6761  t.adminr....Z.ga
+000006a0: 7270 6978 5f6d 656e 752e 6d6f 6465 6c73  rpix_menu.models
+000006b0: 7206 0000 005a 166d 6f64 656c 7472 616e  r....Z.modeltran
+000006c0: 736c 6174 696f 6e2e 6164 6d69 6e72 0700  slation.adminr..
+000006d0: 0000 da08 7265 6769 7374 6572 7208 0000  ....registerr...
+000006e0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+000006f0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000700: 0000 0073 0e00 0000 0c01 0c01 0c01 0c01  ...s............
+00000710: 0c01 0c03 0801                           ......
```

### Comparing `garpix_menu-1.8.0/garpix_menu/admin/menu_item.py` & `garpix_menu-1.9.0/garpix_menu/admin/menu_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     formfield_overrides = {
         models.ManyToManyField: {'widget': CheckboxSelectMultiple},
     }
     search_fields = ('title',)
     list_editable = ('sort',)
     list_display_links = ('indented_title',)
 
+    filter_horizontal = ['sites']
+
     def _rebuild(self):
         try:
             self.model.objects.rebuild()
         except:  # noqa
             pass
 
     def rebuild(self, request, queryset):
```

### Comparing `garpix_menu-1.8.0/garpix_menu/context_processors.py` & `garpix_menu-1.9.0/garpix_menu/context_processors.py`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu/mixins/__pycache__/link_mixin.cpython-38.pyc` & `garpix_menu-1.9.0/garpix_menu/mixins/__pycache__/link_mixin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu/mixins/link_mixin.py` & `garpix_menu-1.9.0/garpix_menu/mixins/link_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu/models/__pycache__/menu_item.cpython-38.pyc` & `garpix_menu-1.9.0/garpix_menu/models/__pycache__/menu_item.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Nov  8 13:58:13 2021 UTC, .py size: 2108 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,174 @@
-00000000: 550d 0d0a 0000 0000 f52c 8961 3c08 0000  U........,.a<...
+00000000: 550d 0d0a 0000 0000 c302 bc62 7209 0000  U..........br...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0005 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
-00000070: 6407 6c0b 6d0c 5a0c 0100 6406 6408 6c0d  d.l.m.Z...d.d.l.
-00000080: 6d0e 5a0e 6d0f 5a0f 0100 4700 6409 640a  m.Z.m.Z...G.d.d.
-00000090: 8400 640a 650c 6507 8304 5a10 640b 5300  ..d.e.e...Z.d.S.
-000000a0: 290c e900 0000 0029 01da 066d 6f64 656c  )......)...model
-000000b0: 7329 01da 0873 6574 7469 6e67 7329 01da  s)...settings)..
-000000c0: 0d67 6574 5f66 696c 655f 7061 7468 2902  .get_file_path).
-000000d0: da09 4d50 5454 4d6f 6465 6cda 0e54 7265  ..MPTTModel..Tre
-000000e0: 6546 6f72 6569 676e 4b65 7929 01da 0d41  eForeignKey)...A
-000000f0: 6374 6976 654d 616e 6167 6572 e902 0000  ctiveManager....
-00000100: 0029 01da 094c 696e 6b4d 6978 696e 2902  .)...LinkMixin).
-00000110: da0d 7661 6c69 6461 7465 5f74 7970 65da  ..validate_type.
-00000120: 0d76 616c 6964 6174 655f 7369 7a65 6300  .validate_sizec.
-00000130: 0000 0000 0000 0000 0000 0000 0000 0009  ................
-00000140: 0000 0040 0000 0073 e800 0000 6500 5a01  ...@...s....e.Z.
-00000150: 6400 5a02 6401 5a03 6504 6a05 6402 6403  d.Z.d.Z.e.j.d.d.
-00000160: 6404 6405 6406 8d04 5a06 6504 6a05 6402  d.d.d...Z.e.j.d.
-00000170: 6407 6408 8d02 5a07 6504 6a08 6509 6409  d.d...Z.e.j.e.d.
-00000180: 6403 6403 650a 650b 6702 640a 8d05 5a0c  d.d.e.e.g.d...Z.
-00000190: 6504 6a05 6404 6402 650d 6a0e 640b 640c  e.j.d.d.e.j.d.d.
-000001a0: 8d04 5a0f 6504 6a10 6403 640d 640e 8d02  ..Z.e.j.d.d.d...
-000001b0: 5a11 6504 6a10 640f 6410 640e 8d02 5a12  Z.e.j.d.d.d...Z.
-000001c0: 6504 6a13 6403 6411 6412 8d02 5a14 6504  e.j.d.d.d...Z.e.
-000001d0: 6a13 6403 6413 6414 8d02 5a15 6504 6a16  j.d.d.d...Z.e.j.
-000001e0: 6402 6415 6416 6417 8d03 5a17 6518 6418  d.d.d.d...Z.e.d.
-000001f0: 6403 6403 6419 6403 641a 6504 6a19 641b  d.d.d.d.d.e.j.d.
-00000200: 8d07 5a1a 640f 5a1b 640f 5a1c 651d 8300  ..Z.d.Z.d.Z.e...
-00000210: 5a1e 4700 641c 641d 8400 641d 8302 5a1f  Z.G.d.d...d...Z.
-00000220: 641e 641f 8400 5a20 6420 6421 8400 5a21  d.d...Z d d!..Z!
-00000230: 6422 5300 2923 da08 4d65 6e75 4974 656d  d"S.)#..MenuItem
-00000240: 7520 0000 000a 2020 2020 d09f d183 d0bd  u ....    ......
-00000250: d0ba d182 d18b 20d0 bcd0 b5d0 bdd1 8e2e  ...... .........
-00000260: 0a20 2020 20e9 6400 0000 54da 0075 2400  .    .d...T..u$.
-00000270: 0000 d09d d0b0 d0b7 d0b2 d0b0 d0bd d0b8  ................
-00000280: d0b5 20d0 b4d0 bbd1 8f20 d0b0 d0b4 d0bc  .. ...... ......
-00000290: d0b8 d0bd d0b0 2904 da0a 6d61 785f 6c65  ......)...max_le
-000002a0: 6e67 7468 da05 626c 616e 6bda 0764 6566  ngth..blank..def
-000002b0: 6175 6c74 da0c 7665 7262 6f73 655f 6e61  ault..verbose_na
-000002c0: 6d65 7510 0000 00d0 9dd0 b0d0 b7d0 b2d0  meu.............
-000002d0: b0d0 bdd0 b8d0 b529 0272 0f00 0000 7212  .......).r....r.
-000002e0: 0000 0075 0c00 0000 d098 d0ba d0be d0bd  ...u............
-000002f0: d0ba d0b0 2905 da09 7570 6c6f 6164 5f74  ....)...upload_t
-00000300: 6f72 1200 0000 7210 0000 00da 046e 756c  or....r......nul
-00000310: 6cda 0a76 616c 6964 6174 6f72 7375 0f00  l..validatorsu..
-00000320: 0000 d0a2 d0b8 d0bf 20d0 bcd0 b5d0 bdd1  ........ .......
-00000330: 8e29 0472 1100 0000 720f 0000 00da 0763  .).r....r......c
-00000340: 686f 6963 6573 7212 0000 0075 1000 0000  hoicesr....u....
-00000350: d092 d0ba d0bb d18e d187 d0b5 d0bd d0be  ................
-00000360: 2902 7211 0000 0072 1200 0000 4675 2900  ).r....r....Fu).
-00000370: 0000 d09e d182 d0ba d180 d18b d0b2 d0b0  ................
-00000380: d182 d18c 20d0 b220 d0bd d0be d0b2 d0be  .... .. ........
-00000390: d0bc 20d0 bed0 bad0 bdd0 b575 1900 0000  .. ........u....
-000003a0: d094 d0b0 d182 d0b0 20d1 81d0 bed0 b7d0  ........ .......
-000003b0: b4d0 b0d0 bdd0 b8d1 8f29 02da 0c61 7574  .........)...aut
-000003c0: 6f5f 6e6f 775f 6164 6472 1200 0000 751b  o_now_addr....u.
-000003d0: 0000 00d0 94d0 b0d1 82d0 b020 d0b8 d0b7  ........... ....
-000003e0: d0bc d0b5 d0bd d0b5 d0bd d0b8 d18f 2902  ..............).
-000003f0: da08 6175 746f 5f6e 6f77 7212 0000 0075  ..auto_nowr....u
-00000400: 1400 0000 d0a1 d0be d180 d182 d0b8 d180  ................
-00000410: d0be d0b2 d0ba d0b0 755a 0000 00d0 a7d0  ........uZ......
-00000420: b5d0 bc20 d0bc d0b5 d0bd d18c d188 d0b5  ... ............
-00000430: 20d1 87d0 b8d1 81d0 bbd0 be2c 20d1 82d0   .........., ...
-00000440: b5d0 bc20 d0b2 d18b d188 d0b5 20d0 b1d1  ... ........ ...
-00000450: 83d0 b4d0 b5d1 8220 d18d d0bb d0b5 d0bc  ....... ........
-00000460: d0b5 d0bd d182 20d0 b220 d181 d0bf d0b8  ...... .. ......
-00000470: d181 d0ba d0b5 2e29 0372 1100 0000 7212  .......).r....r.
-00000480: 0000 00da 0968 656c 705f 7465 7874 da04  .....help_text..
-00000490: 7365 6c66 da08 6368 696c 6472 656e 752c  self..childrenu,
-000004a0: 0000 00d0 a0d0 bed0 b4d0 b8d1 82d0 b5d0  ................
-000004b0: bbd1 8cd1 81d0 bad0 b8d0 b920 d0bf d183  ........... ....
-000004c0: d0bd d0ba d182 20d0 bcd0 b5d0 bdd1 8e29  ...... ........)
-000004d0: 0672 1400 0000 7210 0000 00da 0c72 656c  .r....r......rel
-000004e0: 6174 6564 5f6e 616d 65da 0864 625f 696e  ated_name..db_in
-000004f0: 6465 7872 1200 0000 da09 6f6e 5f64 656c  dexr......on_del
-00000500: 6574 6563 0000 0000 0000 0000 0000 0000  etec............
-00000510: 0000 0000 0100 0000 4000 0000 731c 0000  ........@...s...
-00000520: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00000530: 0464 035a 0564 045a 0664 0553 0029 067a  .d.Z.d.Z.d.S.).z
-00000540: 0d4d 656e 7549 7465 6d2e 4d65 7461 7513  .MenuItem.Metau.
-00000550: 0000 00d0 9fd1 83d0 bdd0 bad1 8220 d0bc  ............. ..
-00000560: d0b5 d0bd d18e 7515 0000 00d0 9fd1 83d0  ......u.........
-00000570: bdd0 bad1 82d1 8b20 d0bc d0b5 d0bd d18e  ....... ........
-00000580: 2901 da04 736f 7274 464e 2907 da08 5f5f  )...sortFN)...__
-00000590: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000005a0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000005b0: 7212 0000 00da 1376 6572 626f 7365 5f6e  r......verbose_n
-000005c0: 616d 655f 706c 7572 616c da08 6f72 6465  ame_plural..orde
-000005d0: 7269 6e67 da08 6162 7374 7261 6374 a900  ring..abstract..
-000005e0: 7226 0000 0072 2600 0000 fa4a 2f55 7365  r&...r&....J/Use
-000005f0: 7273 2f63 7275 7361 742f 7072 6f6a 6563  rs/crusat/projec
-00000600: 7473 2f67 6172 7069 785f 6d65 6e75 2f62  ts/garpix_menu/b
-00000610: 6163 6b65 6e64 2f67 6172 7069 785f 6d65  ackend/garpix_me
-00000620: 6e75 2f6d 6f64 656c 732f 6d65 6e75 5f69  nu/models/menu_i
-00000630: 7465 6d2e 7079 da04 4d65 7461 1f00 0000  tem.py..Meta....
-00000640: 7308 0000 0008 0104 0104 0104 0172 2800  s............r(.
-00000650: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000660: 0000 0001 0000 0043 0000 0073 1200 0000  .......C...s....
-00000670: 7c00 6a00 720c 7c00 6a00 5300 7c00 6a01  |.j.r.|.j.S.|.j.
-00000680: 5300 a901 4e29 02da 0f74 6974 6c65 5f66  S...N)...title_f
-00000690: 6f72 5f61 646d 696e da05 7469 746c 65a9  or_admin..title.
-000006a0: 0172 1a00 0000 7226 0000 0072 2600 0000  .r....r&...r&...
-000006b0: 7227 0000 00da 075f 5f73 7472 5f5f 2500  r'.....__str__%.
-000006c0: 0000 7306 0000 0000 0106 0106 017a 104d  ..s..........z.M
-000006d0: 656e 7549 7465 6d2e 5f5f 7374 725f 5f63  enuItem.__str__c
-000006e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000006f0: 0200 0000 4300 0000 730c 0000 0074 006a  ....C...s....t.j
-00000700: 017c 006a 0219 0053 0072 2900 0000 2903  .|.j...S.r)...).
-00000710: 7203 0000 00da 0a4d 454e 555f 5459 5045  r......MENU_TYPE
-00000720: 53da 096d 656e 755f 7479 7065 722c 0000  S..menu_typer,..
-00000730: 0072 2600 0000 7226 0000 0072 2700 0000  .r&...r&...r'...
-00000740: da0f 6765 745f 6d65 6e75 5f70 6172 616d  ..get_menu_param
-00000750: 732a 0000 0073 0200 0000 0001 7a18 4d65  s*...s......z.Me
-00000760: 6e75 4974 656d 2e67 6574 5f6d 656e 755f  nuItem.get_menu_
-00000770: 7061 7261 6d73 4e29 2272 2000 0000 7221  paramsN)"r ...r!
-00000780: 0000 0072 2200 0000 da07 5f5f 646f 635f  ...r".....__doc_
-00000790: 5f72 0200 0000 da09 4368 6172 4669 656c  _r......CharFiel
-000007a0: 6472 2a00 0000 722b 0000 00da 0946 696c  dr*...r+.....Fil
-000007b0: 6546 6965 6c64 7204 0000 0072 0a00 0000  eFieldr....r....
-000007c0: 720b 0000 005a 0469 636f 6e72 0300 0000  r....Z.iconr....
-000007d0: da11 4348 4f49 4345 5f4d 454e 555f 5459  ..CHOICE_MENU_TY
-000007e0: 5045 5372 2f00 0000 da0c 426f 6f6c 6561  PESr/.....Boolea
-000007f0: 6e46 6965 6c64 da09 6973 5f61 6374 6976  nField..is_activ
-00000800: 655a 0c74 6172 6765 745f 626c 616e 6bda  eZ.target_blank.
-00000810: 0d44 6174 6554 696d 6546 6965 6c64 da0a  .DateTimeField..
-00000820: 6372 6561 7465 645f 6174 da0a 7570 6461  created_at..upda
-00000830: 7465 645f 6174 da0c 496e 7465 6765 7246  ted_at..IntegerF
-00000840: 6965 6c64 721f 0000 0072 0600 0000 da07  ieldr....r......
-00000850: 4341 5343 4144 45da 0670 6172 656e 745a  CASCADE..parentZ
-00000860: 0a69 735f 6375 7272 656e 745a 0f69 735f  .is_currentZ.is_
-00000870: 6375 7272 656e 745f 6675 6c6c 7207 0000  current_fullr...
-00000880: 005a 0e61 6374 6976 655f 6d61 6e61 6765  .Z.active_manage
-00000890: 7272 2800 0000 722d 0000 0072 3000 0000  rr(...r-...r0...
-000008a0: 7226 0000 0072 2600 0000 7226 0000 0072  r&...r&...r&...r
-000008b0: 2700 0000 720c 0000 000a 0000 0073 2e00  '...r........s..
-000008c0: 0000 0801 0403 1201 0e01 0401 0200 0200  ................
-000008d0: 0200 0201 06fe 0604 1401 0e01 0e01 0e01  ................
-000008e0: 0e01 1001 1801 0401 0401 0602 0e06 0805  ................
-000008f0: 720c 0000 004e 2911 da09 646a 616e 676f  r....N)...django
-00000900: 2e64 6272 0200 0000 da0b 646a 616e 676f  .dbr......django
-00000910: 2e63 6f6e 6672 0300 0000 5a11 6761 7270  .confr....Z.garp
-00000920: 6978 5f75 7469 6c73 2e66 696c 6572 0400  ix_utils.filer..
-00000930: 0000 da0b 6d70 7474 2e6d 6f64 656c 7372  ....mptt.modelsr
-00000940: 0500 0000 7206 0000 005a 1567 6172 7069  ....r....Z.garpi
-00000950: 785f 7574 696c 732e 6d61 6e61 6765 7273  x_utils.managers
-00000960: 7207 0000 00da 066d 6978 696e 7372 0900  r......mixinsr..
-00000970: 0000 7215 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000980: 0072 0c00 0000 7226 0000 0072 2600 0000  .r....r&...r&...
-00000990: 7226 0000 0072 2700 0000 da08 3c6d 6f64  r&...r'.....<mod
-000009a0: 756c 653e 0100 0000 730e 0000 000c 010c  ule>....s.......
-000009b0: 010c 0110 010c 010c 0110 03              ...........
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6407 6c0d  m.Z.m.Z...d.d.l.
+00000080: 6d0e 5a0e 0100 6408 6409 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000090: 0100 6408 640a 6c11 6d12 5a12 6d13 5a13  ..d.d.l.m.Z.m.Z.
+000000a0: 0100 6400 640b 6c0d 6d14 5a14 0100 4700  ..d.d.l.m.Z...G.
+000000b0: 640c 640d 8400 640d 6510 650b 8304 5a15  d.d...d.e.e...Z.
+000000c0: 640e 5300 290f e900 0000 0029 01da 0453  d.S.)......)...S
+000000d0: 6974 6529 01da 066d 6f64 656c 7329 01da  ite)...models)..
+000000e0: 0873 6574 7469 6e67 7329 01da 0d67 6574  .settings)...get
+000000f0: 5f61 6c6c 5f73 6974 6573 2901 da0d 6765  _all_sites)...ge
+00000100: 745f 6669 6c65 5f70 6174 6829 02da 094d  t_file_path)...M
+00000110: 5054 544d 6f64 656c da0e 5472 6565 466f  PTTModel..TreeFo
+00000120: 7265 6967 6e4b 6579 2901 da0d 4163 7469  reignKey)...Acti
+00000130: 7665 4d61 6e61 6765 72e9 0200 0000 2901  veManager.....).
+00000140: da09 4c69 6e6b 4d69 7869 6e29 02da 0d76  ..LinkMixin)...v
+00000150: 616c 6964 6174 655f 7479 7065 da0d 7661  alidate_type..va
+00000160: 6c69 6461 7465 5f73 697a 6529 01da 1347  lidate_size)...G
+00000170: 4375 7272 656e 7453 6974 654d 616e 6167  CurrentSiteManag
+00000180: 6572 6300 0000 0000 0000 0000 0000 0000  erc.............
+00000190: 0000 0009 0000 0040 0000 0073 fe00 0000  .......@...s....
+000001a0: 6500 5a01 6400 5a02 6401 5a03 6504 6a05  e.Z.d.Z.d.Z.e.j.
+000001b0: 6402 6403 6404 6405 6406 8d04 5a06 6504  d.d.d.d.d...Z.e.
+000001c0: 6a05 6402 6407 6408 8d02 5a07 6504 6a08  j.d.d.d...Z.e.j.
+000001d0: 6509 6409 6403 6403 650a 650b 6702 640a  e.d.d.d.e.e.g.d.
+000001e0: 8d05 5a0c 6504 6a05 6404 6402 650d 6a0e  ..Z.e.j.d.d.e.j.
+000001f0: 640b 640c 8d04 5a0f 6504 6a10 6403 640d  d.d...Z.e.j.d.d.
+00000200: 640e 8d02 5a11 6504 6a10 640f 6410 640e  d...Z.e.j.d.d.d.
+00000210: 8d02 5a12 6504 6a13 6403 6411 6412 8d02  ..Z.e.j.d.d.d...
+00000220: 5a14 6504 6a13 6403 6413 6414 8d02 5a15  Z.e.j.d.d.d...Z.
+00000230: 6504 6a16 6402 6415 6416 6417 8d03 5a17  e.j.d.d.d.d...Z.
+00000240: 6518 6418 6403 6403 6419 6403 641a 6504  e.d.d.d.d.d.d.e.
+00000250: 6a19 641b 8d07 5a1a 6504 6a1b 651c 651d  j.d...Z.e.j.e.e.
+00000260: 641c 640e 8d03 5a1e 640f 5a1f 640f 5a20  d.d...Z.d.Z.d.Z 
+00000270: 6521 8300 5a22 6523 8300 5a24 4700 641d  e!..Z"e#..Z$G.d.
+00000280: 641e 8400 641e 8302 5a25 641f 6420 8400  d...d...Z%d.d ..
+00000290: 5a26 6421 6422 8400 5a27 6423 5300 2924  Z&d!d"..Z'd#S.)$
+000002a0: da08 4d65 6e75 4974 656d 7520 0000 000a  ..MenuItemu ....
+000002b0: 2020 2020 d09f d183 d0bd d0ba d182 d18b      ............
+000002c0: 20d0 bcd0 b5d0 bdd1 8e2e 0a20 2020 20e9   ..........    .
+000002d0: 6400 0000 54da 0075 2400 0000 d09d d0b0  d...T..u$.......
+000002e0: d0b7 d0b2 d0b0 d0bd d0b8 d0b5 20d0 b4d0  ............ ...
+000002f0: bbd1 8f20 d0b0 d0b4 d0bc d0b8 d0bd d0b0  ... ............
+00000300: 2904 da0a 6d61 785f 6c65 6e67 7468 da05  )...max_length..
+00000310: 626c 616e 6bda 0764 6566 6175 6c74 da0c  blank..default..
+00000320: 7665 7262 6f73 655f 6e61 6d65 7510 0000  verbose_nameu...
+00000330: 00d0 9dd0 b0d0 b7d0 b2d0 b0d0 bdd0 b8d0  ................
+00000340: b529 0272 1200 0000 7215 0000 0075 0c00  .).r....r....u..
+00000350: 0000 d098 d0ba d0be d0bd d0ba d0b0 2905  ..............).
+00000360: da09 7570 6c6f 6164 5f74 6f72 1500 0000  ..upload_tor....
+00000370: 7213 0000 00da 046e 756c 6cda 0a76 616c  r......null..val
+00000380: 6964 6174 6f72 7375 0f00 0000 d0a2 d0b8  idatorsu........
+00000390: d0bf 20d0 bcd0 b5d0 bdd1 8e29 0472 1400  .. ........).r..
+000003a0: 0000 7212 0000 00da 0763 686f 6963 6573  ..r......choices
+000003b0: 7215 0000 0075 1000 0000 d092 d0ba d0bb  r....u..........
+000003c0: d18e d187 d0b5 d0bd d0be 2902 7214 0000  ..........).r...
+000003d0: 0072 1500 0000 4675 2900 0000 d09e d182  .r....Fu).......
+000003e0: d0ba d180 d18b d0b2 d0b0 d182 d18c 20d0  .............. .
+000003f0: b220 d0bd d0be d0b2 d0be d0bc 20d0 bed0  . .......... ...
+00000400: bad0 bdd0 b575 1900 0000 d094 d0b0 d182  .....u..........
+00000410: d0b0 20d1 81d0 bed0 b7d0 b4d0 b0d0 bdd0  .. .............
+00000420: b8d1 8f29 02da 0c61 7574 6f5f 6e6f 775f  ...)...auto_now_
+00000430: 6164 6472 1500 0000 751b 0000 00d0 94d0  addr....u.......
+00000440: b0d1 82d0 b020 d0b8 d0b7 d0bc d0b5 d0bd  ..... ..........
+00000450: d0b5 d0bd d0b8 d18f 2902 da08 6175 746f  ........)...auto
+00000460: 5f6e 6f77 7215 0000 0075 1400 0000 d0a1  _nowr....u......
+00000470: d0be d180 d182 d0b8 d180 d0be d0b2 d0ba  ................
+00000480: d0b0 755a 0000 00d0 a7d0 b5d0 bc20 d0bc  ..uZ......... ..
+00000490: d0b5 d0bd d18c d188 d0b5 20d1 87d0 b8d1  .......... .....
+000004a0: 81d0 bbd0 be2c 20d1 82d0 b5d0 bc20 d0b2  ....., ...... ..
+000004b0: d18b d188 d0b5 20d0 b1d1 83d0 b4d0 b5d1  ...... .........
+000004c0: 8220 d18d d0bb d0b5 d0bc d0b5 d0bd d182  . ..............
+000004d0: 20d0 b220 d181 d0bf d0b8 d181 d0ba d0b5   .. ............
+000004e0: 2e29 0372 1400 0000 7215 0000 00da 0968  .).r....r......h
+000004f0: 656c 705f 7465 7874 da04 7365 6c66 da08  elp_text..self..
+00000500: 6368 696c 6472 656e 752c 0000 00d0 a0d0  childrenu,......
+00000510: bed0 b4d0 b8d1 82d0 b5d0 bbd1 8cd1 81d0  ................
+00000520: bad0 b8d0 b920 d0bf d183 d0bd d0ba d182  ..... ..........
+00000530: 20d0 bcd0 b5d0 bdd1 8e29 0672 1700 0000   ........).r....
+00000540: 7213 0000 00da 0c72 656c 6174 6564 5f6e  r......related_n
+00000550: 616d 65da 0864 625f 696e 6465 7872 1500  ame..db_indexr..
+00000560: 0000 da09 6f6e 5f64 656c 6574 6575 2800  ....on_deleteu(.
+00000570: 0000 d0a1 d0b0 d0b9 d182 d18b 20d0 b4d0  ............ ...
+00000580: bbd1 8f20 d0be d182 d0be d0b1 d180 d0b0  ... ............
+00000590: d0b6 d0b5 d0bd d0b8 d18f 6300 0000 0000  ..........c.....
+000005a0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000005b0: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000005c0: 6401 5a03 6402 5a04 6403 5a05 6404 5a06  d.Z.d.Z.d.Z.d.Z.
+000005d0: 6405 5300 2906 7a0d 4d65 6e75 4974 656d  d.S.).z.MenuItem
+000005e0: 2e4d 6574 6175 1300 0000 d09f d183 d0bd  .Metau..........
+000005f0: d0ba d182 20d0 bcd0 b5d0 bdd1 8e75 1500  .... ........u..
+00000600: 0000 d09f d183 d0bd d0ba d182 d18b 20d0  .............. .
+00000610: bcd0 b5d0 bdd1 8e29 01da 0473 6f72 7446  .......)...sortF
+00000620: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000630: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000640: 6c6e 616d 655f 5f72 1500 0000 da13 7665  lname__r......ve
+00000650: 7262 6f73 655f 6e61 6d65 5f70 6c75 7261  rbose_name_plura
+00000660: 6cda 086f 7264 6572 696e 67da 0861 6273  l..ordering..abs
+00000670: 7472 6163 74a9 0072 2900 0000 7229 0000  tract..r)...r)..
+00000680: 00fa 4a2f 5573 6572 732f 6372 7573 6174  ..J/Users/crusat
+00000690: 2f70 726f 6a65 6374 732f 6761 7270 6978  /projects/garpix
+000006a0: 5f6d 656e 752f 6261 636b 656e 642f 6761  _menu/backend/ga
+000006b0: 7270 6978 5f6d 656e 752f 6d6f 6465 6c73  rpix_menu/models
+000006c0: 2f6d 656e 755f 6974 656d 2e70 79da 044d  /menu_item.py..M
+000006d0: 6574 6124 0000 0073 0800 0000 0801 0401  eta$...s........
+000006e0: 0401 0401 722b 0000 0063 0100 0000 0000  ....r+...c......
+000006f0: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00000700: 0000 7312 0000 007c 006a 0072 0c7c 006a  ..s....|.j.r.|.j
+00000710: 0053 007c 006a 0153 00a9 014e 2902 da0f  .S.|.j.S...N)...
+00000720: 7469 746c 655f 666f 725f 6164 6d69 6eda  title_for_admin.
+00000730: 0574 6974 6c65 a901 721d 0000 0072 2900  .title..r....r).
+00000740: 0000 7229 0000 0072 2a00 0000 da07 5f5f  ..r)...r*.....__
+00000750: 7374 725f 5f2a 0000 0073 0600 0000 0001  str__*...s......
+00000760: 0601 0601 7a10 4d65 6e75 4974 656d 2e5f  ....z.MenuItem._
+00000770: 5f73 7472 5f5f 6301 0000 0000 0000 0000  _str__c.........
+00000780: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000790: 0c00 0000 7400 6a01 7c00 6a02 1900 5300  ....t.j.|.j...S.
+000007a0: 722c 0000 0029 0372 0400 0000 da0a 4d45  r,...).r......ME
+000007b0: 4e55 5f54 5950 4553 da09 6d65 6e75 5f74  NU_TYPES..menu_t
+000007c0: 7970 6572 2f00 0000 7229 0000 0072 2900  yper/...r)...r).
+000007d0: 0000 722a 0000 00da 0f67 6574 5f6d 656e  ..r*.....get_men
+000007e0: 755f 7061 7261 6d73 2f00 0000 7302 0000  u_params/...s...
+000007f0: 0000 017a 184d 656e 7549 7465 6d2e 6765  ...z.MenuItem.ge
+00000800: 745f 6d65 6e75 5f70 6172 616d 734e 2928  t_menu_paramsN)(
+00000810: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+00000820: 075f 5f64 6f63 5f5f 7203 0000 00da 0943  .__doc__r......C
+00000830: 6861 7246 6965 6c64 722d 0000 0072 2e00  harFieldr-...r..
+00000840: 0000 da09 4669 6c65 4669 656c 6472 0600  ....FileFieldr..
+00000850: 0000 720c 0000 0072 0d00 0000 5a04 6963  ..r....r....Z.ic
+00000860: 6f6e 7204 0000 00da 1143 484f 4943 455f  onr......CHOICE_
+00000870: 4d45 4e55 5f54 5950 4553 7232 0000 00da  MENU_TYPESr2....
+00000880: 0c42 6f6f 6c65 616e 4669 656c 64da 0969  .BooleanField..i
+00000890: 735f 6163 7469 7665 5a0c 7461 7267 6574  s_activeZ.target
+000008a0: 5f62 6c61 6e6b da0d 4461 7465 5469 6d65  _blank..DateTime
+000008b0: 4669 656c 64da 0a63 7265 6174 6564 5f61  Field..created_a
+000008c0: 74da 0a75 7064 6174 6564 5f61 74da 0c49  t..updated_at..I
+000008d0: 6e74 6567 6572 4669 656c 6472 2200 0000  ntegerFieldr"...
+000008e0: 7208 0000 00da 0743 4153 4341 4445 da06  r......CASCADE..
+000008f0: 7061 7265 6e74 da0f 4d61 6e79 546f 4d61  parent..ManyToMa
+00000900: 6e79 4669 656c 6472 0200 0000 7205 0000  nyFieldr....r...
+00000910: 00da 0573 6974 6573 5a0a 6973 5f63 7572  ...sitesZ.is_cur
+00000920: 7265 6e74 5a0f 6973 5f63 7572 7265 6e74  rentZ.is_current
+00000930: 5f66 756c 6c72 0900 0000 5a0e 6163 7469  _fullr....Z.acti
+00000940: 7665 5f6d 616e 6167 6572 720e 0000 00da  ve_managerr.....
+00000950: 076f 6e5f 7369 7465 722b 0000 0072 3000  .on_siter+...r0.
+00000960: 0000 7233 0000 0072 2900 0000 7229 0000  ..r3...r)...r)..
+00000970: 0072 2900 0000 722a 0000 0072 0f00 0000  .r)...r*...r....
+00000980: 0d00 0000 7332 0000 0008 0104 0312 010e  ....s2..........
+00000990: 0104 0102 0002 0002 0002 0106 fe06 0414  ................
+000009a0: 010e 010e 010e 010e 0110 0118 0110 0104  ................
+000009b0: 0104 0106 0106 020e 0608 0572 0f00 0000  ...........r....
+000009c0: 4e29 165a 1b64 6a61 6e67 6f2e 636f 6e74  N).Z.django.cont
+000009d0: 7269 622e 7369 7465 732e 6d6f 6465 6c73  rib.sites.models
+000009e0: 7202 0000 00da 0964 6a61 6e67 6f2e 6462  r......django.db
+000009f0: 7203 0000 00da 0b64 6a61 6e67 6f2e 636f  r......django.co
+00000a00: 6e66 7204 0000 005a 1b67 6172 7069 785f  nfr....Z.garpix_
+00000a10: 7061 6765 2e75 7469 6c73 2e61 6c6c 5f73  page.utils.all_s
+00000a20: 6974 6573 7205 0000 005a 1167 6172 7069  itesr....Z.garpi
+00000a30: 785f 7574 696c 732e 6669 6c65 7206 0000  x_utils.filer...
+00000a40: 00da 0b6d 7074 742e 6d6f 6465 6c73 7207  ...mptt.modelsr.
+00000a50: 0000 0072 0800 0000 5a15 6761 7270 6978  ...r....Z.garpix
+00000a60: 5f75 7469 6c73 2e6d 616e 6167 6572 7372  _utils.managersr
+00000a70: 0900 0000 da06 6d69 7869 6e73 720b 0000  ......mixinsr...
+00000a80: 0072 1800 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000a90: 720e 0000 0072 0f00 0000 7229 0000 0072  r....r....r)...r
+00000aa0: 2900 0000 7229 0000 0072 2a00 0000 da08  )...r)...r*.....
+00000ab0: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
+00000ac0: 000c 010c 010c 010c 010c 0110 010c 010c  ................
+00000ad0: 0110 010c 03                             .....
```

### Comparing `garpix_menu-1.8.0/garpix_menu/models/menu_item.py` & `garpix_menu-1.9.0/garpix_menu/models/menu_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from django.contrib.sites.models import Site
 from django.db import models
 from django.conf import settings
+from garpix_page.utils.all_sites import get_all_sites
 from garpix_utils.file import get_file_path
 from mptt.models import MPTTModel, TreeForeignKey
 from garpix_utils.managers import ActiveManager
 from ..mixins import LinkMixin
 from ..validators import validate_type, validate_size
+from garpix_utils.managers import GCurrentSiteManager
 
 
 class MenuItem(LinkMixin, MPTTModel):
     """
     Пункты меню.
     """
     title_for_admin = models.CharField(max_length=100, blank=True, default='', verbose_name='Название для админа')
@@ -20,17 +23,19 @@
     menu_type = models.CharField(default='', max_length=100, choices=settings.CHOICE_MENU_TYPES, verbose_name='Тип меню')
     is_active = models.BooleanField(default=True, verbose_name='Включено')
     target_blank = models.BooleanField(default=False, verbose_name='Открывать в новом окне')
     created_at = models.DateTimeField(auto_now_add=True, verbose_name='Дата создания')
     updated_at = models.DateTimeField(auto_now=True, verbose_name='Дата изменения')
     sort = models.IntegerField(default=100, verbose_name='Сортировка', help_text='Чем меньше число, тем выше будет элемент в списке.')
     parent = TreeForeignKey('self', null=True, blank=True, related_name='children', db_index=True, verbose_name='Родительский пункт меню', on_delete=models.CASCADE)
+    sites = models.ManyToManyField(Site, default=get_all_sites, verbose_name='Сайты для отображения')
     is_current = False
     is_current_full = False
     active_manager = ActiveManager()
+    on_site = GCurrentSiteManager()
 
     class Meta:
         verbose_name = 'Пункт меню'
         verbose_name_plural = 'Пункты меню'
         ordering = ('sort', )
         abstract = False
```

### Comparing `garpix_menu-1.8.0/garpix_menu/setup.py` & `garpix_menu-1.9.0/garpix_menu/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_menu')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_menu',
-    version='1.8.0',
+    version='1.9.0',
     description='',
     long_description=long_description,
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(),
     classifiers=[
@@ -29,10 +29,11 @@
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-mptt >= 0.9.1',
         'django-modeltranslation >= 0.16.2',
-        'garpix_page >= 1.0.0',
+        'garpix_page >= 2.25.0',
+        'garpix_utils >= 1.5.0'
     ],
 )
```

### Comparing `garpix_menu-1.8.0/garpix_menu/utils.py` & `garpix_menu-1.9.0/garpix_menu/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,12 +32,12 @@
                     menu_item.is_current = True
             menus[menu_type_arr[0]].append(model_to_dict(menu_item))
             menus[menu_type_arr[0]][-1]['get_link'] = link
             menus[menu_type_arr[0]][-1]['is_current'] = menu_item.is_current
             menus[menu_type_arr[0]][-1]['is_current_full'] = menu_item.is_current_full
             try:
                 menus[menu_type_arr[0]][-1]['icon'] = menu_item.icon.url
-            except:
+            except Exception:
                 menus[menu_type_arr[0]][-1]['icon'] = None
             menus[menu_type_arr[0]][-1].pop('page', None)
             menus[menu_type_arr[0]][-1].pop('title_for_admin', None)
     return menus
```

### Comparing `garpix_menu-1.8.0/garpix_menu/validators.py` & `garpix_menu-1.9.0/garpix_menu/validators.py`

 * *Files identical despite different names*

### Comparing `garpix_menu-1.8.0/garpix_menu.egg-info/PKG-INFO` & `garpix_menu-1.9.0/garpix_menu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-menu
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: garpix-menu Version: 1.8.0 Summary: UNKNOWN Home-
+Metadata-Version: 2.1 Name: garpix-menu Version: 1.9.0 Summary: UNKNOWN Home-
 page: UNKNOWN Author: Garpix LTD Author-email: info@garpix.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
 Environment :: Web Environment Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Framework :: Django Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `garpix_menu-1.8.0/garpix_menu.egg-info/SOURCES.txt` & `garpix_menu-1.9.0/garpix_menu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 garpix_menu.egg-info/not-zip-safe
 garpix_menu.egg-info/requires.txt
 garpix_menu.egg-info/top_level.txt
 garpix_menu/__pycache__/__init__.cpython-38.pyc
 garpix_menu/__pycache__/apps.cpython-38.pyc
 garpix_menu/__pycache__/context_processors.cpython-38.pyc
 garpix_menu/__pycache__/tests.cpython-38.pyc
+garpix_menu/__pycache__/utils.cpython-38.pyc
 garpix_menu/__pycache__/validators.cpython-38.pyc
 garpix_menu/admin/__init__.py
 garpix_menu/admin/menu_item.py
 garpix_menu/admin/__pycache__/__init__.cpython-38.pyc
 garpix_menu/admin/__pycache__/menu_item.cpython-38.pyc
 garpix_menu/mixins/__init__.py
 garpix_menu/mixins/link_mixin.py
```

### Comparing `garpix_menu-1.8.0/setup.py` & `garpix_menu-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_menu')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_menu',
-    version='1.8.0',
+    version='1.9.0',
     description='',
     long_description=long_description,
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(),
     classifiers=[
@@ -29,10 +29,11 @@
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-mptt >= 0.9.1',
         'django-modeltranslation >= 0.16.2',
-        'garpix_page >= 1.0.0',
+        'garpix_page >= 2.25.0',
+        'garpix_utils >= 1.5.0'
     ],
 )
```

