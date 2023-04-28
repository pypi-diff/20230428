# Comparing `tmp/featurizerai-1.5.0.tar.gz` & `tmp/featurizerai-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.5.0.tar", last modified: Fri Apr 28 06:22:19 2023, max compression
+gzip compressed data, was "featurizerai-1.5.1.tar", last modified: Fri Apr 28 19:36:37 2023, max compression
```

## Comparing `featurizerai-1.5.0.tar` & `featurizerai-1.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.514257 featurizerai-1.5.0/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.0/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.0/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:22:19.514333 featurizerai-1.5.0/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.0/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 06:22:19.514623 featurizerai-1.5.0/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 06:22:10.000000 featurizerai-1.5.0/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.509530 featurizerai-1.5.0/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.511641 featurizerai-1.5.0/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.0/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.0/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-28 06:11:42.000000 featurizerai-1.5.0/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.0/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.5.0/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.512548 featurizerai-1.5.0/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.0/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2764 2023-04-26 01:15:16.000000 featurizerai-1.5.0/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.0/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.514106 featurizerai-1.5.0/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.434312 featurizerai-1.5.1/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.1/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.1/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 19:36:37.434376 featurizerai-1.5.1/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.1/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 19:36:37.434599 featurizerai-1.5.1/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 19:36:14.000000 featurizerai-1.5.1/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.429403 featurizerai-1.5.1/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.431280 featurizerai-1.5.1/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.1/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.1/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4223 2023-04-28 19:36:07.000000 featurizerai-1.5.1/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.1/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.5.1/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.433304 featurizerai-1.5.1/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.1/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2766 2023-04-28 14:47:29.000000 featurizerai-1.5.1/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.1/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 19:36:37.434189 featurizerai-1.5.1/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 19:36:37.000000 featurizerai-1.5.1/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.5.0/LICENSE` & `featurizerai-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.0/PKG-INFO` & `featurizerai-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.5.0/setup.py` & `featurizerai-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.5.0',
+    version='1.5.1',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.5.0/src/features/authenticate.py` & `featurizerai-1.5.1/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.0/src/features/create_stream.py` & `featurizerai-1.5.1/src/features/create_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             return True
         except ValueError:
             return False
 
     def _run(self, token):
         mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
-        raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
+        raw_data_collection = mongo_db[self.mongo_connection['rawdata']]
 
         consumer = Consumer(self.kafka_connection)
         print(self.topicname)
         consumer.subscribe([self.topicname])
 
         while not self._stop_event.is_set():
             msg = consumer.poll(10.0)
```

### Comparing `featurizerai-1.5.0/src/features/custom_schema.py` & `featurizerai-1.5.1/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.0/src/features/materialize.py` & `featurizerai-1.5.1/src/features/materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.0/src/features/tests/test_materialize.py` & `featurizerai-1.5.1/src/features/tests/test_materialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     {"name": "deviceid", "type": "integer"}
 ]
 
 custom_schema = custom_schema(schema_fields)
 
 app = Flask(__name__)
 
-@app.route('/aggregate', methods=['POST'])
+@app.route('/materialize', methods=['POST'])
 def aggregate():
     mongo_connection = {
         'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
         'database': 'kafkastream',
         'rawdata': 'rawdata',
         'collection': 'sparkaggregate'
     }
```

### Comparing `featurizerai-1.5.0/src/features/tests/test_pipeline.py` & `featurizerai-1.5.1/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.5.0/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.1/src/featurizerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

