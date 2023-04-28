# Comparing `tmp/prometheus_flask_exporter-0.9.1.tar.gz` & `tmp/prometheus_flask_exporter-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prometheus_flask_exporter-0.9.1.tar", last modified: Fri Aug  9 11:21:57 2019, max compression
+gzip compressed data, was "dist/prometheus_flask_exporter-0.9.3.tar", last modified: Thu Sep 26 13:39:55 2019, max compression
```

## Comparing `prometheus_flask_exporter-0.9.1.tar` & `prometheus_flask_exporter-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    14497 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11224 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20944 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9322 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter/multiprocess.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14497 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-08-09 11:21:57.000000 prometheus_flask_exporter-0.9.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1312 2019-08-09 11:21:41.000000 prometheus_flask_exporter-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14834 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11521 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21764 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9322 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter/multiprocess.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14834 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      362 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-09-26 13:39:55.000000 prometheus_flask_exporter-0.9.3/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1312 2019-09-26 13:39:39.000000 prometheus_flask_exporter-0.9.3/setup.py
```

### Comparing `prometheus_flask_exporter-0.9.1/LICENSE` & `prometheus_flask_exporter-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_flask_exporter-0.9.1/PKG-INFO` & `prometheus_flask_exporter-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prometheus_flask_exporter
-Version: 0.9.1
+Version: 0.9.3
 Summary: Prometheus metrics exporter for Flask
 Home-page: https://github.com/rycus86/prometheus_flask_exporter
 Author: Viktor Adam
 Author-email: rycus86@gmail.com
 License: MIT
