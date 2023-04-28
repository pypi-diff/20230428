# Comparing `tmp/py_fumen-0.1.3.tar.gz` & `tmp/py_fumen-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_fumen-0.1.3.tar", last modified: Fri Mar 24 19:22:11 2023, max compression
+gzip compressed data, was "py_fumen-0.1.4.tar", last modified: Fri Apr 28 04:04:53 2023, max compression
```

## Comparing `py_fumen-0.1.3.tar` & `py_fumen-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 19:22:11.373443 py_fumen-0.1.3/
--rw-rw-rw-   0        0        0     1068 2022-09-29 08:36:48.000000 py_fumen-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2038 2023-03-24 19:22:11.373443 py_fumen-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1417 2022-11-21 17:49:34.000000 py_fumen-0.1.3/README.md
--rw-rw-rw-   0        0        0      549 2023-03-24 19:20:23.000000 py_fumen-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-03-24 19:22:11.374449 py_fumen-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-03-24 19:20:19.000000 py_fumen-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 19:22:11.114650 py_fumen-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-24 19:22:11.240634 py_fumen-0.1.3/src/py_fumen/
--rw-rw-rw-   0        0        0      212 2022-11-21 17:54:49.000000 py_fumen-0.1.3/src/py_fumen/__init__.py
--rw-rw-rw-   0        0        0     5961 2023-02-24 10:34:04.000000 py_fumen-0.1.3/src/py_fumen/action.py
--rw-rw-rw-   0        0        0      788 2023-02-24 10:40:35.000000 py_fumen-0.1.3/src/py_fumen/comments.py
--rw-rw-rw-   0        0        0      305 2022-12-14 11:54:50.000000 py_fumen-0.1.3/src/py_fumen/constants.py
--rw-rw-rw-   0        0        0     7758 2023-02-24 13:48:43.000000 py_fumen-0.1.3/src/py_fumen/decoder.py
--rw-rw-rw-   0        0        0     2190 2023-03-21 09:24:37.000000 py_fumen-0.1.3/src/py_fumen/defines.py
--rw-rw-rw-   0        0        0     7907 2023-02-24 13:48:43.000000 py_fumen-0.1.3/src/py_fumen/encoder.py
--rw-rw-rw-   0        0        0     4969 2022-09-29 09:17:40.000000 py_fumen-0.1.3/src/py_fumen/field.py
--rw-rw-rw-   0        0        0     1810 2022-09-29 09:17:40.000000 py_fumen-0.1.3/src/py_fumen/fumen_buffer.py
--rw-rw-rw-   0        0        0    10381 2022-12-13 20:15:12.000000 py_fumen-0.1.3/src/py_fumen/inner_field.py
--rw-rw-rw-   0        0        0      829 2022-11-19 17:55:09.000000 py_fumen-0.1.3/src/py_fumen/js_escape.py
--rw-rw-rw-   0        0        0     1430 2023-02-24 10:19:37.000000 py_fumen-0.1.3/src/py_fumen/page.py
--rw-rw-rw-   0        0        0     6169 2023-03-24 19:18:07.000000 py_fumen-0.1.3/src/py_fumen/quiz.py
-drwxrwxrwx   0        0        0        0 2023-03-24 19:22:11.371938 py_fumen-0.1.3/src/py_fumen.egg-info/
--rw-rw-rw-   0        0        0     2038 2023-03-24 19:22:11.000000 py_fumen-0.1.3/src/py_fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2022-12-20 23:19:09.000000 py_fumen-0.1.3/src/py_fumen.egg-info/PKG-INFO-Parker
--rw-rw-rw-   0        0        0      551 2023-03-24 19:22:11.000000 py_fumen-0.1.3/src/py_fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 19:22:11.000000 py_fumen-0.1.3/src/py_fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-24 19:22:11.000000 py_fumen-0.1.3/src/py_fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 04:04:53.292611 py_fumen-0.1.4/
+-rw-rw-rw-   0        0        0     1068 2022-09-29 08:36:48.000000 py_fumen-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      293 2023-04-28 04:04:53.293609 py_fumen-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2022-11-21 17:49:34.000000 py_fumen-0.1.4/README.md
+-rw-rw-rw-   0        0        0      553 2023-04-28 04:01:30.000000 py_fumen-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-04-28 04:04:53.296599 py_fumen-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-04-28 04:01:36.000000 py_fumen-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:04:53.155075 py_fumen-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 04:04:53.237794 py_fumen-0.1.4/src/py_fumen/
+-rw-rw-rw-   0        0        0      212 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/__init__.py
+-rw-rw-rw-   0        0        0     5636 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/action.py
+-rw-rw-rw-   0        0        0      632 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/comments.py
+-rw-rw-rw-   0        0        0      305 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/constants.py
+-rw-rw-rw-   0        0        0     7897 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/decoder.py
+-rw-rw-rw-   0        0        0     2191 2023-04-28 03:52:51.000000 py_fumen-0.1.4/src/py_fumen/defines.py
+-rw-rw-rw-   0        0        0     7938 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/encoder.py
+-rw-rw-rw-   0        0        0     4969 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/field.py
+-rw-rw-rw-   0        0        0     1810 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/fumen_buffer.py
+-rw-rw-rw-   0        0        0    10381 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/inner_field.py
+-rw-rw-rw-   0        0        0      829 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/js_escape.py
+-rw-rw-rw-   0        0        0     1386 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/page.py
+-rw-rw-rw-   0        0        0     6106 2023-04-28 03:52:52.000000 py_fumen-0.1.4/src/py_fumen/quiz.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:04:53.291614 py_fumen-0.1.4/src/py_fumen.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-04-28 04:04:53.000000 py_fumen-0.1.4/src/py_fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-03-01 05:11:02.000000 py_fumen-0.1.4/src/py_fumen.egg-info/PKG-INFO-DESKTOP-PUKF6DK
+-rw-rw-rw-   0        0        0      294 2022-12-20 23:19:09.000000 py_fumen-0.1.4/src/py_fumen.egg-info/PKG-INFO-Parker
+-rw-rw-rw-   0        0        0      598 2023-04-28 04:04:53.000000 py_fumen-0.1.4/src/py_fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 04:04:53.000000 py_fumen-0.1.4/src/py_fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 04:04:53.000000 py_fumen-0.1.4/src/py_fumen.egg-info/top_level.txt
```

### Comparing `py_fumen-0.1.3/LICENSE` & `py_fumen-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/PKG-INFO` & `py_fumen-0.1.4/src/py_fumen.egg-info/PKG-INFO-DESKTOP-PUKF6DK`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_fumen
-Version: 0.1.3
+Name: py-fumen
+Version: 0.1.0
 Summary: Python implementation of knewjade's fumen
 Home-page: https://github.com/hsohliyt105/py-fumen
 Author: hsohliyt105
 Author-email: hsohliyt105 <hsohliyt105@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/hsohliyt105/py-fumen
 Keywords: fumen
```

