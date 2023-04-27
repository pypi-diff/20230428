# Comparing `tmp/djangobible-0.0.8.tar.gz` & `tmp/djangobible-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangobible-0.0.8.tar", last modified: Tue Oct 27 18:25:51 2020, max compression
+gzip compressed data, was "djangobible-0.0.9.tar", last modified: Wed Oct 28 02:01:19 2020, max compression
```

## Comparing `djangobible-0.0.8.tar` & `djangobible-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2262 2020-10-27 18:00:12.441457 djangobible-0.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      715 2020-10-27 17:48:39.342953 djangobible-0.0.8/.github/workflows/django.yml
--rw-r--r--   0        0        0     1971 2020-10-09 03:33:01.891952 djangobible-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-10-09 03:33:01.895945 djangobible-0.0.8/LICENSE
--rw-r--r--   0        0        0     1170 2020-10-27 18:24:04.183073 djangobible-0.0.8/README.md
--rw-r--r--   0        0        0       45 2020-10-18 23:43:36.419870 djangobible-0.0.8/__init__.py
--rw-r--r--   0        0        0      206 2020-10-27 18:24:26.951228 djangobible-0.0.8/djangobible/__init__.py
--rw-r--r--   0        0        0      102 2020-10-10 02:15:26.841191 djangobible-0.0.8/djangobible/apps.py
--rw-r--r--   0        0        0     1207 2020-10-10 02:15:26.901189 djangobible-0.0.8/djangobible/migrations/0001_initial.py
--rw-r--r--   0        0        0       58 2020-10-18 23:25:04.976566 djangobible-0.0.8/djangobible/migrations/__init__.py
--rw-r--r--   0        0        0     2155 2020-10-18 23:44:20.371406 djangobible-0.0.8/djangobible/models.py
--rw-r--r--   0        0        0      697 2020-10-18 23:44:20.327402 djangobible-0.0.8/manage.py
--rw-r--r--   0        0        0      659 2020-10-27 18:22:38.475332 djangobible-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      177 2020-10-10 02:09:17.806309 djangobible-0.0.8/pytest.ini
--rw-r--r--   0        0        0       36 2020-10-18 23:36:32.169986 djangobible-0.0.8/requirements.txt
--rw-r--r--   0        0        0       58 2020-10-12 15:35:46.348106 djangobible-0.0.8/test_django_app/__init__.py
--rw-r--r--   0        0        0      108 2020-10-10 02:15:31.876139 djangobible-0.0.8/test_django_app/apps.py
--rw-r--r--   0        0        0      766 2020-10-10 02:15:31.924137 djangobible-0.0.8/test_django_app/migrations/0001_initial.py
--rw-r--r--   0        0        0       63 2020-10-18 23:25:04.958460 djangobible-0.0.8/test_django_app/migrations/__init__.py
--rw-r--r--   0        0        0      332 2020-10-18 23:37:19.553224 djangobible-0.0.8/test_django_app/models.py
--rw-r--r--   0        0        0       49 2020-10-18 23:26:36.754738 djangobible-0.0.8/test_django_app/tests/__init__.py
--rw-r--r--   0        0        0     2261 2020-10-10 20:06:34.269947 djangobible-0.0.8/test_django_app/tests/conftest.py
--rw-r--r--   0        0        0     2533 2020-10-12 15:15:27.198297 djangobible-0.0.8/test_django_app/tests/test_models.py
--rw-r--r--   0        0        0      823 2020-10-10 20:06:34.221952 djangobible-0.0.8/test_django_app/tests/test_search.py
--rw-r--r--   0        0        0       62 2020-10-18 23:21:06.336139 djangobible-0.0.8/test_django_project/__init__.py
--rw-r--r--   0        0        0      431 2020-10-18 23:32:52.973212 djangobible-0.0.8/test_django_project/asgi.py
--rw-r--r--   0        0        0     3333 2020-10-18 23:32:46.749700 djangobible-0.0.8/test_django_project/settings.py
--rw-r--r--   0        0        0      784 2020-10-18 23:31:50.265596 djangobible-0.0.8/test_django_project/urls.py
--rw-r--r--   0        0        0      431 2020-10-10 02:15:38.198787 djangobible-0.0.8/test_django_project/wsgi.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 djangobible-0.0.8/setup.py
--rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 djangobible-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2262 2020-10-27 18:00:12.441457 djangobible-0.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      715 2020-10-27 17:48:39.342953 djangobible-0.0.9/.github/workflows/django.yml
+-rw-r--r--   0        0        0     1971 2020-10-09 03:33:01.891952 djangobible-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-10-09 03:33:01.895945 djangobible-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1552 2020-10-28 01:59:23.247054 djangobible-0.0.9/README.md
+-rw-r--r--   0        0        0       45 2020-10-18 23:43:36.419870 djangobible-0.0.9/__init__.py
+-rw-r--r--   0        0        0      206 2020-10-28 02:00:26.421394 djangobible-0.0.9/djangobible/__init__.py
+-rw-r--r--   0        0        0      102 2020-10-10 02:15:26.841191 djangobible-0.0.9/djangobible/apps.py
+-rw-r--r--   0        0        0     1207 2020-10-10 02:15:26.901189 djangobible-0.0.9/djangobible/migrations/0001_initial.py
+-rw-r--r--   0        0        0       58 2020-10-18 23:25:04.976566 djangobible-0.0.9/djangobible/migrations/__init__.py
+-rw-r--r--   0        0        0     2155 2020-10-18 23:44:20.371406 djangobible-0.0.9/djangobible/models.py
+-rw-r--r--   0        0        0      697 2020-10-18 23:44:20.327402 djangobible-0.0.9/manage.py
+-rw-r--r--   0        0        0      659 2020-10-28 01:59:53.459453 djangobible-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      177 2020-10-10 02:09:17.806309 djangobible-0.0.9/pytest.ini
+-rw-r--r--   0        0        0       36 2020-10-18 23:36:32.169986 djangobible-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       58 2020-10-12 15:35:46.348106 djangobible-0.0.9/test_django_app/__init__.py
+-rw-r--r--   0        0        0      108 2020-10-10 02:15:31.876139 djangobible-0.0.9/test_django_app/apps.py
+-rw-r--r--   0        0        0      766 2020-10-10 02:15:31.924137 djangobible-0.0.9/test_django_app/migrations/0001_initial.py
+-rw-r--r--   0        0        0       63 2020-10-18 23:25:04.958460 djangobible-0.0.9/test_django_app/migrations/__init__.py
+-rw-r--r--   0        0        0      332 2020-10-18 23:37:19.553224 djangobible-0.0.9/test_django_app/models.py
+-rw-r--r--   0        0        0       49 2020-10-18 23:26:36.754738 djangobible-0.0.9/test_django_app/tests/__init__.py
+-rw-r--r--   0        0        0     2261 2020-10-10 20:06:34.269947 djangobible-0.0.9/test_django_app/tests/conftest.py
+-rw-r--r--   0        0        0     2533 2020-10-12 15:15:27.198297 djangobible-0.0.9/test_django_app/tests/test_models.py
+-rw-r--r--   0        0        0      823 2020-10-10 20:06:34.221952 djangobible-0.0.9/test_django_app/tests/test_search.py
+-rw-r--r--   0        0        0       62 2020-10-18 23:21:06.336139 djangobible-0.0.9/test_django_project/__init__.py
+-rw-r--r--   0        0        0      431 2020-10-18 23:32:52.973212 djangobible-0.0.9/test_django_project/asgi.py
+-rw-r--r--   0        0        0     3333 2020-10-18 23:32:46.749700 djangobible-0.0.9/test_django_project/settings.py
+-rw-r--r--   0        0        0      784 2020-10-18 23:31:50.265596 djangobible-0.0.9/test_django_project/urls.py
+-rw-r--r--   0        0        0      431 2020-10-10 02:15:38.198787 djangobible-0.0.9/test_django_project/wsgi.py
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 djangobible-0.0.9/setup.py
+-rw-r--r--   0        0        0      201 1970-01-01 00:00:00.000000 djangobible-0.0.9/PKG-INFO
```

### Comparing `djangobible-0.0.8/.github/workflows/codeql-analysis.yml` & `djangobible-0.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/.github/workflows/django.yml` & `djangobible-0.0.9/.github/workflows/django.yml`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/.gitignore` & `djangobible-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/LICENSE` & `djangobible-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/README.md` & `djangobible-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # djangobible
 
 The djangobible library is a Django app that wraps the pythonbible library and provides models, managers, and other tools to easily index an object by a scripture reference.
 
+[![PyPI version](https://img.shields.io/pypi/v/djangobible)](https://pypi.org/project/djangobible/)
+[![license MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
 ![Django CI](https://github.com/avendesora/django-bible/workflows/Django%20CI/badge.svg)
 ![CodeQL](https://github.com/avendesora/django-bible/workflows/CodeQL/badge.svg)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/ca34603bdaf8446ba288430b69092093)](https://app.codacy.com/gh/avendesora/django-bible?utm_source=github.com&utm_medium=referral&utm_content=avendesora/django-bible&utm_campaign=Badge_Grade_Settings)
-[![PyPI version](https://badge.fury.io/py/djangobible.svg)](https://badge.fury.io/py/djangobible)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+[![Python 3.8](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue?logo=python)](https://www.python.org/downloads/release/python-380/)
+
 
 ## Installation
 
 ```shell script
 pip install djangobible
 ```
 
 ### Optional Dependencies
 
-If the [defusedxml](https://github.com/tiran/defusedxml) library is installed, djangobible/pythonbible will use it to parse XML files rather than the builtin xml.etree libary.
+If the [defusedxml](https://github.com/tiran/defusedxml) library is installed, djangobible/pythonbible will use it to parse XML files rather than the builtin xml.etree library.
 
 To install djangobible with all optional dependencies, use the following command.
 
 ```shell script
 pip install djangobible[all]
 ```
```

