# Comparing `tmp/runtype-0.3.1.tar.gz` & `tmp/runtype-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtype-0.3.1.tar", max compression
+gzip compressed data, was "runtype-0.3.2.tar", max compression
```

## Comparing `runtype-0.3.1.tar` & `runtype-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.1/LICENSE
--rw-r--r--   0        0        0      928 2022-11-17 13:27:54.194061 runtype-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4098 2022-10-11 13:06:17.811390 runtype-0.3.1/README.md
--rw-r--r--   0        0        0     1207 2022-11-17 13:26:31.679440 runtype-0.3.1/runtype/__init__.py
--rw-r--r--   0        0        0     9279 2022-10-11 12:52:05.446440 runtype-0.3.1/runtype/base_types.py
--rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.1/runtype/common.py
--rw-r--r--   0        0        0    12602 2022-11-16 17:32:54.177843 runtype-0.3.1/runtype/dataclass.py
--rw-r--r--   0        0        0     8098 2021-12-14 13:06:00.734037 runtype-0.3.1/runtype/datetime_parse.py
--rw-r--r--   0        0        0     5815 2022-10-11 12:52:05.448440 runtype-0.3.1/runtype/dispatch.py
--rw-r--r--   0        0        0      838 2022-10-11 12:52:05.449333 runtype-0.3.1/runtype/mypy.py
--rw-r--r--   0        0        0     3115 2022-06-25 08:55:10.918634 runtype-0.3.1/runtype/mypy_bu.py
--rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.1/runtype/py.typed
--rw-r--r--   0        0        0    12707 2022-10-11 12:52:09.938000 runtype-0.3.1/runtype/pytypes.py
--rw-r--r--   0        0        0      496 2022-10-11 12:52:05.450340 runtype-0.3.1/runtype/typesystem.py
--rw-r--r--   0        0        0     1237 2022-10-11 12:52:09.939346 runtype-0.3.1/runtype/utils.py
--rw-r--r--   0        0        0     3193 2022-10-11 12:52:09.940352 runtype-0.3.1/runtype/validation.py
--rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 runtype-0.3.1/setup.py
--rw-r--r--   0        0        0     5115 1970-01-01 00:00:00.000000 runtype-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1196 2023-04-28 16:04:39.515338 runtype-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4098 2022-10-11 13:06:17.811390 runtype-0.3.2/README.md
+-rw-r--r--   0        0        0     1536 2023-04-28 16:04:28.218617 runtype-0.3.2/runtype/__init__.py
+-rw-r--r--   0        0        0     9279 2022-10-11 12:52:05.446440 runtype-0.3.2/runtype/base_types.py
+-rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.2/runtype/common.py
+-rw-r--r--   0        0        0    13658 2023-04-17 13:00:48.910623 runtype-0.3.2/runtype/dataclass.py
+-rw-r--r--   0        0        0     8098 2021-12-14 13:06:00.734037 runtype-0.3.2/runtype/datetime_parse.py
+-rw-r--r--   0        0        0     5839 2023-04-17 13:00:48.912622 runtype-0.3.2/runtype/dispatch.py
+-rw-r--r--   0        0        0      823 2023-04-17 13:00:48.914621 runtype-0.3.2/runtype/mypy.py
+-rw-r--r--   0        0        0     3115 2022-06-25 08:55:10.918634 runtype-0.3.2/runtype/mypy_bu.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.2/runtype/py.typed
+-rw-r--r--   0        0        0    15107 2023-04-17 13:00:48.916621 runtype-0.3.2/runtype/pytypes.py
+-rw-r--r--   0        0        0      552 2023-04-17 13:00:48.919622 runtype-0.3.2/runtype/typesystem.py
+-rw-r--r--   0        0        0     1379 2023-04-17 13:00:48.921619 runtype-0.3.2/runtype/utils.py
+-rw-r--r--   0        0        0     3520 2023-04-17 13:00:48.924620 runtype-0.3.2/runtype/validation.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 runtype-0.3.2/setup.py
+-rw-r--r--   0        0        0     5194 1970-01-01 00:00:00.000000 runtype-0.3.2/PKG-INFO
```

### Comparing `runtype-0.3.1/LICENSE` & `runtype-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runtype-0.3.1/pyproject.toml` & `runtype-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runtype"
-version = "0.3.1"
+version = "0.3.2"
 description = "Type dispatch and validation for run-time Python"
 authors = ["Erez Shinan <erezshin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/erezsh/runtype"
 keywords = ["types", "typing", "dispatch", "multimethods", "dataclass", "runtime"]
 classifiers = [
@@ -18,11 +18,26 @@
 ]
 packages = [{ include = "runtype" }]
 
 
 [tool.poetry.dependencies]
 python = "^3.6"
 dataclasses = {version = "*", python = "~3.6"}
+contextvars = {version = "*", python = "~3.6"}
+
+[tool.poetry.dev-dependencies]
+typing_extensions = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+# addopts = "-ra -q"
+testpaths = [
+    "tests",
+]
+
+[tool.ruff]
+line-length = 120
+target-version = "py311"
```

### Comparing `runtype-0.3.1/README.md` & `runtype-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `runtype-0.3.1/runtype/base_types.py` & `runtype-0.3.2/runtype/base_types.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.1/runtype/dataclass.py` & `runtype-0.3.2/runtype/dataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Enhances Python's built-in dataclass, with type-checking and extra ergonomics.
 """
 
 import random
 from copy import copy
 import dataclasses
-from typing import Union
+from typing import Union, Any, Tuple, Callable, TypeVar
 from abc import ABC, abstractmethod
 import inspect
 
 from .utils import ForwardRef
 from .common import CHECK_TYPES
 from .validation import TypeMismatchError, ensure_isa as default_ensure_isa
-from .pytypes import TypeCaster, type_caster, SumType, NoneType
+from .pytypes import TypeCaster, SumType, NoneType
 
 Required = object()
 MAX_SAMPLE_SIZE = 16
 
 class NopTypeCaster:
     cache = {}
     def to_canon(self, t):
@@ -109,47 +109,55 @@
             type_ = ForwardRef(type_)
         type_ = type_caster.to_canon(type_)
         if field.default is None:
             type_ = SumType([type_, NoneType])
         type_caster.cache[id(field)] = type_
         return type_
 
+def _validate_attr(config, should_cast, sampler, obj, name, type_, value):
+    try:
+        if should_cast:    # Basic cast
+            assert not sampler
+            try:
+                config.ensure_isa(value, type_, sampler)
+                return value
+            except TypeMismatchError:
+                return config.cast(value, type_)
+        else:
+            config.ensure_isa(value, type_, sampler)
+    except TypeMismatchError as e:
+        item_value, item_type = e.args
+        msg = f"[{type(obj).__name__}] Attribute '{name}' expected a value of type '{type_}'."
+        msg += f" Instead got type '{type(value).__name__}', with value {value!r}."
+        if item_value is not value:
+            msg += f'\n\n    Failed on item: {item_value!r}, expected type {item_type}'
+        raise TypeError(msg)
+
 def _post_init(self, config, should_cast, sampler, type_caster):
     for name, field in getattr(self, '__dataclass_fields__', {}).items():
         value = getattr(self, name)
 
         if value is Required:
             raise TypeError(f"Field {name} requires a value")
 
         type_ = _get_field_type(type_caster, field)
-
-        try:
-            if should_cast:    # Basic cast
-                assert not sampler
-                value = config.cast(value, type_)
-                object.__setattr__(self, name, value)
-            else:
-                config.ensure_isa(value, type_, sampler)
-        except TypeMismatchError as e:
-            item_value, item_type = e.args
-            msg = f"[{type(self).__name__}] Attribute '{name}' expected value of type '{type_}'."
-            msg += f" Instead got {value!r}"
-            if item_value is not value:
-                msg += f'\n\n    Failed on item: {item_value!r}, expected type {item_type}'
-            raise TypeError(msg)
+        new_value = _validate_attr(config, should_cast, sampler, self, name, type_, value)
+        if new_value is not None:
+            object.__setattr__(self, name, new_value)
 
 
-def _setattr(self, name, value, config, type_caster):
+def _setattr(obj, setattr, name, value, config, should_cast, sampler, type_caster):
     try:
-        field = self.__dataclass_fields__[name]
+        field = obj.__dataclass_fields__[name]
     except (KeyError, AttributeError):
-        pass
+        new_value = None
     else:
         type_ = _get_field_type(type_caster, field)
-        config.ensure_isa(value, type_)
+        new_value = _validate_attr(config, should_cast, sampler, obj, name, type_, value)
+    setattr(obj, name, value if new_value is None else new_value)
 
 
 def replace(inst, **kwargs):
     """Returns a new instance, with the given attibutes and values overwriting the existing ones.
 
     Useful for making copies with small updates.
 
@@ -240,29 +248,29 @@
     if check_types:
         c = copy(cls)
 
         orig_post_init = getattr(cls, '__post_init__', None)
         sampler = _sample if check_types=='sample' else None
         # eval_type_string = EvalInContext(context_frame)
         type_caster = config.make_type_caster(context_frame)
+        should_cast = check_types == 'cast'
 
         def __post_init__(self):
             # Only now context_frame has complete information
-            _post_init(self, config=config, should_cast=check_types == 'cast', sampler=sampler, type_caster=type_caster)
+            _post_init(self, config=config, should_cast=should_cast, sampler=sampler, type_caster=type_caster)
             if orig_post_init is not None:
                 orig_post_init(self)
 
         c.__post_init__ = __post_init__
 
         if not kw['frozen']:
             orig_set_attr = getattr(cls, '__setattr__')
 
             def __setattr__(self, name, value):
-                _setattr(self, name, value, config, type_caster)
-                orig_set_attr(self, name, value)
+                _setattr(self, orig_set_attr, name, value, config, should_cast, sampler, type_caster)
 
             c.__setattr__ = __setattr__
     else:
         c = cls
 
     _set_if_not_exists(c, {
         'replace': replace,
@@ -311,31 +319,46 @@
         # Need this for pickling frozen classes with slots.
         cls.__getstate__ = _dataclass_getstate
         cls.__setstate__ = _dataclass_setstate
 
     return cls
 
 
+# This is a super-ugly hack called PEP-0681. https://peps.python.org/pep-0681/
+_T = TypeVar("_T")
+def __dataclass_transform__(
+    *,
+    eq_default: bool = True,
+    order_default: bool = False,
+    kw_only_default: bool = False,
+    field_descriptors: Tuple[Union[type, Callable[..., Any]], ...] = (()),
+) -> Callable[[_T], _T]:
+    return lambda a: a
+
+
+@__dataclass_transform__(eq_default=True, order_default=True)
 def dataclass(cls=None, *, check_types: Union[bool, str] = CHECK_TYPES,
                            config: Configuration = PythonConfiguration(),
-                           init=True, repr=True, eq=True, order=False, unsafe_hash=False, frozen=True, slots=False):
+                           init=True, repr=True, eq=True, order=False,
+                           unsafe_hash=False, frozen=True, slots=False) -> Any:
     """Runtype's dataclass is a drop-in replacement to Python's built-in dataclass, with added functionality.
 
     **Differences from builtin dataclass:**
 
     1. Type validation
       - Adds run-time type validation (when check_types is nonzero)
       - Performs automatic casting (when check_types == 'cast')
 
     2. Ergonomics
       - Supports assigning mutable literals (i.e. list, set, and dict).
       - Adds convenience methods: replace(), aslist(), astuple(), and iterator for dict(this).
         These methods won't override existing ones. They will be added only if the names aren't used.
       - Setting the default as ``None`` automatically makes the type into ``Optional``, if it isn't already.
-      - Members without a default are allowed after members with a default (but they are required to create the instance)
+      - Members without a default are allowed after members with a default
+        (but they are required in order to create the instance)
 
     3. Misc
       - Frozen by default
 
     All of the above differences are configurable and extendable.
 
 
@@ -362,15 +385,16 @@
             Point(x=30, y=3)
     """
     assert isinstance(config, Configuration)
 
     context_frame = inspect.currentframe().f_back   # Get parent frame, to resolve forward-references
     def wrap(cls):
         return _process_class(cls, config, check_types, context_frame,
-                              init=init, repr=repr, eq=eq, order=order, unsafe_hash=unsafe_hash, frozen=frozen, slots=slots)
+                              init=init, repr=repr, eq=eq, order=order,
+                              unsafe_hash=unsafe_hash, frozen=frozen, slots=slots)
 
     # See if we're being called as @dataclass or @dataclass().
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as @dataclass without parens.
```

### Comparing `runtype-0.3.1/runtype/datetime_parse.py` & `runtype-0.3.2/runtype/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.1/runtype/dispatch.py` & `runtype-0.3.2/runtype/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,16 @@
                          for i, a in enumerate(args))
 
         return tuple(map(get_type, args))
 
     def find_function(self, args):
         nodes = [self.root]
         for i, a in enumerate(args):
