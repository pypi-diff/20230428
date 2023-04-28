# Comparing `tmp/mssql_dataframe-1.5.2rc3.tar.gz` & `tmp/mssql_dataframe-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mssql_dataframe-1.5.2rc3.tar", last modified: Mon Mar  7 14:06:37 2022, max compression
+gzip compressed data, was "mssql_dataframe-2.0.0.tar", last modified: Fri Apr 28 18:25:52 2023, max compression
```

## Comparing `mssql_dataframe-1.5.2rc3.tar` & `mssql_dataframe-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-03-07 14:06:37.421364 mssql_dataframe-1.5.2rc3/
--rw-rw-rw-   0        0        0     1086 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/LICENSE
--rw-rw-rw-   0        0        0       42 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/MANIFEST.in
--rw-rw-rw-   0        0        0     5084 2022-03-07 14:06:37.421364 mssql_dataframe-1.5.2rc3/PKG-INFO
--rw-rw-rw-   0        0        0     4289 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/README.md
--rw-rw-rw-   0        0        0        8 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/VERSION
-drwxrwxrwx   0        0        0        0 2022-03-07 14:06:37.404370 mssql_dataframe-1.5.2rc3/mssql_dataframe/
--rw-rw-rw-   0        0        0      325 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/__init__.py
--rw-rw-rw-   0        0        0     1922 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/__sample__.py
--rw-rw-rw-   0        0        0     3839 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/connect.py
-drwxrwxrwx   0        0        0        0 2022-03-07 14:06:37.416526 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/
--rw-rw-rw-   0        0        0       28 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/__init__.py
--rw-rw-rw-   0        0        0    24032 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/conversion.py
--rw-rw-rw-   0        0        0     3964 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/conversion_rules.py
--rw-rw-rw-   0        0        0    13198 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/create.py
--rw-rw-rw-   0        0        0     1486 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/custom_errors.py
--rw-rw-rw-   0        0        0     5937 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/dynamic.py
--rw-rw-rw-   0        0        0    12001 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/infer.py
--rw-rw-rw-   0        0        0     8190 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/modify.py
--rw-rw-rw-   0        0        0     5452 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/read.py
-drwxrwxrwx   0        0        0        0 2022-03-07 14:06:37.420344 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/
--rw-rw-rw-   0        0        0       56 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/__init__.py
--rw-rw-rw-   0        0        0     8407 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/_exceptions.py
--rw-rw-rw-   0        0        0     9282 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/insert.py
--rw-rw-rw-   0        0        0    10874 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/merge.py
--rw-rw-rw-   0        0        0     6344 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/update.py
--rw-rw-rw-   0        0        0     1463 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/write.py
--rw-rw-rw-   0        0        0     5353 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe/package.py
-drwxrwxrwx   0        0        0        0 2022-03-07 14:06:37.409354 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/
--rw-rw-rw-   0        0        0     5084 2022-03-07 14:06:37.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      895 2022-03-07 14:06:37.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-07 14:06:37.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-03-07 14:06:37.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-03-07 14:06:37.000000 mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2022-03-07 14:03:25.000000 mssql_dataframe-1.5.2rc3/pyproject.toml
--rw-rw-rw-   0        0        0     1056 2022-03-07 14:06:37.422354 mssql_dataframe-1.5.2rc3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 18:25:52.832287 mssql_dataframe-2.0.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6563 2023-04-28 18:25:52.832287 mssql_dataframe-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5812 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/README.md
+-rw-rw-rw-   0        0        0        5 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/VERSION
+drwxrwxrwx   0        0        0        0 2023-04-28 18:25:52.816670 mssql_dataframe-2.0.0/mssql_dataframe/
+-rw-rw-rw-   0        0        0      398 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/__equality__.py
+-rw-rw-rw-   0        0        0      325 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/__init__.py
+-rw-rw-rw-   0        0        0     3837 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:25:52.832287 mssql_dataframe-2.0.0/mssql_dataframe/core/
+-rw-rw-rw-   0        0        0       28 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/__init__.py
+-rw-rw-rw-   0        0        0    33327 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/conversion.py
+-rw-rw-rw-   0        0        0     5064 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/conversion_rules.py
+-rw-rw-rw-   0        0        0     8136 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/create.py
+-rw-rw-rw-   0        0        0     1620 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/custom_errors.py
+-rw-rw-rw-   0        0        0     5937 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/dynamic.py
+-rw-rw-rw-   0        0        0     8190 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/modify.py
+-rw-rw-rw-   0        0        0     5758 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/read.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:25:52.832287 mssql_dataframe-2.0.0/mssql_dataframe/core/write/
+-rw-rw-rw-   0        0        0       56 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/__init__.py
+-rw-rw-rw-   0        0        0     1496 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/_exceptions.py
+-rw-rw-rw-   0        0        0    10226 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/insert.py
+-rw-rw-rw-   0        0        0    10999 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/merge.py
+-rw-rw-rw-   0        0        0     6568 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/update.py
+-rw-rw-rw-   0        0        0     1072 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/core/write/write.py
+-rw-rw-rw-   0        0        0     4500 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/mssql_dataframe/package.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:25:52.816670 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/
+-rw-rw-rw-   0        0        0     6563 2023-04-28 18:25:52.000000 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2023-04-28 18:25:52.000000 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:25:52.000000 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-28 18:25:52.000000 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-28 18:25:52.000000 mssql_dataframe-2.0.0/mssql_dataframe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      163 2023-04-28 18:22:44.000000 mssql_dataframe-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1117 2023-04-28 18:25:52.832287 mssql_dataframe-2.0.0/setup.cfg
```

### Comparing `mssql_dataframe-1.5.2rc3/LICENSE` & `mssql_dataframe-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-1.5.2rc3/README.md` & `mssql_dataframe-2.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -25,76 +25,132 @@
 ``` python
 import env
 import pandas as pd
 from mssql_dataframe import SQLServer
 
 # connect to database using pyodbc
 sql = SQLServer(database=env.database, server=env.server)
-
-# create a demonstration dataframe
-df = pd.DataFrame({
-    'ColumnA': ['1','2','3','4','5'],
-    'ColumnB': ['a  .','b!','  c','d','e'],
-}, index=pd.Index([0, 1, 2, 3, 4], name='PK'))
-
-# create the table using a dataframe
-df = sql.create.table_from_dataframe(
-    table_name='##mssql_dataframe_readme',
-    dataframe = df,
-    primary_key = 'index'
-)
 ```
 
 ## Update
 
 Records in an SQL table are updated by simply providing a dataframe. By default a match on the SQL table's primary key is required for a record to be updated.
 
 ```python
-# update records for index 0 & 1
+# create demo SQL table
+df = sql.create.table(
+    table_name = '##mssql_update',
+    columns = {'Column1': 'VARCHAR(10)', 'Column2': 'TINYINT', 'PK': 'CHAR(1)'},
+    primary_key_column = 'PK'
+)
+
+# create a demo dataframe
+df = pd.DataFrame({
+    'Column1': ['A_Initial', 'B_Initial'],
+    'Column2': [1, 2],
+}, index=pd.Index(['A', 'B'], name='PK'))
+
+# perform an initial insert
+sql.write.insert('##mssql_update', df)
+
+# update records
 update_df = pd.DataFrame({
-        'ColumnA': ['11','22'],
-        'ColumnB': ['A','B'],
-}, index=pd.Index([0, 1], name='PK'))
+        'Column1': ['A_Updated'],
+}, index=pd.Index(['A'], name='PK'))
 # update data in the SQL table
-update_df = sql.write.update('##mssql_dataframe_readme', update_df)
+update_df = sql.write.update('##mssql_update', update_df)
+
+# validate the result
+result = sql.read.table('##mssql_update')
+assert result.at['A', 'Column1'] == 'A_Updated'
+assert result.at['A', 'Column2'] == 1
+assert result.at['B', 'Column1'] == 'B_Initial'
+assert result.at['B', 'Column2'] == 2
 ```
 
 ## Merge
 
 Records can be inserted/updated/deleted by providing a dataframe to the merge method. Again the primary key in the SQL table is used by default.
 
 1. dataframe column value doesn't match SQL column value -> insert record into SQL
 2. dataframe column value matches SQL column value -> update record in SQL
 3. SQL column value not in dataframe column -> delete record in SQL
 
 ```python
-# update existing record for index 0
-# insert new record for index 5
-# delete missing records for index 1,2,3,4
-merge_df = pd.DataFrame({
-        'ColumnA': ['11','6'],
-        'ColumnB': ['aa','f'],
-}, index=pd.Index([0, 6], name='PK'))
-# merge data in the SQL table
-merged_df = sql.write.merge('##mssql_dataframe_readme', merge_df)
+# create demo SQL table
+df = sql.create.table(
+    table_name = '##mssql_merge',
+    columns = {'Column1': 'VARCHAR(10)', 'Column2': 'TINYINT', 'PK': 'CHAR(1)'},
+    primary_key_column = 'PK'
+)
+
+# create a demo dataframe
+df = pd.DataFrame({
+    'Column1': ['A_Initial', 'B_Initial'],
+    'Column2': [1, 2],
+}, index=pd.Index(['A', 'B'], name='PK'))
+
+# perform an initial insert
+sql.write.insert('##mssql_merge', df)
+
+# perform merge
+sql.write.merge(
+        '##mssql_merge',
+        pd.DataFrame.from_records([
+                {'Column1': 'C_New', 'Column2': 3, 'PK': 'C'},
+                {'Column1': 'B_Updated', 'Column2': 0, 'PK': 'B'},
+        ]).set_index('PK')
+)
+
+# validate the results
+result = sql.read.table('##mssql_merge')
+assert 'A' not in result.index
+assert result.at['C', 'Column1'] == 'C_New'
+assert result.at['B', 'Column1'] == 'B_Updated'
+assert result.at['B', 'Column2'] == 0
 ```
 
 ## Upsert
 
 The merge method can be restricted to not delete records in SQL by specifying the upsert flag. Records in SQL are then only inserted or updated.
 
 ```python
-# update existing record for index 0
-# insert new record for index 7
-# records not in the dataframe but in SQL won't be deleted
-upsert_df = pd.DataFrame({
-        'ColumnA': ['11','7'],
-        'ColumnB': ['AA','g'],
-}, index=pd.Index([0, 7], name='PK'))
-sql.write.merge('##mssql_dataframe_readme', upsert_df, upsert=True)
+# create demo SQL table
+df = sql.create.table(
+    table_name = '##mssql_upsert',
+    columns = {'Column1': 'VARCHAR(10)', 'Column2': 'TINYINT', 'PK': 'CHAR(1)'},
+    primary_key_column = 'PK'
+)
+
+# create a demo dataframe
+df = pd.DataFrame({
+    'Column1': ['A_Initial', 'B_Initial'],
+    'Column2': [1, 2],
+}, index=pd.Index(['A', 'B'], name='PK'))
+
+# perform an initial insert
+sql.write.insert('##mssql_upsert', df)
+
+# perform upsert
+sql.write.merge(
+        '##mssql_upsert',
+        pd.DataFrame.from_records([
+                {'Column1': 'C_New', 'Column2': 3, 'PK': 'C'},
+                {'Column1': 'B_Updated', 'Column2': 0, 'PK': 'B'},
+        ]).set_index('PK'),
+        upsert = True
+)
+
+# validate the results
+result = sql.read.table('##mssql_upsert')
+assert result.at['A', 'Column1'] == 'A_Initial'
+assert result.at['A', 'Column2'] == 1
+assert result.at['C', 'Column1'] == 'C_New'
+assert result.at['B', 'Column1'] == 'B_Updated'
+assert result.at['B', 'Column2'] == 0
 ```
 
 ## Installation
 
 ```cmd
 pip install mssql-dataframe
 ```
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/connect.py` & `mssql_dataframe-2.0.0/mssql_dataframe/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         self,
         database: str = "master",
         server: str = "localhost",
         driver: str = None,
         username: str = None,
         password: str = None,
     ):
