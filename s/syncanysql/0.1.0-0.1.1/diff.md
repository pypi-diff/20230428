# Comparing `tmp/syncanysql-0.1.0.tar.gz` & `tmp/syncanysql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.0.tar", last modified: Tue Apr 25 10:06:27 2023, max compression
+gzip compressed data, was "syncanysql-0.1.1.tar", last modified: Fri Apr 28 09:59:56 2023, max compression
```

## Comparing `syncanysql-0.1.0.tar` & `syncanysql-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.902526 syncanysql-0.1.0/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-25 10:06:27.903523 syncanysql-0.1.0/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2955 2023-04-20 10:10:41.000000 syncanysql-0.1.0/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-25 10:06:27.912524 syncanysql-0.1.0/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-25 10:05:48.000000 syncanysql-0.1.0/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:26.678746 syncanysql-0.1.0/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9128 2023-04-25 02:06:38.000000 syncanysql-0.1.0/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.078749 syncanysql-0.1.0/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.0/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.0/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.379523 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   125161 2023-04-25 03:25:46.000000 syncanysql-0.1.0/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12017 2023-04-21 07:43:33.000000 syncanysql-0.1.0/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.0/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7641 2023-04-25 01:49:10.000000 syncanysql-0.1.0/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3709 2023-04-24 02:09:57.000000 syncanysql-0.1.0/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.0/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.1.0/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.858524 syncanysql-0.1.0/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.0/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.0/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.0/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1126 2023-04-24 01:38:19.000000 syncanysql-0.1.0/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3796 2023-04-25 09:19:43.000000 syncanysql-0.1.0/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.1.0/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.0/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.0/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.0/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.0/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-21 10:34:47.000000 syncanysql-0.1.0/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:26.940746 syncanysql-0.1.0/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-04-25 10:06:26.000000 syncanysql-0.1.0/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:56.588028 syncanysql-0.1.1/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-04-28 09:59:56.589055 syncanysql-0.1.1/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.1/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-28 09:59:56.600409 syncanysql-0.1.1/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-26 02:14:48.000000 syncanysql-0.1.1/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.221394 syncanysql-0.1.1/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.1/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.648537 syncanysql-0.1.1/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.1/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.1/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.985804 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   125599 2023-04-28 09:46:36.000000 syncanysql-0.1.1/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-04-27 09:12:49.000000 syncanysql-0.1.1/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.1/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7755 2023-04-27 09:10:45.000000 syncanysql-0.1.1/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.1/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.1/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.1/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:56.539127 syncanysql-0.1.1/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.1/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.1/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.1/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.1/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.1/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19398 2023-04-28 03:15:43.000000 syncanysql-0.1.1/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.1/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.1/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.1/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.1/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-26 02:14:48.000000 syncanysql-0.1.1/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:55.486511 syncanysql-0.1.1/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.1/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-28 09:59:54.000000 syncanysql-0.1.1/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.0/PKG-INFO` & `syncanysql-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -28,18 +28,24 @@
         - [特性与限制](docs/feature-restrictions.md)
         - [配置详解](docs/configure.md)
         - [驱动依赖](docs/driver-dependency.md)
         - [示例详解](examples)
         
         ## 安装
         
-        ```
+        ```bash
         pip3 install syncanysql
         ```
         
+        #### Docker
+        
+        ```bash
+        docker pull sujin190/syncany-sql
+        ```
+        
         ## 查询Nginx日志
         
         ```sql
         -- 查询访问量最高的三个IP
         SELECT seg0 AS ip, COUNT(*) AS cnt FROM `file://data/access.log?sep= ` GROUP BY seg0 ORDER BY cnt DESC LIMIT 3;
         ```
```

### Comparing `syncanysql-0.1.0/README.md` & `syncanysql-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,24 @@
 - [特性与限制](docs/feature-restrictions.md)
 - [配置详解](docs/configure.md)
 - [驱动依赖](docs/driver-dependency.md)
 - [示例详解](examples)
 
 ## 安装
 
-```
+```bash
 pip3 install syncanysql
 ```
 
+#### Docker
+
+```bash
+docker pull sujin190/syncany-sql
+```
+
 ## 查询Nginx日志
 
 ```sql
 -- 查询访问量最高的三个IP
 SELECT seg0 AS ip, COUNT(*) AS cnt FROM `file://data/access.log?sep= ` GROUP BY seg0 ORDER BY cnt DESC LIMIT 3;
 ```
```