-            nodes = [n for node in nodes for n in node.follow_arg(a, self.typesystem, test_subtype=i in self.test_subtypes)]
+            nodes = [n for node in nodes
+                       for n in node.follow_arg(a, self.typesystem, test_subtype=i in self.test_subtypes)]
 
         funcs = [node.func for node in nodes if node.func]
 
         if len(funcs) == 0:
             raise DispatchError(f"Function '{self.name}' not found for signature {self.get_arg_types(args)}")
         elif len(funcs) > 1:
             f, _sig = self.choose_most_specific_function(*funcs)
```

### Comparing `runtype-0.3.1/runtype/mypy.py` & `runtype-0.3.2/runtype/mypy.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [mypy]
 plugins = runtype.mypy
 
 """
 
 from typing import Callable, Optional, Type
 
-from mypy.plugin import ClassDefContext, MethodContext, Plugin
+from mypy.plugin import ClassDefContext, Plugin
 from mypy.plugins import dataclasses
 
 DATACLASS_PATHS = {"runtype.dataclass.dataclass"}
 
 
 def plugin(version: str) -> "Type[Plugin]":
     """
```

### Comparing `runtype-0.3.1/runtype/mypy_bu.py` & `runtype-0.3.2/runtype/mypy_bu.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.1/runtype/pytypes.py` & `runtype-0.3.2/runtype/pytypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,34 @@
 from datetime import datetime
 
 from .utils import ForwardRef
 from .base_types import DataType, Validator, TypeMismatchError
 from . import base_types
 from . import datetime_parse
 
