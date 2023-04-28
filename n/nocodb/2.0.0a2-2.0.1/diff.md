# Comparing `tmp/nocodb-2.0.0a2-py3-none-any.whl.zip` & `tmp/nocodb-2.0.1-py3.9.egg`

## zipinfo {}

```diff
@@ -1,22 +1,38 @@
-Zip file size: 12365 bytes, number of entries: 20
--rw-r--r--  2.0 unx       24 b- defN 23-Apr-27 20:52 nocodb/__init__.py
--rw-r--r--  2.0 unx     3068 b- defN 23-Apr-27 19:46 nocodb/api.py
--rw-r--r--  2.0 unx      400 b- defN 23-Apr-27 19:41 nocodb/exceptions.py
--rw-r--r--  2.0 unx      530 b- defN 23-Mar-04 12:21 nocodb/filters.py
--rw-r--r--  2.0 unx     4784 b- defN 23-Apr-27 19:46 nocodb/nocodb.py
--rw-r--r--  2.0 unx      185 b- defN 23-Mar-04 12:43 nocodb/utils.py
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-27 20:26 nocodb/filters/__init__.py
--rw-r--r--  2.0 unx      521 b- defN 23-Apr-27 20:03 nocodb/filters/factory.py
--rw-r--r--  2.0 unx      733 b- defN 23-Apr-27 20:03 nocodb/filters/factory_test.py
--rw-r--r--  2.0 unx     2405 b- defN 23-Apr-27 20:50 nocodb/filters/filters_test.py
--rw-r--r--  2.0 unx      806 b- defN 23-Apr-27 20:43 nocodb/filters/logical.py
--rw-r--r--  2.0 unx      516 b- defN 23-Apr-27 20:18 nocodb/filters/raw_filter.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-19 17:22 nocodb/infra/__init__.py
--rw-r--r--  2.0 unx     6143 b- defN 23-Apr-27 19:46 nocodb/infra/requests_client.py
--rw-r--r--  2.0 unx      687 b- defN 23-Apr-27 19:46 nocodb/infra/requests_client_test.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Apr-27 20:53 nocodb-2.0.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7285 b- defN 23-Apr-27 20:53 nocodb-2.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 20:53 nocodb-2.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-27 20:53 nocodb-2.0.0a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1585 b- defN 23-Apr-27 20:53 nocodb-2.0.0a2.dist-info/RECORD
-20 files, 31513 bytes uncompressed, 9787 bytes compressed:  68.9%
+Zip file size: 24810 bytes, number of entries: 36
+-rw-r--r--  2.0 unx     7282 b- defN 23-Apr-28 22:41 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      526 b- defN 23-Apr-28 22:41 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 22:41 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-28 22:41 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-28 22:41 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 22:41 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-28 22:40 nocodb/__init__.py
+-rw-r--r--  2.0 unx     3068 b- defN 23-Apr-27 21:46 nocodb/api.py
+-rw-r--r--  2.0 unx      400 b- defN 23-Apr-27 21:41 nocodb/exceptions.py
+-rw-r--r--  2.0 unx      530 b- defN 23-Mar-04 13:21 nocodb/filters.py
+-rw-r--r--  2.0 unx     4144 b- defN 23-Apr-27 23:48 nocodb/nocodb.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Mar-04 13:43 nocodb/utils.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Apr-28 22:41 nocodb/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     3143 b- defN 23-Apr-28 22:41 nocodb/__pycache__/api.cpython-39.pyc
+-rw-r--r--  2.0 unx      707 b- defN 23-Apr-28 22:41 nocodb/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--  2.0 unx     1175 b- defN 23-Apr-28 22:41 nocodb/__pycache__/filters.cpython-39.pyc
+-rw-r--r--  2.0 unx     5414 b- defN 23-Apr-28 22:41 nocodb/__pycache__/nocodb.cpython-39.pyc
+-rw-r--r--  2.0 unx      348 b- defN 23-Apr-28 22:41 nocodb/__pycache__/utils.cpython-39.pyc
+-rw-r--r--  2.0 unx      683 b- defN 23-Apr-27 23:48 nocodb/filters/__init__.py
+-rw-r--r--  2.0 unx      521 b- defN 23-Apr-27 23:48 nocodb/filters/factory.py
+-rw-r--r--  2.0 unx      733 b- defN 23-Apr-27 23:48 nocodb/filters/factory_test.py
+-rw-r--r--  2.0 unx     2405 b- defN 23-Apr-27 23:48 nocodb/filters/filters_test.py
+-rw-r--r--  2.0 unx      806 b- defN 23-Apr-27 23:48 nocodb/filters/logical.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Apr-27 23:48 nocodb/filters/raw_filter.py
+-rw-r--r--  2.0 unx      580 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     1227 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/factory.cpython-39.pyc
+-rw-r--r--  2.0 unx      855 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/factory_test.cpython-39.pyc
+-rw-r--r--  2.0 unx     2301 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/filters_test.cpython-39.pyc
+-rw-r--r--  2.0 unx     1867 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/logical.cpython-39.pyc
+-rw-r--r--  2.0 unx     1236 b- defN 23-Apr-28 22:41 nocodb/filters/__pycache__/raw_filter.cpython-39.pyc
+-rw-r--r--  2.0 unx        0 b- defN 22-Sep-19 19:22 nocodb/infra/__init__.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-Apr-27 21:46 nocodb/infra/requests_client.py
+-rw-r--r--  2.0 unx      687 b- defN 23-Apr-27 21:46 nocodb/infra/requests_client_test.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Apr-28 22:41 nocodb/infra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     6339 b- defN 23-Apr-28 22:41 nocodb/infra/__pycache__/requests_client.cpython-39.pyc
+-rw-r--r--  2.0 unx      877 b- defN 23-Apr-28 22:41 nocodb/infra/__pycache__/requests_client_test.cpython-39.pyc
+36 files, 55054 bytes uncompressed, 19664 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,7 +1,25 @@
+Filename: EGG-INFO/PKG-INFO
+Comment: 
+
+Filename: EGG-INFO/SOURCES.txt
+Comment: 
+
+Filename: EGG-INFO/dependency_links.txt
+Comment: 
+
+Filename: EGG-INFO/requires.txt
+Comment: 
+
+Filename: EGG-INFO/top_level.txt
+Comment: 
+
+Filename: EGG-INFO/zip-safe
+Comment: 
+
 Filename: nocodb/__init__.py
 Comment: 
 
 Filename: nocodb/api.py
 Comment: 
 
 Filename: nocodb/exceptions.py
@@ -12,14 +30,32 @@
 
 Filename: nocodb/nocodb.py
 Comment: 
 
 Filename: nocodb/utils.py
 Comment: 
 
+Filename: nocodb/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/__pycache__/api.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/__pycache__/exceptions.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/__pycache__/filters.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/__pycache__/nocodb.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/__pycache__/utils.cpython-39.pyc
+Comment: 
+
 Filename: nocodb/filters/__init__.py
 Comment: 
 
 Filename: nocodb/filters/factory.py
 Comment: 
 
 Filename: nocodb/filters/factory_test.py
@@ -30,32 +66,44 @@
 
 Filename: nocodb/filters/logical.py
 Comment: 
 
 Filename: nocodb/filters/raw_filter.py
 Comment: 
 
-Filename: nocodb/infra/__init__.py
+Filename: nocodb/filters/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
-Filename: nocodb/infra/requests_client.py
+Filename: nocodb/filters/__pycache__/factory.cpython-39.pyc
 Comment: 
 
-Filename: nocodb/infra/requests_client_test.py
+Filename: nocodb/filters/__pycache__/factory_test.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/filters/__pycache__/filters_test.cpython-39.pyc
 Comment: 
 
-Filename: nocodb-2.0.0a2.dist-info/LICENSE
+Filename: nocodb/filters/__pycache__/logical.cpython-39.pyc
 Comment: 
 
-Filename: nocodb-2.0.0a2.dist-info/METADATA
+Filename: nocodb/filters/__pycache__/raw_filter.cpython-39.pyc
+Comment: 
+
+Filename: nocodb/infra/__init__.py
+Comment: 
+
+Filename: nocodb/infra/requests_client.py
+Comment: 
+
+Filename: nocodb/infra/requests_client_test.py
 Comment: 
 
-Filename: nocodb-2.0.0a2.dist-info/WHEEL
+Filename: nocodb/infra/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
-Filename: nocodb-2.0.0a2.dist-info/top_level.txt
+Filename: nocodb/infra/__pycache__/requests_client.cpython-39.pyc
 Comment: 
 
-Filename: nocodb-2.0.0a2.dist-info/RECORD
+Filename: nocodb/infra/__pycache__/requests_client_test.cpython-39.pyc
 Comment: 
 
 Zip file comment:
```

