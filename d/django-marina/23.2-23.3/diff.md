# Comparing `tmp/django-marina-23.2.tar.gz` & `tmp/django-marina-23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-marina-23.2.tar", last modified: Sat Apr 22 11:17:04 2023, max compression
+gzip compressed data, was "django-marina-23.3.tar", last modified: Fri Apr 28 10:18:00 2023, max compression
```

## Comparing `django-marina-23.2.tar` & `django-marina-23.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011949 django-marina-23.2/
--rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.2/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      278 2023-04-22 11:05:50.000000 django-marina-23.2/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-22 11:17:04.012023 django-marina-23.2/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      666 2020-10-31 06:45:14.000000 django-marina-23.2/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.007255 django-marina-23.2/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-14 04:57:27.000000 django-marina-23.2/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      905 2023-04-22 08:41:12.000000 django-marina-23.2/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      217 2021-12-04 17:34:31.000000 django-marina-23.2/docs/db.rst
--rw-r--r--   0 dylan      (501) staff       (20)      152 2020-06-15 12:42:52.000000 django-marina-23.2/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-22 08:41:12.000000 django-marina-23.2/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)      220 2022-01-03 06:11:13.000000 django-marina-23.2/docs/test.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.2/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     1148 2022-03-31 10:40:02.000000 django-marina-23.2/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)     1217 2023-04-22 11:17:04.012278 django-marina-23.2/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.004782 django-marina-23.2/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.007844 django-marina-23.2/src/django_marina/
--rw-r--r--   0 dylan      (501) staff       (20)      264 2020-11-02 05:49:45.000000 django-marina-23.2/src/django_marina/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.009144 django-marina-23.2/src/django_marina/db/
--rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.2/src/django_marina/db/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)      717 2020-06-15 12:42:52.000000 django-marina-23.2/src/django_marina/db/migrations.py
--rw-r--r--   0 dylan      (501) staff       (20)     1998 2021-05-31 06:50:39.000000 django-marina-23.2/src/django_marina/db/models.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.009490 django-marina-23.2/src/django_marina/test/
--rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.2/src/django_marina/test/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.2/src/django_marina/test/clients.py
--rw-r--r--   0 dylan      (501) staff       (20)     9271 2023-04-22 08:41:12.000000 django-marina-23.2/src/django_marina/test/test_cases.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.008806 django-marina-23.2/src/django_marina.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1786 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      899 2023-04-22 11:17:04.000000 django-marina-23.2/src/django_marina.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-04-09 08:22:42.000000 django-marina-23.2/src/django_marina.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       80 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       14 2023-04-22 11:17:03.000000 django-marina-23.2/src/django_marina.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011054 django-marina-23.2/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.2/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-22 11:17:04.011808 django-marina-23.2/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.2/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.2/tests/app/views.py
--rw-r--r--   0 dylan      (501) staff       (20)      617 2021-04-13 10:45:33.000000 django-marina-23.2/tests/models.py
--rw-r--r--   0 dylan      (501) staff       (20)     1995 2021-04-23 08:20:35.000000 django-marina-23.2/tests/test_db.py
--rw-r--r--   0 dylan      (501) staff       (20)      694 2020-07-20 04:35:29.000000 django-marina-23.2/tests/test_extended_client.py
--rw-r--r--   0 dylan      (501) staff       (20)     8518 2021-12-04 17:34:51.000000 django-marina-23.2/tests/test_extended_test_case.py
--rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.2/tests/test_imports.py
--rw-r--r--   0 dylan      (501) staff       (20)      303 2021-12-04 17:34:51.000000 django-marina-23.2/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.2/tests/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     2323 2023-04-14 10:12:52.000000 django-marina-23.2/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.478948 django-marina-23.3/
+-rw-r--r--   0 dylan      (501) staff       (20)     1456 2019-04-27 05:10:10.000000 django-marina-23.3/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)      281 2023-04-25 19:11:55.000000 django-marina-23.3/MANIFEST.in
+-rw-r--r--   0 dylan      (501) staff       (20)     1747 2023-04-28 10:18:00.479018 django-marina-23.3/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      666 2020-10-31 06:45:14.000000 django-marina-23.3/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.474386 django-marina-23.3/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       30 2020-06-14 04:57:27.000000 django-marina-23.3/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1023 2023-04-27 11:05:22.000000 django-marina-23.3/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)      217 2021-12-04 17:34:31.000000 django-marina-23.3/docs/db.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      152 2020-06-15 12:42:52.000000 django-marina-23.3/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-27 10:53:35.000000 django-marina-23.3/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      220 2022-01-03 06:11:13.000000 django-marina-23.3/docs/test.rst
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-04-09 08:10:13.000000 django-marina-23.3/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1368 2023-04-26 05:42:59.000000 django-marina-23.3/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)     1175 2023-04-28 10:18:00.479442 django-marina-23.3/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.471983 django-marina-23.3/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.474493 django-marina-23.3/src/django_marina/
+-rw-r--r--   0 dylan      (501) staff       (20)       55 2023-04-28 10:17:53.000000 django-marina-23.3/src/django_marina/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475633 django-marina-23.3/src/django_marina/db/
+-rw-r--r--   0 dylan      (501) staff       (20)      138 2020-06-15 08:02:46.000000 django-marina-23.3/src/django_marina/db/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)      709 2023-04-25 07:56:49.000000 django-marina-23.3/src/django_marina/db/migrations.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1998 2023-04-23 07:42:51.000000 django-marina-23.3/src/django_marina/db/models.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475968 django-marina-23.3/src/django_marina/test/
+-rw-r--r--   0 dylan      (501) staff       (20)      127 2021-12-04 17:34:31.000000 django-marina-23.3/src/django_marina/test/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1908 2021-07-01 04:27:53.000000 django-marina-23.3/src/django_marina/test/clients.py
+-rw-r--r--   0 dylan      (501) staff       (20)     9271 2023-04-23 07:48:36.000000 django-marina-23.3/src/django_marina/test/test_cases.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.475298 django-marina-23.3/src/django_marina.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1747 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      899 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-26 05:41:51.000000 django-marina-23.3/src/django_marina.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)       34 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       14 2023-04-28 10:18:00.000000 django-marina-23.3/src/django_marina.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.477971 django-marina-23.3/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-11 08:49:17.000000 django-marina-23.3/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 10:18:00.478791 django-marina-23.3/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2020-06-13 09:16:54.000000 django-marina-23.3/tests/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1525 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)      616 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1832 2021-04-28 07:14:00.000000 django-marina-23.3/tests/app/views.py
+-rw-r--r--   0 dylan      (501) staff       (20)      617 2023-04-23 07:22:32.000000 django-marina-23.3/tests/models.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1995 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_db.py
+-rw-r--r--   0 dylan      (501) staff       (20)      694 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_extended_client.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8518 2023-04-23 07:22:32.000000 django-marina-23.3/tests/test_extended_test_case.py
+-rw-r--r--   0 dylan      (501) staff       (20)      547 2020-06-15 08:02:46.000000 django-marina-23.3/tests/test_imports.py
+-rw-r--r--   0 dylan      (501) staff       (20)      303 2021-12-04 17:34:51.000000 django-marina-23.3/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)      768 2019-06-10 07:50:32.000000 django-marina-23.3/tests/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1996 2023-04-27 10:53:35.000000 django-marina-23.3/tox.ini
```

### Comparing `django-marina-23.2/LICENSE` & `django-marina-23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/PKG-INFO` & `django-marina-23.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.2
+Version: 23.3
 Summary: Django extensions by Zostera
 Home-page: https://github.com/zostera/django-marina
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-marina-23.2/README.md` & `django-marina-23.3/README.md`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/src/django_marina/db/migrations.py` & `django-marina-23.3/src/django_marina/db/migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-class DisableMigrations(object):
+class DisableMigrations:
     """
     Settings class to disable migrations.
 
     In your `settings_test.py` you can set MIGRATION_MODULES, for example:
 
     .. code-block:: python
```

