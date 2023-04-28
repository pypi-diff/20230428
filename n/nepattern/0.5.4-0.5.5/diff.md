# Comparing `tmp/nepattern-0.5.4.tar.gz` & `tmp/nepattern-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.4.tar", last modified: Mon Apr 24 13:41:55 2023, max compression
+gzip compressed data, was "nepattern-0.5.5.tar", last modified: Fri Apr 28 07:35:36 2023, max compression
```

## Comparing `nepattern-0.5.4.tar` & `nepattern-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.4/LICENSE
--rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.4/nepattern/__init__.py
--rw-r--r--   0        0        0     8885 2023-04-24 13:27:27.344009 nepattern-0.5.4/nepattern/base.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.4/nepattern/context.py
--rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.4/nepattern/context.pyi
--rw-r--r--   0        0        0    15361 2023-04-24 13:27:05.487874 nepattern-0.5.4/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.4/nepattern/exception.py
--rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.4/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.4/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.4/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.4/nepattern/main.py
--rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.4/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-04-24 13:15:20.006654 nepattern-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.4/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.5/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.5/nepattern/__init__.py
+-rw-r--r--   0        0        0     8885 2023-04-24 13:27:27.344009 nepattern-0.5.5/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.5/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.5/nepattern/context.pyi
+-rw-r--r--   0        0        0    15577 2023-04-28 07:29:56.289893 nepattern-0.5.5/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.5/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.5/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.5/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.5/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.5/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.5/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-04-28 06:40:55.722197 nepattern-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.5/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.5/PKG-INFO
```

### Comparing `nepattern-0.5.4/LICENSE` & `nepattern-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/__init__.py` & `nepattern-0.5.5/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/base.py` & `nepattern-0.5.5/nepattern/base.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/context.py` & `nepattern-0.5.5/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/context.pyi` & `nepattern-0.5.5/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/core.py` & `nepattern-0.5.5/nepattern/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 from copy import deepcopy
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from enum import Enum, IntEnum
 from typing import Any, Callable, Generic, TypeVar, overload
 
 from tarina import Empty, generic_isinstance
 from tarina.lang import lang
 
 try:
@@ -19,15 +19,15 @@
 
 
 def _accept(
     input_: Any,
     patterns: list[BasePattern] | None = None,
     types: list[type] | None = None,
 ):
-    res_p = any(map(lambda x: x(input_).success, patterns)) if patterns else False
+    res_p = any(map(lambda x: x.exec(input_).success, patterns)) if patterns else False
     res_t = generic_isinstance(input_, tuple(types)) if types else False
     return res_t or res_p
 
 
 class MatchMode(IntEnum):
     """参数表达式匹配模式"""
 
@@ -54,19 +54,28 @@
 
 T = TypeVar("T")
 TOrigin = TypeVar("TOrigin")
 TVOrigin = TypeVar("TVOrigin")
 TDefault = TypeVar("TDefault")
 
 
-@dataclass
+@dataclass(init=False)
 class ValidateResult(Generic[TVOrigin]):
-    _value: TVOrigin | type[Empty] = field(default=Empty)
-    _error: Exception | type[Empty] = field(default=Empty)
-    flag: ResultFlag = field(default=ResultFlag.VALID)
+    """参数表达式验证结果"""
+    def __init__(
+        self,
+        value: TVOrigin | type[Empty] = Empty,
+        error: Exception | type[Empty] = Empty,
+        flag: ResultFlag = ResultFlag.VALID,
+    ):
+        self._value = value
+        self._error = error
+        self.flag = flag
+
+    __slots__ = ("_value", "_error", "flag")
 
     @property
     def value(self) -> TVOrigin:
         if self.flag == ResultFlag.ERROR or self._value == Empty:
             raise RuntimeError("cannot access value")
         return self._value  # type: ignore
 
@@ -103,14 +112,16 @@
     def step(
         self, other: type[T] | Callable[[TVOrigin], T] | Any | BasePattern[T]
     ) -> T | Self | ValidateResult[T]:
         if other is bool:
             return self.success  # type: ignore
         if callable(other) and self.success:
             return other(self.value)
+        if isinstance(other, BasePattern):
+            return other.exec(self.value)
         if self.success and hasattr(self.value, "__rshift__"):
             return self.value | other  # type: ignore
         return self
 
     @overload
     def __rshift__(self, other: type[T] | T) -> T:
         ...
@@ -296,15 +307,15 @@
 
     def match(self, input_: str | Any) -> TOrigin:
         """
         对传入的参数进行匹配, 如果匹配成功, 则返回转换后的值, 否则返回None
         """
         if (
             self.mode > 0
-            and self.origin not in (str, Any)
+            and self.origin is not str and self.origin is not Any
             and generic_isinstance(input_, self.origin)
         ):
             return input_  # type: ignore
         if (self.type_accepts or self.pattern_accepts) and not _accept(
             input_, self.pattern_accepts, self.type_accepts
         ):
             if not self.previous or not _accept(
@@ -313,43 +324,43 @@
                 self.type_accepts,
             ):  # pragma: no cover
                 raise MatchFailed(
                     lang.require("nepattern", "type_error").format(
                         target=input_.__class__
                     )
                 )
