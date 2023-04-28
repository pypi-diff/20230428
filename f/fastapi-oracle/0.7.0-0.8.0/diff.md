# Comparing `tmp/fastapi_oracle-0.7.0-py3-none-any.whl.zip` & `tmp/fastapi_oracle-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13319 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1412 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
+Zip file size: 13610 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
 -rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
 -rw-r--r--  2.0 unx      893 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
 -rw-r--r--  2.0 unx     8671 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
--rw-r--r--  2.0 unx     2088 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
+-rw-r--r--  2.0 unx     2202 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
 -rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 fastapi_oracle/pools.py
--rw-r--r--  2.0 unx     2004 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/RECORD
-11 files, 32999 bytes uncompressed, 11823 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     2711 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.8.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.8.0.dist-info/RECORD
+11 files, 33908 bytes uncompressed, 12114 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: fastapi_oracle/pools.py
 Comment: 
 
 Filename: fastapi_oracle/utils.py
 Comment: 
 
-Filename: fastapi_oracle-0.7.0.dist-info/LICENSE
+Filename: fastapi_oracle-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_oracle-0.7.0.dist-info/METADATA
+Filename: fastapi_oracle-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_oracle-0.7.0.dist-info/WHEEL
+Filename: fastapi_oracle-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_oracle-0.7.0.dist-info/RECORD
+Filename: fastapi_oracle-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_oracle/__init__.py

```diff
@@ -18,14 +18,15 @@
 )
 from .errors import (
     INTERMITTENT_DATABASE_ERROR_CLASSES,
     INTERMITTENT_DATABASE_ERROR_STRING_MAP,
     IntermittentDatabaseError,
     PackageStateInvalidatedError,
     ProgramUnitNotFoundError,
+    RecordAttributeCharacterEncodingError,
 )
 from .utils import (
     coll_records_as_dicts,
     cursor_rows_as_dicts,
     cursor_rows_as_gen,
     result_keys_to_lower,
     row_keys_to_lower,
@@ -40,14 +41,15 @@
     "PACKAGE_STATE_INVALIDATED_REGEX",
     "DbPoolAndConn",
     "DbPoolConnAndCursor",
     "DbPoolKey",
     "IntermittentDatabaseError",
     "PackageStateInvalidatedError",
     "ProgramUnitNotFoundError",
+    "RecordAttributeCharacterEncodingError",
     "Settings",
     "close_db_pools",
     "coll_records_as_dicts",
     "cursor_rows_as_dicts",
     "cursor_rows_as_gen",
     "get_db_conn",
     "get_db_cursor",
```

## fastapi_oracle/errors.py

```diff
@@ -12,14 +12,18 @@
     """Package state invalidated in PL/SQL."""
 
 
 class ProgramUnitNotFoundError(Exception):
     """Program unit not found in PL/SQL."""
 
 
+class RecordAttributeCharacterEncodingError(Exception):
+    """Character encoding error in record attribute."""
+
+
 # This list acts as a registry. Anything that wants more error classes treated as
 # intermittent database errors, adds to this list on app startup. So the entries that
 # are literally defined here, should only be considered the base set of entries, not the
 # complete set of entries. This list should also, therefore, be imported at the
 # function / method level, not at the module level, to be on the safe side that the
 # complete set of entries is getting imported.
 INTERMITTENT_DATABASE_ERROR_CLASSES: list[Type[Exception]] = [
```

## fastapi_oracle/utils.py

```diff
@@ -2,14 +2,15 @@
 from typing import Any, AsyncGenerator, Generator
 
 from cx_Oracle import Object
 from cx_Oracle_async.cursors import AsyncCursorWrapper
 from loguru import logger
 
 from fastapi_oracle.constants import DEFAULT_MAX_ROWS
+from fastapi_oracle.errors import RecordAttributeCharacterEncodingError
 
 
 def cursor_rows_as_dicts(cursor: AsyncCursorWrapper):
     """Make the specified cursor return its rows as dicts instead of tuples.
 
     This should be called after cursor.execute() and before cursor.fetchall().
 
@@ -36,18 +37,33 @@
         yield row
         i += 1
 
 
 def coll_records_as_dicts(coll: Object) -> Generator[dict[str, Any], None, None]:
     """Make the specified collection of records into simple dicts."""
     for record in coll.aslist():
-        item = {
-            type_attr.name: getattr(record, type_attr.name, None)
-            for type_attr in coll.type.element_type.attributes
-        }
+        item: dict[str, Any] = {}
+
+        for type_attr in coll.type.element_type.attributes:
+            attr_name = type_attr.name
+
+            try:
+                attr_value = getattr(record, type_attr.name, None)
+            except UnicodeDecodeError as ex1:
+                try:
+                    attr_value = ex1.object.decode("windows-1252")
+                except UnicodeDecodeError as ex2:
+                    raise RecordAttributeCharacterEncodingError(
+                        "Character encoding error in record attribute, tried decoding "
+                        "first to utf-8, then to windows-1252, both failed, error: "
+                        f"{ex2}, attribute: {attr_name}, value: {ex2.object!r}"
+                    )
+
+            item[f"{attr_name}"] = attr_value
+
         yield item
 
 
 def row_keys_to_lower(row: Mapping[str, Any]) -> dict[str, Any]:
     """Make the keys lowercase for the specified row."""
     return {k.lower(): v for k, v in row.items()}
```

## Comparing `fastapi_oracle-0.7.0.dist-info/LICENSE` & `fastapi_oracle-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_oracle-0.7.0.dist-info/METADATA` & `fastapi_oracle-0.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oracle
-Version: 0.7.0
+Version: 0.8.0
 Summary: Helpers for using the cx_Oracle_async library with the FastAPI framework.
 Home-page: https://github.com/Jaza/fastapi-oracle
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

