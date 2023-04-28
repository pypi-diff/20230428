# Comparing `tmp/burrowkv-0.0.2.tar.gz` & `tmp/burrowkv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrowkv-0.0.2.tar", last modified: Fri Apr 28 15:36:13 2023, max compression
+gzip compressed data, was "burrowkv-0.0.3.tar", last modified: Fri Apr 28 16:01:40 2023, max compression
```

## Comparing `burrowkv-0.0.2.tar` & `burrowkv-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 15:36:13.402902 burrowkv-0.0.2/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-04-27 20:35:40.000000 burrowkv-0.0.2/LICENSE
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 15:36:13.398902 burrowkv-0.0.2/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1503 2023-04-28 13:02:04.000000 burrowkv-0.0.2/README.md
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 15:36:13.398902 burrowkv-0.0.2/burrowkv/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       55 2023-04-28 13:02:04.000000 burrowkv-0.0.2/burrowkv/__init__.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     4517 2023-04-28 15:21:01.000000 burrowkv-0.0.2/burrowkv/burrowkv.py
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 15:36:13.398902 burrowkv-0.0.2/burrowkv.egg-info/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 15:36:13.000000 burrowkv-0.0.2/burrowkv.egg-info/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      237 2023-04-28 15:36:13.000000 burrowkv-0.0.2/burrowkv.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-04-28 15:36:13.000000 burrowkv-0.0.2/burrowkv.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       15 2023-04-28 15:36:13.000000 burrowkv-0.0.2/burrowkv.egg-info/top_level.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-04-28 15:36:13.402902 burrowkv-0.0.2/setup.cfg
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      694 2023-04-28 15:35:06.000000 burrowkv-0.0.2/setup.py
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 15:36:13.398902 burrowkv-0.0.2/tests/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 10:10:31.000000 burrowkv-0.0.2/tests/__init__.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1708 2023-04-28 15:07:59.000000 burrowkv-0.0.2/tests/test_burrowkv.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.222696 burrowkv-0.0.3/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-04-27 20:35:40.000000 burrowkv-0.0.3/LICENSE
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 16:01:40.222696 burrowkv-0.0.3/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1503 2023-04-28 13:02:04.000000 burrowkv-0.0.3/README.md
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.218696 burrowkv-0.0.3/burrowkv/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       55 2023-04-28 13:02:04.000000 burrowkv-0.0.3/burrowkv/__init__.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     4722 2023-04-28 16:00:24.000000 burrowkv-0.0.3/burrowkv/burrowkv.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.218696 burrowkv-0.0.3/burrowkv.egg-info/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1924 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      237 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       15 2023-04-28 16:01:40.000000 burrowkv-0.0.3/burrowkv.egg-info/top_level.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-04-28 16:01:40.222696 burrowkv-0.0.3/setup.cfg
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      694 2023-04-28 15:59:11.000000 burrowkv-0.0.3/setup.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 16:01:40.222696 burrowkv-0.0.3/tests/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        0 2023-04-28 10:10:31.000000 burrowkv-0.0.3/tests/__init__.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1708 2023-04-28 15:07:59.000000 burrowkv-0.0.3/tests/test_burrowkv.py
```

### Comparing `burrowkv-0.0.2/LICENSE` & `burrowkv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `burrowkv-0.0.2/PKG-INFO` & `burrowkv-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrowkv
-Version: 0.0.2
+Version: 0.0.3
 Summary: key-value store
 Home-page: https://github.com/iunary/burrowkv
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: key value store,kv,key-value
 Platform: UNKNOWN
```

### Comparing `burrowkv-0.0.2/README.md` & `burrowkv-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `burrowkv-0.0.2/burrowkv/burrowkv.py` & `burrowkv-0.0.3/burrowkv/burrowkv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """Burrowkv key value store implementation in python
 """
-from typing import Optional, List, Tuple
-from collections import defaultdict
+import threading
 import json
+from collections import defaultdict
 from contextlib import contextmanager
+from typing import Optional, List, Tuple
 
 
 class Burrowkv:
     """
     A simple key-value store implemented using a dictionary.
     """
 
     def __init__(self):
         """
         Initialize an empty key-value store.
         """
         self.__store = defaultdict(lambda: None)
+        self.__lock = threading.Lock()
 
     def set(self, key: str, value: str) -> None:
         """
         Set a value for the given key.
 
         Args:
             key (str): The key to set.
             value (str): The value to associate with the key.
 
         Example:
             >>> store = KeyValueStore()
             >>> store.set('name', 'John')
         """
-        self.__store[key] = value
+        with self.__lock:
+            self.__store[key] = value
 
     def get(self, key: str) -> Optional[str]:
         """
         Retrieve the value associated with the given key.
 
         Args:
             key (str): The key to retrieve.
@@ -45,24 +48,26 @@
         Example:
             >>> store = KeyValueStore()
             >>> store.set('name', 'John')
             >>> store.get('name')
             'John'
             >>> store.get('age')
         """
-        return self.__store[key]
+        with self.__lock:
+            return self.__store[key]
 
     def delete(self, key: str) -> None:
         """
         Delete the key-value pair for the given key.
 
         Args:
             key (str): The key to delete.
         """
-        del self.__store[key]
+        with self.__lock:
+            del self.__store[key]
 
     def contains(self, key: str) -> bool:
         """
         Check if the key exists in the store.
 
         Args:
             key (str): The key to check.
@@ -141,15 +146,16 @@
 
         Args:
             json_str: The JSON string representing the key-value store.
 
         Returns:
             None
         """
-        self.__store = defaultdict(lambda: None, json.loads(json_data))
+        with self.__lock:
+            self.__store = defaultdict(lambda: None, json.loads(json_data))
 
     @contextmanager
     def transaction(self):
         """
         Create a transaction context for
         performing multiple operations on the store.
 
@@ -169,16 +175,16 @@
     def clear(self):
         """
         Clear the data store
 
         Returns:
             None
         """
-
-        self.__store.clear()
+        with self.__lock:
+            self.__store.clear()
 
     def __len__(self) -> int:
         """
         Return the number of key-value pairs in the store.
 
         Returns:
             int: The number of key-value pairs.
```

### Comparing `burrowkv-0.0.2/burrowkv.egg-info/PKG-INFO` & `burrowkv-0.0.3/burrowkv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrowkv
-Version: 0.0.2
+Version: 0.0.3
 Summary: key-value store
 Home-page: https://github.com/iunary/burrowkv
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: key value store,kv,key-value
 Platform: UNKNOWN
```

### Comparing `burrowkv-0.0.2/setup.py` & `burrowkv-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="burrowkv",
     version=VERSION,
```

### Comparing `burrowkv-0.0.2/tests/test_burrowkv.py` & `burrowkv-0.0.3/tests/test_burrowkv.py`

 * *Files identical despite different names*

