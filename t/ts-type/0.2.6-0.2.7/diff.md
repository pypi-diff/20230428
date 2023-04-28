# Comparing `tmp/ts_type-0.2.6.tar.gz` & `tmp/ts_type-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_type-0.2.6.tar", last modified: Sun Sep  4 13:43:56 2022, max compression
+gzip compressed data, was "ts_type-0.2.7.tar", last modified: Fri Apr 28 12:37:56 2023, max compression
```

## Comparing `ts_type-0.2.6.tar` & `ts_type-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:43:56.310192 ts_type-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-04 13:43:47.000000 ts_type-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7233 2022-09-04 13:43:56.310192 ts_type-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6718 2022-09-04 13:43:47.000000 ts_type-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-04 13:43:47.000000 ts_type-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 13:43:56.310192 ts_type-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-09-04 13:43:47.000000 ts_type-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:43:56.310192 ts_type-0.2.6/ts_type/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8667 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/builders.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    11084 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-04 13:43:47.000000 ts_type-0.2.6/ts_type/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 13:43:56.310192 ts_type-0.2.6/ts_type.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7233 2022-09-04 13:43:56.000000 ts_type-0.2.6/ts_type.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-04 13:43:56.000000 ts_type-0.2.6/ts_type.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 13:43:56.000000 ts_type-0.2.6/ts_type.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-04 13:43:56.000000 ts_type-0.2.6/ts_type.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.391476 ts_type-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 12:37:47.000000 ts_type-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-28 12:37:56.387476 ts_type-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-28 12:37:47.000000 ts_type-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 12:37:47.000000 ts_type-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:37:56.391476 ts_type-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-28 12:37:47.000000 ts_type-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-28 12:37:47.000000 ts_type-0.2.7/tests/test_ts_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/ts_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/ts_type.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/top_level.txt
```

### Comparing `ts_type-0.2.6/LICENSE` & `ts_type-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.6/PKG-INFO` & `ts_type-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts_type
-Version: 0.2.6
+Version: 0.2.7
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ts_type-0.2.6/README.md` & `ts_type-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.6/setup.py` & `ts_type-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,12 @@
         "Bug Tracker": "https://github.com/saryou/ts_type/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=["ts_type"],
+    packages=setuptools.find_packages(exclude=["tests"]),
     package_dir={"ts_type": "ts_type"},
+    package_data={"ts_type": ["py.typed"]},
     python_requires=">=3.9",
 )
```

### Comparing `ts_type-0.2.6/ts_type/builders.py` & `ts_type-0.2.7/ts_type/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         return '\n\n'.join([render(k) for k in ref_names])
 
     def type_to_node(self, t: Any) -> nodes.TypeNode:
         if t in [None, type(None)]:
             return nodes.Null()
 
         origin = getattr(t, '__origin__', None)
-        args = getattr(t, '__args__', tuple())
+        args: tuple[Any, ...] = getattr(t, '__args__', tuple())
 
         if origin is Union or _is_union_type(t):
             assert args
             if len(args) == 1:
                 return self.type_to_node(args[0])
             return nodes.Union(
                 of=[self.type_to_node(a) for a in args])
```

### Comparing `ts_type-0.2.6/ts_type/generators.py` & `ts_type-0.2.7/ts_type/generators.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.6/ts_type/nodes.py` & `ts_type-0.2.7/ts_type/nodes.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.6/ts_type/utils.py` & `ts_type-0.2.7/ts_type/utils.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.6/ts_type.egg-info/PKG-INFO` & `ts_type-0.2.7/ts_type.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-type
-Version: 0.2.6
+Version: 0.2.7
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

