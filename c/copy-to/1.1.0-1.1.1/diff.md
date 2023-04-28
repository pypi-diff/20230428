# Comparing `tmp/copy-to-1.1.0.tar.gz` & `tmp/copy-to-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copy-to-1.1.0.tar", last modified: Fri Apr 28 00:43:51 2023, max compression
+gzip compressed data, was "copy-to-1.1.1.tar", last modified: Fri Apr 28 00:45:04 2023, max compression
```

## Comparing `copy-to-1.1.0.tar` & `copy-to-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:43:51.757149 copy-to-1.1.0/
--rw-r--r--   0 burp      (1000) burp      (1001)     1071 2023-04-25 14:58:58.000000 copy-to-1.1.0/LICENSE
--rw-r--r--   0 burp      (1000) burp      (1001)     2193 2023-04-28 00:43:51.757149 copy-to-1.1.0/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)     1603 2023-04-28 00:43:04.000000 copy-to-1.1.0/README.md
-drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:43:51.757149 copy-to-1.1.0/copy_to.egg-info/
--rw-r--r--   0 burp      (1000) burp      (1001)     2193 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/PKG-INFO
--rw-r--r--   0 burp      (1000) burp      (1001)      201 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/SOURCES.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        1 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/dependency_links.txt
--rw-r--r--   0 burp      (1000) burp      (1001)       41 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/entry_points.txt
--rw-r--r--   0 burp      (1000) burp      (1001)        8 2023-04-28 00:43:51.000000 copy-to-1.1.0/copy_to.egg-info/top_level.txt
--rwxr-xr-x   0 burp      (1000) burp      (1001)    22523 2023-04-28 00:33:19.000000 copy-to-1.1.0/copy_to.py
--rw-r--r--   0 burp      (1000) burp      (1001)      718 2023-04-28 00:43:39.000000 copy-to-1.1.0/pyproject.toml
--rw-r--r--   0 burp      (1000) burp      (1001)       38 2023-04-28 00:43:51.757149 copy-to-1.1.0/setup.cfg
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:45:04.102289 copy-to-1.1.1/
+-rw-r--r--   0 burp      (1000) burp      (1001)     1071 2023-04-25 14:58:58.000000 copy-to-1.1.1/LICENSE
+-rw-r--r--   0 burp      (1000) burp      (1001)     2201 2023-04-28 00:45:04.102289 copy-to-1.1.1/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)     1611 2023-04-28 00:44:45.000000 copy-to-1.1.1/README.md
+drwxr-xr-x   0 burp      (1000) burp      (1001)        0 2023-04-28 00:45:04.102289 copy-to-1.1.1/copy_to.egg-info/
+-rw-r--r--   0 burp      (1000) burp      (1001)     2201 2023-04-28 00:45:04.000000 copy-to-1.1.1/copy_to.egg-info/PKG-INFO
+-rw-r--r--   0 burp      (1000) burp      (1001)      201 2023-04-28 00:45:04.000000 copy-to-1.1.1/copy_to.egg-info/SOURCES.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        1 2023-04-28 00:45:04.000000 copy-to-1.1.1/copy_to.egg-info/dependency_links.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)       41 2023-04-28 00:45:04.000000 copy-to-1.1.1/copy_to.egg-info/entry_points.txt
+-rw-r--r--   0 burp      (1000) burp      (1001)        8 2023-04-28 00:45:04.000000 copy-to-1.1.1/copy_to.egg-info/top_level.txt
+-rwxr-xr-x   0 burp      (1000) burp      (1001)    22523 2023-04-28 00:33:19.000000 copy-to-1.1.1/copy_to.py
+-rw-r--r--   0 burp      (1000) burp      (1001)      718 2023-04-28 00:44:54.000000 copy-to-1.1.1/pyproject.toml
+-rw-r--r--   0 burp      (1000) burp      (1001)       38 2023-04-28 00:45:04.102289 copy-to-1.1.1/setup.cfg
```

### Comparing `copy-to-1.1.0/LICENSE` & `copy-to-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `copy-to-1.1.0/PKG-INFO` & `copy-to-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-to
-Version: 1.1.0
+Version: 1.1.1
 Summary: A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration
 Author-email: Stan Nys <stan96@duck.com>
 Project-URL: Homepage, https://github.com/excited-bore/copy-to
 Project-URL: Bug Tracker, https://github.com/excited-bore/copy-to/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 Copy the files to their destination by running 
 ```
 copy-to run myname1 (myname2)
 ```
 
 Or copy the files back to source by running 
 ```
-copy-to run myname1 (myname2)
+copy-to run-reverse myname1 (myname2)
 ```
 
 Delete set of dest/src by name with 
 ```
 copy-to delete myname1 (myname2)
 ```
```

### Comparing `copy-to-1.1.0/README.md` & `copy-to-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Copy the files to their destination by running 
 ```
 copy-to run myname1 (myname2)
 ```
 
 Or copy the files back to source by running 
 ```
-copy-to run myname1 (myname2)
+copy-to run-reverse myname1 (myname2)
 ```
 
 Delete set of dest/src by name with 
 ```
 copy-to delete myname1 (myname2)
 ```
```

### Comparing `copy-to-1.1.0/copy_to.egg-info/PKG-INFO` & `copy-to-1.1.1/copy_to.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copy-to
-Version: 1.1.0
+Version: 1.1.1
 Summary: A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration
 Author-email: Stan Nys <stan96@duck.com>
 Project-URL: Homepage, https://github.com/excited-bore/copy-to
 Project-URL: Bug Tracker, https://github.com/excited-bore/copy-to/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 Copy the files to their destination by running 
 ```
 copy-to run myname1 (myname2)
 ```
 
 Or copy the files back to source by running 
 ```
-copy-to run myname1 (myname2)
+copy-to run-reverse myname1 (myname2)
 ```
 
 Delete set of dest/src by name with 
 ```
 copy-to delete myname1 (myname2)
 ```
```

### Comparing `copy-to-1.1.0/copy_to.py` & `copy-to-1.1.1/copy_to.py`

 * *Files identical despite different names*

### Comparing `copy-to-1.1.0/pyproject.toml` & `copy-to-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "argcomplete"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "copy-to"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Stan Nys", email="stan96@duck.com" },
 ]
 
 description = "A little commandline tool to copy and paste multiple files and directories to single directory with use of configuration"
 readme = "README.md"
 requires-python = ">=3.7"
```

