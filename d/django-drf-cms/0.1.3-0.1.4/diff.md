# Comparing `tmp/django-drf-cms-0.1.3.tar.gz` & `tmp/django-drf-cms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-cms-0.1.3.tar", last modified: Fri Apr 28 18:07:12 2023, max compression
+gzip compressed data, was "django-drf-cms-0.1.4.tar", last modified: Fri Apr 28 18:09:57 2023, max compression
```

## Comparing `django-drf-cms-0.1.3.tar` & `django-drf-cms-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:07:12.697228 django-drf-cms-0.1.3/
--rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.3/LICENSE
--rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.3/MANIFEST.in
--rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 18:07:12.697365 django-drf-cms-0.1.3/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      666 2023-04-28 16:32:17.000000 django-drf-cms-0.1.3/README.rst
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:07:12.686499 django-drf-cms-0.1.3/django_drf_cms.egg-info/
--rw-r--r--   0 luis       (501) staff       (20)     1567 2023-04-28 18:07:12.000000 django-drf-cms-0.1.3/django_drf_cms.egg-info/PKG-INFO
--rw-r--r--   0 luis       (501) staff       (20)      677 2023-04-28 18:07:12.000000 django-drf-cms-0.1.3/django_drf_cms.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-28 18:07:12.000000 django-drf-cms-0.1.3/django_drf_cms.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (501) staff       (20)       93 2023-04-28 18:07:12.000000 django-drf-cms-0.1.3/django_drf_cms.egg-info/requires.txt
--rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-28 18:07:12.000000 django-drf-cms-0.1.3/django_drf_cms.egg-info/top_level.txt
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:07:12.694242 django-drf-cms-0.1.3/drf_cms/
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.3/drf_cms/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      311 2023-04-26 17:49:50.000000 django-drf-cms-0.1.3/drf_cms/admin.py
--rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.3/drf_cms/apps.py
-drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:07:12.697031 django-drf-cms-0.1.3/drf_cms/migrations/
--rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.3/drf_cms/migrations/0001_initial.py
--rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.3/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
--rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.3/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
--rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.3/drf_cms/migrations/__init__.py
--rw-r--r--   0 luis       (501) staff       (20)      905 2023-04-27 10:37:26.000000 django-drf-cms-0.1.3/drf_cms/models.py
--rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.3/drf_cms/permissions.py
--rw-r--r--   0 luis       (501) staff       (20)      644 2023-04-27 14:35:09.000000 django-drf-cms-0.1.3/drf_cms/serializers.py
--rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.3/drf_cms/shortcuts.py
--rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.3/drf_cms/tests.py
--rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.3/drf_cms/translation.py
--rw-r--r--   0 luis       (501) staff       (20)      361 2023-04-26 17:44:37.000000 django-drf-cms-0.1.3/drf_cms/urls.py
--rw-r--r--   0 luis       (501) staff       (20)     1383 2023-04-28 17:20:05.000000 django-drf-cms-0.1.3/drf_cms/views.py
--rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.3/pyproject.toml
--rw-r--r--   0 luis       (501) staff       (20)      995 2023-04-28 18:07:12.698046 django-drf-cms-0.1.3/setup.cfg
--rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.3/setup.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:09:57.140832 django-drf-cms-0.1.4/
+-rw-r--r--   0 luis       (501) staff       (20)    10936 2023-04-28 16:21:49.000000 django-drf-cms-0.1.4/LICENSE
+-rw-r--r--   0 luis       (501) staff       (20)       59 2023-04-28 16:22:53.000000 django-drf-cms-0.1.4/MANIFEST.in
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-28 18:09:57.140988 django-drf-cms-0.1.4/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      525 2023-04-28 18:09:25.000000 django-drf-cms-0.1.4/README.rst
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:09:57.111234 django-drf-cms-0.1.4/django_drf_cms.egg-info/
+-rw-r--r--   0 luis       (501) staff       (20)     1426 2023-04-28 18:09:57.000000 django-drf-cms-0.1.4/django_drf_cms.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (501) staff       (20)      677 2023-04-28 18:09:57.000000 django-drf-cms-0.1.4/django_drf_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (501) staff       (20)        1 2023-04-28 18:09:57.000000 django-drf-cms-0.1.4/django_drf_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (501) staff       (20)       93 2023-04-28 18:09:57.000000 django-drf-cms-0.1.4/django_drf_cms.egg-info/requires.txt
+-rw-r--r--   0 luis       (501) staff       (20)        8 2023-04-28 18:09:57.000000 django-drf-cms-0.1.4/django_drf_cms.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:09:57.137531 django-drf-cms-0.1.4/drf_cms/
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.4/drf_cms/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      311 2023-04-26 17:49:50.000000 django-drf-cms-0.1.4/drf_cms/admin.py
+-rw-r--r--   0 luis       (501) staff       (20)      146 2023-04-28 08:58:59.000000 django-drf-cms-0.1.4/drf_cms/apps.py
+drwxr-xr-x   0 luis       (501) staff       (20)        0 2023-04-28 18:09:57.140584 django-drf-cms-0.1.4/drf_cms/migrations/
+-rw-r--r--   0 luis       (501) staff       (20)     1589 2023-04-28 08:59:14.000000 django-drf-cms-0.1.4/drf_cms/migrations/0001_initial.py
+-rw-r--r--   0 luis       (501) staff       (20)      434 2023-04-28 08:59:28.000000 django-drf-cms-0.1.4/drf_cms/migrations/0002_alter_text_unique_together_remove_text_site.py
+-rw-r--r--   0 luis       (501) staff       (20)     1302 2023-04-28 08:59:32.000000 django-drf-cms-0.1.4/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py
+-rw-r--r--   0 luis       (501) staff       (20)        0 2023-04-25 16:49:24.000000 django-drf-cms-0.1.4/drf_cms/migrations/__init__.py
+-rw-r--r--   0 luis       (501) staff       (20)      905 2023-04-27 10:37:26.000000 django-drf-cms-0.1.4/drf_cms/models.py
+-rw-r--r--   0 luis       (501) staff       (20)      657 2023-04-28 17:17:06.000000 django-drf-cms-0.1.4/drf_cms/permissions.py
+-rw-r--r--   0 luis       (501) staff       (20)      644 2023-04-27 14:35:09.000000 django-drf-cms-0.1.4/drf_cms/serializers.py
+-rw-r--r--   0 luis       (501) staff       (20)      155 2023-04-28 17:14:19.000000 django-drf-cms-0.1.4/drf_cms/shortcuts.py
+-rw-r--r--   0 luis       (501) staff       (20)       60 2023-04-25 16:49:24.000000 django-drf-cms-0.1.4/drf_cms/tests.py
+-rw-r--r--   0 luis       (501) staff       (20)      302 2023-04-27 09:47:04.000000 django-drf-cms-0.1.4/drf_cms/translation.py
+-rw-r--r--   0 luis       (501) staff       (20)      361 2023-04-26 17:44:37.000000 django-drf-cms-0.1.4/drf_cms/urls.py
+-rw-r--r--   0 luis       (501) staff       (20)     1383 2023-04-28 17:20:05.000000 django-drf-cms-0.1.4/drf_cms/views.py
+-rw-r--r--   0 luis       (501) staff       (20)      108 2023-04-28 09:01:41.000000 django-drf-cms-0.1.4/pyproject.toml
+-rw-r--r--   0 luis       (501) staff       (20)      995 2023-04-28 18:09:57.141826 django-drf-cms-0.1.4/setup.cfg
+-rw-r--r--   0 luis       (501) staff       (20)       37 2023-04-28 09:16:43.000000 django-drf-cms-0.1.4/setup.py
```

### Comparing `django-drf-cms-0.1.3/LICENSE` & `django-drf-cms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/PKG-INFO` & `django-drf-cms-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -36,15 +36,13 @@
 1. Add "cms" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...
         'drf_cms',
     ]
 
