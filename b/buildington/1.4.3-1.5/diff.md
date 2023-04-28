# Comparing `tmp/buildington-1.4.3.tar.gz` & `tmp/buildington-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.4.3.tar", last modified: Sun Apr 23 10:52:06 2023, max compression
+gzip compressed data, was "buildington-1.5.tar", last modified: Fri Apr 28 08:50:17 2023, max compression
```

## Comparing `buildington-1.4.3.tar` & `buildington-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.473681 buildington-1.4.3/
--rw-rw-rw-   0        0        0     2259 2023-04-23 10:52:06.473681 buildington-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.4.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.426808 buildington-1.4.3/buildington/
--rw-rw-rw-   0        0        0     3594 2023-04-23 09:05:44.000000 buildington-1.4.3/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:52:06.473681 buildington-1.4.3/buildington.egg-info/
--rw-rw-rw-   0        0        0     2259 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 10:52:06.000000 buildington-1.4.3/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:52:06.473681 buildington-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-04-23 10:51:54.000000 buildington-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:50:17.167669 buildington-1.5/
+-rw-rw-rw-   0        0        0     2257 2023-04-28 08:50:17.165666 buildington-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 08:50:17.101965 buildington-1.5/buildington/
+-rw-rw-rw-   0        0        0     4343 2023-04-28 08:48:34.000000 buildington-1.5/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:50:17.161411 buildington-1.5/buildington.egg-info/
+-rw-rw-rw-   0        0        0     2257 2023-04-28 08:50:16.000000 buildington-1.5/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-28 08:50:16.000000 buildington-1.5/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:50:16.000000 buildington-1.5/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 08:50:16.000000 buildington-1.5/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 08:50:16.000000 buildington-1.5/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 08:50:17.167669 buildington-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-28 08:49:44.000000 buildington-1.5/setup.py
```

### Comparing `buildington-1.4.3/PKG-INFO` & `buildington-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.4.3
+Version: 1.5
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.4.3/README.txt` & `buildington-1.5/README.txt`

 * *Files identical despite different names*

### Comparing `buildington-1.4.3/buildington/__init__.py` & `buildington-1.5/buildington/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 GETMET = 0
 POSTMET = 1
 GETONLY = DEFAULT = [GETMET]
 POSTONLY = [POSTMET]
 ALLMETS = GETONLY + POSTONLY
 PAGES = tuple()
+FILES = tuple()
 
 class Para:
 	def __init__(self, innerHTML, props=None):
 		self.innerHTML = innerHTML
 		self.props = props
 		if not isinstance(self.props, dict):
 			self.props = {}
@@ -53,15 +54,20 @@
 			for elem in res:
 				if not isinstance(elem, Para):
 					raise ValueError("One of " + str(func).split(" ")[1] + "'s elements was not a valid " + __name__)
 			return res
 		return wrap
 	return decor
 
-def addFile(file):
+def addFile(file, asType="file"):
+	if asType not in ["file", "script", "style"]:
+		raise TypeError("Invalid file type '" + str(asType) + "'")
+	FILES = list(globals()["FILES"])
+	FILES.append((file, asType))
+	globals()["FILES"] = tuple(FILES)
 	PAGES = list(globals()["PAGES"])
 	def returnResp():
 		import flask
 		import os
 		return flask.send_from_directory(os.getcwd(), file)
 	PAGES.append(("/" + file, returnResp, {"met": GETONLY}))
 	globals()["PAGES"] = tuple(PAGES)
@@ -106,14 +112,29 @@
 		bdRes = list(bdRes)
 		for elem in bdRes:
 			if isinstance(elem, str):
 				elem = escapeHTML(elem)
 			elem = str(elem)
 			bdRes[count] = elem
 			count += 1
-		htmlRes = "<!-- Page generated by Buildington -->\n<!DOCTYPE html>\n<html lang=\"en\">\n\t<head>\n\t\t<meta charset=\"utf-8\">\n\t\t<meta name=\"viewport\" content=\"width=device-width\">\n\t\t<title>Buildington</title>\n\t</head>\n\t<body>\n\t"
+		scripts = [""]
+		styles = [""]
+		count = 0
+		while count != len(FILES):
+			if FILES[count][1] == "script":
+				scripts[-1] = "<script src=\"/" + FILES[count][0] + "\"></script>"
+				scripts.append("")
+			elif FILES[count][1] == "style":
+				styles[-1] = "<link href=\"/" + FILES[count][0] + "\" rel=\"stylesheet\">"
+				styles.append("")
+			count += 1
+		scripts = "\n\t\t".join(scripts)
+		styles = "\n\t\t".join(styles)
+		htmlRes = "<!-- Page generated by Buildington -->\n<!DOCTYPE html>\n<html lang=\"en\">\n\t<head>\n\t\t<meta charset=\"utf-8\">\n\t\t<meta name=\"viewport\" content=\"width=device-width\">\n\t\t" + styles + "<title>Buildington</title>\n\t</head>\n\t<body>\n\t"
 		for line in bdRes:
 			htmlRes += "\t" + line + "\n\t"
+		if scripts != "":
+			htmlRes += "\t" + scripts[:-1]
 		htmlRes += "</body>\n</html>"
 		htmlRes = htmlRes.replace("<body>\n\t</body>", "<body></body>")
 		return htmlRes
 	app.run(host, port)
```

### Comparing `buildington-1.4.3/buildington.egg-info/PKG-INFO` & `buildington-1.5/buildington.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.4.3
+Version: 1.5
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.4.3/setup.py` & `buildington-1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.4.3",
+	version="1.5",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

