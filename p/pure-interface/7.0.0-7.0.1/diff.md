# Comparing `tmp/pure_interface-7.0.0.tar.gz` & `tmp/pure_interface-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-kobqf76v\pure_interface-7.0.0.tar", last modified: Wed Mar  1 22:56:18 2023, max compression
+gzip compressed data, was "D:\Source\pure_interface\dist\.tmp-fphbqodx\pure_interface-7.0.1.tar", last modified: Thu Apr 27 23:18:02 2023, max compression
```

## Comparing `pure_interface-7.0.0.tar` & `pure_interface-7.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 22:56:18.602761 pure_interface-7.0.0/
--rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.0.0/LICENSE
--rw-rw-rw-   0        0        0    33881 2023-03-01 22:56:18.602761 pure_interface-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    32913 2023-03-01 22:45:31.000000 pure_interface-7.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-01 22:56:18.576853 pure_interface-7.0.0/pure_interface/
--rw-rw-rw-   0        0        0      617 2023-03-01 21:51:46.000000 pure_interface-7.0.0/pure_interface/__init__.py
--rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.0.0/pure_interface/adaption.py
--rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.0.0/pure_interface/data_classes.py
--rw-rw-rw-   0        0        0     7720 2023-03-01 21:56:00.000000 pure_interface-7.0.0/pure_interface/delegation.py
--rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.0.0/pure_interface/errors.py
--rw-rw-rw-   0        0        0    33894 2023-03-01 21:44:06.000000 pure_interface-7.0.0/pure_interface/interface.py
-drwxrwxrwx   0        0        0        0 2023-03-01 22:56:18.581836 pure_interface-7.0.0/pure_interface.egg-info/
--rw-rw-rw-   0        0        0    33881 2023-03-01 22:56:18.000000 pure_interface-7.0.0/pure_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-03-01 22:56:18.000000 pure_interface-7.0.0/pure_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 22:56:18.000000 pure_interface-7.0.0/pure_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-01 22:56:18.000000 pure_interface-7.0.0/pure_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2023-03-01 22:56:18.604755 pure_interface-7.0.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 22:56:18.601765 pure_interface-7.0.0/tests/
--rw-rw-rw-   0        0        0     3843 2023-03-01 21:34:51.000000 pure_interface-7.0.0/tests/test_adapt_args_anno.py
--rw-rw-rw-   0        0        0     2871 2023-03-01 21:34:51.000000 pure_interface-7.0.0/tests/test_adapt_args_no_anno.py
--rw-rw-rw-   0        0        0    12205 2023-03-01 21:43:08.000000 pure_interface-7.0.0/tests/test_adaption.py
--rw-rw-rw-   0        0        0     1022 2023-03-01 21:34:51.000000 pure_interface-7.0.0/tests/test_dataclass_support.py
--rw-rw-rw-   0        0        0     7462 2023-03-01 22:34:11.000000 pure_interface-7.0.0/tests/test_delegate.py
--rw-rw-rw-   0        0        0     5935 2023-03-01 21:34:51.000000 pure_interface-7.0.0/tests/test_func_sigs3.py
--rw-rw-rw-   0        0        0    11757 2023-03-01 21:34:51.000000 pure_interface-7.0.0/tests/test_function_sigs.py
--rw-rw-rw-   0        0        0      844 2023-03-01 20:45:17.000000 pure_interface-7.0.0/tests/test_generic_support.py
--rw-rw-rw-   0        0        0    16881 2023-03-01 21:44:32.000000 pure_interface-7.0.0/tests/test_implementation_checks.py
--rw-rw-rw-   0        0        0     2803 2023-03-01 21:36:02.000000 pure_interface-7.0.0/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     4040 2023-03-01 21:43:40.000000 pure_interface-7.0.0/tests/test_isinstance.py
--rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.0.0/tests/test_meta_classes.py
--rw-rw-rw-   0        0        0     2877 2023-03-01 21:36:02.000000 pure_interface-7.0.0/tests/test_module_funcs.py
--rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.0.0/tests/test_no_content_checks.py
--rw-rw-rw-   0        0        0     2071 2023-03-01 21:36:02.000000 pure_interface-7.0.0/tests/test_tracker.py
--rw-rw-rw-   0        0        0      514 2023-03-01 21:36:02.000000 pure_interface-7.0.0/tests/test_versions_in_sync.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.710468 pure_interface-7.0.1/
+-rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-7.0.1/LICENSE
+-rw-rw-rw-   0        0        0    34872 2023-04-27 23:18:02.710468 pure_interface-7.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    33904 2023-04-27 23:17:43.000000 pure_interface-7.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.683948 pure_interface-7.0.1/pure_interface/
+-rw-rw-rw-   0        0        0      617 2023-04-27 23:17:43.000000 pure_interface-7.0.1/pure_interface/__init__.py
+-rw-rw-rw-   0        0        0     7884 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/adaption.py
+-rw-rw-rw-   0        0        0     2167 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/data_classes.py
+-rw-rw-rw-   0        0        0     8441 2023-04-27 23:17:43.000000 pure_interface-7.0.1/pure_interface/delegation.py
+-rw-rw-rw-   0        0        0      372 2023-03-01 20:08:43.000000 pure_interface-7.0.1/pure_interface/errors.py
+-rw-rw-rw-   0        0        0    33894 2023-04-27 05:33:41.000000 pure_interface-7.0.1/pure_interface/interface.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.688467 pure_interface-7.0.1/pure_interface.egg-info/
+-rw-rw-rw-   0        0        0    34872 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 23:18:02.000000 pure_interface-7.0.1/pure_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2021-09-21 22:43:47.000000 pure_interface-7.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1088 2023-04-27 23:18:02.712468 pure_interface-7.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2021-09-21 22:43:47.000000 pure_interface-7.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:18:02.709468 pure_interface-7.0.1/tests/
+-rw-rw-rw-   0        0        0     3843 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adapt_args_anno.py
+-rw-rw-rw-   0        0        0     2871 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adapt_args_no_anno.py
+-rw-rw-rw-   0        0        0    12205 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_adaption.py
+-rw-rw-rw-   0        0        0     1022 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_dataclass_support.py
+-rw-rw-rw-   0        0        0     8573 2023-04-27 23:17:43.000000 pure_interface-7.0.1/tests/test_delegate.py
+-rw-rw-rw-   0        0        0     5935 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_func_sigs3.py
+-rw-rw-rw-   0        0        0    11757 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_function_sigs.py
+-rw-rw-rw-   0        0        0      844 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_generic_support.py
+-rw-rw-rw-   0        0        0    16881 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_implementation_checks.py
+-rw-rw-rw-   0        0        0     2803 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     4040 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_isinstance.py
+-rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-7.0.1/tests/test_meta_classes.py
+-rw-rw-rw-   0        0        0     2877 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_module_funcs.py
+-rw-rw-rw-   0        0        0     3364 2023-03-01 20:08:43.000000 pure_interface-7.0.1/tests/test_no_content_checks.py
+-rw-rw-rw-   0        0        0     2071 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_tracker.py
+-rw-rw-rw-   0        0        0      514 2023-04-27 05:33:41.000000 pure_interface-7.0.1/tests/test_versions_in_sync.py
```

### Comparing `pure_interface-7.0.0/LICENSE` & `pure_interface-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/PKG-INFO` & `pure_interface-7.0.1/pure_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure_interface
-Version: 7.0.0
+Name: pure-interface
+Version: 7.0.1
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
@@ -473,15 +473,17 @@
 
 Sometimes when adapting objects to an interface the adapter has to route attributes and methods to another object.
 the ``Delegate`` class assists with this task reducing boiler plate code such as::
 
     def method(self):
         return self.impl.method()
 
