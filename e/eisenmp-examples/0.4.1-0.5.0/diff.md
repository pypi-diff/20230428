# Comparing `tmp/eisenmp_examples-0.4.1.tar.gz` & `tmp/eisenmp_examples-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.4.1.tar", last modified: Fri Apr 14 09:12:24 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.5.0.tar", last modified: Fri Apr 28 19:28:04 2023, max compression
```

## Comparing `eisenmp_examples-0.4.1.tar` & `eisenmp_examples-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/LICENSE.rst
--rw-rw-rw-   0        0        0      230 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4330 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.522563 eisenmp_examples-0.4.1/eisenmp_examples/
--rw-rw-rw-   0        0        0      344 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/__init__.py
--rw-rw-rw-   0        0        0     2141 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0    10406 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     6249 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     3330 2023-04-13 20:55:03.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     6573 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     8641 2023-04-13 20:55:03.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     4614 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     8136 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     6608 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.569645 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_download.py
--rw-rw-rw-   0        0        0     4139 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_search.py
--rw-rw-rw-   0        0        0     6183 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/__init__.py
--rw-rw-rw-   0        0        0     3812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     5300 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3621 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     4603 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     2059 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     2507 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     1571 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.555629 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4330 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 09:12:23.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1066 2023-04-14 09:07:07.000000 eisenmp_examples-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-14 09:12:24.735628 eisenmp_examples-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.357854 eisenmp_examples-0.5.0/
+-rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/LICENSE.rst
+-rw-rw-rw-   0        0        0      204 2023-04-25 15:46:07.000000 eisenmp_examples-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4331 2023-04-28 19:28:04.358853 eisenmp_examples-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3585 2023-04-27 22:03:28.000000 eisenmp_examples-0.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.260494 eisenmp_examples-0.5.0/eisenmp_examples/
+-rw-rw-rw-   0        0        0        0 2023-04-25 15:47:48.000000 eisenmp_examples-0.5.0/eisenmp_examples/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-27 21:36:54.000000 eisenmp_examples-0.5.0/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    12382 2023-04-27 21:35:25.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6178 2023-04-24 09:07:06.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3337 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6806 2023-04-28 18:31:29.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8643 2023-04-25 15:48:13.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4446 2023-04-23 17:20:07.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     8130 2023-04-22 14:38:05.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6613 2023-04-25 15:51:49.000000 eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.322476 eisenmp_examples-0.5.0/eisenmp_examples/test/
+-rw-rw-rw-   0        0        0        0 2023-04-28 07:49:18.000000 eisenmp_examples-0.5.0/eisenmp_examples/test/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-04-28 19:02:18.000000 eisenmp_examples-0.5.0/eisenmp_examples/test/test_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.337474 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-04-28 19:12:09.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/db_exa_schema.sql
+-rw-rw-rw-   0        0        0     1919 2023-04-25 15:43:23.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4419 2023-04-26 18:04:52.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     7644 2023-04-25 15:43:49.000000 eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.356854 eisenmp_examples-0.5.0/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0        0 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/__init__.py
+-rw-rw-rw-   0        0        0     4615 2023-04-27 03:39:04.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     5776 2023-04-21 11:49:17.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3468 2023-04-25 15:49:34.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     4704 2023-04-25 15:44:58.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     2055 2023-04-25 15:45:25.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     2525 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 08:59:21.000000 eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:28:04.317487 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4331 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 19:28:04.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 19:28:02.000000 eisenmp_examples-0.5.0/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1067 2023-04-28 18:50:49.000000 eisenmp_examples-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-28 19:28:04.368850 eisenmp_examples-0.5.0/setup.cfg
```

### Comparing `eisenmp_examples-0.4.1/LICENSE` & `eisenmp_examples-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4.1/LICENSE.rst` & `eisenmp_examples-0.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4.1/PKG-INFO` & `eisenmp_examples-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.4.1
+Version: 0.5.0
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
 Keywords: multiprocess framework,examples eisenmp
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE
 License-File: LICENSE.rst
 
