# Comparing `tmp/trlc-1.0.9.tar.gz` & `tmp/trlc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trlc-1.0.9.tar", last modified: Wed Mar  1 11:00:03 2023, max compression
+gzip compressed data, was "trlc-1.1.1.tar", last modified: Fri Apr 28 09:17:19 2023, max compression
```

## Comparing `trlc-1.0.9.tar` & `trlc-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/
--rw-r--r--   0 florian   (1000) florian   (1000)     3406 2023-03-01 11:00:03.000000 trlc-1.0.9/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.0.9/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-03-01 11:00:03.000000 trlc-1.0.9/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.0.9/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    78894 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6958 2022-12-14 13:45:21.000000 trlc-1.0.9/trlc/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14323 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1000 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/lint.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1003 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/math.py
--rw-r--r--   0 florian   (1000) florian   (1000)    40651 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    12920 2023-02-07 11:53:43.000000 trlc-1.0.9/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-03-01 10:58:55.000000 trlc-1.0.9/trlc/version.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3406 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      299 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       41 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.1/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-04-28 09:17:19.584583 trlc-1.1.1/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.1/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-04-28 09:17:19.584583 trlc-1.1.1/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.1/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    96271 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7240 2023-04-12 08:39:07.000000 trlc-1.1.1/trlc/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15405 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/lint.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.1/trlc/math.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.1/trlc/nested.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    58600 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.1/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-04-28 09:17:12.000000 trlc-1.1.1/trlc/version.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-28 09:17:19.584583 trlc-1.1.1/trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-04-28 09:17:19.000000 trlc-1.1.1/trlc.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trlc-1.0.9/PKG-INFO` & `trlc-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.0.9
+Version: 1.1.1
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/trlc
-Description: # Treat Requirements Like Code (TRLC)
-        TRLC is a domain-specific language developed at BMW for writing (and
-        linking) requirements with meta-data.
-        
-        The repository contains:
-        
-        * The [language reference
-          manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-          for TRLC.
-        
-        * A pure Python reference implementation of TRLC.
-        
-        The implementation is not very fast, but designed to be pedantically
-        correct in following the language definition.  Eventually it will also
-        contain a powerful linter to find issues with types and check
-        rules.
-        
-        The Python implementation can be used for several purposes:
-        
-        * It can be used to validate other TRLC implementations.
-        
-        * It can be used to validate a body of requirements (e.g. a CI check
-          that all requirements are well formed)
-        
-        * The API can be used to write other tools based on TRLC (for example
-          a tool to render the requirements in HTML, a tool to diff
-          requirements or perform an impact analysis, or a tool to perform
-          software traceability, etc.)
-        
-        ## Documentation
-        
-        * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
-        * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
-        * [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
-          (user guide for using the API)
-        * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-          (for language lawyers)
-        * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
-        
-        ## Dependencies
-        
-        ### Run-time
-        * Python3 >= 3.7
-        
-        ### Development tools
-        * GNU Make
-        * [PyCodeStyle](https://pypi.org/project/pycodestyle/) (from PyPI, for
-          basic checking of source code style)
-        * [PyLint](https://pypi.org/project/pylint/) (from PyPI, for basic bug
-          finding)
-        * [Coverage](https://pypi.org/project/coverage/) (from PyPI, to
-          perform branch coverage when running the test suite)
-        * [Sphinx](https://pypi.org/project/Sphinx/) (from PyPI, for building
-          the documentation)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Treat Requirements Like Code (TRLC)
+TRLC is a domain-specific language developed at BMW for writing (and
+linking) requirements with meta-data.
+
+The repository contains:
+
+* The [language reference
+  manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+  for TRLC.
+
+* A pure Python reference implementation of TRLC.
+
+The implementation is not very fast, but designed to be pedantically
+correct in following the language definition.  Eventually it will also
+contain a powerful linter to find issues with types and check
+rules.
+
+The Python implementation can be used for several purposes:
+
+* It can be used to validate other TRLC implementations.
+
+* It can be used to validate a body of requirements (e.g. a CI check
+  that all requirements are well formed)
+
+* The API can be used to write other tools based on TRLC (for example
+  a tool to render the requirements in HTML, a tool to diff
+  requirements or perform an impact analysis, or a tool to perform
+  software traceability, etc.)
+
+## Documentation
+
+* [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
+* [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
+* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
+  (user guide for using the API)
+* [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+  (for language lawyers)
+* [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
+
+## Dependencies
+
+### Run-time
+* Python3 >= 3.7
+
+### Development tools
+* GNU Make
+* [PyCodeStyle](https://pypi.org/project/pycodestyle/) (from PyPI, for
+  basic checking of source code style)
+* [PyLint](https://pypi.org/project/pylint/) (from PyPI, for basic bug
+  finding)
+* [Coverage](https://pypi.org/project/coverage/) (from PyPI, to
+  perform branch coverage when running the test suite)
+* [Sphinx](https://pypi.org/project/Sphinx/) (from PyPI, for building
+  the documentation)
```

### Comparing `trlc-1.0.9/README.md` & `trlc-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `trlc-1.0.9/setup.py` & `trlc-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.9/trlc/__init__.py` & `trlc-1.1.1/trlc/__init__.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.9/trlc/ast.py` & `trlc-1.1.1/trlc/ast.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
 # TRLC - Treat Requirements Like Code
-# Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
+# Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This file is part of the TRLC Python Reference Implementation.
 #
 # TRLC is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -20,14 +20,15 @@
 
 import re
 
 from copy import copy
 from difflib import get_close_matches
 from enum import Enum, auto
 from collections import OrderedDict
+from fractions import Fraction
 
 from trlc.errors import Location, Message_Handler
 from trlc.lexer import Token
 from trlc import math
 
 #
 # This module defines the AST and related object for the TRLC
@@ -49,38 +50,40 @@
 
     Any record references will be fully resolved.
 
     :attribute location: source location this value comes from
     :type: Location
 
     :attribute value: the value or None (for null values)
-    :type: str, int, bool, list[Value], Record_Reference, \
-    Enumeration_Literal_Spec
+    :type: str, int, bool, fractions.Fraction, list[Value], \
+    Record_Reference, Enumeration_Literal_Spec
 
     :attribute typ: type of the value (or None for null values)
     :type: Type
     """
     def __init__(self, location, value, typ):
         assert isinstance(location, Location)
         assert value is None or \
             isinstance(value, (str,
                                int,
                                bool,
-                               list,
+                               list,  # for arrays
+                               dict,  # for tuples
+                               Fraction,
                                Record_Reference,
                                Enumeration_Literal_Spec))
         assert typ is None or isinstance(typ, Type)
         assert (typ is None) == (value is None)
 
         self.location = location
         self.value    = value
         self.typ      = typ
 
     def __eq__(self, other):
-        return self.value == other.value
+        return self.typ == other.typ and self.value == other.value
 
     def __repr__(self):  # pragma: no cover
         return "Value(%s)" % self.value
 
     def resolve_references(self, mh):
         assert isinstance(mh, Message_Handler)
 
@@ -115,19 +118,21 @@
         :class:`Symbol_Table`, and can be very helpful for debugging
         or understanding the parse tree. The dump methods will produce
         output like this::
 
             Symbol_Table
                Builtin_Boolean
                Builtin_Integer
+               Builtin_Decimal
                Builtin_String
+               Builtin_Markup_String
                Package bar
                   Symbol_Table
                      Record_Type MyType
-                        Record_Component name
+                        Composite_Component name
                            Optional: False
                            Type: String
                         Checks
                            Error 'description is too short'
                               Anchor: description
                               Binary Binary_Operator.COMP_GT Expression
                                  Type: Boolean
@@ -159,41 +164,41 @@
 
     This represent a single user-defined check inside a check block::
 
       checks T {
           a /= null implies a > 5, warning "potato", a
           ^^^^^^^^^^^^^^^^^^^^^^^1 ^2      ^3        ^4
 
-    :attribute n_record: The record type this check applies to
-    :type: Record_Type
+    :attribute n_type: The tuple/record type this check applies to
+    :type: Composite_Type
 
     :attribute n_expr: The boolean expression for the check (see 1)
     :type: Expression
 
     :attribute n_anchor: The (optional) record component where the message \
     should be issued (or None) (see 4)
-    :type: Record_Component
+    :type: Composite_Component
 
     :attribute severity: warning, error, or fatal (see 2; also if this is \
     not specified the default is 'error')
     :type: str
 
     :attribute message: the user-supplied message (see 3)
     :type: str
     """
-    def __init__(self, n_record, n_expr, n_anchor, severity, t_message):
-        assert isinstance(n_record, Record_Type)
+    def __init__(self, n_type, n_expr, n_anchor, severity, t_message):
+        assert isinstance(n_type, Composite_Type)
         assert isinstance(n_expr, Expression)
-        assert isinstance(n_anchor, Record_Component) or n_anchor is None
+        assert isinstance(n_anchor, Composite_Component) or n_anchor is None
         assert severity in ("warning", "error", "fatal")
         assert isinstance(t_message, Token)
         assert t_message.kind == "STRING"
         super().__init__(t_message.location)
 
-        self.n_record = n_record
+        self.n_type   = n_type
         self.n_expr   = n_expr
         self.n_anchor = n_anchor
         self.severity = severity
         self.message  = t_message.value
 
     def dump(self, indent=0):  # pragma: no cover
         if self.severity == "warning":
@@ -202,32 +207,40 @@
             self.write_indent(indent, "Error '%s'" % self.message)
         else:
             self.write_indent(indent, "Fatal error '%s'" % self.message)
         if self.n_anchor:
             self.write_indent(indent + 1, "Anchor: %s" % self.n_anchor.name)
         self.n_expr.dump(indent + 1)
 
-    def get_real_location(self, record_object):
-        assert isinstance(record_object, Record_Object)
-        if self.n_anchor is None:
-            return record_object.location
-        elif record_object.field[self.n_anchor.name] is not None:
-            return record_object.field[self.n_anchor.name].location
+    def get_real_location(self, composite_object):
+        assert isinstance(composite_object, (Record_Object,
+                                             Tuple_Aggregate))
+        if isinstance(composite_object, Record_Object):
+            fields = composite_object.field
+        else:
+            fields = composite_object.value
+
+        if self.n_anchor is None or fields[self.n_anchor.name] is None:
+            return composite_object.location
         else:
-            return record_object.location
+            return fields[self.n_anchor.name].location
 
-    def perform(self, mh, record_object):
+    def perform(self, mh, composite_object):
         assert isinstance(mh, Message_Handler)
-        assert isinstance(record_object, Record_Object)
+        assert isinstance(composite_object, (Record_Object,
+                                             Tuple_Aggregate))
 
-        result = self.n_expr.evaluate(mh, copy(record_object.field))
+        if isinstance(composite_object, Record_Object):
+            result = self.n_expr.evaluate(mh, copy(composite_object.field))
+        else:
+            result = self.n_expr.evaluate(mh, copy(composite_object.value))
         assert isinstance(result.value, bool)
 
         if not result.value:
-            loc = self.get_real_location(record_object)
+            loc = self.get_real_location(composite_object)
             if self.severity == "warning":
                 mh.warning(loc,
                            self.message,
                            user = True)
             else:
                 mh.error(loc,
                          self.message,
@@ -247,14 +260,17 @@
     PLUS           = auto()
     LOGICAL_NOT    = auto()
     ABSOLUTE_VALUE = auto()
 
     STRING_LENGTH  = auto()
     ARRAY_LENGTH   = auto()
 
+    CONVERSION_TO_INT     = auto()
+    CONVERSION_TO_DECIMAL = auto()
+
 
 class Binary_Operator(Enum):
     LOGICAL_AND     = auto()    # Short-circuit
     LOGICAL_OR      = auto()    # Short-circuit
     LOGICAL_XOR     = auto()
     LOGICAL_IMPLIES = auto()    # Short-circuit
 
@@ -301,45 +317,51 @@
         evaluated in a static context. Otherwise it must be a
         dictionary that maps names (such as record fields or
         quantified variables) to expressions.
 
         :param mh: the message handler to use
         :type mh: Message_Handler
         :param context: name mapping or None (for a static context)
-        :type context: dict[str] Expression
+        :type context: dict[str, Expression]
         :raise TRLC_Error: if the expression cannot be evaluated
         :return: result of the evaluation
         :rtype: Value
         """
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
         assert False, "evaluate not implemented for %s" % \
             self.__class__.__name__
 
     def to_string(self):  # pragma: no cover
         assert False, "to_string not implemented for %s" % \
             self.__class__.__name__
 
     def ensure_type(self, mh, typ):
-        assert isinstance(typ, type)
-        if not isinstance(self.typ, typ):
+        assert isinstance(typ, (type, Type))
+        if isinstance(typ, type) and not isinstance(self.typ, typ):
             mh.error(self.location,
                      "expected expression of type %s, got %s instead" %
                      (typ.__name__,
                       self.typ.__class__.__name__))
+        elif isinstance(typ, Type) and self.typ != typ:
+            mh.error(self.location,
+                     "expected expression of type %s, got %s instead" %
+                     (typ.name,
+                      self.typ.name))
 
     def resolve_references(self, mh):
         assert isinstance(mh, Message_Handler)
 
 
 class Implicit_Null(Expression):
     """Synthesised null values
 
-    When a record object is declared and an optional component is not
-    specified, we synthesise an implicit null expression for this.
+    When a record object or tuple aggregate is declared and an
+    optional component or field is not specified, we synthesise an
+    implicit null expression for this.
 
     For example given this TRLC type::
 
       type T {
          x optional Integer
       }
 
@@ -352,30 +374,34 @@
       {x: Implicit_Null}
 
     Each field will get its own implicit null. Further note that this
     implicit null is distinct from the explicit :class:`Null_Literal`
     that can appear in check expressions.
 
     """
-    def __init__(self, record_object, record_component):
-        assert isinstance(record_object, Record_Object)
-        assert isinstance(record_component, Record_Component)
-        super().__init__(record_object.location, None)
+    def __init__(self, composite_object, composite_component):
+        assert isinstance(composite_object, (Record_Object,
+                                             Tuple_Aggregate))
+        assert isinstance(composite_component, Composite_Component)
+        super().__init__(composite_object.location, None)
 
     def to_string(self):
         return "null"
 
     def evaluate(self, mh, context):
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
         return Value(self.location, None, None)
 
     def to_python_object(self):
         return None
 
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Implicit_Null")
+
 
 class Literal(Expression):
     """Abstract base for all Literals
 
     Does not offer any additional features, but it's a nice way to
     group together all literal types. This is useful if you want to
     check if you are dealing with a literal::
@@ -458,50 +484,106 @@
         assert context is None or isinstance(context, dict)
         return Value(self.location, self.value, self.typ)
 
     def to_python_object(self):
         return self.value
 
 
+class Decimal_Literal(Literal):
+    """Decimal literals
+
+    Note that these are always positive. A negative decimal is
+    actually a unary negation expression, operating on a positive
+    decimal literal::
+
+      x == -5.0
+
+    This would create the following tree::
+
+       OP_EQUALITY
+          NAME_REFERENCE x
+          UNARY_EXPRESSION -
+             DECIMAL_LITERAL 5.0
+
+    :attribute value: the non-negative decimal value
+    :type: fractions.Fraction
+    """
+    def __init__(self, token, typ):
+        assert isinstance(token, Token)
+        assert token.kind == "DECIMAL"
+        assert isinstance(typ, Builtin_Decimal)
+        super().__init__(token.location, typ)
+
+        self.value = token.value
+
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Decimal Literal %u" % self.value)
+
+    def to_string(self):
+        return str(self.value)
+
+    def evaluate(self, mh, context):
+        assert isinstance(mh, Message_Handler)
+        assert context is None or isinstance(context, dict)
+        return Value(self.location, self.value, self.typ)
+
+    def to_python_object(self):
+        return self.value
+
+
 class String_Literal(Literal):
     """String literals
 
     Note the value of the string does not include the quotation marks,
     and any escape sequences are fully resolved. For example::
 
        "foo\\"bar"
 
     Will have a value of ``foo"bar``.
 
     :attribute value: string content
     :type: str
 
+    :attribute references: resolved references of a markup string
+    :type: list[Record_Reference]
+
     """
     def __init__(self, token, typ):
         assert isinstance(token, Token)
         assert token.kind == "STRING"
         assert isinstance(typ, Builtin_String)
         super().__init__(token.location, typ)
 
-        self.value = token.value
+        self.value          = token.value
+        self.has_references = isinstance(typ, Builtin_Markup_String)
+        self.references     = []
 
     def dump(self, indent=0):  # pragma: no cover
-        self.write_indent(indent, "String Literal %s" % self.value)
+        self.write_indent(indent, "String Literal %s" % repr(self.value))
+        if self.has_references:
+            self.write_indent(indent + 1, "Markup References")
+            for ref in self.references:
+                ref.dump(indent + 2)
 
     def to_string(self):
         return self.value
 
     def evaluate(self, mh, context):
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
         return Value(self.location, self.value, self.typ)
 
     def to_python_object(self):
         return self.value
 
+    def resolve_references(self, mh):
+        assert isinstance(mh, Message_Handler)
+        for ref in self.references:
+            ref.resolve_references(mh)
+
 
 class Boolean_Literal(Literal):
     """Boolean values
 
     :attribute value: the boolean value
     :type: bool
     """
@@ -539,23 +621,23 @@
        foo != my_enum.POTATO
               ^^^^^^^^^^^^^^
 
     To get to the string value of the enumeration literal
     (i.e. ``POTATO`` here) you can get the name of the literal spec
     itself: ``enum_lit.value.name``; and to get the name of the
     enumeration (i.e. ``my_enum`` here) you can use
-    ``enum_lit.value.enum.name``.
+    ``enum_lit.value.n_typ.name``.
 
     :attribute value: enumeration value
     :type: Enumeration_Literal_Spec
 
     """
     def __init__(self, location, literal):
         assert isinstance(literal, Enumeration_Literal_Spec)
-        super().__init__(location, literal.enum)
+        super().__init__(location, literal.n_typ)
 
         self.value = literal
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent,
                           "Enumeration Literal %s.%s" % (self.typ.name,
                                                          self.value.name))
@@ -593,15 +675,17 @@
     """
     def __init__(self, location, typ):
         super().__init__(location, typ)
         self.value = []
 
     def append(self, value):
         assert isinstance(value, (Literal,
+                                  Unary_Expression,
                                   Array_Aggregate,
+                                  Tuple_Aggregate,
                                   Record_Reference))
         self.value.append(value)
 
     def to_string(self):
         return "[" + ", ".join(x.to_string() for x in self.value) + "]"
 
     def evaluate(self, mh, context):
@@ -618,14 +702,99 @@
         for val in self.value:
             val.resolve_references(mh)
 
     def to_python_object(self):
         return [x.to_python_object() for x in self.value]
 
 
+class Tuple_Aggregate(Expression):
+    """Instances of a tuple
+
+    This is created when assigning to a tuple components. There are
+    two forms, the ordinary form::
+
+       coordinate = (12.3, 40.0)
+                    ^^^^^^^^^^^^
+
+    And the separator form::
+
+       item = 12345@42
+              ^^^^^^^^
+
+    In terms of AST there is no difference, as the separator is only
+    syntactic sugar.
+
+    :attribute value: contents of the tuple
+    :type: dict[str, Expression]
+
+    """
+    def __init__(self, location, typ):
+        super().__init__(location, typ)
+        self.value = {n_field.name : Implicit_Null(self, n_field)
+                      for n_field in self.typ.components.values()}
+
+    def assign(self, field, value):
+        assert isinstance(field, str)
+        assert isinstance(value, (Literal,
+                                  Unary_Expression,
+                                  Tuple_Aggregate,
+                                  Record_Reference)), \
+                "value is %s" % value.__class__.__name__
+        assert field in self.typ.components
+
+        self.value[field] = value
+
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Tuple_Aggregate")
+        self.write_indent(indent + 1, "Type: %s" % self.typ.name)
+        for n_item in self.typ.iter_sequence():
+            if isinstance(n_item, Composite_Component):
+                self.value[n_item.name].dump(indent + 1)
+
+    def to_string(self):
+        first = True
+        if self.typ.has_separators():
+            rv = ""
+        else:
+            rv = "("
+        for n_item in self.typ.iter_sequence():
+            if isinstance(n_item, Separator):
+                rv += " %s " % n_item.token.value
+            elif first:
+                first = False
+            else:
+                rv += ", "
+
+            if isinstance(n_item, Composite_Component):
+                rv += self.value[n_item.name].to_string()
+        if self.typ.has_separators():
+            rv = ""
+        else:
+            rv = ")"
+        return rv
+
+    def evaluate(self, mh, context):
+        assert isinstance(mh, Message_Handler)
+        assert context is None or isinstance(context, dict)
+        return Value(self.location,
+                     {name : element.evaluate(mh, context)
+                      for name, element in self.value.items()},
+                     self.typ)
+
+    def resolve_references(self, mh):
+        assert isinstance(mh, Message_Handler)
+
+        for val in self.value.values():
+            val.resolve_references(mh)
+
+    def to_python_object(self):
+        return {name: value.to_python_object()
+                for name, value in self.value.items()}
+
+
 class Record_Reference(Expression):
     """Reference to another record object
 
     This can appear in record object declarations::
 
       Requirement Kitten {
           depends_on = Other_Package.Cat
@@ -649,28 +818,29 @@
     :attribute target: The concrete record object referred to by (2)
     :type: Record_Object
 
     :attribute package: The package (see 1) supposed to contain (2)
     :type: Package
 
     """
-    def __init__(self, referencing_token, typ, package):
-        assert isinstance(referencing_token, Token)
-        assert referencing_token.kind == "IDENTIFIER"
-        assert isinstance(typ, Record_Type)
+    def __init__(self, location, name, typ, package):
+        assert isinstance(location, Location)
+        assert isinstance(name, str)
+        assert isinstance(typ, Record_Type) or typ is None
         assert isinstance(package, Package)
-        super().__init__(referencing_token.location, typ)
+        super().__init__(location, typ)
 
-        self.name    = referencing_token.value
+        self.name    = name
         self.target  = None
         self.package = package
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Record Reference %s" % self.name)
-        self.write_indent(indent + 1, "Resolved: %s" % self.target is not None)
+        self.write_indent(indent + 1,
+                          "Resolved: %s" % (self.target is not None))
 
     def to_string(self):
         return self.name
 
     def evaluate(self, mh, context):
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
@@ -680,42 +850,49 @@
         assert isinstance(mh, Message_Handler)
 
         self.target = self.package.symbols.lookup_direct(
             mh                = mh,
             name              = self.name,
             error_location    = self.location,
             required_subclass = Record_Object)
+        if self.typ is None:
+            self.typ = self.target.n_typ
+        elif not self.target.n_typ.is_subclass_of(self.typ):
+            mh.ice_loc(self.location,
+                       "on resolving references, types do not match; "
+                       "expected %s, got %s" % (self.typ.name,
+                                                self.target.n_typ.name))
 
     def to_python_object(self):
         return self.name
 
 
 class Name_Reference(Expression):
     """Reference to a name
 
-    Name reference to either a :class:`Record_Component` or a
+    Name reference to either a :class:`Composite_Component` or a
     :class:`Quantified_Variable`. The actual value of course depends
     on the context. See :py:meth:`Expression.evaluate()`.
 
     For example::
 
       (forall x in potato => x > 1)
                    ^1        ^2
 
     Both indicated parts are a :class:`Name_Reference`, the first one
-    refers to a :class:`Record_Component`, and the second refers to a
+    refers to a :class:`Composite_Component`, and the second refers to a
     :class:`Quantified_Variable`.
 
     :attribute entity: the entity named here
-    :type: Record_Component, Quantified_Variable
+    :type: Composite_Component, Quantified_Variable
     """
     def __init__(self, location, entity):
-        assert isinstance(entity, (Record_Component,
+        assert isinstance(entity, (Composite_Component,
                                    Quantified_Variable))
-        super().__init__(location, entity.typ)
+        super().__init__(location, entity.n_typ)
         self.entity = entity
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Name Reference to %s" % self.entity.name)
 
     def to_string(self):
         return self.entity.name
@@ -739,14 +916,16 @@
 
     * Unary_Operator.PLUS (e.g. ``+5``)
     * Unary_Operator.MINUS (e.g. ``-5``)
     * Unary_Operator.ABSOLUTE_VALUE (e.g. ``abs 42``)
     * Unary_Operator.LOGICAL_NOT (e.g. ``not True``)
     * Unary_Operator.STRING_LENGTH (e.g. ``len("foobar")``)
     * Unary_Operator.ARRAY_LENGTH (e.g. ``len(component_name)``)
+    * Unary_Operator.CONVERSION_TO_INT (e.g. ``Integer(5.3)``)
+    * Unary_Operator.CONVERSION_TO_DECIMAL (e.g. ``Decimal(5)``)
 
     Note that several builtin functions are mapped to unary operators.
 
     :attribute operator: the operation
     :type: Unary_Operator
 
     :attribute n_operand: the expression we operate on
@@ -760,21 +939,25 @@
         assert isinstance(n_operand, Expression)
         self.operator  = operator
         self.n_operand = n_operand
 
         if operator in (Unary_Operator.MINUS,
                         Unary_Operator.PLUS,
                         Unary_Operator.ABSOLUTE_VALUE):
-            self.n_operand.ensure_type(mh, Builtin_Integer)
+            self.n_operand.ensure_type(mh, Builtin_Numeric_Type)
         elif operator == Unary_Operator.LOGICAL_NOT:
             self.n_operand.ensure_type(mh, Builtin_Boolean)
         elif operator == Unary_Operator.STRING_LENGTH:
             self.n_operand.ensure_type(mh, Builtin_String)
         elif operator == Unary_Operator.ARRAY_LENGTH:
             self.n_operand.ensure_type(mh, Array_Type)
+        elif operator == Unary_Operator.CONVERSION_TO_INT:
+            self.n_operand.ensure_type(mh, Builtin_Numeric_Type)
+        elif operator == Unary_Operator.CONVERSION_TO_DECIMAL:
+            self.n_operand.ensure_type(mh, Builtin_Numeric_Type)
         else:
             mh.ice_loc(self.location,
                        "unexpected unary operation %s" % operator)
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Unary %s Expression" % self.operator)
         self.write_indent(indent + 1, "Type: %s" % self.typ.name)
@@ -785,15 +968,15 @@
         assert context is None or isinstance(context, dict)
 
         v_operand = self.n_operand.evaluate(mh, context)
         if v_operand.value is None:
             mh.error(v_operand.location,
                      "input to unary expression %s (%s) must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         if self.operator == Unary_Operator.MINUS:
             return Value(location = self.location,
                          value    = -v_operand.value,
                          typ      = self.typ)
         elif self.operator == Unary_Operator.PLUS:
             return Value(location = self.location,
@@ -808,14 +991,28 @@
                          value    = abs(v_operand.value),
                          typ      = self.typ)
         elif self.operator in (Unary_Operator.STRING_LENGTH,
                                Unary_Operator.ARRAY_LENGTH):
             return Value(location = self.location,
                          value    = len(v_operand.value),
                          typ      = self.typ)
+        elif self.operator == Unary_Operator.CONVERSION_TO_INT:
+            if isinstance(v_operand.value, Fraction):
+                return Value(
+                    location = self.location,
+                    value    = math.round_nearest_away(v_operand.value),
+                    typ      = self.typ)
+            else:
+                return Value(location = self.location,
+                             value    = v_operand.value,
+                             typ      = self.typ)
+        elif self.operator == Unary_Operator.CONVERSION_TO_DECIMAL:
+            return Value(location = self.location,
+                         value    = Fraction(v_operand.value),
+                         typ      = self.typ)
         else:
             mh.ice_loc(self.location,
                        "unexpected unary operation %s" % self.operator)
 
     def to_python_object(self):
         assert self.operator in (Unary_Operator.MINUS,
                                  Unary_Operator.PLUS)
@@ -852,16 +1049,16 @@
     * Binary_Operator.DIVIDE (e.g. ``x / 2``)
     * Binary_Operator.REMAINDER (e.g. ``x % 2``)
     * Binary_Operator.POWER (e.g. ``x ** 2``)
     * Binary_Operator.INDEX (e.g. ``foo[2]``)
 
     Note that several builtin functions are mapped to unary operators.
 
-    Note also that the plus operation is supported for both integers
-    and strings.
+    Note also that the plus operation is supported for integers,
+    rationals and strings.
 
     :attribute operator: the operation
     :type: Binary_Operator
 
     :attribute n_lhs: the first operand
     :type: Expression
 
@@ -899,40 +1096,46 @@
                          (self.n_lhs.typ.name,
                           self.n_rhs.typ.name))
 
         elif operator in (Binary_Operator.COMP_LT,
                           Binary_Operator.COMP_LEQ,
                           Binary_Operator.COMP_GT,
                           Binary_Operator.COMP_GEQ):
-            self.n_lhs.ensure_type(mh, Builtin_Integer)
-            self.n_rhs.ensure_type(mh, Builtin_Integer)
+            self.n_lhs.ensure_type(mh, Builtin_Numeric_Type)
+            self.n_rhs.ensure_type(mh, self.n_lhs.typ)
 
         elif operator in (Binary_Operator.STRING_CONTAINS,
                           Binary_Operator.STRING_STARTSWITH,
                           Binary_Operator.STRING_ENDSWITH,
                           Binary_Operator.STRING_REGEX):
             self.n_lhs.ensure_type(mh, Builtin_String)
             self.n_rhs.ensure_type(mh, Builtin_String)
 
         elif operator == Binary_Operator.ARRAY_CONTAINS:
             self.n_rhs.ensure_type(mh, Array_Type)
             self.n_lhs.ensure_type(mh, self.n_rhs.typ.element_type.__class__)
 
         elif operator == Binary_Operator.PLUS:
-            if isinstance(self.n_lhs.typ, Builtin_Integer):
-                self.n_rhs.ensure_type(mh, Builtin_Integer)
+            if isinstance(self.n_lhs.typ, Builtin_Numeric_Type):
+                self.n_rhs.ensure_type(mh, self.n_lhs.typ)
             else:
                 self.n_lhs.ensure_type(mh, Builtin_String)
                 self.n_rhs.ensure_type(mh, Builtin_String)
 
         elif operator in (Binary_Operator.MINUS,
                           Binary_Operator.TIMES,
-                          Binary_Operator.DIVIDE,
-                          Binary_Operator.REMAINDER,
-                          Binary_Operator.POWER):
+                          Binary_Operator.DIVIDE):
+            self.n_lhs.ensure_type(mh, Builtin_Numeric_Type)
+            self.n_rhs.ensure_type(mh, self.n_lhs.typ)
+
+        elif operator == Binary_Operator.POWER:
+            self.n_lhs.ensure_type(mh, Builtin_Numeric_Type)
+            self.n_rhs.ensure_type(mh, Builtin_Integer)
+
+        elif operator == Binary_Operator.REMAINDER:
             self.n_lhs.ensure_type(mh, Builtin_Integer)
             self.n_rhs.ensure_type(mh, Builtin_Integer)
 
         elif operator == Binary_Operator.INDEX:
             self.n_lhs.ensure_type(mh, Array_Type)
             self.n_rhs.ensure_type(mh, Builtin_Integer)
 
@@ -997,15 +1200,15 @@
         v_lhs = self.n_lhs.evaluate(mh, context)
         if v_lhs.value is None and \
            self.operator not in (Binary_Operator.COMP_EQ,
                                  Binary_Operator.COMP_NEQ):
             mh.error(v_lhs.location,
                      "lhs of check %s (%s) must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         # Check for the short-circuit operators first
         if self.operator == Binary_Operator.LOGICAL_AND:
             assert isinstance(v_lhs.value, bool)
             if v_lhs.value:
                 return self.n_rhs.evaluate(mh, context)
             else:
@@ -1031,15 +1234,15 @@
         v_rhs = self.n_rhs.evaluate(mh, context)
         if v_rhs.value is None and \
            self.operator not in (Binary_Operator.COMP_EQ,
                                  Binary_Operator.COMP_NEQ):
             mh.error(v_rhs.location,
                      "rhs of check %s (%s) must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         if self.operator == Binary_Operator.LOGICAL_XOR:
             assert isinstance(v_lhs.value, bool)
             assert isinstance(v_rhs.value, bool)
             return Value(location = self.location,
                          value    = v_lhs.value ^ v_rhs.value,
                          typ      = self.typ)
@@ -1101,100 +1304,144 @@
             assert isinstance(v_rhs.value, list)
 
             return Value(location = self.location,
                          value    = v_lhs in v_rhs.value,
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.PLUS:
-            assert isinstance(v_lhs.value, (int, str))
-            assert isinstance(v_rhs.value, (int, str))
+            assert isinstance(v_lhs.value, (int, str, Fraction))
+            assert isinstance(v_rhs.value, (int, str, Fraction))
             return Value(location = self.location,
                          value    = v_lhs.value + v_rhs.value,
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.MINUS:
-            assert isinstance(v_lhs.value, int)
-            assert isinstance(v_rhs.value, int)
+            assert isinstance(v_lhs.value, (int, Fraction))
+            assert isinstance(v_rhs.value, (int, Fraction))
             return Value(location = self.location,
                          value    = v_lhs.value - v_rhs.value,
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.TIMES:
-            assert isinstance(v_lhs.value, int)
-            assert isinstance(v_rhs.value, int)
+            assert isinstance(v_lhs.value, (int, Fraction))
+            assert isinstance(v_rhs.value, (int, Fraction))
             return Value(location = self.location,
                          value    = v_lhs.value * v_rhs.value,
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.DIVIDE:
-            assert isinstance(v_lhs.value, int)
-            assert isinstance(v_rhs.value, int)
+            assert isinstance(v_lhs.value, (int, Fraction))
+            assert isinstance(v_rhs.value, (int, Fraction))
 
             if v_rhs.value == 0:
                 mh.error(v_rhs.location,
                          "division by zero in %s (%s)" %
                          (self.to_string(),
-                          self.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
 
-            return Value(location = self.location,
-                         value    = v_lhs.value // v_rhs.value,
-                         typ      = self.typ)
+            if isinstance(v_lhs.value, int):
+                return Value(location = self.location,
+                             value    = v_lhs.value // v_rhs.value,
+                             typ      = self.typ)
+            else:
+                return Value(location = self.location,
+                             value    = v_lhs.value / v_rhs.value,
+                             typ      = self.typ)
 
         elif self.operator == Binary_Operator.REMAINDER:
             assert isinstance(v_lhs.value, int)
             assert isinstance(v_rhs.value, int)
 
             if v_rhs.value == 0:
                 mh.error(v_rhs.location,
                          "division by zero in %s (%s)" %
                          (self.to_string(),
-                          self.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
 
             return Value(location = self.location,
                          value    = math.remainder(v_lhs.value, v_rhs.value),
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.POWER:
-            assert isinstance(v_lhs.value, int)
+            assert isinstance(v_lhs.value, (int, Fraction))
             assert isinstance(v_rhs.value, int)
             return Value(location = self.location,
                          value    = v_lhs.value ** v_rhs.value,
                          typ      = self.typ)
 
         elif self.operator == Binary_Operator.INDEX:
             assert isinstance(v_lhs.value, list)
             assert isinstance(v_rhs.value, int)
 
             if v_rhs.value < 0:
                 mh.error(v_rhs.location,
                          "index cannot be less than zero in %s (%s)" %
                          (self.to_string(),
-                          self.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
             elif v_lhs.typ.upper_bound is not None and \
                  v_rhs.value > v_lhs.typ.upper_bound:
                 mh.error(v_rhs.location,
                          "index cannot be more than %u in %s (%s)" %
                          (v_lhs.typ.upper_bound,
                           self.to_string(),
-                          self.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
             elif v_rhs.value > len(v_lhs.value):
                 mh.error(v_lhs.location,
                          "array is not big enough in %s (%s)" %
                          (self.to_string(),
-                          self.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
 
             return Value(location = self.location,
                          value    = v_lhs.value[v_rhs.value].value,
                          typ      = self.typ)
 
         else:
             mh.ice_loc(self.location,
                        "unexpected binary operator %s" % self.operator)
 
 
+class Field_Access_Expression(Expression):
+    """Tuple field access
+
+    For example in::
+
+      foo.bar
+      ^1  ^2
+
+    :attribute n_prefix: expression with tuple type (see 1)
+    :type: Expression
+
+    :attribute n_field: a tuple field to dereference (see 2)
+    :type: Composite_Component
+
+    """
+    def __init__(self, mh, location, n_prefix, n_field):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(n_prefix, Expression)
+        assert isinstance(n_field, Composite_Component)
+        super().__init__(location, n_field.n_typ)
+        self.n_prefix = n_prefix
+        self.n_field  = n_field
+
+        self.n_prefix.ensure_type(mh, self.n_field.member_of)
+
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Field_Access (%s)" % self.n_field.name)
+        self.n_prefix.dump(indent + 1)
+
+    def to_string(self):
+        return self.n_prefix.to_string() + "." + self.n_field.name
+
+    def evaluate(self, mh, context):
+        assert isinstance(mh, Message_Handler)
+        assert context is None or isinstance(context, dict)
+
+        return self.n_prefix.evaluate(mh, context).value[self.n_field.name]
+
+
 class Range_Test(Expression):
     """Range membership test
 
     For example in::
 
       x in 1   ..   field+1
       ^lhs ^lower   ^^^^^^^upper
@@ -1218,17 +1465,17 @@
         assert isinstance(n_lhs, Expression)
         assert isinstance(n_lower, Expression)
         assert isinstance(n_upper, Expression)
         self.n_lhs   = n_lhs
         self.n_lower = n_lower
         self.n_upper = n_upper
 
-        self.n_lhs.ensure_type(mh, Builtin_Integer)
-        self.n_lower.ensure_type(mh, Builtin_Integer)
-        self.n_upper.ensure_type(mh, Builtin_Integer)
+        self.n_lhs.ensure_type(mh, Builtin_Numeric_Type)
+        self.n_lower.ensure_type(mh, self.n_lhs.typ)
+        self.n_upper.ensure_type(mh, self.n_lhs.typ)
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Range Test")
         self.write_indent(indent + 1, "Type: %s" % self.typ)
         self.n_lhs.dump(indent + 1)
         self.n_lower.dump(indent + 1)
         self.n_upper.dump(indent + 1)
@@ -1238,29 +1485,29 @@
         assert context is None or isinstance(context, dict)
 
         v_lhs = self.n_lhs.evaluate(mh, context)
         if v_lhs.value is None:
             mh.error(v_lhs.location,
                      "lhs of range check %s (%s) see must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         v_lower = self.n_lower.evaluate(mh, context)
         if v_lower.value is None:
             mh.error(v_lower.location,
                      "lower bound of range check %s (%s) must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         v_upper = self.n_upper.evaluate(mh, context)
         if v_upper.value is None:
             mh.error(v_upper.location,
                      "upper bound of range check %s (%s) must not be null" %
                      (self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
 
         return Value(location = self.location,
                      value    = v_lower.value <= v_lhs.value <= v_upper.value,
                      typ      = self.typ)
 
 
 class Action(Node):
@@ -1389,15 +1636,15 @@
 
         for action in self.actions:
             v_cond = action.n_cond.evaluate(mh, context)
             if v_cond.value is None:
                 mh.error(v_cond.location,
                          "condition of %s (%s) must not be null" %
                          (action.to_string(),
-                          action.location.to_string(False)))
+                          mh.cross_file_reference(self.location)))
             if v_cond.value:
                 return action.n_expr.evaluate(mh, context)
 
         return self.else_expr.evaluate(mh, context)
 
 
 class Quantified_Expression(Expression):
@@ -1468,23 +1715,23 @@
             new_ctx = {}
         else:
             new_ctx = copy(context)
 
         # This is going to be a bit tricky. We essentially eliminate
         # the quantifier and substitute; for the sake of making better
         # error messages.
-        assert isinstance(self.n_source.entity, Record_Component)
+        assert isinstance(self.n_source.entity, Composite_Component)
         array_values = context[self.n_source.entity.name]
         if isinstance(array_values, Implicit_Null):
             mh.error(array_values.location,
                      "%s in quantified expression %s (%s) "
                      "must not be null" %
                      (self.n_source.to_string(),
                       self.to_string(),
-                      self.location.to_string(False)))
+                      mh.cross_file_reference(self.location)))
         else:
             assert isinstance(array_values, Array_Aggregate)
 
         rv  = self.universal
         loc = self.location
         for binding in array_values.value:
             new_ctx[self.n_var.name] = binding
@@ -1521,15 +1768,32 @@
     """
     def __init__(self, name, location):
         super().__init__(location)
         assert isinstance(name, str)
         self.name = name
 
 
-class Quantified_Variable(Entity):
+class Typed_Entity(Entity):
+    """Base class for entities with a type.
+
+    A typed entity is a concrete object (with a name and TRLC type)
+    for which we need to allocate memory. Examples of typed entities
+    are record objects and components.
+
+    :attribute n_typ: type of the entity
+    :type: Type
+
+    """
+    def __init__(self, name, location, n_typ):
+        super().__init__(name, location)
+        assert isinstance(n_typ, Type)
+        self.n_typ = n_typ
+
+
+class Quantified_Variable(Typed_Entity):
     """Variable used in quantified expression.
 
     A quantified expression declares and binds a variable, for which
     we need a named entity. For example in::
 
       (forall x in array => x > 1)
               ^
@@ -1537,28 +1801,54 @@
     We represent this first x as a :class:`Quantified_Variable`, the
     second x will be an ordinary :class:`Name_Reference`.
 
     :attribute typ: type of the variable (i.e. element type of the array)
     :type: Type
 
     """
-    def __init__(self, name, location, typ):
-        super().__init__(name, location)
-        assert isinstance(typ, Type)
-        self.typ = typ
-
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Quantified Variable %s" % self.name)
-        self.typ.dump(indent + 1)
+        self.n_typ.dump(indent + 1)
 
 
 class Type(Entity):
     """Abstract base class for all types.
 
     """
+    def perform_type_checks(self, mh, value):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(value, Expression)
+        return True
+
+
+class Concrete_Type(Type):
+    """Abstract base class for all non-anonymous types.
+
+    :attribute n_package: package where this type was declared
+    :type: Package
+    """
+    def __init__(self, name, location, n_package):
+        super().__init__(name, location)
+        assert isinstance(n_package, Package)
+        self.n_package = n_package
+
+    def fully_qualified_name(self):
+        """Return the FQN for this type (i.e. PACKAGE.NAME)
+
+        :returns: the type's full name
+        :rtype: str
+        """
+        return self.n_package.name + "." + self.name
+
+    def __hash__(self):
+        return hash((self.n_package.name, self.name))
+
+    def __repr__(self):
+        return "%s<%s>" % (self.__class__.__name__,
+                           self.fully_qualified_name())
 
 
 class Builtin_Type(Type):
     """Abstract base class for all builtin types.
 
     """
     LOCATION = Location(file_name = "<builtin>")
@@ -1566,14 +1856,22 @@
     def __init__(self, name):
         super().__init__(name, Builtin_Type.LOCATION)
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, self.__class__.__name__)
 
 
+class Builtin_Numeric_Type(Builtin_Type):
+    """Abstract base class for all builtin numeric types.
+
+    """
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, self.__class__.__name__)
+
+
 class Builtin_Function(Entity):
     """Builtin functions.
 
     These are auto-generated by the :class:`~trlc.trlc.Source_Manager`.
 
     :attribute arity: number of parameters
     :type: int
@@ -1611,21 +1909,23 @@
     :type: int
 
     :attribute element_type: type of the array elements
     :type: Type
 
     """
     def __init__(self, location, element_type, lower_bound, upper_bound):
-        assert isinstance(element_type, Type)
+        assert isinstance(element_type, Type) or element_type is None
         assert isinstance(lower_bound, int)
         assert lower_bound >= 0
         assert upper_bound is None or isinstance(upper_bound, int)
         assert upper_bound is None or upper_bound >= 0
 
-        if upper_bound is None:
+        if element_type is None:
+            name = "universal array"
+        elif upper_bound is None:
             if lower_bound == 0:
                 name = "array of %s" % element_type.name
             else:
                 name = "array of at least %u %s" % (lower_bound,
                                                     element_type.name)
         elif lower_bound == upper_bound:
             name = "array of %u %s" % (lower_bound,
@@ -1635,91 +1935,211 @@
                                              upper_bound,
                                              element_type.name)
         super().__init__(name, location)
         self.lower_bound  = lower_bound
         self.upper_bound  = upper_bound
         self.element_type = element_type
 
+    def perform_type_checks(self, mh, value):
+        assert isinstance(mh, Message_Handler)
+        if isinstance(value, Array_Aggregate):
+            return all(self.element_type.perform_type_checks(mh, v)
+                       for v in value.value)
+        else:
+            assert isinstance(value, Implicit_Null)
+            return True
+
 
-class Builtin_Integer(Builtin_Type):
+class Builtin_Integer(Builtin_Numeric_Type):
     """Builtin integer type."""
     def __init__(self):
         super().__init__("Integer")
 
 
+class Builtin_Decimal(Builtin_Numeric_Type):
+    """Builtin decimal type."""
+    def __init__(self):
+        super().__init__("Decimal")
+
+
 class Builtin_Boolean(Builtin_Type):
     """Builtin boolean type."""
     def __init__(self):
         super().__init__("Boolean")
 
 
 class Builtin_String(Builtin_Type):
     """Builtin string type."""
     def __init__(self):
         super().__init__("String")
 
 
+class Builtin_Markup_String(Builtin_String):
+    """Builtin string type that allows checked references to TRLC
+       objects.
+    """
+    def __init__(self):
+        super().__init__()
+        self.name = "Markup_String"
+
+
 class Package(Entity):
     """Packages.
 
     A package is declared when it is first encountered (in either a
     rsl or trlc file). A package contains all symbols declared in it,
     both types and record objects. A package is not associated with
     just a single file, it can be spread over multiple files.
 
     :attribute symbols: symbol table of the package
     :type: Symbol_Table
 
-
     """
     def __init__(self, name, location, builtin_stab):
         super().__init__(name, location)
         assert isinstance(builtin_stab, Symbol_Table)
         self.symbols = Symbol_Table()
         self.symbols.make_visible(builtin_stab)
         self.declared_late = False
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Package %s" % self.name)
         self.symbols.dump(indent + 1)
 
 
-class Record_Type(Type):
+class Composite_Type(Concrete_Type):
+    """Abstract base for record and tuple types, as they share some
+       functionality.
+
+    :attribute components: type components (including inherited if applicable)
+    :type: Symbol_Table[Composite_Component]
+
+    :attribute description: user-supplied description of the type or None
+    :type: str
+
+    :attribute checks: used-defined checks for this type (excluding \
+      inherited checks)
+    :type: list[Check]
+
+    """
+    def __init__(self,
+                 name,
+                 description,
+                 location,
+                 package,
+                 inherited_symbols=None):
+        super().__init__(name, location, package)
+        assert isinstance(description, str) or description is None
+        assert isinstance(inherited_symbols, Symbol_Table) or \
+            inherited_symbols is None
+
+        self.components  = Symbol_Table(inherited_symbols)
+        self.description = description
+        self.checks      = []
+
+    def add_check(self, n_check):
+        assert isinstance(n_check, Check)
+        self.checks.append(n_check)
+
+    def iter_checks(self):
+        yield from self.checks
+
+
+class Composite_Component(Typed_Entity):
+    """Component in a record or tuple.
+
+    When declaring a composite type, for each component an entity is
+    declared::
+
+      type|tuple T {
+         foo "blah" optional Boolean
+         ^1  ^2     ^3       ^4
+
+    :attribute description: optional text (see 2) for this component, or None
+    :type: str
+
+    :attribute member_of: a link back to the containing record or tuple; \
+    for inherited fields this refers back to the original base record type
+    :type: Composite_Type
+
+    :attribute optional: indicates if the component can be null or not (see 3)
+    :type: bool
+
+    """
+
+    def __init__(self,
+                 name,
+                 description,
+                 location,
+                 member_of,
+                 n_typ,
+                 optional):
+        super().__init__(name, location, n_typ)
+        assert isinstance(description, str) or description is None
+        assert isinstance(member_of, Composite_Type)
+        assert isinstance(optional, bool)
+        self.description = description
+        self.member_of   = member_of
+        self.optional    = optional
+
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Composite_Component %s" % self.name)
+        if self.description:
+            self.write_indent(indent + 1, "Description: %s" % self.description)
+        self.write_indent(indent + 1, "Optional: %s" % self.optional)
+        self.write_indent(indent + 1, "Type: %s" % self.n_typ.name)
+
+
+class Record_Type(Composite_Type):
     """A user-defined record type.
 
     In this example::
 
       type T  "optional description of T" extends Root_T {
-           ^1 ^2                         ^3
+           ^1 ^2                                  ^3
+
+    Note that (1) is part of the :class:`Entity` base, and (2) is part
+    of the :class:`Composite_Type` base.
 
     :attribute parent: root type or None, indicated by (3) above
     :type: Record_Type
 
-    :attribute components: record components (including inherited)
-    :type: Symbol_Table[Record_Component]
+    :attribute frozen: mapping of frozen components
+    :type: dict[str, Expression]
 
-    :attribute description: user-supplied description of the record or \
-    None, see (2)
-    :type: str
+    :attribute is_final: type is final (i.e. no new components may be declared)
+    :type: bool
 
-    :attribute checks: used-defined checks for this record (excluding \
-    inherited checks)
-    :type: list[Check]
+    :attribute is_abstract: type is abstract
+    :type: bool
 
     """
-    def __init__(self, name, description, location, parent=None):
-        super().__init__(name, location)
-        assert isinstance(description, str) or description is None
-        assert isinstance(parent, Record_Type) or parent is None
-        self.parent      = parent
-        self.components  = Symbol_Table(self.parent.components
-                                        if self.parent
-                                        else None)
-        self.description = description
-        self.checks      = []
+    def __init__(self,
+                 name,
+                 description,
+                 location,
+                 package,
+                 n_parent,
+                 is_abstract):
+        assert isinstance(n_parent, Record_Type) or n_parent is None
+        assert isinstance(is_abstract, bool)
+        super().__init__(name,
+                         description,
+                         location,
+                         package,
+                         n_parent.components if n_parent else None)
+        self.parent      = n_parent
+        self.frozen      = {}
+        self.is_final    = (n_parent.is_final if n_parent else False)
+        self.is_abstract = is_abstract
+
+    def iter_checks(self):
+        if self.parent:
+            yield from self.parent.iter_checks()
+        yield from self.checks
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Record_Type %s" % self.name)
         if self.description:
             self.write_indent(indent + 1, "Description: %s" % self.description)
         if self.parent:
             self.write_indent(indent + 1, "Parent: %s" % self.parent.name)
@@ -1730,196 +2150,270 @@
                 n_check.dump(indent + 2)
         else:
             self.write_indent(indent + 1, "Checks: None")
 
     def all_components(self):
         """Convenience function to get a list of all components.
 
-        :rtype: list[Record_Component]
+        :rtype: list[Composite_Component]
         """
         if self.parent:
             return self.parent.all_components() + \
                 list(self.components.table.values())
         else:
             return list(self.components.table.values())
 
-    def add_check(self, n_check):
-        assert isinstance(n_check, Check)
-        self.checks.append(n_check)
-
-    def iter_checks(self):
-        if self.parent:
-            yield from self.parent.iter_checks()
-        yield from self.checks
-
     def is_subclass_of(self, record_type):
         """ Checks if this record type is or inherits from the given type
 
         :param record_type: check if are or extend this type
         :type record_type: Record_Type
 
         :returns: true if we are or extend the given type
         :rtype: Boolean
-
         """
         assert isinstance(record_type, Record_Type)
 
         ptr = self
         while ptr:
             if ptr is record_type:
                 return True
             else:
                 ptr = ptr.parent
         return False
 
+    def is_frozen(self, n_component):
+        """Test if the given component is frozen.
 
-class Record_Component(Entity):
-    """Component in a record.
+        :param n_component: a composite component of this record type \
+          (or any of its parents)
+        :type n_component: Composite_Component
 
-    When declaring a record type, for each component an entity is
-    declared::
+        :rtype: bool
+        """
+        assert isinstance(n_component, Composite_Component)
+        if n_component.name in self.frozen:
+            return True
+        elif self.parent:
+            return self.parent.is_frozen(n_component)
+        else:
+            return False
 
-      type T {
-         foo "blah" optional Boolean
-         ^1  ^2     ^3       ^4
+    def get_freezing_expression(self, n_component):
+        """Retrieve the frozen value for a frozen component
 
-    :attribute description: optional text (see 2) for this field, or None
-    :type: str
+        It is an internal compiler error to call this method with a
+        component that his not frozen.
 
-    :attribute record: a link back to the containing record; for inherited \
-    fields this refers back to the original base record type
-    :type: Record_Type
+        :param n_component: a frozen component of this record type \
+          (or any of its parents)
+        :type n_component: Composite_Component
 
-    :attribute typ: type of this component (see 4), but note it could also \
-    be an anonymous array type
-    :type: Type
+        :rtype: Expression
 
-    :attribute optional: indicates if the component can be null or not (see 3)
-    :type: bool
+        """
+        assert isinstance(n_component, Composite_Component)
+        if n_component.name in self.frozen:
+            return self.frozen[n_component.name]
+        elif self.parent:
+            return self.parent.get_freezing_expression(n_component)
+        else:
+            assert False
 
-    """
 
-    def __init__(self, name, description, location, record, typ, optional):
-        super().__init__(name, location)
-        assert isinstance(description, str) or description is None
-        assert isinstance(record, Record_Type)
-        assert isinstance(typ, Type)
-        assert isinstance(optional, bool)
-        self.description = description
-        self.record      = record
-        self.typ         = typ
-        self.optional    = optional
+class Tuple_Type(Composite_Type):
+    """A user-defined tuple type.
+
+    In this example::
+
+      tuple T  "optional description of T" {
+            ^1 ^2
+
+    Note that (1) is part of the :class:`Entity` base, and (2) is part
+    of the :class:`Composite_Type` base.
+
+    :attribute separators: list of syntactic separators.
+    :type: list[Separator]
+
+    Note the list of separators will either be empty, or there will be
+    precisely one less separator than components.
+
+    """
+    def __init__(self, name, description, location, package):
+        super().__init__(name,
+                         description,
+                         location,
+                         package)
+        self.separators = []
+
+    def add_separator(self, n_separator):
+        assert isinstance(n_separator, Separator)
+        assert len(self.separators) + 1 == len(self.components.table)
+        self.separators.append(n_separator)
+
+    def iter_separators(self):
+        """Iterate over all separators"""
+        yield from self.separators
+
+    def iter_sequence(self):
+        """Iterate over all components and separators in syntactic order"""
+        if self.separators:
+            for i, n_component in enumerate(self.components.table.values()):
+                yield n_component
+                if i < len(self.separators):
+                    yield self.separators[i]
+        else:
+            yield from self.components.table.values()
+
+    def has_separators(self):
+        """Returns true if a tuple type requires separators"""
+        return bool(self.separators)
 
     def dump(self, indent=0):  # pragma: no cover
-        self.write_indent(indent, "Record_Component %s" % self.name)
+        self.write_indent(indent, "Tuple_Type %s" % self.name)
         if self.description:
             self.write_indent(indent + 1, "Description: %s" % self.description)
-        self.write_indent(indent + 1, "Optional: %s" % self.optional)
-        self.write_indent(indent + 1, "Type: %s" % self.typ.name)
+        self.write_indent(indent + 1, "Fields")
+        for n_item in self.iter_sequence():
+            n_item.dump(indent + 2)
+        if self.checks:
+            self.write_indent(indent + 1, "Checks")
+            for n_check in self.checks:
+                n_check.dump(indent + 2)
+        else:
+            self.write_indent(indent + 1, "Checks: None")
+
+    def perform_type_checks(self, mh, value):
+        assert isinstance(mh, Message_Handler)
+        if isinstance(value, Tuple_Aggregate):
+            ok = True
+            for check in self.iter_checks():
+                if not check.perform(mh, value):
+                    ok = False
+            return ok
+        else:
+            assert isinstance(value, Implicit_Null)
+            return True
+
+
+class Separator(Node):
+    """User-defined syntactic separator
 
+    For example::
+
+      separator x
+                ^1
+
+    :attribute token: token used to separate fields of the tuple
+    :type: Token
+    """
+    def __init__(self, token):
+        super().__init__(token.location)
+        assert isinstance(token, Token) and token.kind in ("IDENTIFIER",
+                                                           "AT")
+        self.token = token
 
-class Enumeration_Type(Type):
+    def dump(self, indent=0):  # pragma: no cover
+        self.write_indent(indent, "Separator %s" % self.token.value)
+
+
+class Enumeration_Type(Concrete_Type):
     """User-defined enumeration types.
 
     For example::
 
       enum T  "potato" {
            ^1 ^2
 
     :attribute description: user supplied optional description, or None
     :type: str
 
     :attribute literals: the literals in this enumeration
     :type: Symbol_Table[Enumeration_Literal_Spec]
 
     """
-    def __init__(self, name, description, location):
-        super().__init__(name, location)
+    def __init__(self, name, description, location, package):
+        super().__init__(name, location, package)
         assert isinstance(description, str) or description is None
         self.literals    = Symbol_Table()
         self.description = description
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Enumeration_Type %s" % self.name)
         if self.description:
             self.write_indent(indent + 1, "Description: %s" % self.description)
         self.literals.dump(indent + 1, omit_heading=True)
 
 
-class Enumeration_Literal_Spec(Entity):
+class Enumeration_Literal_Spec(Typed_Entity):
     """Declared literal in an enumeration declaration.
 
     Note that for literals mentioned later in record object
     declarations, we use :class:`Enumeration_Literal`. Literal specs
     are used here::
 
       enum ASIL {
          QM "not safety related"
          ^1 ^2
 
     :attribute description: the optional user-supplied description, or None
     :type: str
 
-    :attribute enum: a link back to the declaring enumeration
-    :type: Enumeration_Type
-
     """
     def __init__(self, name, description, location, enum):
-        super().__init__(name, location)
+        super().__init__(name, location, enum)
         assert isinstance(description, str) or description is None
         assert isinstance(enum, Enumeration_Type)
         self.description = description
-        self.enum        = enum
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Enumeration_Literal_Spec %s" % self.name)
         if self.description:
             self.write_indent(indent + 1, "Description: %s" % self.description)
 
 
-class Record_Object(Entity):
+class Record_Object(Typed_Entity):
     """A declared instance of a record type.
 
     This is going to be the bulk of all entities created by TRLC::
 
        section "Potato" {
                ^5
          Requirement PotatoReq {
          ^1          ^2
              component1 = 42
              ^3           ^4
 
-    Note that the name of the object is provided by the name attribute
-    of the :class:`Entity` base class.
-
-    :attribute e_typ: the type of the object (see 1)
-    :type: Record_Type
+    Note that the name (see 2) and type (see 1) of the object is
+    provided by the name attribute of the :class:`Typed_Entity` base
+    class.
 
     :attribute field: the specific values for all components (see 3 and 4)
-    :type: dict[str] Expression
+    :type: dict[str, Expression]
 
     :attribute section: None or the section this record is contained in (see 5)
     :type: Section
 
     The actual type of expressions in the field attribute are limited
     to:
 
     * :class:`Literal`
+    * :class:`Unary_Expression`
     * :class:`Array_Aggregate`
+    * :class:`Tuple_Aggregate`
     * :class:`Record_Reference`
     * :class:`Implicit_Null`
 
     """
-    def __init__(self, name, location, e_typ, section):
-        super().__init__(name, location)
-        assert isinstance(e_typ, Record_Type)
+    def __init__(self, name, location, n_typ, section):
+        assert isinstance(n_typ, Record_Type)
         assert isinstance(section, Section) or section is None
-        self.e_typ   = e_typ
+        super().__init__(name, location, n_typ)
         self.field   = {name: None
-                        for name in self.e_typ.components.all_names()}
+                        for name in self.n_typ.components.all_names()}
         self.section = section
 
     def to_python_dict(self):
         """Return an evaluated and simplified object for Python.
 
         For example it might provide::
 
@@ -1931,42 +2425,51 @@
         name of the object itself is not in this returned dictionary.
 
         """
         return {name: value.to_python_object()
                 for name, value in self.field.items()}
 
     def assign(self, component, value):
-        assert isinstance(component, Record_Component)
+        assert isinstance(component, Composite_Component)
         assert isinstance(value, (Literal,
                                   Array_Aggregate,
+                                  Tuple_Aggregate,
                                   Record_Reference,
                                   Implicit_Null,
-                                  Unary_Expression))
+                                  Unary_Expression)), \
+                "value is %s" % value.__class__.__name__
         self.field[component.name] = value
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Record_Object %s" % self.name)
-        self.write_indent(indent + 1, "Type: %s" % self.e_typ.name)
+        self.write_indent(indent + 1, "Type: %s" % self.n_typ.name)
         for key, value in self.field.items():
-            self.write_indent(indent + 1,
-                              "Field %s: %s" % (key,
-                                                repr(value.to_string())))
+            self.write_indent(indent + 1, "Field %s" % key)
+            value.dump(indent + 2)
         if self.section:
             self.section.dump(indent + 1)
 
     def resolve_references(self, mh):
         assert isinstance(mh, Message_Handler)
         for val in self.field.values():
             val.resolve_references(mh)
 
     def perform_checks(self, mh):
         assert isinstance(mh, Message_Handler)
 
         ok = True
-        for check in self.e_typ.iter_checks():
+
+        # First evaluate all tuple checks
+        for n_comp in self.n_typ.all_components():
+            if not n_comp.n_typ.perform_type_checks(mh,
+                                                    self.field[n_comp.name]):
+                ok = False
+
+        # Then evaluate all record checks
+        for check in self.n_typ.iter_checks():
             # Prints messages, if applicable. Raises exception on
             # fatal checks, which causes this to abort.
             if not check.perform(mh, self):
                 ok = False
 
         return ok
 
@@ -2050,19 +2553,22 @@
         assert isinstance(mh, Message_Handler)
         assert isinstance(entity, Entity)
 
         if self.contains(entity.name):
             pdef = self.lookup_direct(mh, entity.name, entity.location)
             mh.error(entity.location,
                      "duplicate definition, previous definition at %s" %
-                     pdef.location.to_string(include_column=False))
+                     mh.cross_file_reference(pdef.location))
 
         else:
             self.table[entity.name] = entity
 
+    def __contains__(self, name):
+        return self.contains(name)
+
     def contains(self, name):
         """ Tests if the given name is in the table
 
         :param name: the name to test
         :type name: str
         :rtype: bool
         """
@@ -2205,15 +2711,15 @@
 
         return self.lookup_direct(
             mh                = mh,
             name              = referencing_token.value,
             error_location    = referencing_token.location,
             required_subclass = required_subclass)
 
-    def write_indent(self, indent, message):
+    def write_indent(self, indent, message):  # pragma: no cover
         assert isinstance(indent, int)
         assert indent >= 0
         assert isinstance(message, str)
         print(" " * (3 * indent) + message)
 
     def dump(self, indent=0, omit_heading=False):  # pragma: no cover
         if omit_heading:
@@ -2227,16 +2733,18 @@
                 ptr.table[name].dump(new_indent)
             ptr = ptr.parent
 
     @classmethod
     def create_global_table(cls, mh):
         stab = Symbol_Table()
         stab.register(mh, Builtin_Integer())
+        stab.register(mh, Builtin_Decimal())
         stab.register(mh, Builtin_Boolean())
         stab.register(mh, Builtin_String())
+        stab.register(mh, Builtin_Markup_String())
         # The legacy versions
         stab.register(mh,
                       Builtin_Function("trlc:len", 1))
         stab.register(mh,
                       Builtin_Function("trlc:startswith", 2))
         stab.register(mh,
                       Builtin_Function("trlc:endswith", 2))
```

### Comparing `trlc-1.0.9/trlc/errors.py` & `trlc-1.1.1/trlc/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         there is one)
         :type include_column: bool
 
         :returns: a formatted location
         :rtype: str
 
         """
-        rv = os.path.basename(self.file_name)
+        rv = os.path.relpath(self.file_name)
         if self.line_no:
             rv += ":%u" % self.line_no
             if self.col_no and include_column:
                 rv += ":%u" % self.col_no
         return rv
 
     def context_lines(self):
@@ -122,14 +122,23 @@
 
     """
     def __init__(self, brief=False):
         assert isinstance(brief, bool)
         self.brief    = brief
         self.warnings = 0
         self.errors   = 0
+        self.sm       = None
+
+    def cross_file_reference(self, location):
+        assert isinstance(location, Location)
+
+        if self.sm is None:
+            return location.to_string(include_column=False)
+        else:
+            return self.sm.cross_file_reference(location)
 
     def emit(self, location, kind, message, fatal=True):
         assert isinstance(location, Location)
         assert isinstance(kind, str)
         assert isinstance(message, str)
         assert isinstance(fatal, bool)
```

### Comparing `trlc-1.0.9/trlc/lexer.py` & `trlc-1.1.1/trlc/lexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
 # TRLC - Treat Requirements Like Code
-# Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
+# Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This file is part of the TRLC Python Reference Implementation.
 #
 # TRLC is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -15,14 +15,16 @@
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
 import sys
+from fractions import Fraction
+from abc import ABCMeta, abstractmethod
 
 from trlc.errors import Location, Message_Handler
 
 
 def triple_quoted_string_value(raw_value):
     assert isinstance(raw_value, str)
     assert raw_value.startswith("'''")
@@ -60,162 +62,120 @@
         value += "\n" + line[common_len:].rstrip()
 
     return value
 
 
 class Source_Reference(Location):
     def __init__(self, lexer, start_line, start_col, start_pos, end_pos):
-        assert isinstance(lexer, Lexer)
+        assert isinstance(lexer, TRLC_Lexer)
         assert isinstance(start_line, int)
         assert isinstance(start_col, int)
         assert isinstance(start_pos, int)
         assert isinstance(end_pos, int)
-        assert 0 <= start_pos <= end_pos < lexer.file_length
+        assert 0 <= start_pos <= end_pos < lexer.length
         super().__init__(lexer.file_name,
                          start_line,
                          start_col)
         self.lexer     = lexer
         self.start_pos = start_pos
         self.end_pos   = end_pos
 
     def text(self):
-        return self.lexer.file_content[self.start_pos:self.end_pos + 1]
+        return self.lexer.content[self.start_pos:self.end_pos + 1]
 
     def context_lines(self):
         line = ""
         n = self.start_pos
         while n >= 0:
-            if self.lexer.file_content[n] == "\n":
+            if self.lexer.content[n] == "\n":
                 break
-            line = self.lexer.file_content[n] + line
+            line = self.lexer.content[n] + line
             n -= 1
         offset = self.start_pos - n - 1
         n = self.start_pos + 1
-        while n < self.lexer.file_length:
-            if self.lexer.file_content[n] == "\n":
+        while n < self.lexer.length:
+            if self.lexer.content[n] == "\n":
                 break
-            line = line + self.lexer.file_content[n]
+            line = line + self.lexer.content[n]
             n += 1
         maxtrail = n - self.start_pos
         tlen = self.end_pos + 1 - self.start_pos
 
-        return [line,
-                " " * offset + "^" * min(tlen, maxtrail)]
+        stripped_line = line.lstrip()
+        stripped_offset = offset - (len(line) - len(stripped_line))
 
+        return [stripped_line,
+                " " * stripped_offset + "^" * min(tlen, maxtrail)]
 
-class Token:
+
+class Token_Base:
+    def __init__(self, location, kind, value):
+        assert isinstance(location, Location)
+        assert isinstance(kind, str)
+        self.location = location
+        self.kind     = kind
+        self.value    = value
+
+
+class Token(Token_Base):
     KIND = frozenset(["COMMENT",
                       "IDENTIFIER",
                       "BUILTIN",
                       "KEYWORD",
                       "BRA", "KET",
                       "S_BRA", "S_KET",
                       "C_BRA", "C_KET",
+                      "AT",
                       "COMMA",
                       "DOT",
                       "RANGE",
                       "ASSIGN",
                       "OPERATOR",
                       "ARROW",
                       "INTEGER",
+                      "DECIMAL",
                       "STRING"])
 
     def __init__(self, location, kind, value=None):
-        assert isinstance(location, Location)
         assert kind in Token.KIND
         if kind in ("COMMENT", "IDENTIFIER", "BUILTIN",
                     "KEYWORD", "OPERATOR", "STRING"):
             assert isinstance(value, str)
         elif kind == "INTEGER":
             assert isinstance(value, int)
+        elif kind == "DECIMAL":
+            assert isinstance(value, Fraction)
         else:
             assert value is None
-
-        self.location = location
-        self.kind     = kind
-        self.value    = value
+        super().__init__(location, kind, value)
 
     def __repr__(self):
         if self.value is None:
             return "%s_Token" % self.kind
         else:
             return "%s_Token(%s)" % (self.kind, self.value)
 
 
-class Lexer:
-    KEYWORDS = frozenset(["abs",
-                          "and",
-                          "checks",
-                          "else",
-                          "elsif",
-                          "enum",
-                          "error",
-                          "exists",
-                          "extends",
-                          "false",
-                          "fatal",
-                          "forall",
-                          "if",
-                          "implies",
-                          "import",
-                          "in",
-                          "not",
-                          "null",
-                          "optional",
-                          "or",
-                          "package",
-                          "section",
-                          "then",
-                          "true",
-                          "type",
-                          "warning",
-                          "xor"])
-
-    PUNCTUATION = {
-        "(" : "BRA",
-        ")" : "KET",
-        "{" : "C_BRA",
-        "}" : "C_KET",
-        "[" : "S_BRA",
-        "]" : "S_KET",
-        "," : "COMMA",
-        "/" : "OPERATOR",
-        "%" : "OPERATOR",
-        "+" : "OPERATOR",
-        "-" : "OPERATOR",
-    }
-
-    def __init__(self, mh, file_name):
+class Lexer_Base(metaclass=ABCMeta):
+    def __init__(self, mh, content):
         assert isinstance(mh, Message_Handler)
-        assert isinstance(file_name, str)
+        assert isinstance(content, str)
         self.mh        = mh
-        self.file_name = file_name
-
-    def token(self):
-        assert False
+        self.content   = content
+        self.length    = len(self.content)
 
-
-class Python_Lexer(Lexer):
-    def __init__(self, mh, file_name, file_content=None):
-        super().__init__(mh, file_name)
-        if file_content:
-            self.file_content = file_content
-        else:
-            with open(file_name, "r", encoding="UTF-8") as fd:
-                self.file_content = fd.read()
-
-        self.file_length  = len(self.file_content)
-
-        self.lexpos = -2
+        self.lexpos = -3
         self.line_no = 0
         self.col_no  = 0
-        self.cc = None
-        self.nc = None
+        self.cc  = None
+        self.nc  = None
+        self.nnc = None
 
         self.advance()
+        self.advance()
 
     @staticmethod
     def is_alpha(char):
         assert isinstance(char, str) and len(char) == 1
         return ord('a') <= ord(char) <= ord('z') or \
             ord('A') <= ord(char) <= ord('Z')
 
@@ -227,40 +187,117 @@
     @staticmethod
     def is_alnum(char):
         assert isinstance(char, str) and len(char) == 1
         return ord('a') <= ord(char) <= ord('z') or \
             ord('A') <= ord(char) <= ord('Z') or \
             ord('0') <= ord(char) <= ord('9')
 
+    @abstractmethod
+    def file_location(self):
+        pass
+
+    @abstractmethod
+    def token(self):
+        pass
+
+    def skip_whitespace(self):
+        while self.nc and self.nc.isspace():
+            self.advance()
+        self.advance()
+
     def advance(self):
         self.lexpos += 1
         if self.cc == "\n" or self.lexpos == 0:
             self.line_no += 1
             self.col_no = 0
         if self.nc is not None:
             self.col_no += 1
         self.cc = self.nc
-        self.nc = (self.file_content[self.lexpos + 1]
-                   if self.lexpos + 1 < self.file_length
-                   else None)
+        self.nc = self.nnc
+        self.nnc = (self.content[self.lexpos + 2]
+                    if self.lexpos + 2 < self.length
+                    else None)
+
+
+class TRLC_Lexer(Lexer_Base):
+    KEYWORDS = frozenset([
+        "abs",
+        "abstract",
+        "and",
+        "checks",
+        "else",
+        "elsif",
+        "enum",
+        "error",
+        "exists",
+        "extends",
+        "false",
+        "fatal",
+        "final",
+        "forall",
+        "freeze",
+        "if",
+        "implies",
+        "import",
+        "in",
+        "not",
+        "null",
+        "optional",
+        "or",
+        "package",
+        "section",
+        "separator",
+        "then",
+        "true",
+        "tuple",
+        "type",
+        "warning",
+        "xor"
+    ])
+
+    PUNCTUATION = {
+        "(" : "BRA",
+        ")" : "KET",
+        "{" : "C_BRA",
+        "}" : "C_KET",
+        "[" : "S_BRA",
+        "]" : "S_KET",
+        "," : "COMMA",
+        "@" : "AT",
+        "/" : "OPERATOR",
+        "%" : "OPERATOR",
+        "+" : "OPERATOR",
+        "-" : "OPERATOR",
+    }
+
+    def __init__(self, mh, file_name, file_content=None):
+        if file_content:
+            super().__init__(mh, file_content)
+        else:
+            with open(file_name, "r", encoding="UTF-8") as fd:
+                super().__init__(mh, fd.read())
+        self.file_name = file_name
 
     def current_location(self):
         return Source_Reference(lexer      = self,
                                 start_line = self.line_no,
                                 start_col  = self.col_no,
                                 start_pos  = self.lexpos,
                                 end_pos    = self.lexpos)
 
+    def file_location(self):
+        return Location(self.file_name, 1, 1)
+
     def token(self):
         # Skip whitespace and move to the next char
-        while self.nc and self.nc.isspace():
-            self.advance()
-        if self.nc is None:
+        self.skip_whitespace()
+
+        # Return if we're done
+        if self.cc is None:
             return None
-        self.advance()
 
         start_pos  = self.lexpos
         start_line = self.line_no
         start_col  = self.col_no
 
         if self.cc == "/" and self.nc == "/":
             kind = "COMMENT"
@@ -276,16 +313,16 @@
         elif self.is_alpha(self.cc):
             kind = "IDENTIFIER"
             while self.nc and (self.is_alnum(self.nc) or
                                self.nc == "_" or
                                self.nc == ":"):
                 self.advance()
 
-        elif self.cc in Lexer.PUNCTUATION:
-            kind = Lexer.PUNCTUATION[self.cc]
+        elif self.cc in TRLC_Lexer.PUNCTUATION:
+            kind = TRLC_Lexer.PUNCTUATION[self.cc]
 
         elif self.cc == "=":
             if self.nc == ">":
                 kind = "ARROW"
                 self.advance()
             elif self.nc == "=":
                 kind = "OPERATOR"
@@ -372,27 +409,41 @@
                         "unterminated triple-quoted string")
 
         elif self.is_numeric(self.cc):
             kind = "INTEGER"
             while self.nc and self.is_numeric(self.nc):
                 self.advance()
 
+            if self.nc == "." and self.nnc != ".":
+                kind = "DECIMAL"
+                self.advance()
+                if not self.nc or not self.is_numeric(self.nc):
+                    self.mh.lex_error(
+                        Source_Reference(lexer      = self,
+                                         start_line = start_line,
+                                         start_col  = start_col,
+                                         start_pos  = start_pos,
+                                         end_pos    = self.lexpos),
+                        "unfinished decimal number")
+                while self.nc and self.is_numeric(self.nc):
+                    self.advance()
+
         else:
             self.mh.lex_error(self.current_location(),
                               "unexpected character '%s'" % self.cc)
 
         sref = Source_Reference(lexer      = self,
                                 start_line = start_line,
                                 start_col  = start_col,
                                 start_pos  = start_pos,
                                 end_pos    = self.lexpos)
 
         if kind == "IDENTIFIER":
             value = sref.text()
-            if value in Lexer.KEYWORDS:
+            if value in TRLC_Lexer.KEYWORDS:
                 kind = "KEYWORD"
             elif ":" in value:
                 kind = "BUILTIN"
                 if not value.startswith("trlc:"):
                     self.mh.lex_error(sref,
                                       "builtin function name must start "
                                       "with trlc:")
@@ -407,14 +458,17 @@
                 value = value.replace('\\"', '"')
             else:
                 value = triple_quoted_string_value(value)
 
         elif kind == "INTEGER":
             value = int(sref.text())
 
+        elif kind == "DECIMAL":
+            value = Fraction(sref.text())
+
         elif kind == "COMMENT":
             value = sref.text()
             if value.startswith("//"):
                 value = value[2:].strip()
             else:
                 value = value[2:]
                 if value.endswith("*/"):
@@ -423,24 +477,17 @@
 
         else:
             value = None
 
         return Token(sref, kind, value)
 
 
-def create_lexer(mh, file_name):
-    assert isinstance(mh, Message_Handler)
-    assert isinstance(file_name, str)
-
-    return Python_Lexer(mh, file_name)
-
-
 def sanity_test():
     mh    = Message_Handler()
-    lexer = create_lexer(mh, sys.argv[1])
+    lexer = TRLC_Lexer(mh, sys.argv[1])
 
     while True:
         token  = lexer.token()
         if token is None:
             break
         mh.warning(token.location,
                    str(token))
```

### Comparing `trlc-1.0.9/trlc/lint.py` & `trlc-1.1.1/trlc/math.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-from trlc import ast
-from trlc.errors import Message_Handler
+from fractions import Fraction
+from math import floor, ceil
 
 
-def verify_record(mh, record):
-    assert isinstance(mh, Message_Handler)
-    assert isinstance(record, ast.Record_Type)
+def remainder(lhs, rhs):
+    assert isinstance(lhs, int)
+    assert isinstance(rhs, int)
+
+    mod = abs(lhs) % abs(rhs)
+
+    if lhs >= 0:
+        return mod
+    else:
+        return -mod
+
+
+def round_nearest_away(value):
+    assert isinstance(value, Fraction)
+
+    if value >= Fraction(0):
+        return floor(value + Fraction(1, 2))
+    else:
+        return ceil(value - Fraction(1, 2))
```

### Comparing `trlc-1.0.9/trlc/math.py` & `trlc-1.1.1/trlc/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-def remainder(lhs, rhs):
-    assert isinstance(lhs, int)
-    assert isinstance(rhs, int)
+VERSION_TUPLE = (1, 1, 1)
+VERSION_SUFFIX = ""
 
-    mod = abs(lhs) % abs(rhs)
+TRLC_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
+    ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
-    if lhs >= 0:
-        return mod
-    else:
-        return -mod
+FULL_NAME = "TRLC %s" % TRLC_VERSION
```

### Comparing `trlc-1.0.9/trlc/parser.py` & `trlc-1.1.1/trlc/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
 # TRLC - Treat Requirements Like Code
-# Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
+# Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This file is part of the TRLC Python Reference Implementation.
 #
 # TRLC is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,114 +16,280 @@
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
 import re
 
-from trlc.lexer import Token, Lexer, create_lexer
-from trlc.errors import Location, Message_Handler
+from trlc.nested import Nested_Lexer
+from trlc.lexer import Token_Base, Token, Lexer_Base, TRLC_Lexer
+from trlc.errors import Message_Handler
 from trlc import ast
 
 
-class Parser:
-    COMPARISON_OPERATOR = ("==", "!=", "<", "<=", ">", ">=")
-    ADDING_OPERATOR = ("+", "-")
-    MULTIPLYING_OPERATOR = ("*", "/", "%")
+class Markup_Token(Token_Base):
+    KIND = frozenset(["CHARACTER",
+                      "REFLIST_BEGIN",
+                      "REFLIST_END",
+                      "REFLIST_COMMA",
+                      "REFLIST_DOT",
+                      "REFLIST_IDENTIFIER"])
+
+    def __init__(self, location, kind, value):
+        super().__init__(location, kind, value)
+        assert isinstance(value, str)
+
+
+class Markup_Lexer(Nested_Lexer):
+    def __init__(self, mh, literal):
+        super().__init__(mh, literal)
+
+        self.in_reflist = False
+
+    def file_location(self):
+        return self.origin_location
+
+    def token(self):
+        if self.in_reflist:
+            self.skip_whitespace()
+        else:
+            self.advance()
+        if self.cc is None:
+            return None
+
+        start_pos  = self.lexpos
+        start_line = self.line_no
+        start_col  = self.col_no
+
+        if self.cc == "[" and self.nc == "[":
+            kind = "REFLIST_BEGIN"
+            self.advance()
+            if self.in_reflist:
+                self.mh.lex_error(self.source_location(start_line,
+                                                       start_col,
+                                                       start_pos,
+                                                       start_pos + 1),
+                                  "cannot nest reference lists")
+            else:
+                self.in_reflist = True
+
+        elif self.cc == "]" and self.nc == "]":
+            kind = "REFLIST_END"
+            self.advance()
+            if self.in_reflist:
+                self.in_reflist = False
+            else:
+                self.mh.lex_error(self.source_location(start_line,
+                                                       start_col,
+                                                       start_pos,
+                                                       start_pos + 1),
+                                  "opening [[ for this ]] found")
+
+        elif not self.in_reflist:
+            kind = "CHARACTER"
+
+        elif self.cc == ",":
+            kind = "REFLIST_COMMA"
+
+        elif self.cc == ".":
+            kind = "REFLIST_DOT"
+
+        elif self.is_alpha(self.cc):
+            kind = "REFLIST_IDENTIFIER"
+            while self.nc and (self.is_alnum(self.nc) or
+                               self.nc == "_"):
+                self.advance()
 
-    def __init__(self, mh, stab, file_name, lint_mode, lexer=None):
-        assert isinstance(mh, Message_Handler)
-        assert isinstance(stab, ast.Symbol_Table)
-        assert isinstance(file_name, str)
-        assert isinstance(lint_mode, bool)
-        self.mh        = mh
-        self.lint_mode = lint_mode
-        if lexer:
-            self.lexer = lexer
         else:
-            self.lexer = create_lexer(mh, file_name)
-        self.stab      = stab
-        self.pkg       = None
-        self.raw_deps  = []
-        self.deps      = []
-        self.imports   = set()
+            self.mh.lex_error(self.source_location(start_line,
+                                                   start_col,
+                                                   start_pos,
+                                                   start_pos),
+                              "unexpected character '%s'" % self.cc)
+
+        loc = self.source_location(start_line,
+                                   start_col,
+                                   start_pos,
+                                   self.lexpos)
+
+        return Markup_Token(loc,
+                            kind,
+                            self.content[start_pos:self.lexpos + 1])
+
+
+class Parser_Base:
+    def __init__(self, mh, lexer, eoc_name, token_kinds, keywords):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(lexer, Lexer_Base)
+        assert isinstance(eoc_name, str)
+        assert isinstance(token_kinds, frozenset)
+        assert isinstance(keywords, frozenset)
+        self.mh    = mh
+        self.lexer = lexer
+
+        self.eoc_name          = eoc_name
+        self.language_tokens   = token_kinds
+        self.language_keywords = keywords
 
         self.ct = None
         self.nt = None
         self.advance()
 
-        self.builtin_bool = stab.table["Boolean"]
-        self.builtin_int  = stab.table["Integer"]
-        self.builtin_str  = stab.table["String"]
-
-        self.section = []
-        self.default_scope = ast.Scope()
-        self.default_scope.push(self.stab)
-
     def advance(self):
         self.ct = self.nt
         while True:
             self.nt = self.lexer.token()
             if self.nt is None or self.nt.kind != "COMMENT":
                 break
 
     def peek(self, kind):
-        assert kind in Token.KIND
+        assert kind in self.language_tokens
         return self.nt is not None and self.nt.kind == kind
 
     def peek_eof(self):
         return self.nt is None
 
     def peek_kw(self, value):
-        assert value in Lexer.KEYWORDS
+        assert value in self.language_keywords
         return self.peek("KEYWORD") and self.nt.value == value
 
     def match(self, kind):
-        assert kind in Token.KIND
+        assert kind in self.language_tokens
         if self.nt is None:
-            # Note we do not need to handle the case where self.ct is
-            # None like we do in match_kw, since parsing always starts
-            # with a match_kw. At that point we will always have a ct.
-            self.mh.error(self.ct.location,
-                          "expected %s, encountered end-of-file instead" %
-                          kind)
+            if self.ct is None:
+                self.mh.error(self.lexer.file_location(),
+                              "expected %s, encountered %s instead" %
+                              (kind, self.eoc_name))
+            else:
+                self.mh.error(self.ct.location,
+                              "expected %s, encountered %s instead" %
+                              (kind, self.eoc_name))
         elif self.nt.kind != kind:
             self.mh.error(self.nt.location,
                           "expected %s, encountered %s instead" %
                           (kind, self.nt.kind))
         self.advance()
 
     def match_eof(self):
         if self.nt is not None:
             self.mh.error(self.nt.location,
-                          "expected end-of-file, encountered %s instead" %
-                          self.nt.kind)
+                          "expected %s, encountered %s instead" %
+                          (self.eoc_name, self.nt.kind))
 
     def match_kw(self, value):
-        assert value in Lexer.KEYWORDS
+        assert value in self.language_keywords
         if self.nt is None:
             if self.ct is None:
-                # Special case if we encounter an empty file.
-                self.mh.error(Location(self.lexer.file_name, 1, 1),
-                              "expected %s, encountered end-of-file instead" %
-                              value)
+                self.mh.error(self.lexer.file_location(),
+                              "expected %s, encountered %s instead" %
+                              (value, self.eoc_name))
             else:
                 self.mh.error(self.ct.location,
-                              "expected %s, encountered end-of-file instead" %
-                              value)
+                              "expected %s, encountered %s instead" %
+                              (value, self.eoc_name))
         elif self.nt.kind != "KEYWORD":
             self.mh.error(self.nt.location,
                           "expected %s, encountered %s instead" %
                           (value, self.nt.kind))
         elif self.nt.value != value:
             self.mh.error(self.nt.location,
                           "expected %s, encountered %s instead" %
                           (value, self.nt.value))
         self.advance()
 
+
+class Markup_Parser(Parser_Base):
+    def __init__(self, parent, literal):
+        assert isinstance(parent, Parser)
+        super().__init__(parent.mh, Markup_Lexer(parent.mh, literal),
+                         eoc_name    = "end-of-string",
+                         token_kinds = Markup_Token.KIND,
+                         keywords    = frozenset())
+        self.parent     = parent
+        self.references = literal.references
+
+    def parse_all_references(self):
+        while self.nt:
+            if self.peek("CHARACTER"):
+                self.advance()
+            else:
+                self.parse_ref_list()
+        self.match_eof()
+        return self.references
+
+    def parse_ref_list(self):
+        self.match("REFLIST_BEGIN")
+        self.parse_qualified_name()
+        while self.peek("REFLIST_COMMA"):
+            self.match("REFLIST_COMMA")
+            self.parse_qualified_name()
+        self.match("REFLIST_END")
+
+    def parse_qualified_name(self):
+        self.match("REFLIST_IDENTIFIER")
+        if self.peek("REFLIST_DOT"):
+            package = self.parent.stab.lookup_direct(
+                mh                = self.mh,
+                name              = self.ct.value,
+                error_location    = self.ct.location,
+                required_subclass = ast.Package)
+            if package != self.parent.pkg and \
+               package.name not in self.parent.imports:
+                self.mh.error(self.ct.location,
+                              "package must be imported before use")
+
+            self.match("REFLIST_DOT")
+            self.match("REFLIST_IDENTIFIER")
+        else:
+            package = self.parent.pkg
+
+        ref = ast.Record_Reference(location = self.ct.location,
+                                   name     = self.ct.value,
+                                   typ      = None,
+                                   package  = package)
+        self.references.append(ref)
+
+
+class Parser(Parser_Base):
+    COMPARISON_OPERATOR = ("==", "!=", "<", "<=", ">", ">=")
+    ADDING_OPERATOR = ("+", "-")
+    MULTIPLYING_OPERATOR = ("*", "/", "%")
+
+    def __init__(self, mh, stab, file_name, lint_mode, lexer=None):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(stab, ast.Symbol_Table)
+        assert isinstance(file_name, str)
+        assert isinstance(lint_mode, bool)
+        if lexer:
+            super().__init__(mh, lexer,
+                             eoc_name    = "end-of-file",
+                             token_kinds = Token.KIND,
+                             keywords    = TRLC_Lexer.KEYWORDS)
+        else:
+            super().__init__(mh, TRLC_Lexer(mh, file_name),
+                             eoc_name    = "end-of-file",
+                             token_kinds = Token.KIND,
+                             keywords    = TRLC_Lexer.KEYWORDS)
+        self.lint_mode = lint_mode
+        self.stab      = stab
+        self.pkg       = None
+        self.raw_deps  = []
+        self.deps      = []
+        self.imports   = set()
+
+        self.builtin_bool    = stab.table["Boolean"]
+        self.builtin_int     = stab.table["Integer"]
+        self.builtin_decimal = stab.table["Decimal"]
+        self.builtin_str     = stab.table["String"]
+        self.builtin_mstr    = stab.table["Markup_String"]
+
+        self.section = []
+        self.default_scope = ast.Scope()
+        self.default_scope.push(self.stab)
+
     def parse_described_name(self):
         self.match("IDENTIFIER")
         name = self.ct
 
         if self.peek("STRING"):
             self.match("STRING")
             return name, self.ct.value
@@ -131,15 +297,15 @@
             return name, None
 
     def parse_qualified_name(self,
                              scope,
                              required_subclass=None,
                              match_ident=True):
         assert isinstance(scope, ast.Scope)
-        assert isinstance(required_subclass, type)
+        assert required_subclass is None or isinstance(required_subclass, type)
         assert isinstance(match_ident, bool)
 
         if match_ident:
             self.match("IDENTIFIER")
         sym = scope.lookup(self.mh, self.ct)
 
         if isinstance(sym, ast.Package):
@@ -151,112 +317,250 @@
             return sym.symbols.lookup(self.mh, self.ct, required_subclass)
         else:
             return scope.lookup(self.mh, self.ct, required_subclass)
 
     def parse_type_declaration(self):
         if self.peek_kw("enum"):
             self.parse_enum_declaration()
+        elif self.peek_kw("tuple"):
+            self.parse_tuple_declaration()
         else:
             self.parse_record_declaration()
 
     def parse_enum_declaration(self):
         self.match_kw("enum")
         name, description = self.parse_described_name()
 
         enum = ast.Enumeration_Type(name        = name.value,
                                     description = description,
-                                    location    = name.location)
+                                    location    = name.location,
+                                    package     = self.pkg)
         self.pkg.symbols.register(self.mh, enum)
 
         self.match("C_BRA")
         while not self.peek("C_KET"):
             name, description = self.parse_described_name()
             lit = ast.Enumeration_Literal_Spec(name        = name.value,
                                                description = description,
                                                location    = name.location,
                                                enum        = enum)
             enum.literals.register(self.mh, lit)
         self.match("C_KET")
 
+    def parse_tuple_field(self,
+                          n_tuple,
+                          optional_allowed,
+                          optional_reason,
+                          optional_required):
+        assert isinstance(n_tuple, ast.Tuple_Type)
+        assert isinstance(optional_allowed, bool)
+        assert isinstance(optional_reason, str)
+        assert isinstance(optional_required, bool)
+        assert optional_allowed or not optional_required
+
+        field_name, field_description = self.parse_described_name()
+
+        if optional_required or self.peek_kw("optional"):
+            self.match_kw("optional")
+            if optional_allowed:
+                field_is_optional = True
+            else:
+                self.mh.error(self.ct.location, optional_reason)
+        else:
+            field_is_optional = False
+
+        field_type = self.parse_qualified_name(self.default_scope,
+                                               ast.Type)
+
+        return ast.Composite_Component(
+            name        = field_name.value,
+            description = field_description,
+            location    = field_name.location,
+            member_of   = n_tuple,
+            n_typ       = field_type,
+            optional    = field_is_optional)
+
+    def parse_tuple_declaration(self):
+        self.match_kw("tuple")
+        name, description = self.parse_described_name()
+
+        n_tuple = ast.Tuple_Type(name        = name.value,
+                                 description = description,
+                                 location    = name.location,
+                                 package     = self.pkg)
+
+        self.match("C_BRA")
+
+        n_field = self.parse_tuple_field(
+            n_tuple,
+            optional_allowed  = False,
+            optional_reason   = "first field may not be optional",
+            optional_required = False)
+        n_tuple.components.register(self.mh, n_field)
+
+        has_separators    = False
+        optional_required = False
+        separator_allowed = True
+
+        while self.peek_kw("separator") or self.peek("IDENTIFIER"):
+            if has_separators or self.peek_kw("separator"):
+                has_separators = True
+                self.match_kw("separator")
+                if not separator_allowed:
+                    self.mh.error(self.ct.location,
+                                  "either all fields must be separated,"
+                                  " or none")
+                if self.peek("IDENTIFIER") or self.peek("AT"):
+                    self.advance()
+                    n_tuple.add_separator(ast.Separator(self.ct))
+            else:
+                separator_allowed = False
+            n_field = self.parse_tuple_field(
+                n_tuple,
+                optional_allowed  = has_separators,
+                optional_reason   = ("optional only permitted in tuples"
+                                     " with separators"),
+                optional_required = optional_required)
+            n_tuple.components.register(self.mh, n_field)
+            optional_required |= n_field.optional
+
+        self.match("C_KET")
+
+        # Late registration to avoid recursion in tuples
+        self.pkg.symbols.register(self.mh, n_tuple)
+
+    def parse_record_component(self, n_record):
+        assert isinstance(n_record, ast.Record_Type)
+
+        c_name, c_descr = self.parse_described_name()
+        if self.peek_kw("optional"):
+            self.match_kw("optional")
+            c_optional = True
+        else:
+            c_optional = False
+        c_typ = self.parse_qualified_name(self.default_scope,
+                                          ast.Type)
+
+        if self.peek("S_BRA"):
+            self.match("S_BRA")
+            self.match("INTEGER")
+            a_lo = self.ct.value
+            self.match("RANGE")
+            a_loc = self.ct.location
+            if self.peek("INTEGER"):
+                self.match("INTEGER")
+                a_hi = self.ct.value
+                if a_lo > a_hi:
+                    self.mh.error(self.ct.location,
+                                  "upper bound must be at least %u" % a_lo,
+                                  fatal = False)
+                elif a_hi == 0:
+                    self.mh.error(self.ct.location,
+                                  "this array makes no sense",
+                                  fatal = False)
+                elif a_hi == 1 and a_lo == 1:
+                    self.mh.warning(a_loc,
+                                    "array of fixed size 1 "
+                                    "should not be an array")
+                elif a_hi == 1 and a_lo == 0:
+                    self.mh.warning(a_loc,
+                                    "consider making this array an"
+                                    " optional %s" % c_typ.name)
+
+            elif self.peek("OPERATOR") and self.nt.value == "*":
+                self.match("OPERATOR")
+                a_hi = None
+            else:
+                self.mh.error(self.nt.location,
+                              "expected INTEGER or * for upper bound")
+            self.match("S_KET")
+            c_typ = ast.Array_Type(location     = a_loc,
+                                   element_type = c_typ,
+                                   lower_bound  = a_lo,
+                                   upper_bound  = a_hi)
+
+        return ast.Composite_Component(name        = c_name.value,
+                                       description = c_descr,
+                                       location    = c_name.location,
+                                       member_of   = n_record,
+                                       n_typ       = c_typ,
+                                       optional    = c_optional)
+
     def parse_record_declaration(self):
+        if self.peek_kw("abstract"):
+            self.match_kw("abstract")
+            is_abstract = True
+            is_final    = False
+        elif self.peek_kw("final"):
+            self.match_kw("final")
+            is_abstract = False
+            is_final    = True
+        else:
+            is_abstract = False
+            is_final    = False
+
         self.match_kw("type")
         name, description = self.parse_described_name()
 
         if self.peek_kw("extends"):
             self.match_kw("extends")
             root_record = self.parse_qualified_name(self.default_scope,
                                                     ast.Record_Type)
         else:
             root_record = None
 
+        if self.lint_mode and \
+           root_record and root_record.is_final and \
+           not is_final:
+            self.mh.warning(name.location,
+                            "consider clarifying that this record is final")
+
         record = ast.Record_Type(name        = name.value,
                                  description = description,
                                  location    = name.location,
-                                 parent      = root_record)
+                                 package     = self.pkg,
+                                 n_parent    = root_record,
+                                 is_abstract = is_abstract)
         self.pkg.symbols.register(self.mh, record)
 
         self.match("C_BRA")
         while not self.peek("C_KET"):
-            c_name, c_descr = self.parse_described_name()
-            if self.peek_kw("optional"):
-                self.match_kw("optional")
-                c_optional = True
-            else:
-                c_optional = False
-            c_typ = self.parse_qualified_name(self.default_scope,
-                                              ast.Type)
+            if self.peek_kw("freeze"):
+                self.match_kw("freeze")
+                self.match("IDENTIFIER")
+                n_comp = record.components.lookup(self.mh,
+                                                  self.ct,
+                                                  ast.Composite_Component)
+                if record.is_frozen(n_comp):
+                    n_value = record.get_freezing_expression(n_comp)
+                    self.mh.error(
+                        self.ct.location,
+                        "duplicate freezing of %s, previously frozen at %s" %
+                        (n_comp.name,
+                         self.mh.cross_file_reference(n_value.location)))
+                self.match("ASSIGN")
+                n_value = self.parse_value(n_comp.n_typ)
 
-            if self.peek("S_BRA"):
-                self.match("S_BRA")
-                self.match("INTEGER")
-                a_lo = self.ct.value
-                self.match("RANGE")
-                a_loc = self.ct.location
-                if self.peek("INTEGER"):
-                    self.match("INTEGER")
-                    a_hi = self.ct.value
-                    if a_lo > a_hi:
-                        self.mh.error(self.ct.location,
-                                      "upper bound must be at least %u" % a_lo,
-                                      fatal = False)
-                    elif a_hi == 0:
-                        self.mh.error(self.ct.location,
-                                      "this array makes no sense",
-                                      fatal = False)
-                    elif a_hi == 1 and a_lo == 1:
-                        self.mh.warning(a_loc,
-                                        "array of fixed size 1 "
-                                        "should not be an array")
-                    elif a_hi == 1 and a_lo == 0:
-                        self.mh.warning(a_loc,
-                                        "consider making this array an"
-                                        " optional %s" % c_typ.name)
-
-                elif self.peek("OPERATOR") and self.nt.value == "*":
-                    self.match("OPERATOR")
-                    a_hi = None
+                record.frozen[n_comp.name] = n_value
+
+            else:
+                n_comp = self.parse_record_component(record)
+                if record.is_final:
+                    self.mh.error(n_comp.location,
+                                  "cannot declare new components in"
+                                  " final record type")
                 else:
-                    self.mh.error(self.nt.location,
-                                  "expected INTEGER or * for upper bound")
-                self.match("S_KET")
-                c_typ = ast.Array_Type(location     = a_loc,
-                                       element_type = c_typ,
-                                       lower_bound  = a_lo,
-                                       upper_bound  = a_hi)
-
-            comp = ast.Record_Component(name        = c_name.value,
-                                        description = c_descr,
-                                        location    = c_name.location,
-                                        record      = record,
-                                        typ         = c_typ,
-                                        optional    = c_optional)
-            record.components.register(self.mh, comp)
+                    record.components.register(self.mh, n_comp)
 
         self.match("C_KET")
 
+        # Finally mark record final if applicable
+        if is_final:
+            record.is_final = True
+
     def parse_expression(self, scope):
         assert isinstance(scope, ast.Scope)
 
         n_lhs = self.parse_relation(scope)
 
         if self.peek_kw("and"):
             while self.peek_kw("and"):
@@ -423,23 +727,28 @@
             n_lhs = ast.Unary_Expression(
                 mh        = self.mh,
                 location  = t_unary.location,
                 typ       = n_lhs.typ,
                 operator  = un_add_map[t_unary.value],
                 n_operand = n_lhs)
 
+        if isinstance(n_lhs.typ, ast.Builtin_String):
+            rtyp = self.builtin_str
+        else:
+            rtyp = n_lhs.typ
+
         while self.peek("OPERATOR") and \
               self.nt.value in Parser.ADDING_OPERATOR:
             self.match("OPERATOR")
             t_op  = self.ct
             n_rhs = self.parse_term(scope)
             n_lhs = ast.Binary_Expression(
                 mh       = self.mh,
                 location = t_op.location,
-                typ      = n_lhs.typ,
+                typ      = rtyp,
                 operator = bin_add_map[t_op.value],
                 n_lhs    = n_lhs,
                 n_rhs    = n_rhs)
 
         return n_lhs
 
     def parse_term(self, scope):
@@ -482,41 +791,45 @@
         elif self.peek_kw("abs"):
             self.match_kw("abs")
             t_op      = self.ct
             n_operand = self.parse_primary(scope)
             return ast.Unary_Expression(
                 mh        = self.mh,
                 location  = t_op.location,
-                typ       = self.builtin_int,
+                typ       = n_operand.typ,
                 operator  = ast.Unary_Operator.ABSOLUTE_VALUE,
                 n_operand = n_operand)
 
         else:
             n_lhs = self.parse_primary(scope)
             if self.peek("OPERATOR") and self.nt.value == "**":
                 self.match("OPERATOR")
                 t_op  = self.ct
                 n_rhs = self.parse_primary(scope)
                 n_rhs.evaluate(self.mh, None)
                 n_lhs = ast.Binary_Expression(
                     mh       = self.mh,
                     location = t_op.location,
-                    typ      = self.builtin_int,
+                    typ      = n_lhs.typ,
                     operator = ast.Binary_Operator.POWER,
                     n_lhs    = n_lhs,
                     n_rhs    = n_rhs)
             return n_lhs
 
     def parse_primary(self, scope):
         assert isinstance(scope, ast.Scope)
 
         if self.peek("INTEGER"):
             self.match("INTEGER")
             return ast.Integer_Literal(self.ct, self.builtin_int)
 
+        elif self.peek("DECIMAL"):
+            self.match("DECIMAL")
+            return ast.Decimal_Literal(self.ct, self.builtin_decimal)
+
         elif self.peek("STRING"):
             self.match("STRING")
             return ast.String_Literal(self.ct, self.builtin_str)
 
         elif self.peek_kw("true") or self.peek_kw("false"):
             self.match("KEYWORD")
             return ast.Boolean_Literal(self.ct, self.builtin_bool)
@@ -553,26 +866,26 @@
         t_qv = self.ct
         if scope.contains(t_qv.value):
             pdef = scope.lookup(self.mh, t_qv)
             self.mh.error(t_qv.location,
                           "shadows %s %s from %s" %
                           (pdef.__class__.__name__,
                            pdef.name,
-                           pdef.location.to_string(False)))
+                           self.mh.cross_file_reference(pdef.location)))
         self.match_kw("in")
         self.match("IDENTIFIER")
