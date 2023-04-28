# Comparing `tmp/vidimera-0.1.0-py3-none-any.whl.zip` & `tmp/vidimera-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 3635 bytes, number of entries: 7
--rw-r--r--  2.0 unx       78 b- defN 23-Apr-06 06:36 vidimera/__init__.py
--rw-r--r--  2.0 unx     1346 b- defN 23-Apr-28 09:17 vidimera/behaviour.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-28 09:51 vidimera-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2492 b- defN 23-Apr-28 09:51 vidimera-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 09:51 vidimera-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-28 09:51 vidimera-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-28 09:51 vidimera-0.1.0.dist-info/RECORD
-7 files, 5632 bytes uncompressed, 2671 bytes compressed:  52.6%
+Zip file size: 4583 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      205 b- defN 23-Apr-28 11:57 vidimera/__init__.py
+-rw-r--r--  2.0 unx      198 b- defN 23-Apr-28 12:02 vidimera/assertions.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Apr-28 11:11 vidimera/behaviour.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Apr-28 11:35 vidimera/missing_behaviour.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-28 12:15 vidimera-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2884 b- defN 23-Apr-28 12:15 vidimera-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 12:15 vidimera-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-28 12:15 vidimera-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      707 b- defN 23-Apr-28 12:15 vidimera-0.2.0.dist-info/RECORD
+9 files, 7118 bytes uncompressed, 3365 bytes compressed:  52.7%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: vidimera/__init__.py
 Comment: 
 
+Filename: vidimera/assertions.py
+Comment: 
+
 Filename: vidimera/behaviour.py
 Comment: 
 
-Filename: vidimera-0.1.0.dist-info/LICENSE
+Filename: vidimera/missing_behaviour.py
+Comment: 
+
+Filename: vidimera-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: vidimera-0.1.0.dist-info/METADATA
+Filename: vidimera-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: vidimera-0.1.0.dist-info/WHEEL
+Filename: vidimera-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: vidimera-0.1.0.dist-info/top_level.txt
+Filename: vidimera-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vidimera-0.1.0.dist-info/RECORD
+Filename: vidimera-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vidimera/__init__.py

```diff
@@ -1,4 +1,6 @@
+from .assertions import assert_implements
 from .behaviour import Behaviour
+from .missing_behaviour import MissingBehaviour
 
-__all__ = [Behaviour]
-__version__ = "0.1.0"
+__all__ = [assert_implements, Behaviour, MissingBehaviour]
+__version__ = "0.2.0"
```

## vidimera/behaviour.py

```diff
@@ -1,9 +1,10 @@
 from inspect import signature
 import re
+from .missing_behaviour import MissingBehaviour
 
 
 class Behaviour:
     NO_SIGNATURE = object()
     PUBLIC = r"[a-zA-Z]\w*"
     PRIVATE = f"_{PUBLIC}"
     SPECIAL = r"__\w+__"
@@ -19,15 +20,15 @@
     def __repr__(self):
         return f"<Behaviour of {repr(self.obj)}>"
 
     def implemented_by(self, other):
         return self.__class__(other).implements(self)
 
     def implements(self, other):
-        return self.signatures() >= self.__class__(other).signatures()
+        return MissingBehaviour(self.__class__(other).signatures() - self.signatures())
 
     def signatures(self, scope=PUBLIC_AND_SPECIAL):
         pattern = re.compile(scope)
         contents = dir(self.obj)
         included = filter(pattern.match, contents)
         candidates = map(self._name_and_attribute, included)
         callables = filter(_callable, candidates)
```

## Comparing `vidimera-0.1.0.dist-info/LICENSE` & `vidimera-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vidimera-0.1.0.dist-info/METADATA` & `vidimera-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidimera
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python signature and behaviour checker inspired by Elixir.
 Home-page: https://github.com/DevL/vidimera
 Author: Lennart Fridén
 Author-email: lennart@devl.se
 License: MIT
 Project-URL: Bug Reports, https://github.com/DevL/vidimera/issues
 Project-URL: Source, https://github.com/DevL/vidimera
@@ -30,19 +30,22 @@
 
 _Python signature and behaviour checker inspired by Elixir._
 
 In Swedish, _vidimera_ means _to attest_ or _to certify_. It is commonly used to attest that a copy of a document is accurate compared to the original.
 
 ## Installation
 
-Install the package `vidimera` version `0.1+` from PyPI.
-The recommended `requirements.txt` line is `vidimera~=0.1`.
+Install the package `vidimera` version `0.2+` from PyPI.
+The recommended `requirements.txt` line is `vidimera~=0.2`.
 
 ## Current Functionality
 
+### `assert_implements(object, expected)`
+- Raises an `AssertionError` listing missing callables and their signatures if there are any. Based on `behaviour.implements`.
+
 ### `Behaviour(object)`
 - Creates a new `Behaviour` instance.
 - If `object` already is an instance of `Behaviour`, it is returned unchanged.
 
 ### `behaviour.implemented_by(other)`
 - Verifies that `other` at least has the same public and dunderscore callables with the same signatures as the `behaviour`.
 - Creats a `Behaviour` from `other` before making the comparison.
@@ -50,7 +53,10 @@
 ### `behaviour.implements(other)`
 - Verifies that the `behaviour` at least has the same public and dunderscore callables with the same signatures as `other`.
 - Creats a `Behaviour` from `other` before making the comparison.
 
 ### `behaviour.signatures(scope=Behaviour.PUBLIC_AND_SPECIAL)`
 - Returns a `set` of tuples that represent the name and the callable selected based on the `scope`.
 - Possible scopes include `PUBLIC`, `PRIVATE`, `SPECIAL`, and `PUBLIC_AND_SPECIAL`.
+
+### `MissingBehaviour(delta)`
+- An internal representation of missing behaviour. Created from a set of names and signatures. If the set is empty, this object will be truthy. If the set is non-empty, this object is falsy.
```