-
         driver, drivers_installed = self._get_driver(driver)
         self.connection_spec = {
             "database": database,
             "server": server,
             "driver": driver,
             "drivers_installed": drivers_installed,
         }
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/conversion.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions for data movement between Python pandas dataframes and SQL."""
 import struct
 from typing import Tuple, List
 import logging
+import pytz
 
 import pyodbc
 import numpy as np
 import pandas as pd
 
 from mssql_dataframe.core import (
     custom_errors,
@@ -44,15 +45,15 @@
 
     # add cataglog for temporary tables
     try:
         schema_name, table_name = table_name.split(".")
     except ValueError as err:
         if err.args[0].startswith("not enough values to unpack"):
             schema_name = None
-        else:
+        else:  # pragma: no cover
             raise
     if table_name.startswith("#"):
         catalog = "tempdb"
     else:
         catalog = None
 
     # get schema
@@ -91,22 +92,24 @@
     # format schema
     schema = schema.rename(columns={"type_name": "sql_type"})
     schema = schema[
         [
             "column_name",
             "data_type",
             "column_size",
+            "decimal_digits",
             "sql_type",
             "is_nullable",
             "ss_is_identity",
         ]
     ]
     schema[["column_name", "sql_type"]] = schema[["column_name", "sql_type"]].astype(
         "string"
     )
+    schema["decimal_digits"] = schema["decimal_digits"].fillna(0).astype("int64")
     schema["is_nullable"] = schema["is_nullable"] == "YES"
     schema["ss_is_identity"] = schema["ss_is_identity"] == 1
 
     # add primary key info
     pk = cursor.primaryKeys(table=table_name, catalog=catalog).fetchall()
     pk = pd.DataFrame([list(x) for x in pk], columns=[x[0] for x in cursor.description])
     pk = pk.rename(columns={"key_seq": "pk_seq"})
@@ -164,83 +167,154 @@
     if any(index):
         dataframe = dataframe.reset_index()
 
     # only apply to columns in dataframe
     schema = schema[schema.index.isin(dataframe.columns)].copy()
 
     # convert objects to the largest sql_category type to allow for size check
+    dataframe = convert_largest_sql_category(dataframe, schema)
+
+    # check for insufficient column size, using min and max of dataframe contents
+    check_column_size(dataframe, schema)
+
+    # check if unicode to a nonunicode type
+    check_unicode(dataframe, schema)
+
+    # convert dataframe based on SQL type
+    try:
+        dataframe = dataframe.astype(schema["pandas_type"].to_dict())
+    except TypeError:  # pragma: no cover
+        raise custom_errors.DataframeColumnInvalidValue(
+            "Dataframe columns cannot be converted based on their SQL data type"
+        )
+
+    # set primary key column as dataframe's index
+    if any(schema["pk_seq"].notna()):
+        pk = schema["pk_seq"].sort_values()
+        pk = list(pk[pk.notna()].index)
+        dataframe = dataframe.set_index(keys=pk)
+
+    return dataframe
+
+
+def convert_largest_sql_category(dataframe, schema):
+    """Convert objects to allow for comparison without truncation."""
     # avoids downcast such as UInt8 value of 10000 to 16
     convert = dataframe.columns[dataframe.dtypes == "object"]
     try:
-        # exact numeric
-        columns = convert[schema.loc[convert, "sql_category"] == "exact numeric"]
+        # exact_whole_numeric
+        columns = convert[schema.loc[convert, "sql_category"] == "exact_whole_numeric"]
         # BUG: first convert to float after replacing pandas.NA
         # https://github.com/pandas-dev/pandas/issues/25472
         dataframe[columns] = dataframe[columns].fillna(np.nan).replace([np.nan], [None])
         dataframe[columns] = dataframe[columns].astype("float")
         dataframe[columns] = dataframe[columns].astype("Int64")
-        # approximate numeric
-        columns = convert[schema.loc[convert, "sql_category"] == "approximate numeric"]
+        # approximate_decimal_numeric
+        columns = convert[
+            schema.loc[convert, "sql_category"] == "approximate_decimal_numeric"
+        ]
         dataframe[columns] = dataframe[columns].astype("float64")
-        # date time
-        columns = convert[schema.loc[convert, "sql_category"] == "date time"]
-        dataframe[columns] = dataframe[columns].astype("datetime64")
+        # date_time
+        columns = convert[
+            (schema.loc[convert, "sql_category"] == "date_time")
+            & (schema.loc[convert, "sql_type"] != "datetimeoffset")
+        ]
+        dataframe[columns] = dataframe[columns].astype("datetime64[ns]")
+        # datetime offset
+        columns = convert[
+            (schema.loc[convert, "sql_category"] == "date_time")
+            & (schema.loc[convert, "sql_type"] == "datetimeoffset")
+        ]
+        for col in columns:
+            dataframe[col] = dataframe[col].apply(lambda x: pd.Timestamp(x))
         # character string
         columns = convert[schema.loc[convert, "sql_category"] == "character string"]
         dataframe[columns] = dataframe[columns].astype("string")
-    except (TypeError, ValueError):
+    except (TypeError, ValueError):  # pragma: no cover
         raise custom_errors.DataframeColumnInvalidValue(
             "Dataframe columns cannot be converted based on their SQL data type",
             list(columns),
         )
 
-    # check for insufficient column size, using min and max of dataframe contents
+    return dataframe
+
+
+def check_column_size(dataframe, schema):
+    """Raise exception if dataframe value is too large for SQL data type specification."""
     check = dataframe.copy()
     strings = check.columns[check.dtypes == "string"]
     if any(strings):
         schema.loc[strings, "max_value"] = schema.loc[strings, "column_size"]
         check[strings] = check[strings].apply(lambda x: x.str.len())
-    check = check.agg([min, max]).transpose()
+    datetimeoffset = schema.index[schema["sql_type"] == "datetimeoffset"]
+    standard = check.drop(columns=datetimeoffset)
+    if len(standard.columns) == 0:  # pragma: no cover
+        check = pd.DataFrame(columns=["min", "max"])
+    else:
+        check = standard.agg([min, max]).transpose()
+    # calculate min/max for object pd.Timestamp seperately
+    for col in datetimeoffset:
+        check = pd.concat(
+            [
+                check,
+                pd.DataFrame(
+                    {"min": min(dataframe[col]), "max": max(dataframe[col])},
+                    index=[col],
+                ),
+            ]
+        )
     check = check.merge(
         schema[["min_value", "max_value"]], left_index=True, right_index=True
     )
     try:
         invalid = check[
             (check["min"] < check["min_value"]) | (check["max"] > check["max_value"])
         ]
-    except TypeError:
+    except TypeError:  # pragma: no cover
         raise custom_errors.DataframeColumnInvalidValue(
             "Dataframe columns cannot be converted based on their SQL data type"
         )
 
     if len(invalid) > 0:
         invalid = invalid.astype("string")
         invalid["allowed"] = invalid["min_value"] + " to " + invalid["max_value"]
         invalid["actual"] = invalid["min"] + " to " + invalid["max"]
         columns = list(invalid.index)
         raise custom_errors.SQLInsufficientColumnSize(
             f"columns: {columns}, allowed range: {list(invalid.allowed)}, actual range: {list(invalid.actual)}",
             columns,
         )
 
-    # convert dataframe based on SQL type
-    try:
-        dataframe = dataframe.astype(schema["pandas_type"].to_dict())
-    except TypeError:
-        raise custom_errors.DataframeColumnInvalidValue(
-            "Dataframe columns cannot be converted based on their SQL data type"
-        )
 
-    # set primary key column as dataframe's index
-    if any(schema["pk_seq"].notna()):
-        pk = schema["pk_seq"].sort_values()
-        pk = list(pk[pk.notna()].index)
-        dataframe = dataframe.set_index(keys=pk)
+def contains_unicode(series: pd.Series):
+    """Determine if a string contains unicode.
 
