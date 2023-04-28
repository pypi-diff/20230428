# Comparing `tmp/scrape_schema-0.0.9.tar.gz` & `tmp/scrape_schema-0.1.0.tar.gz`

## Comparing `scrape_schema-0.0.9.tar` & `scrape_schema-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/__init__.py
--rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/LICENSE
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/README.md
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    21663 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/README.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 scrape_schema-0.1.0/PKG-INFO
```

### Comparing `scrape_schema-0.0.9/scrape_schema/base.py` & `scrape_schema-0.1.0/scrape_schema/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from __future__ import annotations
-
 import logging
+import sys
 import warnings
 from abc import ABC, abstractmethod
-from types import NoneType
 from typing import (
     Any,
     ByteString,
     Callable,
     ClassVar,
+    Dict,
     Iterable,
+    List,
     Optional,
+    Tuple,
     Type,
-    TypeAlias,
     TypeVar,
     Union,
-    get_args,
-    get_origin,
-    get_type_hints,
 )
 
-# python < 3.9
-try:
-    from typing import Annotated  # type: ignore
-except ImportError:
-    from typing_extensions import Annotated  # type: ignore
-
-# python < 3.11
-try:
-    from typing import Self  # type: ignore
-except ImportError:
-    from typing_extensions import Self  # type: ignore
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+else:
+    from typing_extensions import Annotated
+
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias, get_args, get_origin, get_type_hints
+else:
+    from typing_extensions import TypeAlias, get_args, get_origin, get_type_hints
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
 from scrape_schema.exceptions import MarkupNotFoundError, ParseFailAttemptsError
 
+NoneType = type(None)
+
 logger = logging.getLogger("scrape_schema")
 logger.setLevel(logging.DEBUG)
 _formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(message)s")
 _stdout_handler = logging.StreamHandler()
 _stdout_handler.setFormatter(_formatter)
 logger.addHandler(_stdout_handler)
 
 T = TypeVar("T")
-MARKUP_TYPE: TypeAlias = str | Any
+MARKUP_TYPE: TypeAlias = Union[str, Any]
 
 
 class ABCField(ABC):
     @abstractmethod
     def _parse(self, markup: MARKUP_TYPE) -> Any:
         ...
 
@@ -59,15 +61,15 @@
         ...
 
     @abstractmethod
     def _callback(self, value: T) -> T:
         ...
 
     @abstractmethod
