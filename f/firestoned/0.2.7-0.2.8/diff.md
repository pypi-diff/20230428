# Comparing `tmp/firestoned-0.2.7.tar.gz` & `tmp/firestoned-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.2.7.tar", max compression
+gzip compressed data, was "firestoned-0.2.8.tar", max compression
```

## Comparing `firestoned-0.2.7.tar` & `firestoned-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-04-28 01:16:21.996657 firestoned-0.2.7/LICENSE
--rw-r--r--   0        0        0     9344 2023-04-28 01:16:21.996657 firestoned-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/__init__.py
--rw-r--r--   0        0        0     4872 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/__main__.py
--rw-r--r--   0        0        0     2045 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/resource.py
--rw-r--r--   0        0        0        0 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     6151 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      408 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      175 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/__init__.py
--rw-r--r--   0        0        0      866 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/_base.py
--rw-r--r--   0        0        0    13390 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9184 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/cli.py
--rw-r--r--   0        0        0    16187 2023-04-28 01:16:22.004658 firestoned-0.2.7/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1683 2023-04-28 01:16:22.004658 firestoned-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 firestoned-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 01:24:07.908996 firestoned-0.2.8/LICENSE
+-rw-r--r--   0        0        0     9344 2023-04-28 01:24:07.908996 firestoned-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/__init__.py
+-rw-r--r--   0        0        0     4872 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/__main__.py
+-rw-r--r--   0        0        0     2045 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/resource.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-28 01:24:07.908996 firestoned-0.2.8/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     6151 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      408 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      175 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13390 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9184 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/cli.py
+-rw-r--r--   0        0        0    16187 2023-04-28 01:24:07.912996 firestoned-0.2.8/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1683 2023-04-28 01:24:07.912996 firestoned-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 firestoned-0.2.8/PKG-INFO
```

### Comparing `firestoned-0.2.7/LICENSE` & `firestoned-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/README.md` & `firestoned-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/__main__.py` & `firestoned-0.2.8/firestone/__main__.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/resource.py` & `firestoned-0.2.8/firestone/resource.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/schema/main.py.jinja2` & `firestoned-0.2.8/firestone/schema/main.py.jinja2`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/schema/resource.yaml` & `firestoned-0.2.8/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/spec/_base.py` & `firestoned-0.2.8/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/spec/asyncapi.py` & `firestoned-0.2.8/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/spec/cli.py` & `firestoned-0.2.8/firestone/spec/cli.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/firestone/spec/openapi.py` & `firestoned-0.2.8/firestone/spec/openapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.2.7/pyproject.toml` & `firestoned-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.2.7"
+version = "0.2.8"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
```

### Comparing `firestoned-0.2.7/PKG-INFO` & `firestoned-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.2.7
+Version: 0.2.8
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.2.7 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.2.8 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.8,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: caching
```

