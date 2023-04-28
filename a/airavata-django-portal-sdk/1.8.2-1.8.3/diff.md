# Comparing `tmp/airavata-django-portal-sdk-1.8.2.tar.gz` & `tmp/airavata-django-portal-sdk-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata-django-portal-sdk-1.8.2.tar", last modified: Tue Feb 21 23:41:35 2023, max compression
+gzip compressed data, was "airavata-django-portal-sdk-1.8.3.tar", last modified: Fri Apr 28 20:30:52 2023, max compression
```

## Comparing `airavata-django-portal-sdk-1.8.2.tar` & `airavata-django-portal-sdk-1.8.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.419434 airavata-django-portal-sdk-1.8.2/
--rw-r--r--   0 machrist (661619347) wheel        (0)    11356 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/LICENSE
--rw-r--r--   0 machrist (661619347) wheel        (0)     3307 2023-02-21 23:41:35.419571 airavata-django-portal-sdk-1.8.2/PKG-INFO
--rw-r--r--   0 machrist (661619347) wheel        (0)     2463 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/README.md
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.413357 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/
--rw-r--r--   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      124 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/apps.py
--rw-r--r--   0 machrist (661619347) wheel        (0)       74 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/decorators.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.414635 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/
--rw-r--r--   0 machrist (661619347) wheel        (0)      119 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     8661 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/api.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     4798 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/intermediate_output.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.415386 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/
--rw-r--r--   0 machrist (661619347) wheel        (0)      687 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0001_initial.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     1020 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     1914 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py
--rw-r--r--   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      731 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/models.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     1783 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/queue_settings_calculators.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     1480 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/remoteapi.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      993 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/serializers.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.416414 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/
--rw-r--r--   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     3848 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      439 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_settings.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    15900 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_user_storage.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      345 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_util.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     5512 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_views.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     1027 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/urls.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.416908 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/
--rw-r--r--   0 machrist (661619347) wheel        (0)     1126 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    42739 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/api.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.419223 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/
--rw-r--r--   0 machrist (661619347) wheel        (0)    15554 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      159 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2_grpc.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    61784 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    14361 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      330 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     2779 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/base.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    13793 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py
--rw-r--r--   0 machrist (661619347) wheel        (0)    12378 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/mft_provider.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      343 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/util.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     9127 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/views.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2023-02-21 23:41:35.414128 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/
--rw-r--r--   0 machrist (661619347) wheel        (0)     3307 2023-02-21 23:41:35.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 machrist (661619347) wheel        (0)     2035 2023-02-21 23:41:35.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)        1 2023-02-21 23:41:35.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)       77 2023-02-21 23:41:35.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/requires.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)       27 2023-02-21 23:41:35.000000 airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/top_level.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)      222 2023-02-21 23:41:35.419984 airavata-django-portal-sdk-1.8.2/setup.cfg
--rw-r--r--   0 machrist (661619347) wheel        (0)     1356 2023-02-21 23:41:08.000000 airavata-django-portal-sdk-1.8.2/setup.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.638175 airavata-django-portal-sdk-1.8.3/
+-rw-r--r--   0 machrist (661619347) 1014028542    11356 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/LICENSE
+-rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-04-28 20:30:52.638276 airavata-django-portal-sdk-1.8.3/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     2463 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/README.md
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.631788 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542      124 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/apps.py
+-rw-r--r--   0 machrist (661619347) 1014028542       74 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/decorators.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.633382 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/
+-rw-r--r--   0 machrist (661619347) 1014028542      119 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     8661 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/api.py
+-rw-r--r--   0 machrist (661619347) 1014028542     4798 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/intermediate_output.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.634260 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/
+-rw-r--r--   0 machrist (661619347) 1014028542      687 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0001_initial.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1020 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1914 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542      731 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/models.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1783 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/queue_settings_calculators.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1480 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/remoteapi.py
+-rw-r--r--   0 machrist (661619347) 1014028542      993 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/serializers.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.635383 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     3848 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py
+-rw-r--r--   0 machrist (661619347) 1014028542      439 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_settings.py
+-rw-r--r--   0 machrist (661619347) 1014028542    15900 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_user_storage.py
+-rw-r--r--   0 machrist (661619347) 1014028542      345 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_util.py
+-rw-r--r--   0 machrist (661619347) 1014028542     5512 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_views.py
+-rw-r--r--   0 machrist (661619347) 1014028542     1027 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/urls.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.635918 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/
+-rw-r--r--   0 machrist (661619347) 1014028542     1126 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542    42739 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/api.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.637965 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/
+-rw-r--r--   0 machrist (661619347) 1014028542    15554 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py
+-rw-r--r--   0 machrist (661619347) 1014028542      159 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2_grpc.py
+-rw-r--r--   0 machrist (661619347) 1014028542    61784 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py
+-rw-r--r--   0 machrist (661619347) 1014028542    14361 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py
+-rw-r--r--   0 machrist (661619347) 1014028542      330 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     2779 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/base.py
+-rw-r--r--   0 machrist (661619347) 1014028542    13793 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py
+-rw-r--r--   0 machrist (661619347) 1014028542    12378 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/mft_provider.py
+-rw-r--r--   0 machrist (661619347) 1014028542      343 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/util.py
+-rw-r--r--   0 machrist (661619347) 1014028542     8926 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/views.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-04-28 20:30:52.632870 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/
+-rw-r--r--   0 machrist (661619347) 1014028542     3307 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     2035 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 machrist (661619347) 1014028542        1 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       77 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/requires.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       27 2023-04-28 20:30:52.000000 airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/top_level.txt
+-rw-r--r--   0 machrist (661619347) 1014028542      222 2023-04-28 20:30:52.638581 airavata-django-portal-sdk-1.8.3/setup.cfg
+-rw-r--r--   0 machrist (661619347) 1014028542     1356 2023-04-28 20:30:35.000000 airavata-django-portal-sdk-1.8.3/setup.py
```

### Comparing `airavata-django-portal-sdk-1.8.2/LICENSE` & `airavata-django-portal-sdk-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/PKG-INFO` & `airavata-django-portal-sdk-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-sdk
-Version: 1.8.2
+Version: 1.8.3
 Summary: The Airavata Django Portal SDK is a library that makes it easier to develop Airavata Django Portal customizations.
 Home-page: https://github.com/apache/airavata-django-portal-sdk
 Author: Apache Software Foundation
 Author-email: dev@airavata.apache.org
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `airavata-django-portal-sdk-1.8.2/README.md` & `airavata-django-portal-sdk-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/api.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/api.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/experiment_util/intermediate_output.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/experiment_util/intermediate_output.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0001_initial.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0002_userfiles_file_resource_id.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/migrations/0003_auto_20220225_1510.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/models.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/models.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/queue_settings_calculators.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/queue_settings_calculators.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/remoteapi.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/remoteapi.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/serializers.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/serializers.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_queue_settings_calculator.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_user_storage.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_user_storage.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/tests/test_views.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/urls.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/__init__.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/api.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/api.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/CredCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/MFTApi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/base.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/base.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/django_filesystem_provider.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/user_storage/backends/mft_provider.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/user_storage/backends/mft_provider.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk/views.py` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,20 @@
         mime_type = request.GET.get('mime-type', mime_type)
     except Exception as e:
         logger.warning("Failed to load DataProduct for {}"
                        .format(data_product_uri), exc_info=True)
         raise Http404("data product does not exist") from e
     try:
         data_file = user_storage.open_file(request, data_product)
