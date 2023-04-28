# Comparing `tmp/python-chi-0.9.0.tar.gz` & `tmp/python-chi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-chi-0.9.0.tar", last modified: Mon Mar 15 22:13:42 2021, max compression
+gzip compressed data, was "dist/python-chi-0.9.1.tar", last modified: Tue May 25 14:34:13 2021, max compression
```

## Comparing `python-chi-0.9.0.tar` & `python-chi-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:42.000000 python-chi-0.9.0/
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/.github/
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/.github/workflows/
--rw-r--r--   0 jasonanderson   (501) staff       (20)      455 2021-01-08 17:53:50.000000 python-chi-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 jasonanderson   (501) staff       (20)      858 2021-02-26 00:03:48.000000 python-chi-0.9.0/.mailmap
--rw-r--r--   0 jasonanderson   (501) staff       (20)      300 2021-01-08 17:50:37.000000 python-chi-0.9.0/.readthedocs.yml
--rw-r--r--   0 jasonanderson   (501) staff       (20)      319 2021-03-15 22:13:33.000000 python-chi-0.9.0/AUTHORS
--rw-r--r--   0 jasonanderson   (501) staff       (20)     5722 2021-03-15 22:13:33.000000 python-chi-0.9.0/ChangeLog
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1452 2021-01-08 17:49:27.000000 python-chi-0.9.0/DEVELOPMENT.rst
--rw-r--r--   0 jasonanderson   (501) staff       (20)    11351 2020-10-22 19:58:52.000000 python-chi-0.9.0/LICENSE
--rw-r--r--   0 jasonanderson   (501) staff       (20)      237 2020-12-16 22:02:42.000000 python-chi-0.9.0/Makefile
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1258 2021-03-15 22:13:42.000000 python-chi-0.9.0/PKG-INFO
--rw-r--r--   0 jasonanderson   (501) staff       (20)      550 2021-01-08 17:58:59.000000 python-chi-0.9.0/README.rst
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/chi/
--rw-r--r--   0 jasonanderson   (501) staff       (20)      303 2021-03-10 18:08:56.000000 python-chi-0.9.0/chi/__init__.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     5745 2021-03-15 22:08:54.000000 python-chi-0.9.0/chi/clients.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)    10062 2021-02-25 22:28:33.000000 python-chi-0.9.0/chi/context.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1274 2021-01-29 01:16:43.000000 python-chi-0.9.0/chi/image.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1106 2020-11-19 04:11:43.000000 python-chi-0.9.0/chi/jupyterhub.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1186 2019-12-31 20:07:05.000000 python-chi-0.9.0/chi/keypair.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)    20051 2021-03-15 18:06:04.000000 python-chi-0.9.0/chi/lease.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)    23931 2021-03-15 22:02:06.000000 python-chi-0.9.0/chi/network.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      301 2021-01-05 19:58:11.000000 python-chi-0.9.0/chi/networking_api_examples.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      296 2021-01-06 22:44:32.000000 python-chi-0.9.0/chi/reservation_api_examples.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)    21339 2021-02-26 00:02:26.000000 python-chi-0.9.0/chi/server.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      294 2021-01-05 19:58:34.000000 python-chi-0.9.0/chi/server_api_examples.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      778 2021-02-26 00:02:26.000000 python-chi-0.9.0/chi/ssh.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      869 2021-02-25 21:44:25.000000 python-chi-0.9.0/chi/util.py
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/docs/
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/docs/_extras/
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:41.000000 python-chi-0.9.0/docs/_extras/notebooks/
--rw-r--r--   0 jasonanderson   (501) staff       (20)        8 2021-01-08 17:35:39.000000 python-chi-0.9.0/docs/_extras/notebooks/.gitignore
--rw-r--r--   0 jasonanderson   (501) staff       (20)     3552 2021-02-25 23:29:13.000000 python-chi-0.9.0/docs/conf.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     3603 2021-01-08 19:31:13.000000 python-chi-0.9.0/docs/generate_notebook.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1923 2021-03-15 22:11:15.000000 python-chi-0.9.0/docs/index.rst
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:42.000000 python-chi-0.9.0/docs/modules/
--rw-r--r--   0 jasonanderson   (501) staff       (20)      210 2021-03-15 22:11:05.000000 python-chi-0.9.0/docs/modules/context.rst
--rw-r--r--   0 jasonanderson   (501) staff       (20)      183 2021-01-06 22:48:54.000000 python-chi-0.9.0/docs/modules/image.rst
--rw-r--r--   0 jasonanderson   (501) staff       (20)      366 2021-01-06 00:30:26.000000 python-chi-0.9.0/docs/modules/lease.rst
--rw-r--r--   0 jasonanderson   (501) staff       (20)      378 2021-01-06 22:43:40.000000 python-chi-0.9.0/docs/modules/network.rst
--rw-r--r--   0 jasonanderson   (501) staff       (20)      700 2021-01-05 23:37:53.000000 python-chi-0.9.0/docs/modules/server.rst
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:42.000000 python-chi-0.9.0/docs/notebooks/
--rw-r--r--   0 jasonanderson   (501) staff       (20)        8 2021-01-08 17:34:51.000000 python-chi-0.9.0/docs/notebooks/.gitignore
--rw-r--r--   0 jasonanderson   (501) staff       (20)       74 2021-01-08 04:37:12.000000 python-chi-0.9.0/docs/requirements.txt
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:42.000000 python-chi-0.9.0/python_chi.egg-info/
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1258 2021-03-15 22:13:33.000000 python-chi-0.9.0/python_chi.egg-info/PKG-INFO
--rw-r--r--   0 jasonanderson   (501) staff       (20)     1017 2021-03-15 22:13:41.000000 python-chi-0.9.0/python_chi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonanderson   (501) staff       (20)        1 2021-03-15 22:13:33.000000 python-chi-0.9.0/python_chi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonanderson   (501) staff       (20)        1 2018-11-26 19:40:30.000000 python-chi-0.9.0/python_chi.egg-info/not-zip-safe
--rw-r--r--   0 jasonanderson   (501) staff       (20)       46 2021-03-15 22:13:33.000000 python-chi-0.9.0/python_chi.egg-info/pbr.json
--rw-r--r--   0 jasonanderson   (501) staff       (20)      156 2021-03-15 22:13:33.000000 python-chi-0.9.0/python_chi.egg-info/requires.txt
--rw-r--r--   0 jasonanderson   (501) staff       (20)        4 2021-03-15 22:13:33.000000 python-chi-0.9.0/python_chi.egg-info/top_level.txt
--rw-r--r--   0 jasonanderson   (501) staff       (20)      156 2021-02-25 21:30:16.000000 python-chi-0.9.0/requirements.txt
--rw-r--r--   0 jasonanderson   (501) staff       (20)      645 2021-03-15 22:13:42.000000 python-chi-0.9.0/setup.cfg
--rw-r--r--   0 jasonanderson   (501) staff       (20)      100 2021-01-08 01:54:12.000000 python-chi-0.9.0/setup.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)       46 2021-01-08 00:51:58.000000 python-chi-0.9.0/test-requirements.txt
-drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-03-15 22:13:42.000000 python-chi-0.9.0/tests/
--rw-r--r--   0 jasonanderson   (501) staff       (20)     4324 2020-12-23 01:44:26.000000 python-chi-0.9.0/tests/test_context.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     8446 2021-01-08 17:18:48.000000 python-chi-0.9.0/tests/test_lease.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     2704 2021-02-15 18:50:53.000000 python-chi-0.9.0/tests/test_network.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)     4029 2021-02-25 23:25:05.000000 python-chi-0.9.0/tests/test_server.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      362 2019-12-31 20:07:05.000000 python-chi-0.9.0/tests/test_ssh.py
--rw-r--r--   0 jasonanderson   (501) staff       (20)      436 2021-01-08 17:54:53.000000 python-chi-0.9.0/tox.ini
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/.github/
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/.github/workflows/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      455 2021-01-08 17:53:50.000000 python-chi-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      858 2021-02-26 00:03:48.000000 python-chi-0.9.1/.mailmap
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      300 2021-01-08 17:50:37.000000 python-chi-0.9.1/.readthedocs.yml
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      319 2021-05-25 14:34:04.000000 python-chi-0.9.1/AUTHORS
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     5996 2021-05-25 14:34:04.000000 python-chi-0.9.1/ChangeLog
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1452 2021-01-08 17:49:27.000000 python-chi-0.9.1/DEVELOPMENT.rst
+-rw-r--r--   0 jasonanderson   (501) staff       (20)    11351 2020-10-22 19:58:52.000000 python-chi-0.9.1/LICENSE
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      237 2020-12-16 22:02:42.000000 python-chi-0.9.1/Makefile
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1258 2021-05-25 14:34:13.000000 python-chi-0.9.1/PKG-INFO
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      550 2021-01-08 17:58:59.000000 python-chi-0.9.1/README.rst
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/chi/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      321 2021-05-05 16:10:41.000000 python-chi-0.9.1/chi/__init__.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     5768 2021-05-05 16:10:41.000000 python-chi-0.9.1/chi/clients.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)    10814 2021-03-15 22:18:50.000000 python-chi-0.9.1/chi/context.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1274 2021-01-29 01:16:43.000000 python-chi-0.9.1/chi/image.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1106 2020-11-19 04:11:43.000000 python-chi-0.9.1/chi/jupyterhub.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1186 2019-12-31 20:07:05.000000 python-chi-0.9.1/chi/keypair.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)    20763 2021-05-25 14:31:58.000000 python-chi-0.9.1/chi/lease.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)    23939 2021-04-20 16:23:55.000000 python-chi-0.9.1/chi/network.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      301 2021-01-05 19:58:11.000000 python-chi-0.9.1/chi/networking_api_examples.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      296 2021-01-06 22:44:32.000000 python-chi-0.9.1/chi/reservation_api_examples.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)    21339 2021-02-26 00:02:26.000000 python-chi-0.9.1/chi/server.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      294 2021-01-05 19:58:34.000000 python-chi-0.9.1/chi/server_api_examples.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      778 2021-02-26 00:02:26.000000 python-chi-0.9.1/chi/ssh.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      869 2021-02-25 21:44:25.000000 python-chi-0.9.1/chi/util.py
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/docs/
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/docs/_extras/
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/docs/_extras/notebooks/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)        8 2021-01-08 17:35:39.000000 python-chi-0.9.1/docs/_extras/notebooks/.gitignore
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     3552 2021-02-25 23:29:13.000000 python-chi-0.9.1/docs/conf.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     3603 2021-01-08 19:31:13.000000 python-chi-0.9.1/docs/generate_notebook.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1955 2021-03-15 22:22:12.000000 python-chi-0.9.1/docs/index.rst
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/docs/modules/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      210 2021-03-15 22:11:05.000000 python-chi-0.9.1/docs/modules/context.rst
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      183 2021-01-06 22:48:54.000000 python-chi-0.9.1/docs/modules/image.rst
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      366 2021-01-06 00:30:26.000000 python-chi-0.9.1/docs/modules/lease.rst
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      378 2021-01-06 22:43:40.000000 python-chi-0.9.1/docs/modules/network.rst
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      700 2021-01-05 23:37:53.000000 python-chi-0.9.1/docs/modules/server.rst
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/docs/notebooks/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)        8 2021-01-08 17:34:51.000000 python-chi-0.9.1/docs/notebooks/.gitignore
+-rw-r--r--   0 jasonanderson   (501) staff       (20)       74 2021-01-08 04:37:12.000000 python-chi-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/python_chi.egg-info/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1258 2021-05-25 14:34:04.000000 python-chi-0.9.1/python_chi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     1017 2021-05-25 14:34:12.000000 python-chi-0.9.1/python_chi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonanderson   (501) staff       (20)        1 2021-05-25 14:34:04.000000 python-chi-0.9.1/python_chi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonanderson   (501) staff       (20)        1 2018-11-26 19:40:30.000000 python-chi-0.9.1/python_chi.egg-info/not-zip-safe
+-rw-r--r--   0 jasonanderson   (501) staff       (20)       46 2021-05-25 14:34:05.000000 python-chi-0.9.1/python_chi.egg-info/pbr.json
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      156 2021-05-25 14:34:04.000000 python-chi-0.9.1/python_chi.egg-info/requires.txt
+-rw-r--r--   0 jasonanderson   (501) staff       (20)        4 2021-05-25 14:34:04.000000 python-chi-0.9.1/python_chi.egg-info/top_level.txt
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      156 2021-02-25 21:30:16.000000 python-chi-0.9.1/requirements.txt
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      645 2021-05-25 14:34:13.000000 python-chi-0.9.1/setup.cfg
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      100 2021-01-08 01:54:12.000000 python-chi-0.9.1/setup.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)       46 2021-01-08 00:51:58.000000 python-chi-0.9.1/test-requirements.txt
+drwxr-xr-x   0 jasonanderson   (501) staff       (20)        0 2021-05-25 14:34:13.000000 python-chi-0.9.1/tests/
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     4324 2020-12-23 01:44:26.000000 python-chi-0.9.1/tests/test_context.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     8446 2021-01-08 17:18:48.000000 python-chi-0.9.1/tests/test_lease.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     2704 2021-02-15 18:50:53.000000 python-chi-0.9.1/tests/test_network.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)     4029 2021-02-25 23:25:05.000000 python-chi-0.9.1/tests/test_server.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      362 2019-12-31 20:07:05.000000 python-chi-0.9.1/tests/test_ssh.py
+-rw-r--r--   0 jasonanderson   (501) staff       (20)      436 2021-01-08 17:54:53.000000 python-chi-0.9.1/tox.ini
```

### Comparing `python-chi-0.9.0/.mailmap` & `python-chi-0.9.1/.mailmap`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/ChangeLog` & `python-chi-0.9.1/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 CHANGES
 =======
 
+v0.9.1
+------
+
+* Fix import error on Lease init
+
+v0.10.1
+-------
+
+* add ironic client to chi \_\_init\_\_
+* Nuke network by name or ID
+
+v0.10.0
+-------
+
+* Add getter for reserved floating IPs
+* Update return type of wait\_for\_active
+* Update docs
+* Add docs for use\_site
+
 v0.9.0
 ------
 
 * Add docs for parent module
 * Allow specifying multiple port addresses
 * Fix reservation parsing
```

