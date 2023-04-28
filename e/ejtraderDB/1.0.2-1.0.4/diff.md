# Comparing `tmp/ejtraderDB-1.0.2.tar.gz` & `tmp/ejtraderDB-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ejtraderDB-1.0.2.tar", last modified: Tue Mar  9 20:29:24 2021, max compression
+gzip compressed data, was "ejtraderDB-1.0.4.tar", last modified: Fri Apr 28 13:59:19 2023, max compression
```

## Comparing `ejtraderDB-1.0.2.tar` & `ejtraderDB-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-09 20:29:24.079494 ejtraderDB-1.0.2/
--rw-r--r--   0 sos        (501) staff       (20)       49 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/MANIFEST.in
--rw-r--r--   0 sos        (501) staff       (20)     1288 2021-03-09 20:29:24.079716 ejtraderDB-1.0.2/PKG-INFO
--rw-r--r--   0 sos        (501) staff       (20)        0 2021-03-04 22:33:09.000000 ejtraderDB-1.0.2/README.md
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-09 20:29:24.074633 ejtraderDB-1.0.2/ejtraderDB/
--rw-r--r--   0 sos        (501) staff       (20)      443 2021-03-09 01:05:03.000000 ejtraderDB-1.0.2/ejtraderDB/__init__.py
--rw-r--r--   0 sos        (501) staff       (20)      321 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/ejtraderDB/common.py
--rw-r--r--   0 sos        (501) staff       (20)     2045 2021-03-09 01:04:03.000000 ejtraderDB-1.0.2/ejtraderDB/dict.py
--rw-r--r--   0 sos        (501) staff       (20)       87 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/ejtraderDB/exceptions.py
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-09 20:29:24.079023 ejtraderDB-1.0.2/ejtraderDB/serializers/
--rw-r--r--   0 sos        (501) staff       (20)       18 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/ejtraderDB/serializers/__init__.py
--rw-r--r--   0 sos        (501) staff       (20)      763 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/ejtraderDB/serializers/json.py
--rw-r--r--   0 sos        (501) staff       (20)     1189 2021-03-09 01:01:49.000000 ejtraderDB-1.0.2/ejtraderDB/serializers/msgpack.py
--rw-r--r--   0 sos        (501) staff       (20)      941 2021-02-22 21:35:11.000000 ejtraderDB-1.0.2/ejtraderDB/serializers/pickle.py
--rw-r--r--   0 sos        (501) staff       (20)     7612 2021-03-09 01:04:15.000000 ejtraderDB-1.0.2/ejtraderDB/sqlbase.py
--rw-r--r--   0 sos        (501) staff       (20)     4839 2021-03-09 01:06:39.000000 ejtraderDB-1.0.2/ejtraderDB/sqlqueue.py
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-09 20:29:24.076335 ejtraderDB-1.0.2/ejtraderDB.egg-info/
--rw-r--r--   0 sos        (501) staff       (20)     1288 2021-03-09 20:29:23.000000 ejtraderDB-1.0.2/ejtraderDB.egg-info/PKG-INFO
--rw-r--r--   0 sos        (501) staff       (20)      492 2021-03-09 20:29:23.000000 ejtraderDB-1.0.2/ejtraderDB.egg-info/SOURCES.txt
--rw-r--r--   0 sos        (501) staff       (20)        1 2021-03-09 20:29:23.000000 ejtraderDB-1.0.2/ejtraderDB.egg-info/dependency_links.txt
--rw-r--r--   0 sos        (501) staff       (20)       23 2021-03-09 20:29:23.000000 ejtraderDB-1.0.2/ejtraderDB.egg-info/requires.txt
--rw-r--r--   0 sos        (501) staff       (20)       11 2021-03-09 20:29:23.000000 ejtraderDB-1.0.2/ejtraderDB.egg-info/top_level.txt
--rw-r--r--   0 sos        (501) staff       (20)       14 2021-03-09 01:01:21.000000 ejtraderDB-1.0.2/requirements.txt
--rw-r--r--   0 sos        (501) staff       (20)       67 2021-03-09 20:29:24.080345 ejtraderDB-1.0.2/setup.cfg
--rw-r--r--   0 sos        (501) staff       (20)     1990 2021-03-09 20:29:19.000000 ejtraderDB-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:19.086006 ejtraderDB-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-28 13:59:19.086006 ejtraderDB-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:19.082006 ejtraderDB-1.0.4/ejtraderDB/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/qdb_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/questdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:19.086006 ejtraderDB-1.0.4/ejtraderDB/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/serializers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/sqlackqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/sqlbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/ejtraderDB/sqlqueue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:59:19.082006 ejtraderDB-1.0.4/ejtraderDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-28 13:59:19.000000 ejtraderDB-1.0.4/ejtraderDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 13:59:19.000000 ejtraderDB-1.0.4/ejtraderDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:59:19.000000 ejtraderDB-1.0.4/ejtraderDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 13:59:19.000000 ejtraderDB-1.0.4/ejtraderDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 13:59:19.000000 ejtraderDB-1.0.4/ejtraderDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 13:59:19.086006 ejtraderDB-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-28 13:59:07.000000 ejtraderDB-1.0.4/setup.py
```

### Comparing `ejtraderDB-1.0.2/ejtraderDB/dict.py` & `ejtraderDB-1.0.4/ejtraderDB/dict.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/ejtraderDB/serializers/json.py` & `ejtraderDB-1.0.4/ejtraderDB/serializers/json.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/ejtraderDB/serializers/msgpack.py` & `ejtraderDB-1.0.4/ejtraderDB/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/ejtraderDB/serializers/pickle.py` & `ejtraderDB-1.0.4/ejtraderDB/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/ejtraderDB/sqlbase.py` & `ejtraderDB-1.0.4/ejtraderDB/sqlbase.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/ejtraderDB/sqlqueue.py` & `ejtraderDB-1.0.4/ejtraderDB/sqlqueue.py`

 * *Files identical despite different names*

### Comparing `ejtraderDB-1.0.2/setup.py` & `ejtraderDB-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,22 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderDB',
-    version='1.0.2',
+    version='1.0.4',
     packages=find_packages(),
     url='https://ejtraderDB.readthedocs.io/',
     download_url='https://ejtrader.com',
     license='MIT License',
     author='Emerson Pedroso',
     author_email='support@ejtrader.com',
-    description='Metatrader API',
+    description='SQlite and QuestDB',
     long_description=readme(),
     long_description_content_type='text/markdown',
     install_requires=requirements(filename='requirements.txt'),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.5",
@@ -39,22 +39,19 @@
         "Intended Audience :: Developers",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries"
     ],
     python_requires='>=3',
-    extras_require={
-        "docs": requirements(filename='docs/requirements.txt')
-    },
     keywords=', '.join([
         'metatrader', 'f-api', 'historical-data',
         'financial-data', 'stocks', 'funds', 'etfs',
         'indices', 'currency crosses', 'bonds', 'commodities',
         'crypto currencies'
     ]),
     project_urls={
-        'Bug Reports': 'https://github.com/traderpedroso/ejtraderDB/issues',
-        'Source': 'https://github.com/traderpedroso/ejtraderDB',
+        'Bug Reports': 'https://github.com/ejtraderLabs/ejtraderDB/issues',
+        'Source': 'https://github.com/ejtraderLabs/ejtraderDB',
         'Documentation': 'https://ejtrader.readthedocs.io/'
     },
-)
+)
```