-    return dataframe
+    Parameters
+    ----------
+    series (pandas.Series) : data to check
+
+    Return
+    ------
+    check (bool) : True if series contains unicode
+
+    """
+    pre = series.str.len()
+    post = series.str.encode("ascii", errors="ignore").str.len().astype("Int64")
+    # check if encodidng removes characeters
+    check = pre.ne(post).any()
+
+    return check
+
+
+def check_unicode(dataframe, schema):
+    """Raise error if string contains unicode for SQL char/varchar column."""
+    columns = schema[schema["sql_type"].isin(["char", "varchar"])].index
+    for col in columns:
+        if contains_unicode(dataframe[col]):
+            raise custom_errors.SQLNonUnicodeTypeColumn
 
 
 def prepare_cursor(
     schema: pd.DataFrame, dataframe: pd.DataFrame, cursor: pyodbc.connect
 ) -> pyodbc.connect:
     """Prepare cursor data types and size for writting values to SQL.
 
@@ -253,131 +327,62 @@
     Returns
     -------
     cursor (pyodbc.connect.cursor) : cursor with SQL data type and size parameters set
     """
     schema = schema[
         [
             "column_size",
+            "decimal_digits",
             "min_value",
             "max_value",
+            "sql_category",
             "sql_type",
             "odbc_type",
-            "odbc_size",
-            "odbc_precision",
         ]
     ]
 
     # insure columns are sorted correctly
     columns = list(dataframe.columns)
     index = dataframe.index.names
     if any(index):
         columns = list(index) + columns
     schema = schema.loc[columns]
 
-    # use dataframe contents to determine size for strings
-    schema, _ = sql_spec(schema, dataframe)
-
     # set SQL data type and size for cursor
-    schema = schema[["odbc_type", "odbc_size", "odbc_precision"]].to_numpy().tolist()
+    schema = schema[["odbc_type", "column_size", "decimal_digits"]].to_numpy().tolist()
     schema = [tuple(x) for x in schema]
     cursor.setinputsizes(schema)
 
     return cursor
 
 
-def sql_spec(
-    schema: pd.DataFrame, dataframe: pd.DataFrame
-) -> Tuple[pd.DataFrame, dict]:
-    """Generate dictionary mapping of column name to SQL data type.
-
-    Data type includes the size of VARCHAR and NVARCHAR columns using dataframe contents.
+def prepare_time(schema, prepped, dataframe):
+    """Prepare time for writting to SQL."""
+    dtype = schema[schema["sql_type"] == "time"].index
 
