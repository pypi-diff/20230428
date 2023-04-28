# Comparing `tmp/nci_cidc_api_modules-0.27.41.tar.gz` & `tmp/nci_cidc_api_modules-0.27.41rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-wjnqwke_/nci_cidc_api_modules-0.27.41.tar", last modified: Tue Apr 25 18:53:08 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-h4p4hh4j/nci_cidc_api_modules-0.27.41rc0.tar", last modified: Thu Apr 27 20:57:46 2023, max compression
```

## Comparing `nci_cidc_api_modules-0.27.41.tar` & `nci_cidc_api_modules-0.27.41rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37107 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    32453 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:08.000000 nci_cidc_api_modules-0.27.41/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-25 18:53:00.000000 nci_cidc_api_modules-0.27.41/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32453 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:57:46.000000 nci_cidc_api_modules-0.27.41rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-27 20:57:34.000000 nci_cidc_api_modules-0.27.41rc0/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-0.27.41/LICENSE` & `nci_cidc_api_modules-0.27.41rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/PKG-INFO` & `nci_cidc_api_modules-0.27.41rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 0.27.41
+Version: 0.27.41rc0
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CIDC API <!-- omit in TOC -->
+# NCI CIDC API <!-- omit in TOC -->
 
-| Environment | Branch                                                                   | Status                                                                                                                               | Maintainability                                                                                                                                                          | Test Coverage                                                                                                                                                      |
-| ----------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| production  | [production](https://github.com/NCI-CIDC/cidc-api-gae/tree/production) | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=production) |                                                                                                                                                                          |                                                                                                                                                                    |
-| staging     | [master](https://github.com/NCI-CIDC/cidc-api-gae)                     | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=master)     | [![Maintainability](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/maintainability)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/maintainability) | [![Test Coverage](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/test_coverage)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/test_coverage) |
+The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
-The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Eve REST API framework backed by Google Cloud SQL, running on Google App Engine.
-
-# Development <!-- omit in TOC -->
+## Development <!-- omit in TOC -->
 
 - [Install Python dependencies](#install-python-dependencies)
 - [Database Management](#database-management)
   - [Setting up a local development database](#setting-up-a-local-development-database)
   - [Connecting to a Cloud SQL database instance](#connecting-to-a-cloud-sql-database-instance)
   - [Running database migrations](#running-database-migrations)
 - [Serving Locally](#serving-locally)
```

### Comparing `nci_cidc_api_modules-0.27.41/README.md` & `nci_cidc_api_modules-0.27.41rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-# CIDC API <!-- omit in TOC -->
+# NCI CIDC API <!-- omit in TOC -->
 
-| Environment | Branch                                                                   | Status                                                                                                                               | Maintainability                                                                                                                                                          | Test Coverage                                                                                                                                                      |
-| ----------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| production  | [production](https://github.com/NCI-CIDC/cidc-api-gae/tree/production) | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=production) |                                                                                                                                                                          |                                                                                                                                                                    |
-| staging     | [master](https://github.com/NCI-CIDC/cidc-api-gae)                     | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=master)     | [![Maintainability](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/maintainability)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/maintainability) | [![Test Coverage](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/test_coverage)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/test_coverage) |
+The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
-The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Eve REST API framework backed by Google Cloud SQL, running on Google App Engine.
-
-# Development <!-- omit in TOC -->
+## Development <!-- omit in TOC -->
 
 - [Install Python dependencies](#install-python-dependencies)
 - [Database Management](#database-management)
   - [Setting up a local development database](#setting-up-a-local-development-database)
   - [Connecting to a Cloud SQL database instance](#connecting-to-a-cloud-sql-database-instance)
   - [Running database migrations](#running-database-migrations)
 - [Serving Locally](#serving-locally)
```

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/config/db.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/config/logging.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/config/secrets.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/config/settings.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 load_dotenv()
 
 ### Configure application environment ###
 ENV = environ.get("ENV")
 DEV_USE_GCS = environ.get("DEV_USE_GCS") == "True"
 assert ENV in (
     "dev",
+    "dev-int",
     "staging",
     "prod",
-), "ENV environment variable must be set to 'dev', 'staging', or 'prod'"
+), "ENV environment variable must be set to 'dev', 'dev-int', 'staging', or 'prod'"
 DEBUG = environ.get("DEBUG") == "True"
 assert ENV == "dev" if DEBUG else True, "DEBUG mode is only allowed when ENV='dev'"
 TESTING = environ.get("TESTING") == "True"
 ALLOWED_CLIENT_URL = environ.get("ALLOWED_CLIENT_URL")
 IS_GUNICORN = "gunicorn" in environ.get("SERVER_SOFTWARE", "")
 
 ### Configure miscellaneous constants ###
```

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/csms/auth.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/files/details.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/migrations.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/models.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/models/schemas.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/shared/auth.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/shared/emails.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/emails.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-0.27.41rc0/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 Metadata-Version: 2.1
 Name: nci-cidc-api-modules
-Version: 0.27.41
+Version: 0.27.41rc0
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CIDC API <!-- omit in TOC -->
+# NCI CIDC API <!-- omit in TOC -->
 
-| Environment | Branch                                                                   | Status                                                                                                                               | Maintainability                                                                                                                                                          | Test Coverage                                                                                                                                                      |
-| ----------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| production  | [production](https://github.com/NCI-CIDC/cidc-api-gae/tree/production) | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=production) |                                                                                                                                                                          |                                                                                                                                                                    |
-| staging     | [master](https://github.com/NCI-CIDC/cidc-api-gae)                     | ![Continuous Integration](https://github.com/NCI-CIDC/cidc-api-gae/workflows/Continuous%20Integration/badge.svg?branch=master)     | [![Maintainability](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/maintainability)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/maintainability) | [![Test Coverage](https://api.codeclimate.com/v1/badges/71d93f067ea23efdc842/test_coverage)](https://codeclimate.com/github/CIMAC-CIDC/cidc-api-gae/test_coverage) |
+The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
-The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Eve REST API framework backed by Google Cloud SQL, running on Google App Engine.
-
-# Development <!-- omit in TOC -->
+## Development <!-- omit in TOC -->
 
 - [Install Python dependencies](#install-python-dependencies)
 - [Database Management](#database-management)
   - [Setting up a local development database](#setting-up-a-local-development-database)
   - [Connecting to a Cloud SQL database instance](#connecting-to-a-cloud-sql-database-instance)
   - [Running database migrations](#running-database-migrations)
 - [Serving Locally](#serving-locally)
```

### Comparing `nci_cidc_api_modules-0.27.41/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-0.27.41rc0/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/setup.py` & `nci_cidc_api_modules-0.27.41rc0/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.41/tests/test_api.py` & `nci_cidc_api_modules-0.27.41rc0/tests/test_api.py`

 * *Files identical despite different names*

