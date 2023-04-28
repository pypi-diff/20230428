# Comparing `tmp/local-database-python-backend-0.0.4.tar.gz` & `tmp/local-database-python-backend-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-database-python-backend-0.0.4.tar", last modified: Thu Apr 27 22:15:10 2023, max compression
+gzip compressed data, was "local-database-python-backend-0.0.5.tar", last modified: Fri Apr 28 03:11:18 2023, max compression
```

## Comparing `local-database-python-backend-0.0.4.tar` & `local-database-python-backend-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:15:10.386195 local-database-python-backend-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:14:59.000000 local-database-python-backend-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:15:10.386195 local-database-python-backend-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:15:10.386195 local-database-python-backend-0.0.4/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:14:59.000000 local-database-python-backend-0.0.4/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 22:14:59.000000 local-database-python-backend-0.0.4/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:15:10.386195 local-database-python-backend-0.0.4/local_database_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 22:15:10.000000 local-database-python-backend-0.0.4/local_database_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-27 22:15:10.000000 local-database-python-backend-0.0.4/local_database_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:15:10.000000 local-database-python-backend-0.0.4/local_database_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 22:15:10.000000 local-database-python-backend-0.0.4/local_database_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 22:14:59.000000 local-database-python-backend-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:15:10.386195 local-database-python-backend-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-27 22:14:59.000000 local-database-python-backend-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:11:18.765896 local-database-python-backend-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:11:07.000000 local-database-python-backend-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 03:11:18.765896 local-database-python-backend-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:11:18.765896 local-database-python-backend-0.0.5/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:11:07.000000 local-database-python-backend-0.0.5/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 03:11:07.000000 local-database-python-backend-0.0.5/circles_local_database_python/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:11:18.765896 local-database-python-backend-0.0.5/local_database_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 03:11:18.000000 local-database-python-backend-0.0.5/local_database_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-28 03:11:18.000000 local-database-python-backend-0.0.5/local_database_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:11:18.000000 local-database-python-backend-0.0.5/local_database_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 03:11:18.000000 local-database-python-backend-0.0.5/local_database_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 03:11:07.000000 local-database-python-backend-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:11:18.765896 local-database-python-backend-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-28 03:11:07.000000 local-database-python-backend-0.0.5/setup.py
```

### Comparing `local-database-python-backend-0.0.4/PKG-INFO` & `local-database-python-backend-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: local-database-python-backend
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Local Database Python
 Home-page: https://github.com/javatechy/dokr
 Author: Circles
-Author-email: info@bubbelz.life
+Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a package for sharing common Logger function used in different repositories
```

### Comparing `local-database-python-backend-0.0.4/local_database_python_backend.egg-info/PKG-INFO` & `local-database-python-backend-0.0.5/local_database_python_backend.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: local-database-python-backend
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Local Database Python
 Home-page: https://github.com/javatechy/dokr
 Author: Circles
-Author-email: info@bubbelz.life
+Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a package for sharing common Logger function used in different repositories
```

### Comparing `local-database-python-backend-0.0.4/setup.py` & `local-database-python-backend-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
-
+# used by python -m build
 setuptools.setup(
      name='local-database-python-backend',  
-     version='0.0.4',
+     version='0.0.5',
      author="Circles",
-     author_email="info@bubbelz.life",
+     author_email="info@circles.life",
      description="PyPI Package for Circles Local Database Python",
      long_description="This is a package for sharing common Logger function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
```