-        field = scope.lookup(self.mh, self.ct, ast.Record_Component)
+        field = scope.lookup(self.mh, self.ct, ast.Composite_Component)
         n_source = ast.Name_Reference(self.ct.location,
                                       field)
-        if not isinstance(field.typ, ast.Array_Type):
+        if not isinstance(field.n_typ, ast.Array_Type):
             self.mh.error(self.ct.location,
                           "you can only quantify over arrays")
         n_var = ast.Quantified_Variable(t_qv.value,
                                         t_qv.location,
-                                        field.typ.element_type)
+                                        field.n_typ.element_type)
         self.match("ARROW")
 
         new_table = ast.Symbol_Table()
         new_table.register(self.mh, n_var)
         scope.push(new_table)
         n_expr = self.parse_expression(scope)
         scope.pop()
@@ -611,19 +924,21 @@
         else_expr = self.parse_expression(scope)
         rv.set_else_part(self.mh, else_expr)
 
         return rv
 
     def parse_builtin(self, scope, n_name, t_name):
         assert isinstance(scope, ast.Scope)
-        assert isinstance(n_name, ast.Builtin_Function)
+        assert isinstance(n_name, (ast.Builtin_Function,
+                                   ast.Builtin_Numeric_Type))
         assert isinstance(t_name, Token)
 
         # Lint: complain about old functions