## nocodb/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "2.0.0a2"
+__version__ = "2.0.1"
```

## nocodb/nocodb.py

```diff
@@ -50,37 +50,14 @@
 
 class WhereFilter(ABC):
     @abstractmethod
     def get_where(self) -> str:
         pass
 
 
-"""This could be great but actually I don't know how to join filters in the
-NocoDB DSL. I event don't know if this is possible through the current API.
-I hope they add docs about it soon.
-
-class NocoDBWhere:
-
-    def __init__(self):
-        self.__filter_array: List[WhereFilter] = []
-
-    def add_filter(self, where_filter: WhereFilter) -> NocoDBWhere:
-        self.__filter_array.append(
-                where_filter
-        )
-        return self
-
-    def get_where(self) -> str:
-        return '&'.join([filter_.get_where() for filter_ in self.__filter_array])
-
-    def __str__(self):
-        return f'Where: "{self.get_where()}"'
-"""
-
-
 class NocoDBProject:
     def __init__(self, org_name: str, project_name: str):
         self.project_name = project_name
         self.org_name = org_name
 
 
 class NocoDBClient:
```

## Comparing `nocodb-2.0.0a2.dist-info/METADATA` & `EGG-INFO/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nocodb
-Version: 2.0.0a2
+Version: 2.0.1
 Summary: A package to use NocoDB API in a simple way
 Home-page: https://github.com/ElChicoDePython/python-nocodb
 Author: Samuel López Saura
 Author-email: samuellopezsaura@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests (>=2.0)
 
 # NocoDB Python Client
 
 NocoDB is a great Airtable alternative. This client allows python developers
 to use NocoDB API in a simple way.
 
 ## Installation
