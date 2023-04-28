# Comparing `tmp/pydwrap-0.5.8.tar.gz` & `tmp/pydwrap-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwrap-0.5.8.tar", max compression
+gzip compressed data, was "pydwrap-0.6.0.tar", max compression
```

## Comparing `pydwrap-0.5.8.tar` & `pydwrap-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-04-13 21:37:36.137941 pydwrap-0.5.8/LICENSE
--rw-r--r--   0        0        0     1205 2023-04-13 21:37:36.137941 pydwrap-0.5.8/README.md
--rw-r--r--   0        0        0       69 2023-04-13 21:37:36.137941 pydwrap-0.5.8/pydwrap/__init__.py
--rw-r--r--   0        0        0     4390 2023-04-21 20:43:09.749102 pydwrap-0.5.8/pydwrap/main.py
--rw-r--r--   0        0        0     1203 2023-04-21 20:43:49.656625 pydwrap-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pydwrap-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-28 13:58:02.987801 pydwrap-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1628 2023-04-28 13:58:02.987801 pydwrap-0.6.0/README.md
+-rw-r--r--   0        0        0       69 2023-04-28 13:58:02.987801 pydwrap-0.6.0/pydwrap/__init__.py
+-rw-r--r--   0        0        0     5753 2023-04-28 13:58:02.987801 pydwrap-0.6.0/pydwrap/main.py
+-rw-r--r--   0        0        0     1235 2023-04-28 13:58:55.823505 pydwrap-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 pydwrap-0.6.0/PKG-INFO
```

### Comparing `pydwrap-0.5.8/LICENSE` & `pydwrap-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwrap-0.5.8/README.md` & `pydwrap-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-# ♻️ pydwrap pydantic optional fields ♻️
+# ♻️ pydwrap pydantic.BaseModel optional fields ♻️
 
 
-pydwrap stores a **Option** object to implement unpacking of values if they are not **None**. The **BaseModel** object is also a little extended to work with the **Option** object.
+pydwrap stores a **Option** type to implement unpacking of values if they are not **None**. The **BaseModel** is also a little extended to work with the **Option** type.
 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pypi](https://img.shields.io/pypi/v/pydwrap.svg)](https://pypi.python.org/pypi/pydwrap)
 [![versions](https://img.shields.io/pypi/pyversions/pydwrap.svg)](https://github.com/luwqz1/pydwrap)
 [![license](https://img.shields.io/github/license/luwqz1/pydwrap.svg)](https://github.com/luwqz1/pydwrap/blob/main/LICENSE)
 
 
 # ⭐️ A simple example ⭐️
 ```python
 from pydwrap import BaseModel, Option
 
+
 class User(BaseModel):
-    name: Option[str]
-    age: int
+    """Anonim User model."""
 
-data = {
-    "age": 20
+    first_name: str
+    last_name: Option[str]
+    about: Option[str]
+    age: Option[int]
+    about: Option[str]
+    city: Option[str]
+    friends: list["User"]
+
+
+some_response = {
+    "first_name": "Max",
+    "last_name": None,
+    "age": None,
+    "about": "Hello, World!",
+    "city": None,
+    "friends": [],
 }
-user = User(**data)
-#> User(name=Option(None), age=20)
-print("Hello", user.name.unwrap(error_msg="What's your name?") + "!")
-#> ValueError: What's your name?
+user = User(**some_response)
+#> User(first_name='Max', last_name=Option(None), about=Option('Hello, World!'), age=Option(None), city=Option(None), friends=[])
+print("Hello,", user.first_name + "!\n" + f"You are {user.age.unwrap(error='How old is he?')} years old.")
+#> ValueError: How old is he?
 ```
 
 # 📚 Documentation 📚
 * In 🇷🇺 [**Russian**](https://github.com/luwqz1/pydwrap/blob/main/docs/RU.md) 🇷🇺
 * In 🇺🇸 [**English**](https://github.com/luwqz1/pydwrap/blob/main/docs/EN.md) 🇺🇸
```

### Comparing `pydwrap-0.5.8/pydwrap/main.py` & `pydwrap-0.6.0/pydwrap/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,154 @@
 from __future__ import annotations
 
-from typing import Any, Generic, Type, TypeVar, cast, get_origin
+from typing import Any, Generic, NewType, Type, TypeVar, cast, get_origin
 
 from pydantic import BaseModel as OriginalBaseModel
 from pydantic import create_model, root_validator
 from pydantic.fields import ModelField
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.typing import is_none_type
 
 _T = TypeVar("_T")
-_V = TypeVar("_V")
-ValidatorOptionValue = TypeVar("ValidatorOptionValue", bound="BaseModel")
+_O = TypeVar("_O")
+ValidatorOptionValue = NewType("ValidatorOptionValue", "BaseModel")
 
 
 class Option(Generic[_T]):
     """Type Option in order to correctly handle optional value."""
 
     __value: _T | None
 
-    def __init__(self, value: _T | None = None):
+    def __init__(self, value: _T | None = None, /):
+        """All or nothing."""
         self.__value = value
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
         return "%s(%s)" % (
             self.__class__.__name__,
             repr(self.__value),
         )
 
     @classmethod
     def __get_validators__(cls):
+        """Getter validators for `BaseModel` object."""
         yield cls.option_validator
 
     @classmethod
     def option_validator(cls, v: Any, field: ModelField) -> Option[_T]:
+        """Validator for `BaseModel` object."""
         field_name: str = field.name.removeprefix("_").removesuffix("_")
         if field.outer_type_ is Option:
-            raise TypeError(
-                "To type an Option, it is necessary to specify a parameter in its generic."
-            )
+            raise TypeError("To type an Option, it is necessary to specify a parameter in its generic.")
         if v is None:
             return cls(v)
         if isinstance(v, cls) and v.is_none:
             return v
         validator = _create_validator_option_value(
             field_name,
             v.unwrap() if isinstance(v, cls) else v,
             field.outer_type_.__args__[0],
         )
         return cls(getattr(validator, field_name))
 
     @property
     def is_none(self) -> bool:
-        """Return True if value is None."""
+        """Return `True` if value is None."""
         return self.__value is None
 
-    def unwrap(self, *, error_msg: str = None) -> _T:
+    def unwrap(self, *, error: str | None = None) -> _T:
         """Unwrap the optional value if it's not None, otherwise a
-        ValueError will be raised with the appropriate error_msg.
+        `ValueError` will be raised with the appropriate `error`.
         """
         if self.__value is None:
-            raise ValueError(error_msg if error_msg is not None else "Value is None.")
+            raise ValueError(error or "Value is None.")
         return self.__value
 
-    def unwrap_or(self, variant: _V, /) -> _T | _V:
+    def unwrap_or(self, variant: _T, /) -> _T:
         """Unwrap the optional value if it's not None,
         otherwise it will return the variant you passed.
         """
         if variant is None:
             raise TypeError("Variant should not be type NoneType.")
         return self.__value if self.__value is not None else variant
 
+    def unwrap_or_other(self, other: _O, /) -> _T | _O:
+        """Similar to the `unwrap_or` method, only this one takes any other type."""
+        if other is None:
+            raise TypeError("Other value should not be type NoneType.")
+        return self.__value if self.__value is not None else other
+
+    def unwrap_or_else(self, option: Option[_T], /) -> _T:
+        """Unwrap optional value this `Option` or if it is None
+        then unwrap optional value of another `Option` if it is
+        also None, then a `ValueError` exception is raised.
+        """
+        if not isinstance(option, type(self)):
+            raise TypeError("Another option cannot be type '%s', only type 'Option'." % type(option).__name__)
+        if self.is_none and option.is_none:
+            raise ValueError("This Option value is None and the other Option value is None.")
+        return self.__value if self.__value is not None else option.unwrap()
+
 
 class BaseModel(OriginalBaseModel):
-    @root_validator(
-        pre=True
-    )  # NOTE: Pycharm doesn't understand that @root_validator returns a classmethod.
+    @root_validator(pre=True)  # NOTE: Pycharm doesn't understand that @root_validator returns a classmethod.
     @classmethod
     def _pre_root_validator(cls, values: dict[str, Any]) -> dict[str, Any]:
+        """Pre root validator to validate an `Option` type unknown to `BaseModel`."""
         model_schema = cls.schema()
         fields = _get_default_fields(model_schema)
-        fields.update(_get_required_option_fields(cls.__annotations__, model_schema))
-        fields.update(values)
+        fields |= _get_required_option_fields(cls.__annotations__, model_schema)
+        fields |= values
         return {
             field: Option(value)
-            if _is_option_type(cls.__annotations__.get(field, None))
-            and not isinstance(value, Option)
+            if _is_option_type(cls.__annotations__.get(field, None)) and not isinstance(value, Option)
             else value
             for field, value in fields.items()
         }
 
 
 def _is_option_type(type_: Type[Any]) -> bool:
+    """Return `True` if type is `Generic Option`."""
     if is_none_type(type_):
         return False
     origin = get_origin(type_)
     if is_none_type(origin):
         return False
     return origin is Option
 
 
 def _get_default_fields(schema: dict[str, Any]) -> dict[str, Any]:
+    """Get default fields by `BaseModel` schema."""
     properties = cast(dict[str, Any], schema.get("properties", {}))
-    return {
-        k: properties[k]["default"] for k in properties if "default" in properties[k]
-    }
+    return {k: properties[k]["default"] for k in properties if "default" in properties[k]}
 
 
-def _get_required_option_fields(
-    model_annotations: dict[str, Any], schema: dict[str, Any]
-) -> dict[str, Option]:
+def _get_required_option_fields(model_annotations: dict[str, Any], schema: dict[str, Any]) -> dict[str, Option]:
+    """Get required fields with the Option type by
+    `BaseModel` schema and `field annotations`.
+    """
     properties = cast(dict[str, Any], schema.get("properties", {}))
     return {
         k: Option()
         for k in properties
-        if k in schema.get("required", [])
-        or "default" not in properties[k]
-        and _is_option_type(model_annotations[k])
+        if k in schema.get("required", []) or "default" not in properties[k] and _is_option_type(model_annotations[k])
     }
 
 
-def _create_validator_option_value(
-    field_name: str, field_value: Any, field_type: Type[Any]
-) -> ValidatorOptionValue:
+def _create_validator_option_value(field_name: str, field_value: Any, field_type: Type[Any]) -> ValidatorOptionValue:
+    """Create instance `ValidatorOptionValue` based on `BaseModel`."""
     return create_model(
         "ValidatorOptionValue",
         __base__=BaseModel,
         **{
             field_name: (
                 field_type,
                 field_value,
             )
         },
-    )()
+    )()  # type: ignore
 
 
-ENCODERS_BY_TYPE.update({Option: lambda o: None if o.is_none else o.unwrap()})
+ENCODERS_BY_TYPE.update({Option: lambda o: None if o.is_none else o.unwrap()})  # Add Option type in json encoders.
```

### Comparing `pydwrap-0.5.8/pyproject.toml` & `pydwrap-0.6.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pydwrap"
-version = "0.5.8"
-description = "pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object."
+version = "0.6.0"
+description = "pydwrap stores a Option type to implement unpacking of values if they are not None. The BaseModel is also a little extended to work with the Option type."
 authors = ["Georgy howl <howluwqz1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydwrap"}]
 homepage = "https://github.com/luwqz1/pydwrap"
 repository = "https://github.com/luwqz1/pydwrap"
 keywords = ["python", "wrapping", "optional handle", "basemodel fields", "option", "pydwrap"]
@@ -31,10 +31,13 @@
 max-doc-length = 90
 per-file-ignores = "__init__.py: F401"
 
 [tool.black]
 line-length = 120
 target-version = ["py39", "py310", "py311"]
 
+[tool.mypy]
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydwrap-0.5.8/PKG-INFO` & `pydwrap-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pydwrap
-Version: 0.5.8
-Summary: pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object.
+Version: 0.6.0
+Summary: pydwrap stores a Option type to implement unpacking of values if they are not None. The BaseModel is also a little extended to work with the Option type.
 Home-page: https://github.com/luwqz1/pydwrap
 License: MIT
 Keywords: python,wrapping,optional handle,basemodel fields,option,pydwrap
 Author: Georgy howl
 Author-email: howluwqz1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pydantic
@@ -18,39 +18,53 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Project-URL: Repository, https://github.com/luwqz1/pydwrap
 Description-Content-Type: text/markdown
 
-# ♻️ pydwrap pydantic optional fields ♻️
+# ♻️ pydwrap pydantic.BaseModel optional fields ♻️
 
 
-pydwrap stores a **Option** object to implement unpacking of values if they are not **None**. The **BaseModel** object is also a little extended to work with the **Option** object.
+pydwrap stores a **Option** type to implement unpacking of values if they are not **None**. The **BaseModel** is also a little extended to work with the **Option** type.
 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pypi](https://img.shields.io/pypi/v/pydwrap.svg)](https://pypi.python.org/pypi/pydwrap)
 [![versions](https://img.shields.io/pypi/pyversions/pydwrap.svg)](https://github.com/luwqz1/pydwrap)
 [![license](https://img.shields.io/github/license/luwqz1/pydwrap.svg)](https://github.com/luwqz1/pydwrap/blob/main/LICENSE)
 
 
 # ⭐️ A simple example ⭐️
 ```python
 from pydwrap import BaseModel, Option
 
+
 class User(BaseModel):
-    name: Option[str]
-    age: int
+    """Anonim User model."""
 
-data = {
-    "age": 20
+    first_name: str
+    last_name: Option[str]
+    about: Option[str]
+    age: Option[int]
+    about: Option[str]
+    city: Option[str]
+    friends: list["User"]
+
+
+some_response = {
+    "first_name": "Max",
+    "last_name": None,
+    "age": None,
+    "about": "Hello, World!",
+    "city": None,
+    "friends": [],
 }
-user = User(**data)
-#> User(name=Option(None), age=20)
-print("Hello", user.name.unwrap(error_msg="What's your name?") + "!")
-#> ValueError: What's your name?
+user = User(**some_response)
+#> User(first_name='Max', last_name=Option(None), about=Option('Hello, World!'), age=Option(None), city=Option(None), friends=[])
+print("Hello,", user.first_name + "!\n" + f"You are {user.age.unwrap(error='How old is he?')} years old.")
+#> ValueError: How old is he?
 ```
 
 # 📚 Documentation 📚
 * In 🇷🇺 [**Russian**](https://github.com/luwqz1/pydwrap/blob/main/docs/RU.md) 🇷🇺
 * In 🇺🇸 [**English**](https://github.com/luwqz1/pydwrap/blob/main/docs/EN.md) 🇺🇸
```