### Comparing `djangobible-0.0.8/djangobible/migrations/0001_initial.py` & `djangobible-0.0.9/djangobible/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/djangobible/models.py` & `djangobible-0.0.9/djangobible/models.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/manage.py` & `djangobible-0.0.9/manage.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/pyproject.toml` & `djangobible-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 author-email = "npatton@gmail.com"
 home-page = "https://github.com/avendesora/django-bible"
 classifiers = ["License :: OSI Approved :: MIT License"]
 description-file = "README.md"
 requires-python = ">=3.6"
 requires = [
     "Django >=3.0.0",
-    "pythonbible >=0.1.2",
+    "pythonbible >=0.1.3",
 ]
 
 [tool.flit.metadata.requires-extra]
 test = [
     "pytest-django >=3.10.0",
 ]
 doc = [
```

### Comparing `djangobible-0.0.8/test_django_app/migrations/0001_initial.py` & `djangobible-0.0.9/test_django_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/test_django_app/tests/conftest.py` & `djangobible-0.0.9/test_django_app/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/test_django_app/tests/test_models.py` & `djangobible-0.0.9/test_django_app/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/test_django_app/tests/test_search.py` & `djangobible-0.0.9/test_django_app/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/test_django_project/settings.py` & `djangobible-0.0.9/test_django_project/settings.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/test_django_project/urls.py` & `djangobible-0.0.9/test_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.0.8/setup.py` & `djangobible-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 packages = \
 ['djangobible', 'djangobible.migrations']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Django >=3.0.0', 'pythonbible >=0.1.2']
+['Django >=3.0.0', 'pythonbible >=0.1.3']
 
 extras_require = \
 {'all': ['defusedxml >=0.6.0'],
  'dev': ['bandit >=1.6.2', 'black >=20.8b1', 'prospector >=1.3.0'],
  'test': ['pytest-django >=3.10.0']}
 
 setup(name='djangobible',
-      version='0.0.8',
+      version='0.0.9',
       description='django-bible python library.',
       author='Nathan Patton',
       author_email='npatton@gmail.com',
       url='https://github.com/avendesora/django-bible',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

