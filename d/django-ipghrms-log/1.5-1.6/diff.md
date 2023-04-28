# Comparing `tmp/django-ipghrms-log-1.5.tar.gz` & `tmp/django-ipghrms-log-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-ipghrms-log-1.5.tar", last modified: Fri Apr 28 22:17:52 2023, max compression
+gzip compressed data, was "dist\django-ipghrms-log-1.6.tar", last modified: Fri Apr 28 22:44:15 2023, max compression
```

## Comparing `django-ipghrms-log-1.5.tar` & `django-ipghrms-log-1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.791499 django-ipghrms-log-1.5/
--rw-rw-rw-   0        0        0     1063 2023-03-27 14:48:18.000000 django-ipghrms-log-1.5/LICENSE
--rw-rw-rw-   0        0        0      106 2023-03-27 14:22:19.000000 django-ipghrms-log-1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1113 2023-04-28 22:17:52.792498 django-ipghrms-log-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-03-27 14:22:26.000000 django-ipghrms-log-1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.758052 django-ipghrms-log-1.5/django_ipghrms_log.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-28 22:17:52.000000 django-ipghrms-log-1.5/django_ipghrms_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1389 2023-04-28 22:17:52.000000 django-ipghrms-log-1.5/django_ipghrms_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 22:17:52.000000 django-ipghrms-log-1.5/django_ipghrms_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 22:17:52.000000 django-ipghrms-log-1.5/django_ipghrms_log.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.766580 django-ipghrms-log-1.5/log/
--rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.5/log/__init__.py
--rw-rw-rw-   0        0        0       89 2023-02-16 04:28:52.000000 django-ipghrms-log-1.5/log/admin.py
--rw-rw-rw-   0        0        0      144 2023-02-16 04:18:51.000000 django-ipghrms-log-1.5/log/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.777452 django-ipghrms-log-1.5/log/migrations/
--rw-rw-rw-   0        0        0     1219 2023-02-16 04:25:03.000000 django-ipghrms-log-1.5/log/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      562 2023-02-23 00:29:37.000000 django-ipghrms-log-1.5/log/migrations/0002_auto_20230223_0929.py
--rw-rw-rw-   0        0        0      767 2023-02-23 01:48:52.000000 django-ipghrms-log-1.5/log/migrations/0003_auto_20230223_1048.py
--rw-rw-rw-   0        0        0      423 2023-02-23 02:03:34.000000 django-ipghrms-log-1.5/log/migrations/0004_log_priv_address.py
--rw-rw-rw-   0        0        0      402 2023-02-23 06:29:44.000000 django-ipghrms-log-1.5/log/migrations/0005_log_hashed.py
--rw-rw-rw-   0        0        0      409 2023-02-23 07:12:11.000000 django-ipghrms-log-1.5/log/migrations/0006_log_device.py
--rw-rw-rw-   0        0        0      410 2023-02-23 14:45:39.000000 django-ipghrms-log-1.5/log/migrations/0007_log_ip_type.py
--rw-rw-rw-   0        0        0      415 2023-02-23 14:55:25.000000 django-ipghrms-log-1.5/log/migrations/0008_alter_log_ip_type.py
--rw-rw-rw-   0        0        0      376 2023-02-23 14:56:41.000000 django-ipghrms-log-1.5/log/migrations/0009_rename_ip_type_log_is_private.py
--rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.5/log/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.789505 django-ipghrms-log-1.5/log/migrations/__pycache__/
--rw-rw-rw-   0        0        0     1140 2023-02-16 04:25:10.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0      611 2023-02-23 00:29:45.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc
--rw-rw-rw-   0        0        0      675 2023-02-23 01:49:01.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc
--rw-rw-rw-   0        0        0      595 2023-02-23 02:03:45.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc
--rw-rw-rw-   0        0        0      572 2023-02-23 06:29:50.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2023-02-23 07:12:18.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0006_log_device.cpython-310.pyc
--rw-rw-rw-   0        0        0      577 2023-02-23 14:45:46.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2023-02-23 14:55:32.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc
--rw-rw-rw-   0        0        0      546 2023-02-23 14:56:46.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc
--rw-rw-rw-   0        0        0      141 2023-02-16 04:25:03.000000 django-ipghrms-log-1.5/log/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1252 2023-02-23 14:56:31.000000 django-ipghrms-log-1.5/log/models.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.740406 django-ipghrms-log-1.5/log/templates/
-drwxrwxrwx   0        0        0        0 2023-04-28 22:17:52.791499 django-ipghrms-log-1.5/log/templates/log/
--rw-rw-rw-   0        0        0     5485 2023-04-28 22:00:40.000000 django-ipghrms-log-1.5/log/templates/log/detail.html
--rw-rw-rw-   0        0        0     6536 2023-04-28 22:17:36.000000 django-ipghrms-log-1.5/log/templates/log/list.html
--rw-rw-rw-   0        0        0       63 2023-02-16 04:18:51.000000 django-ipghrms-log-1.5/log/tests.py
--rw-rw-rw-   0        0        0      188 2023-02-23 06:33:49.000000 django-ipghrms-log-1.5/log/urls.py
--rw-rw-rw-   0        0        0     1148 2023-04-11 09:18:51.000000 django-ipghrms-log-1.5/log/utils.py
--rw-rw-rw-   0        0        0     2664 2023-03-28 03:36:49.000000 django-ipghrms-log-1.5/log/views.py
--rw-rw-rw-   0        0        0      501 2023-04-28 22:17:52.793494 django-ipghrms-log-1.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-log-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.216427 django-ipghrms-log-1.6/
+-rw-rw-rw-   0        0        0     1063 2023-03-27 14:48:18.000000 django-ipghrms-log-1.6/LICENSE
+-rw-rw-rw-   0        0        0      106 2023-03-27 14:22:19.000000 django-ipghrms-log-1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1113 2023-04-28 22:44:15.216427 django-ipghrms-log-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-03-27 14:22:26.000000 django-ipghrms-log-1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.181520 django-ipghrms-log-1.6/django_ipghrms_log.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-28 22:44:15.000000 django-ipghrms-log-1.6/django_ipghrms_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1389 2023-04-28 22:44:15.000000 django-ipghrms-log-1.6/django_ipghrms_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:44:15.000000 django-ipghrms-log-1.6/django_ipghrms_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 22:44:15.000000 django-ipghrms-log-1.6/django_ipghrms_log.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.191495 django-ipghrms-log-1.6/log/
+-rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.6/log/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-02-16 04:28:52.000000 django-ipghrms-log-1.6/log/admin.py
+-rw-rw-rw-   0        0        0      144 2023-02-16 04:18:51.000000 django-ipghrms-log-1.6/log/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.202464 django-ipghrms-log-1.6/log/migrations/
+-rw-rw-rw-   0        0        0     1219 2023-02-16 04:25:03.000000 django-ipghrms-log-1.6/log/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      562 2023-02-23 00:29:37.000000 django-ipghrms-log-1.6/log/migrations/0002_auto_20230223_0929.py
+-rw-rw-rw-   0        0        0      767 2023-02-23 01:48:52.000000 django-ipghrms-log-1.6/log/migrations/0003_auto_20230223_1048.py
+-rw-rw-rw-   0        0        0      423 2023-02-23 02:03:34.000000 django-ipghrms-log-1.6/log/migrations/0004_log_priv_address.py
+-rw-rw-rw-   0        0        0      402 2023-02-23 06:29:44.000000 django-ipghrms-log-1.6/log/migrations/0005_log_hashed.py
+-rw-rw-rw-   0        0        0      409 2023-02-23 07:12:11.000000 django-ipghrms-log-1.6/log/migrations/0006_log_device.py
+-rw-rw-rw-   0        0        0      410 2023-02-23 14:45:39.000000 django-ipghrms-log-1.6/log/migrations/0007_log_ip_type.py
+-rw-rw-rw-   0        0        0      415 2023-02-23 14:55:25.000000 django-ipghrms-log-1.6/log/migrations/0008_alter_log_ip_type.py
+-rw-rw-rw-   0        0        0      376 2023-02-23 14:56:41.000000 django-ipghrms-log-1.6/log/migrations/0009_rename_ip_type_log_is_private.py
+-rw-rw-rw-   0        0        0        0 2023-02-16 04:18:51.000000 django-ipghrms-log-1.6/log/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.213437 django-ipghrms-log-1.6/log/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     1140 2023-02-16 04:25:10.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0      611 2023-02-23 00:29:45.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc
+-rw-rw-rw-   0        0        0      675 2023-02-23 01:49:01.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc
+-rw-rw-rw-   0        0        0      595 2023-02-23 02:03:45.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc
+-rw-rw-rw-   0        0        0      572 2023-02-23 06:29:50.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2023-02-23 07:12:18.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0006_log_device.cpython-310.pyc
+-rw-rw-rw-   0        0        0      577 2023-02-23 14:45:46.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2023-02-23 14:55:32.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc
+-rw-rw-rw-   0        0        0      546 2023-02-23 14:56:46.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc
+-rw-rw-rw-   0        0        0      141 2023-02-16 04:25:03.000000 django-ipghrms-log-1.6/log/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1252 2023-02-23 14:56:31.000000 django-ipghrms-log-1.6/log/models.py
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.162572 django-ipghrms-log-1.6/log/templates/
+drwxrwxrwx   0        0        0        0 2023-04-28 22:44:15.215430 django-ipghrms-log-1.6/log/templates/log/
+-rw-rw-rw-   0        0        0     5485 2023-04-28 22:00:40.000000 django-ipghrms-log-1.6/log/templates/log/detail.html
+-rw-rw-rw-   0        0        0     6531 2023-04-28 22:43:46.000000 django-ipghrms-log-1.6/log/templates/log/list.html
+-rw-rw-rw-   0        0        0       63 2023-02-16 04:18:51.000000 django-ipghrms-log-1.6/log/tests.py
+-rw-rw-rw-   0        0        0      188 2023-02-23 06:33:49.000000 django-ipghrms-log-1.6/log/urls.py
+-rw-rw-rw-   0        0        0     1148 2023-04-11 09:18:51.000000 django-ipghrms-log-1.6/log/utils.py
+-rw-rw-rw-   0        0        0     2664 2023-03-28 03:36:49.000000 django-ipghrms-log-1.6/log/views.py
+-rw-rw-rw-   0        0        0      501 2023-04-28 22:44:15.219418 django-ipghrms-log-1.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-log-1.6/setup.py
```

### Comparing `django-ipghrms-log-1.5/LICENSE` & `django-ipghrms-log-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/PKG-INFO` & `django-ipghrms-log-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-ipghrms-log
-Version: 1.5
+Version: 1.6
 Summary: Django IPG HRMS APP LOG
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-log-1.5/django_ipghrms_log.egg-info/PKG-INFO` & `django-ipghrms-log-1.6/django_ipghrms_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-ipghrms-log
-Version: 1.5
+Version: 1.6
 Summary: Django IPG HRMS APP LOG
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-log-1.5/django_ipghrms_log.egg-info/SOURCES.txt` & `django-ipghrms-log-1.6/django_ipghrms_log.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/0001_initial.py` & `django-ipghrms-log-1.6/log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/0002_auto_20230223_0929.py` & `django-ipghrms-log-1.6/log/migrations/0002_auto_20230223_0929.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/0003_auto_20230223_1048.py` & `django-ipghrms-log-1.6/log/migrations/0003_auto_20230223_1048.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0002_auto_20230223_0929.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0003_auto_20230223_1048.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0004_log_priv_address.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0005_log_hashed.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0006_log_device.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0006_log_device.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0007_log_ip_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0008_alter_log_ip_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc` & `django-ipghrms-log-1.6/log/migrations/__pycache__/0009_rename_ip_type_log_is_private.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/models.py` & `django-ipghrms-log-1.6/log/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/templates/log/detail.html` & `django-ipghrms-log-1.6/log/templates/log/detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/templates/log/list.html` & `django-ipghrms-log-1.6/log/templates/log/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 </div>
 <div class="container-fluid"><br/>
 	<div class="row">
 		<div class="col-sm-12">
 			<div class="card shadow-lg border-info rounded">
 				<div class="card-header border-primary">
 					<center>
-						<h2>TEST {{ legend|upper }}
+						<h2>{{ legend|upper }}
                             {% if page == 'filter' %}
                               <i class="fa fa-arrow-right"></i>
                               Fulan <span class="text-danger" >{{monthname}}</span>, Tinan <span class="text-danger">{{year}}</span>
                             {% endif %}
                         </h2>
 					</center>
                     <div class="row mt-1">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends "main/layout.html" %} {% load static %} {% block content %}
     * {{ legend|upper }}
 
-TEST {{ legend|upper }} {% if page == 'filter' %}  Fulan {{monthname}}, Tinan {
+  {{ legend|upper }} {% if page == 'filter' %}  Fulan {{monthname}}, Tinan {
                               {year}} {% endif %}
 {% csrf_token %}
 {% for y in years %}
 {{ y }}
 {% endfor %}
 {% for m in months %}
 {{ m.name }}
```

### Comparing `django-ipghrms-log-1.5/log/utils.py` & `django-ipghrms-log-1.6/log/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-log-1.5/log/views.py` & `django-ipghrms-log-1.6/log/views.py`

 * *Files identical despite different names*

