# Comparing `tmp/buildington-1.5.1.tar.gz` & `tmp/buildington-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.5.1.tar", last modified: Fri Apr 28 08:55:00 2023, max compression
+gzip compressed data, was "buildington-1.5.2.tar", last modified: Fri Apr 28 09:21:27 2023, max compression
```

## Comparing `buildington-1.5.1.tar` & `buildington-1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:55:00.295672 buildington-1.5.1/
--rw-rw-rw-   0        0        0     2259 2023-04-28 08:55:00.294674 buildington-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.5.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 08:55:00.251278 buildington-1.5.1/buildington/
--rw-rw-rw-   0        0        0     4372 2023-04-28 08:54:47.000000 buildington-1.5.1/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:55:00.290415 buildington-1.5.1/buildington.egg-info/
--rw-rw-rw-   0        0        0     2259 2023-04-28 08:54:59.000000 buildington-1.5.1/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-28 08:55:00.000000 buildington-1.5.1/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:54:59.000000 buildington-1.5.1/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 08:54:59.000000 buildington-1.5.1/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 08:54:59.000000 buildington-1.5.1/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 08:55:00.297677 buildington-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-04-28 08:54:53.000000 buildington-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.445551 buildington-1.5.2/
+-rw-rw-rw-   0        0        0     2259 2023-04-28 09:21:27.442552 buildington-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.5.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.396550 buildington-1.5.2/buildington/
+-rw-rw-rw-   0        0        0     4549 2023-04-28 09:19:41.000000 buildington-1.5.2/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.436549 buildington-1.5.2/buildington.egg-info/
+-rw-rw-rw-   0        0        0     2259 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:21:27.448547 buildington-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-04-28 09:20:12.000000 buildington-1.5.2/setup.py
```

### Comparing `buildington-1.5.1/PKG-INFO` & `buildington-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.5.1
+Version: 1.5.2
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.5.1/README.txt` & `buildington-1.5.2/README.txt`

 * *Files identical despite different names*

### Comparing `buildington-1.5.1/buildington/__init__.py` & `buildington-1.5.2/buildington/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,21 @@
 		import os
 		return flask.send_from_directory(os.getcwd(), file)
 	PAGES.append(("/" + file, returnResp, {"met": GETONLY}))
 	globals()["PAGES"] = tuple(PAGES)
 	del locals()["PAGES"]
 
 def start(host, port):
-	import flask, threading
-	app = flask.Flask(__name__) # The module name will fit :)
+	import flask, threading, inspect
+	targetGlob = inspect.currentframe().f_back.f_globals
+	for var in targetGlob.values():
+		if isinstance(var, flask.Flask):
+			app = var
+	if "app" not in locals():
+		app = flask.Flask(__name__) # The module name will fit :)
 	@app.route("/<path:path>", methods=["GET", "POST"])
 	@app.route("/", methods=["GET", "POST"])
 	def endpnt(path=None):
 		if path is None:
 			path = ""
 		path = "/" + path
 		foundEndpnt = False
```

### Comparing `buildington-1.5.1/buildington.egg-info/PKG-INFO` & `buildington-1.5.2/buildington.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.5.1
+Version: 1.5.2
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.5.1/setup.py` & `buildington-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.5.1",
+	version="1.5.2",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

