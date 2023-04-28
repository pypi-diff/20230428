# Comparing `tmp/skosprovider_sqlalchemy-2.1.0.tar.gz` & `tmp/skosprovider_sqlalchemy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skosprovider_sqlalchemy-2.1.0.tar", last modified: Thu Mar 30 18:56:51 2023, max compression
+gzip compressed data, was "skosprovider_sqlalchemy-2.1.1.tar", last modified: Fri Apr 28 20:05:34 2023, max compression
```

## Comparing `skosprovider_sqlalchemy-2.1.0.tar` & `skosprovider_sqlalchemy-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-03-30 18:56:51.182801 skosprovider_sqlalchemy-2.1.0/
--rw-rw-r--   0 koen      (1001) koen      (1001)     9519 2023-03-30 18:50:09.000000 skosprovider_sqlalchemy-2.1.0/HISTORY.rst
--rw-rw-r--   0 koen      (1001) koen      (1001)     1073 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.0/LICENSE
--rw-rw-r--   0 koen      (1001) koen      (1001)       39 2022-12-15 08:43:42.000000 skosprovider_sqlalchemy-2.1.0/MANIFEST.in
--rw-rw-r--   0 koen      (1001) koen      (1001)     2571 2023-03-30 18:56:51.182801 skosprovider_sqlalchemy-2.1.0/PKG-INFO
--rw-rw-r--   0 koen      (1001) koen      (1001)     1787 2023-01-19 19:39:22.000000 skosprovider_sqlalchemy-2.1.0/README.rst
--rw-rw-r--   0 koen      (1001) koen      (1001)       38 2023-03-30 18:56:51.182801 skosprovider_sqlalchemy-2.1.0/setup.cfg
--rwxrwxr-x   0 koen      (1001) koen      (1001)     1480 2023-03-30 18:50:33.000000 skosprovider_sqlalchemy-2.1.0/setup.py
-drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-03-30 18:56:51.182801 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/
--rw-rw-r--   0 koen      (1001) koen      (1001)        0 2022-12-15 08:43:42.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/__init__.py
--rw-rw-r--   0 koen      (1001) koen      (1001)    19422 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/models.py
--rw-rw-r--   0 koen      (1001) koen      (1001)    18988 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/providers.py
--rw-rw-r--   0 koen      (1001) koen      (1001)    11944 2023-03-30 18:47:54.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/utils.py
-drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-03-30 18:56:51.182801 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/
--rw-rw-r--   0 koen      (1001) koen      (1001)     2571 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/PKG-INFO
--rw-rw-r--   0 koen      (1001) koen      (1001)      521 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/SOURCES.txt
--rw-rw-r--   0 koen      (1001) koen      (1001)        1 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/dependency_links.txt
--rw-rw-r--   0 koen      (1001) koen      (1001)      170 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/entry_points.txt
--rw-rw-r--   0 koen      (1001) koen      (1001)        1 2023-01-19 17:32:37.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/not-zip-safe
--rw-rw-r--   0 koen      (1001) koen      (1001)       31 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/requires.txt
--rw-rw-r--   0 koen      (1001) koen      (1001)       24 2023-03-30 18:56:51.000000 skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/top_level.txt
+drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-04-28 20:05:34.095872 skosprovider_sqlalchemy-2.1.1/
+-rw-rw-r--   0 koen      (1001) koen      (1001)     9625 2023-04-28 20:04:33.000000 skosprovider_sqlalchemy-2.1.1/HISTORY.rst
+-rw-rw-r--   0 koen      (1001) koen      (1001)     1073 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.1/LICENSE
+-rw-rw-r--   0 koen      (1001) koen      (1001)       39 2022-12-15 08:43:42.000000 skosprovider_sqlalchemy-2.1.1/MANIFEST.in
+-rw-rw-r--   0 koen      (1001) koen      (1001)     2551 2023-04-28 20:05:34.095872 skosprovider_sqlalchemy-2.1.1/PKG-INFO
+-rw-rw-r--   0 koen      (1001) koen      (1001)     1787 2023-01-19 19:39:22.000000 skosprovider_sqlalchemy-2.1.1/README.rst
+-rw-rw-r--   0 koen      (1001) koen      (1001)       38 2023-04-28 20:05:34.095872 skosprovider_sqlalchemy-2.1.1/setup.cfg
+-rwxrwxr-x   0 koen      (1001) koen      (1001)     1480 2023-04-28 20:04:33.000000 skosprovider_sqlalchemy-2.1.1/setup.py
+drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-04-28 20:05:34.091873 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/
+-rw-rw-r--   0 koen      (1001) koen      (1001)        0 2022-12-15 08:43:42.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/__init__.py
+-rw-rw-r--   0 koen      (1001) koen      (1001)    19422 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/models.py
+-rw-rw-r--   0 koen      (1001) koen      (1001)    18988 2023-01-19 17:54:19.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/providers.py
+-rw-rw-r--   0 koen      (1001) koen      (1001)    11954 2023-04-28 20:04:33.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/utils.py
+drwxrwxr-x   0 koen      (1001) koen      (1001)        0 2023-04-28 20:05:34.095872 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/
+-rw-rw-r--   0 koen      (1001) koen      (1001)     2551 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/PKG-INFO
+-rw-rw-r--   0 koen      (1001) koen      (1001)      521 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/SOURCES.txt
+-rw-rw-r--   0 koen      (1001) koen      (1001)        1 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/dependency_links.txt
+-rw-rw-r--   0 koen      (1001) koen      (1001)      154 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/entry_points.txt
+-rw-rw-r--   0 koen      (1001) koen      (1001)        1 2023-01-19 17:32:37.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/not-zip-safe
+-rw-rw-r--   0 koen      (1001) koen      (1001)       31 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/requires.txt
+-rw-rw-r--   0 koen      (1001) koen      (1001)       24 2023-04-28 20:05:34.000000 skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/top_level.txt
```

### Comparing `skosprovider_sqlalchemy-2.1.0/HISTORY.rst` & `skosprovider_sqlalchemy-2.1.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.1.1 (2023-04-28)
+------------------
+
+* Fixed an issue with casting ids to string during import. (#104)
+
 2.1.0 (2023-03-30)
 ------------------
 
 * **Minor BC break**: Changed the order of parameters to the import_provider 
   function and make the conceptscheme argument optional. (#100)
 
 2.0.1 (2023-03-20)
```

### Comparing `skosprovider_sqlalchemy-2.1.0/LICENSE` & `skosprovider_sqlalchemy-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skosprovider_sqlalchemy-2.1.0/PKG-INFO` & `skosprovider_sqlalchemy-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: skosprovider_sqlalchemy
-Version: 2.1.0
+Version: 2.1.1
 Summary: A sqlAlchemy implementation of skosprovider.
 Home-page: https://github.com/OnroerendErfgoed/skosprovider_sqlalchemy
 Author: Koen Van Daele
 Author-email: koen_van_daele@telenet.be
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -61,9 +60,7 @@
 
     # activate your virtual env
     $ pip install -r requirements-dev.txt
     $ cd docs
     $ make html
 
 .. _skosprovider: https://github.com/koenedaele/skosprovider
-
-
```

### Comparing `skosprovider_sqlalchemy-2.1.0/README.rst` & `skosprovider_sqlalchemy-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `skosprovider_sqlalchemy-2.1.0/setup.py` & `skosprovider_sqlalchemy-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires = [
     'skosprovider>=1.2.0',
     'sqlalchemy',
 ]
 
 setup(
     name='skosprovider_sqlalchemy',
-    version='2.1.0',
+    version='2.1.1',
     description='A sqlAlchemy implementation of skosprovider.',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     author='Koen Van Daele',
     author_email='koen_van_daele@telenet.be',
     url='https://github.com/OnroerendErfgoed/skosprovider_sqlalchemy',
     packages=packages,
```

### Comparing `skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/models.py` & `skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/providers.py` & `skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/providers.py`

 * *Files identical despite different names*

### Comparing `skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy/utils.py` & `skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,21 +63,21 @@
 
     # First pass: load all concepts and collections
     for stuff in provider.get_all():
         c = provider.get_by_id(stuff['id'])
         log.warning(c)
         if isinstance(c, Concept):
             cm = ConceptModel(
-                concept_id=c.id,
+                concept_id=str(c.id),
                 uri=c.uri,
                 conceptscheme=conceptscheme
             )
         elif isinstance(c, Collection):
             cm = CollectionModel(
-                concept_id=c.id,
+                concept_id=str(c.id),
                 uri=c.uri,
                 conceptscheme=conceptscheme
             )
         session.add(cm)
         _add_labels(cm, c.labels, session)
         _add_notes(cm, c.notes, session)
         _add_sources(cm, c.sources, session)
```

### Comparing `skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/PKG-INFO` & `skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: skosprovider-sqlalchemy
-Version: 2.1.0
+Version: 2.1.1
 Summary: A sqlAlchemy implementation of skosprovider.
 Home-page: https://github.com/OnroerendErfgoed/skosprovider_sqlalchemy
 Author: Koen Van Daele
 Author-email: koen_van_daele@telenet.be
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -61,9 +60,7 @@
 
     # activate your virtual env
     $ pip install -r requirements-dev.txt
     $ cd docs
     $ make html
 
 .. _skosprovider: https://github.com/koenedaele/skosprovider
-
-
```

### Comparing `skosprovider_sqlalchemy-2.1.0/skosprovider_sqlalchemy.egg-info/SOURCES.txt` & `skosprovider_sqlalchemy-2.1.1/skosprovider_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