-The ``Delegate`` class provides 3 special attributes to route attributes to a child object.
+The ``Delegate`` class provides 3 special attributes to route attributes to a child object.  Only attributes and mothods
+not defined on the class (or super-classes) are routed.  (Attributes and methods defined on an interface sub-class are not
+considered part of the implementation and these attributes are routed.)
 Any one or combination of attributes is allowed.
 
 pi_attr_delegates
 --------------
 ``pi_attr_delegates`` is a dictionary mapping delegate attribute names to either an interface or a list of attribute names.
 If an interface is given then the list returned by ``get_interface_names()`` is used for the attribute names to route to the delegate object.
 For example suppose we want to extend an Animal with a new method ``price``::
@@ -555,15 +557,28 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.
+instead.  If you want to override using an instance attribute, first define it as a class attribute::
+
+    class MyDelegate(Delegate, IFoo):
+        pi_attr_delegates = {'impl': IFoo}
+        foo = None  # prevents delegation of foo to `impl`
+
+        def __init__(self, impl):
+            self.impl = impl
+            self.foo = 3
+
+If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
+ ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
+Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
+Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
 Composition
 -----------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
```

### Comparing `pure_interface-7.0.0/README.rst` & `pure_interface-7.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -451,15 +451,17 @@
 
 Sometimes when adapting objects to an interface the adapter has to route attributes and methods to another object.
 the ``Delegate`` class assists with this task reducing boiler plate code such as::
 
     def method(self):
         return self.impl.method()
 
