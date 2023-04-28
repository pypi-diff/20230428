# Comparing `tmp/rele-1.7.0.tar.gz` & `tmp/rele-1.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rele-1.7.0.tar", last modified: Tue Nov 15 10:48:51 2022, max compression
+gzip compressed data, was "rele-1.8.0b0.tar", last modified: Fri Apr 28 09:33:41 2023, max compression
```

## Comparing `rele-1.7.0.tar` & `rele-1.8.0b0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.688318 rele-1.7.0/
--rw-r--r--   0 danielruiz   (501) staff       (20)     4707 2022-11-15 10:48:51.688516 rele-1.7.0/PKG-INFO
--rw-r--r--   0 danielruiz   (501) staff       (20)     2830 2022-04-13 13:52:50.000000 rele-1.7.0/README.md
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.675898 rele-1.7.0/rele/
--rw-r--r--   0 danielruiz   (501) staff       (20)      390 2022-11-15 10:47:26.000000 rele-1.7.0/rele/__init__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1453 2022-04-13 13:52:50.000000 rele-1.7.0/rele/__main__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      199 2022-04-13 13:52:50.000000 rele-1.7.0/rele/apps.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     7842 2022-11-15 09:32:09.000000 rele-1.7.0/rele/client.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     4289 2022-11-15 09:32:09.000000 rele-1.7.0/rele/config.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.682760 rele-1.7.0/rele/contrib/
--rw-r--r--   0 danielruiz   (501) staff       (20)      355 2022-04-13 13:52:50.000000 rele-1.7.0/rele/contrib/__init__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      400 2022-04-13 13:52:50.000000 rele-1.7.0/rele/contrib/django_db_middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      347 2022-04-13 13:52:50.000000 rele-1.7.0/rele/contrib/flask_middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     3860 2022-11-14 18:37:23.000000 rele-1.7.0/rele/contrib/logging_middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      306 2022-04-13 13:52:50.000000 rele-1.7.0/rele/contrib/unrecoverable_middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1224 2022-11-14 18:37:23.000000 rele-1.7.0/rele/contrib/verbose_logging_middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1840 2022-04-13 13:52:50.000000 rele-1.7.0/rele/discover.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.683575 rele-1.7.0/rele/management/
--rw-r--r--   0 danielruiz   (501) staff       (20)        0 2019-06-12 09:20:33.000000 rele-1.7.0/rele/management/__init__.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.685202 rele-1.7.0/rele/management/commands/
--rw-r--r--   0 danielruiz   (501) staff       (20)        0 2019-06-12 09:20:33.000000 rele-1.7.0/rele/management/commands/__init__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1089 2022-04-13 13:52:50.000000 rele-1.7.0/rele/management/commands/runrele.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      728 2022-04-13 13:52:50.000000 rele-1.7.0/rele/management/commands/showsubscriptions.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      537 2022-04-13 13:52:50.000000 rele-1.7.0/rele/management/discover.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     3486 2022-04-13 13:52:50.000000 rele-1.7.0/rele/middleware.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1581 2022-11-15 09:32:09.000000 rele-1.7.0/rele/publishing.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     6820 2022-11-14 18:37:23.000000 rele-1.7.0/rele/subscription.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     5454 2022-11-14 18:37:23.000000 rele-1.7.0/rele/worker.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.678773 rele-1.7.0/rele.egg-info/
--rw-r--r--   0 danielruiz   (501) staff       (20)     4707 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/PKG-INFO
--rw-r--r--   0 danielruiz   (501) staff       (20)      933 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/SOURCES.txt
--rw-r--r--   0 danielruiz   (501) staff       (20)        1 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/dependency_links.txt
--rw-r--r--   0 danielruiz   (501) staff       (20)       49 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/entry_points.txt
--rw-r--r--   0 danielruiz   (501) staff       (20)        1 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/not-zip-safe
--rw-r--r--   0 danielruiz   (501) staff       (20)       80 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/requires.txt
--rw-r--r--   0 danielruiz   (501) staff       (20)       11 2022-11-15 10:48:51.000000 rele-1.7.0/rele.egg-info/top_level.txt
--rw-r--r--   0 danielruiz   (501) staff       (20)      446 2022-11-15 10:48:51.689132 rele-1.7.0/setup.cfg
--rw-r--r--   0 danielruiz   (501) staff       (20)     2227 2022-04-13 13:52:50.000000 rele-1.7.0/setup.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.667716 rele-1.7.0/tests/
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.686858 rele-1.7.0/tests/commands/
--rw-r--r--   0 danielruiz   (501) staff       (20)        0 2022-04-13 13:52:50.000000 rele-1.7.0/tests/commands/__init__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1314 2022-04-13 13:52:50.000000 rele-1.7.0/tests/commands/test_runrele.py
--rw-r--r--   0 danielruiz   (501) staff       (20)     1602 2022-04-13 13:52:50.000000 rele-1.7.0/tests/commands/test_showsubscriptions.py
-drwxr-xr-x   0 danielruiz   (501) staff       (20)        0 2022-11-15 10:48:51.687656 rele-1.7.0/tests/more_subs/
--rw-r--r--   0 danielruiz   (501) staff       (20)        0 2022-04-13 13:52:50.000000 rele-1.7.0/tests/more_subs/__init__.py
--rw-r--r--   0 danielruiz   (501) staff       (20)      131 2022-04-13 13:52:50.000000 rele-1.7.0/tests/more_subs/subs.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.293461 rele-1.8.0b0/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      566 2023-04-24 09:02:19.000000 rele-1.8.0b0/AUTHORS.md
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)    11352 2023-04-24 09:02:19.000000 rele-1.8.0b0/LICENSE
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3969 2023-04-28 09:33:41.293582 rele-1.8.0b0/PKG-INFO
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     2830 2023-04-24 09:02:19.000000 rele-1.8.0b0/README.md
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       76 2023-04-24 09:02:19.000000 rele-1.8.0b0/pyproject.toml
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.286390 rele-1.8.0b0/rele/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      395 2023-04-28 09:19:11.000000 rele-1.8.0b0/rele/__init__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1453 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/__main__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      199 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/apps.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     8719 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/client.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     4352 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/config.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.290519 rele-1.8.0b0/rele/contrib/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      355 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/__init__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      400 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/django_db_middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      347 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/flask_middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3860 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/logging_middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      306 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/unrecoverable_middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1224 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/verbose_logging_middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1840 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/discover.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.291019 rele-1.8.0b0/rele/management/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/__init__.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.291830 rele-1.8.0b0/rele/management/commands/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/__init__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1089 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/runrele.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      728 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/showsubscriptions.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      537 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/discover.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3486 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/middleware.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1581 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/publishing.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1118 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/retry_policy.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     7182 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/subscription.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     5562 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/worker.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.288534 rele-1.8.0b0/rele.egg-info/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3969 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/PKG-INFO
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      988 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/SOURCES.txt
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        1 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/dependency_links.txt
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       49 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/entry_points.txt
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        1 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/not-zip-safe
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       80 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/requires.txt
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       11 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/top_level.txt
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      446 2023-04-28 09:33:41.294105 rele-1.8.0b0/setup.cfg
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     2227 2023-04-24 09:02:19.000000 rele-1.8.0b0/setup.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.277934 rele-1.8.0b0/tests/
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.292636 rele-1.8.0b0/tests/commands/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/commands/__init__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1326 2023-04-28 09:05:12.000000 rele-1.8.0b0/tests/commands/test_runrele.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1602 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/commands/test_showsubscriptions.py
+drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.293187 rele-1.8.0b0/tests/more_subs/
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/more_subs/__init__.py
+-rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      131 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/more_subs/subs.py
```

### Comparing `rele-1.7.0/PKG-INFO` & `rele-1.8.0b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,15 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.7.0
+Version: 1.8.0b0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
-Description: <p align="center">
-            <img src="docs/_static/rele_logo.png" align="center" height="200">
-        </p>
-        
-        <p align="center">
-            <strong>
-                Relé makes integration with Google PubSub straightforward and easy.
-            </strong>
-        </p>
-        
-        <p align="center">
-            <a href="https://travis-ci.org/mercadona/rele">
-                <img src="https://travis-ci.org/mercadona/rele.svg?branch=master"
-                     alt="Build Status">
-            </a>
-            <a href="https://mercadonarele.readthedocs.io/en/latest/?badge=latest">
-                <img src="https://readthedocs.org/projects/mercadonarele/badge/?version=latest"
-                     alt="Read the Docs">
-            </a>
-            <a href="https://codecov.io/gh/mercadona/rele">
-                <img src="https://codecov.io/gh/mercadona/rele/branch/master/graph/badge.svg"
-                     alt="Code Coverage">
-            </a>
-            <a href="https://pypi.org/project/rele/">
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rele.svg">
-            </a>
-            <a href="https://pypi.org/project/rele/">
-                <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/rele">
-            </a>
-        </p>
-        
-        
-        ## Motivation and Features
-        
-        The [Publish-Subscribe pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) 
-        and specifically the Google Cloud [Pub/Sub library](https://pypi.org/project/google-cloud-pubsub/) 
-        are very powerful tools but you can easily cut your fingers on it. Relé makes integration 
-        seamless by providing Publisher, Subscriber and Worker classes with the following features:
-        
-        * Powerful Publishing API
-        * Highly Scalable Worker
-        * Intuitive Subscription Management
-        * Easily Extensible Middleware
-        * Ready to go Django/Flask integration
-        * CLI
-        * And much more!
-        
-        ## What it looks like
-        
-        ```python
-        # Publish to the topic
-        import rele
-        
-        rele.publish(topic='photo-uploaded', data={'customer_id': 123})
-        
-        # Subscribe to the Pub/Sub topic
-        from rele import sub
-        
-        @sub(topic='photo-uploaded')
-        def photo_uploaded(data, **kwargs):
-            print(f"Customer {data['customer_id']} has uploaded an image")
-        ```
-        
-        ## What's in the name
-        
-        "Relé" is Spanish for *relay*, a technology that 
-        [has played a key role](https://technicshistory.wordpress.com/2017/01/29/the-relay/) in 
-        history in the evolution of communication and electrical technology, including the telegraph, 
-        telephone, electricity transmission, and transistors.
-        
-        ## Install
-        
-        Relé supports Python 3.6+ and installing via ``pip``
-        
-        `pip install rele`
-        
-        or with Django integration
-        
-        `pip install rele[django]`
-        
-        or with Flask integration
-        
-        `pip install rele[flask]`
-        
-        ## Quickstart
-        
-        [Please see our documentation to get started.](https://mercadonarele.readthedocs.io/en/latest/guides/basics.html) 
-        
-        You can also read more about it [here](https://medium.com/mercadona-tech/announcing-rel%C3%A9-c2d0540af3b9)
-        
-        ----
-        
-        ## Running Tests
-        
-        Does the code actually work?
-        
-              make test
-        
 Keywords: rele
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
@@ -121,7 +23,109 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: django
 Provides-Extra: flask
+License-File: LICENSE
+License-File: AUTHORS.md
+
+<p align="center">
+    <img src="docs/_static/rele_logo.png" align="center" height="200">
+</p>
+
+<p align="center">
+    <strong>
+        Relé makes integration with Google PubSub straightforward and easy.
+    </strong>
+</p>
+
+<p align="center">
+    <a href="https://travis-ci.org/mercadona/rele">
+        <img src="https://travis-ci.org/mercadona/rele.svg?branch=master"
+             alt="Build Status">
+    </a>
+    <a href="https://mercadonarele.readthedocs.io/en/latest/?badge=latest">
+        <img src="https://readthedocs.org/projects/mercadonarele/badge/?version=latest"
+             alt="Read the Docs">
+    </a>
+    <a href="https://codecov.io/gh/mercadona/rele">
+        <img src="https://codecov.io/gh/mercadona/rele/branch/master/graph/badge.svg"
+             alt="Code Coverage">
+    </a>
+    <a href="https://pypi.org/project/rele/">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rele.svg">
+    </a>
+    <a href="https://pypi.org/project/rele/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/rele">
+    </a>
+</p>
+
+
+## Motivation and Features
+
+The [Publish-Subscribe pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) 
+and specifically the Google Cloud [Pub/Sub library](https://pypi.org/project/google-cloud-pubsub/) 
+are very powerful tools but you can easily cut your fingers on it. Relé makes integration 
+seamless by providing Publisher, Subscriber and Worker classes with the following features:
+
+* Powerful Publishing API
+* Highly Scalable Worker
+* Intuitive Subscription Management
+* Easily Extensible Middleware
+* Ready to go Django/Flask integration
+* CLI
+* And much more!
+
+## What it looks like
+
+```python
+# Publish to the topic
+import rele
+
+rele.publish(topic='photo-uploaded', data={'customer_id': 123})
+
+# Subscribe to the Pub/Sub topic
+from rele import sub
+
+@sub(topic='photo-uploaded')
+def photo_uploaded(data, **kwargs):
+    print(f"Customer {data['customer_id']} has uploaded an image")
+```
+
+## What's in the name
+
+"Relé" is Spanish for *relay*, a technology that 
+[has played a key role](https://technicshistory.wordpress.com/2017/01/29/the-relay/) in 
+history in the evolution of communication and electrical technology, including the telegraph, 
+telephone, electricity transmission, and transistors.
+
+## Install
+
+Relé supports Python 3.6+ and installing via ``pip``
+
+`pip install rele`
+
+or with Django integration
+
+`pip install rele[django]`
+
+or with Flask integration
+
+`pip install rele[flask]`
+
+## Quickstart
+
+[Please see our documentation to get started.](https://mercadonarele.readthedocs.io/en/latest/guides/basics.html) 
+
+You can also read more about it [here](https://medium.com/mercadona-tech/announcing-rel%C3%A9-c2d0540af3b9)
+
+----
+
+## Running Tests
+
+Does the code actually work?
+
+      make test
+
+
```

### Comparing `rele-1.7.0/README.md` & `rele-1.8.0b0/README.md`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/__main__.py` & `rele-1.8.0b0/rele/__main__.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/client.py` & `rele-1.8.0b0/rele/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import time
 from concurrent.futures import TimeoutError
 from contextlib import suppress
 
 import google.auth
 from google.api_core import exceptions
 from google.cloud import pubsub_v1
+from google.protobuf import duration_pb2
+from google.pubsub_v1 import RetryPolicy as GCloudRetryPolicy
 
 from rele.middleware import run_middleware_hook
 
 logger = logging.getLogger(__name__)
 
 USE_EMULATOR = True if os.environ.get("PUBSUB_EMULATOR_HOST") else False
 DEFAULT_ENCODER_PATH = "json.JSONEncoder"
@@ -32,32 +34,39 @@
 
     For convenience, this class wraps the creation and consumption of a topic
     subscription.
 
     :param gc_project_id: str :ref:`settings_project_id` .
     :param credentials: obj :meth:`~rele.config.Config.credentials`.
     :param default_ack_deadline: int Ack Deadline defined in settings
+    :param default_retry_policy: RetryPolicy Rele's RetryPolicy defined in settings
     """
 
-    def __init__(self, gc_project_id, credentials, default_ack_deadline=None):
+    def __init__(
+        self,
+        gc_project_id,
+        credentials,
+        default_ack_deadline=None,
+        default_retry_policy=None,
+    ):
         self._gc_project_id = gc_project_id
         self._ack_deadline = default_ack_deadline or DEFAULT_ACK_DEADLINE
         self.credentials = credentials if not USE_EMULATOR else None
         self._client = pubsub_v1.SubscriberClient(credentials=credentials)
+        self._retry_policy = default_retry_policy
 
     def create_subscription(self, subscription):
         """Handles creating the subscription when it does not exists.
 
         This makes it easier to deploy a worker and forget about the
         subscription side of things. The subscription must
         have a topic to subscribe to. Which means that the topic must be
         created manually before the worker is started.
 
-        :param subscription: str Subscription name
-        :param topic: str Topic name to subscribe
+        :param subscription: obj :class:`~rele.subscription.Subscription`.
         """
         subscription_path = self._client.subscription_path(
             self._gc_project_id, subscription.name
         )
         topic_path = self._client.topic_path(self._gc_project_id, subscription.topic)
 
         with suppress(exceptions.AlreadyExists):
@@ -82,16 +91,33 @@
             "topic": topic_path,
             "ack_deadline_seconds": self._ack_deadline,
         }
 
         if subscription.backend_filter_by:
             request["filter"] = subscription.backend_filter_by
 
+        retry_policy = subscription.retry_policy or self._retry_policy
+
+        if retry_policy:
+            request["retry_policy"] = self._build_gcloud_retry_policy(retry_policy)
+
         self._client.create_subscription(request=request)
 
+    def _build_gcloud_retry_policy(self, rele_retry_policy):
+        minimum_backoff = duration_pb2.Duration(
+            seconds=rele_retry_policy.minimum_backoff
+        )
+        maximum_backoff = duration_pb2.Duration(
+            seconds=rele_retry_policy.maximum_backoff
+        )
+
+        return GCloudRetryPolicy(
+            minimum_backoff=minimum_backoff, maximum_backoff=maximum_backoff
+        )
+
     def consume(self, subscription_name, callback, scheduler):
         """Begin listening to topic from the SubscriberClient.
 
         :param subscription_name: str Subscription name
         :param callback: Function which act on a topic message
         :param scheduler: `Thread pool-based scheduler. <https://googleapis.dev/python/pubsub/latest/subscriber/api/scheduler.html?highlight=threadscheduler#google.cloud.pubsub_v1.subscriber.scheduler.ThreadScheduler>`_  # noqa
         :return: `Future <https://googleapis.github.io/google-cloud-python/latest/pubsub/subscriber/api/futures.html>`_  # noqa
```

### Comparing `rele-1.7.0/rele/config.py` & `rele-1.8.0b0/rele/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         )
         self.publisher_blocking = setting.get("PUBLISHER_BLOCKING", DEFAULT_BLOCKING)
         self._encoder_path = setting.get("ENCODER_PATH", DEFAULT_ENCODER_PATH)
         self.publisher_timeout = setting.get("PUBLISHER_TIMEOUT", 3.0)
         self.threads_per_subscription = setting.get("THREADS_PER_SUBSCRIPTION", 2)
         self.filter_by = setting.get("FILTER_SUBS_BY")
         self._credentials = None
+        self.retry_policy = setting.get("DEFAULT_RETRY_POLICY")
 
     @property
     def encoder(self):
         module_name, class_name = self._encoder_path.rsplit(".", 1)
         module = importlib.import_module(module_name)
         return getattr(module, class_name)
 
@@ -93,15 +94,14 @@
     except TypeError:
         # If attribute is not a class, TypeError is raised when testing issubclass
         return None
     return subscription
 
 
 def load_subscriptions_from_paths(sub_module_paths, sub_prefix=None, filter_by=None):
-
     subscriptions = {}
     for sub_module_path in sub_module_paths:
         sub_module = importlib.import_module(sub_module_path)
         for attr_name in dir(sub_module):
             attribute = getattr(sub_module, attr_name)
 
             subscription = subscription_from_attribute(attribute)
```

### Comparing `rele-1.7.0/rele/contrib/logging_middleware.py` & `rele-1.8.0b0/rele/contrib/logging_middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/contrib/verbose_logging_middleware.py` & `rele-1.8.0b0/rele/contrib/verbose_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/discover.py` & `rele-1.8.0b0/rele/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/management/commands/runrele.py` & `rele-1.8.0b0/rele/management/commands/runrele.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/management/commands/showsubscriptions.py` & `rele-1.8.0b0/rele/management/commands/showsubscriptions.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/management/discover.py` & `rele-1.8.0b0/rele/management/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/middleware.py` & `rele-1.8.0b0/rele/middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/publishing.py` & `rele-1.8.0b0/rele/publishing.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/rele/subscription.py` & `rele-1.8.0b0/rele/subscription.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,33 +31,44 @@
 
     If ``rele-cli run`` is used, the ``DoSomethingSub`` will be a valid subscription
     and registered on Google Cloud.
 
     """
 
     def __init__(
-        self, func, topic, prefix="", suffix="", filter_by=None, backend_filter_by=None
+        self,
+        func,
+        topic,
+        prefix="",
+        suffix="",
+        filter_by=None,
+        backend_filter_by=None,
+        retry_policy=None,
     ):
+        self._validate_filter_by(filter_by)
+
         self._func = func
         self.topic = topic
         self._prefix = prefix
         self._suffix = suffix
         self._filters = self._init_filters(filter_by)
         self.backend_filter_by = backend_filter_by
+        self.retry_policy = retry_policy
 
-    def _init_filters(self, filter_by):
+    def _validate_filter_by(self, filter_by):
         if filter_by and not (
             callable(filter_by)
             or (
                 isinstance(filter_by, Iterable)
                 and all(callable(filter) for filter in filter_by)
             )
         ):
             raise ValueError("Filter_by must be a callable or a list of callables.")
 
+    def _init_filters(self, filter_by):
         if isinstance(filter_by, Iterable):
             return filter_by
         elif filter_by:
             return [filter_by]
 
         return None
 
@@ -141,15 +152,22 @@
                 message,
             )
             return res
         finally:
             run_middleware_hook("post_process_message")
 
 
-def sub(topic, prefix=None, suffix=None, filter_by=None, backend_filter_by=None):
+def sub(
+    topic,
+    prefix=None,
+    suffix=None,
+    filter_by=None,
+    backend_filter_by=None,
+    retry_policy=None,
+):
     """Decorator function that makes declaring a PubSub Subscription simple.
 
     The Subscriber returned will automatically create and name
     the subscription for the topic.
     The subscription name will be the topic name prefixed by the project name.
 
     For example, if the topic name to subscribe too is `lets-tell-everyone`,
@@ -186,14 +204,15 @@
                    Useful to namespace your subscription with your project name
     :param suffix: string An optional suffix to the subscription name.
                    Useful when you have two subscribers in the same project
                    that are subscribed to the same topic.
     :param filter_by: Union[function, list] An optional function or tuple of
                       functions that filters the messages to be processed by
                       the sub regarding their attributes.
+    :param retry_policy: obj :class:`~rele.retry_policy.RetryPolicy`
     :return: :class:`~rele.subscription.Subscription`
     """
 
     def decorator(func):
         args_spec = getfullargspec(func)
         if len(args_spec.args) != 1 or not args_spec.varkw:
             raise RuntimeError(
@@ -210,10 +229,11 @@
         return Subscription(
             func=func,
             topic=topic,
             prefix=prefix,
             suffix=suffix,
             filter_by=filter_by,
             backend_filter_by=backend_filter_by,
+            retry_policy=retry_policy,
         )
 
     return decorator
```

### Comparing `rele-1.7.0/rele/worker.py` & `rele-1.8.0b0/rele/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,19 @@
     def __init__(
         self,
         subscriptions,
         gc_project_id=None,
         credentials=None,
         default_ack_deadline=None,
         threads_per_subscription=None,
+        default_retry_policy=None,
     ):
-        self._subscriber = Subscriber(gc_project_id, credentials, default_ack_deadline)
+        self._subscriber = Subscriber(
+            gc_project_id, credentials, default_ack_deadline, default_retry_policy
+        )
         self._futures = {}
         self._subscriptions = subscriptions
         self.threads_per_subscription = threads_per_subscription
 
     def setup(self):
         """Create the subscriptions on a Google PubSub topic.
 
@@ -148,14 +151,15 @@
         print(f"  {sub}")
     worker = Worker(
         subs,
         config.gc_project_id,
         config.credentials,
         config.ack_deadline,
         config.threads_per_subscription,
+        config.retry_policy,
     )
 
     # to allow killing runrele worker via ctrl+c
     signal.signal(signal.SIGINT, worker.stop)
     signal.signal(signal.SIGTERM, worker.stop)
     signal.signal(_get_stop_signal(), worker.stop)
```

### Comparing `rele-1.7.0/rele.egg-info/PKG-INFO` & `rele-1.8.0b0/rele.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,15 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.7.0
+Version: 1.8.0b0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
-Description: <p align="center">
-            <img src="docs/_static/rele_logo.png" align="center" height="200">
-        </p>
-        
-        <p align="center">
-            <strong>
-                Relé makes integration with Google PubSub straightforward and easy.
-            </strong>
-        </p>
-        
-        <p align="center">
-            <a href="https://travis-ci.org/mercadona/rele">
-                <img src="https://travis-ci.org/mercadona/rele.svg?branch=master"
-                     alt="Build Status">
-            </a>
-            <a href="https://mercadonarele.readthedocs.io/en/latest/?badge=latest">
-                <img src="https://readthedocs.org/projects/mercadonarele/badge/?version=latest"
-                     alt="Read the Docs">
-            </a>
-            <a href="https://codecov.io/gh/mercadona/rele">
-                <img src="https://codecov.io/gh/mercadona/rele/branch/master/graph/badge.svg"
-                     alt="Code Coverage">
-            </a>
-            <a href="https://pypi.org/project/rele/">
-                <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rele.svg">
-            </a>
-            <a href="https://pypi.org/project/rele/">
-                <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/rele">
-            </a>
-        </p>
-        
-        
-        ## Motivation and Features
-        
-        The [Publish-Subscribe pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) 
-        and specifically the Google Cloud [Pub/Sub library](https://pypi.org/project/google-cloud-pubsub/) 
-        are very powerful tools but you can easily cut your fingers on it. Relé makes integration 
-        seamless by providing Publisher, Subscriber and Worker classes with the following features:
-        
-        * Powerful Publishing API
-        * Highly Scalable Worker
-        * Intuitive Subscription Management
-        * Easily Extensible Middleware
-        * Ready to go Django/Flask integration
-        * CLI
-        * And much more!
-        
-        ## What it looks like
-        
-        ```python
-        # Publish to the topic
-        import rele
-        
-        rele.publish(topic='photo-uploaded', data={'customer_id': 123})
-        
-        # Subscribe to the Pub/Sub topic
-        from rele import sub
-        
-        @sub(topic='photo-uploaded')
-        def photo_uploaded(data, **kwargs):
-            print(f"Customer {data['customer_id']} has uploaded an image")
-        ```
-        
-        ## What's in the name
-        
-        "Relé" is Spanish for *relay*, a technology that 
-        [has played a key role](https://technicshistory.wordpress.com/2017/01/29/the-relay/) in 
-        history in the evolution of communication and electrical technology, including the telegraph, 
-        telephone, electricity transmission, and transistors.
-        
-        ## Install
-        
-        Relé supports Python 3.6+ and installing via ``pip``
-        
-        `pip install rele`
-        
-        or with Django integration
-        
-        `pip install rele[django]`
-        
-        or with Flask integration
-        
-        `pip install rele[flask]`
-        
-        ## Quickstart
-        
-        [Please see our documentation to get started.](https://mercadonarele.readthedocs.io/en/latest/guides/basics.html) 
-        
-        You can also read more about it [here](https://medium.com/mercadona-tech/announcing-rel%C3%A9-c2d0540af3b9)
-        
-        ----
-        
-        ## Running Tests
-        
-        Does the code actually work?
-        
-              make test
-        
 Keywords: rele
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
@@ -121,7 +23,109 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: django
 Provides-Extra: flask
+License-File: LICENSE
+License-File: AUTHORS.md
+
+<p align="center">
+    <img src="docs/_static/rele_logo.png" align="center" height="200">
+</p>
+
+<p align="center">
+    <strong>
+        Relé makes integration with Google PubSub straightforward and easy.
+    </strong>
+</p>
+
+<p align="center">
+    <a href="https://travis-ci.org/mercadona/rele">
+        <img src="https://travis-ci.org/mercadona/rele.svg?branch=master"
+             alt="Build Status">
+    </a>
+    <a href="https://mercadonarele.readthedocs.io/en/latest/?badge=latest">
+        <img src="https://readthedocs.org/projects/mercadonarele/badge/?version=latest"
+             alt="Read the Docs">
+    </a>
+    <a href="https://codecov.io/gh/mercadona/rele">
+        <img src="https://codecov.io/gh/mercadona/rele/branch/master/graph/badge.svg"
+             alt="Code Coverage">
+    </a>
+    <a href="https://pypi.org/project/rele/">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rele.svg">
+    </a>
+    <a href="https://pypi.org/project/rele/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/rele">
+    </a>
+</p>
+
+
+## Motivation and Features
+
+The [Publish-Subscribe pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) 
+and specifically the Google Cloud [Pub/Sub library](https://pypi.org/project/google-cloud-pubsub/) 
+are very powerful tools but you can easily cut your fingers on it. Relé makes integration 
+seamless by providing Publisher, Subscriber and Worker classes with the following features:
+
+* Powerful Publishing API
+* Highly Scalable Worker
+* Intuitive Subscription Management
+* Easily Extensible Middleware
+* Ready to go Django/Flask integration
+* CLI
+* And much more!
+
+## What it looks like
+
+```python
+# Publish to the topic
+import rele
+
+rele.publish(topic='photo-uploaded', data={'customer_id': 123})
+
+# Subscribe to the Pub/Sub topic
+from rele import sub
+
+@sub(topic='photo-uploaded')
+def photo_uploaded(data, **kwargs):
+    print(f"Customer {data['customer_id']} has uploaded an image")
+```
+
+## What's in the name
+
+"Relé" is Spanish for *relay*, a technology that 
+[has played a key role](https://technicshistory.wordpress.com/2017/01/29/the-relay/) in 
+history in the evolution of communication and electrical technology, including the telegraph, 
+telephone, electricity transmission, and transistors.
+
+## Install
+
+Relé supports Python 3.6+ and installing via ``pip``
+
+`pip install rele`
+
+or with Django integration
+
+`pip install rele[django]`
+
+or with Flask integration
+
+`pip install rele[flask]`
+
+## Quickstart
+
+[Please see our documentation to get started.](https://mercadonarele.readthedocs.io/en/latest/guides/basics.html) 
+
+You can also read more about it [here](https://medium.com/mercadona-tech/announcing-rel%C3%A9-c2d0540af3b9)
+
+----
+
+## Running Tests
+
+Does the code actually work?
+
+      make test
+
+
```

### Comparing `rele-1.7.0/rele.egg-info/SOURCES.txt` & `rele-1.8.0b0/rele.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+AUTHORS.md
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 rele/__init__.py
 rele/__main__.py
 rele/apps.py
 rele/client.py
 rele/config.py
 rele/discover.py
 rele/middleware.py
 rele/publishing.py
+rele/retry_policy.py
 rele/subscription.py
 rele/worker.py
 rele.egg-info/PKG-INFO
 rele.egg-info/SOURCES.txt
 rele.egg-info/dependency_links.txt
 rele.egg-info/entry_points.txt
 rele.egg-info/not-zip-safe
```

### Comparing `rele-1.7.0/setup.py` & `rele-1.8.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `rele-1.7.0/tests/commands/test_runrele.py` & `rele-1.8.0b0/tests/commands/test_runrele.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     def mock_worker(self):
         with patch("rele.worker.Worker", autospec=True) as p:
             yield p
 
     def test_calls_worker_start_and_setup_when_runrele(self, mock_worker):
         call_command("runrele")
 
-        mock_worker.assert_called_with([], "rele-test", ANY, 60, 2)
+        mock_worker.assert_called_with([], "rele-test", ANY, 60, 2, None)
         mock_worker.return_value.run_forever.assert_called_once_with()
 
     def test_prints_warning_when_conn_max_age_not_set_to_zero(
         self, mock_worker, capsys, settings
     ):
         settings.DATABASES = {"default": {"CONN_MAX_AGE": 1}}
         call_command("runrele")
 
         out, err = capsys.readouterr()
         assert (
             "WARNING: settings.CONN_MAX_AGE is not set to 0. "
             "This may result in slots for database connections to "
             "be exhausted." in err
         )
-        mock_worker.assert_called_with([], "rele-test", ANY, 60, 2)
+        mock_worker.assert_called_with([], "rele-test", ANY, 60, 2, None)
         mock_worker.return_value.run_forever.assert_called_once_with()
```

### Comparing `rele-1.7.0/tests/commands/test_showsubscriptions.py` & `rele-1.8.0b0/tests/commands/test_showsubscriptions.py`

 * *Files identical despite different names*

