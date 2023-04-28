# Comparing `tmp/netbox-documents-0.5.0.tar.gz` & `tmp/netbox-documents-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-documents-0.5.0.tar", last modified: Tue Jan 24 08:10:46 2023, max compression
+gzip compressed data, was "netbox-documents-0.6.0.tar", last modified: Fri Apr 28 11:54:50 2023, max compression
```

## Comparing `netbox-documents-0.5.0.tar` & `netbox-documents-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.402217 netbox-documents-0.5.0/
--rw-r--r--   0 jyates     (501) staff       (20)    11357 2023-01-03 16:33:55.000000 netbox-documents-0.5.0/LICENSE
--rw-r--r--   0 jyates     (501) staff       (20)       80 2023-01-03 16:33:55.000000 netbox-documents-0.5.0/MANIFEST.in
--rw-r--r--   0 jyates     (501) staff       (20)     5351 2023-01-24 08:10:46.401857 netbox-documents-0.5.0/PKG-INFO
--rw-r--r--   0 jyates     (501) staff       (20)     5004 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/README.md
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.368156 netbox-documents-0.5.0/netbox_documents/
--rw-r--r--   0 jyates     (501) staff       (20)      825 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/__init__.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.381820 netbox-documents-0.5.0/netbox_documents/api/
--rw-r--r--   0 jyates     (501) staff       (20)        0 2023-01-03 16:33:55.000000 netbox-documents-0.5.0/netbox_documents/api/__init__.py
--rw-r--r--   0 jyates     (501) staff       (20)     3573 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/api/serializers.py
--rw-r--r--   0 jyates     (501) staff       (20)      413 2023-01-04 13:37:43.000000 netbox-documents-0.5.0/netbox_documents/api/urls.py
--rw-r--r--   0 jyates     (501) staff       (20)     1129 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/api/views.py
--rw-r--r--   0 jyates     (501) staff       (20)     1728 2023-01-05 19:28:23.000000 netbox-documents-0.5.0/netbox_documents/filtersets.py
--rw-r--r--   0 jyates     (501) staff       (20)     3482 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/forms.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.389497 netbox-documents-0.5.0/netbox_documents/migrations/
--rw-r--r--   0 jyates     (501) staff       (20)     3867 2023-01-03 16:33:55.000000 netbox-documents-0.5.0/netbox_documents/migrations/0001_initial.py
--rw-r--r--   0 jyates     (501) staff       (20)     1611 2023-01-04 13:37:43.000000 netbox-documents-0.5.0/netbox_documents/migrations/0002_AddDeviceType.py
--rw-r--r--   0 jyates     (501) staff       (20)     4032 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py
--rw-r--r--   0 jyates     (501) staff       (20)        0 2023-01-03 16:33:55.000000 netbox-documents-0.5.0/netbox_documents/migrations/__init__.py
--rw-r--r--   0 jyates     (501) staff       (20)    13885 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/models.py
--rw-r--r--   0 jyates     (501) staff       (20)     3017 2023-01-05 19:28:23.000000 netbox-documents-0.5.0/netbox_documents/navigation.py
--rw-r--r--   0 jyates     (501) staff       (20)     1146 2023-01-05 11:34:27.000000 netbox-documents-0.5.0/netbox_documents/search.py
--rw-r--r--   0 jyates     (501) staff       (20)     4406 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/tables.py
--rw-r--r--   0 jyates     (501) staff       (20)     3884 2023-01-04 13:37:43.000000 netbox-documents-0.5.0/netbox_documents/template_content.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.331383 netbox-documents-0.5.0/netbox_documents/templates/
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.401281 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/
--rw-r--r--   0 jyates     (501) staff       (20)     1680 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument.html
--rw-r--r--   0 jyates     (501) staff       (20)     1933 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument_edit.html
--rw-r--r--   0 jyates     (501) staff       (20)     2275 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument_include.html
--rw-r--r--   0 jyates     (501) staff       (20)     1670 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument.html
--rw-r--r--   0 jyates     (501) staff       (20)     1932 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument_edit.html
--rw-r--r--   0 jyates     (501) staff       (20)     2253 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument_include.html
--rw-r--r--   0 jyates     (501) staff       (20)     1696 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument.html
--rw-r--r--   0 jyates     (501) staff       (20)     1937 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html
--rw-r--r--   0 jyates     (501) staff       (20)     2297 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument_include.html
--rw-r--r--   0 jyates     (501) staff       (20)     1959 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/document_edit.html
--rw-r--r--   0 jyates     (501) staff       (20)     1660 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument.html
--rw-r--r--   0 jyates     (501) staff       (20)     1930 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument_edit.html
--rw-r--r--   0 jyates     (501) staff       (20)     2250 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument_include.html
--rw-r--r--   0 jyates     (501) staff       (20)     3071 2023-01-05 19:28:23.000000 netbox-documents-0.5.0/netbox_documents/urls.py
--rw-r--r--   0 jyates     (501) staff       (20)      941 2023-01-04 13:37:43.000000 netbox-documents-0.5.0/netbox_documents/utils.py
--rw-r--r--   0 jyates     (501) staff       (20)     2853 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/netbox_documents/views.py
-drwxr-xr-x   0 jyates     (501) staff       (20)        0 2023-01-24 08:10:46.374450 netbox-documents-0.5.0/netbox_documents.egg-info/
--rw-r--r--   0 jyates     (501) staff       (20)     5351 2023-01-24 08:10:46.000000 netbox-documents-0.5.0/netbox_documents.egg-info/PKG-INFO
--rw-r--r--   0 jyates     (501) staff       (20)     1778 2023-01-24 08:10:46.000000 netbox-documents-0.5.0/netbox_documents.egg-info/SOURCES.txt
--rw-r--r--   0 jyates     (501) staff       (20)        1 2023-01-24 08:10:46.000000 netbox-documents-0.5.0/netbox_documents.egg-info/dependency_links.txt
--rw-r--r--   0 jyates     (501) staff       (20)        1 2023-01-04 13:38:41.000000 netbox-documents-0.5.0/netbox_documents.egg-info/not-zip-safe
--rw-r--r--   0 jyates     (501) staff       (20)       17 2023-01-24 08:10:46.000000 netbox-documents-0.5.0/netbox_documents.egg-info/top_level.txt
--rw-r--r--   0 jyates     (501) staff       (20)       38 2023-01-24 08:10:46.402295 netbox-documents-0.5.0/setup.cfg
--rw-r--r--   0 jyates     (501) staff       (20)      757 2023-01-24 08:10:11.000000 netbox-documents-0.5.0/setup.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.282951 netbox-documents-0.6.0/
+-rw-r--r--   0 jasonyates   (502) staff       (20)    11357 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/LICENSE
+-rw-r--r--   0 jasonyates   (502) staff       (20)       80 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/MANIFEST.in
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5512 2023-04-28 11:54:50.282791 netbox-documents-0.6.0/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5165 2023-04-28 11:50:06.000000 netbox-documents-0.6.0/README.md
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.273557 netbox-documents-0.6.0/netbox_documents/
+-rw-r--r--   0 jasonyates   (502) staff       (20)      825 2023-04-28 11:51:34.000000 netbox-documents-0.6.0/netbox_documents/__init__.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.277396 netbox-documents-0.6.0/netbox_documents/api/
+-rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/api/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3573 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/api/serializers.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      413 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/api/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1129 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/api/views.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1728 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/filtersets.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3489 2023-04-28 11:46:48.000000 netbox-documents-0.6.0/netbox_documents/forms.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.278566 netbox-documents-0.6.0/netbox_documents/migrations/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3867 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/migrations/0001_initial.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1611 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/migrations/0002_AddDeviceType.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4032 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/migrations/__init__.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)    13885 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/models.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3017 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/navigation.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1146 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/search.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     4406 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/tables.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3884 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/template_content.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.268113 netbox-documents-0.6.0/netbox_documents/templates/
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.282486 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1680 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1933 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2275 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1670 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1932 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2253 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1696 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1937 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2297 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1959 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/document_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1660 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1930 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument_edit.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2250 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument_include.html
+-rw-r--r--   0 jasonyates   (502) staff       (20)     3071 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/urls.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)      941 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/utils.py
+-rw-r--r--   0 jasonyates   (502) staff       (20)     2853 2023-04-28 11:45:21.000000 netbox-documents-0.6.0/netbox_documents/views.py
+drwxr-xr-x   0 jasonyates   (502) staff       (20)        0 2023-04-28 11:54:50.275944 netbox-documents-0.6.0/netbox_documents.egg-info/
+-rw-r--r--   0 jasonyates   (502) staff       (20)     5512 2023-04-28 11:54:50.000000 netbox-documents-0.6.0/netbox_documents.egg-info/PKG-INFO
+-rw-r--r--   0 jasonyates   (502) staff       (20)     1778 2023-04-28 11:54:50.000000 netbox-documents-0.6.0/netbox_documents.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-04-28 11:54:50.000000 netbox-documents-0.6.0/netbox_documents.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)        1 2023-04-28 11:45:44.000000 netbox-documents-0.6.0/netbox_documents.egg-info/not-zip-safe
+-rw-r--r--   0 jasonyates   (502) staff       (20)       17 2023-04-28 11:54:50.000000 netbox-documents-0.6.0/netbox_documents.egg-info/top_level.txt
+-rw-r--r--   0 jasonyates   (502) staff       (20)       38 2023-04-28 11:54:50.282997 netbox-documents-0.6.0/setup.cfg
+-rw-r--r--   0 jasonyates   (502) staff       (20)      757 2023-04-28 11:51:16.000000 netbox-documents-0.6.0/setup.py
```

### Comparing `netbox-documents-0.5.0/LICENSE` & `netbox-documents-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/PKG-INFO` & `netbox-documents-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-documents
-Version: 0.5.0
+Version: 0.6.0
 Summary: Manage site, circuit and device diagrams and documents in Netbox
 Home-page: https://github.com/jasonyates/netbox-documents
 Author: Jason Yates
 Author-email: me@jasonyates.co.uk
 Keywords: netbox,netbox-plugin,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,20 +26,21 @@
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       |      0.5.0     |
+|     3.5+       |      0.6.0     |
+| 3.2.x - 3.4.x  |      0.5.0     |
 
 
 ## Installation
 
