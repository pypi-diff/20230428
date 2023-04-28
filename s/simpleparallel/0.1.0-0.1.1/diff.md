# Comparing `tmp/simpleparallel-0.1.0.tar.gz` & `tmp/simpleparallel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleparallel-0.1.0.tar", max compression
+gzip compressed data, was "simpleparallel-0.1.1.tar", max compression
```

## Comparing `simpleparallel-0.1.0.tar` & `simpleparallel-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      352 2023-04-28 18:00:48.955887 simpleparallel-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 18:05:17.108822 simpleparallel-0.1.0/simpleparallel/__init__.py
--rw-r--r--   0        0        0     1323 2023-04-28 18:03:57.344533 simpleparallel-0.1.0/simpleparallel/main.py
--rw-r--r--   0        0        0      641 2023-04-28 18:06:44.086347 simpleparallel-0.1.0/setup.py
--rw-r--r--   0        0        0      382 2023-04-28 18:06:44.086578 simpleparallel-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      352 2023-04-28 18:21:44.631952 simpleparallel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-28 18:20:26.066089 simpleparallel-0.1.1/simpleparallel/__init__.py
+-rw-r--r--   0        0        0     1323 2023-04-28 18:03:57.344533 simpleparallel-0.1.1/simpleparallel/main.py
+-rw-r--r--   0        0        0      641 2023-04-28 18:21:53.968259 simpleparallel-0.1.1/setup.py
+-rw-r--r--   0        0        0      382 2023-04-28 18:21:53.968510 simpleparallel-0.1.1/PKG-INFO
```

### Comparing `simpleparallel-0.1.0/simpleparallel/main.py` & `simpleparallel-0.1.1/simpleparallel/main.py`

 * *Files identical despite different names*

### Comparing `simpleparallel-0.1.0/setup.py` & `simpleparallel-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'simpleparallel',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A simple library for running parallel processes',
     'long_description': None,
     'author': 'ericaleman',
     'author_email': 'mail@ericaleman.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