-    def _typing(self, instance: BaseSchema, name: str, value: T) -> T:
+    def _typing(self, instance: "BaseSchema", name: str, value: T) -> T:
         ...
 
 
 class TypeCaster:
     @staticmethod
     def _is_iterable_and_not_string_type(value_type: Type) -> bool:
         return issubclass(value_type, Iterable) and not issubclass(
@@ -76,110 +78,104 @@
 
     @staticmethod
     def _is_iterable_and_not_string_value(value: T) -> bool:
         return isinstance(value, Iterable) and not (
             isinstance(value, (ByteString, str))
         )
 
-    def _cast_type(self, type_annotation: Type, value: Any) -> Any:
-        value_type = type(value)
-        type_origin = get_origin(type_annotation)
-        type_args = get_args(type_annotation)
+    def _typing_to_builtin(self, type_hint: Type) -> Type:
+        origin = get_origin(type_hint)
+        args = get_args(type_hint)
+
+        if origin is not None and args:
+            # Recursively convert the nested generic types
+            converted_args = tuple(self._typing_to_builtin(arg) for arg in args)
+            return origin[converted_args]
+        else:
+            return type_hint
 
-        # skip if value type is annotated correct or is missing
-        if value_type is type_annotation:
-            logger.debug(
-                "`%s` value `%s` has same type, skip cast",
-                self.__class__.__name__,
-                value,
-            )
-            return value
+    def _cast_type(self, type_hint: Type, value: Any) -> Any:
+        if sys.version_info >= (3, 9):
+            type_hint = self._typing_to_builtin(type_hint)
 
-        logger.debug(
-            "`%s` Cast type start. `value[%s]=%s`, type_annotation=%s, `type_origin=%s`, `args=%s`",
+        origin = get_origin(type_hint)
+        args = get_args(type_hint)
+        logger.info(
+            "`%s` Cast type start. `value=%s`, type_annotation=%s, `origin=%s`, `args=%s`",
             self.__class__.__name__,
-            value_type.__name__,
             value,
-            type_annotation,
-            type_origin,
-            type_args,
+            type_hint,
+            origin,
+            args,
         )
+        # None
+        if value is None and type_hint is not bool:
+            return value
 
-        # Optional
-        if type_origin is Union and NoneType in type_args:
-            # get optional type, set
-            if value:
+        if origin is not None and args:
+            # list
+            if origin is list:
                 logger.debug(
-                    "`%s` Cast Optional type `%s(%s)`",
+                    "List cast %s -> arg=%s, value=%s",
                     self.__class__.__name__,
+                    args[0],
                     value,
-                    type_args[0],
                 )
-                if optional_args := get_args(type_args[0]):
-                    # Optional[list[T]]
-                    if isinstance(value, list):
-                        return [optional_args[0](v) for v in value]
-                    # Optional[dict[K, V]]
-                    elif isinstance(value, dict):
-                        k_type, v_type = optional_args
-                        return {k_type(k): v_type(v) for k, v in value.items()}
-                return type_args[0](value)
-            else:
+                return [self._cast_type(type_hint=args[0], value=v) for v in value]
+            # dict
+            elif origin is dict:
+                key_type, value_type = args
                 logger.debug(
-                    "`%s` Cast Optional type, value `%s` is False",
+                    "Dict cast %s -> key=%s, value=%s  `%s`",
                     self.__class__.__name__,
+                    key_type.__name__,
+                    value_type.__name__,
                     value,
                 )
-                return value
-
-        # dict, list
-        elif type_origin:
-            if issubclass(type_origin, dict) and isinstance(value, dict):
-                logger.debug(
-                    "`%s` Cast dict type: `%s(key)`, `%s(value)`",
-                    self.__class__.__name__,
-                    type_args[0],
-                    type_args[1],
-                )
-                # get dict set
-                return {type_args[0](k): type_args[1](v) for k, v in value.items()}
-
-            elif self._is_iterable_and_not_string_type(type_origin) and isinstance(
-                value, list
-            ):
-                logger.debug(
-                    "`%s` Cast list items to `%s(item)`",
-                    self.__class__.__name__,
-                    type_args[0],
-                )
-                # get list, set
-                return [type_args[0](i) for i in value]
-
+                return {
+                    self._cast_type(type_hint=key_type, value=k): self._cast_type(
+                        type_hint=value_type, value=v
+                    )
+                    for k, v in value.items()
+                }
+            # Optional
+            elif origin is Union:
+                if value is None and NoneType in args:
+                    logger.debug(
+                        "Optional cast %s -> %s", self.__class__.__name__, value
+                    )
+                    return None
+                # in python3.8 raise TypeError: issubclass() arg 1 must be a class
+                # example _cast_type(Optional[List[int]], [])
+                non_none_args = [arg for arg in args if arg is not NoneType]
+                if len(non_none_args) == 1:
+                    return self._cast_type(type_hint=non_none_args[0], value=value)
+        # bool cast
+        elif type_hint is bool:
+            logger.debug("Cast %s `%s()` -> bool", self.__class__.__name__, value)
+            return bool(value)
         else:
-            # single type
+            # direct cast
             logger.debug(
-                "Cast `%s` `%s(%s)`",
-                self.__class__.__name__,
-                type_annotation.__name__,
-                value,
+                "Cast `%s` := `%s(%s)`", self.__class__.__name__, type_hint, value
             )
-            return type_annotation(value)
+            return type_hint(value)
 
 
-class BaseConfigField:
+class BaseFieldConfig:
     """BaseField configuration class:
 
     * parser: Optional[Type[Any]] - parser backend object. If value None - work with python str
     """
 
     parser: ClassVar[Optional[Type[Any]]] = None
 
 
 class BaseField(ABCField, TypeCaster):
-    class Config(BaseConfigField):
+    class Config(BaseFieldConfig):
         pass
 
     def __init__(
         self,
         *,
         default: Optional[Any] = None,
         filter_: Optional[Callable[[T], bool]] = None,
@@ -231,80 +227,83 @@
                 f"not {type(markup).__name__}"
             )
         value = self._parse(markup)
         if not value:
             logger.debug(
                 "%s.extract value not found, set default `%s` value",
                 self.__class__.__name__,
-                self.default)
+                self.default,
+            )
             value = self.default
         if self._is_iterable_and_not_string_value(value):
             if self.filter_:
-                logger.debug(
-                    "%s.extract `filter_(%s)`", self.__class__.__name__, value)
+                logger.debug("%s.extract `filter_(%s)`", self.__class__.__name__, value)
             value = self._filter(value)
         if self.callback:
-            logger.debug(
-                "%s.extract `callback(%s)`", self.__class__.__name__, value)
+            logger.debug("%s.extract `callback(%s)`", self.__class__.__name__, value)
             value = self._callback(value)
         if self.factory:
-            logger.debug(
-                "%s.extract `factory(%s)`", self.__class__.__name__, value)
+            logger.debug("%s.extract `factory(%s)`", self.__class__.__name__, value)
             value = self._factory(value)
         elif type_:
             value = self._cast_type(type_, value)
-        logger.info("%s.extract return `%s[%s]`", self.__class__.__name__, value, type(value).__name__)
+        logger.info(
+            "%s.extract return `%s[%s]`",
+            self.__class__.__name__,
+            value,
+            type(value).__name__,
+        )
         return value
 
-    def __call__(self, instance: BaseSchema, name: str, markup: MARKUP_TYPE) -> Any:
+    def __call__(self, instance: "BaseSchema", name: str, markup: MARKUP_TYPE) -> Any:
         logger.info(
-            "`%s.%s[%s]`. Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
+            "%s.%s[%s]: Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
             instance.__class__.__name__,
             name,
             self.Config.parser or "str",
             repr(self.factory),
             repr(self.callback),
             repr(self.filter_),
             self.default,
         )
         value = self._parse(markup)
         if not value:
             logger.debug(
-                "`%s.%s` value not found, set default `%s` value",
+                "%s.%s: value not found, set default `%s` value",
                 instance.__class__.__name__,
                 name,
                 self.default,
             )
             value = self.default
         else:
             logger.debug(
-                "`%s.%s = %s` raw value(s)", instance.__class__.__name__, name, value
+                "%s.%s := %s raw value(s)", instance.__class__.__name__, name, value
             )
 
         if self._is_iterable_and_not_string_value(value):
             value = self._filter(value)
             if self.filter_:
                 logger.debug(
-                    "filter_ `%s.%s = %s`", instance.__class__.__name__, name, value
+                    "%s.%s := filter_(%s)", instance.__class__.__name__, name, value
                 )
 
         value = self._callback(value)
         if self.callback:
             logger.debug(
-                "callback `%s.%s = %s`", instance.__class__.__name__, name, value
+                "%s.%s := callback(%s)", instance.__class__.__name__, name, value
             )
 
         if self.factory:
             value = self._factory(value)
             logger.debug(
-                "factory `%s.%s = %s`", instance.__class__.__name__, name, value
+                "%s.%s := factory(%s)", instance.__class__.__name__, name, value
             )
         else:
             value = self._typing(instance, name, value)
-        logger.info(r"finish parse value %s.%s = %s")
+        logger.info("%s.%s = `%s` Done", instance.__class__.__name__, name, value)
         return value
 
     def _filter(self, value: T) -> Any:
         """filter parsed value by filter_ function, if it passed
 
         :param value: list or dict value. dict filter by values
         :return: filtered value
@@ -336,24 +335,24 @@
             return self.callback(value)
         if isinstance(value, list):
             return [self.callback(i) for i in value]
         elif isinstance(value, dict):
             return {k: self.callback(v) for k, v in value}
         return self.callback(value)
 
-    def _typing(self, instance: BaseSchema, name: str, value: T) -> Any:
+    def _typing(self, instance: "BaseSchema", name: str, value: T) -> Any:
         """auto type-cast method
 
         :param instance: BaseSchema instance
         :param name: field name
         :param value: field value
         :return: typed value
         """
         if instance.Config.type_cast:
-            if type_annotation := instance.__fields_annotations__.get(name):
+            if type_annotation := instance.__schema_annotations__.get(name):
                 value = self._cast_type(type_annotation, value)
         return value
 
 
 class BaseSchemaConfig:
     """Schema configuration for BaseSchema
 
@@ -367,190 +366,221 @@
 
     fails_attempt == 0  - if _first_ field return `default` value - throw `ParseFailAttemptsError`
 
     fails_attempt = n, fails_attempt > 0 - print *n* warnings messages if field return `default` value.
     if `n` msgs - throw `ParseFailAttemptsError`
     """
 
-    parsers_config: ClassVar[dict[Type[Any], dict[str, Any]]] = {}
+    parsers_config: ClassVar[Dict[Type[Any], Dict[str, Any]]] = {}
     type_cast: ClassVar[bool] = True
     fails_attempt: ClassVar[int] = -1
 
 
-class BaseSchema:
+class SchemaMetaClass(type):
+    @staticmethod
+    def _is_type_field(attr: Type) -> bool:
+        return get_origin(attr) is Annotated and all(
+            isinstance(arg, BaseField) for arg in get_args(attr)[1:]
+        )
+
+    @staticmethod
+    def _extract_annotated(attr: Type) -> Tuple[Type, Tuple[BaseField, ...]]:
+        args = get_args(attr)
+        return args[0], tuple(arg for arg in args[1:] if isinstance(arg, BaseField))
+
+    def __new__(mcs, name, bases, attrs):
+        __schema_fields__: Dict[str, Tuple[BaseField, ...]] = {}  # type: ignore
+        __schema_annotations__: Dict[str, Type] = {}  # type: ignore
+        cls_schema = super().__new__(mcs, name, bases, attrs)
+        if cls_schema.__name__ == "BaseSchema":
+            return cls_schema
+
+        # localns={} kwarg avoid TypeError 'function' object is not subscriptable
+        for name, value in get_type_hints(
+            cls_schema, localns={}, include_extras=True
+        ).items():
+            if name in ("__schema_fields__", "__schema_annotations__"):
+                continue
+            if mcs._is_type_field(value):
+                field_type, fields = mcs._extract_annotated(value)
+                __schema_fields__[name] = fields
+                __schema_annotations__[name] = field_type
+        setattr(cls_schema, "__schema_fields__", __schema_fields__)
+        setattr(cls_schema, "__schema_annotations__", __schema_annotations__)
+
+        return cls_schema
+
+
+class BaseSchema(metaclass=SchemaMetaClass):
+    __schema_fields__: Dict[str, Tuple[BaseField, ...]] = {}
+    __schema_annotations__: Dict[str, Type] = {}
+
     class Config(BaseSchemaConfig):
         pass
 
-    @staticmethod
-    def _is_annotated_field(attr: Type):
-        return get_origin(attr) is Annotated and isinstance(
-            get_args(attr)[-1], BaseField
-        )
+    def _get_parser(self, field_parser_class: Type) -> Optional[Dict[str, Any]]:
+        return self.Config.parsers_config.get(field_parser_class, None)
+
+    def _check_parser_config(self, field: BaseField, field_parser: Type) -> bool:
+        if self._get_parser(field_parser) is None:
+            try:
+                raise MarkupNotFoundError(
+                    f"{field.__class__.__name__} required "
+                    f"{field_parser.__class__.__name__} configuration"
+                )
+            except MarkupNotFoundError as e:
+                logger.exception(e)
+                raise e
+        return True
 
     @staticmethod
-    def _is_annotated_tuple_fields(attr: Type):
+    def _success_field_parse(field: BaseField, value) -> bool:
         return (
-            get_origin(attr) is Annotated
-            and isinstance(get_args(attr)[-1], tuple)
-            and all(isinstance(fld, BaseField) for fld in get_args(attr)[-1])
-        )
-
-    def _get_fields(self) -> dict[str, BaseField | tuple[BaseField, ...]]:
-        _fields: dict[str, BaseField | tuple[BaseField, ...]] = {}
-
-        for name, attr in get_type_hints(self.__class__, include_extras=True).items():
-            # get fields from Annotated[Type, Field(..) ]
-            if self._is_annotated_field(attr):
-                _type, _field = get_args(attr)
-                self.__fields_annotations__[name] = _type
-                _fields[name] = _field
-            # get field from Annotated[Type, (Field(..), Field(..), ...)]
-            elif self._is_annotated_tuple_fields(attr):
-                _type, _tuple_fields = get_args(attr)
-                self.__fields_annotations__[name] = _type
-                _fields[name] = _tuple_fields
-
-        # get non-typed fields
-        for name, attr in self.__class__.__dict__.items():
-            if not name.startswith("__") and isinstance(attr, BaseField):
-                _fields[name] = attr
-        return _fields
+            hasattr(field, "default")
+            and value != field.default
+            or value == field.default
+            or not value
+        )
+
+    def _cache_parser(
+        self,
+        *,
+        markup: str,
+        field_parser: Type[Any],
+        cached_parsers: Dict[Type[Any], Any],
+    ) -> Dict[Type[Any], Any]:
+        if not cached_parsers.get(field_parser):
+            parser_kwargs = self.Config.parsers_config.get(field_parser)
+            cached_parsers[field_parser] = field_parser(markup, **parser_kwargs)
+        return cached_parsers
 
     def _parse_field_value(
         self,
-        cached_parsers: dict[Type[Any], Any],
+        cached_parsers: Dict[Type[Any], Any],
         name: str,
-        fields: BaseField | tuple[BaseField, ...],
+        _fields: Tuple[BaseField, ...],
         markup: str,
-    ) -> Any:
+    ) -> Tuple[BaseField, Any]:
         value: Any = None
-        if not isinstance(fields, tuple):
-            fields = (fields,)
-
-        for field in fields:
-            field_parser = field.Config.parser
-            # parser is not defined in field.Config.parser
-            if not field_parser:
+        for field in _fields:
+            if field_parser := field.Config.parser:
+                self._check_parser_config(field=field, field_parser=field_parser)
+                cached_parsers = self._cache_parser(
+                    markup=markup,
+                    field_parser=field_parser,
+                    cached_parsers=cached_parsers,
+                )
+                value = field(self, name, cached_parsers[field_parser])
+            else:
                 value = field(self, name, markup)
+            # get next field if this return default value
+            if self._success_field_parse(field, value):
+                continue
+            else:
+                return field, value
+        return _fields[-1], value
 
-            elif self.Config.parsers_config.get(field_parser, None) is None:
-                try:
-                    raise MarkupNotFoundError(
-                        f"{field.__class__.__name__} required "
-                        f"{field_parser.__class__.__name__} configuration"
-                    )
-                except MarkupNotFoundError as e:
-                    logger.exception(e)
-                    raise e
+    def _is_attempt_fail(self, field: BaseField, value: Any) -> bool:
+        return (
+            self.Config.fails_attempt >= 0
+            and hasattr(field, "default")
+            and value == field.default
+        )
 
-            else:
-                # cache markup parser like BeautifulSoup, HTMLParser, and thing instances
-                if not cached_parsers.get(field_parser):
-                    parser_kwargs = self.Config.parsers_config.get(field_parser)
-                    cached_parsers[field_parser] = field_parser(markup, **parser_kwargs)
+    def _calculate_attempt_parse_errors(
+        self,
+        *,
+        fails_counter: int,
+        field: BaseField,
+        attr_name: str,
+        value: Any,
+    ) -> int:
+        # calculate fails - compare by default value
+        if self._is_attempt_fail(field, value):
+            fails_counter += 1
+            warnings.warn(
+                f"[{fails_counter}] Failed parse `{self.__class__.__name__}.{attr_name}` "
+                f"by {field.__class__.__name__} field, set `{value}`.",
+                stacklevel=2,
+                category=RuntimeWarning,
+            )
 
-                value = field(self, name, cached_parsers[field_parser])
+            logger.warning(
+                "[%i] Failed parse `%s.%s` by `%s`, set `%s`",
+                fails_counter,
+                self.__class__.__name__,
+                attr_name,
+                field.__class__.__name__,
+                value,
+            )
 
-            if (
-                hasattr(field, "default")
-                and value != field.default
-                or value == field.default
-                or not value
-            ):
-                continue
-            else:
-                return value
-        return value
+            if fails_counter > self.Config.fails_attempt:
+                raise ParseFailAttemptsError(
+                    f"{fails_counter} of {len(self.__schema_fields__.keys())} "
+                    "fields failed parse."
+                )
+        logger.debug(
+            "`%s.%s[%s] = %s`",
+            self.__class__.__name__,
+            attr_name,
+            field.__class__.__name__,
+            value,
+        )
+        return fails_counter
 
-    def _parse_markup_to_fields(self, markup: str) -> None:
+    def __init_fields__(self, markup: str) -> None:
         """
         :param str markup: text target
         """
-        self.__fields_annotations__: dict[str, Type] = {}
-
-        _fields = self._get_fields()
-        _parsers: dict[Type[Any], Any] = {}
+        _parsers: Dict[Type[Any], Any] = {}
         _fails_counter = 0
         logger.info(
             "Start parse `%s`. Fields count: %i",
             self.__class__.__name__,
-            len(_fields.keys()),
+            len(self.__schema_fields__.keys()),
         )
 
-        for name, field in _fields.items():
-            value = self._parse_field_value(
-                cached_parsers=_parsers, name=name, fields=field, markup=markup
-            )
-
-            # calculate fails - compare by default value
-            if (
-                self.Config.fails_attempt >= 0
-                and hasattr(field, "default")
-                and value == field.default
-            ):
-                _fails_counter += 1
-                warnings.warn(
-                    f"[{_fails_counter}] Failed parse `{self.__class__.__name__}.{name}` "
-                    f"by {field.__class__.__name__} field, set `{value}`.",
-                    stacklevel=2,
-                    category=RuntimeWarning,
-                )
-
-                logger.warning(
-                    "[%i] Failed parse `%s.%s` by `%s`, set `%s`",
-                    _fails_counter,
-                    self.__class__.__name__,
-                    name,
-                    field.__class__.__name__,
-                    value,
-                )
-
-                if _fails_counter > self.Config.fails_attempt:
-                    raise ParseFailAttemptsError(
-                        f"{_fails_counter} of {len(_fields.keys())} "
-                        "fields failed parse."
-                    )
-            logger.debug(
-                "`%s.%s[%s] = %s`",
-                self.__class__.__name__,
-                name,
-                field.__class__.__name__,
-                value,
+        for name, fields in self.__schema_fields__.items():
+            field, value = self._parse_field_value(
+                cached_parsers=_parsers, name=name, _fields=fields, markup=markup
+            )
+            _fails_counter = self._calculate_attempt_parse_errors(
+                fails_counter=_fails_counter, field=field, attr_name=name, value=value
             )
             setattr(self, name, value)
         logger.debug(
             "%s done! Fields fails: %i", self.__class__.__name__, _fails_counter
         )
 
     def __init__(self, markup: str, *, parse_markup: bool = True, **kwargs):
         """
         :param markup: markup string target
         :param parse_markup: parse field markups. Default True
         :param kwargs: any kwargs attrs
         """
         # TODO rewrite init constructor
         if parse_markup:
-            self._parse_markup_to_fields(markup)
+            self.__init_fields__(markup)
 
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     @classmethod
-    def from_list(cls, markups: Iterable[str], **kwargs) -> list[Self]:
+    def from_list(cls, markups: Iterable[str], **kwargs) -> List[Self]:
         """Init list of schemas by markups sequence
 
         :param markups: iterable markups sequence
         :param kwargs: any attrs
         """
         return [cls(markup, parse_markup=True, **kwargs) for markup in markups]
 
     @classmethod
     def from_crop_rule_list(
         cls, markup: str, *, crop_rule: Callable[[str], Iterable[str]], **kwargs
-    ) -> list[Self]:
+    ) -> List[Self]:
         """Init list of schemas by crop_rule
 
         :param markup: markup string
         :param crop_rule: crop rule function to *parts*
         """
         return cls.from_list(crop_rule(markup), **kwargs)
 
@@ -577,36 +607,36 @@
         """
         if kwargs.get("parse_markup"):
             kwargs.pop("parse_markup")
 
         return cls("", parse_markup=False, **kwargs)
 
     @staticmethod
-    def _to_dict(value: BaseSchema | list | dict):
+    def _to_dict(value: Union["BaseSchema", list, Dict]):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
                 return [val.dict() for val in value]
 
         elif isinstance(value, dict):
             if all(isinstance(val, BaseSchema) for val in value.values()):
                 return {k: v.dict() for k, v in value.items()}
         return value
 
-    def dict(self) -> dict[str, Any]:
+    def dict(self) -> Dict[str, Any]:
         """convert schema object to python dict"""
         return {
             k: self._to_dict(v)
             for k, v in self.__dict__.items()
             if not k.startswith("_") and k != "Config"
         }
 
-    def __repr_args__(self) -> list[str]:
+    def __repr_args__(self) -> List[str]:
         return [
             f"{k}={repr(v)}"
             if isinstance(v, BaseSchema)
             else f"{k}:{type(v).__name__}={repr(v)}"
             for k, v in self.__dict__.items()
             if not k.startswith("_") and k != "Config"
         ]
```

### Comparing `scrape_schema-0.0.9/scrape_schema/callbacks/slax.py` & `scrape_schema-0.1.0/scrape_schema/callbacks/slax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Build-in callbacks for fields.slax
 
 """
-from typing import Any, Callable, Optional
+from typing import Any, Callable, List, Optional, Union
 
 from selectolax.parser import HTMLParser, Node
 
 __all__ = ["crop_by_slax", "crop_by_slax_all", "get_attr", "get_text", "replace_text"]
 
 
 def crop_by_slax(query: str, **slax_config) -> Callable[[str], str]:
@@ -18,38 +18,38 @@
     def wrapper(markup: str) -> str:
         parser = HTMLParser(markup, **slax_config)
         return parser.css_first(query).html
 
     return wrapper
 
 
-def crop_by_slax_all(query: str, **slax_config) -> Callable[[str], list[str]]:
+def crop_by_slax_all(query: str, **slax_config) -> Callable[[str], List[str]]:
     """crop markup document to string chunks by selectolax selector
 
     :param query: css path
     :param slax_config: any selectolax.parser.HTMLParser kwargs
     """
 
-    def wrapper(markup: str) -> list[str]:
+    def wrapper(markup: str) -> List[str]:
         parser = HTMLParser(markup, **slax_config)
         return [m.html for m in parser.css(query)]
 
     return wrapper
 
 
 def get_attr(
     name: str, default: Optional[Any] = None
-) -> Callable[[Node | Any], str | Any]:
+) -> Callable[[Union[Node, Any]], Union[str, Any]]:
     """get attribute from Node object
 
     :param name: tag name
     :param default: default value, if tag is not founded. default None
     """
 
-    def wrapper(node: Node | Any) -> str:
+    def wrapper(node: Union[Node, Any]) -> str:
         if isinstance(node, Node):
             return node.attrs.get(name, default=default)
         return node
 
     return wrapper
 
 
@@ -57,45 +57,45 @@
     old: str,
     new: str,
     count: int = -1,
     *,
     deep: bool = True,
     separator: str = "",
     strip: bool = False,
-) -> Callable[[Node | Any], str | Any]:
+) -> Callable[[Union[Node, Any]], Union[str, Any]]:
     """replace text in Node element
 
     :param old: replace text target
     :param new: new text
     :param count: Maximum number of occurrences to replace. -1 (the default value) means replace all occurrences.
     :param deep: If True, includes text from all child nodes. Default True
     :param separator: The separator to use when joining text from different nodes. Default ''
     :param strip: If true, calls str.strip() on each text part to remove extra white spaces. default False
     :return:
     """
 
-    def wrapper(element: Node | Any) -> str | Node:
+    def wrapper(element: Union[Node, Any]) -> Union[str, Node]:
         if isinstance(element, Node):
             return element.text(deep=deep, separator=separator, strip=strip).replace(
                 old, new, count
             )
         return element
 
     return wrapper
 
 
 def get_text(
     deep: bool = True, separator: str = "", strip: bool = False
-) -> Callable[[Node | Any], str | Any]:
+) -> Callable[[Union[Node, Any]], Union[str, Any]]:
     """get text from Node object
 
     :param deep: If True, includes text from all child nodes.
     :param separator: The separator to use when joining text from different nodes.
     :param strip: If true, calls str.strip() on each text part to remove extra white spaces.
     """
 
-    def wrapper(element: Node | Any) -> str | Any:
+    def wrapper(element: Union[Node, Any]) -> Union[str, Any]:
         if isinstance(element, Node):
             return element.text(deep=deep, separator=separator, strip=strip)
         return element
 
     return wrapper
```

### Comparing `scrape_schema-0.0.9/scrape_schema/callbacks/soup.py` & `scrape_schema-0.1.0/scrape_schema/callbacks/soup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """build-in callbacks for fields.soup"""
-from __future__ import annotations
 import re
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from bs4 import BeautifulSoup, Tag
 
 RE_TAG_NAME = re.compile(r"<(\w+)")
 RE_TAG_ATTRS = re.compile(r'(?P<name>[\w_\-:.]+)="(?P<value>[\w_\-:.]+)"')
 
 __all__ = [
@@ -18,26 +17,28 @@
     "crop_by_selector_all",
     "element_to_dict",
 ]
 
 
 def replace_text(
     old: str, new: str, count: int = -1, *, separator: str = "", strip: bool = False
-) -> Callable[[Tag | Any], str | Any]:
-    def wrapper(tag: Tag | Any) -> str | Any:
+) -> Callable[[Union[Tag, Any]], Union[str, Any]]:
+    def wrapper(tag: Union[Tag, Any]) -> Union[str, Any]:
         if isinstance(tag, Tag):
             return tag.get_text(separator=separator, strip=strip).replace(
                 old, new, count
             )
         return tag
 
     return wrapper
 
 
-def element_to_dict(element: str) -> dict[str, str | dict[str, str | list[str]]]:
+def element_to_dict(
+    element: str,
+) -> Dict[str, Union[str, Dict[str, Union[Union[str, List[str]]]]]]:
     """Convert string element to dict
 
     Example:
         <p> -> {"name": "p", "attrs":{}}
         <a id="1", class="thing"> -> {"name": "a", "attrs": {"id": "1", "class": "thing"}}
     """
     if not (match := RE_TAG_NAME.search(element)):
@@ -47,69 +48,71 @@
     if (klass := attrs.get("class")) and len(klass.split(" ")) != 1:
         attrs["class"] = klass.split(" ")
     return {"name": tag_name, "attrs": attrs}
 
 
 def get_text(
     separator: str = "", strip: bool = False
-) -> Callable[[Tag | Any], str | Any]:
+) -> Callable[[Union[Tag, Any]], Union[str, Any]]:
     """get text from bs4.Tag
 
     :param separator: separator. default ""
     :param strip: strip flag. default False
     :return:
     """
 
-    def wrapper(tag: Tag | Any) -> str | Any:
+    def wrapper(tag: Union[Tag, Any]) -> Union[str, Any]:
         if isinstance(tag, Tag):
             return tag.get_text(separator=separator, strip=strip)
         return tag
 
     return wrapper
 
 
-def get_attr(tag_name: str, default: Any = ...) -> Callable[[Tag | Any], str | Any]:
+def get_attr(
+    tag_name: str, default: Any = ...
+) -> Callable[[Union[Tag, Any]], Union[str, Any]]:
     """get tag from element
 
     :param tag_name: tag name
     :param default: default value, if attr not founded
     :return:
     """
 
-    def wrapper(tag: Tag | Any) -> str | Any:
+    def wrapper(tag: Union[Tag, Any]) -> Union[str, Any]:
         if isinstance(tag, Tag):
             if default == Ellipsis:
                 return tag.get(tag_name)
             return tag.get(tag_name, default=default)
         return tag
 
     return wrapper
 
 
 def crop_by_tag_all(
-    element: str | dict[str, Any], features: str = "html.parser", **soup_config
-) -> Callable[[str], list[str]]:
+    element: Union[str, Dict[str, Any]], features: str = "html.parser", **soup_config
+) -> Callable[[str], List[str]]:
     """crop markup document to string chunks by soup element
 
     :param element: html element or any dict of kwargs for soup.find_all method
     :param features: BeautifulSoup parser. default `html.parser`
     :param soup_config: any BeautifulSoup kwargs config
     """
     if isinstance(element, str):
         element = element_to_dict(element)
 
-    def wrapper(markup: str) -> list[str]:
+    def wrapper(markup: str) -> List[str]:
         soup = BeautifulSoup(markup, features=features, **soup_config)
         return [str(tag) for tag in soup.find_all(**element)]
 
     return wrapper
 
 
 def crop_by_tag(
-    element: str | dict[str, Any], features: str = "html.parser", **soup_config
+    element: Union[str, Dict[str, Any]], features: str = "html.parser", **soup_config
 ) -> Callable[[str], str]:
     """crop markup document to string chunk by soup element
 
     :param element: html element or any dict of kwargs for soup.find method
     :param features: BeautifulSoup parser. default `html.parser`
     :param soup_config: any BeautifulSoup kwargs config
     """
@@ -121,15 +124,15 @@
         return str(soup.find_all(**element))
 
     return wrapper
 
 
 def crop_by_selector(
     selector: str,
-    namespaces: Optional[dict[str, Any]] = None,
+    namespaces: Optional[Dict[str, Any]] = None,
     features: str = "html.parser",
     **soup_config,
 ) -> Callable[[str], str]:
     """crop markup document to string chunk by soup selector
 
     :param selector: css selector for soup.select_one method
     :param namespaces: A dictionary mapping namespace prefixes used
@@ -144,26 +147,26 @@
         return str(soup.select_one(selector, namespaces))
 
     return wrapper
 
 
 def crop_by_selector_all(
     selector: str,
-    namespaces: Optional[dict[str, Any]] = None,
+    namespaces: Optional[Dict[str, Any]] = None,
     features: str = "html.parser",
     **soup_config,
-) -> Callable[[str], list[str]]:
+) -> Callable[[str], List[str]]:
     """crop markup document to string chunks by soup selector
 
     :param selector: css selector for soup.select method
     :param namespaces: A dictionary mapping namespace prefixes used
     in the CSS selector to namespace URIs. By default,
     Beautiful Soup will use the prefixes it encountered while parsing the document.
     :param features: BeautifulSoup parser. default `html.parser`
     :param soup_config: any BeautifulSoup kwargs config
     """
 
