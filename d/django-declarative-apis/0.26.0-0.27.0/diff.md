# Comparing `tmp/django-declarative-apis-0.26.0.tar.gz` & `tmp/django-declarative-apis-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-declarative-apis-0.26.0.tar", last modified: Wed Mar  8 21:44:18 2023, max compression
+gzip compressed data, was "django-declarative-apis-0.27.0.tar", last modified: Fri Apr 28 02:25:09 2023, max compression
```

## Comparing `django-declarative-apis-0.26.0.tar` & `django-declarative-apis-0.27.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.910118 django-declarative-apis-0.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-08 21:44:18.910118 django-declarative-apis-0.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/oauth1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/oauth_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/machinery/
--rw-r--r--   0 runner    (1001) docker     (123)    34444 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29860 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/machinery/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/management/commands/gendocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/migrations/0002_add_consumer_type_field.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.910118 django-declarative-apis-0.26.0/django_declarative_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/resources/emitters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/django_declarative_apis/resources/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.906118 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-08 21:44:18.000000 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-08 21:44:18.000000 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 21:44:18.000000 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-08 21:44:18.000000 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-08 21:44:18.000000 django-declarative-apis-0.26.0/django_declarative_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 21:44:18.910118 django-declarative-apis-0.26.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 21:44:18.910118 django-declarative-apis-0.26.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-03-08 21:44:10.000000 django-declarative-apis-0.26.0/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.622566 django-declarative-apis-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-28 02:25:09.622566 django-declarative-apis-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/oauth1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/oauth_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/machinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    35041 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31885 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/machinery/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/management/commands/gendocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/migrations/0002_add_consumer_type_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.622566 django-declarative-apis-0.27.0/django_declarative_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/resources/emitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/django_declarative_apis/resources/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.618566 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-28 02:25:09.000000 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-28 02:25:09.000000 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:25:09.000000 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 02:25:09.000000 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 02:25:09.000000 django-declarative-apis-0.27.0/django_declarative_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:25:09.622566 django-declarative-apis-0.27.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:25:09.622566 django-declarative-apis-0.27.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-04-28 02:25:00.000000 django-declarative-apis-0.27.0/tests/testutils.py
```

### Comparing `django-declarative-apis-0.26.0/LICENSE` & `django-declarative-apis-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/PKG-INFO` & `django-declarative-apis-0.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-declarative-apis
-Version: 0.26.0
+Version: 0.27.0
 Summary: Simple, readable, declarative APIs for Django
 Keywords: django,rest,declarative,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-declarative-apis-0.26.0/README.md` & `django-declarative-apis-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/adapters.py` & `django-declarative-apis-0.27.0/django_declarative_apis/adapters.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/authentication/__init__.py` & `django-declarative-apis-0.27.0/django_declarative_apis/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/endpoint.py` & `django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/endpoint.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/oauth1.py` & `django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/oauth1.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/oauth_errors.py` & `django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/oauth_errors.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/authentication/oauthlib/request_validator.py` & `django-declarative-apis-0.27.0/django_declarative_apis/authentication/oauthlib/request_validator.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/__init__.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import abc
 import http.client
 import itertools
 import logging
 import sys
 
 import django