+
+if sys.version_info < (3, 9):
+    if sys.version_info < (3, 7):
+        # python 3.6 
+        _orig_eval = ForwardRef._eval_type
+    else:
+        _orig_eval = ForwardRef._evaluate
+
+    def _forwardref_evaluate(self, glob, loc, _):
+        return _orig_eval(self, glob, loc)
+else:
+    _forwardref_evaluate = ForwardRef._evaluate
+
+try:
+    import typing_extensions
+except ImportError:
+    typing_extensions = None
+
+
+
 py38 = sys.version_info >= (3, 8)
 
 
 class LengthMismatchError(TypeMismatchError):
     pass
 
 
@@ -61,14 +81,24 @@
         if self.types and len(obj) != len(self.types):
             raise LengthMismatchError(self, obj)
         for type_, item in zip(self.types, obj):
             type_.validate_instance(item, sampler)
 
 
 class SumType(base_types.SumType, PythonType):
+    def __init__(self, types):
+        # Here we merge all the instances of OneOf into a single one (if necessary).
+        # The alternative is to turn all OneOf instances into SumTypes of single values.
+        # I chose this method due to intuition that it's faster for the common use-case.
+        one_ofs: List[OneOf] = [t for t in types if isinstance(t, OneOf)]
+        if len(one_ofs) > 1:
+            rest = [t for t in types if not isinstance(t, OneOf)]
+            types = rest + [OneOf([v for t in one_ofs for v in t.values])]
+        super().__init__(types)
+
     def validate_instance(self, obj, sampler=None):
         if not any(t.test_instance(obj) for t in self.types):
             raise TypeMismatchError(obj, self)
 
     def cast_from(self, obj):
         for t in self.types:
             with suppress(TypeError):
