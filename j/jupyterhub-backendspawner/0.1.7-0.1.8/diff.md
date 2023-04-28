# Comparing `tmp/jupyterhub-backendspawner-0.1.7.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.7.tar", last modified: Wed Apr 26 14:43:35 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.8.tar", last modified: Fri Apr 28 09:54:39 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.7.tar` & `jupyterhub-backendspawner-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:43:35.880208 jupyterhub-backendspawner-0.1.7/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.7/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 14:43:35.880208 jupyterhub-backendspawner-0.1.7/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.7/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:43:35.880208 jupyterhub-backendspawner-0.1.7/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.7/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.1.7/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.1.7/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10170 2023-04-26 14:16:45.000000 jupyterhub-backendspawner-0.1.7/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 14:43:35.880208 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-26 14:43:35.000000 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-26 14:43:35.000000 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 14:43:35.000000 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-26 14:43:35.000000 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-26 14:43:35.000000 jupyterhub-backendspawner-0.1.7/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 14:43:35.880208 jupyterhub-backendspawner-0.1.7/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-26 14:43:30.000000 jupyterhub-backendspawner-0.1.7/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 09:54:38.963897 jupyterhub-backendspawner-0.1.8/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.8/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-28 09:54:38.953897 jupyterhub-backendspawner-0.1.8/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.8/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 09:54:38.933897 jupyterhub-backendspawner-0.1.8/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.8/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.1.8/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.1.8/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10207 2023-04-28 09:46:35.000000 jupyterhub-backendspawner-0.1.8/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 09:54:38.953897 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-28 09:54:38.000000 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-28 09:54:38.000000 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-28 09:54:38.000000 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-28 09:54:38.000000 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-28 09:54:38.000000 jupyterhub-backendspawner-0.1.8/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-28 09:54:38.963897 jupyterhub-backendspawner-0.1.8/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-28 09:53:46.000000 jupyterhub-backendspawner-0.1.8/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.7/LICENSE` & `jupyterhub-backendspawner-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.7/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.8/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.7/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.8/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.7/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.8/backendspawner/eventspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,23 +120,23 @@
         pattern = re.compile(
             r"([0-9]+(_[0-9]+)+).*[0-9]{2}:[0-9]{2}:[0-9]{2}(\\.[0-9]{1,3})?"
         )
         message = event["html_message"]
         match = re.search(pattern, message)
         return match.group()
 
-    @property
-    def ready_event(self):
-        event = super().ready_event
+    def get_ready_event(self):
+        event = super().get_ready_event()
         ready_msg = f"Service {self.name} started."
         now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
         url = url_path_join(self.user.url, self.name, "/")
         event[
             "html_message"
         ] = f'<details><summary>{now}: {ready_msg}</summary>You will be redirected to <a href="{url}">{url}</a></details>'
+        self.latest_events.append(event)
         return event
 
     cancelling_event = Union(
         [Dict(), Callable()],
         default_value={
             "failed": False,
             "ready": False,
```

### Comparing `jupyterhub-backendspawner-0.1.7/setup.py` & `jupyterhub-backendspawner-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.7",
+    version="0.1.8",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