### Comparing `py_fumen-0.1.3/README.md` & `py_fumen-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/pyproject.toml` & `py_fumen-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-[build-system]
+    [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_fumen"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="hsohliyt105", email="hsohliyt105@gmail.com" },
 ]
 description = "Python implementation of knewjade's fumen"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `py_fumen-0.1.3/src/py_fumen/action.py` & `py_fumen-0.1.4/src/py_fumen/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from dataclasses import dataclass
 from math import floor
 from typing import Tuple
 
 from .defines import is_mino_piece, InnerOperation, Piece, Rotation
+from .constants import FieldConstants
 
 @dataclass
 class Action():
     piece: InnerOperation
     rise: bool
     mirror: bool
     colorize: bool
@@ -18,43 +19,39 @@
 def decode_bool(n: int):
     return n != 0
 
 class ActionDecoder() :
     width: int
     field_top: int
     garbage_line: int
-    field_max_height: int
-    num_field_blocks: int
 
     def __init__(self, width: int, field_top: int, garbage_line: int):
         self.width = width
         self.field_top = field_top
         self.garbage_line = garbage_line
-        self.field_max_height = field_top + garbage_line
-        self.num_field_blocks = self.field_max_height * width
 
     class PieceException(Exception):
         pass
 
     class RotationException(Exception):
         pass
 
     @staticmethod
     def decode_piece(n: int) -> Piece:
         if n in range(0, 9):
             return Piece(n)
 
-        raise ActionDecoder.PieceException(f'Unexpected piece: {n} (0~8)')
+        raise ActionDecoder.PieceException('Unexpected piece')
 
     @staticmethod
     def decode_rotation(n: int) -> Rotation:
         if n in range(0, 4):
             return Rotation(n)
 
-        raise ActionDecoder.RotationException(f'Unexpected rotation: {n} (0~3)')
+        raise ActionDecoder.RotationException('Unexpected rotation')
 
     def decode_coordinate(self, n: int, piece: Piece, rotation: Rotation) -> Tuple[int, int]:
         x = n % self.width
         ORIGIN_Y = floor(n / 10)
         y = self.field_top - ORIGIN_Y - 1
 
         if piece is Piece.O and rotation is Rotation.LEFT:
@@ -81,16 +78,16 @@
 
     def decode(self, v: int) -> Action:
         value = v
         piece_type = self.decode_piece(value % 8)
         value = floor(value / 8)
         rotation = self.decode_rotation(value % 4)
         value = floor(value / 4)
-        coordinate = self.decode_coordinate(value % self.num_field_blocks, piece_type, rotation)
-        value = floor(value / self.num_field_blocks)
+        coordinate = self.decode_coordinate(value % FieldConstants.MAX_BLOCKS, piece_type, rotation)
+        value = floor(value / FieldConstants.MAX_BLOCKS)
         is_block_up = decode_bool(value % 2)
         value = floor(value / 2)
         is_mirror = decode_bool(value % 2)
         value = floor(value / 2)
         is_color = decode_bool(value % 2)
         value = floor(value / 2)
         is_comment = decode_bool(value % 2)
@@ -113,23 +110,19 @@
 def encode_bool(flag: bool) -> int:
     return 1 if flag else 0
 
 class ActionEncoder():
     width: int
     field_top: int
     garbage_line: int
-    field_max_height: int
-    num_field_blocks: int
 
     def __init__(self, width: int, field_top: int, garbage_line: int):
         self.width = width
         self.field_top = field_top
         self.garbage_line = garbage_line
-        self.field_max_height = field_top + garbage_line
-        self.num_field_blocks = self.field_max_height * width
 
     def encode_position(self, operation: InnerOperation) -> int:
         piece_type = operation.piece_type
         rotation = operation.rotation
         x = operation.x
         y = operation.y
 
@@ -165,27 +158,27 @@
     def encode_rotation(operation: InnerOperation) -> int:
         if not is_mino_piece(operation.piece_type):
             return 0
 
         if isinstance(operation.rotation, Rotation):
             return operation.rotation.value
 
-        raise ActionEncoder.NonReachableException('No reachable rotation')
+        raise ActionEncoder.NonReachableException('No reachable')
 
     def encode(self, action: Action) -> int:
         value = encode_bool(not action.lock)
         value *= 2
         value += encode_bool(action.comment)
         value *= 2
         value += encode_bool(action.colorize)
         value *= 2
         value += encode_bool(action.mirror)
         value *= 2
         value += encode_bool(action.rise)
-        value *= self.num_field_blocks
+        value *= FieldConstants.MAX_BLOCKS
         value += self.encode_position(action.piece)
         value *= 4
         value += self.encode_rotation(action.piece)
         value *= 8
         value += action.piece.piece_type.value
 
         return value
```