### Comparing `syncanysql-0.1.0/setup.py` & `syncanysql-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.0"
+version = "0.1.1"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.6",
+        "syncany>=0.2.7",
         'Pygments>=2.14.0',
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.1.0/syncanysql/__init__.py` & `syncanysql-0.1.1/syncanysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         self.executor = None
 
     def setup(self):
         if self.manager is not None:
             return
         init_execute_files = self.config.load()
         self.config.config_logging()
+        self.config.load_extensions()
         self.manager = TaskerManager(DatabaseManager())
         self.executor = Executor(self.manager, self.config.session())
         if init_execute_files:
             self.executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in
                                        range(len(init_execute_files))])
             with self.executor as executor:
                 exit_code = executor.execute()
```

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.1/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.1/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.1/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.1/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/compiler.py` & `syncanysql-0.1.1/syncanysql/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 
 import sqlglot.expressions
 from sqlglot import maybe_parse, ParseError
 from sqlglot import expressions as sqlglot_expressions
 from sqlglot.dialects import Dialect
 from sqlglot import tokens
+from syncany.taskers.core import CoreTasker
 from .errors import SyncanySqlCompileException
 from .calculaters import is_mysql_func, find_aggregate_calculater, CalculaterUnknownException
 from .config import CONST_CONFIG_KEYS
 from .parser import SqlParser
 from .taskers.delete import DeleteTasker
 from .taskers.query import QueryTasker, DEAULT_AGGREGATE
 from .taskers.into import IntoTasker
@@ -80,23 +81,24 @@
             error_sql = "\n".join(sql_lines)
             raise ParseError('syntax error "%s" near "%s"' % (error_info["description"], error_sql), [error_info]) from None
 
     def compile_expression(self, expression, arguments):
         if isinstance(expression, sqlglot_expressions.Delete):
             return DeleteTasker(self.compile_delete(expression, arguments))
         elif isinstance(expression, (sqlglot_expressions.Union, sqlglot_expressions.Insert, sqlglot_expressions.Select)):
-            query_tasker = QueryTasker(self.compile_query(expression, arguments))
+            query_tasker = QueryTasker(self.compile_query(expression, arguments), expression)
             if not expression.args.get("into"):
                 return query_tasker
             if not isinstance(expression, sqlglot_expressions.Select):
                 raise SyncanySqlCompileException('unknown into, related sql "%s"' % self.to_sql(expression))
             return IntoTasker(query_tasker, self.compile_select_into(expression.args.get("into"), arguments))
         elif isinstance(expression, sqlglot_expressions.Command):
             if expression.args["this"].lower() == "explain" and self.is_const(expression.args["expression"], {}, arguments):
-                return ExplainTasker(self.compile(self.parse_const(expression.args["expression"], {}, arguments)["value"], arguments))
+                return ExplainTasker(self.compile(self.parse_const(expression.args["expression"], {}, arguments)["value"],
+                                                  arguments), self.to_sql(expression.args["expression"]))
             if expression.args["this"].lower() == "set" and (isinstance(expression.args["expression"], str)
                                                              or self.is_const(expression.args["expression"], {}, arguments)):
                 if isinstance(expression.args["expression"], str):
                     value = expression.args["expression"].split("=")
                 else:
                     value = self.parse_const(expression.args["expression"], {}, arguments)["value"].split("=")
                 config = {"key": value[0].strip(), "value": "=".join(value[1:]).strip()}
@@ -120,34 +122,34 @@
             if isinstance(set_item_expression, sqlglot_expressions.SetItem) and isinstance(set_item_expression.args["this"], sqlglot_expressions.EQ):
                 value = str(set_item_expression).split("=")
                 config = {"key": value[0].strip(), "value": "=".join(value[1:]).strip()}
                 return SetCommandTasker(config)
         raise SyncanySqlCompileException('unknown sql "%s"' % self.to_sql(expression))
 
     def compile_delete(self, expression, arguments):
-        config = copy.deepcopy(self.config)
+        config = {key: copy.deepcopy(self.config.get(key)) for key in CoreTasker.DEFAULT_CONFIG}
         config.update({
             "input": "&.--.--::id",
             "loader": "const_loader",
-            "loader_arguments":  {"datas": [{}]},
+            "loader_arguments":  {"datas": []},
             "output": "&.-.&1::id",
             "querys": {},
             "schema": "$.*",
         })
 
         table_info = self.parse_table(expression.args["this"], config, arguments)
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
             self.compile_where_condition(where_expression.args["this"], config, arguments, table_info)
             self.parse_condition_typing_filter(expression, config, arguments)
         config["output"] = "".join(["&.", table_info["db"], ".", table_info["name"], "::id use DI"])
         return config
 
     def compile_query(self, expression, arguments):
-        config = copy.deepcopy(self.config)
+        config = {key: copy.deepcopy(self.config.get(key)) for key in CoreTasker.DEFAULT_CONFIG}
         config.update({
             "input": "&.-.&1::id",
             "output": "&.-.&1::id",
             "querys": {},
             "schema": "$.*",
             "intercepts": [],
             "orders": [],
@@ -1027,17 +1029,18 @@
                                                              column_join_tables, join_index))
                 return column
 
             if calculater_name not in ("add", "sub", "mul", "div", "mod") and is_mysql_func(calculater_name):
                 column = ["@mysql::" + calculater_name]
             else:
                 if calculater_name[:8] == "convert_":
-                    column = ["@" + "::".join(calculater_name.split("$")) + "|" + calculater_name[8:]]
+                    column = ["@" + calculater_name + "|" + calculater_name[8:]]
                 else:
-                    column = ["@" + "::".join(calculater_name.split("$"))]
+                    calculater_modules = calculater_name.split("$")
+                    column = ["@" + calculater_modules[0] + (("::" + ".".join(calculater_modules[1:])) if len(calculater_modules) >= 2 else "")]
             for arg_expression in expression.args.get("expressions", []):
                 if self.is_const(arg_expression, config, arguments):
                     column.append(self.compile_const(arg_expression, config, arguments,
                                                      self.parse_const(arg_expression, config, arguments)))
                 else:
                     column.append(self.compile_calculate(arg_expression, config, arguments, primary_table, column_join_tables, join_index))
             return column
@@ -1275,15 +1278,16 @@
         else:
             raise SyncanySqlCompileException('unknown having condition, related sql "%s"' % self.to_sql(expression))
 
     def compile_order(self, expression, config, arguments, primary_table):
         primary_sort_keys, sort_keys = [], []
         for order_expression in expression:
             column = self.parse_column(order_expression.args["this"], config, arguments)
-            if (column["table_name"] and primary_table["table_alias"] == column["table_name"]) or \
+            if not isinstance(config["schema"], dict) or \
+                    (column["table_name"] and primary_table["table_alias"] == column["table_name"]) or \
                     (not column["table_name"] and column["column_name"] in primary_table["columns"]):
                 primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
             sort_keys.append((column["column_name"], True if order_expression.args["desc"] else False))
         if sort_keys and len(primary_sort_keys) < len(sort_keys):
             if isinstance(config["schema"], dict):
                 for sort_key, _ in sort_keys:
                     if sort_key not in config["schema"]:
```