-    def wrapper(markup: str) -> list[str]:
+    def wrapper(markup: str) -> List[str]:
         soup = BeautifulSoup(markup, features=features, **soup_config)
         return [str(tag) for tag in soup.select(selector, namespaces)]
 
     return wrapper
```

### Comparing `scrape_schema-0.0.9/scrape_schema/fields/nested.py` & `scrape_schema-0.1.0/scrape_schema/fields/nested.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Nested fields for create BaseSchema objects"""
+from typing import Any, Callable, List, Optional, Type, Union
 
-from typing import Any, Callable, Optional, Type
-
-from ..base import BaseField, BaseSchema
+from ..base import BaseField, BaseSchema  # type: ignore
 
 __all__ = ["BaseNested", "Nested", "NestedList"]
 
 
 class BaseNested(BaseField):
     def _parse(self, _: str) -> str:
         return _
@@ -28,38 +27,38 @@
         """
         super().__init__(factory=factory)
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
-    ) -> BaseSchema | Any:
+    ) -> Union[BaseSchema, Any]:
         markup = self._parse(markup)
         value = self._schema.from_crop_rule(markup, crop_rule=self.crop_rule)
         return self._factory(value)
 
 
 class NestedList(BaseNested):
     def __init__(
         self,
         schema: Type[BaseSchema],
         *,
-        crop_rule: Callable[[str], list[str]],
-        factory: Optional[Callable[[list[BaseSchema]], Any]] = None,
+        crop_rule: Callable[[str], List[str]],
+        factory: Optional[Callable[[List[BaseSchema]], Any]] = None,
     ):
         """NestedList - convert markup parts to list of `schema` objects
 
         :param schema: BaseSchema type
         :param crop_rule: function for crop markup to parts
         :param factory: function for convert to another type. Default convert to `schema`
         """
         super().__init__(factory=factory)
         self.crop_rule = crop_rule
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
-    ) -> list[BaseSchema] | Any:
+    ) -> Union[List[BaseSchema], Any]:
         markup = self._parse(markup)
         value = self._schema.from_crop_rule_list(markup, crop_rule=self.crop_rule)
         return self._factory(value)