### Comparing `py_fumen-0.1.3/src/py_fumen/comments.py` & `py_fumen-0.1.4/src/py_fumen/comments.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,11 +13,8 @@
             index = value % MAX_COMMENT_CHAR_VALUE
             string += COMMENT_TABLE[index]
             value = floor(value / MAX_COMMENT_CHAR_VALUE)
 
         return string
 
     def encode(ch: str, count: int) -> int:
-        try:
-            return COMMENT_TABLE.index(ch) * (MAX_COMMENT_CHAR_VALUE ** count)
-        except:
-            raise ValueError(f"Encoding character not in the comment table: {ch} (suggestedly wrong encoding, non utf-8)")
+        return COMMENT_TABLE.index(ch) * (MAX_COMMENT_CHAR_VALUE ** count)
```

### Comparing `py_fumen-0.1.3/src/py_fumen/decoder.py` & `py_fumen-0.1.4/src/py_fumen/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     for version in [ "115", "110" ]:
         for prefix in [ "v", "m", "d" ]:
             match = string.find(prefix+version)
             if match != -1:
                 sub = data[match + 5:]
                 return format_data(version, sub)
 
-    raise VersionException(f"Unsupported fumen version: {string} (must be (v|m|d)(115|110))")
+    raise VersionException("Unsupported fumen version")
 
 def decode(fumen: str) -> List[Page]:
     version, data = extract(fumen)
     if version == "115":
         return inner_decode(data, 23)
     if version == "110":
         return inner_decode(data, 21)
 
