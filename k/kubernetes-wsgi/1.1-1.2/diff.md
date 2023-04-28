# Comparing `tmp/kubernetes_wsgi-1.1.tar.gz` & `tmp/kubernetes_wsgi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubernetes_wsgi-1.1.tar", last modified: Fri May  8 19:55:39 2020, max compression
+gzip compressed data, was "kubernetes_wsgi-1.2.tar", last modified: Fri Apr 28 02:39:09 2023, max compression
```

## Comparing `kubernetes_wsgi-1.1.tar` & `kubernetes_wsgi-1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/.github/
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/.github/workflows/
--rw-r--r--   0 coderanger   (501) staff       (20)     1884 2020-04-28 10:42:27.000000 kubernetes_wsgi-1.1/.github/workflows/main.yml
--rw-r--r--   0 coderanger   (501) staff       (20)      800 2020-04-27 07:18:01.000000 kubernetes_wsgi-1.1/.pre-commit-config.yaml
--rw-r--r--   0 coderanger   (501) staff       (20)    11358 2020-04-28 10:29:42.000000 kubernetes_wsgi-1.1/LICENSE
--rw-r--r--   0 coderanger   (501) staff       (20)      356 2020-04-27 06:00:08.000000 kubernetes_wsgi-1.1/MANIFEST.in
--rw-r--r--   0 coderanger   (501) staff       (20)     2626 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/PKG-INFO
--rw-r--r--   0 coderanger   (501) staff       (20)     1791 2020-04-28 10:39:22.000000 kubernetes_wsgi-1.1/README.md
--rw-r--r--   0 coderanger   (501) staff       (20)      645 2020-04-27 07:25:22.000000 kubernetes_wsgi-1.1/pyproject.toml
--rw-r--r--   0 coderanger   (501) staff       (20)      817 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/setup.cfg
--rw-r--r--   0 coderanger   (501) staff       (20)       39 2020-04-27 06:19:37.000000 kubernetes_wsgi-1.1/setup.py
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/src/
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi/
--rw-r--r--   0 coderanger   (501) staff       (20)       20 2020-05-08 19:53:42.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi/__init__.py
--rw-r--r--   0 coderanger   (501) staff       (20)     2399 2020-05-08 19:53:27.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi/__main__.py
--rw-r--r--   0 coderanger   (501) staff       (20)      949 2020-04-27 07:25:22.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi/metrics.py
--rw-r--r--   0 coderanger   (501) staff       (20)     3159 2020-04-28 10:09:39.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi/server.py
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/
--rw-r--r--   0 coderanger   (501) staff       (20)     2626 2020-05-08 19:55:38.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 coderanger   (501) staff       (20)      562 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 coderanger   (501) staff       (20)        1 2020-05-08 19:55:38.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 coderanger   (501) staff       (20)        1 2020-04-27 06:15:43.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/not-zip-safe
--rw-r--r--   0 coderanger   (501) staff       (20)       74 2020-05-08 19:55:38.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/requires.txt
--rw-r--r--   0 coderanger   (501) staff       (20)       16 2020-05-08 19:55:38.000000 kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/top_level.txt
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/tests/
-drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2020-05-08 19:55:39.000000 kubernetes_wsgi-1.1/tests/app1/
--rw-r--r--   0 coderanger   (501) staff       (20)      132 2020-04-27 07:25:21.000000 kubernetes_wsgi-1.1/tests/app1/wsgi.py
--rw-r--r--   0 coderanger   (501) staff       (20)     1741 2020-05-08 19:53:27.000000 kubernetes_wsgi-1.1/tests/test_main.py
--rw-r--r--   0 coderanger   (501) staff       (20)     1263 2020-04-28 10:18:09.000000 kubernetes_wsgi-1.1/tests/test_server.py
--rw-r--r--   0 coderanger   (501) staff       (20)     1884 2020-04-28 10:21:07.000000 kubernetes_wsgi-1.1/tox.ini
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.886032 kubernetes_wsgi-1.2/
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.871514 kubernetes_wsgi-1.2/.github/
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.876681 kubernetes_wsgi-1.2/.github/workflows/
+-rw-r--r--   0 coderanger   (501) staff       (20)     1895 2023-04-28 02:26:54.000000 kubernetes_wsgi-1.2/.github/workflows/main.yml
+-rw-r--r--   0 coderanger   (501) staff       (20)      482 2023-04-28 02:33:35.000000 kubernetes_wsgi-1.2/.pre-commit-config.yaml
+-rw-r--r--   0 coderanger   (501) staff       (20)    11358 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/LICENSE
+-rw-r--r--   0 coderanger   (501) staff       (20)      356 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/MANIFEST.in
+-rw-r--r--   0 coderanger   (501) staff       (20)     2430 2023-04-28 02:39:09.886211 kubernetes_wsgi-1.2/PKG-INFO
+-rw-r--r--   0 coderanger   (501) staff       (20)     1798 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/README.md
+-rw-r--r--   0 coderanger   (501) staff       (20)      645 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/pyproject.toml
+-rw-r--r--   0 coderanger   (501) staff       (20)      869 2023-04-28 02:39:09.887241 kubernetes_wsgi-1.2/setup.cfg
+-rw-r--r--   0 coderanger   (501) staff       (20)       39 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/setup.py
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.871939 kubernetes_wsgi-1.2/src/
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.879438 kubernetes_wsgi-1.2/src/kubernetes_wsgi/
+-rw-r--r--   0 coderanger   (501) staff       (20)       20 2023-04-28 02:23:04.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi/__init__.py
+-rw-r--r--   0 coderanger   (501) staff       (20)     2808 2023-04-28 02:21:31.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi/__main__.py
+-rw-r--r--   0 coderanger   (501) staff       (20)      949 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi/metrics.py
+-rw-r--r--   0 coderanger   (501) staff       (20)     3312 2023-04-28 02:21:25.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi/server.py
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.883370 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/
+-rw-r--r--   0 coderanger   (501) staff       (20)     2430 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 coderanger   (501) staff       (20)      562 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 coderanger   (501) staff       (20)        1 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 coderanger   (501) staff       (20)        1 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/not-zip-safe
+-rw-r--r--   0 coderanger   (501) staff       (20)       74 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/requires.txt
+-rw-r--r--   0 coderanger   (501) staff       (20)       16 2023-04-28 02:39:09.000000 kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/top_level.txt
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.884812 kubernetes_wsgi-1.2/tests/
+drwxr-xr-x   0 coderanger   (501) staff       (20)        0 2023-04-28 02:39:09.885480 kubernetes_wsgi-1.2/tests/app1/
+-rw-r--r--   0 coderanger   (501) staff       (20)      132 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/tests/app1/wsgi.py
+-rw-r--r--   0 coderanger   (501) staff       (20)     1741 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/tests/test_main.py
+-rw-r--r--   0 coderanger   (501) staff       (20)     1263 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/tests/test_server.py
+-rw-r--r--   0 coderanger   (501) staff       (20)     1884 2022-11-15 18:07:59.000000 kubernetes_wsgi-1.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kubernetes_wsgi-1.1/.github/workflows/main.yml` & `kubernetes_wsgi-1.2/.github/workflows/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 jobs:
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: "ubuntu-latest"
     strategy:
       matrix:
-        python-version: ["3.5", "3.6", "3.7", "3.8"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: "actions/checkout@v2"
       - uses: "actions/setup-python@v1"
         with:
           python-version: "${{ matrix.python-version }}"
       - name: "Install dependencies"
@@ -37,15 +37,15 @@
     name: "Build & verify package"
     runs-on: "ubuntu-latest"
 
     steps:
       - uses: "actions/checkout@v2"
       - uses: "actions/setup-python@v1"
         with:
-          python-version: "3.8"
+          python-version: "3.11"
 
       - name: "Install pep517 and twine"
         run: "python -m pip install pep517 twine"
       - name: "Build package"
         run: "python -m pep517.build --source --binary ."
       - name: "List result"
         run: "ls -l dist"
@@ -60,12 +60,12 @@
     name: "Verify dev env"
     runs-on: "${{ matrix.os }}"
 
     steps:
       - uses: "actions/checkout@v2"
       - uses: "actions/setup-python@v1"
         with:
-          python-version: "3.8"
+          python-version: "3.11"
       - name: "Install in dev mode"
         run: "python -m pip install -e .[dev]"
       - name: "Import package"
         run: "python -c 'import kubernetes_wsgi; print(kubernetes_wsgi.__version__)'"
```

### Comparing `kubernetes_wsgi-1.1/LICENSE` & `kubernetes_wsgi-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/PKG-INFO` & `kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
-Name: kubernetes_wsgi
-Version: 1.1
+Name: kubernetes-wsgi
+Version: 1.2
 Summary: A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
-Home-page: UNKNOWN
+Home-page: https://github.com/coderanger/kubernetes-wsgi
 License: Apache License 2.0
-Description: # Kubernetes_WSGI
-        
-        A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
-        
-        This also includes Prometheus metrics support.
-        
-        ## Quick Start
-        
-        To install:
-        
-        ```
-        pip install kubernetes-wsgi
-        ```
-        
-        To launch your application:
-        
-        ```
-        python -m kubernetes_wsgi myapp 8000
-        ```
-        
-        where `myapp` is an importable module name containing your WSGI application function.
-        
-        ## Why Threads?
-        
-        The gold standard for Python WSGI servers is Gunicorn, renowned for its multi-process execution mode for effcient concurrency despite the dreaded Python GIL (Global Interpreter Lock). Unfortunately when working with containers, multi-process worker models can be difficult to work with as containers generally expect to only have a single process. Specifically this means if one of the forked workers is hit by an OOM and killed, the main process will simply restart it without triggering the usual metrics in Kubernetes for OOM'd Pods. Similarly we have a different way to handle multi-process concurrency in Kubernetes, through a Deployment with many replicas. In the simplest version would could use multiple replicas each handling only one request at a time, but using a thread pool improves throughput by taking advantage of the fact that most web applications are blocked on I/O most of the time (usually waiting for a response from a database or another web service).
-        
-        ## Why Twisted?
-        
-        Gunicorn itself does have a threadpool mode, however it's somewhat awkward to work with as it uses the `futures` ThreadPool implementation. Twisted's ThreadPool is more efficent. This also allows installing the Prometheus metrics as a native Twisted web handler so it will work even if the threadpool is exhausted, meaning your metrics keep working even during a system overload.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: tests
+License-File: LICENSE
+
+# Kubernetes_WSGI
+
+A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
+
+This also includes Prometheus metrics support.
+
+## Quick Start
+
+To install:
+
+```
+pip install kubernetes-wsgi
+```
+
+To launch your application:
+
+```
+python -m kubernetes_wsgi myapp --port 8000
+```
+
+where `myapp` is an importable module name containing your WSGI application function.
+
+## Why Threads?
+
+The gold standard for Python WSGI servers is Gunicorn, renowned for its multi-process execution mode for effcient concurrency despite the dreaded Python GIL (Global Interpreter Lock). Unfortunately when working with containers, multi-process worker models can be difficult to work with as containers generally expect to only have a single process. Specifically this means if one of the forked workers is hit by an OOM and killed, the main process will simply restart it without triggering the usual metrics in Kubernetes for OOM'd Pods. Similarly we have a different way to handle multi-process concurrency in Kubernetes, through a Deployment with many replicas. In the simplest version would could use multiple replicas each handling only one request at a time, but using a thread pool improves throughput by taking advantage of the fact that most web applications are blocked on I/O most of the time (usually waiting for a response from a database or another web service).
+
+## Why Twisted?
+
+Gunicorn itself does have a threadpool mode, however it's somewhat awkward to work with as it uses the `futures` ThreadPool implementation. Twisted's ThreadPool is more efficent. This also allows installing the Prometheus metrics as a native Twisted web handler so it will work even if the threadpool is exhausted, meaning your metrics keep working even during a system overload.
```

### Comparing `kubernetes_wsgi-1.1/README.md` & `kubernetes_wsgi-1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 pip install kubernetes-wsgi
 ```
 
 To launch your application:
 
 ```
-python -m kubernetes_wsgi myapp 8000
+python -m kubernetes_wsgi myapp --port 8000
 ```
 
 where `myapp` is an importable module name containing your WSGI application function.
 
 ## Why Threads?
 
 The gold standard for Python WSGI servers is Gunicorn, renowned for its multi-process execution mode for effcient concurrency despite the dreaded Python GIL (Global Interpreter Lock). Unfortunately when working with containers, multi-process worker models can be difficult to work with as containers generally expect to only have a single process. Specifically this means if one of the forked workers is hit by an OOM and killed, the main process will simply restart it without triggering the usual metrics in Kubernetes for OOM'd Pods. Similarly we have a different way to handle multi-process concurrency in Kubernetes, through a Deployment with many replicas. In the simplest version would could use multiple replicas each handling only one request at a time, but using a thread pool improves throughput by taking advantage of the fact that most web applications are blocked on I/O most of the time (usually waiting for a response from a database or another web service).
```

### Comparing `kubernetes_wsgi-1.1/pyproject.toml` & `kubernetes_wsgi-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/setup.cfg` & `kubernetes_wsgi-1.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [metadata]
 name = kubernetes_wsgi
 version = attr: kubernetes_wsgi.__version__
 description = A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
 long_description = file: README.md
 license = Apache License 2.0
+url = https://github.com/coderanger/kubernetes-wsgi
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

### Comparing `kubernetes_wsgi-1.1/src/kubernetes_wsgi/__main__.py` & `kubernetes_wsgi-1.2/src/kubernetes_wsgi/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,20 +42,36 @@
     )
     parser.add_argument(
         "--health-check-path",
         metavar="PATH",
         default="/healthz",
         help="URL path to the health check endpoint",
     )