```

### Comparing `scrape_schema-0.0.9/scrape_schema/fields/regex.py` & `scrape_schema-0.1.0/scrape_schema/fields/regex.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,33 @@
 
 * https://docs.python.org/3.11/library/re.html#re.finditer
 
 **ReMatchDict, ReMatchListDict**
 
 * https://docs.python.org/3.11/library/re.html#re.Match.groupdict
 """
+
 import re
-from typing import Any, Callable, Optional, Pattern
+from typing import Any, Callable, Dict, List, Optional, Pattern, Union
 
 from ..base import BaseField
 
 __all__ = ["ReMatch", "ReMatchList", "ReMatchDict", "ReMatchListDict"]
 
 
 class ReMatch(BaseField):
     def __init__(
         self,
-        pattern: str | Pattern,
+        pattern: Union[str, Pattern],
         group: int = 1,
-        flags: int | re.RegexFlag = 0,
+        flags: Union[int, re.RegexFlag] = 0,
         *,
         default: Optional[Any] = None,
         callback: Optional[Callable[[str], Any]] = None,
-        factory: Optional[Callable[[str | Any], Any]] = None,
+        factory: Optional[Callable[[Union[str, Any]], Any]] = None,
     ):
         """get first match by `re.search`
 
         :param pattern: re.compile pattern or string
         :param group: match group. default 1
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
@@ -66,22 +67,22 @@
             return result.group(self.group)
         return None
 
 
 class ReMatchList(BaseField):
     def __init__(
         self,
-        pattern: str | Pattern,
+        pattern: Union[str, Pattern],
         group: int = 1,
-        flags: int | re.RegexFlag = 0,
+        flags: Union[int, re.RegexFlag] = 0,
         *,
         default: Optional[Any] = None,
         filter_: Optional[Callable[[str], bool]] = None,
         callback: Optional[Callable[[str], Any]] = None,
-        factory: Optional[Callable[[list[str] | Any], Any]] = None,
+        factory: Optional[Callable[[Union[List[str], Any]], Any]] = None,
     ):
         """get all matches by `re.finditer`
 
         :param pattern: re.compile pattern or string
         :param group: match group. default 1
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
@@ -93,29 +94,29 @@
             default=default, filter_=filter_, callback=callback, factory=factory
         )
         self.pattern = (
             re.compile(pattern, flags) if isinstance(pattern, str) else pattern
         )
         self.group = group
 
-    def _parse(self, markup: str) -> list[str]:
+    def _parse(self, markup: str) -> List[str]:
         if matches := self.pattern.finditer(markup):
             return [m.group(self.group) for m in matches]
         return []
 
 
 class ReMatchDict(BaseField):
     def __init__(
         self,
-        pattern: str | Pattern,
-        flags: int | re.RegexFlag = 0,
+        pattern: Union[str, Pattern],
+        flags: Union[int, re.RegexFlag] = 0,
         *,
         default: Optional[Any] = None,
-        callback: Optional[Callable[[dict[str, str]], Any]] = None,
-        factory: Optional[Callable[[dict[str, str] | Any], Any]] = None,
+        callback: Optional[Callable[[Dict[str, str]], Any]] = None,
+        factory: Optional[Callable[[Union[Dict[str, str], Any]], Any]] = None,
     ):
         """get first match by `re.search(...).groupdict()`. Pattern required named groups
 
         :param pattern: re.compile pattern or string. Pattern required named groups
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param callback: function eval result. default None
@@ -124,28 +125,28 @@
         super().__init__(default=default, callback=callback, factory=factory)
         self.pattern = (
             re.compile(pattern, flags) if isinstance(pattern, str) else pattern
         )
         if not self.pattern.groupindex:
             raise AttributeError(f"{pattern.pattern} required named groups")  # type: ignore
 