### Comparing `syncanysql-0.1.0/syncanysql/config.py` & `syncanysql-0.1.1/syncanysql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # -*- coding: utf-8 -*-
 # 2023/2/8
 # create by: snower
 
 import os
-import sys
 import copy
 import re
 import uuid
 import logging.config
 import json
 import pytz
 from syncany.taskers.core import CoreTasker
 from syncany.taskers.config import load_config
+from syncany.logger import get_logger
 from syncany.utils import set_timezone
 
 
 VIRTUAL_VIEW_ARGS_RE = re.compile("(\#\{\w+?(:.*?){0,1}\})", re.DOTALL | re.M)
 CONST_CONFIG_KEYS = ("@verbose", "@timeout", "@limit", "@batch", "@streaming", "@recovery", "@join_batch",
                      "@insert_batch", "@primary_order")
 
 
 class GlobalConfig(object):
     def __init__(self):
         self.config = copy.deepcopy(CoreTasker.DEFAULT_CONFIG)
 
+    def get_home(self):
+        if "SYNCANY_HOME" in os.environ:
+            return os.path.abspath(os.environ["SYNCANY_HOME"])
+        return os.path.abspath(os.path.join(os.path.expanduser('~'), ".syncany"))
+
     def get(self):
         return self.config
 
     def set(self, key, value):
         if not isinstance(key, (list, tuple)):
             key = str(key).split(".")
         if not key:
@@ -117,17 +122,17 @@
             except:
                 default_value = default_value[1:]
             args.append([arg_info[0], exps[arg_info[1]] if len(arg_info) >= 2 else "==", default_value])
             query = query.replace(arg, '%s')
         return query, args
 
     def load(self, custom_config=None):