+    parser.add_argument(
+        "--min-threads",
+        metavar="N",
+        type=int,
+        default=5,
+        help="Minimum number of threads to run",
+    )
+    parser.add_argument(
+        "--max-threads",
+        metavar="N",
+        type=int,
+        default=20,
+        help="Maximum number of threads to run",
+    )
     args = parser.parse_args(argv)
     return {
         "application": args.application,
         "port": args.port,
         "metrics_port": args.metrics_port,
         "health_check_path": args.health_check_path,
+        "min_threads": args.min_threads,
+        "max_threads": args.max_threads,
     }
 
 
 def load_application(app_str: str) -> "WSGIApplication":
     func_name = None  # type: Optional[str]
     if ":" in app_str:
         mod_name, func_name = app_str.split(":", 1)
```

### Comparing `kubernetes_wsgi-1.1/src/kubernetes_wsgi/metrics.py` & `kubernetes_wsgi-1.2/src/kubernetes_wsgi/metrics.py`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/src/kubernetes_wsgi/server.py` & `kubernetes_wsgi-1.2/src/kubernetes_wsgi/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,31 @@
 
 def serve(
     application: "WSGIApplication",
     port: int = 8000,
     metrics_port: int = 9000,
     access_log_formatter: LogFormatter = proxiedLogFormatter,
     health_check_path: str = "/healthz",
+    min_threads: int = 5,
+    max_threads: int = 20,
 ):
     # Quiet the Twisted factory logging.
     Factory.noisy = False
 
     # Start logging.
     logging.basicConfig(level=logging.INFO)
     observers = [STDLibLogObserver()]
-    logger.globalLogBeginner.beginLoggingTo(observers)
+    logger.globalLogBeginner.beginLoggingTo(
+        observers, redirectStandardIO=False
+    )
 
     # Create the server.
-    pool = threadpool.ThreadPool()
+    pool = threadpool.ThreadPool(
+        minthreads=min_threads, maxthreads=max_threads
+    )
     reactor.callWhenRunning(pool.start)
     _listen_wsgi(
         reactor,
         pool,
         application,
         port,
         access_log_formatter,
```

