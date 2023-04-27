# Comparing `tmp/redvox-base-2023.4.25.tar.gz` & `tmp/redvox-base-2023.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-base-2023.4.25.tar", last modified: Wed Apr 26 01:02:13 2023, max compression
+gzip compressed data, was "redvox-base-2023.4.27.tar", last modified: Thu Apr 27 23:30:52 2023, max compression
```

## Comparing `redvox-base-2023.4.25.tar` & `redvox-base-2023.4.27.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-26 01:02:13.800350 redvox-base-2023.4.25/
--rw-r--r--   0 opq       (1000) opq       (1000)       34 2023-04-24 23:40:14.000000 redvox-base-2023.4.25/.gitignore
--rw-r--r--   0 opq       (1000) opq       (1000)      491 2023-04-26 01:02:13.800350 redvox-base-2023.4.25/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)      892 2023-04-26 01:01:45.000000 redvox-base-2023.4.25/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-26 01:02:13.800350 redvox-base-2023.4.25/redvox_base/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-24 23:46:52.000000 redvox-base-2023.4.25/redvox_base/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-26 01:02:13.800350 redvox-base-2023.4.25/redvox_base.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)      491 2023-04-26 01:02:13.000000 redvox-base-2023.4.25/redvox_base.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)      223 2023-04-26 01:02:13.000000 redvox-base-2023.4.25/redvox_base.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-26 01:02:13.000000 redvox-base-2023.4.25/redvox_base.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      463 2023-04-26 01:02:13.000000 redvox-base-2023.4.25/redvox_base.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       12 2023-04-26 01:02:13.000000 redvox-base-2023.4.25/redvox_base.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-26 01:02:13.800350 redvox-base-2023.4.25/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:30:52.814760 redvox-base-2023.4.27/
+-rw-r--r--   0 opq       (1000) opq       (1000)       34 2023-04-24 23:40:14.000000 redvox-base-2023.4.27/.gitignore
+-rw-r--r--   0 opq       (1000) opq       (1000)      491 2023-04-27 23:30:52.814760 redvox-base-2023.4.27/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      954 2023-04-27 23:29:55.000000 redvox-base-2023.4.27/pyproject.toml
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:30:52.813760 redvox-base-2023.4.27/redvox_base/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-24 23:46:52.000000 redvox-base-2023.4.27/redvox_base/__init__.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:30:52.813760 redvox-base-2023.4.27/redvox_base.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)      491 2023-04-27 23:30:52.000000 redvox-base-2023.4.27/redvox_base.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      223 2023-04-27 23:30:52.000000 redvox-base-2023.4.27/redvox_base.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:30:52.000000 redvox-base-2023.4.27/redvox_base.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      504 2023-04-27 23:30:52.000000 redvox-base-2023.4.27/redvox_base.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       12 2023-04-27 23:30:52.000000 redvox-base-2023.4.27/redvox_base.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:30:52.814760 redvox-base-2023.4.27/setup.cfg
```

### Comparing `redvox-base-2023.4.25/pyproject.toml` & `redvox-base-2023.4.27/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redvox-base"
-version = "2023.4.25"
+version = "2023.4.27"
 authors = [
     { name = "RedVox, Inc" }
 ]
 description = "Specifies base dependencies used by multiple RedVox, Inc projects."
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
@@ -16,19 +16,22 @@
     "pylint==2.17.3",
     "mypy==1.2.0",
     "pdoc3==0.10.0",
     "coverage==7.2.3",
     "twine==4.0.2",
     "wheel==0.40.0",
     "build==0.10.0",
+    "toml==0.10.2",
+    "tomli==2.0.1",
+    "tomli-w==1.0.0",
 ]
 keras = ["keras==2.12.0"]
 lz4 = ["lz4==4.3.2"]
 matplotlib = ["matplotlib==3.7.1"]
-numpy = ["numpy==1.24.3"]
+numpy = ["numpy==1.23.5"]
 pandas = ["pandas==2.0.1"]
 protobuf = ["protobuf==4.22.3"]
 pyserde = ["pyserde==0.10.4"]
 scikit-learn = ["scikit-learn==1.2.2"]
 scipy = ["scipy==1.10.1"]
 tensorflow = ["tensorflow==2.12.0"]
 tensorflow-hub = ["tensorflow-hub==0.13.0"]
```

