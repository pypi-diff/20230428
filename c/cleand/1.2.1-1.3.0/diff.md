# Comparing `tmp/cleand-1.2.1.tar.gz` & `tmp/cleand-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleand-1.2.1.tar", last modified: Mon Sep 12 15:05:33 2022, max compression
+gzip compressed data, was "cleand-1.3.0.tar", last modified: Fri Apr 28 12:15:42 2023, max compression
```

## Comparing `cleand-1.2.1.tar` & `cleand-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 15:05:33.087182 cleand-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-12 15:05:22.000000 cleand-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-09-12 15:05:33.087182 cleand-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-09-12 15:05:22.000000 cleand-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 15:05:33.087182 cleand-1.2.1/cleand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-09-12 15:05:33.000000 cleand-1.2.1/cleand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-12 15:05:33.000000 cleand-1.2.1/cleand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 15:05:33.000000 cleand-1.2.1/cleand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-12 15:05:33.000000 cleand-1.2.1/cleand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 15:05:33.087182 cleand-1.2.1/cleaned/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16361 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    16677 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-12 15:05:22.000000 cleand-1.2.1/cleaned/version.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-12 15:05:22.000000 cleand-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 15:05:33.087182 cleand-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-09-12 15:05:22.000000 cleand-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:42.637434 cleand-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 12:15:33.000000 cleand-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-28 12:15:42.637434 cleand-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-28 12:15:33.000000 cleand-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:42.633434 cleand-1.3.0/cleand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-28 12:15:42.000000 cleand-1.3.0/cleand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 12:15:42.000000 cleand-1.3.0/cleand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:15:42.000000 cleand-1.3.0/cleand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:15:42.000000 cleand-1.3.0/cleand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:42.637434 cleand-1.3.0/cleaned/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25132 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:15:33.000000 cleand-1.3.0/cleaned/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 12:15:33.000000 cleand-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:15:42.637434 cleand-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-28 12:15:33.000000 cleand-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:15:42.637434 cleand-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-04-28 12:15:33.000000 cleand-1.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-28 12:15:33.000000 cleand-1.3.0/tests/test_fields.py
```

### Comparing `cleand-1.2.1/LICENSE` & `cleand-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleand-1.2.1/PKG-INFO` & `cleand-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleand
-Version: 1.2.1
+Version: 1.3.0
 Summary: a declarative data validator
 Home-page: https://github.com/saryou/cleaned
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/cleaned/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cleand-1.2.1/README.md` & `cleand-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cleand-1.2.1/cleand.egg-info/PKG-INFO` & `cleand-1.3.0/cleand.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleand
-Version: 1.2.1
+Version: 1.3.0
 Summary: a declarative data validator
 Home-page: https://github.com/saryou/cleaned
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/cleaned/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cleand-1.2.1/cleaned/__init__.py` & `cleand-1.3.0/cleaned/__init__.py`

 * *Files identical despite different names*

### Comparing `cleand-1.2.1/cleaned/errors.py` & `cleand-1.3.0/cleaned/errors.py`

 * *Files identical despite different names*

### Comparing `cleand-1.2.1/cleaned/fields.py` & `cleand-1.3.0/cleaned/fields.py`

 * *Files identical despite different names*

### Comparing `cleand-1.2.1/setup.py` & `cleand-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,11 +19,12 @@
         "Bug Tracker": "https://github.com/saryou/cleaned/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=["cleaned"],
+    packages=setuptools.find_packages(exclude=["tests"]),
     package_dir={"cleaned": "cleaned"},
+    package_data={"cleaned": ["py.typed"]},
     python_requires=">=3.8",
 )
```

