# Comparing `tmp/elastic_helper-1.2.3.tar.gz` & `tmp/elastic_helper-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elastic_helper-1.2.3.tar", last modified: Tue Jun  9 08:27:34 2020, max compression
+gzip compressed data, was "elastic_helper-1.2.4.tar", last modified: Fri Apr 28 11:39:38 2023, max compression
```

## Comparing `elastic_helper-1.2.3.tar` & `elastic_helper-1.2.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 snuids     (501) staff       (20)        0 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/
--rw-r--r--   0 snuids     (501) staff       (20)     2641 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/PKG-INFO
--rw-r--r--   0 snuids     (501) staff       (20)     1814 2019-10-10 08:37:35.000000 elastic_helper-1.2.3/README.md
-drwxr-xr-x   0 snuids     (501) staff       (20)        0 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper/
--rw-r--r--   0 snuids     (501) staff       (20)        0 2019-04-05 07:51:10.000000 elastic_helper-1.2.3/elastic_helper/__init__.py
--rw-r--r--   0 snuids     (501) staff       (20)     7640 2020-05-20 13:05:17.000000 elastic_helper-1.2.3/elastic_helper/es_helper.py
--rw-r--r--   0 snuids     (501) staff       (20)     7233 2019-12-16 14:19:27.000000 elastic_helper-1.2.3/elastic_helper/es_helper_test.py
-drwxr-xr-x   0 snuids     (501) staff       (20)        0 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper.egg-info/
--rw-r--r--   0 snuids     (501) staff       (20)     2641 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper.egg-info/PKG-INFO
--rw-r--r--   0 snuids     (501) staff       (20)      258 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper.egg-info/SOURCES.txt
--rw-r--r--   0 snuids     (501) staff       (20)        1 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper.egg-info/dependency_links.txt
--rw-r--r--   0 snuids     (501) staff       (20)       15 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/elastic_helper.egg-info/top_level.txt
--rw-r--r--   0 snuids     (501) staff       (20)       38 2020-06-09 08:27:34.000000 elastic_helper-1.2.3/setup.cfg
--rw-r--r--   0 snuids     (501) staff       (20)      699 2020-06-09 08:26:39.000000 elastic_helper-1.2.3/setup.py
+drwxr-xr-x   0 snuids     (501) staff       (20)        0 2023-04-28 11:39:38.767246 elastic_helper-1.2.4/
+-rw-r--r--   0 snuids     (501) staff       (20)     2728 2023-04-28 11:39:38.767451 elastic_helper-1.2.4/PKG-INFO
+-rw-r--r--   0 snuids     (501) staff       (20)     1814 2021-10-03 08:58:49.000000 elastic_helper-1.2.4/README.md
+drwxr-xr-x   0 snuids     (501) staff       (20)        0 2023-04-28 11:39:38.766043 elastic_helper-1.2.4/elastic_helper/
+-rw-r--r--   0 snuids     (501) staff       (20)        0 2021-10-03 08:58:49.000000 elastic_helper-1.2.4/elastic_helper/__init__.py
+-rw-r--r--   0 snuids     (501) staff       (20)     8012 2023-04-28 11:27:10.000000 elastic_helper-1.2.4/elastic_helper/es_helper.py
+-rw-r--r--   0 snuids     (501) staff       (20)     7233 2021-10-03 08:58:49.000000 elastic_helper-1.2.4/elastic_helper/es_helper_test.py
+drwxr-xr-x   0 snuids     (501) staff       (20)        0 2023-04-28 11:39:38.767108 elastic_helper-1.2.4/elastic_helper.egg-info/
+-rw-r--r--   0 snuids     (501) staff       (20)     2728 2023-04-28 11:39:38.000000 elastic_helper-1.2.4/elastic_helper.egg-info/PKG-INFO
+-rw-r--r--   0 snuids     (501) staff       (20)      320 2023-04-28 11:39:38.000000 elastic_helper-1.2.4/elastic_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 snuids     (501) staff       (20)        1 2023-04-28 11:39:38.000000 elastic_helper-1.2.4/elastic_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 snuids     (501) staff       (20)       24 2023-04-28 11:39:38.000000 elastic_helper-1.2.4/elastic_helper.egg-info/requires.txt
+-rw-r--r--   0 snuids     (501) staff       (20)       15 2023-04-28 11:39:38.000000 elastic_helper-1.2.4/elastic_helper.egg-info/top_level.txt
+-rw-r--r--   0 snuids     (501) staff       (20)       82 2023-04-28 11:27:10.000000 elastic_helper-1.2.4/pyproject.toml
+-rw-r--r--   0 snuids     (501) staff       (20)      488 2023-04-28 11:39:38.768082 elastic_helper-1.2.4/setup.cfg
+-rw-r--r--   0 snuids     (501) staff       (20)      750 2023-04-28 11:38:39.000000 elastic_helper-1.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elastic_helper-1.2.3/PKG-INFO` & `elastic_helper-1.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: elastic_helper
-Version: 1.2.3
+Version: 1.2.4
 Summary: Elastic Search to Pandas Dataframe
 Home-page: https://github.com/snuids/elastic_helper
 Author: snuids
 Author-email: snuids@mannekentech.com
 License: UNKNOWN
