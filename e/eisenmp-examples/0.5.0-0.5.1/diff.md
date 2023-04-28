# Comparing `tmp/eisenmp_examples-0.5.0.tar.gz` & `tmp/eisenmp_examples-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.5.0.tar", last modified: Fri Apr 28 19:28:04 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.5.1.tar", last modified: Fri Apr 28 20:49:52 2023, max compression
```

## Comparing `eisenmp_examples-0.5.0.tar` & `eisenmp_examples-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.357854 eisenmp_examples-0.5.0/
--rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/LICENSE.rst
--rw-rw-rw-   0        0        0      204 2023-04-25 15:46:07.000000 eisenmp_examples-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4331 2023-04-28 19:28:04.358853 eisenmp_examples-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3585 2023-04-27 22:03:28.000000 eisenmp_examples-0.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.260494 eisenmp_examples-0.5.0/eisenmp_examples/
--rw-rw-rw-   0        0        0        0 2023-04-25 15:47:48.000000 eisenmp_examples-0.5.0/eisenmp_examples/__init__.py
--rw-rw-rw-   0        0        0     2141 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-27 21:36:54.000000 eisenmp_examples-0.5.0/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0    12382 2023-04-27 21:35:25.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     6178 2023-04-24 09:07:06.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     3337 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     6806 2023-04-28 18:31:29.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     8643 2023-04-25 15:48:13.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     4446 2023-04-23 17:20:07.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     8130 2023-04-22 14:38:05.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     6613 2023-04-25 15:51:49.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.322476 eisenmp_examples-0.5.0/eisenmp_examples/test/
--rw-rw-rw-   0        0        0        0 2023-04-28 07:49:18.000000 eisenmp_examples-0.5.0/eisenmp_examples/test/__init__.py
--rw-rw-rw-   0        0        0      692 2023-04-28 19:02:18.000000 eisenmp_examples-0.5.0/eisenmp_examples/test/test_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.337474 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/
--rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/__init__.py
--rw-rw-rw-   0        0        0      295 2023-04-28 19:12:09.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/db_exa_schema.sql
--rw-rw-rw-   0        0        0     1919 2023-04-25 15:43:23.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_download.py
--rw-rw-rw-   0        0        0     4419 2023-04-26 18:04:52.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_search.py
--rw-rw-rw-   0        0        0     7644 2023-04-25 15:43:49.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.356854 eisenmp_examples-0.5.0/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/__init__.py
--rw-rw-rw-   0        0        0     4615 2023-04-27 03:39:04.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     5776 2023-04-21 11:49:17.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3468 2023-04-25 15:49:34.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     4704 2023-04-25 15:44:58.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     2055 2023-04-25 15:45:25.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     2525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.317487 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-28 19:28:02.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1067 2023-04-28 18:50:49.000000 eisenmp_examples-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-28 19:28:04.368850 eisenmp_examples-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.655025 eisenmp_examples-0.5.1/
+-rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      204 2023-04-25 15:46:07.000000 eisenmp_examples-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4319 2023-04-28 20:49:52.655025 eisenmp_examples-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3585 2023-04-27 22:03:28.000000 eisenmp_examples-0.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.569193 eisenmp_examples-0.5.1/eisenmp_examples/
+-rw-rw-rw-   0        0        0        0 2023-04-25 15:47:48.000000 eisenmp_examples-0.5.1/eisenmp_examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.613084 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/
+-rw-rw-rw-   0        0        0      169 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9151 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_bruteforce.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3951 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_double_q.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2284 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_each_flask_orm_srv_one_cpu.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5945 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_entry.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5871 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_http.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2850 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_multi_srv_each_cpu.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5656 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_prime.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5158 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/__pycache__/eisenmp_exa_web_csv.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2141 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-27 21:36:54.000000 eisenmp_examples-0.5.1/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    12378 2023-04-28 20:39:23.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6178 2023-04-24 09:07:06.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3337 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6894 2023-04-28 20:39:23.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8643 2023-04-25 15:48:13.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4446 2023-04-23 17:20:07.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     8130 2023-04-22 14:38:05.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6613 2023-04-25 15:51:49.000000 eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.616985 eisenmp_examples-0.5.1/eisenmp_examples/test/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:49:18.000000 eisenmp_examples-0.5.1/eisenmp_examples/test/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-04-28 19:02:18.000000 eisenmp_examples-0.5.1/eisenmp_examples/test/test_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.626739 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.634542 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__pycache__/
+-rw-rw-rw-   0        0        0      179 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2297 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__pycache__/eisenmp_download.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4941 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__pycache__/eisenmp_search.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8646 2023-04-28 20:40:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/__pycache__/eisenmp_utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0    24576 2023-04-28 20:41:06.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/db_exa.db
+-rw-rw-rw-   0        0        0      295 2023-04-28 19:12:09.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/db_exa_schema.sql
+-rw-rw-rw-   0        0        0     1919 2023-04-25 15:43:23.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4419 2023-04-26 18:04:52.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     7644 2023-04-25 15:43:49.000000 eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.649172 eisenmp_examples-0.5.1/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.653074 eisenmp_examples-0.5.1/eisenmp_examples/worker/__pycache__/
+-rw-rw-rw-   0        0        0     3786 2023-04-28 20:40:45.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_bf_bruteforce.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4498 2023-04-28 20:40:47.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/__pycache__/eisenmp_exa_wrk_bf_reduce.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4615 2023-04-27 03:39:04.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     5776 2023-04-21 11:49:17.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3468 2023-04-25 15:49:34.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     4704 2023-04-25 15:44:58.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     2055 2023-04-25 15:45:25.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     2525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:49:52.595527 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 20:49:52.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 20:49:51.000000 eisenmp_examples-0.5.1/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1055 2023-04-28 20:45:39.000000 eisenmp_examples-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-28 20:49:52.662827 eisenmp_examples-0.5.1/setup.cfg
```

### Comparing `eisenmp_examples-0.5.0/LICENSE` & `eisenmp_examples-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/LICENSE.rst` & `eisenmp_examples-0.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/PKG-INFO` & `eisenmp_examples-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.5.0
-Summary: eisenmp multiprocess(or) example collection for server and mobiles
+Version: 0.5.1
+Summary: eisenmp multiprocess(or) example collection for server
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
 Keywords: multiprocess framework,examples eisenmp