-        if self.lint_mode and n_name.deprecated:
+        if isinstance(n_name, ast.Builtin_Function) and \
+           self.lint_mode and n_name.deprecated:
             self.mh.warning(
                 t_name.location,
                 "deprecated feature, please use function %s instead" %
                 n_name.name.replace("trlc:", ""))
 
         # Parse the arguments.
         parameters = []
@@ -633,22 +948,26 @@
             if self.peek("COMMA"):
                 self.match("COMMA")
             else:
                 break
         self.match("KET")
 
         # Enforce arity
-        if n_name.arity != len(parameters):
+        if isinstance(n_name, ast.Builtin_Function):
+            required_arity = n_name.arity
+        else:
+            required_arity = 1
+        if required_arity != len(parameters):
             self.mh.error(t_name.location,
-                          "function %requires %u parameters" %
+                          "function requires %u parameters" %
                           n_name.arity)
 
         # Enforce types
         if n_name.name in ("len", "trlc:len"):
-            if parameters[0].typ == self.builtin_str:
+            if isinstance(parameters[0].typ, ast.Builtin_String):
                 return ast.Unary_Expression(
                     mh        = self.mh,
                     location  = t_name.location,
                     typ       = self.builtin_int,
                     operator  = ast.Unary_Operator.STRING_LENGTH,
                     n_operand = parameters[0])
             else:
