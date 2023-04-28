# Comparing `tmp/rwexptest-0.0.2.tar.gz` & `tmp/rwexptest-0.0.3.tar.gz`

## Comparing `rwexptest-0.0.2.tar` & `rwexptest-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rwexptest-0.0.2/RWexptest/_init_.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 rwexptest-0.0.2/RWexptest/example.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 rwexptest-0.0.2/RWexptest/toml.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rwexptest-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rwexptest-0.0.2/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 rwexptest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rwexptest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/_init_.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/example.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/toml.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rwexptest-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rwexptest-0.0.3/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 rwexptest-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rwexptest-0.0.3/PKG-INFO
```

### Comparing `rwexptest-0.0.2/RWexptest/toml.py` & `rwexptest-0.0.3/RWexptest/toml.py`

 * *Files identical despite different names*

### Comparing `rwexptest-0.0.2/LICENSE.txt` & `rwexptest-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rwexptest-0.0.2/pyproject.toml` & `rwexptest-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "RWexptest"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="RuiwangW", email="2219312248@qq.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rwexptest-0.0.2/PKG-INFO` & `rwexptest-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RWexptest
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: RuiwangW <2219312248@qq.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

