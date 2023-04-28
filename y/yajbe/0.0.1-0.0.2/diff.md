# Comparing `tmp/yajbe-0.0.1.tar.gz` & `tmp/yajbe-0.0.2.tar.gz`

## Comparing `yajbe-0.0.1.tar` & `yajbe-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 yajbe-0.0.1/example.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 yajbe-0.0.1/test.yajbe
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 yajbe-0.0.1/src/yajbe/__init__.py
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 yajbe-0.0.1/src/yajbe/decoder.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 yajbe-0.0.1/src/yajbe/encoder.py
--rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 yajbe-0.0.1/src/yajbe/freq.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 yajbe-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 yajbe-0.0.1/tests/test_yajbe.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 yajbe-0.0.1/tests/test_yajbe_array.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 yajbe-0.0.1/.gitignore
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 yajbe-0.0.1/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 yajbe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 yajbe-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 yajbe-0.0.2/example.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 yajbe-0.0.2/test.yajbe
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 yajbe-0.0.2/src/yajbe/__init__.py
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 yajbe-0.0.2/src/yajbe/decoder.py
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 yajbe-0.0.2/src/yajbe/encoder.py
+-rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 yajbe-0.0.2/src/yajbe/freq.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 yajbe-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 yajbe-0.0.2/tests/test_yajbe.py
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 yajbe-0.0.2/tests/test_yajbe_array.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 yajbe-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 yajbe-0.0.2/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 yajbe-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 yajbe-0.0.2/PKG-INFO
```

### Comparing `yajbe-0.0.1/example.py` & `yajbe-0.0.2/example.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/src/yajbe/__init__.py` & `yajbe-0.0.2/src/yajbe/__init__.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/src/yajbe/decoder.py` & `yajbe-0.0.2/src/yajbe/decoder.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/src/yajbe/encoder.py` & `yajbe-0.0.2/src/yajbe/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         else:
             delta_length = length - inline_max
             nbytes = int_bytes_width(delta_length)
             self._write_byte(head | (inline_max + nbytes))
             self._write_uint(delta_length, nbytes)
 
     def _write_byte(self, v: int) -> None:
-        self._stream.write(v.to_bytes())
+        self._stream.write(bytes([v & 0xff]))
 
     def _write_bytes(self, value: bytes) -> None:
         self._stream.write(value)
 
     def _write_uint(self, value: int, width: int) -> None:
         buf = bytearray(width)
         for i in range(width):
```

### Comparing `yajbe-0.0.1/src/yajbe/freq.py` & `yajbe-0.0.2/src/yajbe/freq.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/tests/__init__.py` & `yajbe-0.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/tests/test_yajbe.py` & `yajbe-0.0.2/tests/test_yajbe.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/tests/test_yajbe_array.py` & `yajbe-0.0.2/tests/test_yajbe_array.py`

 * *Files identical despite different names*

### Comparing `yajbe-0.0.1/pyproject.toml` & `yajbe-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yajbe"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matteo Bertozzi", email="mbertozzi@apache.org" },
 ]
 description = "YAJBE is a compact binary data format built to be a drop-in replacement for JSON (JavaScript Object Notation)."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `yajbe-0.0.1/PKG-INFO` & `yajbe-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: yajbe
-Version: 0.0.1
+Version: 0.0.2
 Summary: YAJBE is a compact binary data format built to be a drop-in replacement for JSON (JavaScript Object Notation).
 Project-URL: Homepage, https://github.com/matteobertozzi/yajbe-data-format
 Project-URL: Bug Tracker, https://github.com/matteobertozzi/yajbe-data-format/issues
 Author-email: Matteo Bertozzi <mbertozzi@apache.org>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # YAJBE for Python
 
 YAJBE is a compact binary data format built to be a drop-in replacement for JSON (JavaScript Object Notation).
 
 
 ## Motivation for a new format
 We have a lot of services exchanging or storing data using JSON, and most of them don't want to switch to a data format that requires a schema.
 
 We wanted to remove the overhead of the JSON format (especially field names), but keeping the same data model flexibility (numbers, strings, arrays, maps/objects, and a few values such as false, true, and null).
 
 See more at https://github.com/matteobertozzi/yajbe-data-format
 
+### Install the package
+You can find the package at https://pypi.org/project/yajbe. \
+Python >=3.10 is required. To install or upgrade you can use:
+```bash
+$ pip install --upgrade yajbe
+```
+
 ## Usage
 
 ```python
 import yajbe
 
 # encode and decode from bytes
 enc = yajbe.encode_as_bytes({'a': 10, 'b': ['hello', 10]})
```