@@ -672,124 +991,185 @@
                             else ast.Binary_Operator.STRING_ENDSWITH),
                 n_lhs    = parameters[0],
                 n_rhs    = parameters[1])
 
         elif n_name.name in ("matches", "trlc:matches"):
             parameters[1].ensure_type(self.mh, ast.Builtin_String)
             try:
-                # TODO: Fix scope for evaluate()
+                # scope is None on purpose to enforce static context
                 value = parameters[1].evaluate(self.mh, None)
                 assert isinstance(value.typ, ast.Builtin_String)
                 re.compile(value.value)
             except re.error as err:
                 self.mh.error(value.location,
                               str(err))
             return ast.Binary_Expression(
                 mh       = self.mh,
                 location = t_name.location,
                 typ      = self.builtin_bool,
                 operator = ast.Binary_Operator.STRING_REGEX,
                 n_lhs    = parameters[0],
                 n_rhs    = parameters[1])
 
+        elif isinstance(n_name, ast.Builtin_Numeric_Type):
+            parameters[0].ensure_type(self.mh, ast.Builtin_Numeric_Type)
+            if isinstance(n_name, ast.Builtin_Integer):
+                return ast.Unary_Expression(
+                    mh        = self.mh,
+                    location  = t_name.location,
+                    typ       = self.builtin_int,
+                    operator  = ast.Unary_Operator.CONVERSION_TO_INT,
+                    n_operand = parameters[0])
+            elif isinstance(n_name, ast.Builtin_Decimal):
+                return ast.Unary_Expression(
+                    mh        = self.mh,
+                    location  = t_name.location,
+                    typ       = self.builtin_decimal,
+                    operator  = ast.Unary_Operator.CONVERSION_TO_DECIMAL,
+                    n_operand = parameters[0])
+            else:
+                self.mh.ice_loc(t_name.location,
+                                "unexpected type conversion")
+
         else:
             self.mh.ice_loc(t_name.location,
                             "unexpected builtin")
 
     def parse_name(self, scope):
         # This is a bit more complex. The grammar is:
         #
         # qualified_name ::= [ IDENTIFIER_package_name '.' ] IDENTIFIER_name
         #
         # name ::= qualified_name