-Download-URL: https://github.com/snuids/elastic_helper/archive/1.2.3.tar.gz
+Download-URL: https://github.com/snuids/elastic_helper/archive/1.2.4.tar.gz
 Description: # elastic_helper
         Two simple functions
         * One used to convert an elastic search collection into a dataframe. See the code for the various parameters.
         * One used to convert a dataframe into an elastic search collection
         
         
         ## Installation
@@ -58,8 +58,9 @@
         
         es_helper.dataframe_to_elastic(es,my_df)                                                               
         ```
         
         
 Keywords: ElasticSearch,pandas,convert
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `elastic_helper-1.2.3/README.md` & `elastic_helper-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `elastic_helper-1.2.3/elastic_helper/es_helper.py` & `elastic_helper-1.2.4/elastic_helper/es_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,19 +158,22 @@
     Optionally an "_timestamp" column can be used to specify a "@timestamp column.
 
     Parameters:
     es -- The elastic connection object
     df -- The dataframe
     """
 
-    logger = logging.getLogger(__name__)
+    #logger = logging.getLogger(__name__)
+    logger = logging.getLogger()
 
     logger.debug("LOADING DATA FRAME")
     logger.debug("==================")
 
+    print('coucou')
+
     version = int(get_es_info(es).get('version').get('number').split('.')[0])
 
 
     if len([item for item, count in collections.Counter(df.columns).items() if count > 1]) > 0:
         logger.error("NNOOOOOOOOBBBB DUPLICATE COLUMN FOUND "*10)
         raise Exception('Duplicate column in DataFrame')
 
@@ -186,15 +189,18 @@
 
     #df.columns=[_.replace("_timestamp","@timestamp") for _ in df.columns]
     df.rename(columns={"_timestamp": "@timestamp"},inplace=True)
 
     df_json = json.loads(df.to_json(orient='records'))
     
     action = {}
-    action["index"] = {"_type": doc_type}
+    if version > 7:
+        action["index"] = {}
+    else:    
+        action["index"] = {"_type": doc_type}
 
     flag_unique_index = False
 
     if len(df['_index'].unique() == 1):
         flag_unique_index = True
         
         action["index"]["_index"] = df.iloc[0]["_index"]
@@ -209,30 +215,37 @@
         bulkbody += json.dumps(action, cls=DateTimeEncoder) + "\r\n"
         bulkbody += json.dumps({k:v for k,v in row.items() if k!='_id' and k!='_index' and v is not None}, 
                             cls=DateTimeEncoder) + "\r\n"
 
 
         if len(bulkbody) > 512000:
             logger.debug("BULK READY:" + str(len(bulkbody)))
-            # print(bulkbody)
-            bulkres = es.bulk(bulkbody, request_timeout=30)
+            logger.info(version)
+            if version > 7:
+                bulkres = es.bulk(body=bulkbody, request_timeout=30)
+            else:
+                bulkres = es.bulk(bulkbody, request_timeout=30)
+
             logger.debug("BULK DONE")
             bulkbody = ""
 
             if(not(bulkres["errors"])):
                 logger.info("BULK done without errors.")
             else:
                 for item in bulkres["items"]:
                     if "error" in item["index"]:
                         reserrors.append(
                             {"error": item["index"]["error"], "id": item["index"]["_id"]})
 
     if len(bulkbody) > 0:
         logger.debug("BULK READY FINAL:" + str(len(bulkbody)))
-        bulkres = es.bulk(bulkbody)
+        if version > 7:
+            bulkres = es.bulk(body=bulkbody, request_timeout=30)
+        else:
+            bulkres = es.bulk(bulkbody, request_timeout=30)
         logger.debug("BULK DONE FINAL")
 
         if(not(bulkres["errors"])):
             logger.info("BULK done without errors.")
         else:
             for item in bulkres["items"]:
                 if "error" in item["index"]:
```