+import django.db.models
 from django.conf import settings
 from django.http import HttpResponse
 
 from dirtyfields.dirtyfields import reset_state
 
 from django_declarative_apis.machinery.filtering import apply_filters_to_object
 from django_declarative_apis.models import BaseConsumer
 from django_declarative_apis.resources.utils import HttpStatusCode
 from . import errors
 from .attributes import (
     Aggregate,
     ConsumerAttribute,
     DeferrableEndpointTask,
+    DeferrableGenericEndpointTask,
     EndpointAttribute,
     EndpointTask,
     RawRequestObjectProperty,
     RequestAdhocQuerySet,
     RequestAttribute,
     RequestField,
     RequestProperty,
@@ -224,15 +226,17 @@
                 else:
                     logger.error(str(exc_value.args) + "\n" + str(exc_traceback))
 
                 raise exc_value.with_traceback(exc_traceback)
 
             resource = self.bound_endpoint.resource
 
-            if hasattr(resource, "is_dirty"):
+            if isinstance(resource, django.db.models.Model) and hasattr(
+                resource, "is_dirty"
+            ):
                 if resource and resource.is_dirty(check_relationship=True):
                     update_dirty(resource)
 
             endpoint_tasks = sorted(
                 self.manager.endpoint_tasks, key=lambda t: t.priority
             )
             immediate_tasks = filter(
@@ -251,15 +255,17 @@
                     and resource
                     and hasattr(resource, "is_dirty")
                     and resource.is_dirty()
                 ):
                     update_dirty(resource)
                 raise
 
-            if hasattr(resource, "is_dirty"):
+            if isinstance(resource, django.db.models.Model) and hasattr(
+                resource, "is_dirty"
+            ):
                 if resource and resource.is_dirty(check_relationship=True):
                     update_dirty(resource)
 
             for deferred_task in deferred_tasks:
                 deferred_task.run(self.bound_endpoint)
 
             if getattr(resource, "_api_filter", False):
@@ -438,16 +444,17 @@
     def process_request_and_get_response(self, request, *args, **kwargs):
         try:
             bound_endpoint = self.bind_endpoint_to_request(request, *args, **kwargs)
             logger.info(
                 "Processing request with handler %s",
                 bound_endpoint.bound_endpoint.__class__.__name__,
             )
-            return bound_endpoint.get_response()
-
+            result = bound_endpoint.get_response()
+            bound_endpoint.bound_endpoint.finalize()
+            return result
         except errors.ApiError:
             raise
         except Exception as e:  # pragma: nocover
             raise errors.ServerError() from e
 
     def __call__(self, *args, **kwargs):
         return self.process_request_and_get_response(*args, **kwargs)
@@ -603,14 +610,21 @@
     @property
     def response(self):
         """
         By default it returns :code:`self.resource` unless it is overridden.
         """
         return self.resource
 
+    def finalize(self):
+        """
+        Called immediately before a response is returned.  Override this method in an
+        Endpoint Definition to perform any clean-up not handled automatically by the framework.
+        """
+        pass
+
     @classmethod
     def get_endpoint_attributes(cls):
         """Returns a list of endpoint attributes
 
         **Example**
         Let’s define an endpoint that updates a single task in a todo list.
 
@@ -985,14 +999,15 @@
             raise errors.ClientErrorUnprocessableEntity(
                 "Unexpected fields: {}".format(", ".join(unexpected))
             )
 
 
 task = EndpointTask
 deferrable_task = DeferrableEndpointTask
+deferrable_generic_task = DeferrableGenericEndpointTask
 request_attribute = RequestAttribute
 consumer_attribute = ConsumerAttribute
 field = RequestField
 resource_field = ResourceField
 url_field = RequestUrlField
 adhoc_queryset = RequestAdhocQuerySet
 aggregate = Aggregate
```

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/attributes.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -726,14 +726,68 @@
                 retry_exception_filter=self.retry_exception_filter,
                 delay=delay,
                 queue=self.queue,
                 routing_key=self.routing_key,
             )
 
 
+class DeferrableGenericEndpointTask(DeferrableEndpointTask):
+    # very similar to DeferrableEndpointTask, but doesn't assume that the resource is a Django model instance
+
+    def __init__(
+        self,
+        task_args_packer=None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        assert (
+            task_args_packer is not None
+        ), "task_args_packer required for DeferrableGenericEndpointTask"
+        self.task_args_packer = task_args_packer
+
+    def _run_task(self, owner_instance):
+        if self.execute_unless and self.execute_unless(owner_instance):
+            return
+
+        delay = self._resolve_maybe_callable(owner_instance, self.delay) or 0
+        always_defer = self._resolve_maybe_callable(owner_instance, self.always_defer)
+        packed_args = self.task_args_packer.pack(owner_instance)
+
+        if delay == 0 and not always_defer:
+            unpacked_args, unpacked_kwargs = self.task_args_packer.unpack(packed_args)
+            self.task_runner(*unpacked_args, **unpacked_kwargs)
+        else:
+            packer_name = "{0}.{1}".format(
+                self.task_args_packer.__module__, self.task_args_packer.__name__
+            )
+
+            endpoint_class_name = "{0}.{1}".format(
+                owner_instance.__module__, owner_instance.__class__.__name__
+            )
+            task_runner_args = (
+                endpoint_class_name,
+                self.task_runner.__name__,
+                packed_args,
+                packer_name,
+            )
+            task_runner_kwargs = {
+                "task_creation_time": time.time(),
+                "scheduled_execution_delay": delay,
+            }
+            tasks.schedule_generic_future_task_runner(
+                task_runner_args,
+                task_runner_kwargs,
+                retries=self.retries,
+                retry_exception_filter=self.retry_exception_filter,
+                delay=delay,
+                queue=self.queue,
+                routing_key=self.routing_key,
+            )
+
+
 class RequestFieldGroup(RequestProperty):
     def __init__(self, *component_field_getters, **kwargs):
         super().__init__(property_getter=self.get_value, **kwargs)
         self.component_field_getters = component_field_getters
         self.component_field_names = []
         for component_field_getter in self.component_field_getters:
             component_field_getter.required = False
```

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/errors.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/errors.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/filtering.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/filtering.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/tasks.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/tasks.py`

 * *Files 25% similar despite different names*

```diff
@@ -145,18 +145,25 @@
     task_creation_time=None,
     scheduled_execution_delay=0,
     task_args=None,
     retry_params=None,
     correlation_id=None,
 ):
     endpoint_class = locate(endpoint_class_name)
-    resource_class = locate(resource_class_name)
-    resource_instance = resource_class.objects.get(pk=resource_instance_id)
     endpoint_task = getattr(endpoint_class, endpoint_method_name)
 
+    provide_resource = (
+        resource_class_name is not None and resource_instance_id is not None
+    )
+    if provide_resource:
+        resource_class = locate(resource_class_name)
+        resource_instance = resource_class.objects.get(pk=resource_instance_id)
+    else:
+        resource_instance = None
+
     _set_correlation_id(correlation_id)
 
     _log_task_stats(
         endpoint_method_name,
         resource_instance_id,
         scheduled_execution_delay,
         task_creation_time,
@@ -172,25 +179,26 @@
 
     if task_args:
         args, kwargs = task_args
     else:
         args, kwargs = [], {}
 
     try:
-        endpoint_task.task_runner(resource_instance, *args, **kwargs)
+        if provide_resource:
+            endpoint_task.task_runner(resource_instance, *args, **kwargs)
+        else:
+            endpoint_task.task_runner(*args, **kwargs)
     except Exception as e:
         if retry_params is None:
             raise
 
         retry_params = RetryParams(*retry_params)
         if retry_params.retry_exception_filter and not any(
-            [
-                f"{e.__class__.__module__}.{e.__class__.__name__}" == ex_type
-                for ex_type in retry_params.retry_exception_filter
-            ]
+            f"{e.__class__.__module__}.{e.__class__.__name__}" == ex_type
+            for ex_type in retry_params.retry_exception_filter
         ):
             # this exception is not retryable
             raise
 
         if retry_params.retries_remaining == 0:
             # out of chances
             raise
@@ -213,23 +221,101 @@
             retries=retry_params.retries_remaining - 1,
             countdown=retry_params.countdown * 2 or 1,
             queue=retry_params.queue,
             routing_key=retry_params.routing_key,
         )
 
 
-def schedule_future_task_runner(
+@celery_task(
+    ignore_results=True,
+    time_limit=getattr(settings, "DDA_DEFERRED_TASK_TIME_LIMIT", 999999),
+    soft_time_limit=getattr(settings, "DDA_DEFERRED_TASK_SOFT_TIME_LIMIT", 999999),
+)
+def generic_future_task_runner(
+    endpoint_class_name,
+    endpoint_method_name,
+    packed_args,
+    packer_class_name,
+    task_job_count=0,
+    task_creation_time=None,
+    scheduled_execution_delay=0,
+    retry_params=None,
+    correlation_id=None,
+):
+    endpoint_class = locate(endpoint_class_name)
+    endpoint_task = getattr(endpoint_class, endpoint_method_name)
+    packer_class = locate(packer_class_name)
+    args, kwargs = packer_class.unpack(packed_args)
+
+    _set_correlation_id(correlation_id)
+
+    _log_task_stats(
+        endpoint_method_name,
+        None,
+        scheduled_execution_delay,
+        task_creation_time,
+        task_job_count,
+        correlation_id,
+    )
+
+    logger.info(
+        "generic_future_task_runner: method=%s, resource_id=%s",
+        endpoint_method_name,
+        None,
+    )
+
+    try:
+        endpoint_task.task_runner(*args, **kwargs)
+    except Exception as e:
+        if retry_params is None:
+            raise
+
+        retry_params = RetryParams(*retry_params)
+        if retry_params.retry_exception_filter and not any(
+            f"{e.__class__.__module__}.{e.__class__.__name__}" == ex_type
+            for ex_type in retry_params.retry_exception_filter
+        ):
+            # this exception is not retryable
+            raise
+
+        if retry_params.retries_remaining == 0:
+            # out of chances
+            raise
+
+        _log_retry_stats(endpoint_method_name, None, correlation_id)
+        task_runner_args = (
+            endpoint_class_name,
+            endpoint_method_name,
+            packed_args,
+            packer_class_name,
+        )
+        task_runner_kwargs = {
+            "task_creation_time": time.time(),
+            "scheduled_execution_delay": scheduled_execution_delay,
+        }
+        schedule_generic_future_task_runner(
+            task_runner_args,
+            task_runner_kwargs,
+            retries=retry_params.retries_remaining - 1,
+            countdown=retry_params.countdown * 2 or 1,
+            queue=retry_params.queue,
+            routing_key=retry_params.routing_key,
+        )
+
+
+def _schedule_task_runner(
     task_runner_args,
     task_runner_kwargs,
     retries=0,
     retry_exception_filter=(),
     queue=None,
     routing_key=None,
     countdown=0,
     delay=0,
+    runner_fn=None,
 ):
     task_runner_kwargs["task_job_count"] = _get_task_job_count()
     task_runner_kwargs["retry_params"] = RetryParams(
         retries_remaining=retries,
         retry_exception_filter=tuple(
             f"{exc.__module__}.{exc.__name__}" for exc in retry_exception_filter
         ),
@@ -237,28 +323,28 @@
         routing_key=routing_key,
         countdown=countdown,
     )
     task_runner_kwargs["correlation_id"] = _get_correlation_id()
 
     if getattr(settings, "DECLARATIVE_ENDPOINT_TASKS_FORCE_SYNCHRONOUS", False):
         logger.info("Processing tasks synchronously")
-        future_task_runner.apply(task_runner_args, task_runner_kwargs)
+        runner_fn.apply(task_runner_args, task_runner_kwargs)
     else:
         MAX_ATTEMPTS = 3
         for attempt in range(MAX_ATTEMPTS):
             # XXX: This is an attempt to skirt around an unsolved, low repro
             # issue somewhere in the celery/kombu/redis-py stack.  Once in a
             # while, a connection in the pool will timeout prior to a health
             # check being called in redis-py and will result in an error being
             # raised here. This should be removed once the issue has been
             # sorted out.  Note: This is around the use of redis-py in celery
             # where celery's event loop is not running
             # https://github.com/celery/kombu/issues/1019
             try:
-                future_task_runner.apply_async(
+                runner_fn.apply_async(
                     task_runner_args,
                     task_runner_kwargs,
                     queue=queue,
                     routing_key=routing_key,
                     countdown=countdown + delay,
                 )
                 return
@@ -267,19 +353,65 @@
                     "kombu.exceptions.OperationalError (attempt: %s)", attempt
                 )
                 if attempt >= MAX_ATTEMPTS - 1:
                     if getattr(
                         settings, "DECLARATIVE_ENDPOINT_TASKS_SYNCHRONOUS_FALLBACK"
                     ):
                         logger.warning("Falling back to executing task synchronously")
-                        future_task_runner.apply(task_runner_args, task_runner_kwargs)
+                        runner_fn.apply(task_runner_args, task_runner_kwargs)
                         return
                     raise err
 
 
+def schedule_future_task_runner(
+    task_runner_args,
+    task_runner_kwargs,
+    retries=0,
+    retry_exception_filter=(),
+    queue=None,
+    routing_key=None,
+    countdown=0,
+    delay=0,
+):
+    _schedule_task_runner(
+        task_runner_args=task_runner_args,
+        task_runner_kwargs=task_runner_kwargs,
+        retries=retries,
+        retry_exception_filter=retry_exception_filter,
+        queue=queue,
+        routing_key=routing_key,
+        countdown=countdown,
+        delay=delay,
+        runner_fn=future_task_runner,
+    )
+
+
+def schedule_generic_future_task_runner(
+    task_runner_args,
+    task_runner_kwargs,
+    retries=0,
+    retry_exception_filter=(),
+    queue=None,
+    routing_key=None,
+    countdown=0,
+    delay=0,
+):
+    _schedule_task_runner(
+        task_runner_args=task_runner_args,
+        task_runner_kwargs=task_runner_kwargs,
+        retries=retries,
+        retry_exception_filter=retry_exception_filter,
+        queue=queue,
+        routing_key=routing_key,
+        countdown=countdown,
+        delay=delay,
+        runner_fn=generic_future_task_runner,
+    )
+
+
 @celery_task(
     ignore_results=True,
     time_limit=getattr(settings, "DDA_DEFERRED_TASK_TIME_LIMIT", 999999),
     soft_time_limit=getattr(settings, "DDA_DEFERRED_TASK_SOFT_TIME_LIMIT", 999999),
 )
 def resource_task_runner(
     resource_class_name,
```

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/machinery/utils.py` & `django-declarative-apis-0.27.0/django_declarative_apis/machinery/utils.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/management/commands/gendocs.py` & `django-declarative-apis-0.27.0/django_declarative_apis/management/commands/gendocs.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/migrations/0001_initial.py` & `django-declarative-apis-0.27.0/django_declarative_apis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/migrations/0002_add_consumer_type_field.py` & `django-declarative-apis-0.27.0/django_declarative_apis/migrations/0002_add_consumer_type_field.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/models.py` & `django-declarative-apis-0.27.0/django_declarative_apis/models.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/resources/emitters.py` & `django-declarative-apis-0.27.0/django_declarative_apis/resources/emitters.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/resources/resource.py` & `django-declarative-apis-0.27.0/django_declarative_apis/resources/resource.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis/resources/utils.py` & `django-declarative-apis-0.27.0/django_declarative_apis/resources/utils.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis.egg-info/PKG-INFO` & `django-declarative-apis-0.27.0/django_declarative_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-declarative-apis
-Version: 0.26.0
+Version: 0.27.0
 Summary: Simple, readable, declarative APIs for Django
 Keywords: django,rest,declarative,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-declarative-apis-0.26.0/django_declarative_apis.egg-info/SOURCES.txt` & `django-declarative-apis-0.27.0/django_declarative_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/pyproject.toml` & `django-declarative-apis-0.27.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-declarative-apis"
-version = "0.26.0"  # set by bumpversion
+version = "0.27.0"  # set by bumpversion
 description = "Simple, readable, declarative APIs for Django"
 readme = "README.md"
 dependencies = [
   "Django >=3.2, <4",
   "celery>=4.0.2,!=4.1.0",
   "cryptography>=2.0",
   "decorator==4.0.11",
```

### Comparing `django-declarative-apis-0.26.0/tests/test_adapters.py` & `django-declarative-apis-0.27.0/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/tests/test_filters.py` & `django-declarative-apis-0.27.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/tests/test_models.py` & `django-declarative-apis-0.27.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/tests/tests.py` & `django-declarative-apis-0.27.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-declarative-apis-0.26.0/tests/testutils.py` & `django-declarative-apis-0.27.0/tests/testutils.py`

 * *Files identical despite different names*

