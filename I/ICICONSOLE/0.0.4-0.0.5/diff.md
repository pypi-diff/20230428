# Comparing `tmp/ICICONSOLE-0.0.4.tar.gz` & `tmp/ICICONSOLE-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ICICONSOLE-0.0.4.tar", last modified: Thu Apr 27 22:39:31 2023, max compression
+gzip compressed data, was "ICICONSOLE-0.0.5.tar", last modified: Thu Apr 27 22:53:25 2023, max compression
```

## Comparing `ICICONSOLE-0.0.4.tar` & `ICICONSOLE-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.356252 ICICONSOLE-0.0.4/
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.354885 ICICONSOLE-0.0.4/ICICONSOLE/
--rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/ICICONSOLE/BasicCypherCommands.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/ICICONSOLE/__init__.py
--rw-r--r--   0 sahilsamar   (501) staff       (20)     9045 2023-04-27 22:38:06.000000 ICICONSOLE-0.0.4/ICICONSOLE/__main__.py
-drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:39:31.355879 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/
--rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/SOURCES.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/dependency_links.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/entry_points.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/requires.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-04-27 22:39:31.000000 ICICONSOLE-0.0.4/ICICONSOLE.egg-info/top_level.txt
--rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.4/LICENSE
--rw-r--r--   0 sahilsamar   (501) staff       (20)    42960 2023-04-27 22:39:31.356100 ICICONSOLE-0.0.4/PKG-INFO
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1728 2023-04-21 16:27:23.000000 ICICONSOLE-0.0.4/README.md
--rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-04-27 22:38:31.000000 ICICONSOLE-0.0.4/pyproject.toml
--rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-04-27 22:39:31.356291 ICICONSOLE-0.0.4/setup.cfg
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.051113 ICICONSOLE-0.0.5/
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.049755 ICICONSOLE-0.0.5/ICICONSOLE/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      882 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/ICICONSOLE/BasicCypherCommands.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        0 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/ICICONSOLE/__init__.py
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     9045 2023-04-27 22:38:06.000000 ICICONSOLE-0.0.5/ICICONSOLE/__main__.py
+drwxr-xr-x   0 sahilsamar   (501) staff       (20)        0 2023-04-27 22:53:25.050741 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)      318 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/SOURCES.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)        1 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/dependency_links.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       53 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/entry_points.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       28 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/requires.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       11 2023-04-27 22:53:25.000000 ICICONSOLE-0.0.5/ICICONSOLE.egg-info/top_level.txt
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    35149 2023-04-23 22:20:18.000000 ICICONSOLE-0.0.5/LICENSE
+-rw-r--r--   0 sahilsamar   (501) staff       (20)    43040 2023-04-27 22:53:25.050963 ICICONSOLE-0.0.5/PKG-INFO
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1808 2023-04-27 22:52:49.000000 ICICONSOLE-0.0.5/README.md
+-rw-r--r--   0 sahilsamar   (501) staff       (20)     1009 2023-04-27 22:51:50.000000 ICICONSOLE-0.0.5/pyproject.toml
+-rw-r--r--   0 sahilsamar   (501) staff       (20)       38 2023-04-27 22:53:25.051151 ICICONSOLE-0.0.5/setup.cfg
```

### Comparing `ICICONSOLE-0.0.4/ICICONSOLE/BasicCypherCommands.py` & `ICICONSOLE-0.0.5/ICICONSOLE/BasicCypherCommands.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.4/ICICONSOLE/__main__.py` & `ICICONSOLE-0.0.5/ICICONSOLE/__main__.py`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.4/ICICONSOLE.egg-info/PKG-INFO` & `ICICONSOLE-0.0.5/ICICONSOLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,21 @@
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
 ### Installation
 
-Right now, the only way to use this application is to directly run the python code. Additionally, it requies python 3.10.
+Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
+
+```shell 
+pip install ICICONSOLE
+```
+
+**OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
 cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
```

### Comparing `ICICONSOLE-0.0.4/LICENSE` & `ICICONSOLE-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ICICONSOLE-0.0.4/PKG-INFO` & `ICICONSOLE-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ICICONSOLE
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods.
 Author-email: Sahil Samar <sahilsamar031@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,21 @@
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
 ### Installation
 
-Right now, the only way to use this application is to directly run the python code. Additionally, it requies python 3.10.
+Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
+
+```shell 
+pip install ICICONSOLE
+```
+
+**OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
 cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
```

### Comparing `ICICONSOLE-0.0.4/README.md` & `ICICONSOLE-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 ICICONSOLE is designed to provide an efficient and powerful interface to Neo4j Knowledge Graph databases hosted on HPC resources, leveraging Tapis. 
 
 This application is specialized for knowledge graph querying, and has some basic CYPHER commands built in. 
 
 ### Installation
 
-Right now, the only way to use this application is to directly run the python code. Additionally, it requies python 3.10.
+Requires Python 3.10 or higher. You can clone this repository and manually install the requirements, or you can directly install the application from PyPi.
+
+```shell 
+pip install ICICONSOLE
+```
+
+**OR**
 
 ```shell 
 git clone https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients.git
 ```
 
 ```shell
 cd hello_icicle_auth_clients/icicle_rel_03_2023/CLI/ICICONSOLE
```

### Comparing `ICICONSOLE-0.0.4/pyproject.toml` & `ICICONSOLE-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ICICONSOLE"
-version = "0.0.4"
+version = "0.0.5"
 description = "Command-line Interface tailored to working with Neo4j Knowledge Graph Databses hosted through via Tapis Pods."
 readme = "README.md"
 authors = [{ name = "Sahil Samar", email = "sahilsamar031@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

