# Comparing `tmp/smartsheet-pydantic-1.3.0.tar.gz` & `tmp/smartsheet-pydantic-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.3.0.tar", last modified: Sun Apr 23 22:28:37 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.3.1.tar", last modified: Fri Apr 28 21:13:44 2023, max compression
```

## Comparing `smartsheet-pydantic-1.3.0.tar` & `smartsheet-pydantic-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/
--rw-r--r--   0 tak       (1000) tak       (1000)     1091 2023-04-22 15:28:56.000000 smartsheet-pydantic-1.3.0/LICENSE
--rw-r--r--   0 tak       (1000) tak       (1000)     8423 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)     6773 2023-04-23 22:26:10.000000 smartsheet-pydantic-1.3.0/README.md
--rw-r--r--   0 tak       (1000) tak       (1000)      811 2023-04-23 22:27:47.000000 smartsheet-pydantic-1.3.0/pyproject.toml
--rw-r--r--   0 tak       (1000) tak       (1000)       38 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/setup.cfg
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/src/
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/
--rw-r--r--   0 tak       (1000) tak       (1000)        0 2023-04-22 14:53:46.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/__init__.py
--rw-r--r--   0 tak       (1000) tak       (1000)     6740 2023-04-23 20:54:35.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)      493 2023-04-22 14:53:20.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/debug_logger.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2816 2023-04-22 15:44:48.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)    12396 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/smartmodels.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2309 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/sources.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2327 2023-04-22 15:45:13.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/transformer.py
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/
--rw-r--r--   0 tak       (1000) tak       (1000)     8423 2023-04-23 22:28:37.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)      622 2023-04-23 22:28:37.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 tak       (1000) tak       (1000)        1 2023-04-23 22:28:37.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 tak       (1000) tak       (1000)      102 2023-04-23 22:28:37.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/requires.txt
--rw-r--r--   0 tak       (1000) tak       (1000)       20 2023-04-23 22:28:37.000000 smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-23 22:28:37.275301 smartsheet-pydantic-1.3.0/tests/
--rw-r--r--   0 tak       (1000) tak       (1000)     4686 2023-04-23 20:47:34.000000 smartsheet-pydantic-1.3.0/tests/test_controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)     3527 2023-04-22 16:01:06.000000 smartsheet-pydantic-1.3.0/tests/test_filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)    13872 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.0/tests/test_smartmodel.py
--rw-r--r--   0 tak       (1000) tak       (1000)     1714 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.0/tests/test_sources.py
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/
+-rw-r--r--   0 tak       (1000) tak       (1000)     1091 2023-04-22 15:28:56.000000 smartsheet-pydantic-1.3.1/LICENSE
+-rw-r--r--   0 tak       (1000) tak       (1000)     8575 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/PKG-INFO
+-rw-r--r--   0 tak       (1000) tak       (1000)     6925 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/README.md
+-rw-r--r--   0 tak       (1000) tak       (1000)      811 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/pyproject.toml
+-rw-r--r--   0 tak       (1000) tak       (1000)       38 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/setup.cfg
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/
+-rw-r--r--   0 tak       (1000) tak       (1000)        0 2023-04-22 14:53:46.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/__init__.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     6740 2023-04-23 22:32:42.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/controller.py
+-rw-r--r--   0 tak       (1000) tak       (1000)      493 2023-04-22 14:53:20.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/debug_logger.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     2816 2023-04-22 15:44:48.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/filters.py
+-rw-r--r--   0 tak       (1000) tak       (1000)    12396 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/smartmodels.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     2309 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/sources.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     2329 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/transformer.py
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/
+-rw-r--r--   0 tak       (1000) tak       (1000)     8575 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 tak       (1000) tak       (1000)      622 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)        1 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)      102 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-r--r--   0 tak       (1000) tak       (1000)       20 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/tests/
+-rw-r--r--   0 tak       (1000) tak       (1000)     4686 2023-04-23 22:32:42.000000 smartsheet-pydantic-1.3.1/tests/test_controller.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     3527 2023-04-22 16:01:06.000000 smartsheet-pydantic-1.3.1/tests/test_filters.py
+-rw-r--r--   0 tak       (1000) tak       (1000)    13872 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.1/tests/test_smartmodel.py
+-rw-r--r--   0 tak       (1000) tak       (1000)     1714 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.1/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.3.0/LICENSE` & `smartsheet-pydantic-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/PKG-INFO` & `smartsheet-pydantic-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.3.0
+Version: 1.3.1
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -73,19 +73,41 @@
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
     source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
+## Defining a DataSource
+There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
+
+```python
+# DataSource class to call a RESTful API endpoint.
+class WeatherRestAPI(DataSourceAPI):
+    url = 'http://127.0.0.1:8000/weather_data'
+
+
+# DataSource class for PostgreSQL database
+class ExamplePostgres(DataSourcePostgres):
+    user: str          = "username"
+    password: str      = "password"
+    host: str          = "host name"
+    database: str      = "database name"
+    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
+    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
+```
+
+---
+
 
 ## Defining a SmartModel
 A __SmartModel__ class is an extension of Pydantic BaseModel. Therefore the definition of a __SmartModel__ is very similar. Define the data fields and their type as a class attribute.
 
 You will also need to define 2 additional Configuration parameters.
+1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
 from datetime import date
 
 
