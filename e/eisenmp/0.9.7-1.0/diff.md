# Comparing `tmp/eisenmp-0.9.7.tar.gz` & `tmp/eisenmp-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp-0.9.7.tar", last modified: Thu Apr 13 20:59:19 2023, max compression
+gzip compressed data, was "eisenmp-1.0.tar", last modified: Fri Apr 28 19:32:22 2023, max compression
```

## Comparing `eisenmp-0.9.7.tar` & `eisenmp-1.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.419350 eisenmp-0.9.7/
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.7/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-0.9.7/LICENSE.rst
--rw-rw-rw-   0        0        0      187 2023-04-13 16:26:07.000000 eisenmp-0.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0     9965 2023-04-13 20:59:19.420325 eisenmp-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2023-04-13 16:26:07.000000 eisenmp-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.353025 eisenmp-0.9.7/docs/
--rw-rw-rw-   0        0        0      756 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/Makefile
--rwxrwxrwx   0        0        0      804 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.371565 eisenmp-0.9.7/docs/source/
--rw-rw-rw-   0        0        0     6979 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.373508 eisenmp-0.9.7/docs/source/_static/
--rw-rw-rw-   0        0        0      458 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/_static/css-style.css
--rw-rw-rw-   0        0        0     3283 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/conf.py
--rw-rw-rw-   0        0        0     2504 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.rst
--rw-rw-rw-   0        0        0      747 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.utils.rst
--rw-rw-rw-   0        0        0      806 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp.utils_exa.rst
--rw-rw-rw-   0        0        0    27208 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/eisenmp_logo.png
--rw-rw-rw-   0        0        0      237 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/index.rst
--rw-rw-rw-   0        0        0       65 2023-04-13 16:26:07.000000 eisenmp-0.9.7/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.381313 eisenmp-0.9.7/eisenmp/
--rw-rw-rw-   0        0        0     4471 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/__init__.py
--rw-rw-rw-   0        0        0     7459 2023-04-13 20:24:29.000000 eisenmp-0.9.7/eisenmp/eisenmp_procenv.py
--rw-rw-rw-   0        0        0    10522 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/eisenmp_q_coll.py
--rw-rw-rw-   0        0        0     5401 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/eisenmp_worker_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.418374 eisenmp-0.9.7/eisenmp/utils/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_constants.py
--rw-rw-rw-   0        0        0     3918 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_info.py
--rw-rw-rw-   0        0        0     1434 2023-04-13 16:26:07.000000 eisenmp-0.9.7/eisenmp/utils/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:59:19.405694 eisenmp-0.9.7/eisenmp.egg-info/
--rw-rw-rw-   0        0        0     9965 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 20:59:19.000000 eisenmp-0.9.7/eisenmp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 20:59:18.000000 eisenmp-0.9.7/eisenmp.egg-info/zip-safe
--rw-rw-rw-   0        0        0      921 2023-04-13 20:55:32.000000 eisenmp-0.9.7/pyproject.toml
--rw-rw-rw-   0        0        0      392 2023-04-13 20:59:19.428127 eisenmp-0.9.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.383163 eisenmp-1.0/
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:26:07.000000 eisenmp-1.0/LICENSE.rst
+-rw-rw-rw-   0        0        0      160 2023-04-28 00:31:18.000000 eisenmp-1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6450 2023-04-28 19:32:22.384162 eisenmp-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3927 2023-04-27 04:09:38.000000 eisenmp-1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.263214 eisenmp-1.0/docs/
+-rw-rw-rw-   0        0        0      756 2023-04-13 16:26:07.000000 eisenmp-1.0/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2023-04-13 16:26:07.000000 eisenmp-1.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.291192 eisenmp-1.0/docs/source/
+-rw-rw-rw-   0        0        0     2888 2023-04-27 04:09:38.000000 eisenmp-1.0/docs/source/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.307190 eisenmp-1.0/docs/source/_static/
+-rw-rw-rw-   0        0        0      458 2023-04-13 16:26:07.000000 eisenmp-1.0/docs/source/_static/css-style.css
+-rw-rw-rw-   0        0        0    27171 2023-04-20 01:13:44.000000 eisenmp-1.0/docs/source/_static/eisenmp_logo.svg
+-rw-rw-rw-   0        0        0    77077 2023-04-24 13:00:43.000000 eisenmp-1.0/docs/source/_static/eisenmp_pic_generator.svg
+-rw-rw-rw-   0        0        0    61444 2023-04-27 09:54:28.000000 eisenmp-1.0/docs/source/_static/eisenmp_pic_kwargs.svg
+-rw-rw-rw-   0        0        0    79034 2023-04-26 14:51:06.000000 eisenmp-1.0/docs/source/_static/eisenmp_pic_loader.svg
+-rw-rw-rw-   0        0        0   153939 2023-04-26 16:08:21.000000 eisenmp-1.0/docs/source/_static/eisenmp_pic_port_groups.svg
+-rw-rw-rw-   0        0        0     3337 2023-04-27 02:29:52.000000 eisenmp-1.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3078 2023-04-22 08:43:52.000000 eisenmp-1.0/docs/source/constants.rst
+-rw-rw-rw-   0        0        0     6289 2023-04-27 01:40:36.000000 eisenmp-1.0/docs/source/details.rst
+-rw-rw-rw-   0        0        0      784 2023-04-22 17:14:36.000000 eisenmp-1.0/docs/source/eisenmp.rst
+-rw-rw-rw-   0        0        0      747 2023-04-13 16:26:07.000000 eisenmp-1.0/docs/source/eisenmp.utils.rst
+-rw-rw-rw-   0        0        0      321 2023-04-14 18:47:41.000000 eisenmp-1.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0    10527 2023-04-27 04:15:33.000000 eisenmp-1.0/docs/source/modconf.rst
+-rw-rw-rw-   0        0        0       65 2023-04-13 16:26:07.000000 eisenmp-1.0/docs/source/modules.rst
+-rw-rw-rw-   0        0        0       20 2023-04-15 07:02:18.000000 eisenmp-1.0/docs/source/work_conf.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.318184 eisenmp-1.0/eisenmp/
+-rw-rw-rw-   0        0        0     4506 2023-04-25 09:12:46.000000 eisenmp-1.0/eisenmp/__init__.py
+-rw-rw-rw-   0        0        0     8812 2023-04-25 09:12:46.000000 eisenmp-1.0/eisenmp/eisenmp_procenv.py
+-rw-rw-rw-   0        0        0    10456 2023-04-25 06:01:32.000000 eisenmp-1.0/eisenmp/eisenmp_q_coll.py
+-rw-rw-rw-   0        0        0     5879 2023-04-25 10:15:50.000000 eisenmp-1.0/eisenmp/eisenmp_worker_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.382164 eisenmp-1.0/eisenmp/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:26:07.000000 eisenmp-1.0/eisenmp/utils/__init__.py
+-rw-rw-rw-   0        0        0     2726 2023-04-22 17:49:31.000000 eisenmp-1.0/eisenmp/utils/eisenmp_constants.py
+-rw-rw-rw-   0        0        0     3765 2023-04-26 19:05:12.000000 eisenmp-1.0/eisenmp/utils/eisenmp_info.py
+-rw-rw-rw-   0        0        0     1600 2023-04-26 13:32:21.000000 eisenmp-1.0/eisenmp/utils/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:32:22.374170 eisenmp-1.0/eisenmp.egg-info/
+-rw-rw-rw-   0        0        0     6450 2023-04-28 19:32:22.000000 eisenmp-1.0/eisenmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2023-04-28 19:32:22.000000 eisenmp-1.0/eisenmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 19:32:22.000000 eisenmp-1.0/eisenmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-28 19:32:22.000000 eisenmp-1.0/eisenmp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 19:32:22.000000 eisenmp-1.0/eisenmp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-28 19:32:20.000000 eisenmp-1.0/eisenmp.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      922 2023-04-28 03:31:00.000000 eisenmp-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      390 2023-04-28 19:32:22.399158 eisenmp-1.0/setup.cfg
```

### Comparing `eisenmp-0.9.7/LICENSE` & `eisenmp-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.7/LICENSE.rst` & `eisenmp-1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.7/README.md` & `eisenmp-1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,181 +1,153 @@
-# eisenmp
- 
-Python 3.7 
-[Multiprocessor](https://en.wikipedia.org/wiki/Multiprocessing)
-[Framework](https://en.wikipedia.org/wiki/Software_framework) for Server and Mobiles 
+Metadata-Version: 2.1
+Name: eisenmp
+Version: 1.0
+Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
+Author: René Horn
+Author-email: René Horn <rene_horn@gmx.net>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, René Horn
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://github.com/44xtc44
+Project-URL: documentation, https://eisenmp.readthedocs.io/
+Project-URL: repository, https://github.com/44xtc44/eisenmp
+Keywords: multiprocess framework,python multiprocessor framework
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
+License-File: LICENSE
+License-File: LICENSE.rst
+
+Introduction
+############
+
+.. image:: https://github.com/44xtc44/eisenmp/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/44xtc44/eisenmp/actions/workflows/tests.yml
 
-Forget about pools, swim in the sea.
+
+Python 3.7
+
+`Multiprocessor <https://en.wikipedia.org/wiki/Multiprocessing>`_
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for single Server
+
+Kwargs To Go
 
 Features:
 
-* Create **uniform** multiprocess programs for your projects
-* Calculate your Python generator output on _every_ CPU core
-* Worker **module_loader** decouples your Worker imports from Main()
-* **auto Exit** of worker and process
-* Start methods, **spawn**, **fork** and **forkserver**
-* Create VM_ware like **port groups** on CPU cores and stream with (tcp/http) maximum speed via selected NIC adapters
-* Process **START_SEQUENCE_NUM** Worker on a CPU core can grab a specific queue 0=red_q, 1=blue_q,2=yellow_q
-* **Categories of Queues**, read them with **all custom vars** in a worker **ToolBox** dictionary
-* no libraries, light weight; (Linux, Windows)
-
-Visit the features above in the
-[Examples gitHub repository](https://github.com/44xtc44/eisenmp_examples), 
-or get the [Examples PyPi package](https://pypi.org/project/eisenmp-examples/),
-run 
+* **Uniform** foundation to create multiprocess project modules
+* **Workload Chunks** with header to control output and speed up a specific task
+* Chunks get a serial number (ID), findings can be checked in a result dictionary, which ID is missing
+* **module_loader** decouples your Worker imports from Main()
+* **Categories of Queues**, assign Names to Queues and groups of Queues
+* **Queue list** helps to debug your setup and reveals the name, object id and object reference of every Queue
+* **Print Queue** allows formatted print to screen for your processes (blocks)
+* No libraries, (Linux, Windows)
+
+| Visit the features above in the `Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_
+| or
 
-    eisenmp_url 
-    or 
-    eisenmp_menu
-simpleHTTP Ajax server, or terminal menu
+download the all inclusive `PyPi Examples package <https://pypi.org/project/eisenmp-examples/>`_ and
+execute **eisenmp_url** in Terminal to start the simpleHTTP Ajax server
 
-All scenarios run on **reusable Template Modules**. Enjoy the descriptions and discover.
+| All scenarios run on **Template Style Modules**. Enjoy the descriptions.
 
-## How it works
+How it works
+~~~~~~~~~~~~
 You write two functions and two modules.
-Let's call 'em **Generator.py** and **Worker.py**.
+Let's name them **Manager.py** and **Worker.py**.
+
+1. Manager.py defines custom objects and starts a new process, target is **module_loader.py** (loader)
+2. loader imports your (independent) Worker.py module from file system without side effects
+3. loader sits in a loop and calls your Worker.py entry function until queue is empty
+4. **q_feeder** iterator sends a STOP message. Your Worker reads STOP, return False and exit.
+5. **module_loader** module then puts a STOP Worker message in all other input queues.
+6. **Next** Worker reads STOP, exit ...
+7. Loader runs idle and awaits the internal STOP Process message.
+
+.. image:: ./docs/source/_static/eisenmp_pic_loader.svg
+  :width: 640
+  :alt: Worker module loader, loads independent, no imports of parent
+
+Generators
+~~~~~~~~~~~
+
+.. image:: ./docs/source/_static/eisenmp_pic_generator.svg
+  :width: 640
+  :alt: Generator, iterator, lists with name and ID header
+
+Variables transfer to worker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+The worker should be more flexible. Thus, it needs more structured information.
+
+* Information collector is the ``ModuleConfiguration`` class instance. The class can carry any name.
+* All instance attributes are stored in a dictionary __dict__. (self.foo will be kwargs.foo)
+* The instance dictionary is argument (`kwargs`) to call the eisenmp start method.
+* `Kwargs` is updated further with queue information and the START_SEQUENCE_NUM of the process, before process start.
 
-1. Generator.py starts a new process, _but_ the target is **module_loader.py** (loader).
-2. loader imports your (independent) Worker.py module from file system. 
-This makes sure that only imports of the worker.py module are loaded, without side effects.
-3. loader sits in a loop and calls your Worker.py entry function endless. Until there is no more work in the queues.
-This loop keeps the process alive.
-4. **q_feeder** iterator sends a STOP Worker message with the last chunk. Your Worker reads STOP, return False and exit. 
-5. The **module loader** then puts a STOP Worker message in all other input queues.
-Loader runs idle and awaits the internal STOP Process message. **Next** Worker reads STOP, exit ...
+.. image:: ./docs/source/_static/eisenmp_pic_kwargs.svg
+  :width: 640
+  :alt: Generator, Iterator makes lists, result in dictionary
 
-Default ``six Queues``
-- ``Input`` worker lists, ``Output`` result and stop lists, ``Process`` shutdown
+
+Default Queues
+
+- ``Input`` worker lists, ``Output`` result and stop lists
 - ``Tools``, ``Print``, ``Info``
 
-### In detail:
+How to run the examples?
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Fast `PyPi package <https://pypi.org/project/eisenmp-examples/>`_. **eisenmp** will be installed also.
+
+In depth. Clone both repos.
 
-Generator - iterator chunks on every CPU core:
-- [Generator yield](https://docs.python.org/3/reference/expressions.html#yieldexpr)
-or 
-[(expression)](https://peps.python.org/pep-0289/)
-output 1, 2, 3, 4, 5 ➜ eisenmp iterator list [ [1,2] [3,4] [5] ] ➜ **NUM_ROWS** chunks for your Worker
-- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker in (also) a list. 
-- (B) Mngr(): Assign Worker load and process count.
-- (C) Mngr(): Call **iterator** run_q_feeder(generator=Mngr generator)
-- (D) Wkr(): Loop over **NUM_ROWS** list chunks. Return False to **auto exit worker and process**, or get next chunk 
-[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
-or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
-
-One Server (or more) on every CPU core:
-- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (D.1) Wkr(): The **worker** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
-- (D.2) Wkr(): The **worker** starts **MANY** server. Server start call must be threaded, set **STOP_MSG_DISABLE=True**
-- Server read queues: Follow the Generator todo
-[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
-or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
-
-Port groups:
-- Map **START_SEQUENCE_NUM**'s ➜ to multiple (server) ports on CPU cores ➜ to an IP address, 
-[Examples gitHub](https://github.com/44xtc44/eisenmp_examples)
-or get the [PyPi package](https://pypi.org/project/eisenmp-examples/)
-
-
-### ready to use:
-- **run_q_feeder()** iterator lists get a **serial number** header to recreate the original order of chunks
-- **mp_tools_q** for big tools stuff delivery to every single Worker proc module;
-It may be a 27GB rainbow table; See the bruteforce (small) example, please
-- Output **can** be stored if **RESULTS_STORE** is set in config
-
-
-## Issues
-eisenmp can run on Python 3.6 (Ubuntu test), but not the samples.
-
-## How to run the examples?
-Most easy is PyPi package mentioned above. **eisenmp** will be installed also.
-
-Clone both repos.
-[eisenmp](https://github.com/44xtc44/eisenmp) and
-[eisenmp_examples](https://github.com/44xtc44/eisenmp_examples)
+`eisenmp <https://github.com/44xtc44/eisenmp>`_ and
+`eisenmp_examples <https://github.com/44xtc44/eisenmp_examples>`_
 
 Install in editable pip mode.
 
-    cd eisenmp 
+::
+
+    cd eisenmp
     pip3 install -e .  # uninstall (linux pip3) with: pip3 uninstall eisenmp
 
     cd eisenmp_examples
     pip3 install -e .  # uninstall with: pip3 uninstall eisenmp_examples
-Run the examples.
- 
-    eisenmp_url
-    # or
-    eisenmp_menu
 
-Brute force cracks strings of an online-game alphabet salad quest. 
+Run the examples. Either local Ajax Web server or terminal menu.
 
-    .. read wordlist .\lang_dictionaries\ger\german.dic
-    .. read wordlist .\lang_dictionaries\eng\words.txt
+::
 
-	[BRUTE_FORCE]	cfhhilorrs
+    eisenmp_url
+    # or
+    eisenmp_menu
 
-    Create processes. Default: proc/CPU core
-    0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 
-    
-    ... proc Process-7 ... rohrschilf
-    ... proc Process-14 ... rohrschilf
-    ... proc Process-16 ... rohrschilf
-    ... proc Process-7 ... rohrschilf
-    ... proc Process-13 ... schilfrohr
-    ... proc Process-13 ... schilfrohr
-    ... proc Process-11 ... schilfrohr
-    ... proc Process-11 ... schilfrohr
-
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
-
-    --- Result for [CFHHILORRS]---
-    
-     rohrschilf
-    
-     schilfrohr
-
-    --- END ---
-
-	Processes are down.
-    BF Time in sec: 12
-    
-    Process finished with exit code 0
-
-    Inbuild example, assert a scrambled string. Use brute force or condensing.
-    We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
-    (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
-        Permutation lists grow very fast, reaching Terabyte size.
-    (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
-
-`eisenmp` uses Pythons permutation generator
- [itertools](https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations)
-for the brute force attack example.
-
-    Another example downloads a large list and calculates average for one column.
-    Python CSV extracts the column and we calculate the average with the assigned number
-    of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
-
-
-- large lists https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©. 
-All material Stats NZ produces is protected by Crown copyright.
-Creative Commons Attribution 4.0 International licence.
-- German dict https://sourceforge.net/projects/germandict/. License Public Domain
-- English dict Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-- ORM Flask-SQLAlchemy https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
+Get the documentation on readthedocs https://eisenmp.readthedocs.io/
 
-Cheers
```

### Comparing `eisenmp-0.9.7/docs/Makefile` & `eisenmp-1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.7/docs/make.bat` & `eisenmp-1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.7/docs/source/README.rst` & `eisenmp-1.0/eisenmp.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,153 @@
-# eisenmp
-#########
- 
+Metadata-Version: 2.1
+Name: eisenmp
+Version: 1.0
+Summary: Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,
+Author: René Horn
+Author-email: René Horn <rene_horn@gmx.net>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, René Horn
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://github.com/44xtc44
+Project-URL: documentation, https://eisenmp.readthedocs.io/
+Project-URL: repository, https://github.com/44xtc44/eisenmp
+Keywords: multiprocess framework,python multiprocessor framework
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
+License-File: LICENSE
+License-File: LICENSE.rst
+
+Introduction
+############
+
+.. image:: https://github.com/44xtc44/eisenmp/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/44xtc44/eisenmp/actions/workflows/tests.yml
+
+
 Python 3.7
 
 `Multiprocessor <https://en.wikipedia.org/wiki/Multiprocessing>`_
-`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for Server and Mobiles
+`Framework <https://en.wikipedia.org/wiki/Software_framework>`_ for single Server
 
-Forget about pools, swim in the sea.
+Kwargs To Go
 
 Features:
 
-* Create **uniform** multiprocess programs for your projects
-* Calculate your Python generator output on _every_ CPU core
-* Worker **module_loader** decouples your Worker imports from Main()
-* **auto Exit** of worker and process
-* Start methods, **spawn**, **fork** and **forkserver**
-* Create **port groups** on CPU cores and connect network adapters
-* Process **START_SEQUENCE_NUM** Worker on a CPU core can grab a specific queue 0=red_q, 1=blue_q, 2=yellow_q
-* **Categories of Queues**, read them with **all custom vars** in a worker **ToolBox** dictionary
-* Visit the features above in the
-`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
-or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_,
-run **eisenmp_url** simpleHTTP Ajax server
-* All scenarios run on **reusable Template Modules**. Enjoy the descriptions and discover.
-* no libraries, light weight; (Linux, Windows)
+* **Uniform** foundation to create multiprocess project modules
+* **Workload Chunks** with header to control output and speed up a specific task
+* Chunks get a serial number (ID), findings can be checked in a result dictionary, which ID is missing
+* **module_loader** decouples your Worker imports from Main()
+* **Categories of Queues**, assign Names to Queues and groups of Queues
+* **Queue list** helps to debug your setup and reveals the name, object id and object reference of every Queue
+* **Print Queue** allows formatted print to screen for your processes (blocks)
+* No libraries, (Linux, Windows)
+
+| Visit the features above in the `Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_
+| or
+
+download the all inclusive `PyPi Examples package <https://pypi.org/project/eisenmp-examples/>`_ and
+execute **eisenmp_url** in Terminal to start the simpleHTTP Ajax server
+
+| All scenarios run on **Template Style Modules**. Enjoy the descriptions.
 
-## How it works
+How it works
+~~~~~~~~~~~~
 You write two functions and two modules.
-Let's call 'em **Generator.py** and **Worker.py**.
+Let's name them **Manager.py** and **Worker.py**.
+
+1. Manager.py defines custom objects and starts a new process, target is **module_loader.py** (loader)
+2. loader imports your (independent) Worker.py module from file system without side effects
+3. loader sits in a loop and calls your Worker.py entry function until queue is empty
+4. **q_feeder** iterator sends a STOP message. Your Worker reads STOP, return False and exit.
+5. **module_loader** module then puts a STOP Worker message in all other input queues.
+6. **Next** Worker reads STOP, exit ...
+7. Loader runs idle and awaits the internal STOP Process message.
+
+.. image:: ./docs/source/_static/eisenmp_pic_loader.svg
+  :width: 640
+  :alt: Worker module loader, loads independent, no imports of parent
+
+Generators
+~~~~~~~~~~~
+
+.. image:: ./docs/source/_static/eisenmp_pic_generator.svg
+  :width: 640
+  :alt: Generator, iterator, lists with name and ID header
+
+Variables transfer to worker
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+The worker should be more flexible. Thus, it needs more structured information.
+
+* Information collector is the ``ModuleConfiguration`` class instance. The class can carry any name.
+* All instance attributes are stored in a dictionary __dict__. (self.foo will be kwargs.foo)
+* The instance dictionary is argument (`kwargs`) to call the eisenmp start method.
+* `Kwargs` is updated further with queue information and the START_SEQUENCE_NUM of the process, before process start.
 
-1. Generator.py starts a new process, _but_ the target is **module_loader.py** (loader).
-2. loader imports your (independent) Worker.py module from file system. 
-This makes sure that only imports of the worker.py module are loaded, without side effects.
-3. loader sits in a loop and calls your Worker.py entry function endless. Until there is no more work in the queues.
-This loop keeps the process alive.
-4. **q_feeder** iterator sends a STOP Worker message with the last chunk. Your Worker reads STOP, return False and exit. 
-5. The **module loader** then puts a STOP Worker message in all other input queues.
-Loader runs idle and awaits the internal STOP Process message. **Next** Worker reads STOP, exit ...
+.. image:: ./docs/source/_static/eisenmp_pic_kwargs.svg
+  :width: 640
+  :alt: Generator, Iterator makes lists, result in dictionary
 
-Default ``six Queues``
-- ``Input`` worker lists, ``Output`` result and stop lists, ``Process`` shutdown
+
+Default Queues
+
+- ``Input`` worker lists, ``Output`` result and stop lists
 - ``Tools``, ``Print``, ``Info``
 
-### In detail:
+How to run the examples?
+~~~~~~~~~~~~~~~~~~~~~~~~~
+Fast `PyPi package <https://pypi.org/project/eisenmp-examples/>`_. **eisenmp** will be installed also.
+
+In depth. Clone both repos.
+
+`eisenmp <https://github.com/44xtc44/eisenmp>`_ and
+`eisenmp_examples <https://github.com/44xtc44/eisenmp_examples>`_
+
+Install in editable pip mode.
+
+::
+
+    cd eisenmp
+    pip3 install -e .  # uninstall (linux pip3) with: pip3 uninstall eisenmp
+
+    cd eisenmp_examples
+    pip3 install -e .  # uninstall with: pip3 uninstall eisenmp_examples
+
+Run the examples. Either local Ajax Web server or terminal menu.
+
+::
+
+    eisenmp_url
+    # or
+    eisenmp_menu
 
-Generator - iterator chunks on every CPU core:
-- `Generator yield <https://docs.python.org/3/reference/expressions.html#yieldexpr>`_
-or 
-[(expression)](https://peps.python.org/pep-0289/)
-output 1, 2, 3, 4, 5 ➜ eisenmp iterator list [ [1,2] [3,4] [5] ] ➜ **NUM_ROWS** chunks for your Worker
-- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker in (also) a list. 
-- (B) Mngr(): Assign Worker load and process count.
-- (C) Mngr(): Call **iterator** run_q_feeder(generator=Mngr generator)
-- (D) Wkr(): Loop over **NUM_ROWS** list chunks. Return False to **auto exit worker and process**, or get next chunk 
-`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
-or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
-
-One Server (or more) on every CPU core:
-- (A) Mngr(): Import and instantiate **eisenmp**. Register the worker module in a list.
-- (D.1) Wkr(): The **worker** starts **ONE** server, blocks (run_forever on IP: foo port: 42) and serves whatever
-- (D.2) Wkr(): The **worker** starts **MANY** server. Server start call must be threaded, set **STOP_MSG_DISABLE=True**
-- Server read queues: Follow the Generator todo
-`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
-or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
-
-Port groups:
-- Map **toolbox.WORKER_ID**'s ➜ to server ports on CPU cores ➜ to an IP address, 
-`Examples gitHub repository <https://github.com/44xtc44/eisenmp_examples>`_,
-or get the `PyPi package <https://pypi.org/project/eisenmp-examples/>`_
-
-### ready to use:
-- **run_q_feeder()** iterator lists get a **serial number** header to recreate the original order of chunks
-- **mp_tools_q** for big tools stuff delivery to every single Worker proc module;
-It may be a 27GB rainbow table; See the bruteforce (small) example, please
-- Output **can** be stored if **RESULTS_STORE** is set in config
-
-
-## Issues
-eisenmp can run on Python 3.6 (Ubuntu test), but not the samples.
-
-## How to run the examples?
-Clone the repo [Examples gitHub](https://github.com/44xtc44/eisenmp_examples) and ``run an eisenmp_exa_...``.
-
-Brute force cracks strings of an online-game alphabet salad quest. 
-
-    .. read wordlist .\lang_dictionaries\ger\german.dic
-    .. read wordlist .\lang_dictionaries\eng\words.txt
-
-	[BRUTE_FORCE]	cfhhilorrs
-
-    Create processes. Default: proc/CPU core
-    0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 
-    
-    ... proc Process-7 ... rohrschilf
-    ... proc Process-14 ... rohrschilf
-    ... proc Process-16 ... rohrschilf
-    ... proc Process-7 ... rohrschilf
-    ... proc Process-13 ... schilfrohr
-    ... proc Process-13 ... schilfrohr
-    ... proc Process-11 ... schilfrohr
-    ... proc Process-11 ... schilfrohr
-
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
-
-    --- Result for [CFHHILORRS]---
-    
-     rohrschilf
-    
-     schilfrohr
-
-    --- END ---
-
-	Processes are down.
-    BF Time in sec: 12
-    
-    Process finished with exit code 0
-
-    Inbuild example, assert a scrambled string. Use brute force or condensing.
-    We use an english (.6M) plus a german (2M) wordlist and make a dictionary of it. To gain more read speed.
-    (A) len(str) <=  11, combined brute force dictionary attack with a permutation generator. itertool prod. duplicates
-        Permutation lists grow very fast, reaching Terabyte size.
-    (B) len(str) >=  12, pre reduce a len(str) list. Kick out words which are not matching char type and count.
-
-`eisenmp` uses Pythons permutation generator
- `itertools <https://docs.python.org/3/library/itertools.html?highlight=itertools.permutations#itertools.permutations>`_
-for the brute force attack example.
-
-    Another example downloads a large list and calculates average for one column.
-    Python CSV extracts the column and we calculate the average with the assigned number
-    of Porcesses/CPU cores. It can be more processes than CPU cores, if it makes sense.
-
-
-- large lists https://www.stats.govt.nz/large-datasets/csv-files-for-download/ Crown copyright ©. 
-All material Stats NZ produces is protected by Crown copyright.
-Creative Commons Attribution 4.0 International licence.
-- German dict https://sourceforge.net/projects/germandict/. License Public Domain
-- English dict Copyright (c) J Ross Beresford 1993-1999. All Rights Reserved.
-- ORM Flask-SQLAlchemy https://pypi.org/project/Flask-SQLAlchemy-Project-Template/ License MIT 44xtc44
+Get the documentation on readthedocs https://eisenmp.readthedocs.io/
 
-Cheers
```

### Comparing `eisenmp-0.9.7/docs/source/conf.py` & `eisenmp-1.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # -- Project information -----------------------------------------------------
 # !!! indentation of sphinx is mostly 3 leading spaces, code 4, block need one free line above and colon for head
 # pip install -U sphinx
 # pip install sphinx-rtd-theme
 # pip install sphinxcontrib-napoleon
 # Use sphinx-apidoc to build your API documentation:
 # $ cd docs
-# $ sphinx-apidoc -f -o source/ ../eisenradio/   (use full paths for both, __init__.py in the project folders)
+# $ sphinx-apidoc -f -o source/ ../eisenmp/   (use full paths for both, __init__.py(ok).py in the project folders)
 # make html; .\make html, on powerShell
 
 # Docstring Sections¶
 # All of the following section headers are supported:
 # Args (alias of Parameters)
 # Arguments (alias of Parameters)
 # Attention
@@ -67,25 +67,25 @@
 # Yield (alias of Yields)
 # Yields
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'eisenmp'
-copyright = 'BSD-3, 2023, René Horn'
+copyright = 'BSD-3-Clause, 2023, René Horn'
 author = 'René Horn'
 
-
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 # Add napoleon to the extensions list
 extensions = [
     'sphinx.ext.napoleon',
     'sphinx.ext.autodoc',
+    'sphinx.ext.autosectionlabel'
 ]
 
 # Napoleon settings
 napoleon_google_docstring = True
 napoleon_numpy_docstring = True
 napoleon_include_init_with_doc = False
 napoleon_include_private_with_doc = False
@@ -106,13 +106,13 @@
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
 pygments_style = 'sphinx'
 
 html_static_path = ['_static']
-html_logo = "eisenmp_logo.png"
+html_logo = "./_static/eisenmp_logo.svg"
 html_logo_only = True
 html_display_version = False
 html_css_files = [
     "css-style.css",
 ]
```

### Comparing `eisenmp-0.9.7/docs/source/eisenmp.utils.rst` & `eisenmp-1.0/docs/source/eisenmp.utils.rst`

 * *Files identical despite different names*

### Comparing `eisenmp-0.9.7/docs/source/eisenmp.utils_exa.rst` & `eisenmp-1.0/docs/source/eisenmp.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-eisenmp.utils\_exa package
-==========================
+eisenmp package
+===============
+
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   eisenmp.utils
 
 Submodules
 ----------
 
-eisenmp.utils\_exa.eisenmp\_download module
--------------------------------------------
+eisenmp.eisenmp\_procenv module
+-------------------------------
 
-.. automodule:: eisenmp.utils_exa.eisenmp_download
+.. automodule:: eisenmp.eisenmp_procenv
    :members:
    :undoc-members:
    :show-inheritance:
 
-eisenmp.utils\_exa.eisenmp\_search module
------------------------------------------
+eisenmp.eisenmp\_q\_coll module
+-------------------------------
 
-.. automodule:: eisenmp.utils_exa.eisenmp_search
+.. automodule:: eisenmp.eisenmp_q_coll
    :members:
    :undoc-members:
    :show-inheritance:
 
-eisenmp.utils\_exa.eisenmp\_utils module
-----------------------------------------
+eisenmp.eisenmp\_worker\_loader module
+--------------------------------------
 
-.. automodule:: eisenmp.utils_exa.eisenmp_utils
+.. automodule:: eisenmp.eisenmp_worker_loader
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: eisenmp.utils_exa
+.. automodule:: eisenmp
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `eisenmp-0.9.7/eisenmp/__init__.py` & `eisenmp-1.0/eisenmp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-"""eisenmp
+"""
 
 A Python ``multiprocess, multi CPU`` module.
 An example function cracks a game quest.
 
-    ::
+::
 
     Inheritance - proc: ProcEnv -> QueueCollect -> Mp
         Create Queue/Process -> Collect messages in boxes -> Manage, feed queues
 
     Thread names are in ProcEnv:
         QueueCollect [print_q, output_q, input_q, tools_q, info_q],
         GhettoGang [view_output_q_box, tools_q feeder],
         [ProcInfo]
 
 """
 import time
 import threading
 
-import eisenmp.eisenmp_q_coll as coll
-import eisenmp.eisenmp_procenv as procenv
 import eisenmp.utils.eisenmp_utils as e_utils
 import eisenmp.utils.eisenmp_constants as const
 from eisenmp.eisenmp_q_coll import QueueCollect
 
 
 class Mp(QueueCollect):
     """MultiProcessManager.
@@ -36,61 +34,54 @@
     def start(self, **kwargs):
         """enable Processes and eisenmp worker threads.
         """
         self.reset()
         self.kwargs = kwargs
         self.run_proc(**kwargs)
 
-        self.enable_q_box_threads()  # [Baustelle] some q are collected in boxes, 'output', 'print' for later review
+        self.enable_q_box_threads()
 
         self.enable_info_q()  # never disable, else sender blocks, nobody consumes from q
         if 'INFO_ENABLE' in kwargs and kwargs['INFO_ENABLE']:
             self.enable_info_thread()  # collect worker send nums from info box and shows % and ETA
         return
 
     def reset(self):
         """"""
         self.all_threads_stop = False  # frequent calls without exit, see bruteforce
         self.begin_proc_shutdown = False  # frequent calls without exit, see bruteforce
-        if len(e_utils.Result.result_dict):
-            e_utils.Result.result_dict = {}
 
     def run_q_feeder(self, **kwargs):
         """Threaded instance, run multiple q_feeder, called by manager of worker
         """
-        self.kwargs.update(kwargs)  # upd boss kwargs with generator, queues and header_msg
+        self.kwargs.update(kwargs)  # upd kwargs with generator, queues and header_msg
         threading.Thread(name='eisenmp_q_feeder',  # better than class thread here, no overlap, interesting.
                          target=self.q_feeder,
                          ).start()
 
     def q_feeder(self):
-        """Chunk list producer of generator input.
+        """Queue.
+        Chunk list producer of generator input.
 
         - A ticket is attached as header to identify the workload (list chunks)
         - Serial number to rebuild the modified results in the right order
         """
         kw = self.kwargs
         generator = kw['generator']  # no generator for run_q_feeder, crash for sure
-        num_rows = kw['NUM_ROWS'] if 'NUM_ROWS' in kw and kw['NUM_ROWS'] else const.NUM_ROWS  # processor workload
+        rows_max = kw['ROWS_MAX'] if 'ROWS_MAX' in kw and kw['ROWS_MAX'] else const.ROWS_MAX  # processor workload
         feeder_input_q = kw['input_q'] if 'input_q' in kw else self.mp_input_q  # use default if not specified
-
-        result_key = ''  # key name where Queue is stored as value, need a name to distinguish results in result dict
-        for tup in self.q_name_id_lst:
-            name, q_id, _ = tup  # name id q_ref
-            if q_id == id(feeder_input_q):  # unique Python id for objects
-                result_key = name
-                break
+        q_name = q_name_get(self.q_name_id_lst, feeder_input_q)
 
         start = time.perf_counter()
         num_gen = e_utils.consecutive_number()
         while 1:
             if self.all_threads_stop:
                 break
-            chunk_lst = create_transport_ticket(num_gen, result_key)
-            for _ in range(num_rows):
+            chunk_lst = create_transport_header(num_gen, q_name)
+            for _ in range(rows_max):
                 try:
                     chunk_lst.append(next(generator))
                 except StopIteration:
                     chunk_lst.append(const.STOP_MSG)  # signal stop to one worker module, worker module 'loader' to many
                     self.mp_print_q.put(f'\n\tgenerator empty, '
                                         f'run time iterator {round((time.perf_counter() - start))} seconds\n')
                     self.q_input_put(feeder_input_q, chunk_lst)
@@ -103,14 +94,28 @@
             if self.all_threads_stop:
                 break
             if feeder_input_q.empty():
                 feeder_input_q.put(chunk_lst)
                 break
 
 
-def create_transport_ticket(num_gen, result_key):
+def q_name_get(q_name_id_lst, feeder_input_q):
+    """Queue name must be assigned.
+    Name will be dictionary key in result dict, dict in dict.
+    Results are stored like so: {Queue_name: {__TID__1: [foo, bar], {__TID__2: [baz, boo]}}}.
+    """
+    q_name = ''  # result can be stored as dict[q_name] = {_TID_1: foo, _TID_2: bar}
+    for tup in q_name_id_lst:
+        name, q_id, _ = tup  # name id q_ref
+        if q_id == id(feeder_input_q):  # find feeder_input_q in q_name_id_lst, unique Python id() for objects
+            q_name = name
+            break
+    if not q_name:
+        q_name = 'mp_input_q'
+    return q_name
+
+
+def create_transport_header(num_gen, q_name):
     """Semicolon to split easy.
     """
-    if not result_key:
-        result_key = 'mp_input_q'
-    serial_num = ';' + const.TICKET_ID_PREFIX + f'{str(next(num_gen))};'  # ';_TID_1;'
-    return [result_key + serial_num]
+    ticket = q_name + ';' + const.TICKET_ID_PREFIX + f'{str(next(num_gen))};'  # ';_TID_1;'
+    return [ticket]
```

### Comparing `eisenmp-0.9.7/eisenmp/eisenmp_procenv.py` & `eisenmp-1.0/eisenmp/eisenmp_procenv.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,34 +21,36 @@
     - custom Queue builder with a queue in a dict to show a name
     - another Queue builder can add a category name, dict in dict
 
     """
 
     def __init__(self):
         # CPU - process
-        self.NUM_PROCS = self.core_count_get()  # user override in mod
+        self.PROCS_MAX = self.core_count_get()  # user override in mod
         self.proc_list = []  # join processes at the end
         # Queues
         self.q_max_size = 1
         self.mp_info_q = Queue(maxsize=self.q_max_size)  # fake news and performance data
         self.mp_tools_q = Queue(maxsize=self.q_max_size)  # feeder is thread
         self.mp_print_q = Queue(maxsize=self.q_max_size)  # [!mp blocking!] OMG use sparse, formatted output
         self.mp_input_q = Queue(maxsize=self.q_max_size)  # order lists
         self.mp_output_q = Queue(maxsize=self.q_max_size)  # results and stop confirmation
-        self.mp_process_q = Queue(maxsize=self.q_max_size)  # stop order
         self.queue_std_dict = {'mp_info_q': self.mp_info_q,
                                'mp_tools_q': self.mp_tools_q,
                                'mp_print_q': self.mp_print_q,
                                'mp_input_q': self.mp_input_q,
                                'mp_output_q': self.mp_output_q,
-                               'mp_process_q': self.mp_process_q}
+                               }
         self.queue_cust_dict_std = {}  # std dict, val is a q
         self.queue_cust_dict_cat = {}  # custom category, dict in dict
         self.q_lst = []  # all queues in a list, clean up; 'queue_lst_get'
-        self.q_name_id_lst = [('mp_input_q (default)', id(self.mp_input_q), self.mp_info_q)]  # tuple (name, id, q_ref)
+        # queue tuple (name, id, q_ref), all custom created queues will be appended
+        self.q_name_id_lst = [('mp_input_q (default)', id(self.mp_input_q), self.mp_input_q)]
+        # pipe {key: val} {START_SEQUENCE_NUM: Pipe()}, process grabs start id pipe
+        self.pipe_default_dict = {}
 
         # Threads - Collect queue grabber
         self.thread_list = []
         self.info_q_thread_name = 'eisenmp_info_q_thread'
         self.input_q_thread_name = 'eisenmp_input_q_thread'
         self.output_q_thread_name = 'eisenmp_output_q_thread'
         self.print_q_thread_name = 'eisenmp_print_q_thread'
@@ -58,36 +60,44 @@
         self.pi = None  # ProcInfo Sub-thread instance thread, start(), cancel()
 
         # Main switch
         self.all_threads_stop = False  # ends thread loops
         # update
         self.kwargs_env = {}
 
+    def queue_name_avail_get(self, name):
+        """"""
+        for tup in self.q_name_id_lst:
+            if name == tup[0]:
+                raise ValueError(f'eisenmp: Queue {name} already exists in ProcEnv.q_name_id_lst')
+        return True
+
     def queue_cust_dict_std_create(self, *queue_name_maxsize: tuple):
         """create q, name and maxsize as unpacked list ('blue_q_7', 7)
         - Two queue creator functions. All use tuple to ease unpacking.
 
         'queue_cust_dict_std_create' - > 'queue_cust_dict_std'
         'queue_cust_dict_category_create' - > 'queue_cust_dict_cat'
         """
         for name, maxsize in queue_name_maxsize:
+            self.queue_name_avail_get(name)
             self.queue_cust_dict_std[name] = Queue(maxsize=maxsize)
             self.q_name_id_lst.append((name, id(self.queue_cust_dict_std[name]), self.queue_cust_dict_std[name]))
-            pass
 
     def queue_cust_dict_category_create(self, *queue_cat_name_maxsize: tuple):
         """('category_1', 'input_q_3', 10)
         """
         for cat, name, maxsize in queue_cat_name_maxsize:
+            self.queue_name_avail_get(cat + '|' + name)
+
             new_dct = {name: Queue(maxsize=maxsize)}
             if cat not in self.queue_cust_dict_cat:
                 self.queue_cust_dict_cat[cat] = {}
             self.queue_cust_dict_cat[cat].update(new_dct)
             self.q_name_id_lst.append((cat + '|' + name, id(new_dct[name]), new_dct[name]))
-            pass
 
     def queue_lst_get(self):
         """List of qs for shut down msg put in, of ...worker_loader.py
         """
         q_lst = [self.mp_input_q]
 
         for q in self.queue_cust_dict_std.values():  # custom, std dict
@@ -95,66 +105,83 @@
         for cat_dct in self.queue_cust_dict_cat.values():  # custom, category dict
             for q in cat_dct.values():
                 q_lst.append(q)
 
         self.q_lst.extend(q_lst)
         return self.q_lst
 
+    def pipe_lst_create(self):
+        """[Not used so far.]"""
+        for idx in range(self.core_count_get()):
+            self.pipe_default_create(idx)
+
+    def pipe_default_create(self, start_sequence_num):
+        """[Not used so far.] Pipe creation is utter slow.
+
+        wait for worker sent msg's in wait list, then take random corresponding pipe to send list
+        iterator get ready_list=multiprocessing.connection.wait(p_wrk_sender_lst, timeout=None)
+        """
+        recv_mngr, send_wrk = mp.Pipe(duplex=True)  # worker send: 'RDY', manager recv msg remove from pipe
+        recv_wrk, send_mngr = mp.Pipe(duplex=True)  # manager send: list, worker recv list from pipe
+        new_dct = {start_sequence_num: (recv_mngr, send_wrk, recv_wrk, send_mngr)}
+        self.pipe_default_dict.update(new_dct)
+
     @staticmethod
     def core_count_get():
         """"""
         num = 1 if not mp.cpu_count() else mp.cpu_count() / 2  # hyper thread
         return int(num)
 
     def kwargs_env_update_custom(self, **kwargs):
-        """override default NUM_PROCS,
+        """override default PROCS_MAX,
         'queue_lst_get' for worker loader stop msg in all qs
         """
-        self.NUM_PROCS = kwargs['NUM_PROCS'] if 'NUM_PROCS' in kwargs and kwargs['NUM_PROCS'] else self.core_count_get()
+        self.PROCS_MAX = kwargs['PROCS_MAX'] if 'PROCS_MAX' in kwargs and kwargs['PROCS_MAX'] else self.core_count_get()
         kwargs.update(self.queue_std_dict)
         kwargs.update(self.queue_cust_dict_std)
         kwargs.update(self.queue_cust_dict_cat)
-        all_qs_dict = {const.ALL_QUEUES_LIST: self.queue_lst_get()}  # view q name,id,ref in debugger: 'q_name_id_lst'
+        all_qs_dict = {const.ALL_QUEUES_LIST: self.queue_lst_get(),
+                       'Q_NAME_ID_LST': self.q_name_id_lst}  # view q name,id,ref in debugger: 'q_name_id_lst'
+        all_pipes_dict = {'pipe_default_dict': self.pipe_default_dict}
         kwargs.update(all_qs_dict)
+        kwargs.update(all_pipes_dict)
         return kwargs
 
     def run_proc(self, **kwargs):
         """Create a Process for each CPU core, if `num_proc` None set or not set.
         - kwargs dict is updated for worker 'toolbox', reveals all vars and dead references (spawn) available
 
         :params: kwargs: -
         :params: start_method: selection spawn, fork
         :params: START_SEQUENCE_NUM: useful if eisenmp instance is called often, process numbers rise, but start from 0
         :params: target=loader: the worker_loader module is loaded and keeps the process alive
         """
         kwargs = self.kwargs_env_update_custom(**kwargs)
-        self.kwargs_env.update(kwargs)  # eat kwargs
 
         start_method = 'spawn' if 'START_METHOD' not in kwargs else kwargs['START_METHOD']
         mp.set_start_method(start_method, force=True)
 
-        print(f'\nCreate {self.NUM_PROCS} processes.')
-        for core in range(self.NUM_PROCS):
-            print(core, end=" ")
+        print(f'\nCreate {self.PROCS_MAX} processes.')
+        for proc_idx in range(self.PROCS_MAX):
+            print(proc_idx, end=" ")
             # start_sequence_num always starts zero and is independent of sub-process spawn number
-            start_sequence_num = {'START_SEQUENCE_NUM': core}  # worker in proc can grab a specific queue 0=red,1=blue
+            start_sequence_num = {'START_SEQUENCE_NUM': proc_idx}  # wrk in proc can grab a specific queue 0=red,1=blue
             kwargs.update(start_sequence_num)
+            # self.pipe_default_create(proc_idx)
+            self.kwargs_env.update(kwargs)  # pytest preserve kwargs
 
             proc = mp.Process(target=loader.mp_worker_entry,
                               kwargs=kwargs)
             proc.start()
 
             self.proc_list.append(proc)
         self.mp_print_q.put('\n')
 
     def stop_proc(self):
         """All worker must have confirmed shutdown msg."""
-        for proc in range(len(self.proc_list)):
-            self.mp_process_q.put(['Simon Says:', const.STOP_PROCESS])
-
         for process in self.proc_list:
             while process.is_alive():
                 time.sleep(.1)
 
     def end_proc(self):
         """Graceful shutdown join.
         """
```

### Comparing `eisenmp-0.9.7/eisenmp/eisenmp_q_coll.py` & `eisenmp-1.0/eisenmp/eisenmp_q_coll.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,20 +128,19 @@
 
         Note: Multiple threads can loop over the box (dict).
         """
         generator = e_utils.consecutive_number()
         while 1:
             if self.all_threads_stop:
                 break
-            if not self.mp_output_q.empty():
-                worker_output = self.mp_output_q.get()
-                serial_num = next(generator)
-                self.output_q_box[serial_num] = worker_output
-                is_STOP_MSG = self.output_q_search_stop_confirm(serial_num)
-                self.output_q_box_view_results(serial_num) if not is_STOP_MSG else None
+            worker_output = self.mp_output_q.get()
+            serial_num = next(generator)
+            self.output_q_box[serial_num] = worker_output
+            is_STOP_MSG = self.output_q_search_stop_confirm(serial_num)
+            self.output_q_box_view_results(serial_num) if not is_STOP_MSG else None
 
     def output_q_search_stop_confirm(self, serial_num):
         """Search stop msg of workers and put 'em in a list.
         Stop processes and threads, if list is full.
         {1: ['RESULT_HEADER;PRIME_NUM;_TID_1;Process-1', ['10000079']], 24: ['PROC_STOP;Process-5']}
 
         :params: serial_num: serial number of `output_q_loop`
@@ -152,18 +151,18 @@
 
             list_header = outbox_list[0]
             if list_header[:len(const.STOP_CONFIRM)] == const.STOP_CONFIRM:
                 if self.worker_mods_down_ask(list_header):
                     self.print_findings()
 
                     self.begin_proc_shutdown = True
-                    self.all_threads_stop = True
-
                     self.stop_proc()
                     self.end_proc()
+                    self.all_threads_stop = True
+
                     self.stop_thread()
                     self.end_thread()
 
                 return True
 
     def output_q_box_view_results(self, serial_num):
         """Only `lists` with header accepted.
```

### Comparing `eisenmp-0.9.7/eisenmp/eisenmp_worker_loader.py` & `eisenmp-1.0/eisenmp/eisenmp_worker_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         self.mp_info_q = None  # performance data, or other
         self.mp_tools_q = None  # data too big to send with every list to worker
         self.mp_print_q = None  # formatted screen output with multiprocessor lock(), use sparse
         self.mp_input_q = None
         self.mp_output_q = None
         self.mp_process_q = None  # proc shutdown msg's
         # reserved names
-        self.NEXT_LIST = None  # input_q, next list from your generator -> Ghetto is iterator, list creator
-        self.WORKER_ID = None  # name id from Process name
+        self.NEXT_LIST = None  # next list from your generator -> iterator creates list
+        self.WORKER_ID = None  # Process-1 -> 1
         self.WORKER_PID = None  # process pid
-        self.WORKER_NAME = None  # stop confirmations collected by GhettoGang and send shutdown signal to program
-        self.MULTI_TOOL = None  # tools_q, can be any prerequisite object for a module
-        self.STOP_MSG = None  # all q, not mp_print_q, if Boss StopIteration is raised, or this wrk informs other worker
-        self.STOP_CONFIRM = ''  # output_q, GhettoGang collects msg to send shutdown signal to program
+        self.WORKER_NAME = None  # process name
+        self.MULTI_TOOL = None  # tools_q, can be any prerequisite object for a module (made for bruteforce attacks)
+        self.STOP_MSG = None  # not mp_print_q, ...worker_loader in one process informs other processes about stop
+        self.STOP_CONFIRM_AND_PROCNAME = ''  # output_q_box thread gets worker messages, stop and results
         self.OUTPUT_HEADER = ''  # identify proc result in output_q_box
-        self.INPUT_HEADER = ''
-        self.PERF_HEADER_ETA = None  # 'PROC_PERF_ETA_'
-        self.PERF_CURRENT_ETA = None  # list rows done or other count
+        self.INPUT_HEADER = ''  # ident proc result output_q_box (not stop msg) and copy result to result[INPUT_HEADER]
+        self.PERF_HEADER_ETA = None  # str PERF_HEADER_ETA
+        self.PERF_CURRENT_ETA = None  # header of list rows done for info_thread
         self.kwargs = None
 
 
 def module_path_load(file_path):
     """Imports the module from path and returns it in the env.
     """
     path, f_name = os.path.split(file_path)
@@ -60,75 +60,90 @@
     stop_token_lst = [const.OUTPUT_HEADER,
                       const.STOP_MSG]  # 'STOP' was sent if last list was produced; now we inform other worker
 
     for q in toolbox.ALL_QUEUES_LIST:  # next worker on any q reads 'stop_token_lst', except 'mp_print_q'
         if q.empty():
             q.put(stop_token_lst)
 
-    toolbox.mp_output_q.put([toolbox.STOP_CONFIRM])  # essential msg for caller, count stop to exit
+    toolbox.mp_output_q.put([toolbox.STOP_CONFIRM_AND_PROCNAME])  # essential msg for caller, count stop to exit
     toolbox.mp_print_q.put(f'\texit WORKER {toolbox.WORKER_ID}')
-    pass
 
 
-def mp_worker_entry(**kwargs):
-    """Entry.
-    We are 'disconnected' from parent process now.
-    Only Queue communication. Threads can exec() 'string' commands.
-    All references are dead. Variables ok. We read only, here.
+def toolbox_enable(**kwargs):
+    """Populate Toolbox class attributes for the worker to use.
     """
-    worker = None
     # assembled vars and names
     name = mp.process.current_process().name
     proc_id = name.split('-')
     tool_box = {name: ToolBox()}
     tool_box[name].__dict__.update(kwargs)  # ToolBox class, add user defined attributes of ModuleConfiguration inst
     # defaults
     tool_box[name].WORKER_ID = int(proc_id[1])
     tool_box[name].WORKER_PID = int(os.getpid())
     tool_box[name].WORKER_NAME = name
     tool_box[name].STOP_MSG = const.STOP_MSG
-    tool_box[name].STOP_CONFIRM = const.STOP_CONFIRM + name
+    tool_box[name].STOP_CONFIRM_AND_PROCNAME = const.STOP_CONFIRM + name
     tool_box[name].OUTPUT_HEADER = const.OUTPUT_HEADER
     tool_box[name].PERF_HEADER_ETA = const.PERF_HEADER_ETA  # performance list header for ProcInfo
     tool_box[name].PERF_CURRENT_ETA = None
     tool_box[name].kwargs = kwargs
 
     toolbox = tool_box[name]  # use normal instance like
+    return toolbox
+
 
-    # Module Loader
+def module_loader(**kwargs):
+    """Modules loaded and function call stored as a reference in a list.
+    """
     mod_fun_lst = []
     for row in kwargs['worker_modules']:
         if len(row):
             path_t, ref_t = row.items()
             worker_path, worker_ref = path_t[1], ref_t[1]
 
             worker_mod = module_path_load(worker_path)  # str path to -> imported module now available
             fun_ref_exec = getattr(worker_mod, worker_ref)  # reference: can make function call now
             mod_fun_lst.append(fun_ref_exec)
+    return mod_fun_lst
+
 
-    # Function executor
+def function_executor(toolbox, mod_fun_lst):
+    """Worker execution in loop, all other functions must start threaded.
+
+    :params: toolbox: kwargs
+    :params: mod_fun_lst: list with function references to execute
+    """
+    worker = None
     if len(mod_fun_lst):
         mod_fun_len = len(mod_fun_lst)
 
         for workmate in range(mod_fun_len):
             if len(mod_fun_lst) >= 2:
                 mate_fun = mod_fun_lst.pop()
                 mate_fun(toolbox)
-        worker = mod_fun_lst.pop()  # last but not least
+        worker = mod_fun_lst.pop()
+    return worker
 
-    while 1:
 
-        busy = worker(toolbox)  # until worker reads the iterator STOP msg
-        if not busy:
-            if 'STOP_MSG_DISABLE' not in toolbox.kwargs or not toolbox.kwargs['STOP_MSG_DISABLE']:
-                all_worker_exit_msg(toolbox)  # stop msg in all queues, if not all loaded worker are threads
-            break
+def mp_worker_entry(**kwargs):
+    """Entry.
+    We are 'disconnected' from parent process now.
+    Only Queue communication. Threads can exec() 'string' commands.
+    All references are dead. Variables ok. We read only, here.
 
-    while 1:
+    The worker can loop itself and grab a new list from queue; while loop.
+    """
+    toolbox = toolbox_enable(**kwargs)
+
+    if 'worker_modules' not in kwargs or not len(kwargs['worker_modules']):
+        msg = '\n\teisenmp worker_loader: No Worker Module to start - exit process\n'
+        toolbox.mp_print_q.put(msg)
+        return
 
-        msg_lst = toolbox.mp_process_q.get()  # loader keeps proc alive and awaits, 'stop_proc'
-        if const.STOP_PROCESS in msg_lst:
+    mod_fun_lst = module_loader(**kwargs)
+    worker = function_executor(toolbox, mod_fun_lst)
 
-            for q in toolbox.ALL_QUEUES_LIST:  # multiple qs feeder may stick if first sent the worker stop
-                if not q.empty():
-                    q.get()
+    while 1:
+        busy = worker(toolbox)  # until worker reads the iterator STOP msg
+        if not busy:
+            all_worker_exit_msg(toolbox)  # stop msg in all queues, if not all loaded worker are threads
             break
```

### Comparing `eisenmp-0.9.7/eisenmp/utils/eisenmp_info.py` & `eisenmp-1.0/eisenmp/utils/eisenmp_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import time
 import threading
 
 import eisenmp.utils.eisenmp_constants as constants
 
 
 class ProcInfo(threading.Thread):
-    """Thread; start(), cancel()
+    """Thread start() cancel()
     Brute Force uses factorial as target to calculate.
     Prime uses 'range_num' of num generator as target.
-        List rows done are the current state
+    List rows done are the current state
     estimated time of arrival, ETA.
     So far.
 
     We sit on the QueueCollect and loop over the collected items in a list or dict (box).
     instantiated by GhettoGang
 
     """
@@ -60,22 +60,19 @@
         """
         """
         for idx in range(len(info_box)):
             if idx in info_box.keys():
                 if type(info_box[idx]) is list:
 
                     list_header = info_box[idx][0]
-                    if list_header[:14] == constants.PERF_HEADER_ETA:
+                    if list_header[:15] == constants.PERF_HEADER_ETA:
                         a_num = int(info_box[idx][1])
                         if self.INFO_THREAD_MAX:
                             self.perf_dict_eta['target'] = self.INFO_THREAD_MAX
-                            if self.info_td_exec:
-                                exec(self.info_td_exec)
-                            else:
-                                self.perf_dict_eta['rows_done'] += a_num  # ETA
+                            self.perf_dict_eta['rows_done'] += a_num  # ETA
                         info_box[idx] = None
 
     def perf_count_print_eta(self):
         """
         """
         if self.arrival_eta():
             percent, sec_left = self.arrival_eta()
@@ -96,15 +93,15 @@
         self.perf_dict_eta = {'target': 0,
                               'rows_done': 0,
                               'proc_start': time.perf_counter()}
         info_box = self.info_q_box
         while not self.info_shutdown:  # self.perf_dict_eta['rows_done']
             self.perf_count_eta(info_box)
             self.perf_count_print_eta()
-            for _ in range(40):
+            for _ in range(30):
                 if self.info_shutdown:
                     return
                 time.sleep(.1)
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `eisenmp-0.9.7/pyproject.toml` & `eisenmp-1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp"
-version = "0.9.7"
+version = "1.0"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "Multiprocess Framework for Server and Mobiles; run your generator output and server on every CPU core,"
 keywords = ['multiprocess framework', 'python multiprocessor framework']
 license = {file = "LICENSE.rst"}
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable"
 ]
 dependencies = [
@@ -24,8 +24,8 @@
 [project.urls]
 homepage = "https://github.com/44xtc44"
 documentation = "https://eisenmp.readthedocs.io/"
 repository = "https://github.com/44xtc44/eisenmp"
 
 [tool.pytest.ini_options]
 addopts = "--cov=."
-testpaths = "."
+testpaths = ["."]
```

