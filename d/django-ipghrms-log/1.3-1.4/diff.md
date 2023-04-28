# Comparing `tmp/django-ipghrms-log-1.3.tar.gz` & `tmp/django-ipghrms-log-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-log-1.3.tar", last modified: Tue Apr 11 09:24:41 2023, max compression
+gzip compressed data, was "dist\django-ipghrms-log-1.4.tar", last modified: Fri Apr 28 22:02:43 2023, max compression
```

## Comparing `django-ipghrms-log-1.3.tar` & `django-ipghrms-log-1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.546406 django-ipghrms-log-1.3/
--rw-rw-rw-   0        0        0     1063 2023-03-27 14:48:18.000000 django-ipghrms-log-1.3/LICENSE
--rw-rw-rw-   0        0        0      106 2023-03-27 14:22:19.000000 django-ipghrms-log-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      906 2023-04-11 09:24:41.546944 django-ipghrms-log-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-03-27 14:22:26.000000 django-ipghrms-log-1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.266206 django-ipghrms-log-1.3/django_ipghrms_log.egg-info/
--rw-rw-rw-   0        0        0      906 2023-04-11 09:24:41.000000 django-ipghrms-log-1.3/django_ipghrms_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2023-04-11 09:24:41.000000 django-ipghrms-log-1.3/django_ipghrms_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:24:41.000000 django-ipghrms-log-1.3/django_ipghrms_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-11 09:24:41.000000 django-ipghrms-log-1.3/django_ipghrms_log.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.311932 django-ipghrms-log-1.3/log/
--rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.3/log/__init__.py
--rw-rw-rw-   0        0        0       89 2023-02-16 04:28:52.000000 django-ipghrms-log-1.3/log/admin.py
--rw-rw-rw-   0        0        0      144 2023-02-16 04:18:51.000000 django-ipghrms-log-1.3/log/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.363963 django-ipghrms-log-1.3/log/migrations/
--rw-rw-rw-   0        0        0     1219 2023-02-16 04:25:03.000000 django-ipghrms-log-1.3/log/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      562 2023-02-23 00:29:37.000000 django-ipghrms-log-1.3/log/migrations/0002_auto_20230223_0929.py
--rw-rw-rw-   0        0        0      767 2023-02-23 01:48:52.000000 django-ipghrms-log-1.3/log/migrations/0003_auto_20230223_1048.py
--rw-rw-rw-   0        0        0      423 2023-02-23 02:03:34.000000 django-ipghrms-log-1.3/log/migrations/0004_log_priv_address.py
--rw-rw-rw-   0        0        0      402 2023-02-23 06:29:44.000000 django-ipghrms-log-1.3/log/migrations/0005_log_hashed.py
--rw-rw-rw-   0        0        0      409 2023-02-23 07:12:11.000000 django-ipghrms-log-1.3/log/migrations/0006_log_device.py
--rw-rw-rw-   0        0        0      410 2023-02-23 14:45:39.000000 django-ipghrms-log-1.3/log/migrations/0007_log_ip_type.py
--rw-rw-rw-   0        0        0      415 2023-02-23 14:55:25.000000 django-ipghrms-log-1.3/log/migrations/0008_alter_log_ip_type.py
--rw-rw-rw-   0        0        0      376 2023-02-23 14:56:41.000000 django-ipghrms-log-1.3/log/migrations/0009_rename_ip_type_log_is_private.py
--rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.3/log/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.515613 django-ipghrms-log-1.3/log/migrations/__pycache__/
--rw-rw-rw-   0        0        0     1140 2023-02-16 04:25:10.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0      611 2023-02-23 00:29:45.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc
--rw-rw-rw-   0        0        0      675 2023-02-23 01:49:01.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc
--rw-rw-rw-   0        0        0      595 2023-02-23 02:03:45.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc
--rw-rw-rw-   0        0        0      572 2023-02-23 06:29:50.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2023-02-23 07:12:18.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0006_log_device.cpython-310.pyc
--rw-rw-rw-   0        0        0      577 2023-02-23 14:45:46.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2023-02-23 14:55:32.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc
--rw-rw-rw-   0        0        0      546 2023-02-23 14:56:46.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc
--rw-rw-rw-   0        0        0      141 2023-02-16 04:25:03.000000 django-ipghrms-log-1.3/log/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1252 2023-02-23 14:56:31.000000 django-ipghrms-log-1.3/log/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.200854 django-ipghrms-log-1.3/log/templates/
-drwxrwxrwx   0        0        0        0 2023-04-11 09:24:41.535774 django-ipghrms-log-1.3/log/templates/log/
--rw-rw-rw-   0        0        0     5476 2023-02-24 06:35:43.000000 django-ipghrms-log-1.3/log/templates/log/detail.html
--rw-rw-rw-   0        0        0     6531 2023-03-28 03:36:37.000000 django-ipghrms-log-1.3/log/templates/log/list.html
--rw-rw-rw-   0        0        0       63 2023-02-16 04:18:51.000000 django-ipghrms-log-1.3/log/tests.py
--rw-rw-rw-   0        0        0      188 2023-02-23 06:33:49.000000 django-ipghrms-log-1.3/log/urls.py
--rw-rw-rw-   0        0        0     1148 2023-04-11 09:18:51.000000 django-ipghrms-log-1.3/log/utils.py
--rw-rw-rw-   0        0        0     2664 2023-03-28 03:36:49.000000 django-ipghrms-log-1.3/log/views.py
--rw-rw-rw-   0        0        0      501 2023-04-11 09:24:41.550655 django-ipghrms-log-1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-log-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:43.082812 django-ipghrms-log-1.4/
+-rw-rw-rw-   0        0        0     1063 2023-03-27 14:48:18.000000 django-ipghrms-log-1.4/LICENSE
+-rw-rw-rw-   0        0        0      106 2023-03-27 14:22:19.000000 django-ipghrms-log-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1113 2023-04-28 22:02:43.083811 django-ipghrms-log-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-03-27 14:22:26.000000 django-ipghrms-log-1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:42.855598 django-ipghrms-log-1.4/django_ipghrms_log.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-28 22:02:42.000000 django-ipghrms-log-1.4/django_ipghrms_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2023-04-28 22:02:42.000000 django-ipghrms-log-1.4/django_ipghrms_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:02:42.000000 django-ipghrms-log-1.4/django_ipghrms_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:02:42.000000 django-ipghrms-log-1.4/django_ipghrms_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:42.870560 django-ipghrms-log-1.4/log/
+-rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.4/log/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-02-16 04:28:52.000000 django-ipghrms-log-1.4/log/admin.py
+-rw-rw-rw-   0        0        0      144 2023-02-16 04:18:51.000000 django-ipghrms-log-1.4/log/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:42.891034 django-ipghrms-log-1.4/log/migrations/
+-rw-rw-rw-   0        0        0     1219 2023-02-16 04:25:03.000000 django-ipghrms-log-1.4/log/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      562 2023-02-23 00:29:37.000000 django-ipghrms-log-1.4/log/migrations/0002_auto_20230223_0929.py
+-rw-rw-rw-   0        0        0      767 2023-02-23 01:48:52.000000 django-ipghrms-log-1.4/log/migrations/0003_auto_20230223_1048.py
+-rw-rw-rw-   0        0        0      423 2023-02-23 02:03:34.000000 django-ipghrms-log-1.4/log/migrations/0004_log_priv_address.py
+-rw-rw-rw-   0        0        0      402 2023-02-23 06:29:44.000000 django-ipghrms-log-1.4/log/migrations/0005_log_hashed.py
+-rw-rw-rw-   0        0        0      409 2023-02-23 07:12:11.000000 django-ipghrms-log-1.4/log/migrations/0006_log_device.py
+-rw-rw-rw-   0        0        0      410 2023-02-23 14:45:39.000000 django-ipghrms-log-1.4/log/migrations/0007_log_ip_type.py
+-rw-rw-rw-   0        0        0      415 2023-02-23 14:55:25.000000 django-ipghrms-log-1.4/log/migrations/0008_alter_log_ip_type.py
+-rw-rw-rw-   0        0        0      376 2023-02-23 14:56:41.000000 django-ipghrms-log-1.4/log/migrations/0009_rename_ip_type_log_is_private.py
+-rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.4/log/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:43.079876 django-ipghrms-log-1.4/log/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     1140 2023-02-16 04:25:10.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0      611 2023-02-23 00:29:45.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc
+-rw-rw-rw-   0        0        0      675 2023-02-23 01:49:01.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc
+-rw-rw-rw-   0        0        0      595 2023-02-23 02:03:45.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc
+-rw-rw-rw-   0        0        0      572 2023-02-23 06:29:50.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2023-02-23 07:12:18.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0006_log_device.cpython-310.pyc
+-rw-rw-rw-   0        0        0      577 2023-02-23 14:45:46.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2023-02-23 14:55:32.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc
+-rw-rw-rw-   0        0        0      546 2023-02-23 14:56:46.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc
+-rw-rw-rw-   0        0        0      141 2023-02-16 04:25:03.000000 django-ipghrms-log-1.4/log/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1252 2023-02-23 14:56:31.000000 django-ipghrms-log-1.4/log/models.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:42.824726 django-ipghrms-log-1.4/log/templates/
+drwxrwxrwx   0        0        0        0 2023-04-28 22:02:43.081815 django-ipghrms-log-1.4/log/templates/log/
+-rw-rw-rw-   0        0        0     5485 2023-04-28 22:00:40.000000 django-ipghrms-log-1.4/log/templates/log/detail.html
+-rw-rw-rw-   0        0        0     6531 2023-03-28 03:36:37.000000 django-ipghrms-log-1.4/log/templates/log/list.html
+-rw-rw-rw-   0        0        0       63 2023-02-16 04:18:51.000000 django-ipghrms-log-1.4/log/tests.py
+-rw-rw-rw-   0        0        0      188 2023-02-23 06:33:49.000000 django-ipghrms-log-1.4/log/urls.py
+-rw-rw-rw-   0        0        0     1148 2023-04-11 09:18:51.000000 django-ipghrms-log-1.4/log/utils.py
+-rw-rw-rw-   0        0        0     2664 2023-03-28 03:36:49.000000 django-ipghrms-log-1.4/log/views.py
+-rw-rw-rw-   0        0        0      501 2023-04-28 22:02:43.089794 django-ipghrms-log-1.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-log-1.4/setup.py
```

### Comparing `django-ipghrms-log-1.3/LICENSE` & `django-ipghrms-log-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/PKG-INFO` & `django-ipghrms-log-1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: django-ipghrms-log
-Version: 1.3
+Version: 1.4
 Summary: Django IPG HRMS APP LOG
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
+Description: 
+        ============================
+        Django IPG HRMS log
+        ============================
+        
+        
+        Quick start
+        ============
+        
+        
+        1. Add 'log' to your INSTALLED_APPS settings like this::
+        
+            INSTALLED_APPS = [
+                'log'
+            ]
+        
+        2. Include the log to project URLS like this::
+        
+            path('log/', include('log.urls')),
+        
+        3. Run ``python manage.py migrate`` to create log model
+        
+        4. Another Apps Need for this Apps::
+            4.1. custom::
+            4.2. employee::
+            4.3. user
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-
-============================
-Django IPG HRMS log
-============================
-
-
-Quick start
-============
-
-
-1. Add 'log' to your INSTALLED_APPS settings like this::
-
-    INSTALLED_APPS = [
-        'log'
-    ]
-
-2. Include the log to project URLS like this::
-
-    path('log/', include('log.urls')),
-
-3. Run ``python manage.py migrate`` to create log model
-
-4. Another Apps Need for this Apps::
-    4.1. custom::
-    4.2. employee::
-    4.3. user
```

### Comparing `django-ipghrms-log-1.3/django_ipghrms_log.egg-info/PKG-INFO` & `django-ipghrms-log-1.4/django_ipghrms_log.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: django-ipghrms-log
-Version: 1.3
+Version: 1.4
 Summary: Django IPG HRMS APP LOG
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
+Description: 
+        ============================
+        Django IPG HRMS log
+        ============================
+        
+        
+        Quick start
+        ============
+        
+        
+        1. Add 'log' to your INSTALLED_APPS settings like this::
+        
+            INSTALLED_APPS = [
+                'log'
+            ]
+        
+        2. Include the log to project URLS like this::
+        
+            path('log/', include('log.urls')),
+        
+        3. Run ``python manage.py migrate`` to create log model
+        
+        4. Another Apps Need for this Apps::
+            4.1. custom::
+            4.2. employee::
+            4.3. user
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-
-============================
-Django IPG HRMS log
-============================
-
-
-Quick start
-============
-
-
-1. Add 'log' to your INSTALLED_APPS settings like this::
-
-    INSTALLED_APPS = [
-        'log'
-    ]
-
-2. Include the log to project URLS like this::
-
-    path('log/', include('log.urls')),
-
-3. Run ``python manage.py migrate`` to create log model
-
-4. Another Apps Need for this Apps::
-    4.1. custom::
-    4.2. employee::
-    4.3. user
```

### Comparing `django-ipghrms-log-1.3/django_ipghrms_log.egg-info/SOURCES.txt` & `django-ipghrms-log-1.4/django_ipghrms_log.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/0001_initial.py` & `django-ipghrms-log-1.4/log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/0002_auto_20230223_0929.py` & `django-ipghrms-log-1.4/log/migrations/0002_auto_20230223_0929.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/0003_auto_20230223_1048.py` & `django-ipghrms-log-1.4/log/migrations/0003_auto_20230223_1048.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0006_log_device.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0006_log_device.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc` & `django-ipghrms-log-1.4/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/models.py` & `django-ipghrms-log-1.4/log/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/templates/log/detail.html` & `django-ipghrms-log-1.4/log/templates/log/detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                                     <table class="table table-sm table-striped table-bordered">
                                         <thead>
                                             <tr align="center">
                                                 <th colspan="10">INFOMASAUN LOG</th>
                                             </tr>
                                         </thead>
                                         <tr>