### Comparing `python-chi-0.9.0/DEVELOPMENT.rst` & `python-chi-0.9.1/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/LICENSE` & `python-chi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/PKG-INFO` & `python-chi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-chi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Helper library for Chameleon Infrastructure (CHI) testbed
 Home-page: https://www.chameleoncloud.org
 Author: University of Chicago
 Author-email: dev@lists.chameleoncloud.org
 License: UNKNOWN
 Description: python-chi
         ==========
```

### Comparing `python-chi-0.9.0/README.rst` & `python-chi-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/clients.py` & `python-chi-0.9.1/chi/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     Returns:
         A new Ironic client.
     """
     from ironicclient import client as IronicClient
     return IronicClient.get_client(
         '1',
-        session=session,
+        session=(session or session_factory()),
         region_name=getattr(session, 'region_name', None),
         # Ironic client defaults to 1.9 currently,
         # "latest" will be latest the API supports
         os_ironic_api_version='latest'
     )
```

### Comparing `python-chi-0.9.0/chi/context.py` & `python-chi-0.9.1/chi/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,37 @@
     global _auth_plugin
     keys = list(cfg.CONF[CONF_GROUP].keys())
     keys.extend(list(cfg.CONF[_auth_section(_auth_plugin)].keys()))
     return keys
 
 
 def use_site(site_name):
+    """Configure the global request context to target a particular CHI site.
+
+    Targeting a site will mean that leases, instance launch requests, and any
+    other API calls will be sent to that site. By default, no site is selected,
+    and one must be explicitly chosen.
+
+    .. code-block:: python
+
+       chi.use_site("CHI@UC")
+
+    Changing the site will affect future calls the client makes, implicitly.
+    Therefore something like this is possible:
+
+    .. code-block:: python
+
+       chi.use_site("CHI@UC")
+       chi.lease.create_lease("my-uc-lease", reservations)
+       chi.use_site("CHI@TACC")
+       chi.lease.create_lease("my-tacc-lease", reservations)
+
+    Args:
+        site_name (str): The name of the site, e.g., "CHI@UC".
+    """
     global _sites
     if not _sites:
         res = requests.get(f'{RESOURCE_API_URL}/sites.json')
         try:
             res.raise_for_status()
             items = res.json().get('items', [])
             _sites = {s['name']: s for s in items}
```

### Comparing `python-chi-0.9.0/chi/image.py` & `python-chi-0.9.1/chi/image.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/jupyterhub.py` & `python-chi-0.9.1/chi/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/keypair.py` & `python-chi-0.9.1/chi/keypair.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/lease.py` & `python-chi-0.9.1/chi/lease.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import timedelta
 import json
 import numbers
 import sys
 import time
 
 from blazarclient.exception import BlazarClientException
-from neutronclient.v2_0.client import Client as NeutronClient
 
-from .clients import blazar
+from .clients import blazar, neutron
 from .context import get as get_from_context, session
-from .network import get_network_id, PUBLIC_NETWORK
+from .network import get_network_id, PUBLIC_NETWORK, list_floating_ips
 from .server import Server, ServerError
 from .util import random_base32, utcnow
 
 import logging
 LOG = logging.getLogger(__name__)
 
 __all__ = [
     'add_node_reservation',
     'add_network_reservation',
     'add_fip_reservation',
-    'get_floating_ip_by_reservation_id',
+    'get_node_reservation',
+    'get_reserved_floating_ips',
     'lease_duration',
     'get_lease',
     'get_lease_id',
     'create_lease',
     'delete_lease',
     'wait_for_active',
 ]
@@ -183,18 +183,16 @@
         :py:func:`lease_create_args`
     """
 
     def __init__(self, **kwargs):
         kwargs.setdefault("session", session())
 
         self.session = kwargs.pop("session")
