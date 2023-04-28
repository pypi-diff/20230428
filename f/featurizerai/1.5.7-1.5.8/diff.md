# Comparing `tmp/featurizerai-1.5.7.tar.gz` & `tmp/featurizerai-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.7.tar", last modified: Fri Apr 28 21:51:54 2023, max compression
+gzip compressed data, was "featurizerai-1.5.8.tar", last modified: Fri Apr 28 21:55:39 2023, max compression
```

## Comparing `featurizerai-1.5.7.tar` & `featurizerai-1.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:51:54.299069 featurizerai-1.5.7/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.7/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.7/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:51:54.299135 featurizerai-1.5.7/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.7/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:51:54.299341 featurizerai-1.5.7/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:51:28.000000 featurizerai-1.5.7/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:51:54.294134 featurizerai-1.5.7/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:51:54.296224 featurizerai-1.5.7/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.7/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.7/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.7/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.7/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4875 2023-04-28 21:51:23.000000 featurizerai-1.5.7/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:51:54.298037 featurizerai-1.5.7/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.7/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.7/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.7/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:51:54.298942 featurizerai-1.5.7/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:51:54.000000 featurizerai-1.5.7/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:51:54.000000 featurizerai-1.5.7/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:51:54.000000 featurizerai-1.5.7/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:51:54.000000 featurizerai-1.5.7/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:51:54.000000 featurizerai-1.5.7/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.098312 featurizerai-1.5.8/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.8/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.8/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:55:39.098383 featurizerai-1.5.8/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.8/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:55:39.098613 featurizerai-1.5.8/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:55:26.000000 featurizerai-1.5.8/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.094303 featurizerai-1.5.8/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.096418 featurizerai-1.5.8/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.8/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.8/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.8/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.8/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4946 2023-04-28 21:54:27.000000 featurizerai-1.5.8/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.097208 featurizerai-1.5.8/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.8/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.8/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.8/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:55:39.098099 featurizerai-1.5.8/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:55:39.000000 featurizerai-1.5.8/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.7/LICENSE` & `featurizerai-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/PKG-INFO` & `featurizerai-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.7/setup.py` & `featurizerai-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.7',
+    version='1.5.8',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.7/src/features/authenticate.py` & `featurizerai-1.5.8/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/src/features/create_stream.py` & `featurizerai-1.5.8/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/src/features/custom_schema.py` & `featurizerai-1.5.8/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/src/features/materialize.py` & `featurizerai-1.5.8/src/features/materialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,17 @@
         df = df.filter(col(self.groupby_attr) == self.groupby)
         start_time = self.aggregation_date
         df = df.filter((col(self.groupby_attr) == self.groupby) & (col("timestamp") < start_time.timestamp()))
         df = df.withColumn("timestamp_unix", F.col("timestamp").cast("bigint"))
         df.createOrReplaceTempView("temp_table")
 
         # Define empty schema for DataFrame
-        schema = StructType([])
-
+        schema = StructType([
+            StructField(self.groupby_attr, StringType(), True)
+        ])
         # Create empty DataFrame
         result_df = self.spark.createDataFrame([], schema)
 
         # Execute the dynamic Spark SQL
         for sql in self.sparksql:
             sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
             hour = int(sql.split("_")[3])
```

### Comparing `featurizerai-1.5.7/src/features/tests/test_materialize.py` & `featurizerai-1.5.8/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/src/features/tests/test_pipeline.py` & `featurizerai-1.5.8/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.7/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.8/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.7
+Version: 1.5.8
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

