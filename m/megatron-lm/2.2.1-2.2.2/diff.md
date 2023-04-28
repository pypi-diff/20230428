# Comparing `tmp/megatron-lm-2.2.1.tar.gz` & `tmp/megatron-lm-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ashish/sample-pypi-package/dist/tmp41_1mp7e/megatron-lm-2.2.1.tar", last modified: Thu Apr 27 21:30:36 2023, max compression
+gzip compressed data, was "/home/ashish/packj-recon/04-27-2023/pypi/megatron-lm/dist/tmp13cqb0ij/megatron-lm-2.2.2.tar", last modified: Fri Apr 28 15:01:53 2023, max compression
```

## Comparing `megatron-lm-2.2.1.tar` & `megatron-lm-2.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)     1831 2023-04-27 21:24:11.000000 megatron-lm-2.2.1/setup.py
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      571 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/PKG-INFO
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       38 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/setup.cfg
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron_lm.egg-info/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      571 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron_lm.egg-info/PKG-INFO
--rw-rw-r--   0 ashish    (1000) ashish    (1000)        1 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron_lm.egg-info/dependency_links.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)      190 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron_lm.egg-info/SOURCES.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       12 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron_lm.egg-info/top_level.txt
--rw-rw-r--   0 ashish    (1000) ashish    (1000)     1069 2023-04-27 21:19:14.000000 megatron-lm-2.2.1/LICENSE
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       80 2023-04-27 21:19:14.000000 megatron-lm-2.2.1/README.md
-drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-27 21:30:36.000000 megatron-lm-2.2.1/megatron-lm/
--rw-rw-r--   0 ashish    (1000) ashish    (1000)       55 2023-04-27 21:25:04.000000 megatron-lm-2.2.1/megatron-lm/__init__.py
+drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)     1831 2023-04-28 15:01:44.000000 megatron-lm-2.2.2/setup.py
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)      568 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/PKG-INFO
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)       38 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/setup.cfg
+drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron/
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)       84 2023-04-28 14:51:16.000000 megatron-lm-2.2.2/megatron/__init__.py
+drwxrwxr-x   0 ashish    (1000) ashish    (1000)        0 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)      568 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/PKG-INFO
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)        1 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)      187 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)        9 2023-04-28 15:01:53.000000 megatron-lm-2.2.2/megatron_lm.egg-info/top_level.txt
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)     1069 2023-04-27 21:19:14.000000 megatron-lm-2.2.2/LICENSE
+-rw-rw-r--   0 ashish    (1000) ashish    (1000)       77 2023-04-27 21:40:11.000000 megatron-lm-2.2.2/README.md
```

### Comparing `megatron-lm-2.2.1/setup.py` & `megatron-lm-2.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # requirements = ["requests<=2.21.0"]
 
 # Function that takes several arguments. It assigns these values to our package.
 setuptools.setup(
 	# Distribution name the package. Name must be unique so adding your username at the end is common.
 	name="megatron-lm",
 	# Version number of your package. Semantic versioning is commonly used.
-	version="2.2.1",
+	version="2.2.2",
 	# Author name.
 	author="Ashish Bijlani",
 	# Author's email address.
 	author_email="ashish.bijlani@gmail.com",
 	# Short description that will show on the PyPi page.
 	description="A placeholder package for megatron-lm",
 	# Long description that will display on the PyPi page. Uses the repo's README.md to populate this.
```

### Comparing `megatron-lm-2.2.1/PKG-INFO` & `megatron-lm-2.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.1
+Version: 2.2.2
 Summary: A placeholder package for megatron-lm
 Home-page: https://github.com/ashishbijlani/megatron-lm
 Author: Ashish Bijlani
 Author-email: ashish.bijlani@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sample PyPi Package
+# Placeholder package
+
+This is a placeholder for megatron-lm package v1.1.5 
 
-This is a simple exercise to publish a package onto PyPi.
```

### Comparing `megatron-lm-2.2.1/megatron_lm.egg-info/PKG-INFO` & `megatron-lm-2.2.2/megatron_lm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: megatron-lm
-Version: 2.2.1
+Version: 2.2.2
 Summary: A placeholder package for megatron-lm
 Home-page: https://github.com/ashishbijlani/megatron-lm
 Author: Ashish Bijlani
 Author-email: ashish.bijlani@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sample PyPi Package
+# Placeholder package
+
+This is a placeholder for megatron-lm package v1.1.5 
 
-This is a simple exercise to publish a package onto PyPi.
```

### Comparing `megatron-lm-2.2.1/LICENSE` & `megatron-lm-2.2.2/LICENSE`

 * *Files identical despite different names*