@@ -94,52 +116,29 @@
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-
-        unique_key: list[int] = ['index']
+        Source = WeatherRestAPI
+        unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
-
-
-## Defining a DataSource
-There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
-
-```python
-# DataSource class to call a RESTful API endpoint.
-class WeatherRestAPI(DataSourceAPI):
-    url = 'http://127.0.0.1:8000/weather_data'
-
-
-# DataSource class for PostgreSQL database
-class ExamplePostgres(DataSourcePostgres):
-    user: str          = "username"
-    password: str      = "password"
-    host: str          = "host name"
-    database: str      = "database name"
-    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
-    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
-```
-
----
-
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
 from smartsheet_pydantic import SmartsheetControllerFactory
 
-controller_factory = SmartsheetControllerFactory(sheet_detail)
-controller = controller_factory.get_controller()
+controller_factory = SmartsheetControllerFactory()
+controller = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
```

### Comparing `smartsheet-pydantic-1.3.0/README.md` & `smartsheet-pydantic-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,41 @@
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
     source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
+## Defining a DataSource
+There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
+
+```python
+# DataSource class to call a RESTful API endpoint.
+class WeatherRestAPI(DataSourceAPI):
+    url = 'http://127.0.0.1:8000/weather_data'
+
+
+# DataSource class for PostgreSQL database
+class ExamplePostgres(DataSourcePostgres):
+    user: str          = "username"
+    password: str      = "password"
+    host: str          = "host name"
+    database: str      = "database name"
+    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
+    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
+```
+
+---
+
 
 ## Defining a SmartModel
 A __SmartModel__ class is an extension of Pydantic BaseModel. Therefore the definition of a __SmartModel__ is very similar. Define the data fields and their type as a class attribute.
 
 You will also need to define 2 additional Configuration parameters.
+1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
 from datetime import date
 
 
@@ -71,52 +93,29 @@
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-
-        unique_key: list[int] = ['index']
+        Source = WeatherRestAPI
+        unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
-
-
-## Defining a DataSource
-There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
-
-```python
-# DataSource class to call a RESTful API endpoint.
-class WeatherRestAPI(DataSourceAPI):
-    url = 'http://127.0.0.1:8000/weather_data'
-
-
-# DataSource class for PostgreSQL database
-class ExamplePostgres(DataSourcePostgres):
-    user: str          = "username"
-    password: str      = "password"
-    host: str          = "host name"
-    database: str      = "database name"
-    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
-    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
-```
-
----
-
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
 from smartsheet_pydantic import SmartsheetControllerFactory
 
-controller_factory = SmartsheetControllerFactory(sheet_detail)
-controller = controller_factory.get_controller()
+controller_factory = SmartsheetControllerFactory()
+controller = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
```

### Comparing `smartsheet-pydantic-1.3.0/pyproject.toml` & `smartsheet-pydantic-1.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.3.0"
+version = "1.3.1"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/smartmodels.py` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/smartmodels.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/sources.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.source = source
         self.model = model
         self.filter = custom_filter()
 
     def fit(self, dataset) -> set[SmartModel]:
         initializer = dataset
         functions = [
-            self._apply_custom_filter,
+            # self._apply_custom_filter,
             self._smartmodel_fit,
         ]
         return reduce(lambda x, y: y(x), functions, initializer)
 
     def _apply_custom_filter(
                 self,
                 dataset: list[SourceType]
```

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.3.0
+Version: 1.3.1
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -73,19 +73,41 @@
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
     source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
+## Defining a DataSource
+There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
+
+```python
+# DataSource class to call a RESTful API endpoint.
+class WeatherRestAPI(DataSourceAPI):
+    url = 'http://127.0.0.1:8000/weather_data'
+
+
+# DataSource class for PostgreSQL database
+class ExamplePostgres(DataSourcePostgres):
+    user: str          = "username"
+    password: str      = "password"
+    host: str          = "host name"
+    database: str      = "database name"
+    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
+    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
+```
+
+---
+
 
 ## Defining a SmartModel
 A __SmartModel__ class is an extension of Pydantic BaseModel. Therefore the definition of a __SmartModel__ is very similar. Define the data fields and their type as a class attribute.
 
 You will also need to define 2 additional Configuration parameters.
+1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
 from datetime import date
 
 
@@ -94,52 +116,29 @@
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-
-        unique_key: list[int] = ['index']
+        Source = WeatherRestAPI
+        unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
-
-
-## Defining a DataSource
-There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
-
-```python
-# DataSource class to call a RESTful API endpoint.
-class WeatherRestAPI(DataSourceAPI):
-    url = 'http://127.0.0.1:8000/weather_data'
-
-
-# DataSource class for PostgreSQL database
-class ExamplePostgres(DataSourcePostgres):
-    user: str          = "username"
-    password: str      = "password"
-    host: str          = "host name"
-    database: str      = "database name"
-    query: str         = 'SELECT * FROM weather_table WHERE location = "USA"'
-    columns: list[str] = [ "index", "date", "temperature", "humidity", "rain" ]
-```
-
----
-
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
 from smartsheet_pydantic import SmartsheetControllerFactory
 
-controller_factory = SmartsheetControllerFactory(sheet_detail)
-controller = controller_factory.get_controller()
+controller_factory = SmartsheetControllerFactory()
+controller = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
```

### Comparing `smartsheet-pydantic-1.3.0/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/tests/test_controller.py` & `smartsheet-pydantic-1.3.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/tests/test_filters.py` & `smartsheet-pydantic-1.3.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/tests/test_smartmodel.py` & `smartsheet-pydantic-1.3.1/tests/test_smartmodel.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.0/tests/test_sources.py` & `smartsheet-pydantic-1.3.1/tests/test_sources.py`

 * *Files identical despite different names*