-        #        | qualified_name ['.' IDENTIFIER_literal]
+        #        | BUILTIN_IDENTIFIER
+        #        | name '.' IDENTIFIER
         #        | name '[' expression ']'
-        #        | IDENTIFIER_builtin_function '(' parameter_list ')'
-        #        | BUILTIN '(' parameter_list ')'
+        #        | name '(' parameter_list ')'
         #
         # parameter_list ::= expression { ',' expression }
+
         assert isinstance(scope, ast.Scope)
 
+        # All names start with a (qualified) identifier. We parse that
+        # first. There is a special complication for functions, as
+        # builtin functions (e.g. len) can shadow record
+        # components. However as functions cannot be stored in
+        # components the true grammar for function calls is always
+        # IDENTIFIER '('; so we can slightly special case this.
+
         if self.peek("BUILTIN"):
             # Legacy builtin function call. The lookup in the root
             # scope is not an error.
             self.match("BUILTIN")
             n_name = self.stab.lookup(self.mh, self.ct, ast.Builtin_Function)
-            return self.parse_builtin(scope, n_name, self.ct)
 
         else:
             self.match("IDENTIFIER")
+            if self.peek("BRA"):
+                # There is one more way we can have a builtin
+                # function, if we follow our name with brackets
+                # immediately.
+                n_name = self.stab.lookup(self.mh,
+                                          self.ct)
+                if not isinstance(n_name, (ast.Builtin_Function,
+                                           ast.Builtin_Numeric_Type)):
+                    self.mh.error(self.ct.location,
+                                  "not a valid builtin function "
+                                  "or numeric type")
+            else:
+                n_name = self.parse_qualified_name(scope, match_ident=False)
+
+        # Enum literals are a bit different, so we deal with themq
+        # first.
+        if isinstance(n_name, ast.Enumeration_Type):
+            self.match("DOT")
+            self.match("IDENTIFIER")
+            lit = n_name.literals.lookup(self.mh,
+                                         self.ct,
+                                         ast.Enumeration_Literal_Spec)
+            return ast.Enumeration_Literal(location = self.ct.location,
+                                           literal  = lit)
+
+        # Anything that remains is either a function call or an actual
+        # name. Let's just enforce this for sanity.
+        if not isinstance(n_name, (ast.Builtin_Function,
+                                   ast.Builtin_Numeric_Type,
+                                   ast.Composite_Component,
+                                   ast.Quantified_Variable,
+                                   )):
+            self.mh.error(self.ct.location,
+                          "%s %s is not a valid name" %
+                          (n_name.__class__.__name__,
+                           n_name.name))
+
+        # Right now function calls and type conversions must be
+        # top-level, so let's get these out of the way as well.
+        if isinstance(n_name, (ast.Builtin_Function,
+                               ast.Builtin_Numeric_Type)):
+            return self.parse_builtin(scope, n_name, self.ct)
+
+        assert isinstance(n_name, (ast.Composite_Component,
+                                   ast.Quantified_Variable))
+
+        # We now process the potentially recursive part:
+        #        | name '.' IDENTIFIER
+        #        | name '[' expression ']'
+        n_name = ast.Name_Reference(location = self.ct.location,
+                                    entity   = n_name)
+
+        while self.peek("DOT") or self.peek("S_BRA"):
+            if self.peek("DOT"):
+                if not isinstance(n_name.typ, ast.Tuple_Type):
+                    self.mh.error(n_name.location,
+                                  "expression '%s' has type %s, "
+                                  "which is not a tuple" %
+                                  (n_name.to_string(),
+                                   n_name.typ.name))
+                self.match("DOT")
+                self.match("IDENTIFIER")
+                n_field = n_name.typ.components.lookup(self.mh,
+                                                       self.ct,
+                                                       ast.Composite_Component)
+                n_name = ast.Field_Access_Expression(
+                    mh       = self.mh,
+                    location = self.ct.location,
+                    n_prefix = n_name,
+                    n_field  = n_field)
 