-                                            <th>Public IP Address</th><th>Country/City</th> <th>Username</th><th>Model/Table</th> <th>Data ID</th> <th>Action</th> <th>Datetime</th> <th>Lat.</th> <th>Lon.</th>
+                                            <th>Public IP Address</th><th>Country/City</th> <th>Username</th><th>Model/Table</th> <th>Data ID</th> <th>Action</th> <th>Datetime</th> <th>Latitude</th> <th>Longitude</th>
                                         </tr>
                                         <tr>
                                             <td>{{objects.ip_address}}</td>
                                             <td>{{objects.country}} 
                                                 {% if objects.city %} /  
                                                 {{objects.city}}
                                                 {% else %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends "main/layout.html" %} {% load humanize %} {% block content %}
     * LISTA_LOG
     * {{ legend|upper }}
 
                         ***** {{ legend|upper }} *****
                                                                                                                            INFOMASAUN LOG
-Public IP Address     Country/City       Username            Model/Table      Data ID             Action            Datetime             Lat.                Lon.
+Public IP Address     Country/City       Username            Model/Table      Data ID             Action            Datetime             Latitude            Longitude
                       {
                       {objects.country}}
 {                     {% if objects.city {                   {                {                   {                 {                    {                   {
 {objects.ip_address}} %} / {             {objects.username}} {objects.model}} {objects.field_id}} {objects.action}} {objects.timestamp}} {objects.latitude}} {objects.longitude}}
                       {objects.city}} {%
                       else %} - {% endif
                       %}
```

### Comparing `django-ipghrms-log-1.3/log/templates/log/list.html` & `django-ipghrms-log-1.4/log/templates/log/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/utils.py` & `django-ipghrms-log-1.4/log/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.3/log/views.py` & `django-ipghrms-log-1.4/log/views.py`

 * *Files identical despite different names*

