# Comparing `tmp/ICICONSOLE-0.0.3.tar.gz` & `tmp/ICICONSOLE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.3.tar", last modified: Sun Apr 23 23:04:03 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.4.tar", last modified: Thu Apr 27 22:39:31 2023, max compression
```

## Comparing `ICICONSOLE-0.0.3.tar` & `ICICONSOLE-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-23 23:04:03.009758 ICICONSOLE-0.0.3/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-23 23:04:03.008293 ICICONSOLE-0.0.3/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.3/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9045 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.3/ICICONSOLE/ICICONSOLE.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.3/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)      141 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.3/ICICONSOLE/__main__.py
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-23 23:04:03.009384 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      343 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       56 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-04-23 23:04:03.000000 ICICONSOLE-0.0.3/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.3/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-23 23:04:03.009606 ICICONSOLE-0.0.3/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1728 2023-04-21 16:27:23.000000 ICICONSOLE-0.0.3/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1012 2023-04-23 23:03:24.000000 ICICONSOLE-0.0.3/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-04-23 23:04:03.009793 ICICONSOLE-0.0.3/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.356252 ICICONSOLE-0.0.4/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.354885 ICICONSOLE-0.0.4/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     9045 2023-04-27 22:38:06.000000 ICICONSOLE-0.0.4/ICICONSOLE/__main__.py
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.355879 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-27 22:39:31.356100 ICICONSOLE-0.0.4/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1728 2023-04-21 16:27:23.000000 ICICONSOLE-0.0.4/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-04-27 22:38:31.000000 ICICONSOLE-0.0.4/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-04-27 22:39:31.356291 ICICONSOLE-0.0.4/setup.cfg
```

### Comparing `ICICONSOLE-0.0.3/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.4/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.3/ICICONSOLE/ICICONSOLE.py` & `ICICONSOLE-0.0.4/ICICONSOLE/__main__.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.3/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.4/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/ICICONSOLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC,Neo4j
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ICICONSOLE-0.0.3/LICENSE` & `ICICONSOLE-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.3/PKG-INFO` & `ICICONSOLE-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.3
+Version: 0.0.4
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/ICICONSOLE
+Project-URL: Homepage, https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE
 Keywords: Tapis,CLI,Agave,HPC,Tapis Pods,TACC,Neo4j
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ICICONSOLE-0.0.3/README.md` & `ICICONSOLE-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.3/pyproject.toml` & `ICICONSOLE-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.3"
+version = "0.0.4"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -24,11 +24,11 @@
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
-Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_04_2023/CLI/ICICONSOLE"
+Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE"
 
-[project.entry-points."TapisCLICICLE.__main__"]
+[project.entry-points."ICICONSOLE.__main__"]
 tomatoes = "ICICONSOLE:__main__"
```

