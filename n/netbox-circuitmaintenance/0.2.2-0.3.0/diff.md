# Comparing `tmp/netbox-circuitmaintenance-0.2.2.tar.gz` & `tmp/netbox-circuitmaintenance-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-circuitmaintenance-0.2.2.tar", last modified: Wed Jan 18 11:57:34 2023, max compression
+gzip compressed data, was "netbox-circuitmaintenance-0.3.0.tar", last modified: Fri Apr 28 13:28:05 2023, max compression
```

## Comparing `netbox-circuitmaintenance-0.2.2.tar` & `netbox-circuitmaintenance-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.296187 netbox-circuitmaintenance-0.2.2/
--rw-r--r--   0 jyates     (501) staff       (20)     3260 2023-01-16 16:54:53.000000 netbox-circuitmaintenance-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 jyates     (501) staff       (20)        1 2023-01-15 15:30:08.000000 netbox-circuitmaintenance-0.2.2/LICENSE
--rw-r--r--   0 jyates     (501) staff       (20)      327 2023-01-17 09:27:01.000000 netbox-circuitmaintenance-0.2.2/MANIFEST.in
--rw-r--r--   0 jyates     (501) staff       (20)     3110 2023-01-18 11:57:34.296312 netbox-circuitmaintenance-0.2.2/PKG-INFO
--rw-r--r--   0 jyates     (501) staff       (20)     2174 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/README.md
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.169005 netbox-circuitmaintenance-0.2.2/docs/
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.227748 netbox-circuitmaintenance-0.2.2/docs/img/
--rw-r--r--   0 jyates     (501) staff       (20)    29513 2023-01-17 10:39:05.000000 netbox-circuitmaintenance-0.2.2/docs/img/circuit_maintenance.png
--rw-r--r--   0 jyates     (501) staff       (20)   167395 2023-01-17 10:38:49.000000 netbox-circuitmaintenance-0.2.2/docs/img/maintenance.png
--rw-r--r--   0 jyates     (501) staff       (20)    71837 2023-01-17 10:39:38.000000 netbox-circuitmaintenance-0.2.2/docs/img/provider_maintenance.png
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.250667 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/
--rw-r--r--   0 jyates     (501) staff       (20)      481 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/__init__.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.265289 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/
--rw-r--r--   0 jyates     (501) staff       (20)     3385 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/serializers.py
--rw-r--r--   0 jyates     (501) staff       (20)      406 2023-01-16 16:14:57.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/urls.py
--rw-r--r--   0 jyates     (501) staff       (20)     1017 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/views.py
--rw-r--r--   0 jyates     (501) staff       (20)     1389 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/filtersets.py
--rw-r--r--   0 jyates     (501) staff       (20)     2187 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/forms.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.278816 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/
--rw-r--r--   0 jyates     (501) staff       (20)     7196 2023-01-16 14:46:44.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0001_squashed_0005_alter_circuitmaintenance_options.py
--rw-r--r--   0 jyates     (501) staff       (20)      677 2023-01-16 16:05:17.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0006_circuitmaintenancenotifications_email_body_and_more.py
--rw-r--r--   0 jyates     (501) staff       (20)      948 2023-01-16 16:29:43.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0007_alter_circuitmaintenancenotifications_options_and_more.py
--rw-r--r--   0 jyates     (501) staff       (20)        0 2023-01-15 17:29:33.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/__init__.py
--rw-r--r--   0 jyates     (501) staff       (20)     5367 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/models.py
--rw-r--r--   0 jyates     (501) staff       (20)      900 2023-01-17 10:51:55.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/navigation.py
--rw-r--r--   0 jyates     (501) staff       (20)      866 2023-01-16 08:59:05.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/tables.py
--rw-r--r--   0 jyates     (501) staff       (20)     1632 2023-01-16 14:35:17.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/template_content.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.174279 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.288676 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/
--rw-r--r--   0 jyates     (501) staff       (20)     7706 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance.html
--rw-r--r--   0 jyates     (501) staff       (20)     1028 2023-01-16 14:21:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance_include.html
--rw-r--r--   0 jyates     (501) staff       (20)       26 2023-01-16 16:42:54.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenancenotifications.html
--rw-r--r--   0 jyates     (501) staff       (20)     1113 2023-01-16 14:31:43.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/providermaintenance_include.html
--rw-r--r--   0 jyates     (501) staff       (20)     2075 2023-01-16 16:49:19.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/urls.py
--rw-r--r--   0 jyates     (501) staff       (20)     2306 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/views.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.260070 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/
--rw-r--r--   0 jyates     (501) staff       (20)     3110 2023-01-18 11:57:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/PKG-INFO
--rw-r--r--   0 jyates     (501) staff       (20)     1695 2023-01-18 11:57:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/SOURCES.txt
--rw-r--r--   0 jyates     (501) staff       (20)        1 2023-01-18 11:57:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/dependency_links.txt
--rw-r--r--   0 jyates     (501) staff       (20)        1 2023-01-15 15:36:42.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/not-zip-safe
--rw-r--r--   0 jyates     (501) staff       (20)       44 2023-01-18 11:57:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/requires.txt
--rw-r--r--   0 jyates     (501) staff       (20)       26 2023-01-18 11:57:34.000000 netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/top_level.txt
--rw-r--r--   0 jyates     (501) staff       (20)     1116 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/pyproject.toml
--rw-r--r--   0 jyates     (501) staff       (20)      787 2023-01-18 11:57:34.298768 netbox-circuitmaintenance-0.2.2/setup.cfg
--rw-r--r--   0 jyates     (501) staff       (20)     1108 2023-01-18 11:56:22.000000 netbox-circuitmaintenance-0.2.2/setup.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-18 11:57:34.295308 netbox-circuitmaintenance-0.2.2/tests/
--rw-r--r--   0 jyates     (501) staff       (20)       55 2023-01-15 15:30:08.000000 netbox-circuitmaintenance-0.2.2/tests/__init__.py
--rw-r--r--   0 jyates     (501) staff       (20)      142 2023-01-15 15:30:08.000000 netbox-circuitmaintenance-0.2.2/tests/test_netbox_circuitmaintenance.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.562665 netbox-circuitmaintenance-0.3.0/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3260 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/LICENSE
+-rw-r--r--   0 jasonyates   (502) staff       (20)      356 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/MANIFEST.in
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4167 2023-04-28 13:28:05.562743 netbox-circuitmaintenance-0.3.0/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3231 2023-04-28 13:26:03.000000 netbox-circuitmaintenance-0.3.0/README.md
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.544746 netbox-circuitmaintenance-0.3.0/docs/
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.553593 netbox-circuitmaintenance-0.3.0/docs/img/
+-rw-r--r--   0 jasonyates   (502) staff       (20)   118326 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/S3_permissions.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)   324802 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/S3_permissions2.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)    35465 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/SES_Lambda.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)   205483 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/SES_invoke.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)    65717 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/SES_ruleset.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)    29513 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/circuit_maintenance.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)   109410 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/iam_permissions.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)   128075 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/lambda_create.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)   167395 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/maintenance.png
+-rw-r--r--   0 jasonyates   (502) staff       (20)    71837 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/docs/img/provider_maintenance.png
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.556882 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/
+-rw-r--r--   0 jasonyates   (502) staff       (20)      481 2023-04-28 13:23:23.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/__init__.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.559450 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3385 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/serializers.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      406 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1017 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/views.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1389 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/filtersets.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2229 2023-04-28 13:22:19.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/forms.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.560681 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     7196 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0001_squashed_0005_alter_circuitmaintenance_options.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      677 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0006_circuitmaintenancenotifications_email_body_and_more.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      948 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0007_alter_circuitmaintenancenotifications_options_and_more.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5367 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/models.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      900 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/navigation.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      866 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/tables.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1632 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/template_content.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.546014 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.561885 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     7706 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1028 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)       26 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenancenotifications.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1113 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/providermaintenance_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2075 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2306 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/views.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.558579 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4167 2023-04-28 13:28:05.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1881 2023-04-28 13:28:05.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-04-28 13:28:05.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-04-28 13:20:36.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/not-zip-safe
+-rw-r--r--   0 jasonyates   (502) staff       (20)       44 2023-04-28 13:28:05.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/requires.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)       26 2023-04-28 13:28:05.000000 netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/top_level.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1116 2023-04-28 13:24:06.000000 netbox-circuitmaintenance-0.3.0/pyproject.toml
+-rw-r--r--   0 jasonyates   (502) staff       (20)      787 2023-04-28 13:28:05.563143 netbox-circuitmaintenance-0.3.0/setup.cfg
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1108 2023-04-28 13:23:41.000000 netbox-circuitmaintenance-0.3.0/setup.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 13:28:05.562422 netbox-circuitmaintenance-0.3.0/tests/
+-rw-r--r--   0 jasonyates   (502) staff       (20)       55 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/tests/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      142 2023-04-28 12:05:37.000000 netbox-circuitmaintenance-0.3.0/tests/test_netbox_circuitmaintenance.py
```

### Comparing `netbox-circuitmaintenance-0.2.2/CONTRIBUTING.md` & `netbox-circuitmaintenance-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/PKG-INFO` & `netbox-circuitmaintenance-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-circuitmaintenance
-Version: 0.2.2
+Version: 0.3.0
 Summary: Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits.
 Home-page: https://github.com/jasonyates/netbox-circuitmaintenance
 Author: Jason Yates
 Author-email: Jason Yates <me@jasonyates.co.uk>
 License: 
         
 Project-URL: Homepage, https://github.com/jasonyates/netbox-circuitmaintenance
