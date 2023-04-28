# Comparing `tmp/python-observer-0.3.0.tar.gz` & `tmp/python-observer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-observer-0.3.0.tar", max compression
+gzip compressed data, was "python-observer-0.3.1.tar", max compression
```

## Comparing `python-observer-0.3.0.tar` & `python-observer-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.3.0/LICENSE
--rw-r--r--   0        0        0      580 2023-04-28 10:32:48.923265 python-observer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.3.0/python_observer/__init__.py
--rw-r--r--   0        0        0     4446 2023-04-28 10:31:08.927636 python-observer-0.3.0/python_observer/cli.py
--rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.3.0/python_observer/constants.py
--rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.3.0/python_observer/date.py
--rw-r--r--   0        0        0      992 2023-04-28 10:31:06.738394 python-observer-0.3.0/python_observer/display.py
--rw-r--r--   0        0        0      972 2023-04-28 10:24:47.359182 python-observer-0.3.0/python_observer/misc.py
--rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.3.0/python_observer/watch.py
--rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.3.0/README.md
--rw-r--r--   0        0        0      966 2023-04-28 10:33:03.968515 python-observer-0.3.0/setup.py
--rw-r--r--   0        0        0      787 2023-04-28 10:33:03.968515 python-observer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.3.1/LICENSE
+-rw-r--r--   0        0        0      580 2023-04-28 10:51:14.439129 python-observer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.3.1/python_observer/__init__.py
+-rw-r--r--   0        0        0     4446 2023-04-28 10:31:08.927636 python-observer-0.3.1/python_observer/cli.py
+-rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.3.1/python_observer/constants.py
+-rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.3.1/python_observer/date.py
+-rw-r--r--   0        0        0      992 2023-04-28 10:31:06.738394 python-observer-0.3.1/python_observer/display.py
+-rw-r--r--   0        0        0     1019 2023-04-28 10:49:03.740134 python-observer-0.3.1/python_observer/misc.py
+-rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.3.1/python_observer/watch.py
+-rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.3.1/README.md
+-rw-r--r--   0        0        0      966 2023-04-28 10:51:43.005696 python-observer-0.3.1/setup.py
+-rw-r--r--   0        0        0      787 2023-04-28 10:51:43.006696 python-observer-0.3.1/PKG-INFO
```

### Comparing `python-observer-0.3.0/LICENSE` & `python-observer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.0/pyproject.toml` & `python-observer-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-observer"
-version = "0.3.0"
+version = "0.3.1"
 description = "Live reload for Python apps"
 authors = ["Skyascii <savioxavier112@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "python_observer/**/*.py" }
 ]
```

### Comparing `python-observer-0.3.0/python_observer/cli.py` & `python-observer-0.3.1/python_observer/cli.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.0/python_observer/date.py` & `python-observer-0.3.1/python_observer/date.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.0/python_observer/display.py` & `python-observer-0.3.1/python_observer/display.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.0/python_observer/misc.py` & `python-observer-0.3.1/python_observer/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import subprocess
 import sys
 from pathlib import Path
 
 import tomli
 
 from .display import print_observer_error
@@ -12,18 +13,18 @@
         subprocess.check_output(f"{sys.executable} --version", shell=True)
         .strip()
         .decode("utf-8")
     )
 
 
 def get_observer_version():
-    with open("pyproject.toml", "r") as f:
-        toml_data = tomli.loads(f.read())
+    sys.path.insert(0, os.path.abspath(".."))
 
-    return toml_data["tool"]["poetry"]["version"]
+    with open("../pyproject.toml", mode="rb") as pyproject:
+        return tomli.load(pyproject)["tool"]["poetry"]["version"]
 
 
 def run_file(command):
     cmd = [sys.executable, *command]
 
     return subprocess.run(cmd)
```

### Comparing `python-observer-0.3.0/python_observer/watch.py` & `python-observer-0.3.1/python_observer/watch.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.3.0/setup.py` & `python-observer-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'tomli>=2.0.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['observer = python_observer.cli:main']}
 
 setup_kwargs = {
     'name': 'python-observer',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Live reload for Python apps',
     'long_description': "# observer\n\n![observer image](https://i.imgur.com/ZoafdEY.png)\n\n> Live reload for Python apps\n\nDocs coming soon - I've ordered them via Amazon Prime\n",
     'author': 'Skyascii',
     'author_email': 'savioxavier112@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `python-observer-0.3.0/PKG-INFO` & `python-observer-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-observer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Live reload for Python apps
 License: MIT
 Author: Skyascii
 Author-email: savioxavier112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

