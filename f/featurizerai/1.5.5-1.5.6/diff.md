# Comparing `tmp/featurizerai-1.5.5.tar.gz` & `tmp/featurizerai-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.5.tar", last modified: Fri Apr 28 21:32:17 2023, max compression
+gzip compressed data, was "featurizerai-1.5.6.tar", last modified: Fri Apr 28 21:41:26 2023, max compression
```

## Comparing `featurizerai-1.5.5.tar` & `featurizerai-1.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:32:17.282629 featurizerai-1.5.5/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.5/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.5/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:32:17.282714 featurizerai-1.5.5/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.5/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:32:17.282945 featurizerai-1.5.5/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:32:03.000000 featurizerai-1.5.5/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:32:17.280029 featurizerai-1.5.5/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:32:17.281293 featurizerai-1.5.5/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.5/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.5/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.5/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.5/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4866 2023-04-28 21:31:44.000000 featurizerai-1.5.5/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:32:17.281695 featurizerai-1.5.5/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.5/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.5/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.5/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:32:17.282496 featurizerai-1.5.5/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:32:17.000000 featurizerai-1.5.5/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:32:17.000000 featurizerai-1.5.5/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:32:17.000000 featurizerai-1.5.5/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:32:17.000000 featurizerai-1.5.5/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:32:17.000000 featurizerai-1.5.5/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:41:26.981077 featurizerai-1.5.6/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.6/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.6/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:41:26.981149 featurizerai-1.5.6/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.6/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 21:41:26.981379 featurizerai-1.5.6/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 21:41:13.000000 featurizerai-1.5.6/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:41:26.977221 featurizerai-1.5.6/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:41:26.979313 featurizerai-1.5.6/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.6/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.6/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.6/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.6/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4700 2023-04-28 21:40:55.000000 featurizerai-1.5.6/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:41:26.980022 featurizerai-1.5.6/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.6/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.6/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.6/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 21:41:26.980935 featurizerai-1.5.6/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 21:41:26.000000 featurizerai-1.5.6/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 21:41:26.000000 featurizerai-1.5.6/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 21:41:26.000000 featurizerai-1.5.6/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 21:41:26.000000 featurizerai-1.5.6/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 21:41:26.000000 featurizerai-1.5.6/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.5/LICENSE` & `featurizerai-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/PKG-INFO` & `featurizerai-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.5
+Version: 1.5.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.5/setup.py` & `featurizerai-1.5.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.5',
+    version='1.5.6',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.5/src/features/authenticate.py` & `featurizerai-1.5.6/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/src/features/create_stream.py` & `featurizerai-1.5.6/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/src/features/custom_schema.py` & `featurizerai-1.5.6/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/src/features/materialize.py` & `featurizerai-1.5.6/src/features/materialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,17 +85,15 @@
         # Execute the dynamic Spark SQL
         for sql in self.sparksql:
             sql_base = sql.replace("{"+ self.groupby_attr + "}", str(self.groupby))
             hour = int(sql.split("_")[3])
             sql_with_timestamp = sql_base.replace("{timestamp}", str(int((start_time - timedelta(hours=hour)).timestamp())))
             sql_with_timestamp_base = sql_with_timestamp.replace("{timestamp_base}", str(int((start_time).timestamp())))
             c_count = self.spark.sql(sql_with_timestamp_base)
-            joined_df = result_df.join(c_count, self.groupby_attr, "left") \
-                .select(result_df.columns + [col for col in c_count.columns if col not in result_df.columns])
-            result_df = joined_df
+            result_df = c_count.unionByName(result_df)
             print(result_df)
 
         if result_df.isEmpty():
             json_aggregated_data = "{'error': 'No data found'}"
         else:
             json_aggregated_data = result_df.toJSON().collect()[-1]
```

### Comparing `featurizerai-1.5.5/src/features/tests/test_materialize.py` & `featurizerai-1.5.6/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/src/features/tests/test_pipeline.py` & `featurizerai-1.5.6/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.5/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.6/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.5
+Version: 1.5.6
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