-    raise VersionException(f"Unsupported fumen version: {fumen} (must be (v|m|d)(115|110))")
+    raise VersionException("Unsupported fumen version")
 
 @dataclass
 class RefIndex():
     comment: int
     field: int
 
 @dataclass
@@ -212,14 +212,21 @@
                                                    current_piece.y))
                                          if current_piece is not None else None,
                           comment.text if comment.text is not None else store.last_comment_text,
                           Flags(action.lock, action.mirror, action.colorize, action.rise, quiz),
                           Refs(field=field.ref, comment=comment.ref)
                           ))
 
+        """ callback(
+            currentFieldObj.field.copy()
+            , currentPiece
+            , store.quiz !== undefined ? store.quiz.format().toString() : store.lastCommentText,
+            )
+        """
+
         page_index += 1
 
         if action.lock:
             if is_mino_piece(action.piece.piece_type):
                 current_field_obj.field.fill(action.piece)
 
             current_field_obj.field.clear_line()
```

### Comparing `py_fumen-0.1.3/src/py_fumen/defines.py` & `py_fumen-0.1.4/src/py_fumen/defines.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     raise RotationException(f'Unknown rotation: {rotation}')
 
 @dataclass
 class InnerOperation():
     piece_type: Piece
     rotation: Rotation
     x: int
-    y: int
+    y: int
```

### Comparing `py_fumen-0.1.3/src/py_fumen/encoder.py` & `py_fumen-0.1.4/src/py_fumen/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from typing import List, Optional, Tuple
+from urllib.parse import quote
 from re import findall
 
 from .page import Page, Flags
 from .inner_field import InnerField
 from .fumen_buffer import FumenBuffer
 from .field import create_inner_field, create_new_inner_field, Field, Operation
 from .defines import is_mino_piece, parse_piece, parse_rotation, Piece, Rotation, InnerOperation
```

### Comparing `py_fumen-0.1.3/src/py_fumen/field.py` & `py_fumen-0.1.4/src/py_fumen/field.py`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/src/py_fumen/fumen_buffer.py` & `py_fumen-0.1.4/src/py_fumen/fumen_buffer.py`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/src/py_fumen/inner_field.py` & `py_fumen-0.1.4/src/py_fumen/inner_field.py`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/src/py_fumen/js_escape.py` & `py_fumen-0.1.4/src/py_fumen/js_escape.py`

 * *Files identical despite different names*

### Comparing `py_fumen-0.1.3/src/py_fumen/page.py` & `py_fumen-0.1.4/src/py_fumen/page.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from dataclasses import dataclass
-from typing import Optional
+from typing import List, Optional, Tuple
+from math import floor
+from urllib.parse import unquote
 
 from .inner_field import InnerField
 from .field import Field, Mino, Operation, create_inner_field
 
 @dataclass
 class Flags():
     lock: Optional[bool] = True