-            if self.peek("S_BRA"):
-                # Must be an array index on a record field
-                #        | name '[' expression ']'
-                n_name = scope.lookup(self.mh, self.ct, ast.Entity)
+            elif self.peek("S_BRA"):
                 if not isinstance(n_name.typ, ast.Array_Type):
                     self.mh.error(n_name.location,
-                                  "is not of an array type")
-                n_lhs = ast.Name_Reference(location = self.ct.location,
-                                           entity   = n_name)
+                                  "expression '%s' has type %s, "
+                                  "which is not an array" %
+                                  (n_name.to_string(),
+                                   n_name.typ.name))
 
                 self.match("S_BRA")
                 t_bracket = self.ct
                 n_index = self.parse_expression(scope)
                 self.match("S_KET")
-                return ast.Binary_Expression(
+
+                n_name = ast.Binary_Expression(
                     mh       = self.mh,
                     location = t_bracket.location,
                     typ      = n_name.typ.element_type,
                     operator = ast.Binary_Operator.INDEX,
-                    n_lhs    = n_lhs,
+                    n_lhs    = n_name,
                     n_rhs    = n_index)
 
-            elif self.peek("BRA"):
-                # Must be a builtin call
-                #        | IDENTIFIER_builtin_function '(' parameter_list ')'
-                # The lookup in the root scope is not an error. We do
-                # this to avoid finding record fields that happen to
-                # have the same name.
-                n_name = self.stab.lookup(self.mh,
-                                          self.ct,
-                                          ast.Builtin_Function)
-                return self.parse_builtin(scope, n_name, self.ct)
-
-            else:
-                # Must be a qualified name or enumeration
-                # name ::= qualified_name
-                #        | qualified_name ['.' IDENTIFIER_literal]
-                n_name = self.parse_qualified_name(
-                    scope             = scope,
-                    required_subclass = ast.Entity,
-                    match_ident       = False)
-                t_name = self.ct
-
-                if isinstance(n_name, ast.Enumeration_Type):
-                    # If the (qualified) name refers to a enum, then
-                    # we have to narrow it down to a literal.
-                    self.match("DOT")
-                    self.match("IDENTIFIER")
-                    lit = n_name.literals.lookup(self.mh,
-                                                 self.ct,
-                                                 ast.Enumeration_Literal_Spec)
-                    return ast.Enumeration_Literal(location = self.ct.location,
-                                                   literal  = lit)
-
-                else:
-                    # Otherwise we're done
-                    return ast.Name_Reference(location = t_name.location,
-                                              entity   = n_name)
+        return n_name
 
     def parse_check_block(self):
         self.match_kw("checks")
         self.match("IDENTIFIER")
-        record = self.pkg.symbols.lookup(self.mh, self.ct, ast.Record_Type)
+        n_ctype = self.pkg.symbols.lookup(self.mh, self.ct, ast.Composite_Type)
         scope = ast.Scope()
         scope.push(self.stab)
         scope.push(self.pkg.symbols)
-        scope.push(record.components)
+        scope.push(n_ctype.components)
         self.match("C_BRA")
         while not self.peek("C_KET"):
             c_expr = self.parse_expression(scope)
 
             self.match("COMMA")
             if self.peek("KEYWORD"):
                 self.match("KEYWORD")
@@ -802,26 +1182,26 @@
 
             self.match("STRING")
             t_msg = self.ct
 
             if self.peek("COMMA"):
                 self.match("COMMA")
                 self.match("IDENTIFIER")
-                c_anchor = record.components.lookup(self.mh,
-                                                    self.ct,
-                                                    ast.Record_Component)
+                c_anchor = n_ctype.components.lookup(self.mh,
+                                                     self.ct,
+                                                     ast.Composite_Component)
             else:
                 c_anchor = None
 
-            n_check = ast.Check(n_record  = record,
+            n_check = ast.Check(n_type    = n_ctype,
                                 n_expr    = c_expr,
                                 n_anchor  = c_anchor,
                                 severity  = c_sev,
                                 t_message = t_msg)
-            record.add_check(n_check)
+            n_ctype.add_check(n_check)
 
             assert scope.size() == 3
 
         self.match("C_KET")
 
     def parse_section_declaration(self):
         self.match_kw("section")
@@ -848,34 +1228,45 @@
         else:
             self.mh.error(self.ct.location,
                           "expected boolean literal (true or false)")
 
     def parse_value(self, typ):
         assert isinstance(typ, ast.Type)
 
-        if isinstance(typ, ast.Builtin_Integer):
+        if isinstance(typ, ast.Builtin_Numeric_Type):
             if self.peek("OPERATOR") and \
                self.nt.value in Parser.ADDING_OPERATOR:
                 self.match("OPERATOR")
                 t_op = self.ct
                 e_op = (ast.Unary_Operator.PLUS
                         if t_op.value == "+"
                         else ast.Unary_Operator.MINUS)
             else:
                 t_op = None
-            self.match("INTEGER")
-            rv = ast.Integer_Literal(self.ct, self.builtin_int)
+
+            if self.peek("DECIMAL"):
+                self.match("DECIMAL")
+                rv = ast.Decimal_Literal(self.ct, self.builtin_decimal)
+
+            else:
+                self.match("INTEGER")
+                rv = ast.Integer_Literal(self.ct, self.builtin_int)
+
             if t_op:
                 rv = ast.Unary_Expression(mh        = self.mh,
                                           location  = t_op.location,
-                                          typ       = self.builtin_int,
+                                          typ       = rv.typ,
                                           operator  = e_op,
                                           n_operand = rv)
+
             return rv
 
+        elif isinstance(typ, ast.Builtin_Markup_String):
+            return self.parse_markup_string()
+
         elif isinstance(typ, ast.Builtin_String):
             self.match("STRING")
             return ast.String_Literal(self.ct, self.builtin_str)
 
         elif isinstance(typ, ast.Builtin_Boolean):
             return self.parse_boolean()
 
@@ -884,15 +1275,29 @@
             rv = ast.Array_Aggregate(self.ct.location,
                                      typ)
             while not self.peek("S_KET"):
                 rv.append(self.parse_value(typ.element_type))
                 if self.peek("COMMA"):
                     self.match("COMMA")
             self.match("S_KET")
-            # TODO: Check length
+
+            if len(rv.value) < typ.lower_bound:
+                self.mh.error(self.ct.location,
+                              "this array requires at least %u elements "
+                              "(only %u provided)" %
+                              (typ.lower_bound,
+                               len(rv.value)),
+                              fatal=False)
+            if typ.upper_bound and len(rv.value) > typ.upper_bound:
+                self.mh.error(rv.value[typ.upper_bound].location,
+                              "this array requires at most %u elements "
+                              "(%u provided)" %
+                              (typ.upper_bound,
+                               len(rv.value)),
+                              fatal=False)
 
             return rv
 
         elif isinstance(typ, ast.Enumeration_Type):
             enum = self.parse_qualified_name(self.default_scope,
                                              ast.Enumeration_Type)
             if enum != typ:
@@ -903,77 +1308,141 @@
             lit = enum.literals.lookup(self.mh,
                                        self.ct,
                                        ast.Enumeration_Literal_Spec)
             return ast.Enumeration_Literal(self.ct.location,
                                            lit)
 
         elif isinstance(typ, ast.Record_Type):
-            # TODO: Defer name resolution?
-            # TODO: Type check
             self.match("IDENTIFIER")
             t_name = self.ct
             if self.peek("DOT"):
                 self.match("DOT")
                 self.match("IDENTIFIER")
                 the_pkg = self.stab.lookup(self.mh, t_name, ast.Package)
                 if the_pkg != self.pkg and the_pkg.name not in self.imports:
                     self.mh.error(self.ct.location,
                                   "package must be imported before use")
                 t_name = self.ct
             else:
                 the_pkg = self.pkg
 
-            rv = ast.Record_Reference(t_name, typ, the_pkg)
+            rv = ast.Record_Reference(location = t_name.location,
+                                      name     = t_name.value,
+                                      typ      = typ,
+                                      package  = the_pkg)
             if the_pkg.symbols.contains(t_name.value):
                 rv.target = the_pkg.symbols.lookup(self.mh,
                                                    t_name,
                                                    ast.Record_Object)
-                if not rv.target.e_typ.is_subclass_of(typ):
+                if not rv.target.n_typ.is_subclass_of(typ):
                     self.mh.error(t_name.location,
                                   "incorrect type, expected %s but %s is %s" %
                                   (typ.name,
                                    rv.name,
-                                   rv.target.e_typ.name))
+                                   rv.target.n_typ.name))
 
             return rv
 
