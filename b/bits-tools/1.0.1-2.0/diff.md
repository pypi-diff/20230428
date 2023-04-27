# Comparing `tmp/bits_tools-1.0.1.tar.gz` & `tmp/bits_tools-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_tools-1.0.1.tar", last modified: Mon Nov 21 23:02:59 2022, max compression
+gzip compressed data, was "bits_tools-2.0.tar", last modified: Wed Apr 26 22:47:29 2023, max compression
```

## Comparing `bits_tools-1.0.1.tar` & `bits_tools-2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 23:02:59.501402 bits_tools-1.0.1/
--rw-rw-rw-   0        0        0    35820 2022-11-20 21:13:01.000000 bits_tools-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      597 2022-11-21 23:02:59.496400 bits_tools-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       50 2022-11-21 22:58:53.000000 bits_tools-1.0.1/README.md
--rw-rw-rw-   0        0        0     4486 2022-11-19 23:39:12.000000 bits_tools-1.0.1/bits.py
-drwxrwxrwx   0        0        0        0 2022-11-21 23:02:59.489385 bits_tools-1.0.1/bits_tools.egg-info/
--rw-rw-rw-   0        0        0      597 2022-11-21 23:02:59.000000 bits_tools-1.0.1/bits_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2022-11-21 23:02:59.000000 bits_tools-1.0.1/bits_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-21 23:02:59.000000 bits_tools-1.0.1/bits_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-11-21 23:02:59.000000 bits_tools-1.0.1/bits_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2022-11-21 23:00:39.000000 bits_tools-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-21 23:02:59.501402 bits_tools-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 22:47:29.222280 bits_tools-2.0/
+-rw-rw-rw-   0        0        0    35820 2022-11-20 21:13:01.000000 bits_tools-2.0/LICENSE
+-rw-rw-rw-   0        0        0      595 2023-04-26 22:47:29.222280 bits_tools-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2022-11-21 22:58:53.000000 bits_tools-2.0/README.md
+-rw-rw-rw-   0        0        0     5419 2023-03-15 23:40:58.000000 bits_tools-2.0/bits.py
+drwxrwxrwx   0        0        0        0 2023-04-26 22:47:29.094133 bits_tools-2.0/bits_tools.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-04-26 22:47:28.000000 bits_tools-2.0/bits_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-26 22:47:28.000000 bits_tools-2.0/bits_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 22:47:28.000000 bits_tools-2.0/bits_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 22:47:28.000000 bits_tools-2.0/bits_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      729 2023-04-26 22:45:51.000000 bits_tools-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 22:47:29.222280 bits_tools-2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 22:47:29.110135 bits_tools-2.0/tests/
+-rw-rw-rw-   0        0        0     2324 2023-03-15 23:39:27.000000 bits_tools-2.0/tests/test_randombits.py
+-rw-rw-rw-   0        0        0     1531 2023-03-15 23:41:31.000000 bits_tools-2.0/tests/test_twobits.py
```

### Comparing `bits_tools-1.0.1/LICENSE` & `bits_tools-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bits_tools-1.0.1/PKG-INFO` & `bits_tools-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits_tools
-Version: 1.0.1
+Version: 2.0
 Summary: A Python package to simulate bits
 Author-email: Luke Villalobos <luke@bytesizeinfo.com>
 Project-URL: Homepage, https://github.com/LukeVilla/bits
 Project-URL: Bug Tracker, https://github.com/LukeVilla/bits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `bits_tools-1.0.1/bits.py` & `bits_tools-2.0/bits.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 import random
+from exceptions import InvalidBitsError
 class TwoBits(object):
     def __init__(self, bit1, bit2):
         self.bits = []
         self.bit = bit1
         self.bits.append(bit1)
         self.bits.append(bit2)
 
+    def get_bits(self):
+        return self.bits
+
+    def set_bits(self, newbits):
+        self.validate(newbits)
+        self.bits = newbits
+
+    @staticmethod
+    def validate(bits):
+        if len(bits) != 2:
+            raise InvalidBitsError("The number of bits must be 2")
+        for bit in bits:
+            if bit not in [0, 1]:
+                raise InvalidBitsError("Bits must be either 0 or 1")
+
     def andGate(self):
         """Implements a basic AND gate.
         Takes no arguments."""
         if self.bits[0] and self.bits[1]:
             return 1
         return 0
 
@@ -58,14 +74,29 @@
         return 0
 
 
 class RandomBits(object):
     def __init__(self, num_of_bits):
         self.bits = [random.randrange(0, 2) for _ in range(num_of_bits)]
 
+    def get_bits(self):
+        return self.bits
+
+    def set_bits(self, newbits):
+        self.validate(newbits)
+        self.bits = newbits
+
+    def validate(self, bits):
+        if len(self.bits) != len(bits):
+            raise InvalidBitsError("The number of bits must be " + str(len(self.bits)))
+        for bit in bits:
+            if bit not in [0, 1]:
+                raise InvalidBitsError("Bits must be either 0 or 1")
+            return True
+
     def andGate(self, otherBits):
         """Implements a basic AND gate.
         Takes one argument (otherBits), which is a list of bits."""
         results = []
         for i in range(len(self.bits)):
             if self.bits[i] and otherBits[i]:
                 results.append(1)
```

### Comparing `bits_tools-1.0.1/bits_tools.egg-info/PKG-INFO` & `bits_tools-2.0/bits_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits-tools
-Version: 1.0.1
+Version: 2.0
 Summary: A Python package to simulate bits
 Author-email: Luke Villalobos <luke@bytesizeinfo.com>
 Project-URL: Homepage, https://github.com/LukeVilla/bits
 Project-URL: Bug Tracker, https://github.com/LukeVilla/bits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