### Comparing `kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/PKG-INFO` & `kubernetes_wsgi-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
-Name: kubernetes-wsgi
-Version: 1.1
+Name: kubernetes_wsgi
+Version: 1.2
 Summary: A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
-Home-page: UNKNOWN
+Home-page: https://github.com/coderanger/kubernetes-wsgi
 License: Apache License 2.0
-Description: # Kubernetes_WSGI
-        
-        A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
-        
-        This also includes Prometheus metrics support.
-        
-        ## Quick Start
-        
-        To install:
-        
-        ```
-        pip install kubernetes-wsgi
-        ```
-        
-        To launch your application:
-        
-        ```
-        python -m kubernetes_wsgi myapp 8000
-        ```
-        
-        where `myapp` is an importable module name containing your WSGI application function.
-        
-        ## Why Threads?
-        
-        The gold standard for Python WSGI servers is Gunicorn, renowned for its multi-process execution mode for effcient concurrency despite the dreaded Python GIL (Global Interpreter Lock). Unfortunately when working with containers, multi-process worker models can be difficult to work with as containers generally expect to only have a single process. Specifically this means if one of the forked workers is hit by an OOM and killed, the main process will simply restart it without triggering the usual metrics in Kubernetes for OOM'd Pods. Similarly we have a different way to handle multi-process concurrency in Kubernetes, through a Deployment with many replicas. In the simplest version would could use multiple replicas each handling only one request at a time, but using a thread pool improves throughput by taking advantage of the fact that most web applications are blocked on I/O most of the time (usually waiting for a response from a database or another web service).
-        
-        ## Why Twisted?
-        
-        Gunicorn itself does have a threadpool mode, however it's somewhat awkward to work with as it uses the `futures` ThreadPool implementation. Twisted's ThreadPool is more efficent. This also allows installing the Prometheus metrics as a native Twisted web handler so it will work even if the threadpool is exhausted, meaning your metrics keep working even during a system overload.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: tests
+License-File: LICENSE
+
+# Kubernetes_WSGI
+
+A wrapper for running your Python web application using Twisted in a way that works well for Kubernetes.
+
+This also includes Prometheus metrics support.
+
+## Quick Start
+
+To install:
+
+```
+pip install kubernetes-wsgi
+```
+
+To launch your application:
+
+```
+python -m kubernetes_wsgi myapp --port 8000
+```
+
+where `myapp` is an importable module name containing your WSGI application function.
+
+## Why Threads?
+
+The gold standard for Python WSGI servers is Gunicorn, renowned for its multi-process execution mode for effcient concurrency despite the dreaded Python GIL (Global Interpreter Lock). Unfortunately when working with containers, multi-process worker models can be difficult to work with as containers generally expect to only have a single process. Specifically this means if one of the forked workers is hit by an OOM and killed, the main process will simply restart it without triggering the usual metrics in Kubernetes for OOM'd Pods. Similarly we have a different way to handle multi-process concurrency in Kubernetes, through a Deployment with many replicas. In the simplest version would could use multiple replicas each handling only one request at a time, but using a thread pool improves throughput by taking advantage of the fact that most web applications are blocked on I/O most of the time (usually waiting for a response from a database or another web service).
+
+## Why Twisted?
+
+Gunicorn itself does have a threadpool mode, however it's somewhat awkward to work with as it uses the `futures` ThreadPool implementation. Twisted's ThreadPool is more efficent. This also allows installing the Prometheus metrics as a native Twisted web handler so it will work even if the threadpool is exhausted, meaning your metrics keep working even during a system overload.
```

### Comparing `kubernetes_wsgi-1.1/src/kubernetes_wsgi.egg-info/SOURCES.txt` & `kubernetes_wsgi-1.2/src/kubernetes_wsgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/tests/test_main.py` & `kubernetes_wsgi-1.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/tests/test_server.py` & `kubernetes_wsgi-1.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `kubernetes_wsgi-1.1/tox.ini` & `kubernetes_wsgi-1.2/tox.ini`

 * *Files identical despite different names*