-2. Include the polls URLconf in your project urls.py like this::
+2. Include the drf-cms URLconf in your project urls.py like this::
 
     path('cms/', include('drf_cms.urls')),
 
 3. Run ``python manage.py migrate`` to create the cms models.
 
-4. Start the development server and visit http://127.0.0.1:8000/admin/
-   to create cms pages and content (you'll need the Admin app enabled).
```

### Comparing `django-drf-cms-0.1.3/django_drf_cms.egg-info/PKG-INFO` & `django-drf-cms-0.1.4/django_drf_cms.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-cms
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django app to build a simple cms restful server.
 Home-page: https://www.spartanbits.com
 Author: Spartanbits, SLU
 Author-email: info@spartanbits.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -36,15 +36,13 @@
 1. Add "cms" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...
         'drf_cms',
     ]
 
-2. Include the polls URLconf in your project urls.py like this::
+2. Include the drf-cms URLconf in your project urls.py like this::
 
     path('cms/', include('drf_cms.urls')),
 
 3. Run ``python manage.py migrate`` to create the cms models.
 
-4. Start the development server and visit http://127.0.0.1:8000/admin/
-   to create cms pages and content (you'll need the Admin app enabled).
```

### Comparing `django-drf-cms-0.1.3/django_drf_cms.egg-info/SOURCES.txt` & `django-drf-cms-0.1.4/django_drf_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/migrations/0001_initial.py` & `django-drf-cms-0.1.4/drf_cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py` & `django-drf-cms-0.1.4/drf_cms/migrations/0003_page_description_en_page_description_es_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/models.py` & `django-drf-cms-0.1.4/drf_cms/models.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/permissions.py` & `django-drf-cms-0.1.4/drf_cms/permissions.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/serializers.py` & `django-drf-cms-0.1.4/drf_cms/serializers.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/drf_cms/views.py` & `django-drf-cms-0.1.4/drf_cms/views.py`

 * *Files identical despite different names*

### Comparing `django-drf-cms-0.1.3/setup.cfg` & `django-drf-cms-0.1.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-drf-cms
-version = 0.1.3
+version = 0.1.4
 description = A Django app to build a simple cms restful server.
 long_description = file: README.rst
 url = https://www.spartanbits.com
 author = Spartanbits, SLU
 author_email = info@spartanbits.com
 license = Apache-2.0
 classifiers =
```