-        if self.mode == MatchMode.KEEP:
+        if self.mode == 0:
             return input_  # type: ignore
-        if self.mode == MatchMode.TYPE_CONVERT:
+        if self.mode == 2:
             res = self.converter(self, input_)
-            if res is None and self.origin == Any:  # pragma: no cover
+            if res is None and self.origin is Any:  # pragma: no cover
                 raise MatchFailed(
                     lang.require("nepattern", "content_error").format(target=input_)
                 )
             if not generic_isinstance(res, self.origin):
                 if not self.previous or not generic_isinstance(
                     res := self.converter(self, self.previous.match(input_)),
                     self.origin,
                 ):
                     raise MatchFailed(
                         lang.require("nepattern", "content_error").format(target=input_)
                     )
             return res
-        if not isinstance(input_, str):
+        if input_.__class__ is not str:
             if not self.previous or not isinstance(
                 input_ := self.previous.match(input_), str
             ):
                 raise MatchFailed(
                     lang.require("nepattern", "type_error").format(target=type(input_))
                 )
         if mat := self.regex_pattern.match(input_):
             glen = len(mat.groups())
             return (
                 self.converter(self, mat[1] if glen > 0 else mat[0])
-                if self.mode == MatchMode.REGEX_CONVERT
+                if self.mode == 3
                 else mat[1]
                 if glen > 0
                 else mat[0]
             )
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_)
         )
@@ -370,25 +381,24 @@
         """
         对传入的值进行正向验证，返回可能的匹配与转化结果。
 
         若传入默认值，验证失败会返回默认值
         """
         try:
             res = self.match(input_)
-            for i in self.validators:
-                if not i(res):
-                    raise MatchFailed(
-                        lang.require("nepattern", "content_error").format(target=input_)
-                    )
-            return ValidateResult(_value=res, flag=ResultFlag.VALID)
+            if self.validators and not all([i(res) for i in self.validators]):
+                raise MatchFailed(
+                    lang.require("nepattern", "content_error").format(target=input_)
+                )
+            return ValidateResult(value=res, flag=ResultFlag.VALID)
         except Exception as e:
             if default is None:
-                return ValidateResult(_error=e, flag=ResultFlag.ERROR)
+                return ValidateResult(error=e, flag=ResultFlag.ERROR)
             return ValidateResult(
-                _value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
+                value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
             )
 
     @overload
     def invalidate(self, input_: Any) -> ValidateResult[Any]:
         ...
 
     @overload
@@ -404,51 +414,51 @@
         对传入的值进行反向验证，返回可能的匹配与转化结果。
 
         若传入默认值，验证失败会返回默认值
         """
         try:
             res = self.match(input_)
         except MatchFailed:
-            return ValidateResult(_value=input_, flag=ResultFlag.VALID)
+            return ValidateResult(value=input_, flag=ResultFlag.VALID)
         else:
             for i in self.validators:
                 if not i(res):
-                    return ValidateResult(_value=input_, flag=ResultFlag.VALID)
+                    return ValidateResult(value=input_, flag=ResultFlag.VALID)
             if default is None:
                 return ValidateResult(
-                    _error=MatchFailed(
+                    error=MatchFailed(
                         lang.require("nepattern", "content_error").format(target=input_)
                     ),
                     flag=ResultFlag.ERROR,
                 )
             return ValidateResult(
-                _value=None if default is Empty else default, flag=ResultFlag.DEFAULT
+                value=None if default is Empty else default, flag=ResultFlag.DEFAULT
             )
 
     @overload
-    def __call__(self, input_: Any) -> ValidateResult[TOrigin]:
+    def exec(self, input_: Any) -> ValidateResult[TOrigin]:
         ...
 
     @overload
-    def __call__(
+    def exec(
         self, input_: Any, default: TDefault
     ) -> ValidateResult[TOrigin | TDefault]:
         ...
 
-    def __call__(self, input_: Any, default: TDefault | None = None) -> ValidateResult[TOrigin | TDefault | None]:  # type: ignore
+    def exec(self, input_: Any, default: TDefault | None = None) -> ValidateResult[TOrigin | TDefault | None]:  # type: ignore
         """
         依据 anti 值 自动选择验证方式
         """
         if self.anti:
             return self.invalidate(input_, default)
         else:
             return self.validate(input_, default)
 
     def __rrshift__(self, other):
-        return self.__call__(other)
+        return self.exec(other)
 
     def __rmatmul__(self, other) -> Self:  # pragma: no cover
         if isinstance(other, str):
             self.alias = other
         return self
 
     def __matmul__(self, other) -> Self:  # pragma: no cover
```

### Comparing `nepattern-0.5.4/nepattern/main.py` & `nepattern-0.5.5/nepattern/main.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/nepattern/util.py` & `nepattern-0.5.5/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/pyproject.toml` & `nepattern-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.5.4"
+version = "0.5.5"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.3.3",
```

### Comparing `nepattern-0.5.4/README.md` & `nepattern-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.4/PKG-INFO` & `nepattern-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.4
+Version: 0.5.5
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

