# Comparing `tmp/aws-excom-0.0.8.tar.gz` & `tmp/aws-excom-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-excom-0.0.8.tar", last modified: Wed Oct 26 22:23:37 2022, max compression
+gzip compressed data, was "aws-excom-0.0.9.tar", last modified: Wed Oct 26 22:30:41 2022, max compression
```

## Comparing `aws-excom-0.0.8.tar` & `aws-excom-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-26 22:23:37.248851 aws-excom-0.0.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1069 2022-10-26 22:23:28.000000 aws-excom-0.0.8/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2022-10-26 22:23:28.000000 aws-excom-0.0.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2022-10-26 22:23:37.248851 aws-excom-0.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      917 2022-10-26 22:23:28.000000 aws-excom-0.0.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-26 22:23:37.248851 aws-excom-0.0.8/aws_excom/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2227 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5121 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-26 22:23:37.248851 aws-excom-0.0.8/aws_excom/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      976 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/tests/test_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2022-10-26 22:23:28.000000 aws-excom-0.0.8/aws_excom/tests/test_install.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-26 22:23:37.248851 aws-excom-0.0.8/aws_excom.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      397 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       49 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-10-26 22:23:37.000000 aws-excom-0.0.8/aws_excom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      693 2022-10-26 22:23:28.000000 aws-excom-0.0.8/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-10-26 22:23:37.248851 aws-excom-0.0.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       92 2022-10-26 22:23:28.000000 aws-excom-0.0.8/setup.py
+drwxr-xr-x   0 benv      (1000) benv      (1000)        0 2022-10-26 22:30:41.177929 aws-excom-0.0.9/
+-rw-r--r--   0 benv      (1000) benv      (1000)     1069 2022-10-12 21:30:13.000000 aws-excom-0.0.9/LICENSE
+-rw-r--r--   0 benv      (1000) benv      (1000)       18 2022-10-12 21:20:20.000000 aws-excom-0.0.9/MANIFEST.in
+-rw-r--r--   0 benv      (1000) benv      (1000)     1424 2022-10-26 22:30:41.177929 aws-excom-0.0.9/PKG-INFO
+-rw-r--r--   0 benv      (1000) benv      (1000)      917 2022-10-12 22:23:41.000000 aws-excom-0.0.9/README.md
+drwxr-xr-x   0 benv      (1000) benv      (1000)        0 2022-10-26 22:30:41.177929 aws-excom-0.0.9/aws_excom/
+-rw-r--r--   0 benv      (1000) benv      (1000)      140 2022-10-12 20:56:01.000000 aws-excom-0.0.9/aws_excom/__init__.py
+-rw-r--r--   0 benv      (1000) benv      (1000)     2227 2022-10-13 10:20:08.000000 aws-excom-0.0.9/aws_excom/aws.py
+-rw-r--r--   0 benv      (1000) benv      (1000)     5121 2022-10-17 13:43:49.000000 aws-excom-0.0.9/aws_excom/cli.py
+drwxr-xr-x   0 benv      (1000) benv      (1000)        0 2022-10-26 22:30:41.177929 aws-excom-0.0.9/aws_excom/tests/
+-rw-r--r--   0 benv      (1000) benv      (1000)        0 2022-10-26 22:22:24.000000 aws-excom-0.0.9/aws_excom/tests/__init__.py
+-rw-r--r--   0 benv      (1000) benv      (1000)      976 2022-10-26 22:22:24.000000 aws-excom-0.0.9/aws_excom/tests/test_aws.py
+-rw-r--r--   0 benv      (1000) benv      (1000)      519 2022-10-26 22:22:24.000000 aws-excom-0.0.9/aws_excom/tests/test_install.py
+drwxr-xr-x   0 benv      (1000) benv      (1000)        0 2022-10-26 22:30:41.177929 aws-excom-0.0.9/aws_excom.egg-info/
+-rw-r--r--   0 benv      (1000) benv      (1000)     1424 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/PKG-INFO
+-rw-r--r--   0 benv      (1000) benv      (1000)      397 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/SOURCES.txt
+-rw-r--r--   0 benv      (1000) benv      (1000)        1 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/dependency_links.txt
+-rw-r--r--   0 benv      (1000) benv      (1000)       49 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/entry_points.txt
+-rw-r--r--   0 benv      (1000) benv      (1000)       33 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/requires.txt
+-rw-r--r--   0 benv      (1000) benv      (1000)       10 2022-10-26 22:30:41.000000 aws-excom-0.0.9/aws_excom.egg-info/top_level.txt
+-rw-r--r--   0 benv      (1000) benv      (1000)      693 2022-10-26 22:26:12.000000 aws-excom-0.0.9/pyproject.toml
+-rw-r--r--   0 benv      (1000) benv      (1000)       38 2022-10-26 22:30:41.177929 aws-excom-0.0.9/setup.cfg
+-rw-r--r--   0 benv      (1000) benv      (1000)       92 2022-10-26 22:22:24.000000 aws-excom-0.0.9/setup.py
```

### Comparing `aws-excom-0.0.8/LICENSE` & `aws-excom-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/PKG-INFO` & `aws-excom-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-excom
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper for AWS ECS Execute Command
 Author-email: Ben Vosper <author@example.com>
 Project-URL: Homepage, https://github.com/benvosper/aws-excom/
 Project-URL: Bug Tracker, https://github.com/pypa/aws-excom/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-excom-0.0.8/README.md` & `aws-excom-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/aws_excom/aws.py` & `aws-excom-0.0.9/aws_excom/aws.py`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/aws_excom/cli.py` & `aws-excom-0.0.9/aws_excom/cli.py`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/aws_excom/tests/test_aws.py` & `aws-excom-0.0.9/aws_excom/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/aws_excom/tests/test_install.py` & `aws-excom-0.0.9/aws_excom/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `aws-excom-0.0.8/aws_excom.egg-info/PKG-INFO` & `aws-excom-0.0.9/aws_excom.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-excom
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper for AWS ECS Execute Command
 Author-email: Ben Vosper <author@example.com>
 Project-URL: Homepage, https://github.com/benvosper/aws-excom/
 Project-URL: Bug Tracker, https://github.com/pypa/aws-excom/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-excom-0.0.8/pyproject.toml` & `aws-excom-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws-excom"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = ['simple-term-menu', 'termcolor', 'boto3']
 authors = [
   { name="Ben Vosper", email="author@example.com" },
 ]
 description = "Wrapper for AWS ECS Execute Command"
 readme = "README.md"
 requires-python = ">=3.7"
```

