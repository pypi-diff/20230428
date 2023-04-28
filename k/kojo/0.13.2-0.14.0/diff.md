# Comparing `tmp/kojo-0.13.2.tar.gz` & `tmp/kojo-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojo-0.13.2.tar", last modified: Thu Apr 27 09:59:26 2023, max compression
+gzip compressed data, was "kojo-0.14.0.tar", last modified: Fri Apr 28 09:50:17 2023, max compression
```

## Comparing `kojo-0.13.2.tar` & `kojo-0.14.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-27 09:59:26.046955 kojo-0.13.2/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      612 2023-04-27 09:59:26.046955 kojo-0.13.2/PKG-INFO
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-27 09:59:26.046955 kojo-0.13.2/kojo/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.13.2/kojo/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      454 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/duplicatefinder.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2197 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/io.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     3451 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/item.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      952 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/jsonschemavalidator.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      962 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/process.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1844 2023-04-27 08:31:58.877706 kojo-0.13.2/kojo/propertiesconverter.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.13.2/setup.cfg
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      743 2023-04-27 09:56:58.116884 kojo-0.13.2/setup.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-28 09:50:17.305655 kojo-0.14.0/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      612 2023-04-28 09:50:17.305655 kojo-0.14.0/PKG-INFO
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-04-28 09:50:17.305655 kojo-0.14.0/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.14.0/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      454 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/duplicatefinder.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2197 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/io.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3451 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      947 2023-04-28 09:46:09.112495 kojo-0.14.0/kojo/jsonschemavalidator.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      962 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/process.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1844 2023-04-27 08:31:58.877706 kojo-0.14.0/kojo/propertiesconverter.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.14.0/setup.cfg
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      743 2023-04-28 09:48:06.255154 kojo-0.14.0/setup.py
```

### Comparing `kojo-0.13.2/PKG-INFO` & `kojo-0.14.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: kojo
-Version: 0.13.2
+Version: 0.14.0
 Summary: A library to transform data through a pipeline
 Home-page: https://gitlab.com/filchos/kojo
 Author: Olaf Schneider
 Author-email: mail@olafschneider.com
 License: GNU GPLv3
-Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.13.2/kojo-0.13.2.tar.gz
+Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.14.0/kojo-0.14.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kojo-0.13.2/kojo/io.py` & `kojo-0.14.0/kojo/io.py`

 * *Files identical despite different names*

### Comparing `kojo-0.13.2/kojo/item.py` & `kojo-0.14.0/kojo/item.py`

 * *Files identical despite different names*

### Comparing `kojo-0.13.2/kojo/jsonschemavalidator.py` & `kojo-0.14.0/kojo/jsonschemavalidator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import json
-from jsonschema import Draft7Validator, exceptions, RefResolver
+from jsonschema import Draft7Validator, RefResolver
 
 
 class JSONSchemaValidator:
     def __init__(self, schema, schema_dir=None):
         self.schema = schema
 
         if schema_dir:
             base_uri = "file://" + schema_dir + "/"
             resolver = RefResolver(base_uri, None)
             self.validator = Draft7Validator(self.schema, resolver=resolver)
         else:
             self.validator = Draft7Validator(self.schema)
 
     def __call__(self, item):
-        try:
-            self.validator.validate(item)
-        except exceptions.ValidationError as e:
+        for err in self.validator.iter_errors(item):
             item.log.error(
-                "Validation error",
-                error=type(e).__name__,
-                message=str(e),
-                path=e.json_path,
+                "JSON Schema validation error",
+                message=err.message,
+                path=list(err.path),
+                validator=err.validator,
+                value=err.instance,
             )
         return item
 
     @classmethod
     def load(cls, schema_path, schema_dir=None):
         with open(schema_path) as fp:
             return cls(json.load(fp), schema_dir)
```

### Comparing `kojo-0.13.2/kojo/process.py` & `kojo-0.14.0/kojo/process.py`

 * *Files identical despite different names*

### Comparing `kojo-0.13.2/kojo/propertiesconverter.py` & `kojo-0.14.0/kojo/propertiesconverter.py`

 * *Files identical despite different names*

### Comparing `kojo-0.13.2/setup.py` & `kojo-0.14.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name="kojo",
     packages=["kojo"],
-    version="0.13.2",
+    version="0.14.0",
     license="GNU GPLv3",
     description="A library to transform data through a pipeline",
     author="Olaf Schneider",
     author_email="mail@olafschneider.com",
     url="https://gitlab.com/filchos/kojo",
-    download_url="https://gitlab.com/filchos/kojo/-/archive/0.13.2/kojo-0.13.2.tar.gz",
+    download_url="https://gitlab.com/filchos/kojo/-/archive/0.14.0/kojo-0.14.0.tar.gz",
     install_requires=["jsonschema"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
```