+        elif isinstance(typ, ast.Tuple_Type) and typ.has_separators():
+            rv = ast.Tuple_Aggregate(self.nt.location, typ)
+
+            next_is_optional = False
+            for n_item in typ.iter_sequence():
+                if isinstance(n_item, ast.Composite_Component):
+                    if next_is_optional and n_item.optional:
+                        break
+                    rv.assign(n_item.name,
+                              self.parse_value(n_item.n_typ))
+
+                elif n_item.token.kind == "AT":
+                    if self.peek("AT"):
+                        self.match("AT")
+                    else:
+                        next_is_optional = True
+
+                elif n_item.token.kind == "IDENTIFIER":
+                    if self.peek("IDENTIFIER") and \
+                       self.nt.value == n_item.token.value:
+                        self.match("IDENTIFIER")
+                    else:
+                        next_is_optional = True
+
+                else:
+                    assert False
+
+            return rv
+
+        elif isinstance(typ, ast.Tuple_Type) and not typ.has_separators():
+            self.match("BRA")
+            rv = ast.Tuple_Aggregate(self.ct.location, typ)
+
+            first = True
+            for n_field in typ.iter_sequence():
+                if first:
+                    first = False
+                else:
+                    self.match("COMMA")
+                rv.assign(n_field.name,
+                          self.parse_value(n_field.n_typ))
+
+            self.match("KET")
+            return rv
+
         else:
             self.mh.ice_loc(self.ct.location,
                             "logic error: unexpected type %s" %
                             typ.__class__.__name__)
 