-The ``Delegate`` class provides 3 special attributes to route attributes to a child object.
+The ``Delegate`` class provides 3 special attributes to route attributes to a child object.  Only attributes and mothods
+not defined on the class (or super-classes) are routed.  (Attributes and methods defined on an interface sub-class are not
+considered part of the implementation and these attributes are routed.)
 Any one or combination of attributes is allowed.
 
 pi_attr_delegates
 --------------
 ``pi_attr_delegates`` is a dictionary mapping delegate attribute names to either an interface or a list of attribute names.
 If an interface is given then the list returned by ``get_interface_names()`` is used for the attribute names to route to the delegate object.
 For example suppose we want to extend an Animal with a new method ``price``::
@@ -533,15 +535,28 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.
+instead.  If you want to override using an instance attribute, first define it as a class attribute::
+
+    class MyDelegate(Delegate, IFoo):
+        pi_attr_delegates = {'impl': IFoo}
+        foo = None  # prevents delegation of foo to `impl`
+
+        def __init__(self, impl):
+            self.impl = impl
+            self.foo = 3
+
+If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
+ ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
+Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
+Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
 Composition
 -----------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
```

### Comparing `pure_interface-7.0.0/pure_interface/__init__.py` & `pure_interface-7.0.1/pure_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 from .delegation import Delegate
 
 try:
     from .data_classes import dataclass
 except ImportError:
     pass
 
-__version__ = '7.0.0'
+__version__ = '7.0.1'
```

### Comparing `pure_interface-7.0.0/pure_interface/adaption.py` & `pure_interface-7.0.1/pure_interface/adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/pure_interface/data_classes.py` & `pure_interface-7.0.1/pure_interface/data_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/pure_interface/delegation.py` & `pure_interface-7.0.1/pure_interface/delegation.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,42 +94,60 @@
             def foo(self):
                 return self.impl.foo * 2
 
             def bar(self, baz):
                 return 'my bar'
 
     However, attempting to set an instance attribute as an override will just set the property on the underlying
