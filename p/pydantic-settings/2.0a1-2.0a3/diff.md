# Comparing `tmp/pydantic_settings-2.0a1.tar.gz` & `tmp/pydantic_settings-2.0a3.tar.gz`

## Comparing `pydantic_settings-2.0a1.tar` & `pydantic_settings-2.0a3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.github/FUNDING.yml
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/main.py
--rw-r--r--   0        0        0    15054 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/utils.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/all.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/linting.in
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/linting.txt
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/pyproject.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/testing.in
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/testing.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/tests/conftest.py
--rw-r--r--   0        0        0    40327 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/tests/test_settings.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/LICENSE
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/README.md
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pyproject.toml
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    18107 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/docs/index.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/main.py
+-rw-r--r--   0        0        0    19763 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/all.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/linting.in
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/linting.txt
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/pyproject.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/testing.in
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/testing.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/tests/conftest.py
+-rw-r--r--   0        0        0    43806 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/tests/test_settings.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/LICENSE
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/README.md
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/PKG-INFO
```

### Comparing `pydantic_settings-2.0a1/.pre-commit-config.yaml` & `pydantic_settings-2.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/Makefile` & `pydantic_settings-2.0a3/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/.github/workflows/ci.yml` & `pydantic_settings-2.0a3/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
   test:
     name: test py${{ matrix.python }} on ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, macos, windows]
-        python: ['3.7', '3.8', '3.9', '3.10', '3.11-dev']
+        python: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     env:
       PYTHON: ${{ matrix.python }}
       OS: ${{ matrix.os }}
 
     runs-on: ${{ matrix.os }}-latest
 
@@ -99,21 +99,19 @@
 
       - name: set up python
         uses: actions/setup-python@v4
         with:
           python-version: '3.10'
 
       - name: install
-        run: pip install -U build twine
+        run: pip install -U build
 
       - name: check GITHUB_REF matches package version
         uses: samuelcolvin/check-python-version@v3.1
         with:
           version_file_path: pydantic_settings/version.py
 
       - name: build
         run: python -m build
 