-    Parameters
-    ----------
-    schema (pandas.DataFrame) : contains the column size to update and the column sql to identify string columns
-    dataframe (pandas.DataFrame) : dataframe contents
-
-    Returns
-    -------
-    schema (pandas.DataFrame) : column 'odbc_size' set according to size of contents for string columns
-    dtypes (dict) : dictionary mapping of each column SQL data type
-    """
-    if any(dataframe.index.names):
-        dataframe = dataframe.reset_index()
-
-    strings = schema[schema["sql_type"].isin(["varchar", "nvarchar"])].index
-
-    # update odbc_size in schema
-    if any(strings):
-        infer = dataframe[strings].apply(lambda x: x.str.len()).max()
-        infer = pd.DataFrame(infer, columns=["odbc_size"])
-        infer["odbc_size"] = infer["odbc_size"].fillna(1)
-        schema.update(infer)
-    schema["odbc_size"] = schema["odbc_size"].astype("int64")
-
-    # develop dictionary mapping of data types
-    dtypes = schema.loc[:, ["sql_type", "odbc_size"]]
-    dtypes["odbc_size"] = dtypes["odbc_size"].astype("string")
-    dtypes.loc[strings, "sql_type"] = (
-        dtypes.loc[strings, "sql_type"] + "(" + dtypes.loc[strings, "odbc_size"] + ")"
-    )
-    dtypes = dtypes["sql_type"].to_dict()
-
-    return schema, dtypes
-
-
-def prepare_values(
-    schema: pd.DataFrame, dataframe: pd.DataFrame
-) -> Tuple[pd.DataFrame, list]:
-    """Prepare dataframe contents for writting values to SQL.
-
-    Parameters
-    ----------
-    schema (pandas.DataFrame) : data schema definition
-    dataframe (pandas.DataFrame) : dataframe that will be written to SQL
-
-    Returns
-    -------
-    dataframe (pandas.DataFrame) : values that may be altered to conform to SQL precision limitations
-    values (list) : values to pass to pyodbc.connect.cursor.executemany
-
-    """
-    # create a copy to preserve values in return
-    prepped = dataframe.copy()
-
-    # include index as column as it is the primary key
-    if any(prepped.index.names):
-        prepped = prepped.reset_index()
-
-    # only prepare values currently in dataframe
-    schema = schema[schema.index.isin(prepped.columns)]
-
-    # SQL data type TIME as string since python datetime.time allows 6 decimal places but SQL allows 7
-    dtype = schema[schema["odbc_type"] == pyodbc.SQL_SS_TIME2].index
-    # check for valid range in SQL
     invalid = (
         (prepped[dtype] >= pd.Timedelta(days=1))
         | (prepped[dtype] < pd.Timedelta(days=0))
     ).any()
     if any(invalid):
         invalid = list(invalid[invalid].index)
         raise ValueError(
             f"columns {invalid} are out of range for SQL TIME data type. Allowable range is 00:00:00.0000000-23:59:59.9999999"
         )
-    # round and truncate if needed
+
     if any(dtype):
         truncation = prepped[dtype].apply(lambda x: any(x.dt.nanoseconds % 100 > 0))
+        truncation = list(truncation[truncation].index)
     else:
         truncation = []
     if any(truncation):
-        truncation = list(truncation[truncation].index)
         msg = f"Nanosecond precision for dataframe columns {truncation} will be rounded as SQL data type 'time' allows 7 max decimal places."
         logger.warning(msg)
-    # round nanosecond to the 7th decimal place ...123456789 -> ...123456800
-    for col in dtype:
+    # round nanosecond to the 7th decimal place ...123456789 -> ...123456800 for SQL
+    for col in truncation:
         rounded = dataframe[col].apply(
             lambda x: pd.Timedelta(
                 days=x.components.days,
                 hours=x.components.hours,
                 minutes=x.components.minutes,
                 seconds=x.components.seconds,
                 microseconds=x.components.microseconds,
@@ -385,52 +390,216 @@
             )
             if pd.notnull(x)
             else x
         )
         dataframe[col] = rounded
         prepped[col] = rounded
     if any(dtype):
+        # convert to string since python datetime.time allows 6 decimal places but SQL allows 7
         prepped[dtype] = prepped[dtype].astype("str")
         prepped[dtype] = prepped[dtype].replace({"NaT": None})
         prepped[dtype] = prepped[dtype].apply(lambda x: x.str[7:23])
 
-    # SQL data type DATETIME2 as string since python datetime.datetime allows 6 decimals but SQL allows 7
-    dtype = schema[schema["odbc_type"] == pyodbc.SQL_TYPE_TIMESTAMP].index
-    # round and truncate if needed
+    return prepped, dataframe
+
+
+def prepare_datetime(schema, prepped, dataframe):
+    """Prepare datetime for writting to SQL."""
+    dtype = schema[schema["sql_type"] == "datetime"].index
+    if any(dtype):
+        adjust = prepped[dtype].apply(lambda x: any(x.dt.microsecond % 3000 > 0))
+    else:
+        adjust = []
+    if any(adjust):
+        adjust = list(adjust[adjust].index)
+        msg = f"Millisecond precision for dataframe columns {adjust} will be rounded as SQL data type 'datetime' rounds to increments of .000, .003, or .007 seconds."
+        logger.warning(msg)
+        # round millisecond to the 3rd decimal place in approriate increments ...008 -> ..007 for SQL
+        increments = np.array([10, 7, 3, 0]).reshape(-1, 1)
+        for col in adjust:
+            thousandths = (
+                (prepped[col].dt.microsecond / 1000 % 10).to_numpy().reshape(1, -1)
+            )
+            thousandths = increments[np.abs(thousandths - increments).argmin(axis=0)]
+
+            milliseconds = prepped[col].dt.microsecond // 10000 * 10 + pd.Series(
+                thousandths[:, 0], index=prepped.index
+            )
+            milliseconds = pd.to_timedelta(milliseconds, unit="milliseconds")
+
+            rounded = dataframe[col].dt.floor("s") + milliseconds
+
+            dataframe[col] = rounded
+            prepped[col] = rounded
+
+    if any(dtype):
+        # convert to string since python datetime.datetime allows 6 decimals but SQL allows 7
+        prepped[dtype] = prepped[dtype].astype("str")
+        prepped[dtype] = prepped[dtype].replace({"NaT": None})
+        prepped[dtype] = prepped[dtype].apply(lambda x: x.str[0:27])
+
+    return prepped, dataframe
+
+
+def prepare_datetime2(schema, prepped, dataframe):
+    """Prepare datetime2 for writting to SQL."""
+    dtype = schema[schema["sql_type"] == "datetime2"].index
+
     if any(dtype):
         truncation = prepped[dtype].apply(lambda x: any(x.dt.nanosecond % 100 > 0))
     else:
         truncation = []
     if any(truncation):
         truncation = list(truncation[truncation].index)
         msg = f"Nanosecond precision for dataframe columns {truncation} will be rounded as SQL data type 'datetime2' allows 7 max decimal places."
         logger.warning(msg)
-        # round nanosecond to the 7th decimal place ...145224193 -> ...145224200
-        for col in dtype:
+        # round nanosecond to the 7th decimal place ...145224193 -> ...145224200 for SQL
+        for col in truncation:
             rounded = dataframe[col].apply(
                 lambda x: pd.Timestamp(
                     x.year,
                     x.month,
                     x.day,
                     x.hour,
                     x.minute,
                     x.second,
                     x.microsecond,
                     round(x.nanosecond / 100) * 100,
                 )
                 if pd.notnull(x)
                 else x
             )
+            rounded = rounded.astype("datetime64[ns]")
             dataframe[col] = rounded
             prepped[col] = rounded
     if any(dtype):
+        # convret to string since python datetime.datetime allows 6 decimals but SQL allows 7
         prepped[dtype] = prepped[dtype].astype("str")
         prepped[dtype] = prepped[dtype].replace({"NaT": None})
         prepped[dtype] = prepped[dtype].apply(lambda x: x.str[0:27])
 
+    return prepped, dataframe
+
+
+def prepare_datetimeoffset(schema, prepped, dataframe):
+    """Prepare datetimeoffset for writing to SQL."""
+    dtype = schema[schema["sql_type"] == "datetimeoffset"].index
+    truncation = pd.Series(dtype="object")
+    for col in dtype:
+        # replace None with pd.NaT
+        dataframe[col] = dataframe[col].fillna(pd.NaT)
+        # assume +00:00 UTC if time zone is not set
+        dataframe[col] = dataframe[col].apply(
+            lambda x: x.tz_localize("UTC") if x.tzinfo is None else x
+        )
+        # apply adjustments to prepped data that will be inserted
+        prepped[col] = dataframe[col]
+        # check if pandas datatype has greater precision than SQL data type
+        # TODO: check need to round/truncate timezoneoffset?
+        extra = prepped[col].apply(lambda x: x.nanosecond % 100 > 0).any()
+        truncation = pd.concat([truncation, pd.Series(extra, index=[col])])
+
+    if any(truncation):
+        truncation = list(truncation[truncation].index)
+        msg = f"Nanosecond precision for dataframe columns {truncation} will be rounded as SQL data type 'datetimeoffset' allows 7 max decimal places."
+        logger.warning(msg)
+        # round nanosecond to the 7th decimal place ...145224193 -> ...145224200 for SQL
+        for col in truncation:
+            rounded = (
+                dataframe[col]
+                .apply(
+                    lambda x: pd.Timestamp(
+                        year=x.year,
+                        month=x.month,
+                        day=x.day,
+                        hour=x.hour,
+                        minute=x.minute,
+                        second=x.second,
+                        microsecond=x.microsecond,
+                        nanosecond=round(x.nanosecond / 100) * 100,
+                        tzinfo=x.tzinfo,
+                    )
+                    if pd.notnull(x)
+                    else x
+                )
+                .fillna(pd.NaT)
+            )
+            dataframe[col] = rounded
+            prepped[col] = rounded
+    if any(dtype):
+        # convert to string since python datetime.datetime allows 6 decimals but SQL allows 7
+        # string is also needed to represent time zone offset
+        for col in dtype:
+            prepped[col] = prepped[col].astype("str")
+            prepped[col] = prepped[col].replace({"NaT": None})
+            # limit to 7 decimal places
+            prepped[col] = prepped[col].str.replace(r"(?<=\.\d{7})00", "", regex=True)
+            # include +00:00 where tzinfo is None
+            prepped[col] = prepped[col].str.replace(
+                r"(?<=\.\d{7})$", r"\g<0>+00:00", regex=True
+            )
+
+    return prepped, dataframe
+
+
+def prepare_numeric(schema, prepped, dataframe):
+    """Prepare numeric & decimal for writting to SQL."""
+    dtype = schema[schema["sql_type"].isin(["numeric", "decimal"])].index
+    for col in dtype:
+        # set a common missing value
+        dataframe[col] = dataframe[col].replace([pd.NA], None)
+        # round to correct number of decimal digits
+        decimal_digits = int(schema.at[col, "decimal_digits"])
+        prepped[col] = dataframe[col].apply(
+            lambda x: round(x, decimal_digits) if pd.notna(x) else x
+        )
+        if not dataframe[col].equals(prepped[col]):
+            msg = f"Decimal digits for column [{col}] will be rounded to {decimal_digits} decimal places to fit SQL specification for this column."
+            logger.warning(msg)
+        dataframe[col] = prepped[col]
+
+    return prepped, dataframe
+
+
+def prepare_values(
+    schema: pd.DataFrame, dataframe: pd.DataFrame
+) -> Tuple[pd.DataFrame, list]:
+    """Prepare dataframe contents for writting values to SQL.
+
+    Parameters
+    ----------
+    schema (pandas.DataFrame) : data schema definition
+    dataframe (pandas.DataFrame) : dataframe that will be written to SQL
+
+    Returns
+    -------
+    dataframe (pandas.DataFrame) : values that may be altered to conform to SQL precision limitations
+    values (list) : values to pass to pyodbc.connect.cursor.executemany
+
+    """
+    # create a copy to preserve values in return
+    prepped = dataframe.copy()
+
+    # include index as column as it is the primary key
+    # also retain the origional index for dataframe/series comparisons
+    index = prepped.index.names
+    if any(index):
+        prepped = prepped.reset_index()
+        prepped = prepped.set_index(index, drop=False)
+
+    # only prepare values currently in dataframe
+    schema = schema[schema.index.isin(prepped.columns)]
+
+    # round and truncate values to be the same as SQL
+    prepped, dataframe = prepare_time(schema, prepped, dataframe)
+    prepped, dataframe = prepare_datetime(schema, prepped, dataframe)
+    prepped, dataframe = prepare_datetime2(schema, prepped, dataframe)
+    prepped, dataframe = prepare_datetimeoffset(schema, prepped, dataframe)
+    prepped, dataframe = prepare_numeric(schema, prepped, dataframe)
+
     # treat pandas NA,NaT,etc as NULL in SQL
     # prepped = prepped.fillna(np.nan).replace([np.nan], [None])
 
     # # convert single column of datetime to objects
     # # otherwise tolist() will produce ints instead of datetimes
     # if prepped.shape[1] == 1 and prepped.select_dtypes("datetime").shape[1] == 1:
     #     prepped = prepped.astype(object)
@@ -442,70 +611,147 @@
 
     # values for pyodbc cursor executemany
     values = prepped.values.tolist()
 
     return dataframe, values
 
 
-def prepare_connection(connection: pyodbc.connect) -> pyodbc.connect:
-    """Prepare connection by adding output converters for data types directly to a pandas data type.
-
-    1. Avoids errors such as pyodbc.ProgrammingError where the ODBC library doesn't already have a conversion defined.
-    pyodbc.ProgrammingError: ('ODBC SQL type -155 is not yet supported. column-index=0 type=-155', 'HY106')
-
-    2. Conversion directly to a pandas types allows greater precision. Python datetime.datetime allows 6
-    decimal places of precision while pandas Timestamps allows 9.
-
-    Note that adding converters for nullable pandas integer types isn't possible, since those are implemented at the
-    array level. Pandas also doesn't support an exact precision decimal data type.
+def convert_time(connection):
+    """
+    Convert SQL time to timedelta.
 
-    Parameters
-    ----------
-    connection (pyodbc.connect) : connection without default output converters
+    pyodbc "SQL_SS_TIME2" = T-SQL "TIME"
 
-    Returns
-    -------
-    connection (pyodbc.connect) : connection with added output converters
+    python datetime.time has 6 decimal places of precision and isn't nullable
+    pandas Timedelta supports 9 decimal places and is nullable
+    SQL TIME only supports 7 decimal places for precision
+    SQL TIME range is '00:00:00.0000000' to '23:59:59.9999999' while pandas allows multiple days and negatives
     """
