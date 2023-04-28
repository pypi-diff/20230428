# Comparing `tmp/ixcom-1.3.1.tar.gz` & `tmp/ixcom-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixcom-1.3.1.tar", last modified: Mon Apr 24 15:34:41 2023, max compression
+gzip compressed data, was "ixcom-1.3.2.tar", last modified: Fri Apr 28 16:09:22 2023, max compression
```

## Comparing `ixcom-1.3.1.tar` & `ixcom-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-04-24 15:31:45.000000 ixcom-1.3.1/LICENSE
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-24 15:34:41.770173 ixcom-1.3.1/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-04-24 15:31:45.000000 ixcom-1.3.1/README.md
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/ixcom/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/__init__.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/cmdline.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/commands.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/crc16.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/data.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/exceptions.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/grep.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/parameters.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/parser.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/plugin_messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42100 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/protocol.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/ixcom.egg-info/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      415 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/SOURCES.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/dependency_links.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/entry_points.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/requires.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/top_level.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-04-24 15:34:41.770173 ixcom-1.3.1/setup.cfg
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-04-24 15:31:45.000000 ixcom-1.3.1/setup.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-28 16:09:22.349942 ixcom-1.3.2/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-04-28 16:07:36.000000 ixcom-1.3.2/LICENSE
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-28 16:09:22.349942 ixcom-1.3.2/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-04-28 16:07:36.000000 ixcom-1.3.2/README.md
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-28 16:09:22.349942 ixcom-1.3.2/ixcom/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/__init__.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/cmdline.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/commands.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/crc16.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/data.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/exceptions.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/grep.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/parameters.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/parser.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/plugin_messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42576 2023-04-28 16:07:36.000000 ixcom-1.3.2/ixcom/protocol.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-28 16:09:22.349942 ixcom-1.3.2/ixcom.egg-info/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      415 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/entry_points.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/requires.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-04-28 16:09:22.000000 ixcom-1.3.2/ixcom.egg-info/top_level.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-04-28 16:09:22.349942 ixcom-1.3.2/setup.cfg
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-04-28 16:07:36.000000 ixcom-1.3.2/setup.py
```

### Comparing `ixcom-1.3.1/LICENSE` & `ixcom-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/PKG-INFO` & `ixcom-1.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.1
+Version: 1.3.2
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.1/README.md` & `ixcom-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/cmdline.py` & `ixcom-1.3.2/ixcom/cmdline.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/commands.py` & `ixcom-1.3.2/ixcom/commands.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/crc16.py` & `ixcom-1.3.2/ixcom/crc16.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/grep.py` & `ixcom-1.3.2/ixcom/grep.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/messages.py` & `ixcom-1.3.2/ixcom/messages.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/parameters.py` & `ixcom-1.3.2/ixcom/parameters.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/parser.py` & `ixcom-1.3.2/ixcom/parser.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.1/ixcom/protocol.py` & `ixcom-1.3.2/ixcom/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,16 +410,18 @@
         d = {
             'b': 'int8_t',
             'B': 'uint8_t',
             'h': 'int16_t',
             'H': 'uint16_t',
             'i': 'int32_t',
             'I': 'uint32_t',
-            'l': 'int64_t',
-            'L': 'uint64_t',
+            'l': 'int32_t',
+            'L': 'uint32_t',
+            'q': 'int64_t',
+            'Q': 'uint64_t',
             'f': 'int8_t',
             'd': 'int8_t',
             's': 'char',
         }
         result = f'{d.get(self.datatype, "struct")} {self.name}'
         if self.dimension > 1:
             result += f' [{self.dimension}]'
@@ -440,15 +442,15 @@
                 struct_string += '%d' % self.dimension
             struct_string += self.datatype
         elif isinstance(self.datatype, Message):
             struct_string = self.datatype.get_struct_string()*self.dimension
         return struct_string
 
     def get_size(self):
-        basic_sizes = {'b': 1, 'B': 1, 's': 1, 'h': 2, 'H': 2, 'i': 4, 'I': 4, 'f': 4, 'd': 8, 'l': 8, 'L': 8}
+        basic_sizes = {'b': 1, 'B': 1, 's': 1, 'h': 2, 'H': 2, 'i': 4, 'I': 4, 'l': 4, 'L': 4, 'f': 4, 'd': 8, 'q': 8, 'Q': 8}
         if isinstance(self.datatype, str):
             return basic_sizes[self.datatype]*self.dimension
         elif isinstance(self.datatype, Message):
             return self.datatype.get_size()*self.dimension
 
     def get_null_item(self):
         if isinstance(self.datatype, str):
