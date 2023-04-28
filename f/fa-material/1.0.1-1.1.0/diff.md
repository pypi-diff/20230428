# Comparing `tmp/fa_material-1.0.1.tar.gz` & `tmp/fa_material-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa_material-1.0.1.tar", max compression
+gzip compressed data, was "fa_material-1.1.0.tar", max compression
```

## Comparing `fa_material-1.0.1.tar` & `fa_material-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2023-04-27 23:41:31.236428 fa_material-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1767 2023-04-27 23:41:31.236428 fa_material-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 23:41:31.236428 fa_material-1.0.1/fa_material/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-27 23:41:31.236428 fa_material-1.0.1/fa_material/plugin.py
--rw-r--r--   0        0        0      839 2023-04-27 23:41:31.240429 fa_material-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 fa_material-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-28 02:35:09.741199 fa_material-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2014 2023-04-28 02:35:09.741199 fa_material-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 02:35:09.741199 fa_material-1.1.0/fa_material/__init__.py
+-rw-r--r--   0        0        0     1767 2023-04-28 02:35:09.741199 fa_material-1.1.0/fa_material/plugin.py
+-rw-r--r--   0        0        0      912 2023-04-28 02:35:09.741199 fa_material-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 fa_material-1.1.0/PKG-INFO
```

### Comparing `fa_material-1.0.1/LICENSE.md` & `fa_material-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fa_material-1.0.1/README.md` & `fa_material-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -29,10 +29,22 @@
   - fontawesome-pro
 ```
 
 That's it. You can now use Font Awesome Pro icons in the same way you already do Font Awesome Free icons (e.g.
 `:fontawesome-thin-user-secret:`). They'll work in Markdown files, `mkdocs.yml`, and anywhere else Material for MkDocs'
 icon system is used.
 
+### Font Awesome 5
+
+You can use Font Awesome 5 with fa-material by setting `fontawesome-pro`'s `version` option to `5`.
+
+```yaml
+plugins:
+  - fontawesome-pro:
+      version: 5
+```
+
+This option must be either `5` or `6`, defaulting to the latter.
+
 ## License
 
 fa-material is licensed under the [MIT License](LICENSE.md).
```

### Comparing `fa_material-1.0.1/PKG-INFO` & `fa_material-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fa-material
-Version: 1.0.1
+Version: 1.1.0
 Summary: Font Awesome Pro + Material for MkDocs
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
+Requires-Dist: fontawesome-pro (>=5.15.4,<6.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: path (>=16.6.0,<17.0.0)
 Description-Content-Type: text/markdown
 
 # fa-material
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fa-material?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/fa-material)
@@ -49,11 +50,23 @@
   - fontawesome-pro
 ```
 
 That's it. You can now use Font Awesome Pro icons in the same way you already do Font Awesome Free icons (e.g.
 `:fontawesome-thin-user-secret:`). They'll work in Markdown files, `mkdocs.yml`, and anywhere else Material for MkDocs'
 icon system is used.
 
+### Font Awesome 5
+
+You can use Font Awesome 5 with fa-material by setting `fontawesome-pro`'s `version` option to `5`.
+
+```yaml
+plugins:
+  - fontawesome-pro:
+      version: 5
+```
+
+This option must be either `5` or `6`, defaulting to the latter.
+
 ## License
 
 fa-material is licensed under the [MIT License](LICENSE.md).
```

