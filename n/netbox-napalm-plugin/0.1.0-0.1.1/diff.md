# Comparing `tmp/netbox_napalm_plugin-0.1.0.tar.gz` & `tmp/netbox_napalm_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_napalm_plugin-0.1.0.tar", last modified: Wed Apr  5 20:52:20 2023, max compression
+gzip compressed data, was "netbox_napalm_plugin-0.1.1.tar", last modified: Fri Apr 28 18:02:14 2023, max compression
```

## Comparing `netbox_napalm_plugin-0.1.0.tar` & `netbox_napalm_plugin-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.437836 netbox_napalm_plugin-0.1.0/
--rw-r--r--   0 ahanson    (502) staff       (20)     3180 2023-02-21 16:21:29.000000 netbox_napalm_plugin-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 ahanson    (502) staff       (20)    10175 2023-02-17 21:27:33.000000 netbox_napalm_plugin-0.1.0/LICENSE
--rw-r--r--   0 ahanson    (502) staff       (20)      271 2023-03-23 16:18:44.000000 netbox_napalm_plugin-0.1.0/MANIFEST.in
--rw-r--r--   0 ahanson    (502) staff       (20)     3086 2023-04-05 20:52:20.437893 netbox_napalm_plugin-0.1.0/PKG-INFO
--rw-r--r--   0 ahanson    (502) staff       (20)     2419 2023-03-23 17:25:48.000000 netbox_napalm_plugin-0.1.0/README.md
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.435965 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/
--rw-r--r--   0 ahanson    (502) staff       (20)      710 2023-02-21 17:00:57.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/__init__.py
--rw-r--r--   0 ahanson    (502) staff       (20)      796 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/filtersets.py
--rw-r--r--   0 ahanson    (502) staff       (20)      471 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/forms.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.437036 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/
--rw-r--r--   0 ahanson    (502) staff       (20)     1861 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/0001_initial.py
--rw-r--r--   0 ahanson    (502) staff       (20)     1134 2023-03-23 16:24:19.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
--rw-r--r--   0 ahanson    (502) staff       (20)        0 2023-02-15 16:57:03.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/__init__.py
--rw-r--r--   0 ahanson    (502) staff       (20)     1098 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/models.py
--rw-r--r--   0 ahanson    (502) staff       (20)      507 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/navigation.py
--rw-r--r--   0 ahanson    (502) staff       (20)      640 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/tables.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.434217 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.437492 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/
--rw-r--r--   0 ahanson    (502) staff       (20)     2042 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
--rw-r--r--   0 ahanson    (502) staff       (20)     3035 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
--rw-r--r--   0 ahanson    (502) staff       (20)     1063 2023-02-16 22:20:53.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
--rw-r--r--   0 ahanson    (502) staff       (20)     3931 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
--rw-r--r--   0 ahanson    (502) staff       (20)      944 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/urls.py
--rw-r--r--   0 ahanson    (502) staff       (20)     2728 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/views.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.436689 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/
--rw-r--r--   0 ahanson    (502) staff       (20)     3086 2023-04-05 20:52:20.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 ahanson    (502) staff       (20)     1062 2023-04-05 20:52:20.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-04-05 20:52:20.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-02-15 16:27:48.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/not-zip-safe
--rw-r--r--   0 ahanson    (502) staff       (20)       11 2023-04-05 20:52:20.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/requires.txt
--rw-r--r--   0 ahanson    (502) staff       (20)       21 2023-04-05 20:52:20.000000 netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/top_level.txt
--rw-r--r--   0 ahanson    (502) staff       (20)      782 2023-04-05 20:52:20.438177 netbox_napalm_plugin-0.1.0/setup.cfg
--rw-r--r--   0 ahanson    (502) staff       (20)     1129 2023-04-05 20:51:52.000000 netbox_napalm_plugin-0.1.0/setup.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-05 20:52:20.437726 netbox_napalm_plugin-0.1.0/tests/
--rw-r--r--   0 ahanson    (502) staff       (20)       50 2023-01-27 16:45:38.000000 netbox_napalm_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0 ahanson    (502) staff       (20)      127 2023-01-27 16:45:38.000000 netbox_napalm_plugin-0.1.0/tests/test_netbox_napalm_plugin.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.028516 netbox_napalm_plugin-0.1.1/
+-rw-r--r--   0 ahanson    (502) staff       (20)     3180 2023-02-21 16:21:29.000000 netbox_napalm_plugin-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 ahanson    (502) staff       (20)    10175 2023-02-17 21:27:33.000000 netbox_napalm_plugin-0.1.1/LICENSE
+-rw-r--r--   0 ahanson    (502) staff       (20)      271 2023-03-23 16:18:44.000000 netbox_napalm_plugin-0.1.1/MANIFEST.in
+-rw-r--r--   0 ahanson    (502) staff       (20)     3086 2023-04-28 18:02:14.028587 netbox_napalm_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0 ahanson    (502) staff       (20)     2419 2023-03-23 17:25:48.000000 netbox_napalm_plugin-0.1.1/README.md
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.025037 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/
+-rw-r--r--   0 ahanson    (502) staff       (20)      710 2023-02-21 17:00:57.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/__init__.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.026509 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/api/
+-rw-r--r--   0 ahanson    (502) staff       (20)        0 2023-04-28 17:28:55.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/api/__init__.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      824 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/api/serializers.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      226 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/api/urls.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     5820 2023-02-18 00:30:59.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/api/views.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      796 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/filtersets.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      471 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/forms.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.027212 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/
+-rw-r--r--   0 ahanson    (502) staff       (20)     1861 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/0001_initial.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     1134 2023-03-23 16:24:19.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
+-rw-r--r--   0 ahanson    (502) staff       (20)        0 2023-02-15 16:57:03.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/__init__.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     1098 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/models.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      507 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/navigation.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      640 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/tables.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.021628 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.027974 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/
+-rw-r--r--   0 ahanson    (502) staff       (20)     2042 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
+-rw-r--r--   0 ahanson    (502) staff       (20)     3035 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
+-rw-r--r--   0 ahanson    (502) staff       (20)     1063 2023-02-16 22:20:53.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
+-rw-r--r--   0 ahanson    (502) staff       (20)     3931 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
+-rw-r--r--   0 ahanson    (502) staff       (20)      944 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/urls.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     2728 2023-02-17 18:49:54.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/views.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.025916 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/
+-rw-r--r--   0 ahanson    (502) staff       (20)     3086 2023-04-28 18:02:14.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 ahanson    (502) staff       (20)     1206 2023-04-28 18:02:14.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-04-28 18:02:14.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-02-15 16:27:48.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 ahanson    (502) staff       (20)       11 2023-04-28 18:02:14.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/requires.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)       21 2023-04-28 18:02:14.000000 netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)      782 2023-04-28 18:02:14.028908 netbox_napalm_plugin-0.1.1/setup.cfg
+-rw-r--r--   0 ahanson    (502) staff       (20)     1129 2023-04-28 16:54:40.000000 netbox_napalm_plugin-0.1.1/setup.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-04-28 18:02:14.028341 netbox_napalm_plugin-0.1.1/tests/
+-rw-r--r--   0 ahanson    (502) staff       (20)       50 2023-01-27 16:45:38.000000 netbox_napalm_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      127 2023-01-27 16:45:38.000000 netbox_napalm_plugin-0.1.1/tests/test_netbox_napalm_plugin.py
```

### Comparing `netbox_napalm_plugin-0.1.0/CONTRIBUTING.md` & `netbox_napalm_plugin-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/LICENSE` & `netbox_napalm_plugin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/PKG-INFO` & `netbox_napalm_plugin-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_napalm_plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: NetBox plugin for Napalm.
 Home-page: https://github.com/netbox-community/netbox-napalm
 Author: Arthur Hanson
 Author-email: ahanson@netboxlabs.com
 Keywords: netbox_napalm_plugin
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `netbox_napalm_plugin-0.1.0/README.md` & `netbox_napalm_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/__init__.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/filtersets.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/0001_initial.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/models.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/tables.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/urls.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin/views.py` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/PKG-INFO` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-napalm-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: NetBox plugin for Napalm.
 Home-page: https://github.com/netbox-community/netbox-napalm
 Author: Arthur Hanson
 Author-email: ahanson@netboxlabs.com
 Keywords: netbox_napalm_plugin
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `netbox_napalm_plugin-0.1.0/netbox_napalm_plugin.egg-info/SOURCES.txt` & `netbox_napalm_plugin-0.1.1/netbox_napalm_plugin.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 netbox_napalm_plugin/views.py
 netbox_napalm_plugin.egg-info/PKG-INFO
 netbox_napalm_plugin.egg-info/SOURCES.txt
 netbox_napalm_plugin.egg-info/dependency_links.txt
 netbox_napalm_plugin.egg-info/not-zip-safe
 netbox_napalm_plugin.egg-info/requires.txt
 netbox_napalm_plugin.egg-info/top_level.txt
+netbox_napalm_plugin/api/__init__.py
+netbox_napalm_plugin/api/serializers.py
+netbox_napalm_plugin/api/urls.py
+netbox_napalm_plugin/api/views.py
 netbox_napalm_plugin/migrations/0001_initial.py
 netbox_napalm_plugin/migrations/0002_auto_20230215_1752.py
 netbox_napalm_plugin/migrations/__init__.py
 netbox_napalm_plugin/templates/netbox_napalm_plugin/config.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/lldp_neighbors.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/napalmplatformconfig.html
 netbox_napalm_plugin/templates/netbox_napalm_plugin/status.html
```

### Comparing `netbox_napalm_plugin-0.1.0/setup.cfg` & `netbox_napalm_plugin-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [gh-actions]
 python = 
 	3.10: py310
 	3.9: py39
 	3.8: py38, format, lint, build
 
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `netbox_napalm_plugin-0.1.0/setup.py` & `netbox_napalm_plugin-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='netbox_napalm_plugin',
     name='netbox_napalm_plugin',
     packages=find_packages(include=['netbox_napalm_plugin', 'netbox_napalm_plugin.*']),
     test_suite='tests',
     url='https://github.com/netbox-community/netbox-napalm',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