@@ -687,24 +689,30 @@
 
     @structString.setter
     def structString(self, value):
         self._structString = value
         self.struct_inst = struct.Struct(self._structString)
 
     def to_bytes(self):
-        values = []
-        for value in self.data.values():
-            if isinstance(value, (list, tuple)):
-                if isinstance(value[0], dict):
-                    for curd in value:
-                        values += curd.values()
+        def extract_values(diction):
+            values = []
+            for value in diction.values():
+                if isinstance(value, (list, tuple)):
+                    if len(value):
+                        if isinstance(value[0], dict):
+                            for curd in value:
+                                values +=extract_values(curd)
+                        else:
+                            values += value
+                elif isinstance(value, dict):
+                    values += extract_values(value)
                 else:
-                    values += value
-            else:
-                values += [value]
+                    values += [value]
+            return values
+        values = extract_values(self.data)
         return bytearray(self.struct_inst.pack(*values))
 
     def from_bytes(self, inBytes):
         if self.get_varsize_arg_from_bytes:
             _varsiz_arg = self.get_varsize_arg_from_bytes(inBytes)
             if _varsiz_arg != self._initarg:
                 self.__init__(_varsiz_arg)
@@ -781,15 +789,15 @@
         return struct_inst.iter_unpack(buffer)
 
     def get_numpy_dtype(self):
         struct_string = self.header.structString[1:] + self.payload.structString[1:] + self.bottom.structString[1:]
         current_item = ''
         item_list = []
         dtype_list = []
-        type_string = 'fdsbBhHiIlL'
+        type_string = 'fdsbBhHiIlLqQ'
         while len(struct_string) > 0:
             while struct_string[0] not in type_string:
                 current_item += struct_string[0]
                 struct_string = struct_string[1:]
             current_item += struct_string[0]
             struct_string = struct_string[1:]
             item_list.append(current_item)
@@ -802,21 +810,21 @@
             else:
                 cardinality = int(cardinality)
             dtype = item[-1]
             if dtype in 'bB':
                 byte_size = '1'
             elif dtype in 'hH':
                 byte_size = '2'
-            elif dtype in 'iIf':
+            elif dtype in 'iIflL':
                 byte_size = '4'
-            elif dtype in 'dLl':
+            elif dtype in 'dQq':
                 byte_size = '8'
-            if dtype in 'bhil':
+            if dtype in 'bhilq':
                 out_type = 'i'
-            elif dtype in 'BHIL':
+            elif dtype in 'BHILQ':
                 out_type = 'u'
             elif dtype in 'fd':
                 out_type = 'f'
             elif dtype in 's':
                 out_type = 'S'
 
             if out_type == 'S':
@@ -1129,14 +1137,18 @@
     for char in string:
         if char.isdigit():
             dimension += char
         else:
             datatype += char
     if dimension == '':
         dimension = '1'
+    if datatype == 'L':
+        datatype = 'Q'
+    if datatype == 'l':
+        datatype = 'q'
     return int(dimension), datatype
 
 def parse_payload_item(payload):
     messageList = []
     for idx in range(payload.__len__()):
         if "structFields" in payload[idx]:
             nestedMessageList = parse_payload_item(payload[idx]['structFields'])
```

### Comparing `ixcom-1.3.1/ixcom.egg-info/PKG-INFO` & `ixcom-1.3.2/ixcom.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.1
+Version: 1.3.2
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.1/setup.py` & `ixcom-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 if __name__ == '__main__':
 
     readmePath = os.path.join(os.path.dirname(__file__), 'README.md')
     long_description = open(readmePath, "rt").read()
 
     setup(name='ixcom',
-          version='1.3.1',
+          version='1.3.2',
           description='Library for communicating with xcom devices over network',
           author='iMAR Navigation GmbH',
           author_email='support@imar-navigation.de',
           url='http://www.imar-navigation.de',
           keywords=['XCOM', 'Inertial navigation', 'INS', 'iMAR', 'iNAT', 'GNSS', 'GPS', 'AHRS'],
           packages=['ixcom'],
           entry_points={
```

