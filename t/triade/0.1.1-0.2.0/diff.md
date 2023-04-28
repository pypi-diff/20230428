# Comparing `tmp/triade-0.1.1.tar.gz` & `tmp/triade-0.2.0.tar.gz`

## Comparing `triade-0.1.1.tar` & `triade-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 triade-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.1.1/triade/__init__.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triade-0.1.1/triade/cli.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 triade-0.1.1/triade/lib.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 triade-0.1.1/.gitignore
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.1.1/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 triade-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 triade-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 triade-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triade-0.2.0/triade/__init__.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triade-0.2.0/triade/cli.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 triade-0.2.0/triade/lib.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 triade-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 triade-0.2.0/LICENSE
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 triade-0.2.0/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 triade-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 triade-0.2.0/PKG-INFO
```

### Comparing `triade-0.1.1/triade/cli.py` & `triade-0.2.0/triade/cli.py`

 * *Files identical despite different names*

### Comparing `triade-0.1.1/pyproject.toml` & `triade-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Makefile",
     "dev_requirements.txt",
     ".?*",
 ]
 
 [project]
 name = "triade"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Lucas L. S. Haine", email="lucaslshaine@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `triade-0.1.1/PKG-INFO` & `triade-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: triade
-Version: 0.1.1
+Version: 0.2.0
 Project-URL: Homepage, https://github.com/llucasls/triade
 Author-email: "Lucas L. S. Haine" <lucaslshaine@gmail.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pyyaml
 Requires-Dist: toml
 Description-Content-Type: text/markdown
```

