# Comparing `tmp/django-drf-cms-0.1.1.tar.gz` & `tmp/django-drf-cms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-cms-0.1.1.tar", last modified: Fri Apr 28 17:18:01 2023, max compression
+gzip compressed data, was "django-drf-cms-0.1.2.tar", last modified: Fri Apr 28 17:20:25 2023, max compression
```

## Comparing `django-drf-cms-0.1.1.tar` & `django-drf-cms-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:18:01.094016 django-drf-cms-0.1.1/
--rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.1/LICENSE
--rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.1/MANIFEST.in
--rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 17:18:01.094125 django-drf-cms-0.1.1/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      666 2023-04-28 16:32:17.000000 django-drf-cms-0.1.1/README.rst
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:18:01.089042 django-drf-cms-0.1.1/django_drf_cms.egg-info/
--rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 17:18:01.000000 django-drf-cms-0.1.1/django_drf_cms.egg-info/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      677 2023-04-28 17:18:01.000000 django-drf-cms-0.1.1/django_drf_cms.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-28 17:18:01.000000 django-drf-cms-0.1.1/django_drf_cms.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (501) staff       (20)       93 2023-04-28 17:18:01.000000 django-drf-cms-0.1.1/django_drf_cms.egg-info/requires.txt
--rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-28 17:18:01.000000 django-drf-cms-0.1.1/django_drf_cms.egg-info/top_level.txt
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:18:01.092550 django-drf-cms-0.1.1/drf_cms/
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.1/drf_cms/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      311 2023-04-26 17:49:50.000000 django-drf-cms-0.1.1/drf_cms/admin.py
--rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.1/drf_cms/apps.py
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:18:01.093845 django-drf-cms-0.1.1/drf_cms/migrations/
--rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.1/drf_cms/migrations/0001_initial.py
--rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.1/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
--rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.1/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.1/drf_cms/migrations/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      905 2023-04-27 10:37:26.000000 django-drf-cms-0.1.1/drf_cms/models.py
--rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.1/drf_cms/permissions.py
--rw-r--r--   0 luis       (501) staff       (20)      644 2023-04-27 14:35:09.000000 django-drf-cms-0.1.1/drf_cms/serializers.py
--rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.1/drf_cms/shortcuts.py
--rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.1/drf_cms/tests.py
--rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.1/drf_cms/translation.py
--rw-r--r--   0 luis       (501) staff       (20)      361 2023-04-26 17:44:37.000000 django-drf-cms-0.1.1/drf_cms/urls.py
--rw-r--r--   0 luis       (501) staff       (20)     1386 2023-04-27 14:29:32.000000 django-drf-cms-0.1.1/drf_cms/views.py
--rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.1/pyproject.toml
--rw-r--r--   0 luis       (501) staff       (20)      995 2023-04-28 17:18:01.095508 django-drf-cms-0.1.1/setup.cfg
--rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.1/setup.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:20:25.955002 django-drf-cms-0.1.2/
+-rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.2/LICENSE
+-rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.2/MANIFEST.in
+-rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 17:20:25.955125 django-drf-cms-0.1.2/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      666 2023-04-28 16:32:17.000000 django-drf-cms-0.1.2/README.rst
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:20:25.950399 django-drf-cms-0.1.2/django_drf_cms.egg-info/
+-rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 17:20:25.000000 django-drf-cms-0.1.2/django_drf_cms.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      677 2023-04-28 17:20:25.000000 django-drf-cms-0.1.2/django_drf_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-28 17:20:25.000000 django-drf-cms-0.1.2/django_drf_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (501) staff       (20)       93 2023-04-28 17:20:25.000000 django-drf-cms-0.1.2/django_drf_cms.egg-info/requires.txt
+-rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-28 17:20:25.000000 django-drf-cms-0.1.2/django_drf_cms.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:20:25.953588 django-drf-cms-0.1.2/drf_cms/
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.2/drf_cms/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      311 2023-04-26 17:49:50.000000 django-drf-cms-0.1.2/drf_cms/admin.py
+-rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.2/drf_cms/apps.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 17:20:25.954804 django-drf-cms-0.1.2/drf_cms/migrations/
+-rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.2/drf_cms/migrations/0001_initial.py
+-rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.2/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
+-rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.2/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.2/drf_cms/migrations/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      905 2023-04-27 10:37:26.000000 django-drf-cms-0.1.2/drf_cms/models.py
+-rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.2/drf_cms/permissions.py
+-rw-r--r--   0 luis       (501) staff       (20)      644 2023-04-27 14:35:09.000000 django-drf-cms-0.1.2/drf_cms/serializers.py
+-rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.2/drf_cms/shortcuts.py
+-rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.2/drf_cms/tests.py
+-rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.2/drf_cms/translation.py
+-rw-r--r--   0 luis       (501) staff       (20)      361 2023-04-26 17:44:37.000000 django-drf-cms-0.1.2/drf_cms/urls.py
+-rw-r--r--   0 luis       (501) staff       (20)     1383 2023-04-28 17:20:05.000000 django-drf-cms-0.1.2/drf_cms/views.py
+-rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.2/pyproject.toml
+-rw-r--r--   0 luis       (501) staff       (20)      995 2023-04-28 17:20:25.955783 django-drf-cms-0.1.2/setup.cfg
+-rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.2/setup.py
```

### Comparing `django-drf-cms-0.1.1/LICENSE` & `django-drf-cms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/PKG-INFO` & `django-drf-cms-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.1/README.rst` & `django-drf-cms-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/django_drf_cms.egg-info/PKG-INFO` & `django-drf-cms-0.1.2/django_drf_cms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-cms-0.1.1/django_drf_cms.egg-info/SOURCES.txt` & `django-drf-cms-0.1.2/django_drf_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/migrations/0001_initial.py` & `django-drf-cms-0.1.2/drf_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py` & `django-drf-cms-0.1.2/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/models.py` & `django-drf-cms-0.1.2/drf_cms/models.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/permissions.py` & `django-drf-cms-0.1.2/drf_cms/permissions.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/serializers.py` & `django-drf-cms-0.1.2/drf_cms/serializers.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.1/drf_cms/views.py` & `django-drf-cms-0.1.2/drf_cms/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.shortcuts import render
 from rest_framework import generics, mixins
 from .models import Text
 from .serializers import *
 from .permissions import IsOwnerOrReadOnly
-from cms.shortcuts import get_current_site
+from .shortcuts import get_current_site
 
 
 class TextView(
 		mixins.ListModelMixin, 
 		mixins.RetrieveModelMixin,
 		mixins.UpdateModelMixin,
 		generics.GenericAPIView):
```

### Comparing `django-drf-cms-0.1.1/setup.cfg` & `django-drf-cms-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-drf-cms
-version = 0.1.1
+version = 0.1.2
 description = A Django app to build a simple cms restful server.
 long_description = file: README.rst
 url = https://www.spartanbits.com
 author = Spartanbits, SLU
 author_email = info@spartanbits.com
 license = Apache-2.0
 classifiers =
```