-        home_config_path = os.path.join(os.path.expanduser('~'), ".syncany")
-        for filename in (os.path.join(home_config_path, "config.json"), os.path.join(home_config_path, "config.yaml"),
-                         "config.json", "config.yaml"):
+        home_config_path, cwd_config_path = self.get_home(), os.path.abspath(os.getcwd())
+        for filename in {os.path.join(home_config_path, "config.json"), os.path.join(home_config_path, "config.yaml"),
+                         os.path.join(cwd_config_path, "config.json"), os.path.join(cwd_config_path, "config.yaml")}:
             if not os.path.exists(filename):
                 continue
             if "extends" not in self.config or not isinstance(self.config["extends"], list):
                 self.config["extends"] = []
             if filename not in self.config["extends"]:
                 self.config["extends"].append(filename)
         self.load_config()
@@ -181,14 +186,24 @@
         if isinstance(extends, list):
             for config_filename in extends:
                 self.load_config(config_filename)
         else:
             self.load_config(extends)
         self.merge_config(config)
 
+    def load_extensions(self):
+        extensions = self.config.get("extensions")
+        if not extensions or not isinstance(extensions, list):
+            return
+        for extension in extensions:
+            try:
+                __import__(extension, globals(), locals(), [extension.rpartition(".")[-1]])
+            except Exception as e:
+                get_logger().warning("import extension %s error %s:%s", extension, e.__class__.__name__, str(e))
+
     def merge_config(self, config):
         for k, v in config.items():
             if k in ("arguments", "imports", "defines", "variables", "sources", "logger", "options"):
                 if not isinstance(v, dict) or not isinstance(self.config.get(k, {}), dict):
                     continue
 
                 if k not in self.config:
```

### Comparing `syncanysql-0.1.0/syncanysql/executor.py` & `syncanysql-0.1.1/syncanysql/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # 2023/2/13
 # create by: snower
 
 import os
 import sys
 import re
-import copy
 import threading
 from collections import deque
 from syncany.filters import StringFilter
 from syncany.calculaters import find_calculater
 from syncany.database import find_database
 from .errors import SyncanySqlCompileException
 from .utils import parse_value
@@ -23,19 +22,19 @@
 class EnvVariables(dict):
     def __init__(self, parent=None, *args, **kwargs):
         super(EnvVariables, self).__init__(*args, **kwargs)
 
         self.parent = parent
 
     @classmethod
-    def build_global(cls):
+    def build_global(cls, session_config):
         env_variables = cls()
         env_variables.update({key.lower(): value for key, value in os.environ.items()})
         env_variables["home"] = os.path.expanduser('~')
-        env_variables["syncany_home"] = os.path.join(os.path.expanduser('~'), ".syncany")
+        env_variables["syncany_home"] = session_config.get_home()
         env_variables["cwd"] = os.getcwd()
         env_variables["platform"] = sys.platform
         for arg in sys.argv:
             if arg[:2] != "--":
                 continue
             arg_info = arg[2:].split("=")
             arg_value = arg_info[1] if len(arg_info) >= 2 else True
@@ -74,16 +73,17 @@
     def __init__(self, manager, session_config, parent_executor=None):
         self.manager = manager
         self.session_config = session_config
         self.parent_executor = parent_executor
         self.runners = deque()
         self.tasker = None
         if self.global_env_variables is None:
-            self.__class__.global_env_variables = EnvVariables.build_global()
-        self.env_variables = EnvVariables(parent_executor.env_variables if parent_executor else self.global_env_variables)
+            self.__class__.global_env_variables = EnvVariables.build_global(session_config)
+        self.env_variables = EnvVariables(parent_executor.env_variables if parent_executor
+                                          else self.global_env_variables)
 
     def compile_variable(self, sql):
         variables = ENV_VARIABLE_RE.findall(sql)
         for variable, default_value in variables:
             variable_name = variable[2:-1].split(":")[0]
             try:
                 variable_value = self.env_variables.get_value(variable_name.lower())
@@ -116,23 +116,26 @@
                     raise SyncanySqlCompileException("raw sql name error: %s", raw)
                 raw_sql = "set @config.databases." + raw_name_info[0] + ".virtual_views." + raw_name_info[1] + "='''\n" + raw_sql.strip() + "\n'''"
                 self.compile(name + "(" + str(lineno) + ")#set_virtual_view", raw_sql)
                 sql = sql.replace(raw, raw_name)
             self.compile(name + "(" + str(lineno) + ")", sql)
 
     def compile(self, name, sql):
