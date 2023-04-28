# Comparing `tmp/nip-config-0.9.0.tar.gz` & `tmp/nip-config-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nip-config-0.9.0.tar", last modified: Fri Apr 28 08:22:55 2023, max compression
+gzip compressed data, was "nip-config-0.9.1.tar", last modified: Fri Apr 28 08:29:03 2023, max compression
```

## Comparing `nip-config-0.9.0.tar` & `nip-config-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.557201 nip-config-0.9.0/
--rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.9.0/LICENSE
--rw-rw-rw-   0        0        0      740 2023-04-28 08:22:55.558469 nip-config-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.540770 nip-config-0.9.0/nip/
--rw-rw-rw-   0        0        0      137 2023-04-28 07:36:18.000000 nip-config-0.9.0/nip/__init__.py
--rw-rw-rw-   0        0        0     5869 2023-04-28 07:37:49.000000 nip-config-0.9.0/nip/constructor.py
--rw-rw-rw-   0        0        0     3078 2023-04-28 08:21:33.000000 nip-config-0.9.0/nip/convertor.py
--rw-rw-rw-   0        0        0     1581 2023-04-28 08:19:13.000000 nip-config-0.9.0/nip/directives.py
--rw-rw-rw-   0        0        0      807 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/dumper.py
--rw-rw-rw-   0        0        0    19040 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/elements.py
--rw-rw-rw-   0        0        0     1632 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/iter_parser.py
--rw-rw-rw-   0        0        0     8749 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/main.py
--rw-rw-rw-   0        0        0     2453 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/non_seq_constructor.py
--rw-rw-rw-   0        0        0     1603 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/parser.py
--rw-rw-rw-   0        0        0     2478 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/stream.py
--rw-rw-rw-   0        0        0     6848 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/tokens.py
--rw-rw-rw-   0        0        0     1462 2023-04-28 07:35:38.000000 nip-config-0.9.0/nip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.556112 nip-config-0.9.0/nip_config.egg-info/
--rw-rw-rw-   0        0        0      740 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 08:22:55.000000 nip-config-0.9.0/nip_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0      841 2023-04-28 08:22:55.559897 nip-config-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 08:22:55.557201 nip-config-0.9.0/tests/
--rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.9.0/tests/test_multi.py
--rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.9.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.155334 nip-config-0.9.1/
+-rw-rw-rw-   0        0        0     1082 2022-10-04 13:30:14.000000 nip-config-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      740 2023-04-28 08:29:03.155334 nip-config-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2022-10-04 13:30:14.000000 nip-config-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.141738 nip-config-0.9.1/nip/
+-rw-rw-rw-   0        0        0      137 2023-04-28 07:36:18.000000 nip-config-0.9.1/nip/__init__.py
+-rw-rw-rw-   0        0        0     5869 2023-04-28 07:37:49.000000 nip-config-0.9.1/nip/constructor.py
+-rw-rw-rw-   0        0        0     3078 2023-04-28 08:21:33.000000 nip-config-0.9.1/nip/convertor.py
+-rw-rw-rw-   0        0        0     1576 2023-04-28 08:28:10.000000 nip-config-0.9.1/nip/directives.py
+-rw-rw-rw-   0        0        0      807 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/dumper.py
+-rw-rw-rw-   0        0        0    19040 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/elements.py
+-rw-rw-rw-   0        0        0     1632 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/iter_parser.py
+-rw-rw-rw-   0        0        0     8749 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/main.py
+-rw-rw-rw-   0        0        0     2453 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/non_seq_constructor.py
+-rw-rw-rw-   0        0        0     1603 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/parser.py
+-rw-rw-rw-   0        0        0     2478 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/stream.py
+-rw-rw-rw-   0        0        0     6848 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/tokens.py
+-rw-rw-rw-   0        0        0     1462 2023-04-28 07:35:38.000000 nip-config-0.9.1/nip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.152953 nip-config-0.9.1/nip_config.egg-info/
+-rw-rw-rw-   0        0        0      740 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 08:29:03.000000 nip-config-0.9.1/nip_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2022-10-04 13:30:14.000000 nip-config-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2023-04-28 08:29:03.157369 nip-config-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 08:29:03.153988 nip-config-0.9.1/tests/
+-rw-rw-rw-   0        0        0      216 2023-03-29 19:27:12.000000 nip-config-0.9.1/tests/test_multi.py
+-rw-rw-rw-   0        0        0     1351 2023-03-29 17:47:22.000000 nip-config-0.9.1/tests/test_utils.py
```

### Comparing `nip-config-0.9.0/LICENSE` & `nip-config-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/PKG-INFO` & `nip-config-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.9.0
+Version: 0.9.1
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nip-config-0.9.0/README.md` & `nip-config-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/constructor.py` & `nip-config-0.9.1/nip/constructor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/convertor.py` & `nip-config-0.9.1/nip/convertor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/directives.py` & `nip-config-0.9.1/nip/directives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Contains nip directives."""
 
 
 import nip.parser  # This import pattern because of cycle imports
-import nip.elements
 import nip.constructor
 import nip.stream
 
 
 def insert_directive(right_value, stream: nip.stream.Stream):
-    if isinstance(right_value, nip.elements.Value):
+    from nip.elements import Value, Args
+    if isinstance(right_value, Value):
         constructor = nip.constructor.Constructor()
         path = constructor.construct(right_value)
         assert isinstance(path, str), "Load directive expects path as an argument."
         parser = nip.parser.Parser()
         config = parser.parse(path)  # nip.elements.Document
         return config.value
 
-    elif isinstance(right_value, nip.elements.Args):
+    elif isinstance(right_value, Args):
         assert len(right_value.value[0]) == 1, "only single positional argument will be treated as config path."
         constructor = nip.constructor.Constructor()
         path = constructor.construct(right_value.value[0][0])
         assert isinstance(path, str), "Load directive expects path as first argument."
         parser = nip.parser.Parser()
         parser.link_replacements = right_value.value[1]
         config = parser.parse(path)  # nip.elements.Document
```

### Comparing `nip-config-0.9.0/nip/dumper.py` & `nip-config-0.9.1/nip/dumper.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/elements.py` & `nip-config-0.9.1/nip/elements.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/iter_parser.py` & `nip-config-0.9.1/nip/iter_parser.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/main.py` & `nip-config-0.9.1/nip/main.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/non_seq_constructor.py` & `nip-config-0.9.1/nip/non_seq_constructor.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/parser.py` & `nip-config-0.9.1/nip/parser.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/stream.py` & `nip-config-0.9.1/nip/stream.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/tokens.py` & `nip-config-0.9.1/nip/tokens.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip/utils.py` & `nip-config-0.9.1/nip/utils.py`

 * *Files identical despite different names*

### Comparing `nip-config-0.9.0/nip_config.egg-info/PKG-INFO` & `nip-config-0.9.1/nip_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nip-config
-Version: 0.9.0
+Version: 0.9.1
 Summary: Advanced configs for python
 Home-page: https://github.com/spairet/nip
 Author: Ilya Vasiliev
 Author-email: spairet@bk.ru
 Project-URL: Guide, https://github.com/spairet/nip/tree/main/doc
 Project-URL: Issues, https://github.com/spairet/nip/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nip-config-0.9.0/setup.cfg` & `nip-config-0.9.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6970 2d63 6f6e 6669 670d 0a76   = nip-config..v
-00000020: 6572 7369 6f6e 203d 2030 2e39 2e30 0d0a  ersion = 0.9.0..
+00000020: 6572 7369 6f6e 203d 2030 2e39 2e31 0d0a  ersion = 0.9.1..
 00000030: 6175 7468 6f72 203d 2049 6c79 6120 5661  author = Ilya Va
 00000040: 7369 6c69 6576 0d0a 6175 7468 6f72 5f65  siliev..author_e
 00000050: 6d61 696c 203d 2073 7061 6972 6574 4062  mail = spairet@b
 00000060: 6b2e 7275 0d0a 6465 7363 7269 7074 696f  k.ru..descriptio
 00000070: 6e20 3d20 4164 7661 6e63 6564 2063 6f6e  n = Advanced con
 00000080: 6669 6773 2066 6f72 2070 7974 686f 6e0d  figs for python.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
```

### Comparing `nip-config-0.9.0/tests/test_utils.py` & `nip-config-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