@@ -25,23 +27,23 @@
     operation: Optional[Operation]
     comment: Optional[str]
     flag: Optional[Flags]
     refs: Optional[Refs]
 
     def __init__(self, index: Optional[int] = None, field: Optional[InnerField] = None, operation: Optional[Operation] = None, comment: Optional[str] = None, flags: Optional[Flags] = None, refs: Optional[Refs] = None):
         self.index = index
-        self.__field = field.copy() if isinstance(field, InnerField) else None
+        self.__field = field.copy()
         self.operation = operation
         self.comment = comment
         self.flags = flags
         self.refs = refs
 
         return
 
     def get_field(self) -> Field:
-        return None if self.__field is None else Field(self.__field.copy())
+        return Field(self.__field.copy())
 
     def set_field(self, field: Field):
         self.__field = create_inner_field(field)
 
     def mino(self) -> Mino:
-        return None if self.operation is None else Mino.minoFrom(self.operation)
+        return Mino.minoFrom(self.operation)
```

### Comparing `py_fumen-0.1.3/src/py_fumen/quiz.py` & `py_fumen-0.1.4/src/py_fumen/quiz.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,115 +34,113 @@
 
         return replaced
 
     def __init__(self, quiz: str):
         self.quiz = self.__verify(quiz)
 
     def next(self) -> str:
-        index = self.quiz.index(')') + 1
-        name = self.quiz[index:]
+        index = self.quiz.find(')') + 1
+        name = self.quiz[index]
 
         if name is None or name == ';':
             return ''
 
         return name
 
     @staticmethod
     def is_quiz_comment(comment: str) -> bool:
         return comment.startswith('#Q=')
 
     @staticmethod
-    def create(nexts: str) -> Quiz:
-        return Quiz(f"#Q=[]({nexts[0]}){nexts[1:]}")
-
-    @staticmethod
-    def create(hold: str, nexts: str) -> Quiz:        
-        return Quiz(f"#Q=[{hold}]({nexts[0]}){nexts[1:]}")
+    def create(first: str, second: Optional[str]=None) -> Quiz:
+        if second is None:
+            return Quiz(f"#Q=[]({first[0]}){first[1:]}")
+        return Quiz(f"#Q=[{first}]({second[0]}){second[1:]}")
 
     def least(self) -> str:
-        index = self.quiz.index(')')
+        index = self.quiz.find(')')
         return self.quiz[index+1:]
 
     def current(self) -> str:
-        index = self.quiz.index('(') + 1
+        index = self.quiz.find('(') + 1
         name = self.quiz[index]
         if name == ')':
             return ''
 
         return name
 
     def hold(self) -> str:
-        index = self.quiz.index('[') + 1
+        index = self.quiz.find('[') + 1
         name = self.quiz[index]
         if name == ']':
             return ''
 
         return name
 
     def least_after_next2(self) -> str:
-        index = self.quiz.index(')')
+        index = self.quiz.find(')')
         if self.quiz[index+1] == ';':
             return self.quiz[index+1:]
 
-        return self.quiz.substr[index+2:]
+        return self.quiz[index+2:]
 
     class HoldException(Exception):
         pass
 
     def get_operation(self, used: Piece) -> Operation:
         used_name = parse_piece_name(used)
         current = self.current()
         if used_name == current:
             return Operation.DIRECT
 
         hold = self.hold()
         if used_name == hold:
             return Operation.SWAP
-        
+
         if hold == '':
             if used_name == self.next():
                 return Operation.STOCK
 
         else:
             if current == '' and used_name == self.next():
                 return Operation.DIRECT
 
         raise self.HoldException(f"Unexpected hold piece in quiz: {self.quiz}")
 
     def least_in_active_bag(self) -> str:
-        separate_index = self.quiz.index(';')
-        quiz = self.quiz[0, separate_index] if 0 <= separate_index else self.quiz
-        index = quiz.indexOf(')')
+        separate_index = self.quiz.find(';')
+        quiz = self.quiz[0:separate_index] if 0 <= separate_index else self.quiz
+        index = quiz.find(')')
         if quiz[index+1] == ';':
             return quiz[index+1:]
 
