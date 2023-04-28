# Comparing `tmp/CharacterAPI-0.1.0.tar.gz` & `tmp/CharacterAPI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CharacterAPI-0.1.0.tar", last modified: Fri Apr 28 17:31:01 2023, max compression
+gzip compressed data, was "dist\CharacterAPI-0.1.1.tar", last modified: Fri Apr 28 18:35:57 2023, max compression
```

## Comparing `CharacterAPI-0.1.0.tar` & `CharacterAPI-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 17:31:01.346704 CharacterAPI-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-28 17:31:01.255698 CharacterAPI-0.1.0/CharacterAPI/
--rw-rw-rw-   0        0        0     4457 2023-04-28 17:13:01.000000 CharacterAPI-0.1.0/CharacterAPI/CharacterAI.py
--rw-rw-rw-   0        0        0     4850 2023-04-28 17:25:33.000000 CharacterAPI-0.1.0/CharacterAPI/CharacterAI_async.py
--rw-rw-rw-   0        0        0       66 2023-04-28 17:03:21.000000 CharacterAPI-0.1.0/CharacterAPI/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.0/CharacterAPI/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:31:01.341707 CharacterAPI-0.1.0/CharacterAPI.egg-info/
--rw-rw-rw-   0        0        0      457 2023-04-28 17:31:00.000000 CharacterAPI-0.1.0/CharacterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-28 17:31:00.000000 CharacterAPI-0.1.0/CharacterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:31:00.000000 CharacterAPI-0.1.0/CharacterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-28 17:31:00.000000 CharacterAPI-0.1.0/CharacterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 17:31:00.000000 CharacterAPI-0.1.0/CharacterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      457 2023-04-28 17:31:01.345705 CharacterAPI-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 17:31:01.348836 CharacterAPI-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-04-28 17:27:01.000000 CharacterAPI-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.827737 CharacterAPI-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.711878 CharacterAPI-0.1.1/CharacterAPI/
+-rw-rw-rw-   0        0        0     4457 2023-04-28 17:13:01.000000 CharacterAPI-0.1.1/CharacterAPI/CharacterAI.py
+-rw-rw-rw-   0        0        0     4850 2023-04-28 17:25:33.000000 CharacterAPI-0.1.1/CharacterAPI/CharacterAI_async.py
+-rw-rw-rw-   0        0        0       66 2023-04-28 17:03:21.000000 CharacterAPI-0.1.1/CharacterAPI/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.1/CharacterAPI/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-28 18:35:57.811732 CharacterAPI-0.1.1/CharacterAPI.egg-info/
+-rw-rw-rw-   0        0        0      457 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 18:35:57.000000 CharacterAPI-0.1.1/CharacterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      457 2023-04-28 18:35:57.819735 CharacterAPI-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:35:57.827737 CharacterAPI-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-28 18:35:17.000000 CharacterAPI-0.1.1/setup.py
```

### Comparing `CharacterAPI-0.1.0/CharacterAPI/CharacterAI.py` & `CharacterAPI-0.1.1/CharacterAPI/CharacterAI.py`

 * *Files identical despite different names*

### Comparing `CharacterAPI-0.1.0/CharacterAPI/CharacterAI_async.py` & `CharacterAPI-0.1.1/CharacterAPI/CharacterAI_async.py`

 * *Files identical despite different names*

### Comparing `CharacterAPI-0.1.0/LICENSE` & `CharacterAPI-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CharacterAPI-0.1.0/setup.py` & `CharacterAPI-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='CharacterAPI',
-    version='0.1.0',
+    version='0.1.1',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/CharacterAPI',
-    packages=['CharacterAPI'],
-    install_requires=open('requirements.txt').read().strip().split('\n'),
+    packages=find_packages(),
+    install_requires=["playwright==1.32.1"],
     classifiers=[
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
     ],
 )
```

