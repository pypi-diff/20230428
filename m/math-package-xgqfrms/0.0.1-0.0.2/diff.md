# Comparing `tmp/math_package_xgqfrms-0.0.1.tar.gz` & `tmp/math_package_xgqfrms-0.0.2.tar.gz`

## Comparing `math_package_xgqfrms-0.0.1.tar` & `math_package_xgqfrms-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/.editorconfig
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/src/math_package_xgqfrms/__init__.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/src/math_package_xgqfrms/math.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/tests/demo.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/LICENSE
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/.DS_Store
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/build.sh
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/upload.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/src/math_package_xgqfrms/__init__.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/src/math_package_xgqfrms/math.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/tests/demo.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/tests/test.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/README.md
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 math_package_xgqfrms-0.0.2/PKG-INFO
```

### Comparing `math_package_xgqfrms-0.0.1/src/math_package_xgqfrms/math.py` & `math_package_xgqfrms-0.0.2/src/math_package_xgqfrms/math.py`

 * *Files identical despite different names*

### Comparing `math_package_xgqfrms-0.0.1/tests/demo.py` & `math_package_xgqfrms-0.0.2/tests/demo.py`

 * *Files identical despite different names*

### Comparing `math_package_xgqfrms-0.0.1/LICENSE` & `math_package_xgqfrms-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `math_package_xgqfrms-0.0.1/README.md` & `math_package_xgqfrms-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# xgqfrms_package_math
+# math_package_xgqfrms
 
 > A math package of python 3. 🐍
 
 This package includes math methods: `add`ition, `sub`traction, `mul`tiplication and `div`ision.
 
 ## PyPI
 
@@ -22,21 +22,25 @@
 
 ```sh
 # math_package_project
 $ tree
 .
 ├── LICENSE
 ├── README.md
+├── dist
+│   ├── math_package_xgqfrms-0.0.2-py3-none-any.whl
+│   └── math_package_xgqfrms-0.0.2.tar.gz
 ├── pyproject.toml
 ├── src
 │   └── math_package_xgqfrms
 │       ├── __init__.py
 │       └── math.py
 └── tests
-    └── demo.py
+    ├── demo.py
+    └── test.py
 ```
 
 
 ## Examples
 
 1. add
 
@@ -85,7 +89,21 @@
 n1 = 6
 n2 = 2
 divide = Math.div(n1, n2)
 print("divide =", divide)
 # div = 3.0
 
 ```
+
+
+<!-- 
+
+```sh
+# build
+$ python3 -m build
+
+# upload
+$ python3 -m twine upload dist/*
+
+```
+
+ -->
```

### Comparing `math_package_xgqfrms-0.0.1/pyproject.toml` & `math_package_xgqfrms-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "math_package_xgqfrms"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="xgqfrms", email="xgqfrms@xgqfrms.xyz" },
 ]
 description = "A math package of python 3. 🐍"
 # summary = "Addition, subtraction, multiplication and division"
 # Additional properties are not allowed ('summary' was unexpected)Even Better TOML ❌
 readme = "README.md"
@@ -30,9 +30,12 @@
 license = "MIT"
 # license_files = "LICENSE"
 # Additional properties are not allowed ('license_files' was unexpected)Even Better TOML ❌
 
 
 
 [project.urls]
-"Homepage" = "https://github.com/xgqfrms/math_package_project"
-"Bug Tracker" = "https://github.com/xgqfrms/math_package_project/issues"
+"PyPi 🐍" = "https://pypi.org/project/math-package-xgqfrms/"
+"Website 🌏" = "https://math_package_project.xgqfrms.xyz/"
+"GitHub 🐙" = "https://github.com/xgqfrms/math_package_project"
+"Issues ❓" = "https://github.com/xgqfrms/math_package_project/issues"
+"Wiki 🗂️" = "https://github.com/xgqfrms/math_package_project/issues"
```

### Comparing `math_package_xgqfrms-0.0.1/PKG-INFO` & `math_package_xgqfrms-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: math_package_xgqfrms
-Version: 0.0.1
+Version: 0.0.2
 Summary: A math package of python 3. 🐍
-Project-URL: Homepage, https://github.com/xgqfrms/math_package_project
-Project-URL: Bug Tracker, https://github.com/xgqfrms/math_package_project/issues
+Project-URL: PyPi 🐍, https://pypi.org/project/math-package-xgqfrms/
+Project-URL: Website 🌏, https://math_package_project.xgqfrms.xyz/
+Project-URL: GitHub 🐙, https://github.com/xgqfrms/math_package_project
+Project-URL: Issues ❓, https://github.com/xgqfrms/math_package_project/issues
+Project-URL: Wiki 🗂️, https://github.com/xgqfrms/math_package_project/issues
 Author-email: xgqfrms <xgqfrms@xgqfrms.xyz>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: linux,math,package,python,xgqfrms
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# xgqfrms_package_math
+# math_package_xgqfrms
 
 > A math package of python 3. 🐍
 
 This package includes math methods: `add`ition, `sub`traction, `mul`tiplication and `div`ision.
 
 ## PyPI
 
@@ -40,21 +43,25 @@
 
 ```sh
 # math_package_project
 $ tree
 .
 ├── LICENSE
 ├── README.md
+├── dist
+│   ├── math_package_xgqfrms-0.0.2-py3-none-any.whl
+│   └── math_package_xgqfrms-0.0.2.tar.gz
 ├── pyproject.toml
 ├── src
 │   └── math_package_xgqfrms
 │       ├── __init__.py
 │       └── math.py
 └── tests
-    └── demo.py
+    ├── demo.py
+    └── test.py
 ```
 
 
 ## Examples
 
 1. add
 
@@ -103,7 +110,21 @@
 n1 = 6
 n2 = 2
 divide = Math.div(n1, n2)
 print("divide =", divide)
 # div = 3.0
 
 ```
+
+
+<!-- 
+
+```sh
+# build
+$ python3 -m build
+
+# upload
+$ python3 -m twine upload dist/*
+
+```
+
+ -->
```