-# eisenmp_examples
- 
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
-[Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
+eisenmp_examples
+##################
+
+.. image:: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml
+
+
+Python 3.7 `Multiprocess <https://en.wikipedia.org/wiki/Multiprocessing>`_
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for single Server
 
 Examples:
 
 * simple style prime number calculation to see the basic use
 * simple http server on one cpu gets content via queue
 * one flask orm server on each cpu - share a user db
 * multiple flask orm server on each cpu, port groups - share a user db
@@ -33,85 +38,94 @@
 * brute_force_attack with itertools generator and dictionary
 * example with two, double fed queues
 * All scenarios follow the **Template style** and have descriptions
 
 ## How to run the examples?
 
 1. Clone the repo and ``run an eisenmp_exa_...`` or
-2. Install [PyPi package](https://pypi.org/project/eisenmp-examples/)
+2. Install `PyPi package <https://pypi.org/project/eisenmp-examples>`_
+
 * in terminal run: `eisenmp_url` and open the local Python SimpleHTTP **URL**
 * in terminal run: `eisenmp_menu` and choose from **Menu**
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
+::
+
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
-
-	[BRUTE_FORCE]	cfhhilorrs
-
+    [BRUTE_FORCE]
+    cfhhilorrs
     Create processes. Default: proc/CPU core
     0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 
     
     ... proc Process-7 ... rohrschilf
     ... proc Process-14 ... rohrschilf
     ... proc Process-16 ... rohrschilf
     ... proc Process-7 ... rohrschilf
     ... proc Process-13 ... schilfrohr
     ... proc Process-13 ... schilfrohr
     ... proc Process-11 ... schilfrohr
     ... proc Process-11 ... schilfrohr
 
-	generator empty, run time iterator 5 seconds
-
-	exit WORKER 15
-	exit WORKER 16
-	exit WORKER 2
-	exit WORKER 10
-	exit WORKER 11
-	exit WORKER 12
-	exit WORKER 8
-	exit WORKER 3
-	exit WORKER 4
-	exit WORKER 6
-	exit WORKER 14
-	exit WORKER 5
-	exit WORKER 7
-	exit WORKER 13
-	exit WORKER 1
-	exit WORKER 9
+    generator empty, run time iterator 5 seconds
 
+    exit WORKER 15
+    exit WORKER 16
+    exit WORKER 2
+    exit WORKER 10
+    exit WORKER 11
+    exit WORKER 12
+    exit WORKER 8
+    exit WORKER 3
+    exit WORKER 4
+    exit WORKER 6
+    exit WORKER 14
+    exit WORKER 5
+    exit WORKER 7
+    exit WORKER 13
+    exit WORKER 1
+    exit WORKER 9
+    
     --- Result for [CFHHILORRS]---
     
      rohrschilf
     
      schilfrohr
 
     --- END ---
 
-	Processes are down.
+    Processes are down.
     BF Time in sec: 12
     
     Process finished with exit code 0
 
-    Inbuild example, assert a scrambled string. Use brute force or condensing.
+
+Brute Force
     We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
-    (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
-        Permutation lists grow very fast, reaching Terabyte size.
-    (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
-
-`eisenmp` uses Pythons permutation generator
- [itertools](https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations)
-for the brute force attack example.
 
-    Another example downloads a large list and calculates average for one column.
+    len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
+    Permutation lists grow very fast, reaching Terabyte size.
+
+    len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
+
+Web download a large list
+    Calculates the average for one column.
     Python CSV extracts the column and we calculate the average with the assigned number
     of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
 
 
-- large lists https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©. 
-All material Stats NZ produces is protected by Crown copyright.
-Creative Commons Attribution 4.0 International licence.
-- German dict https://sourceforge.net/projects/germandict/. License Public Domain
-- English dict Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-- ORM Flask-SQLAlchemy https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
+large lists
+    https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©.
+    All material Stats NZ produces is protected by Crown copyright.
+    Creative Commons Attribution 4.0 International licence.
+
+German dict
+    https://sourceforge.net/projects/germandict/. License Public Domain
+
+English dict
+    Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
+
+ORM Flask-SQLAlchemy
+     https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
 
 Cheers
```

### Comparing `eisenmp_examples-0.4.1/README.md` & `eisenmp_examples-0.5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-# eisenmp_examples
- 
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
-[Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
+eisenmp_examples
+##################
+
+.. image:: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml
+
+
+Python 3.7 `Multiprocess <https://en.wikipedia.org/wiki/Multiprocessing>`_
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for single Server
 
 Examples:
 
 * simple style prime number calculation to see the basic use
 * simple http server on one cpu gets content via queue
 * one flask orm server on each cpu - share a user db
 * multiple flask orm server on each cpu, port groups - share a user db
@@ -13,85 +18,94 @@
 * brute_force_attack with itertools generator and dictionary
 * example with two, double fed queues
 * All scenarios follow the **Template style** and have descriptions
 
 ## How to run the examples?
 
 1. Clone the repo and ``run an eisenmp_exa_...`` or
-2. Install [PyPi package](https://pypi.org/project/eisenmp-examples/)
+2. Install `PyPi package <https://pypi.org/project/eisenmp-examples>`_
+
 * in terminal run: `eisenmp_url` and open the local Python SimpleHTTP **URL**
 * in terminal run: `eisenmp_menu` and choose from **Menu**
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
+::
+
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
-
-	[BRUTE_FORCE]	cfhhilorrs
-
+    [BRUTE_FORCE]
+    cfhhilorrs
     Create processes. Default: proc/CPU core
     0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 
     
     ... proc Process-7 ... rohrschilf
     ... proc Process-14 ... rohrschilf
     ... proc Process-16 ... rohrschilf
     ... proc Process-7 ... rohrschilf
     ... proc Process-13 ... schilfrohr
     ... proc Process-13 ... schilfrohr
     ... proc Process-11 ... schilfrohr
     ... proc Process-11 ... schilfrohr
 
-	generator empty, run time iterator 5 seconds
-
-	exit WORKER 15
-	exit WORKER 16
-	exit WORKER 2
-	exit WORKER 10
-	exit WORKER 11
-	exit WORKER 12
-	exit WORKER 8
-	exit WORKER 3
-	exit WORKER 4
-	exit WORKER 6
-	exit WORKER 14
-	exit WORKER 5
-	exit WORKER 7
-	exit WORKER 13
-	exit WORKER 1
-	exit WORKER 9
+    generator empty, run time iterator 5 seconds
 
+    exit WORKER 15
+    exit WORKER 16
+    exit WORKER 2
+    exit WORKER 10
+    exit WORKER 11
+    exit WORKER 12
+    exit WORKER 8
+    exit WORKER 3
+    exit WORKER 4
+    exit WORKER 6
+    exit WORKER 14
+    exit WORKER 5
+    exit WORKER 7
+    exit WORKER 13
+    exit WORKER 1
+    exit WORKER 9
+    
     --- Result for [CFHHILORRS]---
     
      rohrschilf
     
      schilfrohr
 
     --- END ---
 
-	Processes are down.
+    Processes are down.
     BF Time in sec: 12
     
     Process finished with exit code 0
 
-    Inbuild example, assert a scrambled string. Use brute force or condensing.
+
+Brute Force
     We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
-    (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
-        Permutation lists grow very fast, reaching Terabyte size.
-    (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
-
-`eisenmp` uses Pythons permutation generator
- [itertools](https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations)
-for the brute force attack example.
 
-    Another example downloads a large list and calculates average for one column.
+    len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
+    Permutation lists grow very fast, reaching Terabyte size.
+
+    len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
+
+Web download a large list
+    Calculates the average for one column.
     Python CSV extracts the column and we calculate the average with the assigned number
     of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
 
 
-- large lists https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©. 
-All material Stats NZ produces is protected by Crown copyright.
-Creative Commons Attribution 4.0 International licence.
-- German dict https://sourceforge.net/projects/germandict/. License Public Domain
-- English dict Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-- ORM Flask-SQLAlchemy https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
+large lists
+    https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©.
+    All material Stats NZ produces is protected by Crown copyright.
+    Creative Commons Attribution 4.0 International licence.
+
+German dict
+    https://sourceforge.net/projects/germandict/. License Public Domain
+
+English dict
+    Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
+
+ORM Flask-SQLAlchemy
+     https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
 
 Cheers
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/cmd.py` & `eisenmp_examples-0.5.0/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/database.db` & `eisenmp_examples-0.5.0/eisenmp_examples/database.db`

 * *Files 26% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -9,18 +9,19 @@
 	UNIQUE (username), 
 	UNIQUE (email)
 );
 INSERT INTO users VALUES(1,'pi','pi@pipapo.org','ceo');
 INSERT INTO users VALUES(2,'pa','pa@pipapo.org','chief');
 INSERT INTO users VALUES(3,'po','po@pipapo.org','leader');
 INSERT INTO users VALUES(4,'dave mops','dave.mops@pipapo.org','devops');
-INSERT INTO users VALUES(5,'foo','foo@pipapo.org','Data Entry');
 CREATE TABLE internal_use (
 	id INTEGER NOT NULL, 
 	browser_open INTEGER, 
 	statistics VARCHAR, 
 	commercials VARCHAR, 
 	PRIMARY KEY (id)
 );
 INSERT INTO internal_use VALUES(1,1,'98.6','sold');
 INSERT INTO internal_use VALUES(2,0,'70.2','bid');
+INSERT INTO internal_use VALUES(3,0,'67.4','offer');
+INSERT INTO internal_use VALUES(4,1,NULL,'bid');
 COMMIT;
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 
 Mandatory:
 - import eisenmp
 - worker must have the 'toolbox' (kwargs) as arg in entry function (arg count 1)
 - path to worker module and the entry function reference, all are str
 
 """
+import math
 import os
 import io
 import time
 from zipfile import ZipFile
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 try:
     from eisenmp.utils_exa.eisenmp_search import SearchStr
     from eisenmp.utils_exa.eisenmp_download import DownLoad
+    import eisenmp.utils_exa.eisenmp_utils as utils_exa
 except ImportError:
-    import eisenmp_examples
     from eisenmp_examples.utils_exa.eisenmp_search import SearchStr
     from eisenmp_examples.utils_exa.eisenmp_download import DownLoad
+    import eisenmp_examples.utils_exa.eisenmp_utils as utils_exa
 
 dir_name = os.path.dirname(__file__)  # absolute dir path
 
 
 class ModuleConfiguration:
     """
-    - Loading the worker module has nothing to do with name resolution in 'this' module.
-    We can load from network share.
+    | Loading the worker module has nothing to do with name resolution in 'this' module.
+    | We can load from network share.
 
-    We have full access to all queues and methods. eisenmp = eisenmp.Mp()
+    | We have full access to all queues and methods. eisenmp = eisenmp.Mp()
+    | We can transfer as much variable values to the worker as we want. Smaller is better. Spawn start copies values.
 
     """
     # path to worker module and entry function reference, worker module import in [isolated] process environment
     # -------------------- MANDATORY WORKER STRINGS (large worker live in /worker) --------------------
     bruteforce_module = {
         'worker_path': os.path.join(dir_name, 'worker', 'eisenmp_exa_wrk_bf_bruteforce.py'),
         'worker_ref': 'worker_entrance',
@@ -57,46 +60,50 @@
     }
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = []  # this example sets it later in `worker_module_set`
 
         # Multiprocess vars - override default
-        # self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
-        # self.NUM_ROWS = 2  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        # self.PROCS_MAX = 2  # your process count, default is None: one proc/CPU core
+        # self.ROWS_MAX = 50_000  # your workload spread, list (generator) to calc in one loop, default None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # Worker part - toolbox vars survive multiple worker calls
         self.multi_tool_get = None  # custom var to allow only one download of MULTI_TOOL; init later in this example
         self.MULTI_TOOL = None  # pre-defined toolbox.MULTI_TOOL can host the dict from mp_tools_q
-        self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
+
+        # self.INFO_ENABLE = True  # info thread collects list row count, makes sense if no instances start overlapped
+        # self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
 
         # custom
         self.use_file_system = False  # False: download and unzip in mem        ------------ SWITCH --------------------
         self.result_lbl = None  # set by caller
         self.num_lists = 0  # add one for each list done, print out worker
         self.lowercase = True
         self.url = None  # 'use_file_system' False, URL of csv file
         self.zipped_filename = None  # None: have to loop over two archives; name of the uncompressed file in zip arch.
         self.str_permutation = None  # the search string we want to find in the dictionary/wordlist
+        # instance creation overlaps if shrink on; info thread dev needs full length wordlist and sequence on mp_info_q
+        self.shrink_wordlist = False   # shrink wordlist to len(search_str) is much faster
 
 
 modConf = ModuleConfiguration()  # accessible in module
 searchStr = SearchStr()
 
 
 def load_lang_word_dict():
     """Load dictionaries from disk or gitHub"""
     word_dicts_file_system_load() if modConf.use_file_system else word_dicts_git_hub_load()
 
 
-def mp_start_raid():
+def start_raid():
     """
     - Manager -
 
     Decide raid tactics.
     Brute force on smaller strings. List reduce attempt for larger strings.
 
     Grab config values and push it to the two possible functions.
@@ -105,35 +112,59 @@
     - (B) len(String) >=  11, Reduce a dictionary len(str) condensed list and count characters.
 
     See `mp_brute_force` and `mp_reduce` for more info.
     """
     modConf.str_permutation = searchStr.search_string
     if modConf.lowercase:
         modConf.str_permutation = modConf.str_permutation.lower()
-    searchStr.create_key_word_val_none_shrink(lowercase=modConf.lowercase)  # dict, remove words != len(search str)
-    modConf.INFO_THREAD_MAX = len(searchStr.words_dict)  # info thread calc rows done and len
+
+    shrink = True if modConf.shrink_wordlist else False
+    searchStr.word_dict_size(shrink, lowercase=modConf.lowercase)  # shrink remove words != len(search str)
+    modConf.INFO_THREAD_MAX = math.factorial(len(modConf.str_permutation))  # info thread calc rows done and len
 
     # ---------- selection of generator function reference, no () ----------
     brute_force = True if len(modConf.str_permutation) <= 10 else False
     function_ref = mp_brute_force if brute_force else mp_reduce  # decide which function to call
     worker_module_set(function_ref)
 
     msg_b, msg_r = f'\n\t[BRUTE_FORCE]\t{modConf.str_permutation}', f'\n\t[LIST_REDUCTION]\t{modConf.str_permutation}'
     msg = msg_b if function_ref == mp_brute_force else msg_r
     print(msg)
 
     generator = function_ref(searchStr)  # `mp_brute_force` or `mp_reduce`
     words_dict = searchStr.words_dict if function_ref == mp_brute_force else None
 
-    mP = eisenmp.Mp()
-    mP.start(**modConf.__dict__)
+    emp = eisenmp.Mp()
+    emp.start(**modConf.__dict__)
+
     if brute_force:
-        for _ in mP.proc_list:
-            mP.mp_tools_q.put(words_dict)
-    mP.run_q_feeder(generator=generator, input_q=mP.mp_input_q)
+        for _ in emp.proc_list:
+            emp.mp_tools_q.put(words_dict)
+    emp.run_q_feeder(generator=generator, input_q=emp.mp_input_q)
+    return emp
+
+
+def rt_loader():
+    """rainbow table
+    test if dict is only hosted in parent proc, if spawn
+    """
+    file_bin = bytearray()
+    i = 0
+    with open(r'f:\w.iso', 'rb') as bin_reader:
+        while 1:
+            if not (i % 100):
+                print('.', end="", flush=True)
+            chunk = bin_reader.read(io.DEFAULT_BUFFER_SIZE)
+            if not chunk:
+                print('\n')
+                break
+            file_bin += chunk
+            i += 1
+    rt_dct = {'rt': file_bin}
+    return rt_dct
 
 
 def worker_module_set(function_ref):
     """which worker module and function to load"""
     modConf.worker_modules = []  # del existing
 
     if function_ref == mp_brute_force:
@@ -207,14 +238,15 @@
         modConf.zipped_filename = in_zip
         wordlist_download(downloader)  # stored the response object
         mem_word_lst.extend(wordlists_in_memory(downloader))  # download the zip archive, open one file, return txt file
 
     if modConf.lowercase:  # store the word list in searchStr instance with lowercase if set {'ethic': None}
         # .rstrip() else single chars, later in shrink method of searchStr
         searchStr.loader_words_dict = {word.lower().rstrip(): None for word in mem_word_lst}
+        pass
     else:
         searchStr.loader_words_dict = {word.rstrip(): None for word in mem_word_lst}
     pass
 
 
 def wordlists_in_memory(downloader):
     """Open zip archive and load one file 'zipped_filename'
@@ -233,38 +265,58 @@
     """
     downloader.url = modConf.url
     downloader.zipped_filename = modConf.zipped_filename
     print(downloader.url)
     downloader.load_url()
 
 
+def start_raid_sequential():
+    """Blocks creation of a new instance,
+    else next instance starts while previous instances runs
+    """
+    emp = start_raid()
+    while 1:
+        if emp.begin_proc_shutdown:
+            break
+        time.sleep(.1)
+
+
 def main():
     """
     """
     str_list_alphabet_salad = [
         'AMGNO',
         'AACEFHKLMSS',
         'DIKKLOOR', 'BEEINNRST',
         'CEEHNNRST', 'EEHINORST',
         'EEEFFIKORRS', 'CFHHILORRS'
     ]
 
     start = time.perf_counter()
 
-    res_coll_dct = {}
+    utils_exa.empty_db_from_schema()  # collect exit msg (search string alphabet) from instances
     load_lang_word_dict()
+    msg_result = e_utils.Result.result_dict  # shown in browser if example server is started
+
     for idx, string in enumerate(str_list_alphabet_salad):
         searchStr.search_string = string
         modConf.result_lbl = string
         modConf.lowercase = True
-        mp_start_raid()
-        msg_result = e_utils.Result.result_dict
-        res_coll_dct[idx] = msg_result
-        print(msg_result)
-        time.sleep(.5)
 
-    print(f'BF Time in sec: {round((time.perf_counter() - start))}')
-    return res_coll_dct
+        modConf.shrink_wordlist = True  # either start_raid or start_raid_sequential
+        start_raid() if modConf.shrink_wordlist else start_raid_sequential()  # else block instantiate
+
+    while 1:
+        # need a database for asking done; some instances may return earlier than other
+        title_lst = utils_exa.table_select_column('exa', 'title')
+        done = all(item in title_lst for item in str_list_alphabet_salad)
+
+        if done:
+            break
+        time.sleep(1)
+
+    print(f'bruteforce time: {round((time.perf_counter() - start))}')
+    return msg_result
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_double_q.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_double_q.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 - fake production of audio and video coding, is loop through to result dict
 - two processors work on different streams, batches, (src is same here, so what)
 
 """
 import os
 import threading
 import time
-import platform
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 dir_name = os.path.dirname(__file__)
 
 
 chunks_0 = [
@@ -74,23 +73,23 @@
     }
     watchdog_module = {
         'WORKER_PATH': os.path.join(os.path.dirname(dir_name), 'worker', 'eisenmp_exa_wrk_watchdog.py'),
         'WORKER_REF': 'mp_start_show_threads',
     }
 
     def __init__(self):
-        super().__init__()
+
         self.worker_modules = [  # in-bld-res
             self.template_module,  # other modules must start threaded, else we hang
-            self.watchdog_module  # second; thread function call mandatory, last module loaded first
+            # self.watchdog_module  # second; thread function call mandatory, last module loaded first
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 2  # your process count, each 'batch' on one CPU core, default is None: one proc/CPU core
-        self.NUM_ROWS = 3  # arbitrary num here
+        self.PROCS_MAX = 2  # your process count, each 'batch' on one CPU core, default is None: one proc/CPU core
+        self.ROWS_MAX = 3  # arbitrary num here
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULT_LABEL = 'fake production of audio and video for WHO studios'  # RESULT_LABEL for RESULTS_PRINT
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # work to do
@@ -115,34 +114,34 @@
     Divide workload between processes / CPU
     -
     """
     q_cat_name_maxsize = [
         # q_category, q_name, q_maxsize; find your 100 Queues in the debugger, toolbox
         ('batch_1', 'audio_lg', 5),  # queues for batch_1
         ('batch_1', 'video_in', 1),  # dict avail. in worker module: toolbox.batch_1['video_in'].get()
-        ('batch_7', 'audio_lg', 3),  # queues for batch_7, created but not used so far, can play with
+        ('batch_7', 'audio_lg', 3),  # queues for batch_7
         ('batch_7', 'video_in', 1)
     ]
-    mP = eisenmp.Mp()
+    emp = eisenmp.Mp()
 
     # create custom queues with category and name
-    mP.queue_cust_dict_category_create(*q_cat_name_maxsize)  # create queues, store in {custom} {category} dict
+    emp.queue_cust_dict_category_create(*q_cat_name_maxsize)  # create queues, store in {custom} {category} dict
 
-    audio_q_b1 = mP.queue_cust_dict_cat['batch_1']['audio_lg']  # USE Queue:
-    video_q_b1 = mP.queue_cust_dict_cat['batch_1']['video_in']  # worker module: toolbox.batch_1['video_in'].get()
-    audio_q_b7 = mP.queue_cust_dict_cat['batch_7']['audio_lg']
-    video_q_b7 = mP.queue_cust_dict_cat['batch_7']['video_in']  # toolbox.batch_7['video_in'].get()
-
-    mP.start(**modConf.__dict__)  # create processes, load worker mods, start threads (output_p coll, info)
-    mP.run_q_feeder(generator=audio_generator_batch_1(), input_q=audio_q_b1)
-    mP.run_q_feeder(generator=video_generator_batch_1(), input_q=video_q_b1)
-    mP.run_q_feeder(generator=audio_generator_batch_7(), input_q=audio_q_b7)
-    mP.run_q_feeder(generator=video_generator_batch_7(), input_q=video_q_b7)
+    audio_q_b1 = emp.queue_cust_dict_cat['batch_1']['audio_lg']  # USE Queue:
+    video_q_b1 = emp.queue_cust_dict_cat['batch_1']['video_in']  # worker module: toolbox.batch_1['video_in'].get()
+    audio_q_b7 = emp.queue_cust_dict_cat['batch_7']['audio_lg']
+    video_q_b7 = emp.queue_cust_dict_cat['batch_7']['video_in']  # toolbox.batch_7['video_in'].get()
+
+    emp.start(**modConf.__dict__)  # create processes, load worker mods, start threads (output_p coll, info)
+    emp.run_q_feeder(generator=audio_generator_batch_1(), input_q=audio_q_b1)
+    emp.run_q_feeder(generator=video_generator_batch_1(), input_q=video_q_b1)
+    emp.run_q_feeder(generator=audio_generator_batch_7(), input_q=audio_q_b7)
+    emp.run_q_feeder(generator=video_generator_batch_7(), input_q=video_q_b7)
 
-    return mP
+    return emp
 
 
 def audio_generator_batch_1():
     """"""
     for _ in chunks_0:
         yield _
 
@@ -166,18 +165,18 @@
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
-    mP = manager_entry()
+    emp = manager_entry()
     while 1:
         # running threads, wait
-        if mP.begin_proc_shutdown:
+        if emp.begin_proc_shutdown:
             break
         time.sleep(1)
 
     msg_time = 'Fake production, Time in sec: ', round((time.perf_counter() - start))
     print(msg_time)
     msg_result = e_utils.Result.result_dict
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     foo = {'WORKER_PATH': 'bar', 'WORKER_REF': 'baz'}
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = [self.first_module]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 6  # your process count, default is None: one proc/CPU core
-        self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
+        self.PROCS_MAX = 6  # your process count, default is None: one proc/CPU core
+        self.ROWS_MAX = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULT_LABEL = 'No result, server blocks'  # pretty print as result header for RESULTS_PRINT
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
 
@@ -49,26 +49,26 @@
     # need a Queue for yellow and blue and an `existing` Database with numbers or generator range step
     q_name_maxsize = [
         # q_name, q_maxsize;
         ('mp_blue_q', 1),  # tuple, worker: toolbox.mp_blue_q.get()
         ('mp_yellow_q', 1)
     ]
     # default call
-    mP = eisenmp.Mp()
+    emp = eisenmp.Mp()
 
     # custom queues for port groups ---> need a generator for each queue
-    mP.queue_cust_dict_std_create(*q_name_maxsize)  # unpack, create Qs in std {default} dict ..['mp_blue_q']=Queue()
+    emp.queue_cust_dict_std_create(*q_name_maxsize)  # unpack, create Qs in std {default} dict ..['mp_blue_q']=Queue()
 
     port_blue = (port_number for port_number in range(13_000, 13_006, 2))
     port_yellow = (port_number for port_number in range(14_000, 14_006, 2))
 
     # !!! config write instance dictionary if all args set !!!
-    mP.start(**modConf.__dict__)  # feed toolbox, instance attributes available for worker and feeder loop
-    mP.run_q_feeder(generator=port_blue, input_q=mP.queue_cust_dict_std['mp_blue_q'])
-    mP.run_q_feeder(generator=port_yellow, input_q=mP.queue_cust_dict_std['mp_yellow_q'])
+    emp.start(**modConf.__dict__)  # feed toolbox, instance attributes available for worker and feeder loop
+    emp.run_q_feeder(generator=port_blue, input_q=emp.queue_cust_dict_std['mp_blue_q'])
+    emp.run_q_feeder(generator=port_yellow, input_q=emp.queue_cust_dict_std['mp_yellow_q'])
 
 
 def main():
     """
     """
     start = time.perf_counter()
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,100 +4,104 @@
 import os
 
 import json
 import time
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
 try:
-    import eisenmp
     import eisenmp.eisenmp_exa_multi_srv_each_cpu as multi_on_each_cpu
     import eisenmp.eisenmp_exa_each_flask_orm_srv_one_cpu as single_on_each_cpu
     import eisenmp.eisenmp_exa_prime as prime
     import eisenmp.eisenmp_exa_web_csv as web_csv
     import eisenmp.eisenmp_exa_http as http_srv
     import eisenmp.eisenmp_exa_double_q as double_q
     import eisenmp.eisenmp_exa_bruteforce as bruteforce
 
 except ImportError:
-    import eisenmp_examples
     import eisenmp_examples.eisenmp_exa_multi_srv_each_cpu as multi_on_each_cpu
     import eisenmp_examples.eisenmp_exa_each_flask_orm_srv_one_cpu as single_on_each_cpu
     import eisenmp_examples.eisenmp_exa_prime as prime
     import eisenmp_examples.eisenmp_exa_web_csv as web_csv
     import eisenmp_examples.eisenmp_exa_http as http_srv
     import eisenmp_examples.eisenmp_exa_double_q as double_q
     import eisenmp_examples.eisenmp_exa_bruteforce as bruteforce
 
 hostName = "localhost"
-serverPort = 12_321
+serverPort = 12321
 dir_name = os.path.dirname(__file__)
+os.environ['EXA_ENTRY_KILL'] = 'False'
 
 
 class Menu:
     example_menu = [
         'Multiple server in each process/CPU core - share a port range - share a DB. Worker Green, Yellow and Blue',
         'Prime Number calculation',
         'Every Flask server in a different process - share a port range - share a DB. Worker Yellow and Blue',
         'Web CSV large list. Average for each chunk of a large list column to simply calc the results later.',
         'One simple http server presents a radio on every process. "Unemployed" worker exit.',
         'Each process has two Queues feed audio and video. Merge in a fake production.',
         'Brute force attack with dictionary and itertools generator'
     ]
 
     exa_tpl_lst = [
-        (0, example_menu[0], multi_on_each_cpu.main),
-        (1, example_menu[1], prime.main),
-        (2, example_menu[2], single_on_each_cpu.main),
-        (3, example_menu[3], web_csv.main),
-        (4, example_menu[4], http_srv.main),
-        (5, example_menu[5], double_q.main),
-        (6, example_menu[6], bruteforce.main)
+        # idx, text,        , func                  , kill blocking - option
+        (0, example_menu[0], multi_on_each_cpu.main, 'True'),
+        (1, example_menu[1], prime.main, 'False'),
+        (2, example_menu[2], single_on_each_cpu.main, 'True'),
+        (3, example_menu[3], web_csv.main, 'False'),
+        (4, example_menu[4], http_srv.main, 'True'),
+        (5, example_menu[5], double_q.main, 'False'),
+        (6, example_menu[6], bruteforce.main, 'False')
     ]
 
 
-def run_http():
+def run_http(com_queue):
     """Blocked, no loop here
     """
     global serverPort
 
     while 1:
         try:
             webServer = HTTPServer((hostName, serverPort), MyServer)
             break
         except OSError:
-            print(f'serverPort in use {serverPort}\n\tadd one to port number')
+            print(f'serverPort in use {serverPort}')
+            print('\n\tadd one to port number')
             serverPort += 1  # port already in use
 
-    print(f"Examples http://%s:%s" % (hostName, serverPort))
+    print("Examples http://%s:%s" % (hostName, serverPort))
+
+    com_queue.put(b'ready')
     try:
         webServer.serve_forever()
     except KeyboardInterrupt:
         pass
     webServer.server_close()
     print("Server stopped.")
 
 
 class MyServer(BaseHTTPRequestHandler):
 
     def do_POST(self):
         """"""
         # print(self.headers)
         length = int(self.headers.get_all('content-length')[0])
-        print(self.headers.get_all('content-length'))
+        print('content-length is ', self.headers.get_all('content-length'))
         data_string = self.rfile.read(length)
-        example_fun = Menu.exa_tpl_lst[int(data_string)][2]
+        example_fun = Menu.exa_tpl_lst[int(data_string)][2]  # now run desired example
         ret_val = example_fun()
-        # print(data_string)
+        print(data_string)
         self.send_response(200)
         # self.send_header("Content-type", "text/plain")
         self.send_header('Content-Type', 'application/json')
         self.end_headers()
         self.flush_headers()
         json_string = json.dumps(str(ret_val))
         self.wfile.write(bytes(json_string, "utf-8"))
+
         return True
 
     def do_GET(self):
         self.send_response(200)
         self.send_header("Content-type", "text/html")
         self.end_headers()
 
@@ -115,26 +119,26 @@
 
             "body{font-family:PT Sans, arial; color:black;background-color:#ccc;}",
             "h1 {color:brown;text-align:center;}",
             ".container {display: flex;}",
             ".middle {display: flex;flex-direction: column;margin: auto;color:brown;}",
             ".pMid {color: black; text-align:center;}",
             "</style>",
-            f"<title>Examples</title>",
+            "<title>Examples</title>",
             "</head>",
 
             "<body>",
-            f"<h1> Welcome to eisenmp_examples</h1>",
-            f"<p class=pMid> Examples run in the terminal window. </p>",
-            f"<div class='container'>",
-            f"<div class='middle'>",
+            "<h1> Welcome to eisenmp_examples</h1>",
+            "<p class=pMid> Examples run in the terminal window. </p>",
+            "<div class='container'>",
+            "<div class='middle'>",
             '_o__example_buttons____',
             "</div></div>",
             "send: <p id=pRspReturn class=pInOut> </p>",
-            f"resp: <p id=pMsg class=pInOut> </p>",
+            "resp: <p id=pMsg class=pInOut> </p>",
             "</body></html>",
 
             "<script>",
             "function getExa(radio_btn_id) {",
             "document.getElementById('pMsg').innerHTML='';",
             "const xhr = new XMLHttpRequest();",
             "xhr.open('POST', '/');",
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = [
             self.first_module,  # second module must be threaded, else we hang
             # self.watchdog_module,  # enable for threaded module start live example
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 16  # your process count, default is None: one proc/CPU core
-        self.NUM_ROWS = 1  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        self.PROCS_MAX = 16  # your process count, default is None: one proc/CPU core
+        self.ROWS_MAX = 1  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # 'not enough work example', useless worker auto shutdown, the modules return False
@@ -78,28 +78,28 @@
 
 def manager_http_srv():
     """
     - Manager -
 
     """
     # default call feeds all variables of 'ModuleConfiguration' in kwargs -> toolbox of worker
-    mP = eisenmp.Mp()
-    mP.start(**modConf.__dict__)  # instance attributes available for worker and feeder loop
+    emp = eisenmp.Mp()
+    emp.start(**modConf.__dict__)  # instance attributes available for worker and feeder loop
     # custom, don't need a generator and q feeder to run a server
     generator = (radio_url for radio_url in radio_url_lst)
-    mP.run_q_feeder(generator=generator)
+    emp.run_q_feeder(generator=generator)
 
 
 def worker_http(toolbox):  # arg for loader, all ModuleConfiguration instance vars can be pulled from toolbox
     """
     - Worker -
 
     Blocked, no loop here
     toolbox is the all-in-one box for vars and queues. incl. ModuleConfiguration
-    We have num_procs, we have ports to add, we need worker in groups to serve ports
+    We have PROCS_MAX, we have ports to add, we need worker in groups to serve ports
     """
     global serverPort
 
     WORKER_ID = toolbox.WORKER_ID
     serverPort = serverPort + WORKER_ID
     while 1:
         toolbox.next_lst = toolbox.mp_input_q.get()
@@ -136,15 +136,15 @@
         self.wfile.write(bytes("initial-scale=1, shrink-to-fit=no'/>", "utf-8"))
         self.wfile.write(bytes("<link rel=stylesheet href=https://fonts.googleapis.com/css?family=Roboto/>", "utf-8"))
         self.wfile.write(bytes("<title>https://pythonbasics.org</title>", "utf-8"))
         self.wfile.write(bytes("</head>", "utf-8"))
         self.wfile.write(bytes("<p>Request: %s</p>" % self.path, "utf-8"))
         self.wfile.write(bytes("<body>", "utf-8"))
         self.wfile.write(bytes("<h1 style='text-align:center;color:brown;font-family:Roboto;'> Server </h1> ", "utf-8"))
-        self.wfile.write(bytes(f"<p style='text-align:center;color:brown;font-family:Roboto;'>", "utf-8"))
+        self.wfile.write(bytes("<p style='text-align:center;color:brown;font-family:Roboto;'>", "utf-8"))
         self.wfile.write(bytes("Visit 44xtc44 on PyPi or SnapCraft.io, EisenRadio ,", "utf-8"))
         self.wfile.write(bytes("<a href=https://pypi.org/project/eisenradio/>link</a>", "utf-8"))
         self.wfile.write(bytes(" for a better Show, ", "utf-8"))
         self.wfile.write(bytes("Blacklist, recording and a 'Gain' slider\t", "utf-8"))
         self.wfile.write(bytes(f"\t{self.toolbox.radio_name}\n", "utf-8"))
         self.wfile.write(bytes(f"\t{self.toolbox.radio_url} <a href={self.toolbox.radio_url}>link</a>\n", "utf-8"))
         self.wfile.write(bytes("<hr>", "utf-8"))
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 it's always the same process,
 you extend or switch off defaults
 
 
 Multiple server on each CPU core, if server has that many cores.
 needs Flask_SQLAlchemy_Project_Template >=1.3
 
-module_loader mod of eisenmp must be informed, STOP_MSG_DISABLE=True.
 All worker are thread started -> and can not send 'return False' (run_forever()),
 no stop confirmation of module_loader mod of eisenmp avail
 """
 import os
 import time
 
 import eisenmp
@@ -38,23 +37,21 @@
             self.first_module,  # each module_loader in the process loads this list
             self.first_module,
             self.first_module,
             self.first_module,  # just demo, same can be achieved if server called in a worker loop
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 3  # your process count, default is None: one proc/CPU core
-        self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
+        self.PROCS_MAX = 3  # your process count, default is None: one proc/CPU core
+        self.ROWS_MAX = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
-        self.STOP_MSG_DISABLE = True  # module_loader leaves worker loop and waits for stop msg in mp_process_q
-
         # worker port groups, nailed on one cpu
         self.blue_lst = [0]  # one CPU core for blue list, if toolbox.kwargs['START_SEQUENCE_NUM'] in worker_blue_lst,
         self.yellow_lst = [1]  # one CPU core for yellow, process spawn num 1; (class ProcEnv 'run_proc -> core')
         self.green_lst = [2]
 
 
 modConf = ModuleConfiguration()  # Accessible in the module.
@@ -73,37 +70,39 @@
     q_name_maxsize = [
         # q_name, q_maxsize;
         ('mp_blue_q', 1),  # tuple, worker: toolbox.mp_blue_q.get()
         ('mp_yellow_q', 1),
         ('mp_green_q', 1)
     ]
     # default call
-    mP = eisenmp.Mp()
+    emp = eisenmp.Mp()
 
     # custom queues for port groups ---> need a generator for each queue
-    mP.queue_cust_dict_std_create(*q_name_maxsize)  # unpack, create Qs in std {default} dict ..['mp_blue_q']=Queue()
+    emp.queue_cust_dict_std_create(*q_name_maxsize)  # unpack, create Qs in std {default} dict ..['mp_blue_q']=Queue()
 
     # !!! config write instance dictionary if all args set !!!
-    mP.start(**modConf.__dict__)  # feed toolbox, instance attributes available for worker and feeder loop
+    emp.start(**modConf.__dict__)  # feed toolbox, instance attributes available for worker and feeder loop
 
     port_generator_blue = (port_number for port_number in range(11_000, 11_006, 1))
     port_generator_yellow = (port_number for port_number in range(14_000, 14_006, 1))
     port_generator_green = (port_number for port_number in range(15_000, 15_006, 1))
-    mP.run_q_feeder(generator=port_generator_blue, input_q=mP.queue_cust_dict_std['mp_blue_q'])
-    mP.run_q_feeder(generator=port_generator_yellow, input_q=mP.queue_cust_dict_std['mp_yellow_q'])
-    mP.run_q_feeder(generator=port_generator_green, input_q=mP.queue_cust_dict_std['mp_green_q'])
+    emp.run_q_feeder(generator=port_generator_blue, input_q=emp.queue_cust_dict_std['mp_blue_q'])
+    emp.run_q_feeder(generator=port_generator_yellow, input_q=emp.queue_cust_dict_std['mp_yellow_q'])
+    emp.run_q_feeder(generator=port_generator_green, input_q=emp.queue_cust_dict_std['mp_green_q'])
+    return emp
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
     manager()
 
     msg_time = f'\nMulti loader Time in sec: {round((time.perf_counter() - start))} - main() exits'
     print(msg_time)
-    return msg_time
+
+    return
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_prime.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,45 +36,45 @@
         # load order list, first module is called in an endless loop
         self.worker_modules = [
             self.first_module,   # second module must be threaded, else we hang
             # foo
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
-        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
-        self.NUM_ROWS = 42  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        # self.PROCS_MAX = 5  # your process count, default is None: one proc/CPU core
+        # max generator / ROWS_MAX = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
+        self.ROWS_MAX = 42  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # custom part, write your own Attributes
-        self.range_num = 10 ** 4  # got a target/max value and NUM_ROWS for each proc, can calc ETA est. time arrival
+        self.range_num = 10 ** 4  # got a target/max value and ROWS_MAX for each proc, can calc ETA est. time arrival
         self.INFO_THREAD_MAX = self.range_num  # target value for info thread to calculate % and ETA
         # self.INFO_ENABLE = True  # [baustelle]
         self.n = 10 ** 12  # ten with zero count, 10_000_000_000_000_000
         self.say_hello = 'Hello'  # just to show that worker can [read] all attributes of instance, in 'worker_prime()'
 
 
 modConf = ModuleConfiguration()  # Accessible in the module.
 
 
 def generator_prime():
     """Manager - One time execution.
     Exits if generator is empty.
     """
     # auto
-    mP = eisenmp.Mp()
+    emp = eisenmp.Mp()
 
-    mP.start(**modConf.__dict__)  # instance attributes available for worker and feeder loop
+    emp.start(**modConf.__dict__)  # instance attributes available for worker and feeder loop
     generator = number_generator()
-    mP.run_q_feeder(generator=generator, input_q=mP.mp_input_q)  # here default mp_input_q, use if only one q needed
+    emp.run_q_feeder(generator=generator, input_q=emp.mp_input_q)  # here default mp_input_q, use if only one q needed
 
-    return mP
+    return emp
 
 
 def number_generator():
     """Generates numbers from start count.
     Has an end value, range.
     """
     range_num = modConf.range_num
@@ -186,20 +186,20 @@
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
-    mP = generator_prime()
+    emp = generator_prime()
 
     while 1:
         # running generator threads and procs,
-        # keep main() alive, else procs end, and we can not access results
-        if mP.begin_proc_shutdown:
+        # keep main() alive, else we can not access results
+        if emp.begin_proc_shutdown:
             break
         time.sleep(1)
 
     msg_time = 'Example Prime numbers, Time in sec: ', round((time.perf_counter() - start))
     print(msg_time)
     msg_result = e_utils.Result.result_dict
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_web_csv.py` & `eisenmp_examples-0.5.0/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
         self.worker_modules = [
             self.first_module,  # second module must be started by a thread, else we hang
             self.watchdog_module,
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
-        # max generator / NUM_ROWS = number of tickets; 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
-        self.NUM_ROWS = 50_000  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
+        self.PROCS_MAX = 5  # your process count, default is None: one proc/CPU core
+        # max generator / ROWS_MAX = number of tickets; 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
+        self.ROWS_MAX = 50_000  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
         # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # CSV part
@@ -76,28 +76,28 @@
     Generator part of calc CSV. Worker module in /worker folder.
 
     :params: result_lbl: find result in a list; sum findings, mandatory
     :params: use_file_system: True 'use_file_system'; False: in mem unzip
     :params: url: dl_url, if not 'use_file_system', URL of csv file
     :params: zipped_filename: 'revised.csv',  name of the uncompressed file in zip archive
     :params: csv_col_name: 'value',  # table column header name, mandatory
-    :params: 'num_rows': num list rows to calc in one loop for each process
+    :params: 'ROWS_MAX': num list rows to calc in one loop for each process
     :params: 'num_proc': procs to start, can be more or less than system CPU core count
     """
-    mP = eisenmp.Mp()
-    mP.start(**modConf.__dict__)  # thread & processes start, attributes avail. for worker and feeder loop
-    mP.mp_print_q.put('\tDownload large list')
-    mP.mp_print_q.put(modConf.dl_url)
+    emp = eisenmp.Mp()
+    emp.start(**modConf.__dict__)  # thread & processes start, attributes avail. for worker and feeder loop
+    emp.mp_print_q.put('\tDownload large list')
+    emp.mp_print_q.put(modConf.dl_url)
 
     report_file = os.path.join(dir_name, 'download', 'report.zip')
-    downloader = download_report_zip_archive(mP, report_file)  # and prn msg
+    downloader = download_report_zip_archive(emp, report_file)  # and prn msg
     generator = g_use_fs_csv(report_file) if modConf.use_file_system else g_in_mem_csv(downloader)  # CSV generator
-    mP.run_q_feeder(generator=generator)
+    emp.run_q_feeder(generator=generator)
 
-    return mP
+    return emp
 
 
 def g_in_mem_csv(downloader):
     """
     """
     archive = downloader.unzip_mem()
     in_file = archive.open(modConf.zipped_filename, 'r')
@@ -108,31 +108,30 @@
 
 def g_use_fs_csv(report_file):
     """
     """
     file_path = os.path.join(os.path.dirname(report_file), modConf.zipped_filename)
     filename = open(file_path, 'r')
     dict_reader = csv.DictReader(filename)
-    
     generator = (column[modConf.csv_col_name] for column in dict_reader)
     return generator
 
 
 def unzip_on_file_system(downloader, report_f):
     """
     """
     downloader.save(report_f)
     with ZipFile(report_f, 'r') as un_zip:
         un_zip.extractall(os.path.dirname(report_f))
 
 
-def download_report_zip_archive(mP, report_file):
+def download_report_zip_archive(emp, report_file):
     """
     """
-    mP.mp_print_q.put(origin_msg_create())
+    emp.mp_print_q.put(origin_msg_create())
     downloader = DownLoad()
     downloader.url = modConf.url
     downloader.zipped_filename = modConf.zipped_filename
     downloader.load_url()  # now decide to read csv from mem or file
     if modConf.use_file_system:
         unzip_on_file_system(downloader, report_file)  # comment no dl
     return downloader
@@ -150,18 +149,18 @@
 
 
 def main():
     """
     """
     start = time.perf_counter()
 
-    mP = generator_calc_csv()
+    emp = generator_calc_csv()
     while 1:
         # running threads, wait
-        if mP.begin_proc_shutdown:
+        if emp.begin_proc_shutdown:
             break
         time.sleep(1)
 
     print(f'Time in sec: {round((time.perf_counter() - start))}')
 
     msg_result = e_utils.Result.result_dict
     return msg_result
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_download.py` & `eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,8 +65,7 @@
                 break
             self.file_bin += chunk
             i += 1
 
 
 if __name__ == '__main__':
     pass
-
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_utils.py` & `eisenmp_examples-0.5.0/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import ssl
 import time
 import random
 import urllib
+import sqlite3
 import certifi
 import threading
 from hashlib import sha256
 from zipfile import ZipFile
 from urllib.request import urlopen, Request
 from collections import defaultdict
 
 
 os.environ['SSL_CERT_FILE'] = certifi.where()
 context_ssl = ssl.create_default_context(cafile=certifi.where())
+dir_name = os.path.dirname(__file__)  # absolute dir path
 
 agent_list = [   # agent orange or agent white
     'Mozilla/5.0 (iPad; CPU OS 8_4_1 like Mac OS X) AppleWebKit/600.1.4 (KHTML, like Gecko) '
     'Version/8.0 Mobile/12H321 Safari/600.1.4',
     'Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
     'Chrome/45.0.2454.85 Safari/537.36',
     'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
@@ -81,15 +83,15 @@
         if user_agent:
             opener.addheaders = [('User-agent', user_agent)]
         urllib.request.install_opener(opener)
         response = urlopen(request, timeout=15, context=context_ssl)
         return response
 
     except TimeoutError:
-        print(f'TimeoutError in load_url().')
+        print('TimeoutError in load_url().')
         return False
     except Exception as error:
         print(f'unknown error in load_url() {error}')
         return False
 
 
 def thread_shutdown_wait(*threads):
@@ -204,7 +206,56 @@
     elif 'Ö' in word:
         word = word.replace('Ö', 'OE')
     elif "'" in word:
         word = word.replace("'", '')
     else:
         pass
     return word
+
+
+def get_db_path(db_name='db_exa.db'):
+    return os.path.join(dir_name, db_name)
+
+
+def get_db_connection():
+
+    db = get_db_path()
+    conn = sqlite3.connect(str(db))
+    conn.row_factory = sqlite3.Row
+    return conn
+
+
+def table_insert(sql_statement, *args):
+    conn = get_db_connection()
+    cur = conn.cursor()
+    cur.execute(sql_statement, [*args])
+    conn.commit()
+    conn.close()
+
+
+def table_select_column(table, col):
+    conn = get_db_connection()
+    column = conn.execute('SELECT ' + col + ' FROM ' + table + ';')
+    rows = []
+    for row in column:
+        if row[col]:
+            rows.append(row[col])
+
+    conn.close()
+    return rows
+
+
+def empty_db_from_schema(db_name='db_exa.db', schema_file='db_exa_schema.sql'):
+    """Initial for bruteforce, instances return not sequential,
+    Caller exit is possible if last instance writes code word, to identify
+    database.db in root is from SQLAlchemy template package
+    """
+    conn = sqlite3.connect((str(os.path.join(dir_name, db_name))))
+
+    with open((os.path.join(dir_name, schema_file)), encoding='utf-8') as f:
+        conn.executescript(f.read())
+
+    cur = conn.cursor()
+    cur.execute("INSERT INTO exa (title,col_1,col_2,col_3,col_4,col_5,col_6) VALUES (?,?,?,?,?,?,?)",
+                ('init_tbl', 1, 2, 3, 4, 5, 6))
+    conn.commit()
+    conn.close()
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-"""Example 1 brute force
-
-eisenmp uses a list reducer module in example 2.
-Generated list rows from language dict are compared with chars.
-
-Vars and Queues stored in the toolbox instance.
-See documentation for a quick overview, please.
+"""Economy Example CSV column calculation.
 
 """
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
@@ -17,95 +11,84 @@
     We return True to get next list chunk, whatever object is in the rows.
     Fed from mp_input_q to our toolbox. toolbox is our work instance with queues,
     messages, list chunk, and work tools like language dictionary or hash list.
 
     toolbox.foo, gives also access to all attributes and values
     of the 'modConf.foo' instance, you have created
     """
-    if toolbox.multi_tool_get:
-        tool_get(toolbox)  # dict mp_tools_q
-    workload_get(toolbox)
-    busy = brute_force(toolbox)  # worker function
+    # toolbox.mp_print_q.put(toolbox.say_hello)
+    busy = workload_get(toolbox)
+    calc_average(toolbox)  # start worker function
     if not busy:
         return False
-    send_eta_data(toolbox)
+    send_eta_data(toolbox)  # send data list, first row is header, info thread can find it in eisenmp.output_q_box
     return True
 
 
-def tool_get(toolbox):
-    """"""
-    while 1:
-        if not toolbox.mp_tools_q.empty():
-            toolbox.multi_tool = toolbox.mp_tools_q.get()
-            toolbox.multi_tool_get = False  # can be set in modConf
-            break
-
-
 def workload_get(toolbox):
     """"""
     while 1:
         if not toolbox.mp_input_q.empty():
             toolbox.NEXT_LIST = toolbox.mp_input_q.get()
-            toolbox.num_lists += 1
             break
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
+        return False  # loop worker sends shutdown msg to next worker - generator is empty
+    return True
 
 
 def remove_header(toolbox):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
 
     Use self.header_msg attribute to overwrite default header string
     """
     # toolbox.mp_print_q.put(toolbox.NEXT_LIST[0])
     toolbox.INPUT_HEADER = toolbox.NEXT_LIST[0]
     del toolbox.NEXT_LIST[0]  # remove header str
 
 
-def send_output(toolbox, formatted_str):
+def calc_average(toolbox):
+    """Calc average from strings.
+    Pandas can make float, but we use raw Python csv import.
+    Table column has 'nan' and empty cells we can not read.
+    """
+    busy = True
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # inform we want exit
+        busy = False
+    remove_header(toolbox)
+
+    lst = toolbox.NEXT_LIST
+    STOP_MSG = toolbox.STOP_MSG
+    # kick out 'nan' string and binary stop message from list, stop message is appended on GhettoBoss iterator loop end
+    tbl_flt = [float(num) for num in lst if str(num) and 'nan' not in str(num) and num != STOP_MSG]
+
+    average = 0
+    if len(tbl_flt):  # calc with float type to get comma values
+        average = sum([num for num in tbl_flt]) / len(tbl_flt)
+    average = average if average else 0
+
+    send_output(toolbox, average)
+    return busy
+
+
+def send_output(toolbox, average):
     """Put your findings in the output list.
     Find results in the 'eisenmp_utils.Result.result_dict'
 
     :params: toolbox: -
     :params: average: average of the (chunk of) column
     """
     # header for output result list
     header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
     result_lst = [header,
-                  formatted_str]  # your findings here
+                  average]  # your findings here
     toolbox.mp_output_q.put(result_lst)
 
 
 def send_eta_data(toolbox):
     """list of [PERF_HEADER_ETA, PERF_CURRENT_ETA] to ProcInfo, to calc arrival time ETA
     """
     toolbox.PERF_CURRENT_ETA = len(toolbox.NEXT_LIST)
     perf_lst = [toolbox.PERF_HEADER_ETA + toolbox.WORKER_NAME,  # binary head
                 toolbox.PERF_CURRENT_ETA]
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from mp_info_q, of all proc lists
-
-
-def brute_force(toolbox):
-    """List -> dict str compare until stop order in last list, generator empty.
-
-    :params: worker_msg: test for a valid string
-    """
-    busy = True
-    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
-        busy = False  # loop worker sends shutdown msg to next worker - generator is empty
-    remove_header(toolbox)  # remove if no reassembling
-
-    for str_permutation in toolbox.NEXT_LIST:  # 'iiattbz' string permutation in the row
-        search_str(str_permutation, toolbox)
-    return busy
-
-
-def search_str(s_str, toolbox):
-    """Write to result Q if str matched.
-
-    :params: s_str: current generated string to test
-    :params: multi_tool: here the words dict
-    """
-    if s_str in toolbox.multi_tool:  # match dict
-        send_output(toolbox, f'... proc {toolbox.WORKER_NAME} ... {s_str}')
-
-        toolbox.mp_print_q.put(f'... proc {toolbox.WORKER_NAME} ... {s_str}')
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 """
 
 import time
 from collections import defaultdict  # this time factory int to sum
 
 try:
-    import eisenmp.utils_exa.eisenmp_utils as e_utils
+    import eisenmp.utils_exa.eisenmp_utils as utils_exa
 except ImportError:
-    import eisenmp_examples.utils_exa.eisenmp_utils as e_utils
+    import eisenmp_examples.utils_exa.eisenmp_utils as utils_exa
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
 
     Start, Entry, Exit of this single process worker.
@@ -24,14 +24,21 @@
     toolbox.foo, gives also access to all attributes and values
     of the 'modConf.foo' instance, you have created
     """
     # don't need a dictionary in mp_tools_q, we get generator lists to reduce, find a valid word
     busy = workload_get(toolbox)
     list_reduce(toolbox)  # start worker function
     if not busy:
+        # put the search string in db; mngr knows task for string is done
+        str_p = toolbox.kwargs['str_permutation']
+        args = [str_p.upper(),  # search str
+                toolbox.WORKER_PID,  # process id
+                toolbox.INPUT_HEADER,  # iterator list name, chunk id
+                'reducer module']
+        utils_exa.table_insert("INSERT INTO exa (title,col_1,col_2,col_3) VALUES (?,?,?,?)", *args)
         return False
     # send_eta_data(toolbox)  # no data, pb list shrink, worker has timer
     return True
 
 
 def workload_get(toolbox):
     """"""
@@ -60,16 +67,16 @@
 def send_output(toolbox, word_list):
     """Put your findings in the output list.
     Find results in the 'eisenmp_utils.Result.result_dict'
 
     :params: toolbox: -
     :params: average: average of the (chunk of) column
     """
-    # header for output result list
-    header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
+    # header for output result list, q collector can distinguish queues and store result in dict
+    header = toolbox.OUTPUT_HEADER + toolbox.kwargs['str_permutation'] + '_' + toolbox.INPUT_HEADER
     result_lst = [header,
                   word_list]  # your findings here
     toolbox.mp_output_q.put(result_lst)
 
 
 def list_reduce(toolbox):
     """Each Process takes only one chunk of the dict/list.
@@ -124,15 +131,15 @@
 
     :params: str_to_comp: search str
     :params: word_list: list to shrink with strings only of size str_to_comp
     """
     ret_list = []
     for word in word_list:
         if len(word) == len(str_to_comp):
-            replaced = e_utils.replace_special_char(word)
+            replaced = utils_exa.replace_special_char(word)
             ret_list.append(replaced)
     return ret_list
 
 
 def timer_show_rows_left(idx, start_time, word_list, toolbox):
     """Better readable.
     Show rows left in list.
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,125 @@
-"""Economy Example CSV column calculation.
+"""Example 1 brute force
+
+eisenmp uses a list reducer module in example 2.
+Generated list rows from language dict are compared with chars.
+
+Vars and Queues stored in the toolbox instance.
+See documentation for a quick overview, please.
 
 """
+try:
+    import eisenmp.utils_exa.eisenmp_utils as utils_exa
+except ImportError:
+    import eisenmp_examples.utils_exa.eisenmp_utils as utils_exa
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
 
     Start, Entry, Exit of this single process worker.
     We return True to get next list chunk, whatever object is in the rows.
     Fed from mp_input_q to our toolbox. toolbox is our work instance with queues,
     messages, list chunk, and work tools like language dictionary or hash list.
 
     toolbox.foo, gives also access to all attributes and values
     of the 'modConf.foo' instance, you have created
     """
-    # toolbox.mp_print_q.put(toolbox.say_hello)
-    busy = workload_get(toolbox)
-    calc_average(toolbox)  # start worker function
+    if toolbox.multi_tool_get:
+        tool_get(toolbox)  # dict mp_tools_q
+    workload_get(toolbox)
+    busy = brute_force(toolbox)  # worker function
     if not busy:
+        # put the search string in db; mngr knows task for string is done
+        str_p = toolbox.kwargs['str_permutation']
+        args = [str_p.upper(),  # search str
+                toolbox.WORKER_PID,  # process id
+                toolbox.INPUT_HEADER,  # iterator list name, chunk id
+                'bruteforce module']  # the other is reducer module
+        utils_exa.table_insert("INSERT INTO exa (title,col_1,col_2,col_3) VALUES (?,?,?,?)", *args)  # caller view done
         return False
-    send_eta_data(toolbox)  # send data list, first row is header, info thread can find it in eisenmp.output_q_box
+    send_eta_data(toolbox)
     return True
 
 
+def tool_get(toolbox):
+    """"""
+    while 1:
+        if not toolbox.mp_tools_q.empty():
+            toolbox.multi_tool = toolbox.mp_tools_q.get()
+            toolbox.multi_tool_get = False  # can be set in modConf
+            break
+
+
 def workload_get(toolbox):
     """"""
     while 1:
         if not toolbox.mp_input_q.empty():
             toolbox.NEXT_LIST = toolbox.mp_input_q.get()
+            toolbox.num_lists += 1
             break
-    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
-        return False  # loop worker sends shutdown msg to next worker - generator is empty
-    return True
 
 
 def remove_header(toolbox):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
 
     Use self.header_msg attribute to overwrite default header string
     """
-    # toolbox.mp_print_q.put(toolbox.NEXT_LIST[0])
+    # toolbox.mp_print_q.put(f'toolbox.NEXT_LIST[0] {toolbox.NEXT_LIST[0]} {toolbox.WORKER_NAME}')
     toolbox.INPUT_HEADER = toolbox.NEXT_LIST[0]
     del toolbox.NEXT_LIST[0]  # remove header str
 
 
-def calc_average(toolbox):
-    """Calc average from strings.
-    Pandas can make float, but we use raw Python csv import.
-    Table column has 'nan' and empty cells we can not read.
-    """
-    busy = True
-    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # inform we want exit
-        busy = False
-    remove_header(toolbox)
-
-    lst = toolbox.NEXT_LIST
-    STOP_MSG = toolbox.STOP_MSG
-    # kick out 'nan' string and binary stop message from list, stop message is appended on GhettoBoss iterator loop end
-    tbl_flt = [float(num) for num in lst if str(num) and 'nan' not in str(num) and num != STOP_MSG]
-
-    average = 0
-    if len(tbl_flt):  # calc with float type to get comma values
-        average = sum([num for num in tbl_flt]) / len(tbl_flt)
-    average = average if average else 0
-
-    send_output(toolbox, average)
-
-    output_msg = f' ... {toolbox.WORKER_NAME} ... [ average |{average}| ] of {len(toolbox.NEXT_LIST)} rows'
-    toolbox.mp_print_q.put(output_msg)
-
-    return busy
-
-
-def send_output(toolbox, average):
+def send_output(toolbox, str_lst):
     """Put your findings in the output list.
     Find results in the 'eisenmp_utils.Result.result_dict'
 
     :params: toolbox: -
     :params: average: average of the (chunk of) column
     """
-    # header for output result list
-    header = toolbox.OUTPUT_HEADER + toolbox.INPUT_HEADER  # q collector can distinguish queues and store result in dict
+    # header for output result list, q collector can distinguish queues and store result in dict
+    header = toolbox.OUTPUT_HEADER + toolbox.kwargs['str_permutation'] + '_' + toolbox.INPUT_HEADER
     result_lst = [header,
-                  average]  # your findings here
+                  str_lst]  # your findings here
     toolbox.mp_output_q.put(result_lst)
 
 
 def send_eta_data(toolbox):
     """list of [PERF_HEADER_ETA, PERF_CURRENT_ETA] to ProcInfo, to calc arrival time ETA
     """
     toolbox.PERF_CURRENT_ETA = len(toolbox.NEXT_LIST)
     perf_lst = [toolbox.PERF_HEADER_ETA + toolbox.WORKER_NAME,  # binary head
                 toolbox.PERF_CURRENT_ETA]
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from mp_info_q, of all proc lists
+
+
+def brute_force(toolbox):
+    """List -> dict str compare until stop order in last list, generator empty.
+
+    :params: worker_msg: test for a valid string
+    """
+    busy = True
+    if toolbox.STOP_MSG in toolbox.NEXT_LIST:  # eisenmp.iterator_loop() informs stop, no more lists
+        busy = False  # loop worker sends shutdown msg to next worker - generator is empty
+    remove_header(toolbox)  # remove if no reassembling
+
+    result_lst = []
+    for str_permutation in toolbox.NEXT_LIST:  # 'iiattbz' string permutation in the row
+        match_str = search_str(str_permutation, toolbox)
+        result_lst.append(match_str) if match_str else None
+    send_output(toolbox, result_lst)
+    return busy
+
+
+def search_str(s_str, toolbox):
+    """Write to result Q if str matched.
+
+    :params: s_str: current generated string to test
+    :params: multi_tool: here the words dict
+    """
+    if s_str in toolbox.multi_tool:  # match dict
+        toolbox.mp_print_q.put(f'... proc {toolbox.WORKER_NAME} ... {s_str}')
+        return s_str
+    return False
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_double.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import time
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
     """
+    print('Name             |id()           |reference      ')
+    print(*toolbox.Q_NAME_ID_LST)
+
     audio_chunk_lst, video_chunk_lst = None, None
     if not toolbox.WORKER_ID % 2:  # mod is 1 odd
         audio_chunk_lst = batch_1_audio_get(toolbox)
         video_chunk_lst = batch_1_video_get(toolbox)  # batch_1_video_get(toolbox) ['head_1', 'foo', 'bar', 'buz']
     if toolbox.WORKER_ID % 2:  # mod is 0 even
         audio_chunk_lst = batch_7_audio_get(toolbox)
         video_chunk_lst = batch_7_video_get(toolbox)
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,9 +53,7 @@
 
 def yellow_q_get(toolbox):
     """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_yellow_q.empty():
             port_lst = toolbox.mp_yellow_q.get()  # has header with serial number
             return port_lst
-
-
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         target=lambda: app_factory.run(host="localhost", port=port)).start()
 
     msg = col + f'\nWORKER_MSG worker: {toolbox.WORKER_ID} pid: {toolbox.WORKER_PID} server port: {port}\n' \
                 f'SERVER: http://{network}:{port}' + col_end
     toolbox.mp_print_q.put(msg)
 
     # end, return None (Nothing is None), loader leaves worker loop and waits for stop msg in mp_process_q
+    return False
 
 
 def blue_q_get(toolbox):
     """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_blue_q.empty():
             port_lst = toolbox.mp_blue_q.get()  # has header with serial number
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.5.0/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.5.0/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.4.1
+Version: 0.5.0
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
 Keywords: multiprocess framework,examples eisenmp
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 License-File: LICENSE
 License-File: LICENSE.rst
 
-# eisenmp_examples
- 
-Python 3.7 [Multiprocess](https://en.wikipedia.org/wiki/Multiprocessing) 
-[Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
+eisenmp_examples
+##################
+
+.. image:: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/44xtc44/eisenmp_examples/actions/workflows/tests.yml
+
+
+Python 3.7 `Multiprocess <https://en.wikipedia.org/wiki/Multiprocessing>`_
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for single Server
 
 Examples:
 
 * simple style prime number calculation to see the basic use
 * simple http server on one cpu gets content via queue
 * one flask orm server on each cpu - share a user db
 * multiple flask orm server on each cpu, port groups - share a user db
@@ -33,85 +38,94 @@
 * brute_force_attack with itertools generator and dictionary
 * example with two, double fed queues
 * All scenarios follow the **Template style** and have descriptions
 
 ## How to run the examples?
 
 1. Clone the repo and ``run an eisenmp_exa_...`` or
-2. Install [PyPi package](https://pypi.org/project/eisenmp-examples/)
+2. Install `PyPi package <https://pypi.org/project/eisenmp-examples>`_
+
 * in terminal run: `eisenmp_url` and open the local Python SimpleHTTP **URL**
 * in terminal run: `eisenmp_menu` and choose from **Menu**
 
 Brute force cracks strings of an online-game alphabet salad quest. 
 
+::
+
     .. read wordlist .\lang_dictionaries\ger\german.dic
     .. read wordlist .\lang_dictionaries\eng\words.txt
-
-	[BRUTE_FORCE]	cfhhilorrs
-
+    [BRUTE_FORCE]
+    cfhhilorrs
     Create processes. Default: proc/CPU core
     0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 
     
     ... proc Process-7 ... rohrschilf
     ... proc Process-14 ... rohrschilf
     ... proc Process-16 ... rohrschilf
     ... proc Process-7 ... rohrschilf
     ... proc Process-13 ... schilfrohr
     ... proc Process-13 ... schilfrohr
     ... proc Process-11 ... schilfrohr
     ... proc Process-11 ... schilfrohr
 
-	generator empty, run time iterator 5 seconds
-
-	exit WORKER 15
-	exit WORKER 16
-	exit WORKER 2
-	exit WORKER 10
-	exit WORKER 11
-	exit WORKER 12
-	exit WORKER 8
-	exit WORKER 3
-	exit WORKER 4
-	exit WORKER 6
-	exit WORKER 14
-	exit WORKER 5
-	exit WORKER 7
-	exit WORKER 13
-	exit WORKER 1
-	exit WORKER 9
+    generator empty, run time iterator 5 seconds
 
+    exit WORKER 15
+    exit WORKER 16
+    exit WORKER 2
+    exit WORKER 10
+    exit WORKER 11
+    exit WORKER 12
+    exit WORKER 8
+    exit WORKER 3
+    exit WORKER 4
+    exit WORKER 6
+    exit WORKER 14
+    exit WORKER 5
+    exit WORKER 7
+    exit WORKER 13
+    exit WORKER 1
+    exit WORKER 9
+    
     --- Result for [CFHHILORRS]---
     
      rohrschilf
     
      schilfrohr
 
     --- END ---
 
-	Processes are down.
+    Processes are down.
     BF Time in sec: 12
     
     Process finished with exit code 0
 
-    Inbuild example, assert a scrambled string. Use brute force or condensing.
+
+Brute Force
     We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
-    (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
-        Permutation lists grow very fast, reaching Terabyte size.
-    (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
-
-`eisenmp` uses Pythons permutation generator
- [itertools](https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations)
-for the brute force attack example.
 
-    Another example downloads a large list and calculates average for one column.
+    len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
+    Permutation lists grow very fast, reaching Terabyte size.
+
+    len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
+
+Web download a large list
+    Calculates the average for one column.
     Python CSV extracts the column and we calculate the average with the assigned number
     of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
 
 
-- large lists https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©. 
-All material Stats NZ produces is protected by Crown copyright.
-Creative Commons Attribution 4.0 International licence.
-- German dict https://sourceforge.net/projects/germandict/. License Public Domain
-- English dict Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-- ORM Flask-SQLAlchemy https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
+large lists
+    https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©.
+    All material Stats NZ produces is protected by Crown copyright.
+    Creative Commons Attribution 4.0 International licence.
+
+German dict
+    https://sourceforge.net/projects/germandict/. License Public Domain
+
+English dict
+    Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
+
+ORM Flask-SQLAlchemy
+     https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
 
 Cheers
```

### Comparing `eisenmp_examples-0.4.1/eisenmp_examples.egg-info/SOURCES.txt` & `eisenmp_examples-0.5.0/eisenmp_examples.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 LICENSE.rst
 MANIFEST.in
-README.md
+README.rst
 pyproject.toml
 setup.cfg
 eisenmp_examples/__init__.py
 eisenmp_examples/cmd.py
 eisenmp_examples/database.db
 eisenmp_examples/eisenmp_exa_bruteforce.py
 eisenmp_examples/eisenmp_exa_double_q.py
@@ -18,15 +18,18 @@
 eisenmp_examples.egg-info/PKG-INFO
 eisenmp_examples.egg-info/SOURCES.txt
 eisenmp_examples.egg-info/dependency_links.txt
 eisenmp_examples.egg-info/entry_points.txt
 eisenmp_examples.egg-info/requires.txt
 eisenmp_examples.egg-info/top_level.txt
 eisenmp_examples.egg-info/zip-safe
+eisenmp_examples/test/__init__.py
+eisenmp_examples/test/test_entry.py
 eisenmp_examples/utils_exa/__init__.py
+eisenmp_examples/utils_exa/db_exa_schema.sql
 eisenmp_examples/utils_exa/eisenmp_download.py
 eisenmp_examples/utils_exa/eisenmp_search.py
 eisenmp_examples/utils_exa/eisenmp_utils.py
 eisenmp_examples/worker/__init__.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
 eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
```

### Comparing `eisenmp_examples-0.4.1/pyproject.toml` & `eisenmp_examples-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.4.1"
+version = "0.5.0"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "eisenmp multiprocess(or) example collection for server and mobiles"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.7"
 
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable"
```