-Download-URL: https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.1.tar.gz
+Download-URL: https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.3.tar.gz
 Description: # Prometheus Flask exporter
         
         [![PyPI](https://img.shields.io/pypi/v/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![PyPI](https://img.shields.io/pypi/pyversions/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![Travis](https://img.shields.io/travis/rycus86/prometheus_flask_exporter.svg)](https://travis-ci.org/rycus86/prometheus_flask_exporter)
         [![Coverage Status](https://coveralls.io/repos/github/rycus86/prometheus_flask_exporter/badge.svg?branch=master)](https://coveralls.io/github/rycus86/prometheus_flask_exporter?branch=master)
@@ -76,14 +76,19 @@
           Total number of HTTP requests for all Flask requests.
         - `flask_exporter_info` (Gauge)
           Information about the Prometheus Flask exporter itself (e.g. `version`).
         
         The prefix for the default metrics can be controlled by the `defaults_prefix` parameter.
         Is you don't want to use any prefix, pass the `prometheus_flask_exporter.NO_PREFIX` value in.
         
+        You can avoid recording metrics on individual endpoints by decorating them
+        with `@metrics.do_not_track()`, or use the `excluded_paths` argument when
+        creating the `PrometheusMetrics` instance that takes a regular expression
+        (either a single string, or a list) and matching paths will be excluded.
+        
         ## Configuration
         
         By default, the metrics are exposed on the same Flask application on the
         `/metrics` endpoint and using the core Prometheus registry.
         If this doesn't suit your needs, set the `path` argument to `None` and/or
         the `export_defaults` argument to `False` plus change the `registry`
         argument if needed.
```

### Comparing `prometheus_flask_exporter-0.9.1/README.md` & `prometheus_flask_exporter-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
   Total number of HTTP requests for all Flask requests.
 - `flask_exporter_info` (Gauge)
   Information about the Prometheus Flask exporter itself (e.g. `version`).
 
 The prefix for the default metrics can be controlled by the `defaults_prefix` parameter.
 Is you don't want to use any prefix, pass the `prometheus_flask_exporter.NO_PREFIX` value in.
 
+You can avoid recording metrics on individual endpoints by decorating them
+with `@metrics.do_not_track()`, or use the `excluded_paths` argument when
+creating the `PrometheusMetrics` instance that takes a regular expression
+(either a single string, or a list) and matching paths will be excluded.
+
 ## Configuration
 
 By default, the metrics are exposed on the same Flask application on the
 `/metrics` endpoint and using the core Prometheus registry.
 If this doesn't suit your needs, set the `path` argument to `None` and/or
 the `export_defaults` argument to `False` plus change the `registry`
 argument if needed.
```

### Comparing `prometheus_flask_exporter-0.9.1/prometheus_flask_exporter/__init__.py` & `prometheus_flask_exporter-0.9.3/prometheus_flask_exporter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import inspect
 import warnings
 import functools
 import threading
 from timeit import default_timer
 
 from flask import request, make_response, current_app
@@ -71,15 +72,15 @@
         - With a single argument that will be the Flask Response object
         - Without an argument, possibly to use with the Flask `request` object
     """
 
     def __init__(self, app, path='/metrics',
                  export_defaults=True, defaults_prefix='flask',
                  group_by='path', buckets=None, static_labels=None,
-                 registry=None, **kwargs):
+                 excluded_paths=None, registry=None, **kwargs):
         """
         Create a new Prometheus metrics export configuration.
 
         :param app: the Flask application
         :param path: the metrics path (defaults to `/metrics`)
         :param export_defaults: expose all HTTP request latencies
             and number of HTTP requests
@@ -90,14 +91,16 @@
         :param group_by: group default HTTP metrics by
             this request property, like `path`, `endpoint`, `url_rule`, etc.
             (defaults to `path`)
         :param buckets: the time buckets for request latencies
             (will use the default when `None`)
         :param static_labels: static labels to attach to each of the
             metrics exposed by this `PrometheusMetrics` instance
+        :param excluded_paths: regular expression(s) as a string or
+            a list of strings for paths to exclude from tracking
         :param registry: the Prometheus Registry to use
         """
 
         self.app = app
         self.path = path
         self._export_defaults = export_defaults
         self._defaults_prefix = defaults_prefix or 'flask'
@@ -125,14 +128,24 @@
 
         elif group_by:
             self.group_by = group_by
 
         else:
             self.group_by = 'path'
 
+        if excluded_paths:
+            if PrometheusMetrics._is_string(excluded_paths):
+                excluded_paths = [excluded_paths]
+
+            self.excluded_paths = [
+                re.compile(p) for p in excluded_paths
+            ]
+        else:
+            self.excluded_paths = None
+
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
         """
         This callback can be used to initialize an application for the
         use with this prometheus reporter setup.
@@ -295,14 +308,18 @@
         def before_request():
             request.prom_start_time = default_timer()
 
         def after_request(response):
             if hasattr(request, 'prom_do_not_track'):
                 return response
 
+            if self.excluded_paths:
+                if any(pattern.match(request.path) for pattern in self.excluded_paths):
+                    return response
+
             if hasattr(request, 'prom_start_time'):
                 total_time = max(default_timer() - request.prom_start_time, 0)
 
                 if callable(duration_group):
                     group = duration_group(request)
                 else:
                     group = getattr(request, duration_group)
@@ -587,9 +604,16 @@
         if labels:
             gauge = gauge.labels(**labels)
 
         gauge.set(1)
 
         return gauge
 
+    @staticmethod
+    def _is_string(value):
+        try:
+            return isinstance(value, basestring)  # python2
+        except NameError:
+            return isinstance(value, str)  # python3
+
 
-__version__ = '0.9.1'
+__version__ = '0.9.3'
```

### Comparing `prometheus_flask_exporter-0.9.1/prometheus_flask_exporter/multiprocess.py` & `prometheus_flask_exporter-0.9.3/prometheus_flask_exporter/multiprocess.py`

 * *Files identical despite different names*

### Comparing `prometheus_flask_exporter-0.9.1/prometheus_flask_exporter.egg-info/PKG-INFO` & `prometheus_flask_exporter-0.9.3/prometheus_flask_exporter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prometheus-flask-exporter
-Version: 0.9.1
+Version: 0.9.3
 Summary: Prometheus metrics exporter for Flask
 Home-page: https://github.com/rycus86/prometheus_flask_exporter
 Author: Viktor Adam
 Author-email: rycus86@gmail.com
 License: MIT
-Download-URL: https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.1.tar.gz
+Download-URL: https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.3.tar.gz
 Description: # Prometheus Flask exporter
         
         [![PyPI](https://img.shields.io/pypi/v/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![PyPI](https://img.shields.io/pypi/pyversions/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/prometheus-flask-exporter.svg)](https://pypi.python.org/pypi/prometheus-flask-exporter)
         [![Travis](https://img.shields.io/travis/rycus86/prometheus_flask_exporter.svg)](https://travis-ci.org/rycus86/prometheus_flask_exporter)
         [![Coverage Status](https://coveralls.io/repos/github/rycus86/prometheus_flask_exporter/badge.svg?branch=master)](https://coveralls.io/github/rycus86/prometheus_flask_exporter?branch=master)
@@ -76,14 +76,19 @@
           Total number of HTTP requests for all Flask requests.
         - `flask_exporter_info` (Gauge)
           Information about the Prometheus Flask exporter itself (e.g. `version`).
         
         The prefix for the default metrics can be controlled by the `defaults_prefix` parameter.
         Is you don't want to use any prefix, pass the `prometheus_flask_exporter.NO_PREFIX` value in.
         
+        You can avoid recording metrics on individual endpoints by decorating them
+        with `@metrics.do_not_track()`, or use the `excluded_paths` argument when
+        creating the `PrometheusMetrics` instance that takes a regular expression
+        (either a single string, or a list) and matching paths will be excluded.
+        
         ## Configuration
         
         By default, the metrics are exposed on the same Flask application on the
         `/metrics` endpoint and using the core Prometheus registry.
         If this doesn't suit your needs, set the `path` argument to `None` and/or
         the `export_defaults` argument to `False` plus change the `registry`
         argument if needed.
```

### Comparing `prometheus_flask_exporter-0.9.1/setup.py` & `prometheus_flask_exporter-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='prometheus_flask_exporter',
     packages=['prometheus_flask_exporter'],
-    version='0.9.1',
+    version='0.9.3',
     description='Prometheus metrics exporter for Flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     author='Viktor Adam',
     author_email='rycus86@gmail.com',
     url='https://github.com/rycus86/prometheus_flask_exporter',
-    download_url='https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.1.tar.gz',
+    download_url='https://github.com/rycus86/prometheus_flask_exporter/archive/0.9.3.tar.gz',
     keywords=['prometheus', 'flask', 'monitoring', 'exporter'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Topic :: System :: Monitoring',
         'License :: OSI Approved :: MIT License',
```