@@ -143,27 +173,49 @@
 
     def validate_instance(self, obj, sampler=None):
         if not isinstance(obj, tuple):
             raise TypeMismatchError(obj, self)
 
 
 class OneOf(PythonType):
+    values: typing.Sequence
+
     def __init__(self, values):
         self.values = values
 
     def __le__(self, other):
+        if isinstance(other, OneOf):
+            return set(self.values) <= set(other.values)
+        elif isinstance(other, PythonType):
+            try:
+                for v in self.values:
+                    other.validate_instance(v)
+            except TypeMismatchError:
+                return False
+            return True
+        return NotImplemented
+
+    def __ge__(self, other):
+        if isinstance(other, OneOf):
+            return set(self.values) >= set(other.values)
+        elif isinstance(other, PythonType):
+            return False
         return NotImplemented
 
     def validate_instance(self, obj, sampler=None):
         if obj not in self.values:
             raise TypeMismatchError(obj, self)
 
     def __repr__(self):
         return 'Literal[%s]' % ', '.join(map(repr, self.values))
 
+    def cast_from(self, obj):
+        if obj not in self.values:
+            raise TypeMismatchError(obj, self)
+
 
 class GenericType(base_types.GenericType, PythonType):
     def __init__(self, base, item=Any):
         return super().__init__(base, item)
 
 
 class SequenceType(GenericType):