+    def parse_markup_string(self):
+        self.match("STRING")
+        rv = ast.String_Literal(self.ct, self.builtin_mstr)
+        mpar = Markup_Parser(self, rv)
+        mpar.parse_all_references()
+        return rv
+
     def parse_record_object_declaration(self):
         r_typ = self.parse_qualified_name(self.default_scope,
                                           ast.Record_Type)
+        if r_typ.is_abstract:
+            self.mh.error(self.ct.location,
+                          "cannot declare object of abstract record type %s" %
+                          r_typ.name)
+
         self.match("IDENTIFIER")
         obj = ast.Record_Object(
             name     = self.ct.value,
             location = self.ct.location,
-            e_typ    = r_typ,
+            n_typ    = r_typ,
             section  = self.section[-1] if self.section else None)
         self.pkg.symbols.register(self.mh, obj)
         self.match("C_BRA")
         while not self.peek("C_KET"):
             self.match("IDENTIFIER")
             comp = r_typ.components.lookup(self.mh,
                                            self.ct,
-                                           ast.Record_Component)
+                                           ast.Composite_Component)
+            if r_typ.is_frozen(comp):
+                self.mh.error(self.ct.location,
+                              "cannot overwrite frozen component %s" %
+                              comp.name)
             self.match("ASSIGN")
-            value = self.parse_value(comp.typ)
+            value = self.parse_value(comp.n_typ)
             obj.assign(comp, value)
 
         # Check that each non-optional component has been specified
         for comp in r_typ.all_components():
             if obj.field[comp.name] is None:
-                if not comp.optional:
+                if r_typ.is_frozen(comp):
+                    obj.assign(comp, r_typ.get_freezing_expression(comp))
+                elif not comp.optional:
                     self.mh.error(
                         obj.location,
                         "required component %s (see %s) is not defined" %
                         (comp.name,
-                         comp.location.to_string(False)))
+                         self.mh.cross_file_reference(comp.location)))
                 else:
                     obj.assign(comp, ast.Implicit_Null(obj, comp))
 
         self.match("C_KET")
 
     def parse_trlc_entry(self):
         if self.peek_kw("section"):
@@ -996,21 +1465,19 @@
             self.match("IDENTIFIER")
             self.raw_deps.append(self.ct)
             self.imports.add(self.ct.value)
 
     def parse_rsl_file(self):
         assert self.pkg is not None
 
-        while self.peek_kw("enum") or \
-              self.peek_kw("type") or \
-              self.peek_kw("checks"):
-            if self.peek_kw("enum") or self.peek_kw("type"):
-                self.parse_type_declaration()
-            else:
+        while not self.peek_eof():
+            if self.peek_kw("checks"):
                 self.parse_check_block()
+            else:
+                self.parse_type_declaration()
 
         self.match_eof()
 
     def parse_check_file(self):
         self.match_kw("package")
         self.match("IDENTIFIER")
```

### Comparing `trlc-1.0.9/trlc/trlc.py` & `trlc-1.1.1/trlc/trlc.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
+import re
 import os
+import sys
 import json
 from argparse import ArgumentParser
+from fractions import Fraction
 
 from trlc import ast
 from trlc import lint
 from trlc.errors import TRLC_Error, Location, Message_Handler
 from trlc.parser import Parser
 from trlc.version import TRLC_VERSION
 
@@ -45,21 +48,49 @@
 
     """
     def __init__(self, mh, lint_mode=False):
         assert isinstance(mh, Message_Handler)
         assert isinstance(lint_mode, bool)
 
         self.mh          = mh
+        self.mh.sm       = self
         self.stab        = ast.Symbol_Table.create_global_table(mh)
         self.rsl_files   = {}
         self.check_files = {}
         self.trlc_files  = {}
         self.packages    = {}
         self.lint_mode   = lint_mode
 
+        self.exclude_patterns = []
+
+        self.common_root    = None
+
+    def cross_file_reference(self, location):
+        assert isinstance(location, Location)
+
+        if self.common_root is None:
+            return location.to_string(False)
+        else:
+            return "%s:%u" % (os.path.relpath(location.file_name,
+                                              self.common_root),
+                              location.line_no)
+
+    def update_common_root(self, file_name):
+        assert isinstance(file_name, str)
+
+        if self.common_root is None:
+            self.common_root = os.path.dirname(os.path.abspath(file_name))
+        else:
+            new_root = os.path.dirname(os.path.abspath(file_name))
+            for n, (char_a, char_b) in enumerate(zip(self.common_root,
+                                                     new_root)):
+                if char_a != char_b:
+                    self.common_root = self.common_root[0:n]
+                    break
+
     def create_parser(self, file_name):
         assert os.path.isfile(file_name)
 
         return Parser(mh           = self.mh,
                       stab         = self.stab,
                       file_name    = file_name,
                       lint_mode    = self.lint_mode)
@@ -120,26 +151,37 @@
 
         :return: true if the directory could be registered without issues
         :rtype: bool
         """
         assert os.path.isdir(dir_name)
 
         ok = True
-        for path, _, files in os.walk(dir_name):
+        for path, dirs, files in os.walk(dir_name):
+            for n, dirname in reversed(list(enumerate(dirs))):
+                keep = True
+                for exclude_pattern in self.exclude_patterns:
+                    if exclude_pattern.match(dirname):
+                        keep = False
+                        break
+                if not keep:
+                    del dirs[n]
+
             for file_name in sorted(files):
                 if os.path.splitext(file_name)[1] in (".rsl",
                                                       ".check",
                                                       ".trlc"):
                     ok &= self.register_file(os.path.join(path, file_name))
         return ok
 
     def register_rsl_file(self, file_name):
         assert os.path.isfile(file_name)
         assert file_name not in self.rsl_files
 
+        self.update_common_root(file_name)
+
         self.rsl_files[file_name] = self.create_parser(file_name)
         self.rsl_files[file_name].parse_rsl_header()
 
         self.register_package(
             package_name = self.rsl_files[file_name].pkg.name,
             file_name    = file_name)
         for import_name in self.rsl_files[file_name].raw_deps:
@@ -147,20 +189,22 @@
                 package_name = self.rsl_files[file_name].pkg.name,
                 import_name  = import_name.value)
 
     def register_check_file(self, file_name):
         assert os.path.isfile(file_name)
         assert file_name not in self.check_files
 
+        self.update_common_root(file_name)
         self.check_files[file_name] = self.create_parser(file_name)
 
     def register_trlc_file(self, file_name):
         assert os.path.isfile(file_name)
         assert file_name not in self.trlc_files
 
+        self.update_common_root(file_name)
         self.trlc_files[file_name] = self.create_parser(file_name)
 
     def parse_rsl_files(self):
         # First, check that each package import is known
         for parser in self.rsl_files.values():
             for t_import in parser.raw_deps:
                 parser.deps.append(parser.stab.lookup(self.mh,
@@ -239,22 +283,16 @@
                         ok = False
                 except TRLC_Error:
                     ok = False
 
         return ok
 
     def perform_sanity_checks(self):
-        ok = True
-        for package in self.stab.values(ast.Package):
-            for obj in package.symbols.values(ast.Record_Type):
-                try:
-                    lint.verify_record(self.mh, obj)
-                except TRLC_Error:
-                    ok = False
-        return ok
+        linter = lint.Linter(self.mh, self.stab)
+        return linter.verify()
 
     def process(self):
         """Parse all registered files.
 
         :return: a symbol table (or None if there were any errors)
         :rtype: Symbol_Table
         """
@@ -273,27 +311,14 @@
 
         # If we run in lint mode, then we perform the checks now and then
         # stop. We do not process the TRLC files.
         if self.lint_mode:
             if not ok:
                 return None
             self.perform_sanity_checks()
-            summary = "Verified %u model(s) and check(s)" % \
-                (len(self.rsl_files) + len(self.check_files))
-            summary += " and found"
-            if self.mh.errors and self.mh.warnings:
-                summary += " %u warning(s)" % self.mh.warnings
-                summary += " and %u error(s)" % self.mh.errors
-            elif self.mh.warnings:
-                summary += " %u warning(s)" % self.mh.warnings
-            elif self.mh.errors:
-                summary += " %u error(s)" % self.mh.errors
-            else:
-                summary += " no issues"
-            print(summary)
             return None if self.mh.errors or self.mh.warnings else self.stab
 
         # Parse TRLC files. Almost all the semantic analysis and name
         # resolution happens here, with the notable exception of resolving
         # record references (as we can have circularity here).
         if not self.parse_trlc_files():
             return None
@@ -330,37 +355,113 @@
                     default=False,
                     action="store_true",
                     help="dump json")
     ap.add_argument("--brief",
                     default=False,
                     action="store_true",
                     help="simpler output intended for CI")
-    ap.add_argument("dir_name",
-                    metavar="DIR")
+    ap.add_argument("items",
+                    nargs="*",
+                    metavar="DIR|FILE")
+    ap.add_argument("--include-bazel-dirs",
+                    action="store_true",
+                    help="by default we do not enter bazel-* directories")
+    ap.add_argument("--show-file-list",
+                    action="store_true",
+                    help=("if there are no errors, produce a summary "
+                          "naming every file processed"))
     options = ap.parse_args()
 
     mh = Message_Handler(options.brief)
     sm = Source_Manager(mh, options.lint)
 
-    if not os.path.isdir(options.dir_name):
-        ap.error("%s is not a directory" % options.dir_name)
+    if not options.include_bazel_dirs:
+        sm.exclude_patterns.append(re.compile("^bazel-.*$"))
+
+    for path_name in options.items:
+        if not (os.path.isdir(path_name) or
+                os.path.isfile(path_name)):
+            ap.error("%s is not a file or directory" % path_name)
+
+    # Process input files, defaulting to the current directory if none
+    # given.
+    ok = True
+    if options.items:
+        for path_name in options.items:
+            if os.path.isdir(path_name):
+                ok &= sm.register_directory(path_name)
+            else:
+                try:
+                    ok &= sm.register_file(path_name)
+                except TRLC_Error:
+                    ok = False
+    else:
+        ok &= sm.register_directory(".")
 
-    # Process input files
-    ok = sm.register_directory(options.dir_name)
     if not ok:
         return 1
 
     if sm.process() is None:
-        return 1
-    else:
+        ok = False
+
+    if ok:
         if options.debug_dump:
             sm.stab.dump()
         if options.debug_api_dump:
             tmp = {}
             for obj in sm.stab.iter_record_objects():
                 tmp[obj.name] = obj.to_python_dict()
+                for key in tmp[obj.name]:
+                    if isinstance(tmp[obj.name][key], Fraction):
+                        tmp[obj.name][key] = float(tmp[obj.name][key])
+
             print(json.dumps(tmp, indent=2, sort_keys=True))
+
+    if options.show_file_list or options.lint:
+        if options.lint:
+            summary = "Verified"
+        else:
+            summary = "Processed"
+
+        summary += " %u model(s)" % len(sm.rsl_files)
+        if options.lint:
+            summary += " and"
+        else:
+            summary += ", "
+        summary += " %u check(s)" % len(sm.check_files)
+        if not options.lint:
+            summary += " and %u requirement file(s)" % len(sm.trlc_files)
+
+        summary += " and found"
+
+        if mh.errors and mh.warnings:
+            summary += " %u warning(s)" % mh.warnings
+            summary += " and %u error(s)" % mh.errors
+        elif mh.warnings:
+            summary += " %u warning(s)" % mh.warnings
+        elif mh.errors:
+            summary += " %u error(s)" % mh.errors
+        else:
+            summary += " no issues"
+
+        print(summary)
+
+        if options.show_file_list and ok:
+            for filename in sorted(sm.rsl_files):
+                print("> Model %s (Package %s)" %
+                      (filename, sm.rsl_files[filename].pkg.name))
+            for filename in sorted(sm.check_files):
+                print("> Checks %s (Package %s)" %
+                      (filename, sm.check_files[filename].pkg.name))
+            if not options.lint:
+                for filename in sorted(sm.trlc_files):
+                    print("> Requirements %s (Package %s)" %
+                          (filename, sm.trlc_files[filename].pkg.name))
+
+    if ok:
         return 0
+    else:
+        return 1
 
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

### Comparing `trlc-1.0.9/trlc.egg-info/PKG-INFO` & `trlc-1.1.1/trlc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.0.9
+Version: 1.1.1
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/trlc
-Description: # Treat Requirements Like Code (TRLC)
-        TRLC is a domain-specific language developed at BMW for writing (and
-        linking) requirements with meta-data.
-        
-        The repository contains:
-        
-        * The [language reference
-          manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-          for TRLC.
-        
-        * A pure Python reference implementation of TRLC.
-        
-        The implementation is not very fast, but designed to be pedantically
-        correct in following the language definition.  Eventually it will also
-        contain a powerful linter to find issues with types and check
-        rules.
-        
-        The Python implementation can be used for several purposes:
-        
-        * It can be used to validate other TRLC implementations.
-        
-        * It can be used to validate a body of requirements (e.g. a CI check
-          that all requirements are well formed)
-        
-        * The API can be used to write other tools based on TRLC (for example
-          a tool to render the requirements in HTML, a tool to diff
-          requirements or perform an impact analysis, or a tool to perform
-          software traceability, etc.)
-        
-        ## Documentation
-        
-        * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
-        * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
-        * [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
-          (user guide for using the API)
-        * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-          (for language lawyers)
-        * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
-        
-        ## Dependencies
-        
-        ### Run-time
-        * Python3 >= 3.7
-        
-        ### Development tools
-        * GNU Make
-        * [PyCodeStyle](https://pypi.org/project/pycodestyle/) (from PyPI, for
-          basic checking of source code style)
-        * [PyLint](https://pypi.org/project/pylint/) (from PyPI, for basic bug
-          finding)
-        * [Coverage](https://pypi.org/project/coverage/) (from PyPI, to
-          perform branch coverage when running the test suite)
-        * [Sphinx](https://pypi.org/project/Sphinx/) (from PyPI, for building
-          the documentation)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Treat Requirements Like Code (TRLC)
+TRLC is a domain-specific language developed at BMW for writing (and
+linking) requirements with meta-data.
+
+The repository contains:
+
+* The [language reference
+  manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+  for TRLC.
+
+* A pure Python reference implementation of TRLC.
+
+The implementation is not very fast, but designed to be pedantically
+correct in following the language definition.  Eventually it will also
+contain a powerful linter to find issues with types and check
+rules.
+
+The Python implementation can be used for several purposes:
+
+* It can be used to validate other TRLC implementations.
+
+* It can be used to validate a body of requirements (e.g. a CI check
+  that all requirements are well formed)
+
+* The API can be used to write other tools based on TRLC (for example
+  a tool to render the requirements in HTML, a tool to diff
+  requirements or perform an impact analysis, or a tool to perform
+  software traceability, etc.)
+
+## Documentation
+
+* [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
+* [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
+* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
+  (user guide for using the API)
+* [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+  (for language lawyers)
+* [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
+
+## Dependencies
+
+### Run-time
+* Python3 >= 3.7
+
+### Development tools
+* GNU Make
+* [PyCodeStyle](https://pypi.org/project/pycodestyle/) (from PyPI, for
+  basic checking of source code style)
+* [PyLint](https://pypi.org/project/pylint/) (from PyPI, for basic bug
+  finding)
+* [Coverage](https://pypi.org/project/coverage/) (from PyPI, to
+  perform branch coverage when running the test suite)
+* [Sphinx](https://pypi.org/project/Sphinx/) (from PyPI, for building
+  the documentation)
```

