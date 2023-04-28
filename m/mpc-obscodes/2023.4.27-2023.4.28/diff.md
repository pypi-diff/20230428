# Comparing `tmp/mpc_obscodes-2023.4.27.tar.gz` & `tmp/mpc_obscodes-2023.4.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.4.27.tar", last modified: Thu Apr 27 17:26:20 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.4.28.tar", last modified: Fri Apr 28 01:16:48 2023, max compression
```

## Comparing `mpc_obscodes-2023.4.27.tar` & `mpc_obscodes-2023.4.28.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.317140 mpc_obscodes-2023.4.27/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245177 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 17:26:01.000000 mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:26:20.317140 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 17:26:20.000000 mpc_obscodes-2023.4.27/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-27 17:26:05.000000 mpc_obscodes-2023.4.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:26:20.321140 mpc_obscodes-2023.4.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245177 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 01:16:31.000000 mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:16:48.000000 mpc_obscodes-2023.4.28/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 01:16:36.000000 mpc_obscodes-2023.4.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:16:48.204168 mpc_obscodes-2023.4.28/setup.cfg
```

### Comparing `mpc_obscodes-2023.4.27/mpc_obscodes/compare.py` & `mpc_obscodes-2023.4.28/mpc_obscodes/compare.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,61 @@
-
 import argparse
 import hashlib
 import sys
 
-def compare_md5(md5_hash, file):
+
+def calculate_md5(file):
     """
-    Compares the MD5 hash of the given file to the given MD5 hash.
+    Calculates the MD5 hash of the given file.
 
     Parameters
     ----------
-    md5_hash : str
-        The MD5 hash to compare to.
     file : str
         The path to the file.
 
     Returns
     -------
-    bool
-        True if the MD5 hashes match, False otherwise.
+    str
+        The MD5 hash of the file.
     """
     with open(file, "rb") as f:
         contents = f.read()
-        return md5_hash == hashlib.md5(contents).hexdigest()
-    
+        return hashlib.md5(contents).hexdigest()
+
+
+def compare_md5(file1, file2):
+    """
+    Calculate and compare the MD5 hashes of the given files.
+
+    Parameters
+    ----------
+    file1 : str
+        The path to the first file.
+    file2 : str
+        The path to the second file.
+
+    Returns
+    -------
+    bool
+        True if the MD5 hashes match, False otherwise.
+    """
+    md5_hash1 = calculate_md5(file1)
+    md5_hash2 = calculate_md5(file2)
+
+    return md5_hash1 == md5_hash2
+
+
 if __name__ == "__main__":
-    
-    
+
     parser = argparse.ArgumentParser(
         description="Compares the MD5 hash of the given file to the given MD5 hash."
     )
-    parser.add_argument("md5_hash", help="The MD5 hash to compare to.")
-    parser.add_argument("file", help="The path to the file.")
+    parser.add_argument("file1", help="The path to the first file.")
+    parser.add_argument("file2", help="The path to the second file.")
     args = parser.parse_args()
 
-    if compare_md5(args.md5_hash, args.file):
+    if compare_md5(args.file1, args.file2):
         print("MD5 hashes match.")
         sys.exit(0)
     else:
         print("MD5 hashes do not match.")
         sys.exit(1)
```

### Comparing `mpc_obscodes-2023.4.27/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.4.28/mpc_obscodes/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import os
 import shutil
 
 import requests
 
 URL = "https://minorplanetcenter.net/Extended_Files/obscodes_extended.json.gz"
 FILE_COMPRESSED = os.path.join(os.path.dirname(__file__), "obscodes_extended.json.gz")
-FILE_DECOMPRESSED =  os.path.join(os.path.dirname(__file__), "obscodes_extended.json")
-MD5_FILE =  os.path.join(os.path.dirname(__file__), "obscodes_extended.md5")
+FILE_DECOMPRESSED = os.path.join(os.path.dirname(__file__), "obscodes_extended.json")
+MD5_FILE = os.path.join(os.path.dirname(__file__), "obscodes_extended.md5")
 
 
 def fetch_file(url: str, output_file: str):
     """
     Fetches the file from the given URL and saves it to the output file.
 
     Parameters
```

### Comparing `mpc_obscodes-2023.4.27/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.4.28/mpc_obscodes/obscodes_extended.json`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.27/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.4.28/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.27/pyproject.toml` & `mpc_obscodes-2023.4.28/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.04.27"
+version = "2023.04.28"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