-        self.blazar = BlazarClient(
-            "1", service_type="reservation", session=self.session
-        )
-        self.neutron = NeutronClient(session=self.session)
+        self.blazar = blazar(session=self.session)
+        self.neutron = neutron(session=self.session)
 
         self.lease = None
 
         self._servers = {}
 
         self._sequester = kwargs.pop("sequester", False)
 
@@ -384,44 +382,72 @@
 
     Returns:
         The ID of the reservation, if found.
 
     Raises:
         ValueError: If no reservation was found, or multiple were found.
     """
-    lease = get_lease(lease_ref)
-    reservations = lease.get("reservations", [])
-    if isinstance(reservations, str):
-        LOG.info("Blazar returned nested JSON structure, unpacking.")
-        try:
-            reservations = json.loads(reservations)
-        except Exception:
-            pass
-
-    def _passes(res):
+    def _find_node_reservation(res):
         if res.get("resource_type") != "physical:host":
             return False
         if (count is not None
             and not all(int(res.get(key)) == count
                         for key in ["min_count", "max_count"])):
             return False
         if (node_type is not None
             and node_type not in res.get("resource_properties")):
             return False
         return True
 
-    node_reservations = [r for r in reservations if _passes(r)]
-    if not node_reservations:
-        raise ValueError("No node reservation found")
-    elif len(node_reservations) > 1:
-        raise ValueError("Multiple node reservations found")
-    else:
-        return node_reservations[0]
+    res = _reservation_matching(lease_ref, _find_node_reservation)
+    return res["id"]
+
+
+def get_reserved_floating_ips(lease_ref) -> "list[str]":
+    """Get a list of Floating IP addresses reserved in a lease.
+
+    Args:
+        lease_ref (str): The ID or name of the lease.
+
+    Returns:
+        A list of all reserved Floating IP addresses, if any were reserved.
+    """
+    def _find_fip_reservation(res):
+        return res.get("resource_type") == "virtual:floatingip"
+
+    res = _reservation_matching(lease_ref, _find_fip_reservation, multiple=True)
+    fips = list_floating_ips()
+    return [
+        fip["floating_ip_address"] for fip in fips
+        if any(f"reservation:{r['id']}" in fip["tags"] for r in res)
+    ]
 
 
+def _reservation_matching(lease_ref, match_fn, multiple=False):
+    lease = get_lease(lease_ref)
+    reservations = lease.get("reservations", [])
+    if isinstance(reservations, str):
+        LOG.info("Blazar returned nested JSON structure, unpacking.")
+        try:
+            reservations = json.loads(reservations)
+        except Exception:
+            pass
+
+    matches = [r for r in reservations if match_fn(r)]
+
+    if not matches:
+        raise ValueError("No matching reservation found")
+
+    if multiple:
+        return matches
+    else:
+        if len(matches) > 1:
+            raise ValueError("Multiple matching reservations found")
+        return matches[0]
+
 
 def add_network_reservation(reservation_list,
                             network_name,
                             of_controller_ip=None,
                             of_controller_port=None,
                             vswitch_name=None,
                             physical_network="physnet1"):
@@ -471,19 +497,14 @@
     reservation_list.append({
         'resource_type': 'virtual:floatingip',
         'network_id': get_network_id(PUBLIC_NETWORK),
         'amount': count
     })
 
 
-def get_floating_ip_by_reservation_id(reservation_id):
-    # blazar().lease.list()
-    pass
-
-
 def lease_duration(days=1, hours=0):
     """Compute the start and end dates for a lease given its desired duration.
 
     When providing both ``days`` and ``hours``, the duration is summed. So,
     the following would be a lease for one and a half days:
 
     .. code-block:: python