-      - run: twine check dist/*
-
       - name: Upload package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pydantic_settings-2.0a1/pydantic_settings/main.py` & `pydantic_settings-2.0a3/pydantic_settings/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/pydantic_settings/sources.py` & `pydantic_settings-2.0a3/pydantic_settings/sources.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations as _annotations
 
 import json
 import os
 import warnings
 from abc import ABC, abstractmethod
+from collections import deque
 from dataclasses import is_dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
 
 from pydantic import BaseModel
 from pydantic._internal._typing_extra import origin_is_union
 from pydantic._internal._utils import deep_update, lenient_issubclass
 from pydantic.fields import FieldInfo
 from typing_extensions import get_origin
 
@@ -49,18 +50,24 @@
 
         Returns:
             Tuple[str, Any, bool]: The key, value and a flag to determine whether value is complex.
         """
         pass
 
     def field_is_complex(self, field: FieldInfo) -> bool:
-        def _annotation_is_complex(annotation: type[Any] | None) -> bool:
-            return lenient_issubclass(annotation, (BaseModel, list, set, frozenset, dict)) or is_dataclass(annotation)
+        """
+        Checks whether a field is complex, in which case it will attempt to be parsed as JSON.
 
-        return _annotation_is_complex(field.annotation) or _annotation_is_complex(get_origin(field.annotation))
+        Args:
+            field (FieldInfo): The field.
+
+        Returns:
+            bool: Whether the field is complex.
+        """
+        return _annotation_is_complex(field.annotation)
 
     def prepare_field_value(self, field_name: str, field: FieldInfo, value: Any, value_is_complex: bool) -> Any:
         """
         Prepares the value of a field.
 
         Args:
             field_name (str): The field name.
@@ -125,24 +132,81 @@
                     if isinstance(alias, str):  # AliasPath
                         field_info.append((alias, self._apply_case_sensitive(alias), True if len(alias) > 1 else False))
                     elif isinstance(alias, list):  # AliasChoices
                         field_info.append(
                             (alias[0], self._apply_case_sensitive(alias[0]), True if len(alias) > 1 else False)
                         )
             else:  # string validation alias
-                field_info.append(
-                    (v_alias, self._apply_case_sensitive(self.config.get('env_prefix', '') + v_alias), False)
-                )
+                field_info.append((v_alias, self._apply_case_sensitive(v_alias), False))
         else:
             field_info.append(
                 (field_name, self._apply_case_sensitive(self.config.get('env_prefix', '') + field_name), False)
             )
 
         return field_info
 
+    def _replace_field_names_case_insensitively(self, field: FieldInfo, field_values: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Replace field names in values dict by looking in models fields insensitively.
+
+        By having the following models:
+
+            ```py
+            class SubSubSub(BaseModel):
+                VaL3: str
+
+            class SubSub(BaseModel):
+                Val2: str
+                SUB_sub_SuB: SubSubSub
+
+            class Sub(BaseModel):
+                VAL1: str
+                SUB_sub: SubSub
+
+            class Settings(BaseSettings):
+                nested: Sub
+
+                model_config = ConfigDict(env_nested_delimiter='__')
+            ```
+
+        Then:
+            _replace_field_names_case_insensitively(
+                field,
+                {"val1": "v1", "sub_SUB": {"VAL2": "v2", "sub_SUB_sUb": {"vAl3": "v3"}}}
+            )
+            Returns {'VAL1': 'v1', 'SUB_sub': {'Val2': 'v2', 'SUB_sub_SuB': {'VaL3': 'v3'}}}
+        """
+        values: Dict[str, Any] = {}
+
+        for name, value in field_values.items():
+            sub_model_field: Optional[FieldInfo] = None
+
+            # This is here to make mypy happy
+            # Item "None" of "Optional[Type[Any]]" has no attribute "model_fields"
+            if not field.annotation or not hasattr(field.annotation, 'model_fields'):
+                values[name] = value
+                continue
+
+            # Find field in sub model by looking in fields case insensitively
+            for sub_model_field_name, f in field.annotation.model_fields.items():
+                if not f.validation_alias and sub_model_field_name.lower() == name.lower():
+                    sub_model_field = f
+                    break
+
+            if not sub_model_field:
+                values[name] = value
+                continue
+
+            if lenient_issubclass(sub_model_field.annotation, BaseModel):
+                values[sub_model_field_name] = self._replace_field_names_case_insensitively(sub_model_field, value)
+            else:
+                values[sub_model_field_name] = value
+
+        return values
+
     def __call__(self) -> Dict[str, Any]:
         d: Dict[str, Any] = {}
 
         for field_name, field in self.settings_cls.model_fields.items():
             try:
                 field_value, field_key, value_is_complex = self.get_field_value(field, field_name)
             except Exception as e:
@@ -154,15 +218,18 @@
                 field_value = self.prepare_field_value(field_name, field, field_value, value_is_complex)
             except ValueError as e:
                 raise SettingsError(
                     f'error parsing value for field "{field_name}" from source "{self.__class__.__name__}"'
                 ) from e
 
             if field_value is not None:
-                d[field_key] = field_value
+                if not self.config.get('case_sensitive', False) and lenient_issubclass(field.annotation, BaseModel):
+                    d[field_key] = self._replace_field_names_case_insensitively(field, field_value)
+                else:
+                    d[field_key] = field_value
 
         return d
 
 
 class SecretsSettingsSource(PydanticBaseEnvSettingsSource):
     def __init__(self, settings_cls: Type[BaseSettings], secrets_dir: Optional[Union[str, Path]]):
         self.secrets_dir = secrets_dir
@@ -284,14 +351,45 @@
         elif origin_is_union(get_origin(field.annotation)):
             allow_parse_failure = True
         else:
             return False, False
 
         return True, allow_parse_failure
 
+    @staticmethod
+    def next_field(field: Optional[FieldInfo], key: str) -> Optional[FieldInfo]:
+        """
+        Find the field in a sub model by key(env name)
+
+        By having the following models:
+
+            ```py
+            class SubSubModel(BaseSettings):
+                dvals: Dict
+
+            class SubModel(BaseSettings):
+                vals: List[str]
+                sub_sub_model: SubSubModel
+
+            class Cfg(BaseSettings):
+                sub_model: SubModel
+            ```
+
+        Then:
+            next_field(sub_model, 'vals') Returns the `vals` field of `SubModel` class
+            next_field(sub_model, 'sub_sub_model') Returns `sub_sub_model` field of `SubModel` class
+        """
+        if not field or origin_is_union(get_origin(field.annotation)):
+            # no support for Unions of complex BaseSettings fields
+            return None
+        elif field.annotation and hasattr(field.annotation, 'model_fields') and field.annotation.model_fields.get(key):
+            return field.annotation.model_fields[key]
+
+        return None
+
     def explode_env_vars(
         self, field_name: str, field: FieldInfo, env_vars: Mapping[str, Optional[str]]
     ) -> Dict[str, Any]:
         """
         Process env_vars and extract the values of keys containing env_nested_delimiter into nested dictionaries.
 
         This is applied to a single field, hence filtering by env_var prefix.
@@ -303,16 +401,32 @@
         for env_name, env_val in env_vars.items():
             if not any(env_name.startswith(prefix) for prefix in prefixes):
                 continue
             # we remove the prefix before splitting in case the prefix has characters in common with the delimiter
             env_name_without_prefix = env_name[self.env_prefix_len :]
             _, *keys, last_key = env_name_without_prefix.split(self.env_nested_delimiter)
             env_var = result
+            target_field: Optional[FieldInfo] = field
+
             for key in keys:
+                target_field = self.next_field(target_field, key)
                 env_var = env_var.setdefault(key, {})
+
+            # get proper field with last_key
+            target_field = self.next_field(target_field, last_key)
+
+            # check if env_val maps to a complex field and if so, parse the env_val
+            if target_field and env_val:
+                is_complex, allow_json_failure = self._field_is_complex(target_field)
+                if is_complex:
+                    try:
+                        env_val = json.loads(env_val)
+                    except ValueError as e:
+                        if not allow_json_failure:
+                            raise e
             env_var[last_key] = env_val
 
         return result
 
     def __repr__(self) -> str:
         return (
             f'EnvSettingsSource(env_nested_delimiter={self.env_nested_delimiter!r}, '
@@ -386,7 +500,26 @@
     """
     for f in dir_path.iterdir():
         if f.name == file_name:
             return f
         elif not case_sensitive and f.name.lower() == file_name.lower():
             return f
     return None
+
+
+def _annotation_is_complex(annotation: type[Any] | None) -> bool:
+    origin = get_origin(annotation)
+    return (
+        _annotation_is_complex_inner(annotation)
+        or _annotation_is_complex_inner(origin)
+        or hasattr(origin, '__pydantic_core_schema__')
+        or hasattr(origin, '__get_pydantic_core_schema__')
+    )
+
+
+def _annotation_is_complex_inner(annotation: type[Any] | None) -> bool:
+    if lenient_issubclass(annotation, str):
+        return False
+
+    return lenient_issubclass(annotation, (BaseModel, Mapping, Sequence, tuple, set, frozenset, deque)) or is_dataclass(
+        annotation
+    )
```

### Comparing `pydantic_settings-2.0a1/pydantic_settings/utils.py` & `pydantic_settings-2.0a3/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/requirements/linting.txt` & `pydantic_settings-2.0a3/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/requirements/testing.txt` & `pydantic_settings-2.0a3/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/tests/test_settings.py` & `pydantic_settings-2.0a3/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,26 +414,26 @@
 
     env.set('foobar_parent_from_field', 'foobar_parent_from_field')
     env.set('prefix_foobar_parent_from_field', 'prefix_foobar_parent_from_field')
 
     env.set('foobar_parent_from_config', 'foobar_parent_from_config')
     env.set('foobar_child_from_config', 'foobar_child_from_config')
 
-    env.set('prefix_foobar_child_from_field', 'prefix_foobar_child_from_field')
+    env.set('foobar_child_from_field', 'foobar_child_from_field')
 
     # a. Child class config overrides prefix
     class Parent(BaseSettings):
         foobar: str = Field(None, validation_alias='foobar_parent_from_field')
 
         model_config = ConfigDict(env_prefix='p_')
 
     class Child(Parent):
         model_config = ConfigDict(env_prefix='prefix_')
 
-    assert Child().foobar == 'prefix_foobar_parent_from_field'
+    assert Child().foobar == 'foobar_parent_from_field'
 
     # b. Child class overrides field
     class Parent(BaseSettings):
         foobar: str = Field(None, validation_alias='foobar_parent_from_config')
 
     class Child(Parent):
         foobar: str = Field(None, validation_alias='foobar_child_from_config')
@@ -447,15 +447,15 @@
         model_config = ConfigDict(env_prefix='p_')
 
     class Child(Parent):
         foobar: str = Field(None, validation_alias='foobar_child_from_field')
 
         model_config = ConfigDict(env_prefix='prefix_')
 
-    assert Child().foobar == 'prefix_foobar_child_from_field'
+    assert Child().foobar == 'foobar_child_from_field'
 
 
 def test_invalid_validation_alias(env):
     with pytest.raises(
         TypeError, match='Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`'
     ):
 
@@ -494,14 +494,29 @@
     assert Settings().foobar == 'val2'
 
     env.pop('foo1')
     env.set('bar', '["val1", "val2", "val3"]')
     assert Settings().foobar == 'val3'
 
 
+def test_validation_alias_with_env_prefix(env):
+    class Settings(BaseSettings):
+        foobar: str = Field(validation_alias='foo')
+
+        model_config = ConfigDict(env_prefix='p_')
+
+    env.set('p_foo', 'bar')
+    with pytest.raises(ValidationError) as exc_info:
+        Settings()
+    assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('foo',), 'msg': 'Field required', 'input': {}}]
+
+    env.set('foo', 'bar')
+    assert Settings().foobar == 'bar'
+
+
 def test_case_sensitive(monkeypatch):
     class Settings(BaseSettings):
         foo: str
 
         model_config = ConfigDict(case_sensitive=True)
 
     # Need to patch os.environ to get build to work on Windows, where os.environ is case insensitive
@@ -603,14 +618,18 @@
 
     class B(BaseSettings):
         b: int
 
     class Settings(BaseSettings):
         content: Union[A, B, datetime]
 
+    env.set('content', '{"a": "test"}')
+    s = Settings()
+    assert s.content == A(a='test')
+
     env.set('content', '2020-07-05T00:00:00Z')
     s = Settings()
     assert s.content == datetime(2020, 7, 5, 0, 0, tzinfo=timezone.utc)
 
 
 def test_env_union_without_complex_subfields_does_not_parse_json(env):
     class Settings(BaseSettings):
@@ -1386,7 +1405,110 @@
         ) -> Tuple[PydanticBaseSettingsSource, ...]:
             return (BadCustomSettingsSource(settings_cls),)
 
     with pytest.raises(
         SettingsError, match='error getting value for field "top" from source "BadCustomSettingsSource"'
     ):
         Settings()
+
+
+def test_nested_env_complex_values(env):
+    class SubSubModel(BaseSettings):
+        dvals: Dict
+
+    class SubModel(BaseSettings):
+        vals: List[str]
+        sub_sub_model: SubSubModel
+
+    class Cfg(BaseSettings):
+        sub_model: SubModel
+
+        model_config = ConfigDict(env_prefix='cfg_', env_nested_delimiter='__')
+
+    env.set('cfg_sub_model__vals', '["one", "two"]')
+    env.set('cfg_sub_model__sub_sub_model__dvals', '{"three": 4}')
+
+    assert Cfg().model_dump() == {'sub_model': {'vals': ['one', 'two'], 'sub_sub_model': {'dvals': {'three': 4}}}}
+
+    env.set('cfg_sub_model__vals', 'invalid')
+    with pytest.raises(
+        SettingsError, match='error parsing value for field "sub_model" from source "EnvSettingsSource"'
+    ):
+        Cfg()
+
+
+def test_nested_env_nonexisting_field(env):
+    class SubModel(BaseSettings):
+        vals: List[str]
+
+    class Cfg(BaseSettings):
+        sub_model: SubModel
+
+        model_config = ConfigDict(env_prefix='cfg_', env_nested_delimiter='__')
+
+    env.set('cfg_sub_model__foo_vals', '[]')
+    with pytest.raises(ValidationError):
+        Cfg()
+
+
+def test_nested_env_nonexisting_field_deep(env):
+    class SubModel(BaseSettings):
+        vals: List[str]
+
+    class Cfg(BaseSettings):
+        sub_model: SubModel
+
+        model_config = ConfigDict(env_prefix='cfg_', env_nested_delimiter='__')
+
+    env.set('cfg_sub_model__vals__foo__bar__vals', '[]')
+    with pytest.raises(ValidationError):
+        Cfg()
+
+
+def test_nested_env_union_complex_values(env):
+    class SubModel(BaseSettings):
+        vals: Union[List[str], Dict[str, str]]
+
+    class Cfg(BaseSettings):
+        sub_model: SubModel
+
+        model_config = ConfigDict(env_prefix='cfg_', env_nested_delimiter='__')
+
+    env.set('cfg_sub_model__vals', '["one", "two"]')
+    assert Cfg().model_dump() == {'sub_model': {'vals': ['one', 'two']}}
+
+    env.set('cfg_sub_model__vals', '{"three": "four"}')
+    assert Cfg().model_dump() == {'sub_model': {'vals': {'three': 'four'}}}
+
+    env.set('cfg_sub_model__vals', 'stringval')
+    with pytest.raises(ValidationError):
+        Cfg()
+
+    env.set('cfg_sub_model__vals', '{"invalid": dict}')
+    with pytest.raises(ValidationError):
+        Cfg()
+
+
+def test_nested_model_case_insensitive(env):
+    class SubSubSub(BaseModel):
+        VaL3: str
+        val4: str = Field(validation_alias='VAL4')
+
+    class SubSub(BaseModel):
+        Val2: str
+        SUB_sub_SuB: SubSubSub
+
+    class Sub(BaseModel):
+        VAL1: str
+        SUB_sub: SubSub
+
+    class Settings(BaseSettings):
+        nested: Sub
+
+        model_config = ConfigDict(env_nested_delimiter='__')
+
+    env.set('nested', '{"val1": "v1", "sub_SUB": {"VAL2": "v2", "sub_SUB_sUb": {"vAl3": "v3", "VAL4": "v4"}}}')
+    s = Settings()
+    assert s.nested.VAL1 == 'v1'
+    assert s.nested.SUB_sub.Val2 == 'v2'
+    assert s.nested.SUB_sub.SUB_sub_SuB.VaL3 == 'v3'
+    assert s.nested.SUB_sub.SUB_sub_SuB.val4 == 'v4'
```

### Comparing `pydantic_settings-2.0a1/LICENSE` & `pydantic_settings-2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a1/pyproject.toml` & `pydantic_settings-2.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = 'pydantic-settings'
 description = 'Settings management using Pydantic'
 authors = [
     {name = 'Samuel Colvin', email = 's@muelcolvin.com'},
     {name = 'Eric Jolibois', email = 'em.jolibois@gmail.com'},
     {name = 'Hasan Ramezani', email = 'hasan.r67@gmail.com'},
 ]
-license = {file = 'LICENSE'}
+license = 'MIT'
 readme = 'README.md'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
@@ -75,15 +75,14 @@
     'pragma: no cover',
     'raise NotImplementedError',
     'raise NotImplemented',
     'if TYPE_CHECKING:',
     '@overload',
 ]
 
-
 [tool.coverage.paths]
 source = [
     'pydantic_settings/',
 ]
 
 [tool.black]
 color = true
```

### Comparing `pydantic_settings-2.0a1/PKG-INFO` & `pydantic_settings-2.0a3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,17 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 2.0a1
+Version: 2.0a3
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2022 Samuel Colvin and other contributors
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -53,10 +33,19 @@
 Requires-Dist: python-dotenv>=0.21.0
 Description-Content-Type: text/markdown
 
 # pydantic-settings
 
 [![CI](https://github.com/pydantic/pydantic-settings/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic-settings/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![Coverage](https://codecov.io/gh/pydantic/pydantic-settings/branch/main/graph/badge.svg)](https://codecov.io/gh/pydantic/pydantic-settings)
+[![pypi](https://img.shields.io/pypi/v/pydantic-settings.svg)](https://pypi.python.org/pypi/pydantic-settings)
 [![license](https://img.shields.io/github/license/pydantic/pydantic-settings.svg)](https://github.com/pydantic/pydantic-settings/blob/main/LICENSE)
 
-Settings management using Pydantic. **Currently a work in progress.**
+Settings management using Pydantic, this is the new official home of Pydantic's `BaseSettings`.
+
+**Currently a work in progress.**
+
+This package will be officially released as V2 when pydantic V2 is released.
+
+This package was kindly donated to the [Pydantic organisation](https://github.com/pydantic) by Daniel Daniels, see [pydantic/pydantic#4492](https://github.com/pydantic/pydantic/pull/4492) for discussion.
+
+For the old "Hipster-orgazmic tool to mange application settings" package, see [version 0.2.5](https://pypi.org/project/pydantic-settings/0.2.5/).
```