@@ -17,37 +17,44 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-=================================
 # Netbox Circuit Maintenance Plugin
-=================================
 
-NetBox plugin for managing Circuit Maintenance events.
+Documentation: [https://jasonyates.github.io/netbox-circuitmaintenance/](https://jasonyates.github.io/netbox-circuitmaintenance/)
 
-See Github Feature Requests for upcoming list of features.
+A NetBox plugin built to track circuit maintenance events, the plugin itself is agnostic in that it is only built to store data surrounding maintenance events and provide an overview of historical, active and upcoming circuit and provider maintenance events. The plugin tracks maintenance events at the provider level and associates impact from each event at the circuit level.
+
+The plugin does not directly provide an automated approach to ingesting provider notifications, instead it extends NetBox's extensive REST API and provides GET/POST/PUT/PATCH methods to manage maintenance events. The plugin is intended to be coupled with an automated parser to handle the parsing of provider notifications and the delivery of the maintenance events to the plugin's REST API. Several example parsers have been documented [here](https://jasonyates.github.io/netbox-circuitmaintenance/parsers/).
 
 ## Features
 
-Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits.
+ - Track provider maintenance events
+ - Track circuit impact from provider maintenance
+ - Provides a consolidated view of active, upcoming and historical maintenance events at the provider and circuit level
+ - Consolidated notifications (coming soon)
+ - Maintenance overlap detection (coming soon)
 
 ## Compatibility
-
+This plugin is only supported on NetBox 3.4 or higher, for exact compatibility information, see the table below.  
 | NetBox Version | Plugin Version |
-|----------------|----------------|
-|     3.4        |      0.2.2     |
+|--|--|
+| 3.5 | 0.3.0 |
+| 3.4 | 0.2.2 |
+
+
 
 ## Installing
 
 A working installation of Netbox 3.4+ is required - [see official documentation](https://netbox.readthedocs.io/en/stable/plugins/).
 
-### Package Installation from PyPi
+### Package Installation
 
 Activate your virtual env and install via pip::
 
 ```bash
 $ source /opt/netbox/venv/bin/activate
 (venv) $ pip install netbox-circuitmaintenance
 ```
```

### Comparing `netbox-circuitmaintenance-0.2.2/README.md` & `netbox-circuitmaintenance-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-=================================
 # Netbox Circuit Maintenance Plugin
-=================================
 
-NetBox plugin for managing Circuit Maintenance events.
+Documentation: [https://jasonyates.github.io/netbox-circuitmaintenance/](https://jasonyates.github.io/netbox-circuitmaintenance/)
 
-See Github Feature Requests for upcoming list of features.
+A NetBox plugin built to track circuit maintenance events, the plugin itself is agnostic in that it is only built to store data surrounding maintenance events and provide an overview of historical, active and upcoming circuit and provider maintenance events. The plugin tracks maintenance events at the provider level and associates impact from each event at the circuit level.
+
+The plugin does not directly provide an automated approach to ingesting provider notifications, instead it extends NetBox's extensive REST API and provides GET/POST/PUT/PATCH methods to manage maintenance events. The plugin is intended to be coupled with an automated parser to handle the parsing of provider notifications and the delivery of the maintenance events to the plugin's REST API. Several example parsers have been documented [here](https://jasonyates.github.io/netbox-circuitmaintenance/parsers/).
 
 ## Features
 
-Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits.
+ - Track provider maintenance events
+ - Track circuit impact from provider maintenance
+ - Provides a consolidated view of active, upcoming and historical maintenance events at the provider and circuit level
+ - Consolidated notifications (coming soon)
+ - Maintenance overlap detection (coming soon)
 
 ## Compatibility
-
+This plugin is only supported on NetBox 3.4 or higher, for exact compatibility information, see the table below.  
 | NetBox Version | Plugin Version |
-|----------------|----------------|
-|     3.4        |      0.2.2     |
+|--|--|
+| 3.5 | 0.3.0 |
+| 3.4 | 0.2.2 |
+
+
 
 ## Installing
 
 A working installation of Netbox 3.4+ is required - [see official documentation](https://netbox.readthedocs.io/en/stable/plugins/).
 
-### Package Installation from PyPi
+### Package Installation
 
 Activate your virtual env and install via pip::
 
 ```bash
 $ source /opt/netbox/venv/bin/activate
 (venv) $ pip install netbox-circuitmaintenance
 ```
```

### Comparing `netbox-circuitmaintenance-0.2.2/docs/img/circuit_maintenance.png` & `netbox-circuitmaintenance-0.3.0/docs/img/circuit_maintenance.png`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/docs/img/maintenance.png` & `netbox-circuitmaintenance-0.3.0/docs/img/maintenance.png`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/docs/img/provider_maintenance.png` & `netbox-circuitmaintenance-0.3.0/docs/img/provider_maintenance.png`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/serializers.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/api/views.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/filtersets.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/forms.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
-from utilities.forms import DateTimePicker, DynamicModelChoiceField
+from utilities.forms.fields import DynamicModelChoiceField
+from utilities.forms.widgets import DateTimePicker
 from circuits.models import Provider, Circuit
 from .models import CircuitMaintenance, CircuitMaintenanceImpact, CircuitMaintenanceNotifications, CircuitMaintenanceTypeChoices, CircuitMaintenanceImpactTypeChoices
 
 class CircuitMaintenanceForm(NetBoxModelForm):
 
     provider = DynamicModelChoiceField(
         queryset=Provider.objects.all()
```

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0001_squashed_0005_alter_circuitmaintenance_options.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0001_squashed_0005_alter_circuitmaintenance_options.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0006_circuitmaintenancenotifications_email_body_and_more.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0006_circuitmaintenancenotifications_email_body_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/migrations/0007_alter_circuitmaintenancenotifications_options_and_more.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/migrations/0007_alter_circuitmaintenancenotifications_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/models.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/models.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/navigation.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/tables.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/template_content.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance.html` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance.html`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance_include.html` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/circuitmaintenance_include.html`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/providermaintenance_include.html` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/templates/netbox_circuitmaintenance/providermaintenance_include.html`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/urls.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance/views.py` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance/views.py`

 * *Files identical despite different names*

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/PKG-INFO` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-circuitmaintenance
-Version: 0.2.2
+Version: 0.3.0
 Summary: Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits.
 Home-page: https://github.com/jasonyates/netbox-circuitmaintenance
 Author: Jason Yates
 Author-email: Jason Yates <me@jasonyates.co.uk>
 License: 
         
 Project-URL: Homepage, https://github.com/jasonyates/netbox-circuitmaintenance
@@ -17,37 +17,44 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-=================================
 # Netbox Circuit Maintenance Plugin
-=================================
 
-NetBox plugin for managing Circuit Maintenance events.
+Documentation: [https://jasonyates.github.io/netbox-circuitmaintenance/](https://jasonyates.github.io/netbox-circuitmaintenance/)
 
-See Github Feature Requests for upcoming list of features.
+A NetBox plugin built to track circuit maintenance events, the plugin itself is agnostic in that it is only built to store data surrounding maintenance events and provide an overview of historical, active and upcoming circuit and provider maintenance events. The plugin tracks maintenance events at the provider level and associates impact from each event at the circuit level.
+
+The plugin does not directly provide an automated approach to ingesting provider notifications, instead it extends NetBox's extensive REST API and provides GET/POST/PUT/PATCH methods to manage maintenance events. The plugin is intended to be coupled with an automated parser to handle the parsing of provider notifications and the delivery of the maintenance events to the plugin's REST API. Several example parsers have been documented [here](https://jasonyates.github.io/netbox-circuitmaintenance/parsers/).
 
 ## Features
 
-Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits.
+ - Track provider maintenance events
+ - Track circuit impact from provider maintenance
+ - Provides a consolidated view of active, upcoming and historical maintenance events at the provider and circuit level
+ - Consolidated notifications (coming soon)
+ - Maintenance overlap detection (coming soon)
 
 ## Compatibility
-
+This plugin is only supported on NetBox 3.4 or higher, for exact compatibility information, see the table below.  
 | NetBox Version | Plugin Version |
-|----------------|----------------|
-|     3.4        |      0.2.2     |
+|--|--|
+| 3.5 | 0.3.0 |
+| 3.4 | 0.2.2 |
+
+
 
 ## Installing
 
 A working installation of Netbox 3.4+ is required - [see official documentation](https://netbox.readthedocs.io/en/stable/plugins/).
 
-### Package Installation from PyPi
+### Package Installation
 
 Activate your virtual env and install via pip::
 
 ```bash
 $ source /opt/netbox/venv/bin/activate
 (venv) $ pip install netbox-circuitmaintenance
 ```
```

### Comparing `netbox-circuitmaintenance-0.2.2/netbox_circuitmaintenance.egg-info/SOURCES.txt` & `netbox-circuitmaintenance-0.3.0/netbox_circuitmaintenance.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+docs/img/S3_permissions.png
+docs/img/S3_permissions2.png
+docs/img/SES_Lambda.png
+docs/img/SES_invoke.png
+docs/img/SES_ruleset.png
 docs/img/circuit_maintenance.png
+docs/img/iam_permissions.png
+docs/img/lambda_create.png
 docs/img/maintenance.png
 docs/img/provider_maintenance.png
 netbox_circuitmaintenance/__init__.py
 netbox_circuitmaintenance/filtersets.py
 netbox_circuitmaintenance/forms.py
 netbox_circuitmaintenance/models.py
 netbox_circuitmaintenance/navigation.py
```

### Comparing `netbox-circuitmaintenance-0.2.2/pyproject.toml` & `netbox-circuitmaintenance-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-circuitmaintenance"
-version = "0.2.2"
+version = "0.3.0"
 description = "Provides the ability to record circuit maintenance, maintenance impact and maintenance notifications in Netbox and link them to Providers and Circuits."
 readme = "README.md"
 authors = [{ name = "Jason Yates", email = "me@jasonyates.co.uk" }]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/jasonyates/netbox-circuitmaintenance"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.2.2"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `netbox-circuitmaintenance-0.2.2/setup.cfg` & `netbox-circuitmaintenance-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [gh-actions]
 python = 
 	3.10: py310
 	3.9: py39
 	3.8: py38, format, lint, build
 
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `netbox-circuitmaintenance-0.2.2/setup.py` & `netbox-circuitmaintenance-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     long_description=readme + '\n\n',
     include_package_data=True,
     keywords='netbox_circuitmaintenance',
     name='netbox_circuitmaintenance',
     packages=find_packages(include=['netbox_circuitmaintenance', 'netbox_circuitmaintenance.*']),
     test_suite='tests',
     url='https://github.com/jasonyates/netbox-circuitmaintenance',
-    version='0.2.2',
+    version='0.3.0',
     zip_safe=False,
 )
```

