# Comparing `tmp/polyfactory-2.0.0a1.tar.gz` & `tmp/polyfactory-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.0.0a1.tar", max compression
+gzip compressed data, was "polyfactory-2.0.1.tar", max compression
```

## Comparing `polyfactory-2.0.0a1.tar` & `polyfactory-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1092 2023-04-11 13:54:46.061917 polyfactory-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     4513 2023-04-11 13:54:46.061917 polyfactory-2.0.0a1/README.md
--rw-r--r--   0        0        0      425 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/__init__.py
--rw-r--r--   0        0        0      605 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/constants.py
--rw-r--r--   0        0        0      591 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    26088 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     1074 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     9542 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     1976 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     3311 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3633 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     5964 2023-04-11 13:54:46.065917 polyfactory-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     6538 1970-01-01 00:00:00.000000 polyfactory-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-28 01:42:41.001077 polyfactory-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8276 2023-04-28 01:42:41.001077 polyfactory-2.0.1/README.md
+-rw-r--r--   0        0        0      425 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/constants.py
+-rw-r--r--   0        0        0      591 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-04-28 01:42:41.001077 polyfactory-2.0.1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    30183 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2250 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     6275 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     2939 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     3311 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3633 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-04-28 01:42:41.005077 polyfactory-2.0.1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6030 2023-04-28 01:42:41.005077 polyfactory-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10299 1970-01-01 00:00:00.000000 polyfactory-2.0.1/PKG-INFO
```

### Comparing `polyfactory-2.0.0a1/LICENSE` & `polyfactory-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/constants.py` & `polyfactory-2.0.1/polyfactory/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,7 +25,9 @@
     Set: set,
     Tuple: tuple,
     abc.Iterable: list,
     abc.Mapping: dict,
     abc.Sequence: list,
     abc.Set: set,
 }
+
+IGNORED_TYPE_ARGS: Set = {Ellipsis}
```

### Comparing `polyfactory-2.0.0a1/polyfactory/exceptions.py` & `polyfactory-2.0.1/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/factories/base.py` & `polyfactory-2.0.1/polyfactory/factories/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,22 +47,30 @@
 from polyfactory.utils.predicates import (
     get_type_origin,
     is_literal,
     is_optional_union,
     is_safe_subclass,
 )
 from polyfactory.value_generators.complex_types import handle_complex_type
+from polyfactory.value_generators.constrained_collections import handle_constrained_collection
+from polyfactory.value_generators.constrained_dates import handle_constrained_date
+from polyfactory.value_generators.constrained_numbers import (
+    handle_constrained_float,
+    handle_constrained_int,
+    handle_constrained_decimal,
+)
+from polyfactory.value_generators.constrained_strings import handle_constrained_string_or_bytes
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
 )
 
 if TYPE_CHECKING:
     from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
-    from polyfactory.field_meta import FieldMeta
+    from polyfactory.field_meta import FieldMeta, Constraints
     from typing_extensions import TypeGuard
 
 
 def _create_pydantic_type_map(cls: "type[BaseFactory]") -> dict[type, Callable[[], Any]]:
     """Creates a mapping of pydantic types to mock data functions.
 
     :param cls: The base factory class.
@@ -167,15 +175,15 @@
     __random_seed__: ClassVar[int]
     """
     An integer to seed the factory's Faker and Random instances with.
     This attribute can be used to control random generation.
     """
 
     # cached attributes
-    _fields_metadata: list["FieldMeta"]
+    _fields_metadata: list[FieldMeta]
     # BaseFactory only attributes
     _factory_type_mapping: ClassVar[dict[Any, type["BaseFactory"]]]
     _base_factories: ClassVar[list[type["BaseFactory"]]]
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init_subclass__(*args, **kwargs)
 
@@ -195,24 +203,23 @@
                 for factory in BaseFactory._base_factories:
                     if factory.is_supported_type(model):
                         raise ConfigurationException(
                             f"{cls.__name__} does not support {model.__name__}, but this type is support by the {factory.__name__} base factory class. T"
                             f"o resolve this error, subclass the factory from {factory.__name__} instead of {cls.__name__}"
                         )
                     raise ConfigurationException(
-                        "Model type {model.__name__} is not supported. "
+                        f"Model type {model.__name__} is not supported. "
                         "To support it, register an appropriate base factory and subclass it for your factory."
                     )
+        else:
+            BaseFactory._base_factories.append(cls)
 
         if random_seed := getattr(cls, "__random_seed__", None) is not None:
             cls.seed_random(random_seed)
 
-        if cls.__is_base_factory__:
-            BaseFactory._base_factories.append(cls)
-
         if cls.__set_as_default_factory_for_type__:
             BaseFactory._factory_type_mapping[cls.__model__] = cls
 
     @classmethod
     def _get_sync_persistence(cls) -> SyncPersistenceProtocol[T]:
         """Return a SyncPersistenceHandler if defined for the factory, otherwise raises a ConfigurationException.
 
