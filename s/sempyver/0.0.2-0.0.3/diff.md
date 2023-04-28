# Comparing `tmp/sempyver-0.0.2.tar.gz` & `tmp/sempyver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sempyver-0.0.2.tar", last modified: Fri Apr 28 08:51:16 2023, max compression
+gzip compressed data, was "sempyver-0.0.3.tar", last modified: Fri Apr 28 08:58:14 2023, max compression
```

## Comparing `sempyver-0.0.2.tar` & `sempyver-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.226146 sempyver-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 08:51:02.000000 sempyver-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:51:16.222145 sempyver-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 08:51:02.000000 sempyver-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 08:51:02.000000 sempyver-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/cli_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/changelog_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/changeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/modules/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver/cli_application/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/tags_for_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 08:51:02.000000 sempyver-0.0.2/sempyver/cli_application/utilities/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:51:16.222145 sempyver-0.0.2/sempyver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 08:51:16.000000 sempyver-0.0.2/sempyver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:51:16.226146 sempyver-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 08:51:02.000000 sempyver-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 08:58:04.000000 sempyver-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:58:14.685491 sempyver-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 08:58:04.000000 sempyver-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-28 08:58:04.000000 sempyver-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/cli_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver/cli_application/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/modules/changelog_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/modules/changeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/modules/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver/cli_application/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/utilities/tags_for_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/cli_application/utilities/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-28 08:58:04.000000 sempyver-0.0.3/sempyver/helpers/cache_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:58:14.685491 sempyver-0.0.3/sempyver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 08:58:14.000000 sempyver-0.0.3/sempyver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:58:14.685491 sempyver-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 08:58:04.000000 sempyver-0.0.3/setup.py
```

### Comparing `sempyver-0.0.2/LICENSE` & `sempyver-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/PKG-INFO` & `sempyver-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sempyver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for teams to manage the CHANGELOG given a list of different changes.
 Home-page: 
 Author: Ricardo Leal
 Author-email: ricardo.lealpz@gmail.com
 Maintainer: Ricardo Leal
 Maintainer-email: ricardo.lealpz@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sempyver-0.0.2/README.md` & `sempyver-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/pyproject.toml` & `sempyver-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/cli_app.py` & `sempyver-0.0.3/sempyver/cli_application/cli_app.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/modules/changelog_generator.py` & `sempyver-0.0.3/sempyver/cli_application/modules/changelog_generator.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/modules/changeset.py` & `sempyver-0.0.3/sempyver/cli_application/modules/changeset.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/modules/commit.py` & `sempyver-0.0.3/sempyver/cli_application/modules/commit.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/utilities/tags_for_change.py` & `sempyver-0.0.3/sempyver/cli_application/utilities/tags_for_change.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver/cli_application/utilities/theme.py` & `sempyver-0.0.3/sempyver/cli_application/utilities/theme.py`

 * *Files identical despite different names*

### Comparing `sempyver-0.0.2/sempyver.egg-info/PKG-INFO` & `sempyver-0.0.3/sempyver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sempyver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for teams to manage the CHANGELOG given a list of different changes.
 Home-page: 
 Author: Ricardo Leal
 Author-email: ricardo.lealpz@gmail.com
 Maintainer: Ricardo Leal
 Maintainer-email: ricardo.lealpz@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sempyver-0.0.2/sempyver.egg-info/SOURCES.txt` & `sempyver-0.0.3/sempyver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 sempyver/cli_application/cli_app.py
 sempyver/cli_application/modules/__init__.py
 sempyver/cli_application/modules/changelog_generator.py
 sempyver/cli_application/modules/changeset.py
 sempyver/cli_application/modules/commit.py
 sempyver/cli_application/utilities/__init__.py
 sempyver/cli_application/utilities/tags_for_change.py
-sempyver/cli_application/utilities/theme.py
+sempyver/cli_application/utilities/theme.py
+sempyver/helpers/__init__.py
+sempyver/helpers/cache_generator.py
```

### Comparing `sempyver-0.0.2/setup.py` & `sempyver-0.0.3/setup.py`

 * *Files identical despite different names*

