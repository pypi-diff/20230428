# Comparing `tmp/django_graphbox-1.2.1.tar.gz` & `tmp/django_graphbox-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_graphbox-1.2.1.tar", last modified: Fri Mar 17 16:23:12 2023, max compression
+gzip compressed data, was "django_graphbox-1.2.2.tar", last modified: Fri Apr 28 18:45:08 2023, max compression
```

## Comparing `django_graphbox-1.2.1.tar` & `django_graphbox-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.470115 django_graphbox-1.2.1/
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.1/LICENSE
--rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.1/MANIFEST.in
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-03-17 16:23:12.470115 django_graphbox-1.2.1/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.1/README.md
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.422125 django_graphbox-1.2.1/docs/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.438122 django_graphbox-1.2.1/docs/source/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    17710 2023-02-23 15:06:34.000000 django_graphbox-1.2.1/docs/source/quickstart.rst
--rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.1/pyproject.toml
--rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-03-17 16:23:12.474114 django_graphbox-1.2.1/setup.cfg
--rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.1/setup.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.422125 django_graphbox-1.2.1/src/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.446120 django_graphbox-1.2.1/src/django_graphbox/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.1/src/django_graphbox/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    12252 2023-03-17 16:22:00.000000 django_graphbox-1.2.1/src/django_graphbox/builder.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1698 2023-02-23 21:43:45.000000 django_graphbox-1.2.1/src/django_graphbox/constants.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.1/src/django_graphbox/exceptions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.1/src/django_graphbox/hasher.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.470115 django_graphbox-1.2.1/src/django_graphbox/helpers/
--rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.1/src/django_graphbox/helpers/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    16165 2023-02-24 03:36:43.000000 django_graphbox-1.2.1/src/django_graphbox/helpers/mutations.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     6584 2022-08-08 14:39:50.000000 django_graphbox-1.2.1/src/django_graphbox/helpers/queries.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.1/src/django_graphbox/helpers/sessions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.1/src/django_graphbox/helpers/shared.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.1/src/django_graphbox/session.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-03-17 16:23:12.458118 django_graphbox-1.2.1/src/django_graphbox.egg-info/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-03-17 16:23:12.000000 django_graphbox-1.2.1/src/django_graphbox.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-03-17 16:23:12.000000 django_graphbox-1.2.1/src/django_graphbox.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-03-17 16:23:12.000000 django_graphbox-1.2.1/src/django_graphbox.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-03-17 16:23:12.000000 django_graphbox-1.2.1/src/django_graphbox.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-03-17 16:23:12.000000 django_graphbox-1.2.1/src/django_graphbox.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.2/LICENSE
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.2/README.md
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.525729 django_graphbox-1.2.2/docs/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.529731 django_graphbox-1.2.2/docs/source/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    17710 2023-02-23 15:06:34.000000 django_graphbox-1.2.2/docs/source/quickstart.rst
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/pyproject.toml
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/setup.cfg
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.2/setup.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.525729 django_graphbox-1.2.2/src/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.533733 django_graphbox-1.2.2/src/django_graphbox/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    12252 2023-03-17 16:22:00.000000 django_graphbox-1.2.2/src/django_graphbox/builder.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1750 2023-04-28 18:44:37.000000 django_graphbox-1.2.2/src/django_graphbox/constants.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.2/src/django_graphbox/exceptions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/hasher.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.537735 django_graphbox-1.2.2/src/django_graphbox/helpers/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    16165 2023-02-24 03:36:43.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/mutations.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     6584 2022-08-08 14:39:50.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/queries.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/sessions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.2/src/django_graphbox/helpers/shared.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.2/src/django_graphbox/session.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-04-28 18:45:08.533733 django_graphbox-1.2.2/src/django_graphbox.egg-info/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18253 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-04-28 18:45:08.000000 django_graphbox-1.2.2/src/django_graphbox.egg-info/top_level.txt
```

### Comparing `django_graphbox-1.2.1/LICENSE` & `django_graphbox-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/PKG-INFO` & `django_graphbox-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_graphbox
-Version: 1.2.1
+Version: 1.2.2
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_graphbox-1.2.1/README.md` & `django_graphbox-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/docs/source/quickstart.rst` & `django_graphbox-1.2.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/setup.cfg` & `django_graphbox-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_graphbox
-version = 1.2.1
+version = 1.2.2
 description = Package for easy building GraphQL API with Django
 long_description = file:docs/source/quickstart.rst
 url = https://github.com/yefeza/django-graphbox
 author = Yeison Fernandez
 author_email = contacto@90horasporsemana.com
 license = MIT
 classifiers =
```

### Comparing `django_graphbox-1.2.1/src/django_graphbox/builder.py` & `django_graphbox-1.2.2/src/django_graphbox/builder.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/constants.py` & `django_graphbox-1.2.2/src/django_graphbox/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import graphene
 import graphene_file_upload.scalars
 
 MODEL_FIELD_TO_GRAPHENE_TYPE = {
     'AutoField': graphene.ID,
     'BigAutoField': graphene.ID,
-    'BigIntegerField': graphene.Int,
+    'BigIntegerField': graphene.BigInt if hasattr(graphene, 'BigInt') else graphene.Int,
     'BooleanField': graphene.Boolean,
     'CharField': graphene.String,
     'DateField': graphene.Date,
     'DateTimeField': graphene.DateTime,
     'DecimalField': graphene.Decimal,
     'DurationField': graphene.String,
     'EmailField': graphene.String,
```

### Comparing `django_graphbox-1.2.1/src/django_graphbox/exceptions.py` & `django_graphbox-1.2.2/src/django_graphbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/hasher.py` & `django_graphbox-1.2.2/src/django_graphbox/hasher.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/helpers/mutations.py` & `django_graphbox-1.2.2/src/django_graphbox/helpers/mutations.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/helpers/queries.py` & `django_graphbox-1.2.2/src/django_graphbox/helpers/queries.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/helpers/sessions.py` & `django_graphbox-1.2.2/src/django_graphbox/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/helpers/shared.py` & `django_graphbox-1.2.2/src/django_graphbox/helpers/shared.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox/session.py` & `django_graphbox-1.2.2/src/django_graphbox/session.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.1/src/django_graphbox.egg-info/PKG-INFO` & `django_graphbox-1.2.2/src/django_graphbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphbox
-Version: 1.2.1
+Version: 1.2.2
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_graphbox-1.2.1/src/django_graphbox.egg-info/SOURCES.txt` & `django_graphbox-1.2.2/src/django_graphbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