-A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
+A working installation of Netbox 3.2+ is required. 3.5+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
 
 #### Package Installation from PyPi
 
 Activate your virtual env and install via pip:
 
 ```
 $ source /opt/netbox/venv/bin/activate
```

### Comparing `netbox-documents-0.5.0/README.md` & `netbox-documents-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       |      0.5.0     |
+|     3.5+       |      0.6.0     |
+| 3.2.x - 3.4.x  |      0.5.0     |
 
 
 ## Installation
 
-A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
+A working installation of Netbox 3.2+ is required. 3.5+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
 
 #### Package Installation from PyPi
 
 Activate your virtual env and install via pip:
 
 ```
 $ source /opt/netbox/venv/bin/activate
```

### Comparing `netbox-documents-0.5.0/netbox_documents/__init__.py` & `netbox-documents-0.6.0/netbox_documents/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from extras.plugins import PluginConfig
 
 class NetboxDocuments(PluginConfig):
     name = 'netbox_documents'
     verbose_name = 'Document Storage'
     description = 'Manage site, circuit and device diagrams and documents in Netbox'
-    version = '0.5.0'
+    version = '0.6.0'
     author = 'Jason Yates'
     author_email = 'me@jasonyates.co.uk'
-    min_version = '3.2.0'
+    min_version = '3.5.0'
     base_url = 'documents'
     default_settings = {
         "enable_site_documents": True,
         "enable_circuit_documents": True,
         "enable_device_documents": True,
         "enable_device_type_documents": True, 
         "enable_navigation_menu": True,
```

### Comparing `netbox-documents-0.5.0/netbox_documents/api/serializers.py` & `netbox-documents-0.6.0/netbox_documents/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/api/views.py` & `netbox-documents-0.6.0/netbox_documents/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/filtersets.py` & `netbox-documents-0.6.0/netbox_documents/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/forms.py` & `netbox-documents-0.6.0/netbox_documents/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
 from dcim.models import Site, Device, DeviceType 
 from circuits.models import Circuit
-from utilities.forms import TagFilterField, CommentField, DynamicModelChoiceField
+from utilities.forms.fields import TagFilterField, CommentField, DynamicModelChoiceField
 from .models import SiteDocument, DeviceDocument, DeviceTypeDocument, CircuitDocument, CircuitDocTypeChoices, SiteDocTypeChoices, DeviceDocTypeChoices, DeviceTypeDocTypeChoices 
 
 
 #### Site Document Form & Filter Form
 class SiteDocumentForm(NetBoxModelForm):
     comments = CommentField()
```

### Comparing `netbox-documents-0.5.0/netbox_documents/migrations/0001_initial.py` & `netbox-documents-0.6.0/netbox_documents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/migrations/0002_AddDeviceType.py` & `netbox-documents-0.6.0/netbox_documents/migrations/0002_AddDeviceType.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py` & `netbox-documents-0.6.0/netbox_documents/migrations/0003_alter_circuitdocument_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/models.py` & `netbox-documents-0.6.0/netbox_documents/models.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/navigation.py` & `netbox-documents-0.6.0/netbox_documents/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/search.py` & `netbox-documents-0.6.0/netbox_documents/search.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/tables.py` & `netbox-documents-0.6.0/netbox_documents/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/template_content.py` & `netbox-documents-0.6.0/netbox_documents/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument_edit.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/circuitdocument_include.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/circuitdocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument_edit.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicedocument_include.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/devicetypedocument_include.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/devicetypedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/document_edit.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/document_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument_edit.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/templates/netbox_documents/sitedocument_include.html` & `netbox-documents-0.6.0/netbox_documents/templates/netbox_documents/sitedocument_include.html`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/urls.py` & `netbox-documents-0.6.0/netbox_documents/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/utils.py` & `netbox-documents-0.6.0/netbox_documents/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents/views.py` & `netbox-documents-0.6.0/netbox_documents/views.py`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/netbox_documents.egg-info/PKG-INFO` & `netbox-documents-0.6.0/netbox_documents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-documents
-Version: 0.5.0
+Version: 0.6.0
 Summary: Manage site, circuit and device diagrams and documents in Netbox
 Home-page: https://github.com/jasonyates/netbox-documents
 Author: Jason Yates
 Author-email: me@jasonyates.co.uk
 Keywords: netbox,netbox-plugin,plugin
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,20 +26,21 @@
 * Store links to external URL's to save duplication of remote documents
 
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|     3.2+       |      0.5.0     |
+|     3.5+       |      0.6.0     |
+| 3.2.x - 3.4.x  |      0.5.0     |
 
 
 ## Installation
 
-A working installation of Netbox 3.2+ is required. 3.4+ is recommended.
+A working installation of Netbox 3.2+ is required. 3.5+ is recommended. **NOTE: Netbox 3.5 introduced breaking changes for plugins, please use the correct plugin version for your netbox install.**
 
 #### Package Installation from PyPi
 
 Activate your virtual env and install via pip:
 
 ```
 $ source /opt/netbox/venv/bin/activate
```

### Comparing `netbox-documents-0.5.0/netbox_documents.egg-info/SOURCES.txt` & `netbox-documents-0.6.0/netbox_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-documents-0.5.0/setup.py` & `netbox-documents-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='netbox-documents',
-    version='0.5.0',
+    version='0.6.0',
     description='Manage site, circuit and device diagrams and documents in Netbox',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason Yates',
     author_email='me@jasonyates.co.uk',
     url='https://github.com/jasonyates/netbox-documents',
     install_requires=[],
```