### Comparing `elastic_helper-1.2.3/elastic_helper/es_helper_test.py` & `elastic_helper-1.2.4/elastic_helper/es_helper_test.py`

 * *Files identical despite different names*

### Comparing `elastic_helper-1.2.3/elastic_helper.egg-info/PKG-INFO` & `elastic_helper-1.2.4/elastic_helper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: elastic-helper
-Version: 1.2.3
+Version: 1.2.4
 Summary: Elastic Search to Pandas Dataframe
 Home-page: https://github.com/snuids/elastic_helper
 Author: snuids
 Author-email: snuids@mannekentech.com
 License: UNKNOWN
-Download-URL: https://github.com/snuids/elastic_helper/archive/1.2.3.tar.gz
+Download-URL: https://github.com/snuids/elastic_helper/archive/1.2.4.tar.gz
 Description: # elastic_helper
         Two simple functions
         * One used to convert an elastic search collection into a dataframe. See the code for the various parameters.
         * One used to convert a dataframe into an elastic search collection
         
         
         ## Installation
@@ -58,8 +58,9 @@
         
         es_helper.dataframe_to_elastic(es,my_df)                                                               
         ```
         
         
 Keywords: ElasticSearch,pandas,convert
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `elastic_helper-1.2.3/setup.py` & `elastic_helper-1.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #from distutils.core import setup
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-  name = 'elastic_helper',
-  packages = ['elastic_helper'], # this must be the same as the name above
-  version = '1.2.3',
-  description = 'Elastic Search to Pandas Dataframe',
-  long_description=long_description,
-  long_description_content_type="text/markdown",
-  author = 'snuids',
-  author_email = 'snuids@mannekentech.com',
-  url = 'https://github.com/snuids/elastic_helper', 
-  download_url = 'https://github.com/snuids/elastic_helper/archive/1.2.3.tar.gz',
-  keywords = ['ElasticSearch', 'pandas', 'convert'], # arbitrary keywords
-  classifiers = [],
-)
+name = 'elastic_helper',
+packages = ['elastic_helper'], # this must be the same as the name above
+version = '1.2.4',
+description = 'Elastic Search to Pandas Dataframe',
+long_description=long_description,
+long_description_content_type="text/markdown",
+author = 'snuids',
+author_email = 'snuids@mannekentech.com',
+url = 'https://github.com/snuids/elastic_helper', 
+download_url = 'https://github.com/snuids/elastic_helper/archive/1.2.4.tar.gz',
+keywords = ['ElasticSearch', 'pandas', 'convert'], # arbitrary keywords
+classifiers = ["License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"],
+)
```