@@ -277,15 +284,15 @@
         :param model: A model type.
         :returns: A Factory sub-class.
 
         """
         if factory := BaseFactory._factory_type_mapping.get(model):
             return factory
 
-        for factory in BaseFactory._base_factories:
+        for factory in reversed(BaseFactory._base_factories):
             if factory.is_supported_type(model):
                 return factory.create_factory(model)
 
         raise ParameterException(f"unsupported model type {model.__name__}")  # pragma: no cover
 
     # Public Methods
 
@@ -307,15 +314,15 @@
         """
         origin = get_type_origin(annotation) or annotation
         if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation)):  # type: ignore
             return len(args) == 1 and BaseFactory.is_factory_type(annotation=args[0])
         return False
 
     @classmethod
-    def extract_field_build_parameters(cls, field_meta: "FieldMeta", build_args: dict[str, Any]) -> Any:
+    def extract_field_build_parameters(cls, field_meta: FieldMeta, build_args: dict[str, Any]) -> Any:
         """Extract from the build kwargs any build parameters passed for a given field meta - if it is a factory type.
 
         :param field_meta: A field meta instance.
         :param build_args: Any kwargs passed to the factory.
         :returns: Any values
         """
         if build_arg := build_args.get(field_meta.name):
@@ -459,54 +466,129 @@
         :param model: A type to model.
         :param bases: Base classes to use when generating the new class.
         :param kwargs: Any kwargs.
 
         :returns: A 'ModelFactory' subclass.
 
         """
-
-        for key in (attr for attr in dir(cls) if attr.startswith("__") and attr != "__model__"):
-            kwargs.setdefault(key, getattr(cls, key, None))
-
         return cast(
             "Type[BaseFactory]",
             type(
                 f"{model.__name__}Factory",
                 (*(bases or ()), cls),
                 {"__model__": model, **kwargs},
             ),
         )
 
     @classmethod
-    def get_field_value(cls, field_meta: "FieldMeta", field_build_parameters: Any | None = None) -> Any:
+    def get_constrained_field_value(cls, annotation: Any, field_meta: FieldMeta) -> Any:
+        constraints = cast("Constraints", field_meta.constraints)
+        if is_safe_subclass(annotation, float):
+            return handle_constrained_float(
+                random=cls.__random__,
+                multiple_of=cast("Any", constraints.get("multiple_of")),
+                gt=cast("Any", constraints.get("gt")),
+                ge=cast("Any", constraints.get("ge")),
+                lt=cast("Any", constraints.get("lt")),
+                le=cast("Any", constraints.get("le")),
+            )
+
+        if is_safe_subclass(annotation, int):
+            return handle_constrained_int(
+                random=cls.__random__,
+                multiple_of=cast("Any", constraints.get("multiple_of")),
+                gt=cast("Any", constraints.get("gt")),
+                ge=cast("Any", constraints.get("ge")),
+                lt=cast("Any", constraints.get("lt")),
+                le=cast("Any", constraints.get("le")),
+            )
+
+        if is_safe_subclass(annotation, Decimal):
+            return handle_constrained_decimal(
+                random=cls.__random__,
+                decimal_places=cast("Any", constraints.get("decimal_places")),
+                max_digits=cast("Any", constraints.get("max_digits")),
+                multiple_of=cast("Any", constraints.get("multiple_of")),
+                gt=cast("Any", constraints.get("gt")),
+                ge=cast("Any", constraints.get("ge")),
+                lt=cast("Any", constraints.get("lt")),
+                le=cast("Any", constraints.get("le")),
+            )
+
+        if is_safe_subclass(annotation, str) or is_safe_subclass(annotation, bytes):
+            return handle_constrained_string_or_bytes(
+                random=cls.__random__,
+                t_type=str if is_safe_subclass(annotation, str) else bytes,
+                lower_case=constraints.get("lower_case") or False,
+                upper_case=constraints.get("upper_case") or False,
+                min_length=constraints.get("min_length"),
+                max_length=constraints.get("max_length"),
+                pattern=constraints.get("pattern"),
+            )
+
+        if (
+            is_safe_subclass(annotation, set)
+            or is_safe_subclass(annotation, list)
+            or is_safe_subclass(annotation, frozenset)
+        ):
+            result = handle_constrained_collection(
+                collection_type=list if is_safe_subclass(annotation, list) else set,  # pyright: ignore
+                factory=cls,
+                field_meta=field_meta.children[0] if field_meta.children else field_meta,
+                item_type=constraints.get("item_type"),
+                max_items=constraints.get("max_length"),
+                min_items=constraints.get("min_length"),
+                unique_items=constraints.get("unique_items", False),
+            )
+            return frozenset(result) if is_safe_subclass(annotation, frozenset) else result
+
+        if is_safe_subclass(annotation, date):
+            return handle_constrained_date(
+                faker=cls.__faker__,
+                ge=cast("Any", constraints.get("ge")),
+                gt=cast("Any", constraints.get("gt")),
+                le=cast("Any", constraints.get("le")),
+                lt=cast("Any", constraints.get("lt")),
+            )
+
+        raise ParameterException(f"received constraints for unsupported type {annotation}")
+
+    @classmethod
+    def get_field_value(cls, field_meta: FieldMeta, field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
 
         :param field_meta: FieldMeta instance.
         :param field_build_parameters: Any build parameters passed to the factory as kwarg values.
 
         :returns: An arbitrary value.
 
         """
         if cls.is_ignored_type(field_meta.annotation):
             return None
 
