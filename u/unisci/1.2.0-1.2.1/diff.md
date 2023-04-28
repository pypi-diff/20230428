# Comparing `tmp/unisci-1.2.0.tar.gz` & `tmp/unisci-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.2.0.tar", last modified: Thu Apr 27 04:26:09 2023, max compression
+gzip compressed data, was "unisci-1.2.1.tar", last modified: Fri Apr 28 04:24:21 2023, max compression
```

## Comparing `unisci-1.2.0.tar` & `unisci-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-27 04:26:09.956693 unisci-1.2.0/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.2.0/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.2.0/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1526 2023-04-27 04:26:09.956174 unisci-1.2.0/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1197 2023-04-26 23:42:15.000000 unisci-1.2.0/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-27 04:26:09.956822 unisci-1.2.0/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-27 04:24:57.000000 unisci-1.2.0/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-27 04:26:09.948886 unisci-1.2.0/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-27 04:24:33.000000 unisci-1.2.0/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.2.0/unisci/constants.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.2.0/unisci/conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.2.0/unisci/error.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-27 04:26:09.951117 unisci-1.2.0/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.2.0/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     8112 2023-04-26 16:06:26.000000 unisci-1.2.0/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.2.0/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-27 04:26:09.955307 unisci-1.2.0/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.2.0/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.2.0/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.2.0/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38836 2023-04-26 16:06:26.000000 unisci-1.2.0/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-27 04:26:09.950565 unisci-1.2.0/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1526 2023-04-27 04:26:09.000000 unisci-1.2.0/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      492 2023-04-27 04:26:09.000000 unisci-1.2.0/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-27 04:26:09.000000 unisci-1.2.0/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-27 04:26:09.000000 unisci-1.2.0/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-27 04:26:09.000000 unisci-1.2.0/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 04:24:21.111077 unisci-1.2.1/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.2.1/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.2.1/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1526 2023-04-28 04:24:21.110600 unisci-1.2.1/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1197 2023-04-26 23:42:15.000000 unisci-1.2.1/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-04-28 04:24:21.111184 unisci-1.2.1/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-04-28 04:22:37.000000 unisci-1.2.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 04:24:21.102745 unisci-1.2.1/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-04-28 04:22:43.000000 unisci-1.2.1/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.2.1/unisci/constants.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1508 2023-04-26 14:57:12.000000 unisci-1.2.1/unisci/conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.2.1/unisci/error.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 04:24:21.105009 unisci-1.2.1/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.2.1/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     8112 2023-04-26 16:06:26.000000 unisci-1.2.1/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1840 2023-04-26 16:06:26.000000 unisci-1.2.1/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 04:24:21.109655 unisci-1.2.1/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.2.1/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.2.1/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.2.1/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    38863 2023-04-28 04:22:19.000000 unisci-1.2.1/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-04-28 04:24:21.104471 unisci-1.2.1/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1526 2023-04-28 04:24:21.000000 unisci-1.2.1/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      492 2023-04-28 04:24:21.000000 unisci-1.2.1/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-04-28 04:24:21.000000 unisci-1.2.1/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-04-28 04:24:21.000000 unisci-1.2.1/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-04-28 04:24:21.000000 unisci-1.2.1/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.2.0/LICENSE` & `unisci-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/PKG-INFO` & `unisci-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.2.0
+Version: 1.2.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.2.0/README.md` & `unisci-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/setup.py` & `unisci-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.2.0',
+    version='1.2.1',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.2.0/unisci/conversion_factors.py` & `unisci-1.2.1/unisci/conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/error.py` & `unisci-1.2.1/unisci/error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/formulas/chemistry.py` & `unisci-1.2.1/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/metric.py` & `unisci-1.2.1/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/periodic/periodic-table-lookup.json` & `unisci-1.2.1/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/periodic/periodic-table-numbers.json` & `unisci-1.2.1/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/periodic/periodic-table-symbols.json` & `unisci-1.2.1/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.2.0/unisci/types.py` & `unisci-1.2.1/unisci/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,15 @@
 
         # simplifies unit if possible 
         if Quantity.auto_format:
             return output.simplified()
         else:
             return output
         
+    @__register_conversion
     def converted_metric(self, target: str, original: str = None) -> Quantity:
         """
         Performs metric conversions.
         Arguments: a Quantity, a target metric unit, and an original unit. If both are entered, they must be of the same metric base.
 
         Raises: CompatabilityError for incompatible units.
```

### Comparing `unisci-1.2.0/unisci.egg-info/PKG-INFO` & `unisci-1.2.1/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.2.0
+Version: 1.2.1
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