### Comparing `django-marina-23.2/src/django_marina/db/models.py` & `django-marina-23.3/src/django_marina/db/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/src/django_marina/test/clients.py` & `django-marina-23.3/src/django_marina/test/clients.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/src/django_marina/test/test_cases.py` & `django-marina-23.3/src/django_marina/test/test_cases.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/src/django_marina.egg-info/PKG-INFO` & `django-marina-23.3/src/django_marina.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-marina
-Version: 23.2
+Version: 23.3
 Summary: Django extensions by Zostera
 Home-page: https://github.com/zostera/django-marina
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-marina-23.2/src/django_marina.egg-info/SOURCES.txt` & `django-marina-23.3/src/django_marina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/app/settings.py` & `django-marina-23.3/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/app/urls.py` & `django-marina-23.3/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/app/views.py` & `django-marina-23.3/tests/app/views.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/models.py` & `django-marina-23.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/test_db.py` & `django-marina-23.3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/test_extended_client.py` & `django-marina-23.3/tests/test_extended_client.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/test_extended_test_case.py` & `django-marina-23.3/tests/test_extended_test_case.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/test_imports.py` & `django-marina-23.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tests/urls.py` & `django-marina-23.3/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-marina-23.2/tox.ini` & `django-marina-23.3/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tox]
 isolated_build = True
 envlist =
     lint
     docs
     py37-django{32}
