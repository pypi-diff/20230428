# Comparing `tmp/squad-foundries-plugins-1.0.tar.gz` & `tmp/squad-foundries-plugins-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad-foundries-plugins-1.0.tar", last modified: Mon Apr 24 11:10:53 2023, max compression
+gzip compressed data, was "squad-foundries-plugins-1.1.tar", last modified: Thu Apr 27 11:16:45 2023, max compression
```

## Comparing `squad-foundries-plugins-1.0.tar` & `squad-foundries-plugins-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-24 11:10:53.290684 squad-foundries-plugins-1.0/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)    26526 2023-04-24 10:54:53.000000 squad-foundries-plugins-1.0/LICENSE
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-24 11:10:53.290684 squad-foundries-plugins-1.0/PKG-INFO
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       73 2023-04-24 10:55:55.000000 squad-foundries-plugins-1.0/README
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-24 11:10:53.286683 squad-foundries-plugins-1.0/mcu/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)     2409 2023-04-24 10:51:00.000000 squad-foundries-plugins-1.0/mcu/__init__.py
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       38 2023-04-24 11:10:53.290684 squad-foundries-plugins-1.0/setup.cfg
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      661 2023-04-24 10:51:48.000000 squad-foundries-plugins-1.0/setup.py
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-24 11:10:53.290684 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/PKG-INFO
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      340 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       37 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/entry_points.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       31 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/requires.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)        4 2023-04-24 11:10:53.000000 squad-foundries-plugins-1.0/squad_foundries_plugins.egg-info/top_level.txt
-drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-24 11:10:53.290684 squad-foundries-plugins-1.0/test/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)     9150 2023-04-24 10:51:01.000000 squad-foundries-plugins-1.0/test/test_mcu.py
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)    26526 2023-04-24 10:54:53.000000 squad-foundries-plugins-1.1/LICENSE
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/PKG-INFO
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       73 2023-04-24 10:55:55.000000 squad-foundries-plugins-1.1/README
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/mcu/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)     2427 2023-04-27 11:13:25.000000 squad-foundries-plugins-1.1/mcu/__init__.py
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       38 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/setup.cfg
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      661 2023-04-27 11:13:32.000000 squad-foundries-plugins-1.1/setup.py
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      414 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      340 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       37 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/entry_points.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       31 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/requires.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)        4 2023-04-27 11:16:45.000000 squad-foundries-plugins-1.1/squad_foundries_plugins.egg-info/top_level.txt
+drwxrwxr-x   0 milosz    (1000) milosz    (1000)        0 2023-04-27 11:16:45.111244 squad-foundries-plugins-1.1/test/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)     9150 2023-04-24 10:51:01.000000 squad-foundries-plugins-1.1/test/test_mcu.py
```

### Comparing `squad-foundries-plugins-1.0/LICENSE` & `squad-foundries-plugins-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squad-foundries-plugins-1.0/mcu/__init__.py` & `squad-foundries-plugins-1.1/mcu/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             issues[issue.test_name].append(issue)
         for line in  testrun.log_file.split('\n'):
             result = regex.search(line)
             if result:
                 suite_slug = result.group("test_unit")
                 # found a potential test result
                 test_name = result.group("test_case_id")
-                expected_result = testrun.metadata.get(test_name, None)
+                expected_result = testrun.metadata.get(f"{suite_slug}/{test_name}", None)
                 if expected_result:
                     # found a matching key in metadata
                     test_result = False  # set fail as default
                     measurement = result.group("measurement")
                     if result.group("measurement") == str(expected_result):
                         # test pass
                         test_result = True
```

### Comparing `squad-foundries-plugins-1.0/setup.py` & `squad-foundries-plugins-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='squad-foundries-plugins',
-    version='1.0',
+    version='1.1',
     author='Milosz Wasilewski',
     author_email='milosz.wasilewski@foundries.io',
     url='https://github.com/foundries/squadplugins',
     packages=['mcu'],
     entry_points={
         'squad_plugins': [
             'mcu=mcu:MCUResults',
```

### Comparing `squad-foundries-plugins-1.0/test/test_mcu.py` & `squad-foundries-plugins-1.1/test/test_mcu.py`

 * *Files identical despite different names*

