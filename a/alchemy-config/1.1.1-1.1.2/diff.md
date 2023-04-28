# Comparing `tmp/alchemy-config-1.1.1.tar.gz` & `tmp/alchemy-config-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alchemy-config-1.1.1.tar", last modified: Tue Apr 25 21:56:59 2023, max compression
+gzip compressed data, was "dist/alchemy-config-1.1.2.tar", last modified: Fri Apr 28 01:09:19 2023, max compression
```

## Comparing `alchemy-config-1.1.1.tar` & `alchemy-config-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1316 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/alchemy_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/test/
--rw-r--r--   0 root         (0) root         (0)    11628 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/test/test_attribute_access_dict.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      964 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 21:56:59.000000 alchemy-config-1.1.1/aconfig/
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/aconfig/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14360 2023-04-25 21:56:32.000000 alchemy-config-1.1.1/aconfig/aconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/alchemy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/aconfig/
+-rw-r--r--   0 root         (0) root         (0)    14434 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/aconfig/aconfig.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/aconfig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 01:09:19.000000 alchemy-config-1.1.2/test/
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/test/test_attribute_access_dict.py
+-rw-r--r--   0 root         (0) root         (0)    11777 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 01:08:53.000000 alchemy-config-1.1.2/LICENSE
```

### Comparing `alchemy-config-1.1.1/LICENSE` & `alchemy-config-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.1/PKG-INFO` & `alchemy-config-1.1.2/alchemy_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-config
-Version: 1.1.1
+Version: 1.1.2
 Summary: Configuration framework in Python for general configuration use.
 Home-page: https://github.com/IBM/alchemy-config
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: config
 Platform: UNKNOWN
```

### Comparing `alchemy-config-1.1.1/alchemy_config.egg-info/PKG-INFO` & `alchemy-config-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-config
-Version: 1.1.1
+Version: 1.1.2
 Summary: Configuration framework in Python for general configuration use.
 Home-page: https://github.com/IBM/alchemy-config
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: config
 Platform: UNKNOWN
```

### Comparing `alchemy-config-1.1.1/setup.py` & `alchemy-config-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.1/test/test_config.py` & `alchemy-config-1.1.2/test/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,24 @@
         self.assertEqual(getattr(locals(), 'bad_config1', None), None)
 
         # tests a bad-location error
         with self.assertRaises(AssertionError) as ex2:
             bad_config2 = aconfig.Config._verify_config_location(fixtures.BAD_CONFIG_LOCATION)
         raised_exception2 = ex2.exception
         self.assertIsInstance(raised_exception2, AssertionError)
+        self.assertIn(fixtures.BAD_CONFIG_LOCATION, str(ex2.exception))
         # make sure bad_config2 was NOT initialized
         self.assertEqual(getattr(locals(), 'bad_config2', None), None)
 
         # tests a non-config-file error
         with self.assertRaises(AssertionError) as ex3:
             bad_config3 = aconfig.Config._verify_config_location(fixtures.NOT_YAML_CONFIG_LOCATION)
         raised_exception3 = ex3.exception
         self.assertIsInstance(raised_exception3, AssertionError)
+        self.assertIn(fixtures.NOT_YAML_CONFIG_LOCATION, str(ex3.exception))
         # make sure bad_config3 was NOT initialized
         self.assertEqual(getattr(locals(), 'bad_config3', None), None)
 
     def test__load_yaml_file_pass(self):
         '''Test _load_yaml_file passes. By the time it gets here, the file location has been verified
         '''
         loaded_yaml = aconfig.Config._load_yaml_file(fixtures.GOOD_CONFIG_LOCATION)
```

### Comparing `alchemy-config-1.1.1/test/test_attribute_access_dict.py` & `alchemy-config-1.1.2/test/test_attribute_access_dict.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.1/README.md` & `alchemy-config-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.1/aconfig/__init__.py` & `alchemy-config-1.1.2/aconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemy-config-1.1.1/aconfig/aconfig.py` & `alchemy-config-1.1.2/aconfig/aconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,18 +209,18 @@
         assert isinstance(config_location, str), \
             'config_location must be str, but you sent in type: <{0}>'.format(type(config_location))
 
         # cross-platform location relative to this file
         config_location = os.path.normpath(config_location)
 
         assert (config_location.endswith('.yml') or config_location.endswith('.yaml')), \
-            'Must send in a .yaml or .yaml file'
+            'Must send in a .yaml or .yaml file, you sent in: <{0}>'.format(config_location)
 
         assert os.path.exists(config_location), \
-            'config_location does not exist or cannot be found!'
+            'config_location <{0}> does not exist or cannot be found!'.format(config_location)
 
         # finally found it's valid
         return config_location
 
     @staticmethod
     def _load_yaml_file(config_location):
         '''Helper to load .yaml file at location. Assumes file location has been validated.
```