-    delegate.
+    delegate.  If you want to override using an instance attribute, first define it as a class attribute
+
+        class MyDelegate(Delegate, IFoo):
+            pi_attr_delegates = {'impl': IFoo}
+            foo = None  # prevents delegation of foo to `impl`
+
+            def __init__(self, impl):
+                self.impl = impl
+                self.foo = 3
+
     """
     pi_attr_fallback = None
     pi_attr_delegates = {}
     pi_attr_mapping = {}
 
     def __init_subclass__(cls, **kwargs):
+        # get non-interface base class ignoring abc.ABC and object.
+        non_interface_bases = [base for base in cls.mro()[:-2] if not type_is_interface(base)]
+
+        def i_have_attribute(attrib):
+            for klass in non_interface_bases:
+                if attrib in klass.__dict__:
+                    return True
+            return False
+
         for delegate, attr_list in cls.pi_attr_delegates.items():
             if isinstance(attr_list, type):
                 attr_list = list(get_interface_names(attr_list))
             if delegate in cls.pi_attr_mapping:
                 raise ValueError(f'Delegate {delegate} is in pi_attr_map')
             for attr in attr_list:
                 if attr in cls.pi_attr_mapping:
                     raise ValueError(f'{attr} in pi_attr_map and handled by delegate {delegate}')
-                if attr in cls.__dict__:
+                if i_have_attribute(attr):
                     continue
                 dotted_name = f'{delegate}.{attr}'
                 setattr(cls, attr, _Delegated(dotted_name))
         for attr, dotted_name in cls.pi_attr_mapping.items():
-            if attr not in cls.__dict__:
+            if not i_have_attribute(attr):
                 setattr(cls, attr, _Delegated(dotted_name))
         if cls.pi_attr_fallback:
             fallback = cls.pi_attr_fallback
             for interface in get_type_interfaces(cls):
                 interface_names = get_interface_names(interface)
                 for attr in interface_names:
-                    if attr not in cls.__dict__:
+                    if not i_have_attribute(attr):
                         dotted_name = f'{fallback}.{attr}'
                         setattr(cls, attr, _Delegated(dotted_name))
 
     @classmethod
     def provided_by(cls, obj):
         if not hasattr(cls, 'pi_composed_interfaces'):
             raise InterfaceError('provided_by() can only be called on composed types')
```

### Comparing `pure_interface-7.0.0/pure_interface/interface.py` & `pure_interface-7.0.1/pure_interface/interface.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/pure_interface.egg-info/PKG-INFO` & `pure_interface-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pure-interface
-Version: 7.0.0
+Name: pure_interface
+Version: 7.0.1
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Home-page: https://github.com/seequent/pure_interface
 Download-URL: https://pypi.org/project/pure-interface/
 Author: Tim Mitchell
 Author-email: tim.mitchell@seequent.com
 License: MIT
 Keywords: abc interface adapt adaption mapper structural typing dataclass
@@ -473,15 +473,17 @@
 
 Sometimes when adapting objects to an interface the adapter has to route attributes and methods to another object.
 the ``Delegate`` class assists with this task reducing boiler plate code such as::
 
     def method(self):
         return self.impl.method()
 
-The ``Delegate`` class provides 3 special attributes to route attributes to a child object.
+The ``Delegate`` class provides 3 special attributes to route attributes to a child object.  Only attributes and mothods
+not defined on the class (or super-classes) are routed.  (Attributes and methods defined on an interface sub-class are not
+considered part of the implementation and these attributes are routed.)
 Any one or combination of attributes is allowed.
 
 pi_attr_delegates
 --------------
 ``pi_attr_delegates`` is a dictionary mapping delegate attribute names to either an interface or a list of attribute names.
 If an interface is given then the list returned by ``get_interface_names()`` is used for the attribute names to route to the delegate object.
 For example suppose we want to extend an Animal with a new method ``price``::
@@ -555,15 +557,28 @@
         def foo(self):
             return self.impl.foo * 2
 
         def bar(self, baz):
             return 'my bar'
 
 However, attempting to set an instance attribute as an override will just set the attribute on the underlying delegate
-instead.
+instead.  If you want to override using an instance attribute, first define it as a class attribute::
+
+    class MyDelegate(Delegate, IFoo):
+        pi_attr_delegates = {'impl': IFoo}
+        foo = None  # prevents delegation of foo to `impl`
+
+        def __init__(self, impl):
+            self.impl = impl
+            self.foo = 3
+
+If you supply more than one delegation rule (e.g. both ``pi_attr_mapping`` and ``pi_attr_fallack``) then
+ ``pi_attr_delegates`` delegates are created first and any attributes defined there are now part of the class.
+Then ``pi_attr_mapping`` delegates are created (and become part of the class) and finally ``pi_attr_fallback`` is processed.
+Thus if there are duplicate delegates defined, the one defined first takes precedence.
 
 Composition
 -----------
 A special case where all delegated attributes are defined in an ``Interface`` is handled by the ``composed_type`` factory function.
 ``composed_type`` takes 2 or more interfaces and returns a new type that inherits from all the interfaces with a
 constructor that takes instances that implement those interfaces (in the same order).  For exmaple::
```

### Comparing `pure_interface-7.0.0/pure_interface.egg-info/SOURCES.txt` & `pure_interface-7.0.1/pure_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/setup.cfg` & `pure_interface-7.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7572 655f 696e 7465 7266 6163   = pure_interfac
 00000020: 650d 0a76 6572 7369 6f6e 203d 2037 2e30  e..version = 7.0
-00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
+00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
 00000040: 3d20 4120 5079 7468 6f6e 2069 6e74 6572  = A Python inter
 00000050: 6661 6365 206c 6962 7261 7279 2074 6861  face library tha
 00000060: 7420 6469 7361 6c6c 6f77 7320 6675 6e63  t disallows func
 00000070: 7469 6f6e 2062 6f64 7920 636f 6e74 656e  tion body conten
 00000080: 7420 6f6e 2069 6e74 6572 6661 6365 7320  t on interfaces 
 00000090: 616e 6420 7375 7070 6f72 7473 2061 6461  and supports ada
 000000a0: 7074 696f 6e2e 0d0a 6b65 7977 6f72 6473  ption...keywords
```

### Comparing `pure_interface-7.0.0/tests/test_adapt_args_anno.py` & `pure_interface-7.0.1/tests/test_adapt_args_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_adapt_args_no_anno.py` & `pure_interface-7.0.1/tests/test_adapt_args_no_anno.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_adaption.py` & `pure_interface-7.0.1/tests/test_adaption.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_dataclass_support.py` & `pure_interface-7.0.1/tests/test_dataclass_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_delegate.py` & `pure_interface-7.0.1/tests/test_delegate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import dataclasses
+
 import pure_interface
 import unittest
 from unittest import mock
 
 from pure_interface import delegation
 
 
@@ -25,41 +27,59 @@
         return 'talk'
 
 
 class IPoint(pure_interface.Interface):
     x: int
     y: int
 
+    def to_str(self) -> str:
+        pass
+
+
+class IPoint3(IPoint):
+    z: int
+
+
+@dataclasses.dataclass
+class PointImpl:
+    x: int
+    y: int
+    z: int
+
 
 class Point(IPoint, object):
     def __init__(self, x=0, y=1):
         self.x = int(x)
         self.y = int(y)
 
+    def to_str(self) -> str:
+        return f'{self.x}, {self.y}'
+
 
 class DFallback(delegation.Delegate, ITalker):
     pi_attr_fallback = 'impl'
 
     def __init__(self, impl):
         self.impl = impl
 
 
 class DAttrMap(delegation.Delegate, IPoint):
     pi_attr_mapping = {'x': 'a.x',
-                    'y': 'b.y',
-                    }
+                       'y': 'b.y',
+                       'to_str': 'b.to_str',
+                       }
 
     def __init__(self, a, b):
         self.a = a
         self.b = b
 
 
 class DDelegateList(delegation.Delegate, IPoint):
-    pi_attr_delegates = {'a': ['x'],
-                      'b': ['x', 'y']}
+    pi_attr_delegates = {'a': ['x', 'to_str'],
+                         'b': ['x', 'y']}
 
     def __init__(self, a, b):
         self.a = a
         self.b = b
 
 
 class DDelegateIFace(delegation.Delegate, IPoint, ITalker):
@@ -106,14 +126,36 @@
 
     def __init__(self):
         a = Talker()
         a.b = Point(3, 4)
         self.a = a
 
 
+class ScaledPoint(pure_interface.Delegate, IPoint):
+    pi_attr_fallback = '_p'
+
+    def __init__(self, point):
+        self._p = point
+
+    @property
+    def y(self):
+        return self._p.y * 2
+
+    @y.setter
+    def y(self, value):
+        self._p.y = int(value // 2)
+
+    def to_str(self) -> str:
+        return f'{self.x}, {self.y}'
+
+
+class ScaledPoint3(ScaledPoint, IPoint3):
+    pi_attr_fallback = '_p'
+
+
 class DelegateTest(unittest.TestCase):
     def test_descriptor_get_class(self):
         d = pure_interface.delegation._Delegated('foo.bar')
 
         e = d.__get__(None, mock.Mock)
         self.assertIs(d, e)
 
@@ -219,14 +261,24 @@
     def test_double_dotted_delegate(self):
         d = DoubleDottedDelegate()
         self.assertEqual(3, d.x)
         self.assertEqual(4, d.y)
         d.x = 1
         self.assertEqual(1, d.a.b.x)
 
+    def test_delegate_subclass(self):
+        """test that subclass methods are not delegated """
+        p = PointImpl(1, 2, 3)
+        d3 = ScaledPoint3(p)
+        self.assertEqual(4, d3.y)
+        self.assertEqual('1, 4', d3.to_str())
+        d3.y = 8  # delegates to p
+        self.assertEqual(4, p.y)
+        self.assertEqual(3, d3.z)
+
 
 class CompositionTest(unittest.TestCase):
 
     def test_type_composition(self):
         a = Point(1, 2)
         b = Talker()
```

### Comparing `pure_interface-7.0.0/tests/test_func_sigs3.py` & `pure_interface-7.0.1/tests/test_func_sigs3.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_function_sigs.py` & `pure_interface-7.0.1/tests/test_function_sigs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_generic_support.py` & `pure_interface-7.0.1/tests/test_generic_support.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_implementation_checks.py` & `pure_interface-7.0.1/tests/test_implementation_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_inheritance.py` & `pure_interface-7.0.1/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_isinstance.py` & `pure_interface-7.0.1/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_meta_classes.py` & `pure_interface-7.0.1/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_module_funcs.py` & `pure_interface-7.0.1/tests/test_module_funcs.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_no_content_checks.py` & `pure_interface-7.0.1/tests/test_no_content_checks.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_tracker.py` & `pure_interface-7.0.1/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pure_interface-7.0.0/tests/test_versions_in_sync.py` & `pure_interface-7.0.1/tests/test_versions_in_sync.py`

 * *Files identical despite different names*

