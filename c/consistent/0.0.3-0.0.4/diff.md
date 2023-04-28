# Comparing `tmp/consistent-0.0.3.tar.gz` & `tmp/consistent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistent-0.0.3.tar", last modified: Fri Apr 28 08:57:13 2023, max compression
+gzip compressed data, was "consistent-0.0.4.tar", last modified: Fri Apr 28 09:02:21 2023, max compression
```

## Comparing `consistent-0.0.3.tar` & `consistent-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 08:57:01.000000 consistent-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 08:57:13.945818 consistent-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 08:57:01.000000 consistent-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.941818 consistent-0.0.3/consisTent/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/cache/chroma_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/base_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consisTent/validators/semantic_validators/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/consistency_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/semantic_validators/labels_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 08:57:01.000000 consistent-0.0.3/consisTent/validators/syntactic_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/consistent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 08:57:13.000000 consistent-0.0.3/consistent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 08:57:01.000000 consistent-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:57:13.945818 consistent-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:57:13.945818 consistent-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 08:57:01.000000 consistent-0.0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.181751 consistent-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 09:02:04.000000 consistent-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 09:02:21.181751 consistent-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 09:02:04.000000 consistent-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.177750 consistent-0.0.4/consisTent/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.177750 consistent-0.0.4/consisTent/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/cache/chroma_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.177750 consistent-0.0.4/consisTent/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/base_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.177750 consistent-0.0.4/consisTent/validators/semantic_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/semantic_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/semantic_validators/consistency_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/semantic_validators/labels_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 09:02:04.000000 consistent-0.0.4/consisTent/validators/syntactic_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.181751 consistent-0.0.4/consistent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 09:02:21.000000 consistent-0.0.4/consistent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-28 09:02:21.000000 consistent-0.0.4/consistent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:02:21.000000 consistent-0.0.4/consistent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 09:02:21.000000 consistent-0.0.4/consistent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:02:21.000000 consistent-0.0.4/consistent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 09:02:04.000000 consistent-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:02:21.181751 consistent-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:02:21.181751 consistent-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 09:02:04.000000 consistent-0.0.4/tests/test.py
```

### Comparing `consistent-0.0.3/LICENSE` & `consistent-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/PKG-INFO` & `consistent-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `consistent-0.0.3/consisTent/cache/chroma_cache.py` & `consistent-0.0.4/consisTent/cache/chroma_cache.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/consisTent/validators/semantic_validators/consistency_validator.py` & `consistent-0.0.4/consisTent/validators/semantic_validators/consistency_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/consisTent/validators/semantic_validators/labels_validator.py` & `consistent-0.0.4/consisTent/validators/semantic_validators/labels_validator.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/consisTent/validators/syntactic_validators.py` & `consistent-0.0.4/consisTent/validators/syntactic_validators.py`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/consistent.egg-info/PKG-INFO` & `consistent-0.0.4/consistent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consistent
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make sure AI model outputs are consistent
 License: MIT License
         
         Copyright (c) 2023 drorIvry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `consistent-0.0.3/consistent.egg-info/SOURCES.txt` & `consistent-0.0.4/consistent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consistent-0.0.3/pyproject.toml` & `consistent-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "consistent"
-version = "0.0.3"
+version = "0.0.4"
 description = "Make sure AI model outputs are consistent"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -30,15 +30,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "pre-commit", "pyflakes"]
 
 [project.urls]
 Homepage = "https://github.com/drorivry/consistent"
 
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

