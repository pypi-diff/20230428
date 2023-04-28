# Comparing `tmp/scorpionsql-0.0.4.tar.gz` & `tmp/scorpionsql-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scorpionsql-0.0.4.tar", last modified: Mon Jul 21 16:01:21 2014, max compression
+gzip compressed data, was "dist/scorpionsql-0.0.5.tar", last modified: Fri Apr 28 16:38:04 2023, max compression
```

## Comparing `scorpionsql-0.0.4.tar` & `scorpionsql-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 sirrice    (502) staff       (20)        0 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/
--rw-r--r--   0 sirrice    (502) staff       (20)      281 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/PKG-INFO
-drwxr-xr-x   0 sirrice    (502) staff       (20)        0 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql/
--rw-r--r--   0 sirrice    (502) staff       (20)       21 2014-07-21 16:01:09.000000 scorpionsql-0.0.4/scorpionsql/__init__.py
--rw-r--r--   0 sirrice    (502) staff       (20)     1797 2014-06-19 18:40:07.000000 scorpionsql-0.0.4/scorpionsql/aggerror.py
--rwxr-xr-x   0 sirrice    (502) staff       (20)     2428 2014-06-19 18:37:01.000000 scorpionsql-0.0.4/scorpionsql/db.py
--rw-r--r--   0 sirrice    (502) staff       (20)    10590 2014-06-23 21:00:53.000000 scorpionsql-0.0.4/scorpionsql/errfunc.py
--rw-r--r--   0 sirrice    (502) staff       (20)     8681 2014-06-20 16:24:20.000000 scorpionsql-0.0.4/scorpionsql/functions.py
--rw-r--r--   0 sirrice    (502) staff       (20)       36 2014-06-19 18:37:11.000000 scorpionsql-0.0.4/scorpionsql/settings.py
--rw-r--r--   0 sirrice    (502) staff       (20)     8175 2014-06-19 18:38:12.000000 scorpionsql-0.0.4/scorpionsql/sql.py
--rw-r--r--   0 sirrice    (502) staff       (20)     5080 2014-07-17 19:34:39.000000 scorpionsql-0.0.4/scorpionsql/sqlparser.py
-drwxr-xr-x   0 sirrice    (502) staff       (20)        0 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/
--rw-r--r--   0 sirrice    (502) staff       (20)        1 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/dependency_links.txt
--rw-r--r--   0 sirrice    (502) staff       (20)      281 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/PKG-INFO
--rw-r--r--   0 sirrice    (502) staff       (20)       35 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/requires.txt
--rw-r--r--   0 sirrice    (502) staff       (20)      374 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/SOURCES.txt
--rw-r--r--   0 sirrice    (502) staff       (20)       12 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/scorpionsql.egg-info/top_level.txt
--rw-r--r--   0 sirrice    (502) staff       (20)      100 2014-07-21 16:01:21.000000 scorpionsql-0.0.4/setup.cfg
--rwxr-xr-x   0 sirrice    (502) staff       (20)      850 2014-07-21 16:01:01.000000 scorpionsql-0.0.4/setup.py
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.622840 scorpionsql-0.0.5/
+-rw-r--r--   0 eugenewu   (502) staff       (20)     1054 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/LICENSE
+-rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:38:04.622899 scorpionsql-0.0.5/PKG-INFO
+-rw-r--r--   0 eugenewu   (502) staff       (20)      132 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/README.md
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.621984 scorpionsql-0.0.5/scorpionsql/
+-rw-r--r--   0 eugenewu   (502) staff       (20)       22 2023-04-28 16:34:11.000000 scorpionsql-0.0.5/scorpionsql/__init__.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     1797 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/aggerror.py
+-rwxr-xr-x   0 eugenewu   (502) staff       (20)     2428 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/db.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)    10590 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/errfunc.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     8681 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/functions.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)       36 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/settings.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     8175 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/sql.py
+-rw-r--r--   0 eugenewu   (502) staff       (20)     5080 2023-04-28 16:31:36.000000 scorpionsql-0.0.5/scorpionsql/sqlparser.py
+drwxr-xr-x   0 eugenewu   (502) staff       (20)        0 2023-04-28 16:38:04.622721 scorpionsql-0.0.5/scorpionsql.egg-info/
+-rw-r--r--   0 eugenewu   (502) staff       (20)      264 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/PKG-INFO
+-rw-r--r--   0 eugenewu   (502) staff       (20)      392 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/SOURCES.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)        1 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/dependency_links.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       43 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/requires.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       12 2023-04-28 16:38:04.000000 scorpionsql-0.0.5/scorpionsql.egg-info/top_level.txt
+-rw-r--r--   0 eugenewu   (502) staff       (20)       79 2023-04-28 16:38:04.623205 scorpionsql-0.0.5/setup.cfg
+-rwxr-xr-x   0 eugenewu   (502) staff       (20)      857 2023-04-28 16:33:46.000000 scorpionsql-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scorpionsql-0.0.4/scorpionsql/aggerror.py` & `scorpionsql-0.0.5/scorpionsql/aggerror.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/scorpionsql/db.py` & `scorpionsql-0.0.5/scorpionsql/db.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/scorpionsql/errfunc.py` & `scorpionsql-0.0.5/scorpionsql/errfunc.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/scorpionsql/functions.py` & `scorpionsql-0.0.5/scorpionsql/functions.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/scorpionsql/sql.py` & `scorpionsql-0.0.5/scorpionsql/sql.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/scorpionsql/sqlparser.py` & `scorpionsql-0.0.5/scorpionsql/sqlparser.py`

 * *Files identical despite different names*

### Comparing `scorpionsql-0.0.4/setup.py` & `scorpionsql-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,10 +21,10 @@
     package_data = {
       'scorpion': [
         'jars/scala-library.jar',
         'jars/sqlparser.jar'
       ]
     },
     install_requires = [
-      'psycopg2', 'sqlalchemy', 'numpy', 'pyparsing'
+      'psycopg2-binary', 'sqlalchemy', 'numpy', 'pyparsing'
     ],
     keywords= "")
```

