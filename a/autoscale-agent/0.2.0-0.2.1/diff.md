# Comparing `tmp/autoscale_agent-0.2.0.tar.gz` & `tmp/autoscale_agent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoscale_agent-0.2.0.tar", max compression
+gzip compressed data, was "autoscale_agent-0.2.1.tar", max compression
```

## Comparing `autoscale_agent-0.2.0.tar` & `autoscale_agent-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1081 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/LICENSE
--rw-r--r--   0        0        0     1567 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/README.md
--rw-r--r--   0        0        0      382 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/__init__.py
--rw-r--r--   0        0        0       38 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/agent.py
--rw-r--r--   0        0        0     1233 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/configuration.py
--rw-r--r--   0        0        0     1886 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/middleware/__init__.py
--rw-r--r--   0        0        0      983 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/middleware/django.py
--rw-r--r--   0        0        0     1215 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/middleware/flask.py
--rw-r--r--   0        0        0      814 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/util.py
--rw-r--r--   0        0        0     2172 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/web_dispatcher.py
--rw-r--r--   0        0        0      748 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/worker_dispatcher.py
--rw-r--r--   0        0        0      639 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/worker_dispatchers.py
--rw-r--r--   0        0        0      307 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/worker_server.py
--rw-r--r--   0        0        0      296 2023-04-25 10:00:38.849529 autoscale_agent-0.2.0/autoscale_agent/worker_servers.py
--rw-r--r--   0        0        0     1252 2023-04-25 10:00:38.853529 autoscale_agent-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 autoscale_agent-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1567 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/README.md
+-rw-r--r--   0        0        0      382 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/agent.py
+-rw-r--r--   0        0        0     1233 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/configuration.py
+-rw-r--r--   0        0        0     1886 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/middleware/__init__.py
+-rw-r--r--   0        0        0      983 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/middleware/django.py
+-rw-r--r--   0        0        0     1215 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/middleware/flask.py
+-rw-r--r--   0        0        0      814 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/util.py
+-rw-r--r--   0        0        0     2172 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/web_dispatcher.py
+-rw-r--r--   0        0        0      748 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/worker_dispatcher.py
+-rw-r--r--   0        0        0      639 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/worker_dispatchers.py
+-rw-r--r--   0        0        0      236 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/worker_server.py
+-rw-r--r--   0        0        0      296 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/autoscale_agent/worker_servers.py
+-rw-r--r--   0        0        0     1252 2023-04-28 10:16:47.856794 autoscale_agent-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 autoscale_agent-0.2.1/PKG-INFO
```

### Comparing `autoscale_agent-0.2.0/LICENSE` & `autoscale_agent-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/README.md` & `autoscale_agent-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/configuration.py` & `autoscale_agent-0.2.1/autoscale_agent/configuration.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/middleware/__init__.py` & `autoscale_agent-0.2.1/autoscale_agent/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/middleware/django.py` & `autoscale_agent-0.2.1/autoscale_agent/middleware/django.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/middleware/flask.py` & `autoscale_agent-0.2.1/autoscale_agent/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/util.py` & `autoscale_agent-0.2.1/autoscale_agent/util.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/web_dispatcher.py` & `autoscale_agent-0.2.1/autoscale_agent/web_dispatcher.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/worker_dispatcher.py` & `autoscale_agent-0.2.1/autoscale_agent/worker_dispatcher.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/autoscale_agent/worker_dispatchers.py` & `autoscale_agent-0.2.1/autoscale_agent/worker_dispatchers.py`

 * *Files identical despite different names*

### Comparing `autoscale_agent-0.2.0/pyproject.toml` & `autoscale_agent-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoscale-agent"
-version = "0.2.0"
+version = "0.2.1"
 description = "Provides Autoscale.app with the necessary metrics for autoscaling web and worker processes"
 authors = ["Michael R. van Rooijen <support@autoscale.app>"]
 license = "MIT"
 repository = "https://github.com/autoscale-app/python-agent"
 readme = "README.md"
 homepage = "https://autoscale.app"
 keywords = ["agent", "middleware", "autoscale", "render", "web", "worker", "queue", "job"]
```

### Comparing `autoscale_agent-0.2.0/PKG-INFO` & `autoscale_agent-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoscale-agent
-Version: 0.2.0
+Version: 0.2.1
 Summary: Provides Autoscale.app with the necessary metrics for autoscaling web and worker processes
 Home-page: https://autoscale.app
 License: MIT
 Keywords: agent,middleware,autoscale,render,web,worker,queue,job
 Author: Michael R. van Rooijen
 Author-email: support@autoscale.app
 Requires-Python: >=3.8,<3.12
```