@@ -592,19 +613,22 @@
 
     This function will wait for 2.5 minutes, which is a somewhat arbitrary
     amount of time.
 
     Args:
         ref (str): The name or ID of the lease.
 
+    Returns:
+        The lease in ACTIVE state.
+
     Raises:
         TimeoutError: If the lease fails to become active within the timeout.
     """
     for _ in range(15):
-        time.sleep(10)
-        status = get_lease(ref)['status']
+        lease = get_lease(ref)
+        status = lease['status']
         if status == 'ACTIVE':
-            break
+            return lease
         elif status == 'ERROR':
             raise RuntimeError("Lease went into ERROR state")
-    else:
-        raise TimeoutError("Lease failed to start")
+        time.sleep(10)
+    raise TimeoutError("Lease failed to start")
```

### Comparing `python-chi-0.9.0/chi/network.py` & `python-chi-0.9.1/chi/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
         "floatingip": {
             "port_id": port_id,
             "fixed_ip_address": fixed_ip_address,
         }
     })
 
 
-def nuke_network(network_name):
+def nuke_network(network_ref: str):
     """Completely tear down the network.
 
     Cleanly tearing down an OpenStack network representation involves a few
     separate steps:
 
     1. Detach the network's subnets from the router.
     2. Delete the router.
@@ -752,17 +752,17 @@
     .. note::
 
        This function will not work well for very advance networks, perhaps
        those connected to multiple routers. You should perform your own cleanup
        if your network's subnets are attached to multiple routers.
 
     Args:
-        network_name (str): The network name.
+        network_ref (str): The network name or ID.
     """
-    network = get_network(network_name)
+    network = get_network(network_ref)
     network_id = network["id"]
 
     #Detach the router from all of its networks
     router_ports = [
         port for port in neutron().list_ports()["ports"]
         if port["device_owner"] == "network:router_interface" and port["network_id"] == network_id
     ]
```

### Comparing `python-chi-0.9.0/chi/server.py` & `python-chi-0.9.1/chi/server.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/ssh.py` & `python-chi-0.9.1/chi/ssh.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/chi/util.py` & `python-chi-0.9.1/chi/util.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/docs/conf.py` & `python-chi-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/docs/generate_notebook.py` & `python-chi-0.9.1/docs/generate_notebook.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/docs/index.rst` & `python-chi-0.9.1/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -37,24 +37,25 @@
   import chi
 
   # Select your project
   chi.set('project_name', 'CH-XXXXXX')
   # Select your site
   chi.use_site('CHI@UC')
 
-  # Make a reservation
+  # Make a reservation ...
   reservations = []
+  # ... for one node of type "compute_skylake"
   chi.lease.add_node_reservation(
-    reservations, node_type='compute_skylake', count=1)
+      reservations, node_type='compute_skylake', count=1)
+  # ... and one Floating IP
+  chi.lease.add_fip_reservation(count=1)
+  # ... for one day.
   start_date, end_date = chi.lease.lease_duration(days=1)
-  blazar().lease.create(name=lease_name,
-                        start=start_date,
-                        end=end_date,
-                        reservations=reservation_list,
-                        events=[])
+  chi.lease.create_lease(
+      lease_name, reservations, start_date=start_date, end_date=end_date)
 
 .. toctree::
    :caption: Modules
    :maxdepth: 1
 
    modules/context
    modules/lease
```

### Comparing `python-chi-0.9.0/docs/modules/server.rst` & `python-chi-0.9.1/docs/modules/server.rst`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/python_chi.egg-info/PKG-INFO` & `python-chi-0.9.1/python_chi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-chi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Helper library for Chameleon Infrastructure (CHI) testbed
 Home-page: https://www.chameleoncloud.org
 Author: University of Chicago
 Author-email: dev@lists.chameleoncloud.org
 License: UNKNOWN
 Description: python-chi
         ==========
```

### Comparing `python-chi-0.9.0/python_chi.egg-info/SOURCES.txt` & `python-chi-0.9.1/python_chi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/setup.cfg` & `python-chi-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/tests/test_context.py` & `python-chi-0.9.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/tests/test_lease.py` & `python-chi-0.9.1/tests/test_lease.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/tests/test_network.py` & `python-chi-0.9.1/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `python-chi-0.9.0/tests/test_server.py` & `python-chi-0.9.1/tests/test_server.py`

 * *Files identical despite different names*

