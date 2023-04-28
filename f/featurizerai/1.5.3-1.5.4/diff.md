# Comparing `tmp/featurizerai-1.5.3.tar.gz` & `tmp/featurizerai-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.3.tar", last modified: Fri Apr 28 21:17:56 2023, max compression
+gzip compressed data, was "featurizerai-1.5.4.tar", last modified: Fri Apr 28 21:24:30 2023, max compression
```

## Comparing `featurizerai-1.5.3.tar` & `featurizerai-1.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:17:55.998591 featurizerai-1.5.3/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.3/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.3/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:17:55.998656 featurizerai-1.5.3/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.3/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:17:55.998878 featurizerai-1.5.3/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:15:43.000000 featurizerai-1.5.3/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:17:55.994727 featurizerai-1.5.3/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:17:55.996787 featurizerai-1.5.3/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.3/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.3/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.3/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.3/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4766 2023-04-28 21:17:45.000000 featurizerai-1.5.3/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:17:55.997569 featurizerai-1.5.3/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.3/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.3/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.3/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:17:55.998469 featurizerai-1.5.3/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:17:55.000000 featurizerai-1.5.3/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:17:55.000000 featurizerai-1.5.3/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:17:55.000000 featurizerai-1.5.3/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:17:55.000000 featurizerai-1.5.3/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:17:55.000000 featurizerai-1.5.3/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:24:30.087145 featurizerai-1.5.4/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.4/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.4/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:24:30.087215 featurizerai-1.5.4/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.4/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:24:30.087424 featurizerai-1.5.4/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:24:20.000000 featurizerai-1.5.4/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:24:30.083697 featurizerai-1.5.4/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:24:30.085485 featurizerai-1.5.4/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.4/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.4/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.4/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.4/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4718 2023-04-28 21:23:10.000000 featurizerai-1.5.4/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:24:30.086197 featurizerai-1.5.4/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.4/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.4/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.4/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:24:30.087023 featurizerai-1.5.4/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:24:30.000000 featurizerai-1.5.4/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:24:30.000000 featurizerai-1.5.4/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:24:30.000000 featurizerai-1.5.4/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:24:30.000000 featurizerai-1.5.4/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:24:30.000000 featurizerai-1.5.4/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.3/LICENSE` & `featurizerai-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/PKG-INFO` & `featurizerai-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.3/setup.py` & `featurizerai-1.5.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.3',
+    version='1.5.4',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.3/src/features/authenticate.py` & `featurizerai-1.5.4/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/src/features/create_stream.py` & `featurizerai-1.5.4/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/src/features/custom_schema.py` & `featurizerai-1.5.4/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/src/features/materialize.py` & `featurizerai-1.5.4/src/features/materialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pymongo import MongoClient
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import col, count
 from pyspark.sql.types import StringType, StructType, StructField, TimestampType, IntegerType
 from pyspark.sql import functions as F
 import certifi
 from pymongo.server_api import ServerApi
+from pyspark.sql.functions import col
 
 
 class materialize:
     def __init__(self, mongo_connection, aggregation_date, groupby_attr, groupby_value, token, schema, sparksql, partition_column=None):
         self.mongo_connection = mongo_connection
         self.aggregation_date = datetime.strptime(aggregation_date, "%Y-%m-%d %H:%M:%S")
         self.groupby = groupby_value
@@ -83,15 +84,14 @@
             sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
             c_count = self.spark.sql(sql_with_timestamp_base)
             joined_df = df.join(c_count, self.groupby_attr, "left") \
                 .select(df.columns + [col for col in c_count.columns if col not in df.columns])
             df = joined_df
             print(joined_df)
 
-        df = df.drop(columns=[col for col in df.columns if col != self.groupby_attr])
         # Convert the aggregated data to JSON
         print(df)
 
         if df.isEmpty():
             json_aggregated_data = "{'error': 'No data found'}"
         else:
             json_aggregated_data = df.toJSON().collect()[0]
```

### Comparing `featurizerai-1.5.3/src/features/tests/test_materialize.py` & `featurizerai-1.5.4/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/src/features/tests/test_pipeline.py` & `featurizerai-1.5.4/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.3/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.4/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