-    def _parse(self, markup: str) -> dict[str, str]:
+    def _parse(self, markup: str) -> Dict[str, str]:
         return result.groupdict() if (result := self.pattern.search(markup)) else {}
 
 
 class ReMatchListDict(BaseField):
     def __init__(
         self,
-        pattern: str | Pattern,
-        flags: int | re.RegexFlag = 0,
+        pattern: Union[str, Pattern],
+        flags: Union[int, re.RegexFlag] = 0,
         *,
         default: Optional[Any] = None,
-        filter_: Optional[Callable[[dict[str, str]], bool]] = None,
-        callback: Optional[Callable[[dict[str, str]], Any]] = None,
-        factory: Optional[Callable[[dict[str, str] | Any], Any]] = None,
+        filter_: Optional[Callable[[Dict[str, str]], bool]] = None,
+        callback: Optional[Callable[[Dict[str, str]], Any]] = None,
+        factory: Optional[Callable[[Union[Dict[str, str], Any]], Any]] = None,
     ):
         """get all matches by `re.finditer` and `re.search(...).groupdict()`. Pattern required named groups
 
         :param pattern: re.compile pattern or string. Pattern required named groups
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
@@ -157,11 +158,11 @@
         )
         self.pattern = (
             re.compile(pattern, flags) if isinstance(pattern, str) else pattern
         )
         if not self.pattern.groupindex:
             raise AttributeError(f"{pattern.pattern} required named groups")  # type: ignore
 
-    def _parse(self, markup: str) -> list[dict[str, str]]:
+    def _parse(self, markup: str) -> List[Dict[str, str]]:
         if results := self.pattern.finditer(markup):
             return [result.groupdict() for result in results]
         return []
```

### Comparing `scrape_schema-0.0.9/scrape_schema/fields/slax.py` & `scrape_schema-0.1.0/scrape_schema/fields/slax.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,39 +9,40 @@
 * https://selectolax.readthedocs.io/en/latest/parser.html#selectolax.parser.HTMLParser.css_first
 
 **SlaxSelectList**
 
 * https://selectolax.readthedocs.io/en/latest/parser.html#selectolax.parser.HTMLParser.css
 
 """