-    py38-django{32,40,41,42}
-    py39-django{32,40,41,42}
-    py310-django{32,40,41,42,main}
-    py311-django{32,40,41,42,main}
+    py38-django{32,41,42}
+    py39-django{32,41,42}
+    py310-django{32,41,42,main}
+    py311-django{41,42,main}
     check-description
     check-manifest
     coverage
 
 [gh-actions]
 python =
     3.7: py37
@@ -25,24 +25,22 @@
     make
 setenv =
     PYTHONWARNINGS=once::DeprecationWarning
 commands =
     coverage run --parallel-mode manage.py test -v1 --noinput
 deps =
     django32: Django==3.2.*
-    django40: Django==4.0.*
     django41: Django==4.1.*
     django42: Django==4.2.*
     djangomain: https://github.com/django/django/archive/main.tar.gz
     coverage[toml]
-    coveralls
 
 [testenv:coverage]
 depends =
-    py37,py38,py39,py310
+    py37,py38,py39,py310,py311
 commands =
     coverage combine
     coverage report
 
 [testenv:lint]
 commands =
     make lint
@@ -59,34 +57,25 @@
 # correctly when uploaded to the Python Package Index, or fail if not.
 [testenv:check-description]
 description = Check that the package description will render on the Python Package Index.
 basepython = python3.9
 changedir = {toxinidir}
 skip_install = true
 deps =
-  twine
+    twine
 # In this environment, we need latest the pip, setuptools, and wheel.
 commands_pre =
-  {envpython} -m pip install -U pip setuptools wheel
+    {envpython} -m pip install -U pip setuptools wheel
 commands =
     make check-description
 # Runs check-manifest, a tool that builds the package and compares the
 # files in the package to the files under version control, and fails
 # if any version-controlled files do not end up in the package.
 [testenv:check-manifest]
 description = Check that the set of packaged files matches the set of version-controlled files.
 basepython = python3.9
 changedir = {toxinidir}
 skip_install = true
 deps =
-  check-manifest
+    check-manifest
 commands =
-  make check-manifest
-
-[flake8]
-# flake8 does not support pyproject.toml, so we use tox.ini
-# E731 do not assign a lambda expression
-# W503 line break before binary operator (black introduces these)
-# E203 whitespace before ':'
-ignore = E731,W503,E203
-exclude = .git,.tox,__pycache__
-max-line-length = 120
+    make check-manifest
```