@@ -238,19 +290,14 @@
 TupleEllipsis = SequenceType(PythonDataType(tuple))
 # Float = PythonDataType(float)
 Bytes = PythonDataType(bytes)
 Callable = PythonDataType(abc.Callable)  # TODO: Generic
 Literal = OneOf
 
 
-class _NoneType(PythonDataType):
-    def cast_from(self, obj):
-        if obj is not None:
-            raise TypeMismatchError(obj, self)
-
 class _Number(PythonDataType):
     def __call__(self, min=None, max=None):
         predicates = []
         if min is not None:
             predicates += [lambda i: i >= min]
         if max is not None:
             predicates += [lambda i: i <= max]
@@ -286,18 +333,29 @@
             try:
                 return datetime_parse.parse_datetime(obj)
             except datetime_parse.DateTimeError:
                 raise TypeMismatchError(obj, self)
         return super().cast_from(obj)
 
 
+class _NoneType(OneOf):
+    def __init__(self):
+        super().__init__([None])
+
+    def cast_from(self, obj):
+        assert self.values == [None]
+        if obj is not None:
+            raise TypeMismatchError(obj, self)
+        return None
+
+
 String = _String(str)
 Int = _Int(int)
 Float = _Float(float)
-NoneType = _NoneType(type(None))
+NoneType =  _NoneType()
 DateTime = _DateTime(datetime)
 
 
 _type_cast_mapping = {
     iter: Iter,
     list: List,
     set: Set,
@@ -338,19 +396,29 @@
     def _to_canon(self, t):
         to_canon = self.to_canon
 
         if isinstance(t, (base_types.Type, Validator)):
             return t
 
         if isinstance(t, ForwardRef):
-            t = t._evaluate(self.frame.f_globals, self.frame.f_locals, set())
+            t = _forwardref_evaluate(t, self.frame.f_globals, self.frame.f_locals, set())
 
         if isinstance(t, tuple):
             return SumType([to_canon(x) for x in t])
 
+        if hasattr(typing, '_AnnotatedAlias') and isinstance(t, typing._AnnotatedAlias):
+            return to_canon(t.__origin__)
+
+        if typing_extensions:
+            if hasattr(typing_extensions, '_AnnotatedAlias') and isinstance(t, typing_extensions._AnnotatedAlias):
+                return to_canon(t.__origin__)
+            elif hasattr(typing_extensions, 'AnnotatedMeta') and isinstance(t, typing_extensions.AnnotatedMeta):
+                # Python 3.6
+                return to_canon(t.__args__[0])
+
         try:
             t.__origin__
         except AttributeError:
             pass
         else:
             if getattr(t, '__args__', None) is None:
                 if t is typing.List:
@@ -385,27 +453,27 @@
                     if len(t.__args__) != 2 or t.__args__[0] == Ellipsis:
                         raise ValueError("Tuple with '...'' expected to be of the exact form: tuple[t, ...].")
                     return TupleEllipsis[to_canon(t.__args__[0])]
 
                 return ProductType([to_canon(x) for x in t.__args__])
 
             elif t.__origin__ is typing.Union:
-                return SumType([to_canon(x) for x in t.__args__])
+                res = [to_canon(x) for x in t.__args__]
+                return SumType(res)
             elif t.__origin__ is abc.Callable or t is typing.Callable:
                 # return Callable[ProductType(to_canon(x) for x in t.__args__)]
                 return Callable  # TODO
             elif py38 and t.__origin__ is typing.Literal:
                 return OneOf(t.__args__)
             elif t.__origin__ is abc.Mapping or t.__origin__ is typing.Mapping:
                 k, v = t.__args__
                 return Mapping[to_canon(k), to_canon(v)]
             elif t.__origin__ is abc.Sequence or t.__origin__ is typing.Sequence:
                 x ,= t.__args__
                 return Sequence[to_canon(x)]
-
             elif t.__origin__ is type or t.__origin__ is typing.Type:
                 # TODO test issubclass on t.__args__
                 return PythonDataType(type)
 
             raise NotImplementedError("No support for type:", t)
 
         if isinstance(t, typing.TypeVar):
```

### Comparing `runtype-0.3.1/runtype/utils.py` & `runtype-0.3.2/runtype/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 import inspect
 import sys
+import contextvars
+from contextlib import contextmanager
 
 if sys.version_info < (3, 7):
     # python 3.6 
     from typing import _ForwardRef as ForwardRef
-    _orig_eval = ForwardRef._eval_type
-elif sys.version_info < (3, 9):
-    from typing import ForwardRef
-    _orig_eval = ForwardRef._evaluate
 else:
-    from typing import ForwardRef
-
-if sys.version_info < (3, 9):
-    def _evaluate(self, g, l, _):
-        return _orig_eval(self, g, l)
-    ForwardRef._evaluate = _evaluate
-
-
+    from typing import ForwardRef as ForwardRef
 
 def get_func_signatures(typesystem, f):
     sig = inspect.signature(f)
     typesigs = []
     typesig = []
     for p in sig.parameters.values():
         # if p.kind is p.VAR_KEYWORD or p.kind is p.VAR_POSITIONAL:
@@ -37,7 +28,23 @@
             # From now on, everything is optional
             typesigs.append(list(typesig))
 
         typesig.append(t)
 
     typesigs.append(typesig)
     return typesigs
+
+
+class ContextVar:
+    def __init__(self, default, name=''):
+        self._var = contextvars.ContextVar(name, default=default)
+
+    def get(self):
+        return self._var.get()
+
+    @contextmanager
+    def __call__(self, value):
+        token = self._var.set(value)
+        try:
+            yield
+        finally:
+            self._var.reset(token)
```

### Comparing `runtype-0.3.1/runtype/validation.py` & `runtype-0.3.2/runtype/validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 "User-facing API for validation"
 
-from typing import Any, Dict, List, Tuple, Set, FrozenSet, Callable
+from typing import Any, Dict, List, Tuple, Set, FrozenSet
 from functools import wraps
 
 from .common import CHECK_TYPES
-from .utils import get_func_signatures
+from .utils import get_func_signatures, ContextVar
 from .pytypes import TypeMismatchError, type_caster
 from .typesystem import TypeSystem
 
+# cv_type_checking allows the user to define different behaviors for their objects
+# while they are being type-checked.
+# This is especially useful if they overrode __hash__ or __eq__ in nonconventional ways.
+cv_type_checking: ContextVar = ContextVar(False, name='type_checking')
 
 def ensure_isa(obj, t, sampler=None):
     """Ensure 'obj' is of type 't'. Otherwise, throws a TypeError
     """
-    t = type_caster.to_canon(t)
-    t.validate_instance(obj, sampler)
+    with cv_type_checking(True):
+        t = type_caster.to_canon(t)
+        t.validate_instance(obj, sampler)
 
 
 def is_subtype(t1, t2):
     """Test if t1 is a subtype of t2
     """
 
-    t1 = type_caster.to_canon(t1)
-    t2 = type_caster.to_canon(t2)
-    return t1 <= t2
+    ct1 = type_caster.to_canon(t1)
+    ct2 = type_caster.to_canon(t2)
+    return ct1 <= ct2
 
 
 def isa(obj, t):
     """Tests if 'obj' is of type 't'
 
     Behaves like Python's isinstance, but supports the ``typing`` module and constraints.
     """
     try:
         ensure_isa(obj, t)
         return True
-    except TypeMismatchError as e:
+    except TypeMismatchError:
         return False
 
 
 def assert_isa(obj, t):
     """Ensure 'obj' is of type 't'. Otherwise, throws a TypeError
 
     Does nothing if Python is run with -O. (like the assert statement)
```

### Comparing `runtype-0.3.1/setup.py` & `runtype-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 packages = \
 ['runtype']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{':python_version >= "3.6" and python_version < "3.7"': ['dataclasses']}
+{':python_version >= "3.6" and python_version < "3.7"': ['dataclasses',
+                                                         'contextvars']}
 
 setup_kwargs = {
     'name': 'runtype',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Type dispatch and validation for run-time Python',
     'long_description': '![alt text](logo.png "Logo")\n\n\nRuntype is a collection of run-time type utilities for Python.\n\nIt is:\n\n:runner: Fast! Uses an internal typesystem for maximum performance.\n\n:brain: Smart! Supports `typing`, forward-references, constraints, auto-casting, and more.\n\n:gear: Configurative! Write your own type system, and use it with *dataclass* and *dispatch*.\n\n------\n\n### Modules\n\n- :star: [**validation**](https://runtype.readthedocs.io/en/latest/validation.html) - Provides a smarter alternative to `isinstance` and `issubclass`, with support for the `typing` module, and type constraints.\n\n- :star: [**dataclass**](https://runtype.readthedocs.io/en/latest/dataclass.html) - Adds run-time type validation to the built-in dataclass.\n\n    - Improves dataclass ergonomics.\n    - Supports most mypy constructs, like `typing` and forward-references (`foo: \'Bar\'`).\n    - Supports automatic value casting, Pydantic-style. (Optional, off by default)\n    - Supports types with constraints. (e.g. `String(max_length=10)`)\n    - Supports optional sampling for faster validation of big lists and dicts.\n    - Twice faster than Pydantic ([read here](https://runtype.readthedocs.io/en/latest/dataclass.html#compared-to-pydantic))\n\n- :star: [**dispatch**](https://runtype.readthedocs.io/en/latest/dispatch.html) - Provides fast multiple-dispatch for functions and methods, via a decorator.\n\n    - Inspired by Julia.\n\n- :star: [**type utilities**](https://runtype.readthedocs.io/en/latest/types.html) - Provides a set of classes to implement your own type-system.\n\n    - Used by runtype itself, to emulate the Python type-system.\n\n\n## Docs\n\nRead the docs here: https://runtype.readthedocs.io/\n\n## Install\n\n```bash\npip install runtype\n```\n\nNo dependencies.\n\nRequires Python 3.6 or up.\n\n[![Build Status](https://travis-ci.org/erezsh/runtype.svg?branch=master)](https://travis-ci.org/erezsh/runtype)\n[![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)\n\n## Examples\n\n### Validation (Isa & Subclass)\n\n```python\nfrom typing import Dict, Mapping\nfrom runtype import isa, issubclass\n\nprint( isa({\'a\': 1}, Dict[str, int]) )\n#> True\nprint( isa({\'a\': \'b\'}, Dict[str, int]) )\n#> False\n\nprint( issubclass(Dict[str, int], Mapping[str, int]) )\n#> True\nprint( issubclass(Dict[str, int], Mapping[int, str]) )\n#> False\n```\n\n### Dataclasses\n\n```python\nfrom typing import List\nfrom datetime import datetime\nfrom runtype import dataclass\n\n@dataclass(check_types=\'cast\')  # Cast values to the target type, when applicable\nclass Person:\n    name: str\n    birthday: datetime = None   # Optional\n    interests: List[str] = []   # The list is copied for each instance\n\n\nprint( Person("Beetlejuice") )\n#> Person(name=\'Beetlejuice\', birthday=None, interests=[])\nprint( Person("Albert", "1955-04-18T00:00", [\'physics\']) )\n#> Person(name=\'Albert\', birthday=datetime.datetime(1955, 4, 18, 0, 0), interests=[\'physics\'])\nprint( Person("Bad", interests=[\'a\', 1]) )\n# Traceback (most recent call last):\n#   ...\n# TypeError: [Person] Attribute \'interests\' expected value of type list[str]. Instead got [\'a\', 1]\n\n#     Failed on item: 1, expected type str\n\n```\n\n### Multiple Dispatch\n\n```python\nfrom runtype import Dispatch\ndp = Dispatch()\n\n@dp\ndef append(a: list, b):\n    return a + [b]\n\n@dp\ndef append(a: tuple, b):\n    return a + (b,)\n\n@dp\ndef append(a: str, b: str):\n    return a + b\n\n\nprint( append([1, 2, 3], 4) )\n#> [1, 2, 3, 4]\nprint( append((1, 2, 3), 4) )\n#> (1, 2, 3, 4)\nprint( append(\'foo\', \'bar\') )\n#> foobar\nprint( append(\'foo\', 4)     )\n# Traceback (most recent call last):\n#    ...\n# runtype.dispatch.DispatchError: Function \'append\' not found for signature (<class \'str\'>, <class \'int\'>)\n```\n\n\n## License\n\nRuntype uses the [MIT license](LICENSE).\n\n## Donate\n\nIf you like Runtype and want to show your appreciation, you can do so at my [patreon page](https://www.patreon.com/erezsh), or [ko-fi page](https://ko-fi.com/erezsh).\n',
     'author': 'Erez Shinan',
     'author_email': 'erezshin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/erezsh/runtype',
```

### Comparing `runtype-0.3.1/PKG-INFO` & `runtype-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtype
-Version: 0.3.1
+Version: 0.3.2
 Summary: Type dispatch and validation for run-time Python
 Home-page: https://github.com/erezsh/runtype
 License: MIT
 Keywords: types,typing,dispatch,multimethods,dataclass,runtime
 Author: Erez Shinan
 Author-email: erezshin@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
+Requires-Dist: contextvars; python_version >= "3.6" and python_version < "3.7"
 Requires-Dist: dataclasses; python_version >= "3.6" and python_version < "3.7"
 Project-URL: Repository, https://github.com/erezsh/runtype
 Description-Content-Type: text/markdown
 
 ![alt text](logo.png "Logo")
```