-        if field_meta.constant:
+        if field_meta.constraints and field_meta.constraints.get("constant", False):
             return field_meta.default
 
         if cls.should_set_none_value(field_meta=field_meta):
             return None
 
         unwrapped_annotation = unwrap_annotation(field_meta.annotation)
 
         if is_literal(annotation=unwrapped_annotation) and (literal_args := get_args(unwrapped_annotation)):
             return cls.__random__.choice(literal_args)
 
         if isinstance(unwrapped_annotation, EnumMeta):
             return cls.__random__.choice(list(unwrapped_annotation))  # pyright: ignore
 
+        if field_meta.constraints and (
+            unwrapped_annotation in (float, int, Decimal, str, list, tuple, set, frozenset)
+            or unwrapped_annotation not in cls.get_provider_map()
+        ):
+            return cls.get_constrained_field_value(annotation=unwrapped_annotation, field_meta=field_meta)
+
         if BaseFactory.is_factory_type(annotation=unwrapped_annotation):
             return cls._get_or_create_factory(model=unwrapped_annotation).build(
                 **(field_build_parameters if isinstance(field_build_parameters, Mapping) else {})
             )
 
         if BaseFactory.is_batch_factory_type(annotation=unwrapped_annotation):
             factory = cls._get_or_create_factory(model=field_meta.type_args[0])
@@ -516,15 +598,15 @@
 
         if field_meta.children:
             return handle_complex_type(field_meta=field_meta, factory=cls)
 
         return cls.get_mock_value(annotation=unwrapped_annotation)
 
     @classmethod
-    def should_set_none_value(cls, field_meta: "FieldMeta") -> bool:
+    def should_set_none_value(cls, field_meta: FieldMeta) -> bool:
         """Determine whether a given model field_meta should be set to None.
 
         :param field_meta: Field metadata.
 
         :notes:
             - This method is distinct to allow overriding.
 
@@ -534,15 +616,15 @@
         return (
             cls.__allow_none_optionals__
             and is_optional_union(field_meta.annotation)
             and create_random_boolean(random=cls.__random__)
         )
 
     @classmethod
-    def should_set_field_value(cls, field_meta: "FieldMeta", **kwargs: Any) -> bool:
+    def should_set_field_value(cls, field_meta: FieldMeta, **kwargs: Any) -> bool:
         """Determine whether to set a value for a given field_name.
 
         :param field_meta: FieldMeta instance.
         :param kwargs: Any kwargs passed to the factory.
 
         :notes:
             - This method is distinct to allow overriding.
