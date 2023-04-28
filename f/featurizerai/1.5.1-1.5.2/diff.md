# Comparing `tmp/featurizerai-1.5.1.tar.gz` & `tmp/featurizerai-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.1.tar", last modified: Fri Apr 28 19:36:37 2023, max compression
+gzip compressed data, was "featurizerai-1.5.2.tar", last modified: Fri Apr 28 20:57:48 2023, max compression
```

## Comparing `featurizerai-1.5.1.tar` & `featurizerai-1.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.434312 featurizerai-1.5.1/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.1/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.1/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 19:36:37.434376 featurizerai-1.5.1/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.1/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 19:36:37.434599 featurizerai-1.5.1/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 19:36:14.000000 featurizerai-1.5.1/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.429403 featurizerai-1.5.1/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.431280 featurizerai-1.5.1/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.1/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.1/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.1/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.1/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.5.1/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.433304 featurizerai-1.5.1/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.1/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.1/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.1/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.434189 featurizerai-1.5.1/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 20:57:48.130646 featurizerai-1.5.2/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.2/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.2/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 20:57:48.130714 featurizerai-1.5.2/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.2/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 20:57:48.130939 featurizerai-1.5.2/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 20:57:38.000000 featurizerai-1.5.2/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 20:57:48.126299 featurizerai-1.5.2/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 20:57:48.128403 featurizerai-1.5.2/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.2/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.2/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.2/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.2/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4702 2023-04-28 20:57:34.000000 featurizerai-1.5.2/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 20:57:48.129640 featurizerai-1.5.2/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.2/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.2/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.2/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 20:57:48.130530 featurizerai-1.5.2/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 20:57:48.000000 featurizerai-1.5.2/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 20:57:48.000000 featurizerai-1.5.2/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 20:57:48.000000 featurizerai-1.5.2/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 20:57:48.000000 featurizerai-1.5.2/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 20:57:48.000000 featurizerai-1.5.2/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.1/LICENSE` & `featurizerai-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/PKG-INFO` & `featurizerai-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.1/setup.py` & `featurizerai-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.1',
+    version='1.5.2',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.1/src/features/authenticate.py` & `featurizerai-1.5.2/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/src/features/create_stream.py` & `featurizerai-1.5.2/src/features/create_stream.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/src/features/custom_schema.py` & `featurizerai-1.5.2/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/src/features/materialize.py` & `featurizerai-1.5.2/src/features/materialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         if df.isEmpty():
             json_aggregated_data = "{'error': 'No data found'}"
         else:
             json_aggregated_data = df.toJSON().collect()[0]
 
         if json_aggregated_data is not None:
             aggregated_data_collection.update_one(
-                {"date": start_time, "deviceid": self.groupby},
+                {"date": start_time, self.groupby_attr: self.groupby},
                 {"$set": {"aggregated_data": json_aggregated_data}},
                 upsert=True
             )
         else:
             logging.error("Serialized aggregated data is None, skipping update")
 
         return json_aggregated_data
```

### Comparing `featurizerai-1.5.1/src/features/tests/test_materialize.py` & `featurizerai-1.5.2/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/src/features/tests/test_pipeline.py` & `featurizerai-1.5.2/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.1/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.2/src/featurizerai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

