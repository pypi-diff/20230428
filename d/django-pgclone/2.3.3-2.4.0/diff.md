# Comparing `tmp/django-pgclone-2.3.3.tar.gz` & `tmp/django_pgclone-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgclone-2.3.3.tar", max compression
+gzip compressed data, was "django_pgclone-2.4.0.tar", max compression
```

## Comparing `django-pgclone-2.3.3.tar` & `django_pgclone-2.4.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1456 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/LICENSE
--rw-r--r--   0        0        0     2372 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/README.rst
--rw-r--r--   0        0        0      196 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/__init__.py
--rw-r--r--   0        0        0     3980 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/db.py
--rw-r--r--   0        0        0     3351 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/logging.py
--rw-r--r--   0        0        0     3521 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     6457 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/options.py
--rw-r--r--   0        0        0     8966 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1911 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/run.py
--rw-r--r--   0        0        0     1807 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/settings.py
--rw-r--r--   0        0        0     3202 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/storage.py
--rw-r--r--   0        0        0      152 2022-09-03 06:18:53.927928 django-pgclone-2.3.3/pgclone/version.py
--rw-r--r--   0        0        0     2336 2022-09-03 06:20:30.025039 django-pgclone-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     3294 2022-09-03 06:20:52.394471 django-pgclone-2.3.3/setup.py
--rw-r--r--   0        0        0     3579 2022-09-03 06:20:52.395676 django-pgclone-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2372 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/README.rst
+-rw-r--r--   0        0        0      196 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/__init__.py
+-rw-r--r--   0        0        0     4004 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/db.py
+-rw-r--r--   0        0        0     3351 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/logging.py
+-rw-r--r--   0        0        0     3521 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     6457 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/options.py
+-rw-r--r--   0        0        0     8964 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1911 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/run.py
+-rw-r--r--   0        0        0     1807 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/settings.py
+-rw-r--r--   0        0        0     3202 2023-04-28 15:23:33.432068 django_pgclone-2.4.0/pgclone/storage.py
+-rw-r--r--   0        0        0      152 2023-04-28 15:23:33.436068 django_pgclone-2.4.0/pgclone/version.py
+-rw-r--r--   0        0        0     2333 2023-04-28 15:24:11.855854 django_pgclone-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-2.4.0/PKG-INFO
```

### Comparing `django-pgclone-2.3.3/LICENSE` & `django_pgclone-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/README.rst` & `django_pgclone-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/db.py` & `django_pgclone-2.4.0/pgclone/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import copy
 import functools
+import shlex
 
 from django.conf import settings as django_settings
 from django.db import connections, DEFAULT_DB_ALIAS
 from django.db.utils import load_backend
 
 from pgclone import exceptions, settings
 
@@ -97,11 +98,11 @@
 def conn(*, using):
     """Return the database used when making connections to psql"""
     return make(settings.conn_db(), using=using)
 
 
 def url(db_config):
     """Convert a database dictionary config to a url"""
-    return (
+    return shlex.quote(
         f'postgresql://{db_config["USER"]}:{db_config["PASSWORD"]}'
         f'@{db_config["HOST"]}:{db_config["PORT"]}/{db_config["NAME"]}'
     )
```

### Comparing `django-pgclone-2.3.3/pgclone/dump_cmd.py` & `django_pgclone-2.4.0/pgclone/dump_cmd.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/logging.py` & `django_pgclone-2.4.0/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/ls_cmd.py` & `django_pgclone-2.4.0/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/management/commands/pgclone.py` & `django_pgclone-2.4.0/pgclone/management/commands/pgclone.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/options.py` & `django_pgclone-2.4.0/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/restore_cmd.py` & `django_pgclone-2.4.0/pgclone/restore_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     logging.success_msg("Creating the temporary restore db")
     _drop_db(temp_db, using=using)
     create_temp_sql = f'CREATE DATABASE "{temp_db["NAME"]}"'
     run.psql(create_temp_sql, using=using)
     _set_search_path(temp_db, using=using)
 
     logging.success_msg(f'Running pg_restore on "{dump_key}"')
-    pg_restore_cmd = f"pg_restore --verbose --no-acl --no-owner -d '{db.url(temp_db)}'"
+    pg_restore_cmd = f"pg_restore --verbose --no-acl --no-owner -d {db.url(temp_db)}"
     pg_restore_cmd = storage_client.pg_restore(file_path) + " " + pg_restore_cmd
 
     # When restoring, we need to ignore errors because there are certain
     # errors we cannot get around when pg restoring some DBs (like Aurora).
     # In the future, we may parse the output of the pg_restore command to see
     # if an unexpected error happened.
     run.shell(pg_restore_cmd, env=storage_client.env, ignore_errors=True)
```

### Comparing `django-pgclone-2.3.3/pgclone/run.py` & `django_pgclone-2.4.0/pgclone/run.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/settings.py` & `django_pgclone-2.4.0/pgclone/settings.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pgclone/storage.py` & `django_pgclone-2.4.0/pgclone/storage.py`

 * *Files identical despite different names*

### Comparing `django-pgclone-2.3.3/pyproject.toml` & `django_pgclone-2.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 name = "django-pgclone"
 packages = [
   { include = "pgclone" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.3.3"
+version = "2.4.0"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
@@ -65,19 +65,19 @@
 dj-database-url = "0.5.0"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
+git-tidy = "1.2.0"
 myst-parser = "0.18.0"
 packaging = ">=19.2"
 pip = "*"
-poetry-core = "1.1.0rc3"
+poetry-core = "1.3.2"
 pre-commit = "2.13.0"
 psycopg2-binary = "2.9.3"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 pytest-mock = "3.8.2"
```

### Comparing `django-pgclone-2.3.3/PKG-INFO` & `django_pgclone-2.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 2.3.3
+Version: 2.4.0
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -12,21 +12,26 @@
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pgclone.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgclone
 Description-Content-Type: text/x-rst
 
 django-pgclone
 ##############
```