-        response = FileResponse(data_file, content_type=mime_type)
+        as_attachment = (mime_type == 'application/octet-stream' or force_download)
         if user_storage.is_input_file(request, data_product):
             file_name = data_product.productName
         else:
             file_name = os.path.basename(data_file.name)
-        if mime_type == 'application/octet-stream' or force_download:
-            response['Content-Disposition'] = ('attachment; filename="{}"'
-                                               .format(file_name))
-        else:
-            response['Content-Disposition'] = f'inline; filename="{file_name}"'
-        return response
+        return FileResponse(data_file, content_type=mime_type, as_attachment=as_attachment, filename=file_name)
     except ObjectDoesNotExist as e:
         raise Http404(str(e)) from e
 
 
 @api_view()
 def download_dir(request):
     path = request.GET.get('path', "")
```

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/PKG-INFO` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-sdk
-Version: 1.8.2
+Version: 1.8.3
 Summary: The Airavata Django Portal SDK is a library that makes it easier to develop Airavata Django Portal customizations.
 Home-page: https://github.com/apache/airavata-django-portal-sdk
 Author: Apache Software Foundation
 Author-email: dev@airavata.apache.org
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `airavata-django-portal-sdk-1.8.2/airavata_django_portal_sdk.egg-info/SOURCES.txt` & `airavata-django-portal-sdk-1.8.3/airavata_django_portal_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-sdk-1.8.2/setup.py` & `airavata-django-portal-sdk-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="airavata-django-portal-sdk",
-    version="1.8.2",
+    version="1.8.3",
     url="https://github.com/apache/airavata-django-portal-sdk",
     author="Apache Software Foundation",
     author_email="dev@airavata.apache.org",
     description=(
         "The Airavata Django Portal SDK is a library that makes "
         "it easier to develop Airavata Django Portal customizations."
     ),
```