+
 from abc import ABC
-from typing import Any, Callable, Optional
+from typing import Any, Callable, List, Optional, Union
 
 from selectolax.parser import HTMLParser, Node
 
-from ..base import BaseConfigField, BaseField
+from ..base import BaseField, BaseFieldConfig
 from ..callbacks.slax import get_text
 
 __all__ = ["BaseSlax", "SlaxSelect", "SlaxSelectList"]
 
 
 class BaseSlax(BaseField, ABC):
-    class Config(BaseConfigField):
+    class Config(BaseFieldConfig):
         parser = HTMLParser
 
 
 class SlaxSelect(BaseSlax):
     def __init__(
         self,
         selector: str,
         strict: bool = False,
         *,
         default: Optional[Any] = None,
-        callback: Optional[Callable[[Node], str | Any]] = get_text(),
-        factory: Optional[Callable[[str | Any], Any]] = None,
+        callback: Optional[Callable[[Node], Union[str, Any]]] = get_text(),
+        factory: Optional[Callable[[Union[str, Any]], Any]] = None,
     ):
         """Get Node by HTMLParser(...).css_first
 
         :param selector: css selector
         :param strict: Check if there is strictly only one match in the document. Default False
         :param default: default value if match not founded. default None
         :param callback: function eval result. default get text from element
@@ -58,25 +59,25 @@
 class SlaxSelectList(BaseSlax):
     def __init__(
         self,
         selector: str,
         *,
         default: Optional[Any] = None,
         filter_: Optional[Callable[[Node], bool]] = None,
-        callback: Optional[Callable[[Node], str | Any]] = get_text(),
-        factory: Optional[Callable[[list[str | Any]], Any]] = None,
+        callback: Optional[Callable[[Node], Union[str, Any]]] = get_text(),
+        factory: Optional[Callable[[List[Union[str, Any]]], Any]] = None,
     ):
         """get all Nodes by HTMLParser(...).css
 
         :param selector: css selector
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(
             default=default, callback=callback, factory=factory, filter_=filter_
         )
         self.selector = selector
 