-        config = copy.deepcopy(self.session_config.get())
+        config = self.session_config.get()
         config["name"] = name
-        compiler = Compiler(config, self.env_variables)
-        arguments = {"@verbose": self.env_variables.get("@verbose", False), "@timeout": self.env_variables.get("@timeout", 0),
-                     "@limit": self.env_variables.get("@limit", 0), "@batch": self.env_variables.get("@batch", 0),
-                     "@streaming": self.env_variables.get("@streaming", False), "@recovery": self.env_variables.get("@recovery", False),
-                     "@join_batch": self.env_variables.get("@join_batch", 10000), "@insert_batch": self.env_variables.get("@insert_batch", 0),
-                     "@primary_order": False}
-        tasker = compiler.compile(sql, arguments)
+        try:
+            compiler = Compiler(config, self.env_variables)
+            arguments = {"@verbose": self.env_variables.get("@verbose", False), "@timeout": self.env_variables.get("@timeout", 0),
+                         "@limit": self.env_variables.get("@limit", 0), "@batch": self.env_variables.get("@batch", 0),
+                         "@streaming": self.env_variables.get("@streaming", False), "@recovery": self.env_variables.get("@recovery", False),
+                         "@join_batch": self.env_variables.get("@join_batch", 10000), "@insert_batch": self.env_variables.get("@insert_batch", 0),
+                         "@primary_order": False}
+            tasker = compiler.compile(sql, arguments)
+        finally:
+            config["name"] = ""
         self.runners.extend(tasker.start(name, self, self.session_config, self.manager, arguments))
 
     def execute(self):
         while self.runners:
             self.tasker = self.runners.popleft()
             try:
                 exit_code = self.tasker.run(self, self.session_config, self.manager)
```

### Comparing `syncanysql-0.1.0/syncanysql/main.py` & `syncanysql-0.1.1/syncanysql/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         global_config = GlobalConfig()
         init_execute_files = global_config.load()
         if not sys.stdin.isatty() and (len(sys.argv) == 1 or (
                 len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
             global_config.config_logging(False)
         else:
             global_config.config_logging(True)
+        global_config.load_extensions()
         manager = TaskerManager(DatabaseManager())
 
         try:
             with Executor(manager, global_config.session()) as executor:
                 if init_execute_files:
                     executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in range(len(init_execute_files))])
                     exit_code = executor.execute()
```

### Comparing `syncanysql-0.1.0/syncanysql/parser.py` & `syncanysql-0.1.1/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/prompt.py` & `syncanysql-0.1.1/syncanysql/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,154 +1,150 @@
 # -*- coding: utf-8 -*-
 # 2023/2/8
 # create by: snower
 
 import os
 import sys
-from collections import defaultdict
 from pygments.lexers import SqlLexer
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.lexers import PygmentsLexer
 from prompt_toolkit.styles import Style
 from prompt_toolkit.filters import Condition
 from prompt_toolkit.cursor_shapes import CursorShape
 from .version import version
 from .parser import SqlParser, SqlSegment
 
