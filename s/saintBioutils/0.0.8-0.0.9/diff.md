# Comparing `tmp/saintBioutils-0.0.8.tar.gz` & `tmp/saintBioutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saintBioutils-0.0.8.tar", last modified: Sun Jan  9 21:30:15 2022, max compression
+gzip compressed data, was "saintBioutils-0.0.9.tar", last modified: Sun Jan  9 21:34:02 2022, max compression
```

## Comparing `saintBioutils-0.0.8.tar` & `saintBioutils-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:30:15.131109 saintBioutils-0.0.8/
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     1184 2022-01-09 20:47:20.000000 saintBioutils-0.0.8/LICENSE
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2329 2022-01-09 21:30:15.131109 saintBioutils-0.0.8/PKG-INFO
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     1512 2022-01-09 20:47:20.000000 saintBioutils-0.0.8/README.md
-drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:30:15.089108 saintBioutils-0.0.8/saintBioutils/
-drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:30:15.108108 saintBioutils-0.0.8/saintBioutils/genbank/
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2751 2022-01-09 21:16:10.000000 saintBioutils-0.0.8/saintBioutils/genbank/__init__.py
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     6151 2022-01-09 21:16:10.000000 saintBioutils-0.0.8/saintBioutils/genbank/get_genomes.py
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     4549 2022-01-09 21:16:10.000000 saintBioutils-0.0.8/saintBioutils/genbank/parse_genomes.py
-drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:30:15.128109 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2329 2022-01-09 21:30:15.000000 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/PKG-INFO
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)      390 2022-01-09 21:30:15.000000 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        1 2022-01-09 21:30:15.000000 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)       21 2022-01-09 21:30:15.000000 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/requires.txt
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        8 2022-01-09 21:30:15.000000 saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/top_level.txt
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)       38 2022-01-09 21:30:15.132108 saintBioutils-0.0.8/setup.cfg
--rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     3036 2022-01-09 21:29:10.000000 saintBioutils-0.0.8/setup.py
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.129821 saintBioutils-0.0.9/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     1184 2022-01-09 20:47:20.000000 saintBioutils-0.0.9/LICENSE
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2329 2022-01-09 21:34:02.129821 saintBioutils-0.0.9/PKG-INFO
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     1512 2022-01-09 20:47:20.000000 saintBioutils-0.0.9/README.md
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.059822 saintBioutils-0.0.9/saintBioutils/
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.082821 saintBioutils-0.0.9/saintBioutils/genbank/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2751 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/genbank/__init__.py
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     6151 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/genbank/get_genomes.py
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     4549 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/genbank/parse_genomes.py
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.108821 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     2329 2022-01-09 21:34:02.000000 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)      558 2022-01-09 21:34:02.000000 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        1 2022-01-09 21:34:02.000000 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)       21 2022-01-09 21:34:02.000000 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/requires.txt
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)       18 2022-01-09 21:34:02.000000 saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/top_level.txt
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.113821 saintBioutils-0.0.9/saintBioutils/utilities/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     1545 2022-01-09 21:32:57.000000 saintBioutils-0.0.9/saintBioutils/utilities/__init__.py
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.121840 saintBioutils-0.0.9/saintBioutils/utilities/file_io/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     3050 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/utilities/file_io/__init__.py
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     4678 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/utilities/file_io/get_paths.py
+drwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)        0 2022-01-09 21:34:02.126821 saintBioutils-0.0.9/saintBioutils/utilities/logger/
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     3587 2022-01-09 21:16:10.000000 saintBioutils-0.0.9/saintBioutils/utilities/logger/__init__.py
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)       38 2022-01-09 21:34:02.130822 saintBioutils-0.0.9/setup.cfg
+-rwxrwxrwx   0 hobnobmancer  (1000) hobnobmancer  (1000)     3036 2022-01-09 21:33:16.000000 saintBioutils-0.0.9/setup.py
```

### Comparing `saintBioutils-0.0.8/LICENSE` & `saintBioutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `saintBioutils-0.0.8/PKG-INFO` & `saintBioutils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saintBioutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package of utility and miscellaneous functions for using in bioinformaticspipelines, primarily in Python.
 Home-page: https://github.com/HobnobMancer/saintBioutils
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics python
 Platform: Posix
```

### Comparing `saintBioutils-0.0.8/README.md` & `saintBioutils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `saintBioutils-0.0.8/saintBioutils/genbank/__init__.py` & `saintBioutils-0.0.9/saintBioutils/genbank/__init__.py`

 * *Files identical despite different names*

### Comparing `saintBioutils-0.0.8/saintBioutils/genbank/get_genomes.py` & `saintBioutils-0.0.9/saintBioutils/genbank/get_genomes.py`

 * *Files identical despite different names*

### Comparing `saintBioutils-0.0.8/saintBioutils/genbank/parse_genomes.py` & `saintBioutils-0.0.9/saintBioutils/genbank/parse_genomes.py`

 * *Files identical despite different names*

### Comparing `saintBioutils-0.0.8/saintBioutils/saintBioutils.egg-info/PKG-INFO` & `saintBioutils-0.0.9/saintBioutils/saintBioutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saintBioutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package of utility and miscellaneous functions for using in bioinformaticspipelines, primarily in Python.
 Home-page: https://github.com/HobnobMancer/saintBioutils
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics python
 Platform: Posix
```

### Comparing `saintBioutils-0.0.8/setup.py` & `saintBioutils-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="saintBioutils",
-    version="0.0.8",
+    version="0.0.9",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A package of utility and miscellaneous functions for using in bioinformatics"
```