-    # TIME (pyodbc.SQL_SS_TIME2, SQL TIME)
-    # python datetime.time has 6 decimal places of precision and isn't nullable
-    # pandas Timedelta supports 9 decimal places and is nullable
-    # SQL TIME only supports 7 decimal places for precision
-    # SQL TIME range is '00:00:00.0000000' to '23:59:59.9999999' while pandas allows multiple days and negatives
+
     def SQL_SS_TIME2(raw_bytes, pattern=struct.Struct("<4hI")):
         hour, minute, second, _, fraction = pattern.unpack(raw_bytes)
         return pd.Timedelta(
             hours=hour,
             minutes=minute,
             seconds=second,
             microseconds=fraction // 1000,
             nanoseconds=fraction % 1000,
         )
 
     connection.add_output_converter(pyodbc.SQL_SS_TIME2, SQL_SS_TIME2)
 
-    # TIMESTAMP (pyodbc.SQL_TYPE_TIMESTMAP, SQL DATETIME2)
-    # python datetime.datetime has 6 decimal places of precision and isn't nullable
-    # pandas Timestamp supports 9 decimal places and is nullable
-    # SQL DATETIME2 only supports 7 decimal places for precision
-    # pandas Timestamp range range is '1677-09-21 00:12:43.145225' to '2262-04-11 23:47:16.854775807' while SQL allows '0001-01-01' through '9999-12-31'
-    def SQL_TYPE_TIMESTAMP(raw_bytes, pattern=struct.Struct("hHHHHHI")):
-        year, month, day, hour, minute, second, fraction = pattern.unpack(raw_bytes)
-        return pd.Timestamp(
+    return connection
+
+
+def convert_timestamp(connection):
+    """
+    Convert SQL DATETIME2/DATETIME to datetime.
+
+    Types: pyodbc "SQL_TYPE_TIMESTAMP" = T-SQL "DATETIME2" or pyodbc "SQL_TYPE_TIMESTAMP" =  T-SQL "DATETIME"
+    python datetime.datetime has 6 decimal places of precision and isn't nullable
+    pandas Timestamp supports 9 decimal places and is nullable
+    SQL DATETIME2 only supports 7 decimal places for precision
+    SQL DATETIME only supports 3 decimal places for precision in rounded increments of .000, .003, or .007 seconds
+    pandas Timestamp range range is '1677-09-21 00:12:43.145225' to '2262-04-11 23:47:16.854775807'
+    DATETIME2 allows '0001-01-01' through '9999-12-31'
+    DATETIME allows '1753-01-01' through '9999-12-31'
+    """
+
+    def SQL_TYPE_TIMESTAMP(raw_bytes):
+        # DATETIME2 (16 bytes)
+        if len(raw_bytes) == 16:
+            pattern = struct.Struct("hHHHHHI")
+            year, month, day, hour, minute, second, fraction = pattern.unpack(raw_bytes)
+            timestamp = pd.Timestamp(
+                year=year,
+                month=month,
+                day=day,
+                hour=hour,
+                minute=minute,
+                second=second,
+                microsecond=fraction // 1000,
+                nanosecond=fraction % 1000,
+            )
+        # DATETIME (8 bytes)
+        else:
+            pattern = struct.Struct("iI")
+            days, ticks = pattern.unpack(raw_bytes)
+            timestamp = pd.Timestamp(year=1900, month=1, day=1) + pd.Timedelta(
+                days=days, milliseconds=round(3.33333333 * ticks)
+            )
+
+        return timestamp
+
+    connection.add_output_converter(pyodbc.SQL_TYPE_TIMESTAMP, SQL_TYPE_TIMESTAMP)
+
+    return connection
+
+
+def convert_datetimeoffset(connection):
+    """
+    Convert SQL datetimeoffset to datetime with timezone.
+
+    Types: pyodbc "UNDEFINED" = T-SQL "DATETIMEOFFSET" = ODBC SQL type "-155"
+    """
+
+    def SQL_TYPE_DATETIMEOFFSET(raw_bytes):
+        (
+            year,
+            month,
+            day,
+            hour,
+            minute,
+            second,
+            fraction,
+            offset_hour,
+            offset_minute,
+        ) = struct.unpack("<6hI2h", raw_bytes)
+
+        timestamp = pd.Timestamp(
             year=year,
             month=month,
             day=day,
             hour=hour,
             minute=minute,
             second=second,
             microsecond=fraction // 1000,
             nanosecond=fraction % 1000,
+            tzinfo=pytz.FixedOffset(offset_hour * 60 + offset_minute),
         )
 
-    connection.add_output_converter(pyodbc.SQL_TYPE_TIMESTAMP, SQL_TYPE_TIMESTAMP)
+        return timestamp
+
+    connection.add_output_converter(-155, SQL_TYPE_DATETIMEOFFSET)
+
+    return connection
+
+
+def prepare_connection(connection: pyodbc.connect) -> pyodbc.connect:
+    """Prepare connection by adding output converters for data types directly to a pandas data type.
+
+    1. Avoids errors such as pyodbc.ProgrammingError where the ODBC library doesn't already have a conversion defined.
+    pyodbc.ProgrammingError: ('ODBC SQL type -155 is not yet supported. column-index=0 type=-155', 'HY106')
+
+    2. Conversion directly to a pandas types allows greater precision. Python datetime.datetime allows 6
+    decimal places of precision while pandas Timestamps allows 9.
+
+    Note that adding converters for nullable pandas integer types isn't possible, since those are implemented at the
+    array level. Pandas also doesn't support an exact precision decimal data type.
+
+    Parameters
+    ----------
+    connection (pyodbc.connect) : connection without default output converters
+
+    Returns
+    -------
+    connection (pyodbc.connect) : connection with added output converters
+    """
+    connection = convert_time(connection)
+    connection = convert_timestamp(connection)
+    connection = convert_datetimeoffset(connection)
 
     return connection
 
 
 def insert_values(
     table_name: str,
     dataframe: pd.DataFrame,
@@ -547,22 +793,24 @@
     # issue insert statement
     if include_metadata_timestamps:
         insert = "_time_insert, " + ", ".join(columns)
         params = "GETDATE(), " + ", ".join(["?"] * len(columns))
     else:
         insert = ", ".join(columns)
         params = ", ".join(["?"] * len(columns))
+
+    # skip security check since table and columns have been escaped
     statement = f"""
     INSERT INTO
     {table} (
         {insert}
     ) VALUES (
         {params}
     )
-    """
+    """  # nosec hardcoded_sql_expressions
     cursor.executemany(statement, values)
     cursor.commit()
 
     # values that may be altered to conform to SQL precision limitations
     return dataframe
 
 
@@ -600,14 +848,18 @@
         columns = list(columns[~columns.isin(schema.index)])
         raise AttributeError(f"missing columns from schema: {columns}")
     dtypes = schema.loc[columns, "pandas_type"].to_dict()
     result = {col: [row[idx] for row in result] for idx, col in enumerate(columns)}
     result = {col: pd.Series(vals, dtype=dtypes[col]) for col, vals in result.items()}
     result = pd.DataFrame(result)
 
+    # replace missing values in object columns with pandas type
+    datetimeoffset = schema.index[schema["sql_type"] == "datetimeoffset"]
+    result[datetimeoffset] = result[datetimeoffset].fillna(pd.NaT)
+
     # set primary key columns as index
     keys = list(schema[schema["pk_seq"].notna()].index)
     if keys:
         try:
             result = result.set_index(keys=keys)
         except KeyError:
             raise KeyError(f"primary key column missing from query: {keys}")
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/conversion_rules.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/conversion_rules.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,148 @@
 """Rules for conversion between SQL, pandas, and odbc data types."""
 import pandas as pd
+from numpy import inf
 import pyodbc
 
 rules = pd.DataFrame.from_records(
     [
         {
             "sql_type": "bit",
             "sql_category": "boolean",
             "min_value": False,
             "max_value": True,
             "pandas_type": "boolean",
             "odbc_type": pyodbc.SQL_BIT,
-            "odbc_size": 1,
-            "odbc_precision": 0,
         },
         {
             "sql_type": "tinyint",
-            "sql_category": "exact numeric",
+            "sql_category": "exact_whole_numeric",
             "min_value": 0,
             "max_value": 255,
             "pandas_type": "UInt8",
             "odbc_type": pyodbc.SQL_TINYINT,
-            "odbc_size": 1,
-            "odbc_precision": 0,
         },
         {
             "sql_type": "smallint",
-            "sql_category": "exact numeric",
+            "sql_category": "exact_whole_numeric",
             "min_value": -(2**15),
             "max_value": 2**15 - 1,
             "pandas_type": "Int16",
             "odbc_type": pyodbc.SQL_SMALLINT,
-            "odbc_size": 2,
-            "odbc_precision": 0,
         },
         {
             "sql_type": "int",
-            "sql_category": "exact numeric",
+            "sql_category": "exact_whole_numeric",
             "min_value": -(2**31),
             "max_value": 2**31 - 1,
             "pandas_type": "Int32",
             "odbc_type": pyodbc.SQL_INTEGER,
-            "odbc_size": 4,
-            "odbc_precision": 0,
         },
         {
             "sql_type": "bigint",
-            "sql_category": "exact numeric",
+            "sql_category": "exact_whole_numeric",
             "min_value": -(2**63),
             "max_value": 2**63 - 1,
             "pandas_type": "Int64",
             "odbc_type": pyodbc.SQL_BIGINT,
-            "odbc_size": 8,
-            "odbc_precision": 0,
         },
         {
             "sql_type": "float",
-            "sql_category": "approximate numeric",
+            "sql_category": "approximate_decimal_numeric",
             "min_value": -(1.79**308),
             "max_value": 1.79**308,
             "pandas_type": "float64",
             "odbc_type": pyodbc.SQL_FLOAT,
-            "odbc_size": 8,
-            "odbc_precision": 53,
+        },
+        {
+            "sql_type": "numeric",
+            "sql_category": "exact_decimal_numeric",
+            "min_value": -inf,
+            "max_value": inf,
+            "pandas_type": "object",
+            "odbc_type": pyodbc.SQL_NUMERIC,
+        },
+        {
+            "sql_type": "decimal",
+            "sql_category": "exact_decimal_numeric",
+            "min_value": -inf,
+            "max_value": inf,
+            "pandas_type": "object",
+            "odbc_type": pyodbc.SQL_DECIMAL,
         },
         {
             "sql_type": "time",
-            "sql_category": "date time",
+            "sql_category": "date_time",
             "min_value": pd.Timedelta("00:00:00.0000000"),
             "max_value": pd.Timedelta("23:59:59.9999999"),
             "pandas_type": "timedelta64[ns]",
             "odbc_type": pyodbc.SQL_SS_TIME2,
-            "odbc_size": 16,
-            "odbc_precision": 7,
         },
         {
             "sql_type": "date",
-            "sql_category": "date time",
+            "sql_category": "date_time",
             "min_value": pd.Timestamp((pd.Timestamp.min + pd.Timedelta(days=1)).date()),
             "max_value": pd.Timestamp(pd.Timestamp.max.date()),
             "pandas_type": "datetime64[ns]",
             "odbc_type": pyodbc.SQL_TYPE_DATE,
-            "odbc_size": 10,
-            "odbc_precision": 0,
+        },
+        {
+            "sql_type": "datetime",
+            "sql_category": "date_time",
+            "min_value": pd.Timestamp(1753, 1, 1, 0, 0, 0),
+            "max_value": pd.Timestamp(1900, 1, 1) + pd.Timedelta.max,
+            "pandas_type": "datetime64[ns]",
+            "odbc_type": pyodbc.SQL_TYPE_TIMESTAMP,
+        },
+        {
+            "sql_type": "datetimeoffset",
+            "sql_category": "date_time",
+            # TODO: inforce SQL TZ offset limit of -14:00 through +14:00
+            "min_value": pd.Timestamp(pd.Timestamp.min, tz="UTC"),
+            "max_value": pd.Timestamp(pd.Timestamp.max, tz="UTC"),
+            "pandas_type": "object",
+            "odbc_type": -155,
         },
         {
             "sql_type": "datetime2",
-            "sql_category": "date time",
-            "min_value": pd.Timestamp.min,
+            "sql_category": "date_time",
+            "min_value": pd.Timestamp.min.ceil("us"),
             "max_value": pd.Timestamp.max,
             "pandas_type": "datetime64[ns]",
             "odbc_type": pyodbc.SQL_TYPE_TIMESTAMP,
-            "odbc_size": 27,
-            "odbc_precision": 7,
+        },
+        {
+            "sql_type": "char",
+            "sql_category": "character string",
+            "min_value": 1,
+            "max_value": 0,
+            "pandas_type": "string",
+            "odbc_type": pyodbc.SQL_CHAR,
         },
         {
             "sql_type": "varchar",
             "sql_category": "character string",
             "min_value": 1,
             "max_value": 0,
             "pandas_type": "string",
             "odbc_type": pyodbc.SQL_VARCHAR,
-            "odbc_size": 0,
-            "odbc_precision": 0,
+        },
+        {
+            "sql_type": "nchar",
+            "sql_category": "character string",
+            "min_value": 1,
+            "max_value": 0,
+            "pandas_type": "string",
+            "odbc_type": pyodbc.SQL_WCHAR,
         },
         {
             "sql_type": "nvarchar",
             "sql_category": "character string",
             "min_value": 1,
             "max_value": 0,
             "pandas_type": "string",
             "odbc_type": pyodbc.SQL_WVARCHAR,
-            "odbc_size": 0,
-            "odbc_precision": 0,
         },
     ]
 )
 rules["sql_type"] = rules["sql_type"].astype("string")
 rules["pandas_type"] = rules["pandas_type"].astype("string")
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/custom_errors.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/custom_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 
 class SQLInsufficientColumnSize(Exception):
     """Exception for insufficient column size to insert a numeric or string."""
 
     pass
 
 
+class SQLNonUnicodeTypeColumn(Exception):
+    """Exception for data containing unicode but SQL column is a non-unicode type."""
+
+
 class SQLRecastColumnUnchanged(Exception):
     """Exception for SQLInsufficientColumnSize handling not resulting in change of type or size."""
 
     pass
 
 
 class SQLInvalidLengthObjectName(Exception):
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/dynamic.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/dynamic.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/modify.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/modify.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/read.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/read.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,31 +44,35 @@
         dataframe (pandas.DataFrame): tabular data from select statement
 
         Examples
         --------
         A sample table to read, created from a dataframe.
         >>> df = pd.DataFrame(
         ...    {
-        ...        "ColumnA": [5, 6, 7],
-        ...        "ColumnB": [5, 6, None],
-        ...        "ColumnC": [pd.NA, 6, 7],
-        ...        "ColumnD": ["06-22-2021", "06-22-2021", pd.NaT],
-        ...        "ColumnE": ["a", "b", None],
-        ...    }, index = ["xxx", "yyy", "zzz"]
+        ...        "ColumnA": [5, 6, None],
+        ...        "ColumnB": ["06-22-2021", "06-22-2021", pd.NaT],
+        ...        "ColumnC": ["aa", "b", None],
+        ...    }, index = pd.Index(["xxx", "yyy", "zzz"], name='PK')
         ... )
-        >>> df = create.table_from_dataframe('##ExampleRead', df, primary_key='index')
+        >>> create.table('##ExampleRead',
+        ...     {
+        ...         'ColumnA': 'TINYINT', 'ColumnB': 'DATETIME2', 'ColumnC': 'VARCHAR(2)', 'PK': 'CHAR(3)'
+        ...     },
+        ...     primary_key_column = 'PK'
+        ... )
+        >>> df = insert('##ExampleRead', df)
 
         Select the entire table. The primary key is set as the dataframe's index.
         >>> query = read.table('##ExampleRead')
 
         Select specific columns.
         >>> query = read.table('##ExampleRead', column_names=['ColumnA','ColumnB'])
 
         Select using conditions grouped by parentheses while applying a limit and order.
-        >>> query = read.table('##ExampleRead', where="(ColumnB>4 AND ColumnC IS NOT NULL) OR ColumnE IS NULL", limit=5, order_column='ColumnB', order_direction='DESC')
+        >>> query = read.table('##ExampleRead', where="(ColumnA>5 AND ColumnB IS NOT NULL) OR ColumnC IS NULL", limit=5, order_column='ColumnB', order_direction='DESC')
         """
         # get table schema for conversion to pandas
         schema, _ = conversion.get_schema(self._connection, table_name)
 
         # always read in primary key columns for dataframe index
         primary_key_columns = list(
             schema.loc[schema["pk_seq"].notna(), "pk_seq"]
@@ -125,23 +129,24 @@
                 + dynamic.escape(self._connection.cursor(), order_column)
                 + " "
                 + order_direction
             )
         else:
             order = ""
 
-        # select values
+        # skip security check since table_name, column_names, where_statement, order have been escaped
+        # limit has been enforced to be an integer
         statement = f"""
         SELECT {limit}
             {column_names}
         FROM
             {table_name}
             {where_statement}
             {order}
-        """
+        """  # nosec hardcoded_sql_expressions
 
         # read sql query
         dataframe = conversion.read_values(
             statement, schema, self._connection, where_args
         )
 
         return dataframe
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/insert.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/write/insert.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,49 +11,43 @@
 class insert:
     """Class for inserting data into SQL."""
 
     def __init__(
         self,
         connection: pyodbc.connect,
         include_metadata_timestamps: bool = False,
-        autoadjust_sql_objects: bool = False,
     ):
         """Class for inserting data into SQL.
 
         Parameters
         ----------
         connection (pyodbc.Connection) : connection for executing statement
         include_metadata_timestamps (bool, default=False) : include metadata timestamps _time_insert & _time_update for write operations
-        autoadjust_sql_objects (bool, default=False) : if True, create SQL tables or alter SQL columns if needed
         """
         self._connection = connection
         self.include_metadata_timestamps = include_metadata_timestamps
-        self.autoadjust_sql_objects = autoadjust_sql_objects
 
-        # max attempts for creating/modifing SQL tables
-        # value of 3 will: add include_metadata_timestamps columns and/or add other columns and/or increase column size
-        self._adjust_sql_attempts = 3
+        # create temporary tables for upsert/merging
+        self._create = create.create(connection)
 
-        # handle failures if autoadjust_sql_objects==True
+        # add include_metadata_timestamps if needed
         self._modify = modify.modify(connection)
-        self._create = create.create(connection)
 
     def insert(
         self,
         table_name: str,
         dataframe: pd.DataFrame,
         include_metadata_timestamps: bool = None,
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """Insert data into SQL table from a dataframe.
 
         Parameters
         ----------
         table_name (str) : name of table to insert data into
         dataframe (pandas.DataFrame): tabular data to insert
-        include_metadata_timestamps (bool, default=None) : override for the class initialized parameter autoadjust_sql_objects to include _time_insert column
 
         Returns
         -------
         dataframe (pandas.DataFrame) : input dataframe that may have been altered to conform to SQL
 
         Examples
         --------
@@ -106,51 +100,86 @@
         updating_table (bool, default=False) : flag that indicates if target table is being updated
 
         Returns
         -------
         schema (pandas.DataFrame) : table column specifications and conversion rules
         dataframe (pandas.DataFrame) : input dataframe with optimal values and types for inserting into SQL
         """
-        for _ in range(0, self._adjust_sql_attempts + 1):
-            try:
-                # dataframe values converted according to SQL data type
-                schema, dataframe = conversion.get_schema(
-                    self._connection,
-                    table_name,
-                    dataframe,
-                    additional_columns,
-                )
-                break
-            except (
-                custom_errors.SQLTableDoesNotExist,
-                custom_errors.SQLColumnDoesNotExist,
-                custom_errors.SQLInsufficientColumnSize,
-            ) as failure:
-                cursor.rollback()
-                # dataframe values may be converted according to SQL data type
-                dataframe = _exceptions.handle(
-                    failure,
-                    table_name,
-                    dataframe,
-                    updating_table,
-                    self.autoadjust_sql_objects,
-                    self._modify,
-                    self._create,
-                )
-                cursor.commit()
-            except Exception as err:
-                cursor.rollback()
-                raise err
-        else:
-            raise RecursionError(
-                f"adjust_sql_attempts={self._adjust_sql_attempts} reached"
+        try:
+            schema, dataframe = conversion.get_schema(
+                self._connection,
+                table_name,
+                dataframe,
+                additional_columns,
+            )
+        except custom_errors.SQLColumnDoesNotExist as failure:
+            # add metadata_timestamps
+            cursor.rollback()
+            dataframe = _exceptions.add_metadata_timestamps(
+                failure,
+                table_name,
+                dataframe,
+                self._modify,
+            )
+            cursor.commit()
+            # retry data insert
+            schema, dataframe = conversion.get_schema(
+                self._connection,
+                table_name,
+                dataframe,
+                additional_columns,
             )
+        except Exception as err:
+            cursor.rollback()
+            raise err
 
         return schema, dataframe
 
+    def _column_spec(self, schema: pd.DataFrame, columns: list) -> dict:
+        """Generate dictionary mapping of column name to SQL data type and specifications.
+
+        Parameters
+        ----------
+        schema (pandas.DataFrame) : output of get_schema for a table
+
+        Returns
+        -------
+        dtypes (dict) : dictionary mapping of each column name to SQL data type and specifications
+        """
+        # select only columns present in dataframe to prevent updating with nulls
+        dtypes = schema.loc[
+            columns, ["sql_category", "sql_type", "column_size", "decimal_digits"]
+        ]
+        dtypes = dtypes.astype("string")
+
+        # add byte size for string columns
+        idx = dtypes[dtypes["sql_category"] == "character string"].index
+        dtypes.loc[idx, "sql_type"] = (
+            dtypes.loc[idx, "sql_type"] + "(" + dtypes.loc[idx, "column_size"] + ")"
+        )
+
+        # add precision and scale for exact decimal numerics
+        idx = dtypes[dtypes["sql_category"] == "exact_decimal_numeric"].index
+        dtypes.loc[idx, "sql_type"] = (
+            dtypes.loc[idx, "sql_type"]
+            + "("
+            + dtypes.loc[idx, "column_size"]
+            + ","
+            + dtypes.loc[idx, "decimal_digits"]
+            + ")"
+        )
+
+        # avoid creating an int identify data type column for a source table
+        dtypes["sql_type"] = dtypes["sql_type"].replace("int identity", "int")
+
+        # convert to dictionary of column name : data type
+        dtypes = dtypes["sql_type"].to_dict()
+
+        return dtypes
+
     def _source_table(
         self,
         table_name,
         dataframe,
         cursor,
         match_columns: list = None,
         additional_columns: list = None,
@@ -204,16 +233,26 @@
             )
 
         # insert data into source temporary table
         temp_name = "##__source_" + table_name
         columns = list(dataframe.columns)
         if any(dataframe.index.names):
             columns = list(dataframe.index.names) + columns
-        _, dtypes = conversion.sql_spec(schema.loc[columns], dataframe)
-        dtypes = {k: v.replace("int identity", "int") for k, v in dtypes.items()}
+
+        dtypes = self._column_spec(schema, columns)
+
         not_nullable = list(schema[~schema["is_nullable"]].index)
+
         self._create.table(
             temp_name, dtypes, not_nullable, primary_key_column=match_columns
         )
-        _ = self.insert(temp_name, dataframe, include_metadata_timestamps=False)
+
+        dataframe = self.insert(temp_name, dataframe, include_metadata_timestamps=False)
+
+        # reset match columns that were part of the primary key in the source table
+        # dataframe needs returned in the event values were adjusted but indicies/columns should be the same
+        names = schema.loc[dataframe.index.names, "pk_seq"]
+        extra = names[names.isna()].index.tolist()
+        if any(extra):
+            dataframe = dataframe.reset_index(level=extra)
 
         return schema, dataframe, match_columns, temp_name
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/merge.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/write/merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,55 +28,59 @@
         Parameters
         ----------
         table_name (str) : name of the SQL table
         dataframe (pandas.DataFrame): tabular data to merge into SQL table
         match_columns (list, default=None) : combination of columns or index to determine matches, if None the SQL primary key and dataframe index is used
         upsert (bool, default=False) : delete records if they do not match
         delete_requires (list, default=None) : column(s) that need to have a matching row for records to be deleted
-        include_metadata_timestamps (bool, default=None) : override for the class initialized parameter autoadjust_sql_objects to include _time_insert and _time_update columns
+        include_metadata_timestamps (bool, default=None) : include _time_insert and _time_update columns
 
         Returns
         -------
         dataframe (pandas.DataFrame) : input dataframe that may have been altered to conform to SQL
 
         Examples
         --------
         A sample table to merge, created from a dataframe.
-        >>> df = create.table_from_dataframe(
-        ...    "##ExampleMergeDF", pd.DataFrame({"State": ["A", "B"], "ColumnA": [3, 4], "ColumnB": ["a", "b"]}), primary_key="index"
+        >>> create.table(
+        ...     '##ExampleMergeDF',
+        ...     {'State': 'CHAR(1)', 'ColumnA': 'TINYINT', 'ColumnB': 'CHAR(1)', 'PK': 'TINYINT'},
+        ...     primary_key_column = 'PK'
         ... )
+        >>> df = pd.DataFrame({"State": ["A", "B"], "ColumnA": [3, 4], "ColumnB": ["a", "b"]}, index=pd.Index([0, 1], name='PK'))
+        >>> df = insert('##ExampleMergeDF', df)
 
         Merge using the dataframe's index and SQL primary key. Include the column _time_insert and _time_update (automatically created).
         >>> # delete first row
         >>> df = df[df.index != 0]
         >>> # update second row
         >>> df.loc[df.index == 1, "ColumnA"] = 5
         >>> # insert new row
-        >>> new = pd.DataFrame({"State": ["C"], "ColumnA": [6], "ColumnB": ["d"]}, index=pd.Index([2], name="_index"))
+        >>> new = pd.DataFrame({"State": ["C"], "ColumnA": [6], "ColumnB": ["d"]}, index=pd.Index([2], name="PK"))
         >>> df = pd.concat([df, new])
         >>> # perform the merge.
         >>> df_merged = merge("##ExampleMergeDF", df, include_metadata_timestamps=True)
 
-        Incremntally merge a dataframe. Index=2 will remain unchanged since State=C is not part of the increment.
+        Incremntally merge a dataframe. Index=2 will remain unchanged since State=C is not included in df_increment.
         >>> df_increment = pd.DataFrame.from_records([
         ...    # updated record
         ...    {"State": "B", "ColumnA": 6, "ColumnB": "d"},
         ...    # new record
         ...    {"State": "D", "ColumnA": 6, "ColumnB": "d"},
-        ...    ],index=pd.Index([1, 3], name="_index"),
+        ...    ],index=pd.Index([1, 3], name="PK"),
         ... )
         >>> df_increment = merge("##ExampleMergeDF", df_increment, delete_requires=['State'], include_metadata_timestamps=True)
 
         Perform an UPSERT action (if exists update, otherwise insert). Records will never be deleted.
         >>> df_upsert = pd.DataFrame.from_records([
         ...    # updated record
         ...    {"State": "B", "ColumnA": 10, "ColumnB": "x"},
         ...    # new record
         ...    {"State": "E", "ColumnA": 0, "ColumnB": "y"},
-        ...    ],index=pd.Index([1, 4], name="_index"),
+        ...    ],index=pd.Index([1, 4], name="PK"),
         ... )
         >>> df_merge = merge('##ExampleMergeDF', df_upsert, upsert=True, include_metadata_timestamps=True)
         """
         # check inputs
         if delete_requires is not None and upsert:
             raise ValueError("delete_requires can only be specified if upsert==False")
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/core/write/update.py` & `mssql_dataframe-2.0.0/mssql_dataframe/core/write/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,41 @@
         """Update column(s) in an SQL table using a dataframe.
 
         Parameters
         ----------
         table_name (str) : name of table to insert data into
         dataframe (pandas.DataFrame): tabular data to insert
         match_columns (list, default=None) : matches records between dataframe and SQL table, if None the SQL primary key and dataframe index is used
-        include_metadata_timestamps (bool, default=None) : override for the class initialized parameter autoadjust_sql_objects to include _time_update column
+        include_metadata_timestamps (bool, default=None) : include _time_update column
 
         Returns
         -------
         dataframe (pandas.DataFrame) : input dataframe that may have been altered to conform to SQL
 
         Examples
         --------
         A sample table to update, created from a dataframe.
+        >>> create.table(
+        ... '##ExampleUpdateDF',
+        ... {
+        ...     '_index': 'CHAR(3)', 'ColumnA': 'TINYINT', 'ColumnB': 'TINYINT',
+        ...     'ColumnC': 'TINYINT', 'ColumnD': 'DATE', 'ColumnE': 'CHAR(1)'
+        ... },
+        ... primary_key_column = '_index'
+        ... )
         >>> df = pd.DataFrame(
         ...    {
         ...    "ColumnA": [5, 6, 7],
         ...    "ColumnB": [5, 6, 7],
         ...    "ColumnC": [8, 9, 10],
         ...    "ColumnD": ["06-22-2021", "06-22-2021", pd.NaT],
         ...    "ColumnE": ["a", "b", None],
-        ...    }, index = ["xxx", "yyy", "zzz"]
+        ...    }, index = pd.Series(["xxx", "yyy", "zzz"], name='_index')
         ... )
-        >>> df = create.table_from_dataframe('##ExampleUpdateDF', df, primary_key='index')
+        >>> df = insert('##ExampleUpdateDF', df)
 
         Update ColumnA only using the dataframe index & SQL primary key.
         >>> df['ColumnA'] = [8,9,10]
         >>> df_updated = update('##ExampleUpdateDF', df[['ColumnA']])
 
         Update ColumnB based on ColumnC, which isn't the SQL primary key. Include the column _time_update (automatically created) to reflect in server time when the record was updated.
         >>> df['ColumnB'] += 1
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe/package.py` & `mssql_dataframe-2.0.0/mssql_dataframe/package.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,27 +15,22 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SQLServer(connect):
     """Class containing methods for creating, modifying, reading, and writing between dataframes and SQL Server.
 
-    If autoadjust_sql_objects is True SQL objects may be modified such as creating a table, adding a column,
-    or increasing the size of a column. The exception is internal tracking metadata columns _time_insert and
-    _time_update which will always be created if include_metadata_timestamps=True.
-
     Parameters
     ----------
     database (str, default='master') : name of database to connect to
     server (str, default='localhost') : name of server to connect to
     driver (str, default=None) : ODBC driver name to use, if not given is automatically determined
     username (str, default=None) : if not given, use Windows account credentials to connect
     password (str, default=None) : if not given, use Windows account credentials to connect
     include_metadata_timestamps (bool, default=False) : include metadata timestamps _time_insert & _time_update in server time for write operations
-    autoadjust_sql_objects (bool, default=False) : create and modify SQL table and columns as needed if True
 
     Properties
     ----------
     create : methods for creating SQL tables objects
     modify : methods for modifying tables columns and primary keys
     read : methods for reading from SQL tables
     write : methods for inserting, updating, and merging records
@@ -43,18 +38,14 @@
     Examples
     --------
     Connect to localhost server master database.
 
     >>> import env
     >>> sql = SQLServer(database=env.database, server=env.server)
 
-    Connect with the ability to automatically adjust SQL objects.
-
-    >>> sql = SQLServer(database=env.database, server=env.server, autoadjust_sql_objects=True)
-
     Enable logging from mssql_dataframe.
 
     >>> import logging
     >>> logging.basicConfig(
     ... filename='example.log', encoding='utf-8', level=logging.DEBUG,
     ... format='%(asctime)s %(name)s %(filename)s %(levelname)s: %(message)s'
     ... )
@@ -70,40 +61,32 @@
         self,
         database: str = "master",
         server: str = "localhost",
         driver: str = None,
         username: str = None,
         password: str = None,
         include_metadata_timestamps: bool = False,
-        autoadjust_sql_objects: bool = False,
     ):
-
         connect.__init__(self, database, server, driver, username, password)
 
         # log initialization details
         self.log_init()
 
         # initialize mssql_dataframe functionality with shared connection
         self.exceptions = custom_errors
         self.create = create.create(self.connection, include_metadata_timestamps)
         self.modify = modify.modify(self.connection)
         self.read = read.read(self.connection)
-        self.write = write(
-            self.connection, include_metadata_timestamps, autoadjust_sql_objects
-        )
+        self.write = write(self.connection, include_metadata_timestamps)
 
         # issue warnings for automated functionality
         if include_metadata_timestamps:
             msg = "SQL write operations will include metadata '_time_insert' & '_time_update' columns as 'include_metadata_timestamps=True'."
             logger.warning(msg)
 
-        if autoadjust_sql_objects:
-            msg = "SQL objects will be created/modified as needed as 'autoadjust_sql_objects=True'."
-            logger.warning(msg)
-
     def log_init(self):
         """Log connection info and versions for Python, SQL, and required packages."""
         # determine versions for debugging
         self.version_spec = {}
         # Python
         self.version_spec["python"] = sys.version_info
         # SQL
```

### Comparing `mssql_dataframe-1.5.2rc3/mssql_dataframe.egg-info/SOURCES.txt` & `mssql_dataframe-2.0.0/mssql_dataframe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 pyproject.toml
 setup.cfg
+mssql_dataframe/__equality__.py
 mssql_dataframe/__init__.py
-mssql_dataframe/__sample__.py
 mssql_dataframe/connect.py
 mssql_dataframe/package.py
 mssql_dataframe.egg-info/PKG-INFO
 mssql_dataframe.egg-info/SOURCES.txt
 mssql_dataframe.egg-info/dependency_links.txt
 mssql_dataframe.egg-info/requires.txt
 mssql_dataframe.egg-info/top_level.txt
 mssql_dataframe/core/__init__.py
 mssql_dataframe/core/conversion.py
 mssql_dataframe/core/conversion_rules.py
 mssql_dataframe/core/create.py
 mssql_dataframe/core/custom_errors.py
 mssql_dataframe/core/dynamic.py
-mssql_dataframe/core/infer.py
 mssql_dataframe/core/modify.py
 mssql_dataframe/core/read.py
 mssql_dataframe/core/write/__init__.py
 mssql_dataframe/core/write/_exceptions.py
 mssql_dataframe/core/write/insert.py
 mssql_dataframe/core/write/merge.py
 mssql_dataframe/core/write/update.py
```

### Comparing `mssql_dataframe-1.5.2rc3/setup.cfg` & `mssql_dataframe-2.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -57,10 +57,14 @@
 00000380: 6669 6c74 6572 7761 726e 696e 6773 203d  filterwarnings =
 00000390: 200d 0a09 6967 6e6f 7265 3a50 7955 6e69   ...ignore:PyUni
 000003a0: 636f 6465 5f46 726f 6d55 6e69 636f 6465  code_FromUnicode
 000003b0: 5c28 4e55 4c4c 2c20 7369 7a65 5c29 2069  \(NULL, size\) i
 000003c0: 7320 6465 7072 6563 6174 6564 0d0a 0d0a  s deprecated....
 000003d0: 5b66 6c61 6b65 385d 0d0a 6967 6e6f 7265  [flake8]..ignore
 000003e0: 203d 200d 0a09 4535 3031 2c0d 0a09 5735   = ...E501,...W5
-000003f0: 3033 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  03....[egg_info]
-00000400: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000410: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000003f0: 3033 0d0a 0d0a 5b63 6f76 6572 6167 653a  03....[coverage:
+00000400: 7275 6e5d 0d0a 6f6d 6974 203d 200d 0a09  run]..omit = ...
+00000410: 6d73 7371 6c5f 6461 7461 6672 616d 655c  mssql_dataframe\
+00000420: 5f5f 6571 7561 6c69 7479 5f5f 2e70 790d  __equality__.py.
+00000430: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000440: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000450: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