-    def _parse(self, markup: HTMLParser) -> list[Node]:
+    def _parse(self, markup: HTMLParser) -> List[Node]:
         return markup.css(self.selector)
```

### Comparing `scrape_schema-0.0.9/scrape_schema/fields/soup.py` & `scrape_schema-0.1.0/scrape_schema/fields/soup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,121 +21,122 @@
 * https://beautiful-soup-4.readthedocs.io/en/latest/#a-function
 
 
 **SoupSelect, SoupSelectList**
 
 * https://beautiful-soup-4.readthedocs.io/en/latest/#css-selectors
 """
+
 from abc import ABC
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from bs4 import BeautifulSoup, ResultSet, Tag
 
-from ..base import BaseConfigField, BaseField
+from ..base import BaseField, BaseFieldConfig
 from ..callbacks.soup import element_to_dict, get_text
 
 __all__ = ["BaseSoup", "SoupFind", "SoupFindList", "SoupSelect", "SoupSelectList"]
 
 
 class BaseSoup(BaseField, ABC):
-    class Config(BaseConfigField):
+    class Config(BaseFieldConfig):
         parser = BeautifulSoup
 
 
 class SoupFind(BaseSoup):
     def __init__(
         self,
-        element: str | dict[str, Any],
+        element: Union[str, Dict[str, Any]],
         *,
         default: Optional[Any] = None,
-        callback: Optional[Callable[[Tag], str | Any]] = get_text(),
-        factory: Optional[Callable[[str | Any], Any]] = None,
+        callback: Optional[Callable[[Tag], Union[str, Any]]] = get_text(),
+        factory: Optional[Callable[[Union[str, Any]], Any]] = None,
     ):
         """get Tag by BeautifulSoup(...).find method
 
         :param element: html tag or dict of keyword args for BeautifulSoup(...).find method
         :param default: default value if match not founded. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(default=default, callback=callback, factory=factory)
         self.element = element_to_dict(element) if isinstance(element, str) else element
 
-    def _parse(self, markup: BeautifulSoup | Tag) -> Optional[Tag]:
+    def _parse(self, markup: Union[BeautifulSoup, Tag]) -> Optional[Tag]:
         return markup.find(**self.element)
 
 
 class SoupFindList(BaseSoup):
     def __init__(
         self,
-        element: str | dict[str, Any],
+        element: Union[str, Dict[str, Any]],
         *,
         default: Optional[Any] = None,
         filter_: Optional[Callable[[Tag], bool]] = None,
-        callback: Optional[Callable[[Tag], str | Any]] = get_text(),
-        factory: Optional[Callable[[list[str | Any] | Any], Any]] = None,
+        callback: Optional[Callable[[Tag], Union[str, Any]]] = get_text(),
+        factory: Optional[Callable[[Union[List[Union[str, Any]], Any]], Any]] = None,
     ):
         """get Tags by BeautifulSoup(...).find_all method
 
         :param element: html tag or dict of keyword args for BeautifulSoup(...).find_all method
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(
             default=default, callback=callback, factory=factory, filter_=filter_
         )
         self.element = element_to_dict(element) if isinstance(element, str) else element
 
-    def _parse(self, markup: BeautifulSoup | Tag) -> ResultSet:
+    def _parse(self, markup: Union[BeautifulSoup, Tag]) -> ResultSet:
         return markup.find_all(**self.element)
 
 
 class SoupSelect(BaseSoup):
     def __init__(
         self,
         selector: str,
         *,
         default: Optional[Any] = None,
         callback: Optional[Callable[[Tag], Any]] = get_text(),
-        factory: Optional[Callable[[str | Any], Any]] = None,
+        factory: Optional[Callable[[Union[str, Any]], Any]] = None,
     ):
         """Get tag by BeautifulSoup(...).select_one method
 
         :param selector: css selector
         :param default: default value if match not founded. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(default=default, callback=callback, factory=factory)
         self.selector = selector
 