-sql_completer = WordCompleter(
-    [
-        "abort",
-        "action",
-        "add",
-        "after",
-        "all",
-        "alter",
-        "analyze",
-        "and",
-        "as",
-        "asc",
-        "attach",
-        "autoincrement",
-        "before",
-        "begin",
-        "between",
-        "by",
-        "cascade",
-        "case",
-        "cast",
-        "check",
-        "collate",
-        "column",
-        "commit",
-        "conflict",
-        "constraint",
-        "create",
-        "cross",
-        "current_date",
-        "current_time",
-        "current_timestamp",
-        "database",
-        "default",
-        "deferrable",
-        "deferred",
-        "delete",
-        "desc",
-        "detach",
-        "distinct",
-        "drop",
-        "each",
-        "else",
-        "end",
-        "escape",
-        "except",
-        "exclusive",
-        "exists",
-        "explain",
-        "fail",
-        "for",
-        "foreign",
-        "from",
-        "full",
-        "glob",
-        "group",
-        "having",
-        "if",
-        "ignore",
-        "immediate",
-        "in",
-        "index",
-        "indexed",
-        "initially",
-        "inner",
-        "insert",
-        "instead",
-        "intersect",
-        "into",
-        "is",
-        "isnull",
-        "join",
-        "key",
-        "left",
-        "like",
-        "limit",
-        "match",
-        "natural",
-        "no",
-        "not",
-        "notnull",
-        "null",
-        "of",
-        "offset",
-        "on",
-        "or",
-        "order",
-        "outer",
-        "plan",
-        "pragma",
-        "primary",
-        "query",
-        "raise",
-        "recursive",
-        "references",
-        "regexp",
-        "reindex",
-        "release",
-        "rename",
-        "replace",
-        "restrict",
-        "right",
-        "rollback",
-        "row",
-        "savepoint",
-        "select",
-        "set",
-        "table",
-        "temp",
-        "temporary",
-        "then",
-        "to",
-        "transaction",
-        "trigger",
-        "union",
-        "unique",
-        "update",
-        "using",
-        "vacuum",
-        "values",
-        "view",
-        "virtual",
-        "when",
-        "where",
-        "with",
-        "without",
-    ],
-    ignore_case=True,
-)
+SQL_COMPLETER_WORDS = [
+    "abort",
+    "action",
+    "add",
+    "after",
+    "all",
+    "alter",
+    "analyze",
+    "and",
+    "as",
+    "asc",
+    "attach",
+    "autoincrement",
+    "before",
+    "begin",
+    "between",
+    "by",
+    "cascade",
+    "case",
+    "cast",
+    "check",
+    "collate",
+    "column",
+    "commit",
+    "conflict",
+    "constraint",
+    "create",
+    "cross",
+    "current_date",
+    "current_time",
+    "current_timestamp",
+    "database",
+    "default",
+    "deferrable",
+    "deferred",
+    "delete",
+    "desc",
+    "detach",
+    "distinct",
+    "drop",
+    "each",
+    "else",
+    "end",
+    "escape",
+    "except",
+    "exclusive",
+    "exists",
+    "explain",
+    "fail",
+    "for",
+    "foreign",
+    "from",
+    "full",
+    "glob",
+    "group",
+    "having",
+    "if",
+    "ignore",
+    "immediate",
+    "in",
+    "index",
+    "indexed",
+    "initially",
+    "inner",
+    "insert",
+    "instead",
+    "intersect",
+    "into",
+    "is",
+    "isnull",
+    "join",
+    "key",
+    "left",
+    "like",
+    "limit",
+    "match",
+    "natural",
+    "no",
+    "not",
+    "notnull",
+    "null",
+    "of",
+    "offset",
+    "on",
+    "or",
+    "order",
+    "outer",
+    "plan",
+    "pragma",
+    "primary",
+    "query",
+    "raise",
+    "recursive",
+    "references",
+    "regexp",
+    "reindex",
+    "release",
+    "rename",
+    "replace",
+    "restrict",
+    "right",
+    "rollback",
+    "row",
+    "savepoint",
+    "select",
+    "set",
+    "table",
+    "temp",
+    "temporary",
+    "then",
+    "to",
+    "transaction",
+    "trigger",
+    "union",
+    "unique",
+    "update",
+    "using",
+    "vacuum",
+    "values",
+    "view",
+    "virtual",
+    "when",
+    "where",
+    "with",
+    "without",
+]
 
 style = Style.from_dict(
     {
         "completion-menu.completion": "bg:#008888 #ffffff",
         "completion-menu.completion.current": "bg:#00aaaa #000000",
         "scrollbar.background": "bg:#88aaaa",
         "scrollbar.button": "bg:#222222",
@@ -197,17 +193,20 @@
 class CliPrompt(object):
     def __init__(self, manager, session_config, executor):
         self.manager = manager
         self.session_config = session_config
         self.executor = executor
 
     def run(self):
-        home_config_path = os.path.join(os.path.expanduser('~'), ".syncany")
+        home_config_path = self.session_config.get_home()
         if not os.path.exists(home_config_path):
             os.mkdir(home_config_path)
+        database_completer_words = [database["name"] for database in (self.session_config.get().get("databases") or [])
+                                    if database["name"] not in ("-", "--")]
+        sql_completer = WordCompleter(SQL_COMPLETER_WORDS + database_completer_words, ignore_case=True)
         history = CliFileHistory(os.path.join(home_config_path, "history"))
         session = PromptSession(
             lexer=PygmentsLexer(SqlLexer), completer=sql_completer, style=style, history=history
         )
         print("Python %s" % sys.version)
         print("Syncany-SQL %s -- Simple and easy-to-use sql execution engine" % version)
         lineno = 1
```

### Comparing `syncanysql-0.1.0/syncanysql/taskers/delete.py` & `syncanysql-0.1.1/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/taskers/execute.py` & `syncanysql-0.1.1/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/taskers/explain.py` & `syncanysql-0.1.1/syncanysql/taskers/explain.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 # 2023/2/14
 # create by: snower
 
 import copy
 import datetime
 from syncany.main import beautify_print
 
+
 class ExplainTasker(object):
-    def __init__(self, tasker):
+    def __init__(self, tasker, sql=None):
         self.config = None
         self.tasker = tasker
+        self.sql = sql
 
     def start(self, name, executor, session_config, manager, arguments):
         self.config = copy.deepcopy(self.tasker.config)
+        if self.sql:
+            beautify_print("%s tasker %s execute sql:\n%s" % (datetime.datetime.now(), self.config["name"], self.sql))
+            print()
         beautify_print("%s tasker %s compiled config:" % (datetime.datetime.now(), self.config["name"]))
         beautify_print(self.config)
         print()
 
         for key in list(arguments.keys()):
             if key.endswith("@verbose"):
                 arguments[key] = True
```

### Comparing `syncanysql-0.1.0/syncanysql/taskers/into.py` & `syncanysql-0.1.1/syncanysql/taskers/into.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,15 +42,19 @@
             database = database_cls(manager.database_manager, database_config).build()
             try:
                 query = database.query(name, ["id"])
                 datas = query.commit()
                 delete = database.delete(name, ["id"])
                 delete.commit()
 
-                if schema_keys and len(schema_keys) == 1:
+                if not schema_keys:
+                    value = datas[0] if len(datas) == 1 else datas
+                    if len(self.config["variables"]) == 1 and isinstance(value, dict) and len(value) == 1:
+                        value = list(value.values())[0]
+                elif len(schema_keys) == 1:
                     if len(datas) == 1:
                         value = datas[0][schema_keys[0]] if schema_keys[0] in datas[0] else None
                     else:
                         value = [data[schema_keys[0]] for data in datas if schema_keys[0] in data]
                 else:
                     if len(datas) == 1:
                         value = {key: datas[0].get(key) for key in schema_keys}
@@ -65,15 +69,18 @@
                         executor.env_variables[self.config["variables"][0]] = value
                 else:
                     for i in range(len(self.config["variables"])):
                         if i >= len(schema_keys):
                             if self.config["variables"][i] in executor.env_variables:
                                 executor.env_variables[self.config["variables"][i]] = None
                             continue
-                        executor.env_variables[self.config["variables"][i]] = value[schema_keys[i]]
+                        if isinstance(value, dict):
+                            executor.env_variables[self.config["variables"][i]] = value[schema_keys[i]]
+                        else:
+                            executor.env_variables[self.config["variables"][i]] = [v[schema_keys[i]] for v in value]
                 return exit_code
             finally:
                 database.close()
         finally:
             self.tasker = None
 
     def terminate(self):
```

### Comparing `syncanysql-0.1.0/syncanysql/taskers/query.py` & `syncanysql-0.1.1/syncanysql/taskers/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # 2023/2/8
 # create by: snower
 
 import os
 import copy
+import time
 import traceback
 import uuid
 from syncany.logger import get_logger
 from syncany.taskers.core import CoreTasker
 from syncany.hook import Hooker
 from syncany.taskers.tasker import _thread_local
 from syncany.main import TaskerYieldNext, warp_database_logging
@@ -45,23 +46,26 @@
     def finaled(self, tasker, e=None):
         if e is not None or self.batch_count <= 1:
             return
         self.tasker.run_reduce(self.executor, self.session_config, self.manager, self.arguments, False)
 
 
 class QueryTasker(object):
-    def __init__(self, config):
+    def __init__(self, config, sql_expression=None):
+        self.name = config.get("name", "")
         self.config = config
+        self.sql_expression = sql_expression
         self.reduce_config = None
         self.tasker = None
         self.dependency_taskers = []
         self.arguments = None
         self.tasker_generator = None
         self.updaters = []
         self.temporary_memory_collections = set([])
+        self.run_start_time = 0
 
     def start(self, name, executor, session_config, manager, arguments):
         dependency_taskers, aggregate = [], self.config.pop("aggregate", None)
         if aggregate and aggregate.get("distinct_keys"):
             self.config, distinct_config = self.compile_distinct_config(aggregate), self.config
             distinct_config["name"] = distinct_config["name"] + "#select@distinct"
             distinct_tasker = QueryTasker(distinct_config)
@@ -119,29 +123,36 @@
         return [self]
 
     def run(self, executor, session_config, manager):
         try:
             self.execute_updater(executor, session_config, manager)
             if not self.tasker_generator:
                 self.tasker_generator = self.run_tasker(executor, session_config, manager, self.tasker, self.dependency_taskers)
+                self.run_start_time = time.time()
             else:
                 _thread_local.current_tasker = self.tasker
             while True:
                 try:
                     value = self.tasker_generator.send(None)
                     if isinstance(value, TaskerYieldNext):
                         executor.add_runner(self)
                         return 0
                 except StopIteration as e:
                     exit_code = e.value
                     if exit_code is not None and exit_code != 0:
+                        if self.sql_expression:
+                            get_logger().info("execute SQL %s finish with code %s %.2fms", self.name, exit_code,
+                                              (time.time() - self.run_start_time) * 1000)
                         return exit_code
                     break
             if self.reduce_config:
-                return self.run_reduce(executor, session_config, manager, self.arguments, True)
+                exit_code = self.run_reduce(executor, session_config, manager, self.arguments, True)
+            if self.sql_expression:
+                get_logger().info("execute SQL %s finish with code %s %.2fms", self.name, exit_code,
+                                  (time.time() - self.run_start_time) * 1000)
             return exit_code
         finally:
             names = self.get_temporary_memory_collections()
             if names:
                 executor.clear_temporary_memory_collection(names)
 
     def run_yield(self, executor, session_config, manager, tasker, dependency_taskers):
@@ -174,14 +185,16 @@
             return
         self.tasker.terminate()
         self.tasker = None
 
     def compile_distinct_config(self, aggregate):
         subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_distinct"
         config = copy.deepcopy(self.config)
+        config.pop("loader", None)
+        config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
             "querys": [],
             "caches": [],
             "imports": {},
             "sources": {},
@@ -232,19 +245,23 @@
         self.config["aggregate"] = distinct_aggregate
         if [having_column for having_column in aggregate["having_columns"] if having_column in aggregate["schema"]]:
             config["intercepts"] = self.config.pop("intercepts", [])
         else:
             distinct_aggregate["having_columns"] = aggregate["having_columns"]
         config["pipelines"] = self.config.pop("pipelines", [])
         self.config["output"] = "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0] + " use I"
+        self.config.pop("outputer", None)
+        self.config.pop("outputer_arguments", None)
         return config
 
     def compile_reduce_config(self, aggregate):
         subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_reduce"
         config = copy.deepcopy(self.config)
+        config.pop("loader", None)
+        config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
             "querys": [],
             "caches": [],
             "imports": {},
             "sources": {},
@@ -264,14 +281,16 @@
             else:
                 config["schema"][key] = "$." + key
         if aggregate["key"]:
             config["schema"]["_aggregate_key_"] = "$._aggregate_key_"
             self.config["schema"]["_aggregate_key_"] = aggregate["key"]
         config["aggregate"] = aggregate
         self.config["output"] = "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0] + " use I"
+        self.config.pop("outputer", None)
+        self.config.pop("outputer_arguments", None)
         self.reduce_config = config
 
     def run_reduce(self, executor, session_config, manager, arguments, final_reduce=False):
         config, arguments = copy.deepcopy(self.reduce_config), copy.deepcopy(arguments)
         if final_reduce:
             config["schema"].pop("_aggregate_key_", None)
             for key, column in config["schema"].items():
```

### Comparing `syncanysql-0.1.0/syncanysql/taskers/set.py` & `syncanysql-0.1.1/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/taskers/show.py` & `syncanysql-0.1.1/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/taskers/use.py` & `syncanysql-0.1.1/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql/utils.py` & `syncanysql-0.1.1/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.0/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.1/syncanysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -28,18 +28,24 @@
         - [特性与限制](docs/feature-restrictions.md)
         - [配置详解](docs/configure.md)
         - [驱动依赖](docs/driver-dependency.md)
         - [示例详解](examples)
         
         ## 安装
         
-        ```
+        ```bash
         pip3 install syncanysql
         ```
         
+        #### Docker
+        
+        ```bash
+        docker pull sujin190/syncany-sql
+        ```
+        
         ## 查询Nginx日志
         
         ```sql
         -- 查询访问量最高的三个IP
         SELECT seg0 AS ip, COUNT(*) AS cnt FROM `file://data/access.log?sep= ` GROUP BY seg0 ORDER BY cnt DESC LIMIT 3;
         ```
```

### Comparing `syncanysql-0.1.0/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.1/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