-        return quiz.substr[index+2:]
+        return quiz[index+2:]
 
     def direct(self) -> Quiz:
         if self.current() == '':
             least = self.least_after_next2()
             return Quiz(f"#Q=[{self.hold()}]({least[0]}){least[1:]}")
 
-        return Quiz("#Q=[{self.hold}](${self.next()})${self.leastAfterNext2()}")
+        return Quiz(f"#Q=[{self.hold()}]({self.next()}){self.least_after_next2()}")
 
     def swap(self) -> Quiz:
         if self.hold() == '':
             raise self.HoldException(f"Cannot find hold piece: {self.quiz}")
 
         next = self.next()
-        return Quiz(f"#Q=[${self.current()}]({next})${self.leastAfterNext2()}")
+        return Quiz(f"#Q=[{self.current()}]({next}){self.least_after_next2()}")
 
     class StockException(Exception):
         pass
 
     def stock(self) -> Quiz:
         if self.hold() != '' or self.next() == '':
              raise self.StockException(f"Cannot stock: {self.quiz}")
 
-        least = self.leastAfterNext2()
+        least = self.least_after_next2()
         head = least[0] if least[0] is not None else ''
 
         if 1 < len(least):
             return Quiz(f"#Q=[{self.current()}]({head}){least[1:]}")
 
         return Quiz(f"#Q=[{self.current()}]({head})")
 
@@ -152,15 +150,15 @@
     def operate(self, operation: Operation) -> Quiz:
         if operation is Operation.DIRECT:
             return self.direct()
         if operation is  Operation.SWAP:
             return self.swap()
         if operation is  Operation.STOCK:
             return self.stock()
-        
+
         raise self.OperationException('Unexpected operation')
 
     def can_operate(self) -> bool:
         quiz = self.quiz
         if quiz.startswith('#Q=[]();'):
             quiz = self.quiz[8:]
 
@@ -169,23 +167,22 @@
     def get_hold_piece(self) -> Piece:
         if not self.can_operate():
             return Piece.EMPTY
 
         name = self.hold()
         if name is None or name == '' or name == ';':
             return Piece.EMPTY
-        
+
         return parse_piece(name)
 
     def get_next_pieces(self, maximum: Optional[int] = None) -> List[Piece]:
         if not self.can_operate():
             return [Piece.EMPTY] * maximum if maximum is not None else []
-        
 
-        names = self.current() + self.next() + self.least_in_active_bag()[0, maximum]
+        names = (self.current() + self.next() + self.least_in_active_bag())[0:maximum]
         if maximum is not None and len(names) < maximum:
             names += ' ' * (maximum - len(names))
 
         return [Piece.EMPTY if name is None or name == ' ' or name == ';' else parse_piece_name(name) for name in [*names]]
 
     def to_string(self) -> str:
         return self.quiz
@@ -214,8 +211,8 @@
                 return Quiz('')
 
             if head == ';':
                 return Quiz(least[1:])
 
             return Quiz(f"#Q=[]({head}){least[1:]}")
 
-        return quiz
+        return quiz
```

### Comparing `py_fumen-0.1.3/src/py_fumen.egg-info/SOURCES.txt` & `py_fumen-0.1.4/src/py_fumen.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 src/py_fumen/field.py
 src/py_fumen/fumen_buffer.py
 src/py_fumen/inner_field.py
 src/py_fumen/js_escape.py
 src/py_fumen/page.py
 src/py_fumen/quiz.py
 src/py_fumen.egg-info/PKG-INFO
+src/py_fumen.egg-info/PKG-INFO-DESKTOP-PUKF6DK
 src/py_fumen.egg-info/PKG-INFO-Parker
 src/py_fumen.egg-info/SOURCES.txt
 src/py_fumen.egg-info/dependency_links.txt
 src/py_fumen.egg-info/top_level.txt
```

