# Comparing `tmp/resotoeventlog-3.4.0.tar.gz` & `tmp/resotoeventlog-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoeventlog-3.4.0.tar", last modified: Thu Apr 27 11:21:25 2023, max compression
+gzip compressed data, was "resotoeventlog-3.4.1.tar", last modified: Fri Apr 28 15:17:44 2023, max compression
```

## Comparing `resotoeventlog-3.4.0.tar` & `resotoeventlog-3.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/logs/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/resotoeventlog/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/resotoeventlog/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/resotoeventlog/web/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:25.765789 resotoeventlog-3.4.0/resotoeventlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 11:21:25.000000 resotoeventlog-3.4.0/resotoeventlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 11:21:25.769789 resotoeventlog-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-27 11:19:52.000000 resotoeventlog-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/resotoeventlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/resotoeventlog/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/logs/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/resotoeventlog/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/resotoeventlog/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/resotoeventlog/web/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:44.123533 resotoeventlog-3.4.1/resotoeventlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 15:17:44.000000 resotoeventlog-3.4.1/resotoeventlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-28 15:17:44.127533 resotoeventlog-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-28 15:16:15.000000 resotoeventlog-3.4.1/setup.py
```

### Comparing `resotoeventlog-3.4.0/resotoeventlog/__main__.py` & `resotoeventlog-3.4.1/resotoeventlog/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/resotoeventlog/logs/log_handler.py` & `resotoeventlog-3.4.1/resotoeventlog/logs/log_handler.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/resotoeventlog/model.py` & `resotoeventlog-3.4.1/resotoeventlog/model.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/resotoeventlog/web/api.py` & `resotoeventlog-3.4.1/resotoeventlog/web/api.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/resotoeventlog/web/directives.py` & `resotoeventlog-3.4.1/resotoeventlog/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/resotoeventlog.egg-info/SOURCES.txt` & `resotoeventlog-3.4.1/resotoeventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/setup.cfg` & `resotoeventlog-3.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.4.0/setup.py` & `resotoeventlog-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return [str(requirement) for requirement in pkg_resources.parse_requirements(read(fname))]
 
 
 setup_requirements = ["pytest-runner"]
 
 setup(
     name="resotoeventlog",
-    version="3.4.0",
+    version="3.4.1",
     description="Event log aggregator for resoto.",
     python_requires=">=3.5",
     classifiers=["Programming Language :: Python :: 3"],
     entry_points={"console_scripts": ["resotoeventlog=resotoeventlog.__main__:main"]},
     install_requires=read_requirements("requirements.txt"),
     license="Apache Software License 2.0",
     long_description=read("README.md"),
```