@@ -26,15 +25,15 @@
 ```
 
 ## Usage
 
 ### Client configuration
 ```python
 from nocodb.nocodb import NocoDBProject, APIToken, JWTAuthToken
-from nocodb.filters import LikeFilter, EqFilter
+from nocodb.filters import LikeFilter, EqFilter, And
 from nocodb.infra.requests_client import NocoDBRequestsClient
 
 
 # Usage with API Token
 client = NocoDBRequestsClient(
         # Your API Token retrieved from NocoDB conf
         APIToken("YOUR-API-TOKEN"),
@@ -108,17 +107,16 @@
 # Retrieve the first 10000 rows
 table_rows = client.table_row_list(project, table_name, params={'limit': 10000})
 
 # Skip 100 rows
 table_rows = client.table_row_list(project, table_name, params={'offset': 100})
 
 # Filter the query
-# Currently only one filter at a time is allowed. I don't know how to join
-# multiple conditions in nocodb dsl. If you know how please let me know :).
 table_rows = client.table_row_list(project, table_name, LikeFilter("name", "%sam%"))
+table_rows = client.table_row_list(project, table_name, And(LikeFilter("name", "%sam%"), EqFilter("age", 26)))
 table_rows = client.table_row_list(project, table_name, filter_obj=EqFilter("Id", 100))
 
 # Filter and count rows
 count = client.table_count(project, table_name, filter_obj=EqFilter("Id", 100))
 
 # Find one row
 table_row = client.table_find_one(project, table_name, filter_obj=EqFilter("Id", 100), params={"sort": "-created_at"})
@@ -152,18 +150,45 @@
 - EqualFilter (Alias of EqFilter)
 - NotEqualFilter
 - GreaterThanFilter
 - GreaterOrEqualFilter
 - LessThanFilter
 - LessOrEqualFilter
 - LikeFilter
+- Or
+- Not
+- And
+
+#### Combining filters using Logical operations
+
+```python
+from nocodb import filters
+
+# Basic filters...
+nick_filter = filters.EqFilter("nickname", "elchicodepython")
+country_filter = filters.EqFilter("country", "es")
+girlfriend_code = filters.EqFilter("gfcode", "404")
+current_mood_code = filters.EqFilter("moodcode", "418")
+
+# Combining filters using logical filters
+or_filter = filters.Or(nick_filter, country_filter)
+and_filter = filters.And(girlfriend_code, current_mood_code)
+
+# Negating filters with a Not filter
+not_me = filters.Not(filters.EqFilter("nickname", "elchicodepython"))
+
+# You can also combine combinations
+or_combined_filter = filters.Or(or_filter, and_filter)
+and_combined_filter = filters.And(or_filter, and_filter)
+
+```
 
 ### Using custom filters
 
-Nocodb is evolving and new operators are comming with each release.
+Nocodb is evolving and new operators are coming with each release.
 
 Most of the basic operations are inside this package but you could need some new
 feature that could not be added yet.
 For those filters you can build your own.
 
 Example for basic filters:
 
@@ -197,35 +222,14 @@
 ExactDateOpFilter = raw_template_filter_class_factory('({},{op},exactDate,{})')
 
 table_rows = client.table_row_list(project, table_name, BirthdayDateFilter('2023-06-01'))
 table_rows = client.table_row_list(project, table_name, ExactDateEqFilter('column', '2023-06-01'))
 table_rows = client.table_row_list(project, table_name, ExactDateOpFilter('column', '2023-06-01', op='eq'))
 ```
 
-```python
-from nocodb import filters
-
-# Basic filters...
-nick_filter = filters.EqFilter("nickname", "elchicodepython")
-country_filter = filters.EqFilter("country", "es")
-girlfriend_code = filters.EqFilter("gfcode", "404")
-current_mood_code = filters.EqFilter("moodcode", "418")
-
-# Combining filters using logical filters
-or_filter = filters.Or(nick_filter, country_filter)
-and_filter = filters.And(girlfriend_code, current_mood_code)
-
-# Negating filters with a Not filter
-not_me = filters.Not(filters.EqFilter("nickname", "elchicodepython"))
-
-# You can also combine combinations
-or_combined_filter = filters.Or(or_filter, and_filter)
-and_combined_filter = filters.And(or_filter, and_filter)
-
-```
 
 Credits to @MitPitt for asking this feature.
 
 ## Author notes
 
 I created this package to bootstrap some personal projects and I hope it
 will help other developers from the python community. It's not completed but
```