-    def _parse(self, markup: BeautifulSoup | Tag) -> Tag:
+    def _parse(self, markup: Union[BeautifulSoup, Tag]) -> Tag:
         return markup.select_one(self.selector)
 
 
 class SoupSelectList(BaseSoup):
     def __init__(
         self,
         selector: str,
         *,
         default: Optional[Any] = None,
         filter_: Optional[Callable[[Tag], bool]] = None,
         callback: Optional[Callable[[Tag], Any]] = get_text(),
-        factory: Optional[Callable[[list[str | Any]], Any]] = None,
+        factory: Optional[Callable[[List[Union[str, Any]]], Any]] = None,
     ):
         """Get tags by BeautifulSoup(...).select method
 
         :param selector: css selector
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(
             default=default, callback=callback, factory=factory, filter_=filter_
         )
         self.selector = selector
 
-    def _parse(self, markup: BeautifulSoup | Tag) -> ResultSet:
+    def _parse(self, markup: Union[BeautifulSoup, Tag]) -> ResultSet:
         return markup.select(self.selector)
```

### Comparing `scrape_schema-0.0.9/.gitignore` & `scrape_schema-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.9/LICENSE` & `scrape_schema-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.9/README.md` & `scrape_schema-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
+![CI](https://github.com/vypivshiy/scrape_schema/actions/workflows/ci.yml/badge.svg)
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for unstructured text data (like html, stdout or any text) and
 is inspired by dataclasses
 
 # Motivation
 Simplifying parsers support, where it is difficult to use 
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
+* python 3.8+ support
+* decrease lines of code for your parsers
 * partial support type-casting from annotations (str, int, float, bool, list, dict, Optional)
-* converting parsed values using callbacks, filters, factories
-* logging to quickly find problems in getting values
+* interacting with values with callbacks, filters, factories
+* logging to quickly find problems in extracted values
 * optional success-attempts parse values checker from fields objects
-* decrease code lines for your parsers
 * standardization, modularity* of structures-parsers
-
 *If you usage schema-structures and they are separated from the logic of getting the text
 (stdout output, HTTP requests, etc)
 ____
 # Build-in libraries parsers support:
 - [x] re
 - [x] bs4
 - [x] selectolax(Modest)
@@ -51,15 +52,70 @@
 ```
 
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
-# Example
+# Code comparison
+Before scrape_schema: harder to maintain, change logic
+```python
+import re
+import pprint
+
+TEXT = """
+banana potato BANANA POTATO
+-foo:10
+-bar:20
+lorem upsum dolor
+192.168.0.1
+"""
+
+
+def parse_text(text: str) -> dict:
+    if match := re.search(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})", text):
+        ipv4 = match[1]
+    else:
+        ipv4 = None
+
+    if matches := re.findall(r"(\d+)", text):
+        max_digit = max(int(i) for i in matches)
+    else:
+        max_digit = None
+
+    failed_value = bool(re.search(r"(ora)", text))
+
+    if matches := re.findall(r"(\d+)", text):
+        digits = [int(i) for i in matches]
+        digits_float = [float(f'{i}.5') for i in matches]
+    else:
+        digits = None
+        digits_float = None
+    words_lower = matches if (matches := re.findall(r"([a-z]+)", text)) else None
+    words_upper = matches if (matches := re.findall(r"([A-Z]+)", text)) else None
+
+    return dict(ipv4=ipv4, max_digit=max_digit, failed_value=failed_value,
+                digits=digits, digits_float=digits_float, 
+                words_lower=words_lower, words_upper=words_upper)
+    
+
+if __name__ == '__main__':
+    pprint.pprint(parse_text(TEXT), width=48, compact=True)
+    # {'digits': [10, 20, 192, 168, 0, 1],
+    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
+    #                   1.5],
+    #  'failed_value': False,
+    #  'ip_v4': '192.168.0.1',
+    #  'max_digit': 192,
+    #  'words_lower': ['banana', 'potato', 'foo',
+    #                  'bar', 'lorem', 'upsum',
+    #                  'dolor'],
+    #  'words_upper': ['BANANA', 'POTATO']}
+```
+After scrape_schema: easy change of logic, support, portability
 ```python
 from typing import Annotated
 import pprint
 
 from scrape_schema import BaseSchema
 from scrape_schema.fields.regex import ReMatch, ReMatchList
 
@@ -104,15 +160,15 @@
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
 ```python
 import logging
 
 logger = logging.getLogger("scrape_schema")
-logger.setLevel(logging.ERROR)
+logger.setLevel(logging.INFO)
 ...
 ```
 
 See more [examples](examples) and [documentation](https://scrape-schema.readthedocs.io/en/latest/) 
 for get more information/examples
 ____
 This project is licensed under the terms of the MIT license.
```

### Comparing `scrape_schema-0.0.9/pyproject.toml` & `scrape_schema-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,20 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.mypy]
+python_version = 3.8
 pretty = true
 ignore_missing_imports = true
 exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
 files = "scrape_schema/*.py,scrape_schema/fields/*.py,scrape_schema/callbacks/*.py"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
-    "ignore::RuntimeWarning",
-    # note the use of single quote below to denote "raw" strings in TOML
-    'ignore: Failed parse',
+    'ignore::RuntimeWarning',
 ]
```

### Comparing `scrape_schema-0.0.9/PKG-INFO` & `scrape_schema-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -39,35 +39,36 @@
 Requires-Dist: mkdocs-material; extra == 'docs'
 Provides-Extra: selectolax
 Requires-Dist: selectolax; extra == 'selectolax'
 Description-Content-Type: text/markdown
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
+![CI](https://github.com/vypivshiy/scrape_schema/actions/workflows/ci.yml/badge.svg)
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for unstructured text data (like html, stdout or any text) and
 is inspired by dataclasses
 
 # Motivation
 Simplifying parsers support, where it is difficult to use 
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
+* python 3.8+ support
+* decrease lines of code for your parsers
 * partial support type-casting from annotations (str, int, float, bool, list, dict, Optional)
-* converting parsed values using callbacks, filters, factories
-* logging to quickly find problems in getting values
+* interacting with values with callbacks, filters, factories
+* logging to quickly find problems in extracted values
 * optional success-attempts parse values checker from fields objects
-* decrease code lines for your parsers
 * standardization, modularity* of structures-parsers
-
 *If you usage schema-structures and they are separated from the logic of getting the text
 (stdout output, HTTP requests, etc)
 ____
 # Build-in libraries parsers support:
 - [x] re
 - [x] bs4
 - [x] selectolax(Modest)
@@ -94,15 +95,70 @@
 ```
 
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
-# Example
+# Code comparison
+Before scrape_schema: harder to maintain, change logic
+```python
+import re
+import pprint
+
+TEXT = """
+banana potato BANANA POTATO
+-foo:10
+-bar:20
+lorem upsum dolor
+192.168.0.1
+"""
+
+
+def parse_text(text: str) -> dict:
+    if match := re.search(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})", text):
+        ipv4 = match[1]
+    else:
+        ipv4 = None
+
+    if matches := re.findall(r"(\d+)", text):
+        max_digit = max(int(i) for i in matches)
+    else:
+        max_digit = None
+
+    failed_value = bool(re.search(r"(ora)", text))
+
+    if matches := re.findall(r"(\d+)", text):
+        digits = [int(i) for i in matches]
+        digits_float = [float(f'{i}.5') for i in matches]
+    else:
+        digits = None
+        digits_float = None
+    words_lower = matches if (matches := re.findall(r"([a-z]+)", text)) else None
+    words_upper = matches if (matches := re.findall(r"([A-Z]+)", text)) else None
+
+    return dict(ipv4=ipv4, max_digit=max_digit, failed_value=failed_value,
+                digits=digits, digits_float=digits_float, 
+                words_lower=words_lower, words_upper=words_upper)
+    
+
+if __name__ == '__main__':
+    pprint.pprint(parse_text(TEXT), width=48, compact=True)
+    # {'digits': [10, 20, 192, 168, 0, 1],
+    #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
+    #                   1.5],
+    #  'failed_value': False,
+    #  'ip_v4': '192.168.0.1',
+    #  'max_digit': 192,
+    #  'words_lower': ['banana', 'potato', 'foo',
+    #                  'bar', 'lorem', 'upsum',
+    #                  'dolor'],
+    #  'words_upper': ['BANANA', 'POTATO']}
+```
+After scrape_schema: easy change of logic, support, portability
 ```python
 from typing import Annotated
 import pprint
 
 from scrape_schema import BaseSchema
 from scrape_schema.fields.regex import ReMatch, ReMatchList
 
@@ -147,15 +203,15 @@
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
 ```python
 import logging
 
 logger = logging.getLogger("scrape_schema")
-logger.setLevel(logging.ERROR)
+logger.setLevel(logging.INFO)
 ...
 ```
 
 See more [examples](examples) and [documentation](https://scrape-schema.readthedocs.io/en/latest/) 
 for get more information/examples
 ____
 This project is licensed under the terms of the MIT license.
```

