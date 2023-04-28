# Comparing `tmp/rwexptest-0.0.3.tar.gz` & `tmp/RWexptest-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "RWexptest-0.0.4.tar", last modified: Fri Apr 28 10:59:44 2023, max compression
```

## Comparing `rwexptest-0.0.3.tar` & `RWexptest-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/_init_.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/example.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 rwexptest-0.0.3/RWexptest/toml.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rwexptest-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rwexptest-0.0.3/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 rwexptest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 rwexptest-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 10:59:44.505217 RWexptest-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 RWexptest-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2023-04-28 10:59:44.504712 RWexptest-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-25 08:29:52.000000 RWexptest-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 10:59:44.477714 RWexptest-0.0.4/RWexptest/
+-rw-rw-rw-   0        0        0        0 2023-04-24 09:02:16.000000 RWexptest-0.0.4/RWexptest/_init_.py
+-rw-rw-rw-   0        0        0      466 2023-04-28 08:54:19.000000 RWexptest-0.0.4/RWexptest/example.py
+-rw-rw-rw-   0        0        0     2126 2023-04-25 09:28:17.000000 RWexptest-0.0.4/RWexptest/toml.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:59:44.499198 RWexptest-0.0.4/RWexptest.egg-info/
+-rw-rw-rw-   0        0        0      687 2023-04-28 10:59:44.000000 RWexptest-0.0.4/RWexptest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-28 10:59:44.000000 RWexptest-0.0.4/RWexptest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:59:44.000000 RWexptest-0.0.4/RWexptest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 10:59:44.000000 RWexptest-0.0.4/RWexptest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 10:59:44.000000 RWexptest-0.0.4/RWexptest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2023-04-28 10:58:40.000000 RWexptest-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:59:44.505217 RWexptest-0.0.4/setup.cfg
```

### Comparing `rwexptest-0.0.3/RWexptest/toml.py` & `RWexptest-0.0.4/RWexptest/toml.py`

 * *Files identical despite different names*

### Comparing `rwexptest-0.0.3/LICENSE.txt` & `RWexptest-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rwexptest-0.0.3/pyproject.toml` & `RWexptest-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "RWexptest"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="RuiwangW", email="2219312248@qq.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-install_requires = [
+dependencies = [
     "numpy",
     "scipy",
     "sklearn" 
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
```

### Comparing `rwexptest-0.0.3/PKG-INFO` & `RWexptest-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: RWexptest
-Version: 0.0.3
-Summary: A small example package
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Author-email: RuiwangW <2219312248@qq.com>
-License-File: LICENSE.txt
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Example Package
-
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+Metadata-Version: 2.1
+Name: RWexptest
+Version: 0.0.4
+Summary: A small example package
+Author-email: RuiwangW <2219312248@qq.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Example Package
+
+This is a simple example package. You can use
+[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
```