@@ -550,15 +632,15 @@
         :returns: A boolean determining whether a value should be set for the given field_meta.
 
         """
         return not field_meta.name.startswith("_") and field_meta.name not in kwargs
 
     @classmethod
     @abstractmethod
-    def get_model_fields(cls) -> list["FieldMeta"]:  # pragma: no cover
+    def get_model_fields(cls) -> list[FieldMeta]:  # pragma: no cover
         """Retrieve a list of fields from the factory's model.
 
 
         :returns: A list of field MetaData instances.
 
         """
         raise NotImplementedError
```

### Comparing `polyfactory-2.0.0a1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.0.1/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.0.1/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.0.1/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/fields.py` & `polyfactory-2.0.1/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/persistence.py` & `polyfactory-2.0.1/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/pytest_plugin.py` & `polyfactory-2.0.1/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/utils/helpers.py` & `polyfactory-2.0.1/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/utils/predicates.py` & `polyfactory-2.0.1/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.0.1/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.0.1/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.0.1/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.0.1/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.0.1/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/primitives.py` & `polyfactory-2.0.1/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/polyfactory/value_generators/regex.py` & `polyfactory-2.0.1/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.0.0a1/pyproject.toml` & `polyfactory-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.0.0alpha1"
+version = "2.0.1"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
+    "Jacob Coffee <jacob@z7x.org>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
+    "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
 repository = "https://github.com/litestar-org/polyfactory"
 documentation = "https://github.com/litestar-org/polyfactory"
 keywords = [
```

### Comparing `polyfactory-2.0.0a1/PKG-INFO` & `polyfactory-2.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.0.0a1
+Version: 2.0.1
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -67,19 +67,25 @@
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_polyfactory&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_polyfactory)
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
 </div>
 <!-- markdownlint-restore -->
 
-This library offers factories for mock data generation using python type hints. It part of the LiteStar-API project and
-is actively maintained by a community of maintainers and contributors.
+Polyfactory is a simple and powerful mock data generation library, based around type
+hints and supporting dataclasses, typed-dicts, Pydantic models and more.
+
+Polyfactory part of the Litestar project and as such actively maintained by a community of maintainers and contributors.
 
 ## Example
 
 ```python
 from dataclasses import dataclass
 
 from polyfactory.factories import DataclassFactory
@@ -98,43 +104,66 @@
 
 
 def test_is_person() -> None:
     person_instance = PersonFactory.build()
     assert isinstance(person_instance, Person)
 ```
 
-That's it - with almost no work, we are able to create a mock data object fitting the Person class model definition.
+That's it - with almost no work, we are able to create a mock data object fitting the `Person` class model definition.
 
 This is possible because of the typing information available on the dataclass, which are used as a
 source of truth for data generation.
 
 The factory parses the information stored in the dataclass and generates a dictionary of kwargs that are passed to
-the Person class constructor.
+`Person`.
 
 ## Documentation
 
-A full API reference and usage documentation is available in
-the [dedicated documentation site](https://polyfactory.litestar.dev/).
+Usage and API reference documentation is available on https://polyfactory.litestar.dev/.
 
 ## Installation
 
 ```shell
 pip install polyfactory
 ```
 
 ## Relation to Pydantic-Factories
 
-The earlier version of this library was released under the
-name [pydantic-factories](https://pypi.org/project/pydantic-factories/).
-While this library became very popular (above 100K monthly downloads), we decided to rename it because we changed the
-core architecture -
-`polyfactory` is a fitting name because we no longer rely on pydantic, which is now an optional dependency. This library
-is capable of
-generating mock data for dataclasses, typed-dicts and any custom factory using type annotations.
-It also supports using pydantic models - but that is optional.
+Prior to version 2, this library was known as [pydantic-factories](https://pypi.org/project/pydantic-factories/), a name
+under which it gained quite a bit of popularity.
+A main motivator for the 2.0 release was that we wanted to support more than just Pydantic models, something which also
+required a change to its core architecture. As this library would no longer be directly tied to Pydantic, `polyfactory`
+was chosen as its new name to reflect its capabilities; It can generate mock data for dataclasses, typed-dicts,
+Pydantic, odmantic, and beanie ODM models, as well as custom factories.
 
 ## Contributing
 
 This library is a community driven open source project. We welcome and encourage contributions. Please checkout the
 GitHub issues, read the contribution guide (at the repository's root), and you're always welcome
 to [join our discord server](https://discord.gg/F4jPQzHpBU).
 
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://scriptr.dev/"><img src="https://avatars.githubusercontent.com/u/45884264?v=4?s=100" width="100px;" alt="Jacob Coffee"/><br /><sub><b>Jacob Coffee</b></sub></a><br /><a href="#infra-JacobCoffee" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Code">💻</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=JacobCoffee" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/provinzkraut"><img src="https://avatars.githubusercontent.com/u/25355197?v=4?s=100" width="100px;" alt="Janek Nouvertné"/><br /><sub><b>Janek Nouvertné</b></sub></a><br /><a href="#infra-provinzkraut" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Code">💻</a> <a href="#design-provinzkraut" title="Design">🎨</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=provinzkraut" title="Documentation">📖</a> <a href="#maintenance-provinzkraut" title="Maintenance">🚧</a> <a href="#projectManagement-provinzkraut" title="Project Management">📆</a> <a href="https://github.com/litestar-org/polyfactory/pulls?q=is%3Apr+reviewed-by%3Aprovinzkraut" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Goldziher"><img src="https://avatars.githubusercontent.com/u/30733348?v=4?s=100" width="100px;" alt="Na'aman Hirschfeld"/><br /><sub><b>Na'aman Hirschfeld</b></sub></a><br /><a href="#infra-Goldziher" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/polyfactory/commits?author=Goldziher" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://czaplicki.it/"><img src="https://avatars.githubusercontent.com/u/9108586?v=4?s=100" width="100px;" alt="Marek Czaplicki"/><br /><sub><b>Marek Czaplicki</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=mdczaplicki" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/przybylop"><img src="https://avatars.githubusercontent.com/u/82805821?v=4?s=100" width="100px;" alt="Piotr Przybyło"/><br /><sub><b>Piotr Przybyło</b></sub></a><br /><a href="https://github.com/litestar-org/polyfactory/commits?author=przybylop" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

