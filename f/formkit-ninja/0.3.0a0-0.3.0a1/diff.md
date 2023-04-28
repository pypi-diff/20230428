# Comparing `tmp/formkit_ninja-0.3.0a0.tar.gz` & `tmp/formkit_ninja-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.3.0a0.tar", max compression
+gzip compressed data, was "formkit_ninja-0.3.0a1.tar", max compression
```

## Comparing `formkit_ninja-0.3.0a0.tar` & `formkit_ninja-0.3.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a0/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a0/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a0/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14754 2023-04-26 06:27:35.615331 formkit_ninja-0.3.0a0/formkit_ninja/admin.py
--rw-r--r--   0        0        0     1714 2023-04-26 06:10:12.439548 formkit_ninja-0.3.0a0/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.0a0/formkit_ninja/fields.py
--rw-r--r--   0        0        0    13135 2023-04-13 06:01:40.565549 formkit_ninja-0.3.0a0/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.0a0/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a0/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3955 2023-04-26 06:10:12.528997 formkit_ninja-0.3.0a0/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19101 2023-04-26 06:35:40.064339 formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15058 2023-04-26 08:00:47.228814 formkit_ninja-0.3.0a0/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.0a0/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0    11459 2023-04-26 06:10:12.671301 formkit_ninja-0.3.0a0/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a0/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1201 2023-04-26 08:36:38.027669 formkit_ninja-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a1/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14754 2023-04-26 06:27:35.615331 formkit_ninja-0.3.0a1/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     1714 2023-04-26 06:10:12.439548 formkit_ninja-0.3.0a1/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.0a1/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    13135 2023-04-13 06:01:40.565549 formkit_ninja-0.3.0a1/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.0a1/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3955 2023-04-26 06:10:12.528997 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19101 2023-04-26 06:35:40.064339 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15058 2023-04-26 08:00:47.228814 formkit_ninja-0.3.0a1/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.0a1/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0    11459 2023-04-26 06:10:12.671301 formkit_ninja-0.3.0a1/formkit_ninja/models.py
+-rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a1/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1201 2023-04-28 02:14:47.604734 formkit_ninja-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.3.0a1/PKG-INFO
```

### Comparing `formkit_ninja-0.3.0a0/README.md` & `formkit_ninja-0.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/admin.py` & `formkit_ninja-0.3.0a1/formkit_ninja/admin.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/api.py` & `formkit_ninja-0.3.0a1/formkit_ninja/api.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/fields.py` & `formkit_ninja-0.3.0a1/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.3.0a1/formkit_ninja/formkit_schema.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/common_nodes.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.3.0a1/formkit_ninja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/formkit_ninja/models.py` & `formkit_ninja-0.3.0a1/formkit_ninja/models.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a0/pyproject.toml` & `formkit_ninja-0.3.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.3.0a0"
+version = "0.3.0a1"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
```

### Comparing `formkit_ninja-0.3.0a0/PKG-INFO` & `formkit_ninja-0.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