```

### Comparing `eisenmp_examples-0.5.0/README.rst` & `eisenmp_examples-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/cmd.py` & `eisenmp_examples-0.5.1/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/database.db` & `eisenmp_examples-0.5.1/eisenmp_examples/database.db`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # Worker part - toolbox vars survive multiple worker calls
         self.multi_tool_get = None  # custom var to allow only one download of MULTI_TOOL; init later in this example
         self.MULTI_TOOL = None  # pre-defined toolbox.MULTI_TOOL can host the dict from mp_tools_q
 
-        # self.INFO_ENABLE = True  # info thread collects list row count, makes sense if no instances start overlapped
-        # self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
+        self.INFO_ENABLE = True  # info thread collects list row count, makes sense if no instances start overlapped
+        self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
 
         # custom
         self.use_file_system = False  # False: download and unzip in mem        ------------ SWITCH --------------------
         self.result_lbl = None  # set by caller
         self.num_lists = 0  # add one for each list done, print out worker
         self.lowercase = True
         self.url = None  # 'use_file_system' False, URL of csv file
```

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_double_q.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_double_q.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,31 +50,33 @@
         (3, example_menu[3], web_csv.main, 'False'),
         (4, example_menu[4], http_srv.main, 'True'),
         (5, example_menu[5], double_q.main, 'False'),
         (6, example_menu[6], bruteforce.main, 'False')
     ]
 
 
-def run_http(com_queue):
+def run_http(com_queue=None):
     """Blocked, no loop here
+
+    :params: com_queue: test setup, know when server is up
     """
     global serverPort
 
     while 1:
         try:
             webServer = HTTPServer((hostName, serverPort), MyServer)
             break
         except OSError:
             print(f'serverPort in use {serverPort}')
             print('\n\tadd one to port number')
             serverPort += 1  # port already in use
 
     print("Examples http://%s:%s" % (hostName, serverPort))
-
-    com_queue.put(b'ready')
+    if com_queue:
+        com_queue.put(b'ready')
     try:
         webServer.serve_forever()
     except KeyboardInterrupt:
         pass
     webServer.server_close()
     print("Server stopped.")
```

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_http.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_prime.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_web_csv.py` & `eisenmp_examples-0.5.1/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/test/test_entry.py` & `eisenmp_examples-0.5.1/eisenmp_examples/test/test_entry.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_download.py` & `eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_search.py` & `eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_search.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_utils.py` & `eisenmp_examples-0.5.1/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_double.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.5.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.5.0/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.5.1/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.5.0
-Summary: eisenmp multiprocess(or) example collection for server and mobiles
+Version: 0.5.1
+Summary: eisenmp multiprocess(or) example collection for server
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
 Keywords: multiprocess framework,examples eisenmp
```

### Comparing `eisenmp_examples-0.5.0/pyproject.toml` & `eisenmp_examples-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.5.0"
+version = "0.5.1"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
-description = "eisenmp multiprocess(or) example collection for server and mobiles"
+description = "eisenmp multiprocess(or) example collection for server"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
 readme = "README.rst"
 requires-python = ">=3.7"
 
 
 classifiers = [
```

