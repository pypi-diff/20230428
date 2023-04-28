# Comparing `tmp/google-chad-3.2.tar.gz` & `tmp/google-chad-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-chad-3.2.tar", last modified: Sun Apr  9 22:32:40 2023, max compression
+gzip compressed data, was "google-chad-3.3.tar", last modified: Fri Apr 28 13:18:44 2023, max compression
```

## Comparing `google-chad-3.2.tar` & `google-chad-3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-04-06 18:22:56.000000 google-chad-3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-06 18:22:56.000000 google-chad-3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10408 2023-04-09 22:32:40.330834 google-chad-3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10002 2023-04-09 22:32:10.000000 google-chad-3.2/README.md
--rw-r--r--   0 root         (0) root         (0)      863 2023-04-08 21:46:58.000000 google-chad-3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 22:32:40.330834 google-chad-3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.326836 google-chad-3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.326836 google-chad-3.2/src/chad/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 18:22:56.000000 google-chad-3.2/src/chad/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19361 2023-04-09 21:26:00.000000 google-chad-3.2/src/chad/chad.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/chad_extractor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-06 18:22:56.000000 google-chad-3.2/src/chad_extractor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22500 2023-04-09 21:28:17.000000 google-chad-3.2/src/chad_extractor/chad_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/dorks/
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-06 18:22:56.000000 google-chad-3.2/src/dorks/social_media_dorks.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/google_chad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10408 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-09 22:32:40.000000 google-chad-3.2/src/google_chad.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 22:32:40.330834 google-chad-3.2/src/templates/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-04-09 22:32:15.000000 google-chad-3.2/src/templates/social_media_template.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:13:40.000000 google-chad-3.3/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      111 2023-04-28 13:13:40.000000 google-chad-3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-04-28 13:18:44.763366 google-chad-3.3/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    10307 2023-04-28 13:17:05.000000 google-chad-3.3/README.md
+-rwxrwx---   0 root         (0) root         (0)      893 2023-04-28 13:16:39.000000 google-chad-3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:18:44.763366 google-chad-3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/chad/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.3/src/chad/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    19973 2023-04-28 13:15:26.000000 google-chad-3.3/src/chad/chad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/chad_extractor/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 google-chad-3.3/src/chad_extractor/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    23152 2023-04-28 13:16:23.000000 google-chad-3.3/src/chad_extractor/chad_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/dorks/
+-rwxrwx---   0 root         (0) root         (0)      237 2023-04-28 13:13:40.000000 google-chad-3.3/src/dorks/social_media_dorks.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/google_chad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-28 13:18:44.000000 google-chad-3.3/src/google_chad.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:18:44.763366 google-chad-3.3/src/templates/
+-rwxrwx---   0 root         (0) root         (0)     1739 2023-04-28 13:13:40.000000 google-chad-3.3/src/templates/social_media_template.json
```

### Comparing `google-chad-3.2/PKG-INFO` & `google-chad-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-chad
-Version: 3.2
+Version: 3.3
 Summary: Not another Google Dorking tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/chad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
@@ -54,15 +54,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.3-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -203,15 +203,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.2 ( github.com/ivan-sincek/chad )
+Chad v3.3 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -270,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.2/README.md` & `google-chad-3.3/src/google_chad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: google-chad
+Version: 3.3
+Summary: Not another Google Dorking tool.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/chad
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Chad
 
 Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
 
 Tested on Kali Linux v2023.1 (64-bit).
 
 Made for educational purposes. I hope it will help!
@@ -41,15 +54,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/chad && cd chad
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
+python3 -m pip install dist/google_chad-3.3-py3-none-any.whl
 
 playwright install chromium
 ```
 
 ## Shortest Possible
 
 ```bash
@@ -190,15 +203,15 @@
 To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
 
 Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
 
 ## Usage
 
 ```fundamental
-Chad v3.2 ( github.com/ivan-sincek/chad )
+Chad v3.3 ( github.com/ivan-sincek/chad )
 
 Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
 Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
 
 DESCRIPTION
     Search Google Dorks like Chad
 QUERIES
@@ -257,15 +270,15 @@
     -sos <sleep-on-start> - no 
 DEBUG
     Debug output
     -dbg <debug> - yes
 ```
 
 ```fundamental
-Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
+Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
 
 Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
 Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
 
 DESCRIPTION
     Extract and validate data from Chad results or plaintext files
 TEMPLATE
```

### Comparing `google-chad-3.2/pyproject.toml` & `google-chad-3.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "google-chad"
-version = "3.2"
-authors = [{ name = "Ivan Sincek" }]
-description = "Not another Google Dorking tool."
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-	"Programming Language :: Python :: 3",
-	"License :: OSI Approved :: MIT License",
-	"Operating System :: POSIX :: Linux"
-]
-dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "nagooglesearch>=6.0", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
-
-[project.urls]
-"Homepage" = "https://github.com/ivan-sincek/chad"
-
-[project.scripts]
-chad = "chad.chad:main"
-chad-extractor = "chad_extractor.chad_extractor:main"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.package-data]
-"*" = ["dorks/*.txt", "templates/*.json"]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "google-chad"
+version = "3.3"
+authors = [{ name = "Ivan Sincek" }]
+description = "Not another Google Dorking tool."
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [
+	"Programming Language :: Python :: 3",
+	"License :: OSI Approved :: MIT License",
+	"Operating System :: POSIX :: Linux"
+]
+dependencies = ["datetime>=5.0", "termcolor>=1.1.0", "nagooglesearch>=6.0", "requests>=2.27.1", "jq>=1.2.1", "asyncio>=3.4.3", "playwright>=1.27.1", "regex>=2022.4.24"]
+
+[project.urls]
+"Homepage" = "https://github.com/ivan-sincek/chad"
+
+[project.scripts]
+chad = "chad.chad:main"
+chad-extractor = "chad_extractor.chad_extractor:main"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["dorks/*.txt", "templates/*.json"]
```

### Comparing `google-chad-3.2/src/chad/chad.py` & `google-chad-3.3/src/chad_extractor/chad_extractor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,572 +1,612 @@
-#!/usr/bin/env python3
-
-import datetime
-import dateutil.relativedelta as relativedelta
-import sys
-import os
-import termcolor
-import time
-import random
-from nagooglesearch import nagooglesearch
-import regex as re
-import concurrent.futures
-import subprocess
-import requests
-import urllib.parse
-import json
-
-start = datetime.datetime.now()
-
-requests.packages.urllib3.disable_warnings(requests.packages.urllib3.exceptions.InsecureRequestWarning)
-
-# -------------------------- INFO --------------------------
-
-def basic():
-	global proceed
-	proceed = False
-	print("Chad v3.2 ( github.com/ivan-sincek/chad )")
-	print("")
-	print("Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]")
-	print("Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]")
-
-def advanced():
-	basic()
-	print("")
-	print("DESCRIPTION")
-	print("    Search Google Dorks like Chad")
-	print("QUERIES")
-	print("    File with Google Dorks or a single query to use")
-	print("    -q <queries> - queries.txt | intext:password | \"ext:tar OR ext:zip\" | etc.")
-	print("SITE")
-	print("    Domain[s] to search")
-	print("    -s <site> - example.com | sub.example.com | *.example.com | \"*.example.com -www\" | etc.")
-	print("TIME")
-	print("    Get results not older than the specified time in months")
-	print("    -t <time> - 6 | 12 | 24 | etc.")
-	print("TOTAL RESULTS")
-	print("    Total number of unique results")
-	print("    Default: 100")
-	print("    -tr <total-results> - 200 | etc.")
-	print("PAGE RESULTS")
-	print("    Number of results per page - capped at 100 by Google")
-	print("    Default: randint(75, 100) per page")
-	print("    -pr <page-results> - 50 | etc.")
-	print("MINIMUM QUERIES")
-	print("    Minimum sleep between Google queries")
-	print("    Default: 75")
-	print("    -min-q <minimum-queries> - 120 | etc.")
-	print("MAXIMUM QUERIES")
-	print("    Maximum sleep between Google queries")
-	print("    Default: minimum + 50")
-	print("    -max-q <maximum-queries> - 180 | etc.")
-	print("MINIMUM PAGES")
-	print("    Minimum sleep between Google pages")
-	print("    Default: 15")
-	print("    -min-p <minimum-pages> - 30 | etc.")
-	print("MAXIMUM PAGES")
-	print("    Maximum sleep between Google pages")
-	print("    Default: minimum + 10")
-	print("    -max-p <maximum-pages> - 60 | etc.")
-	print("AGENTS")
-	print("    File with user agents to use")
-	print("    Default: nagooglesearch user agents")
-	print("    -a <agents> - user_agents.txt | etc.")
-	print("PROXIES")
-	print("    File with proxies to use")
-	print("    -p <proxies> - proxies.txt | etc.")
-	print("DIRECTORY")
-	print("    Downloads directory")
-	print("    All downloaded files will be saved in this directory")
-	print("    -d <directory> - downloads | etc.")
-	print("THREADS")
-	print("    Number of parallel files to download")
-	print("    Default: 5")
-	print("    -th <threads> - 20 | etc.")
-	print("OUT")
-	print("    Output file")
-	print("    -o <out> - results.json | etc.")
-	print("SLEEP ON START")
-	print("    Safety feature to prevent accidental rate limit triggering")
-	print("    -sos <sleep-on-start> - no ")
-	print("DEBUG")
-	print("    Debug output")
-	print("    -dbg <debug> - yes")
-
-# ------------------- MISCELENIOUS BEGIN -------------------
-
-def unique(sequence):
-	seen = set()
-	return [x for x in sequence if not (x in seen or seen.add(x))]
-
-def read_file(file):
-	tmp = []
-	with open(file, "r", encoding = "ISO-8859-1") as stream:
-		for line in stream:
-			line = line.strip()
-			if line:
-				tmp.append(line)
-	stream.close()
-	return unique(tmp)
-
-def jdump(data):
-	return json.dumps(data, indent = 4, ensure_ascii = False)
-
-def write_file(data, out):
-	confirm = "yes"
-	if os.path.isfile(out):
-		print(("'{0}' already exists").format(out))
-		confirm = input("Overwrite the output file (yes): ")
-	if confirm.lower() == "yes":
-		open(out, "w").write(data)
-		print(("Results have been saved to '{0}'").format(out))
-
-def write_file_silent(data, out):
-	open(out, "wb").write(data)
-
-# -------------------- MISCELENIOUS END --------------------
-
-# -------------------- VALIDATION BEGIN --------------------
-
-# my own validation algorithm
-
-proceed = True
-
-def print_error(msg):
-	print(("ERROR: {0}").format(msg))
-
-def error(msg, help = False):
-	global proceed
-	proceed = False
-	print_error(msg)
-	if help:
-		print("Use -h for basic and --help for advanced info")
-
-args = {"queries": None, "site": None, "time": None, "total": None, "page": None, "min-q": None, "max-q": None, "min-p": None, "max-p": None, "sleep": None, "proxies": None, "agents": None, "out": None, "threads": None, "directory": None, "debug": None}
-
-# TO DO: Better site validation.
-def validate(key, value):
-	global args
-	value = value.strip()
-	if len(value) > 0:
-		if key == "-q" and args["queries"] is None:
-			args["queries"] = value
-			if os.path.isdir(args["queries"]):
-				error("File with Google Dorks is a directory")
-			elif os.path.isfile(args["queries"]):
-				if not os.access(args["queries"], os.R_OK):
-					error("File with Google Dorks does not have read permission")
-				elif not os.stat(args["queries"]).st_size > 0:
-					error("File with Google Dorks is empty")
-				else:
-					args["queries"] = read_file(args["queries"])
-					if not args["queries"]:
-						error("No Google Dorks were found")
-			else:
-				args["queries"] = [args["queries"]]
-		elif key == "-s" and args["site"] is None:
-			args["site"] = value
-		elif key == "-t" and args["time"] is None:
-			args["time"] = value
-			if not args["time"].isdigit():
-				error("Number of months must be numeric")
-			else:
-				args["time"] = int(args["time"])
-				if args["time"] < 1:
-					error("Number of months must be greater than zero")
-		elif key == "-tr" and args["total"] is None:
-			args["total"] = value
-			if not args["total"].isdigit():
-				error("Total number of unique results must be numeric")
-			else:
-				args["total"] = int(args["total"])
-				if args["total"] < 1:
-					error("Total number of unique results must be greater than zero")
-		elif key == "-pr" and args["page"] is None:
-			args["page"] = value
-			if not args["page"].isdigit():
-				error("Number of results per page must be numeric")
-			else:
-				args["page"] = int(args["page"])
-				if args["page"] < 1 or args["page"] > 1000:
-					error("Number of results per page must be between 1 and 1000")
-		elif key == "-min-q" and args["min-q"] is None:
-			args["min-q"] = value
-			if not args["min-q"].isdigit():
-				error("Minimum sleep between Google queries must be numeric")
-			else:
-				args["min-q"] = int(args["min-q"])
-				if args["min-q"] < 1:
-					error("Minimum sleep between Google queries must be greater than zero")
-		elif key == "-max-q" and args["max-q"] is None:
-			args["max-q"] = value
-			if not args["max-q"].isdigit():
-				error("Maximum sleep between Google queries must be numeric")
-			else:
-				args["max-q"] = int(args["max-q"])
-				if args["max-q"] < 1:
-					error("Maximum sleep between Google queries must be greater than zero")
-		elif key == "-min-p" and args["min-p"] is None:
-			args["min-p"] = value
-			if not args["min-p"].isdigit():
-				error("Minimum sleep between Google pages must be numeric")
-			else:
-				args["min-p"] = int(args["min-p"])
-				if args["min-p"] < 1:
-					error("Minimum sleep between Google pages must be greater than zero")
-		elif key == "-max-p" and args["max-p"] is None:
-			args["max-p"] = value
-			if not args["max-p"].isdigit():
-				error("Maximum sleep between Google pages must be numeric")
-			else:
-				args["max-p"] = int(args["max-p"])
-				if args["max-p"] < 1:
-					error("Maximum sleep between Google pages must be greater than zero")
-		elif key == "-a" and args["agents"] is None:
-			args["agents"] = value
-			if not os.path.isfile(args["agents"]):
-				error("File with user agents does not exists")
-			elif not os.access(args["agents"], os.R_OK):
-				error("File with user agents does not have read permission")
-			elif not os.stat(args["agents"]).st_size > 0:
-				error("File with user agents is empty")
-			else:
-				args["agents"] = read_file(args["agents"])
-				if not args["agents"]:
-					error("No user agents were found")
-		elif key == "-p" and args["proxies"] is None:
-			args["proxies"] = value
-			if not os.path.isfile(args["proxies"]):
-				error("File with proxies does not exists")
-			elif not os.access(args["proxies"], os.R_OK):
-				error("File with proxies does not have read permission")
-			elif not os.stat(args["proxies"]).st_size > 0:
-				error("File with proxies is empty")
-			else:
-				args["proxies"] = read_file(args["proxies"])
-				if not args["proxies"]:
-					error("No proxies were found")
-		elif key == "-d" and args["directory"] is None:
-			args["directory"] = os.path.abspath(value)
-			if not os.path.exists(args["directory"]):
-				error("Downloads directory does not exists")
-		elif key == "-th" and args["threads"] is None:
-			args["threads"] = value
-			if not args["threads"].isdigit():
-				error("Number of parallel files to download must be numeric")
-			else:
-				args["threads"] = int(args["threads"])
-				if args["threads"] < 1:
-					error("Number of parallel files to download must be greater than zero")
-		elif key == "-o" and args["out"] is None:
-			args["out"] = value
-		elif key == "-sos" and args["sleep"] is None:
-			args["sleep"] = value.lower()
-			if args["sleep"] != "no":
-				error("Specify 'no' to disable sleep on start")
-		elif key == "-dbg" and args["debug"] is None:
-			args["debug"] = value.lower()
-			if args["debug"] != "yes":
-				error("Specify 'yes' to enable debug output")
-
-def check(argc, args):
-	count = 0
-	for key in args:
-		if args[key] is not None:
-			count += 1
-	return argc - count == argc / 2
-
-# --------------------- VALIDATION END ---------------------
-
-# ----------------------- TASK BEGIN -----------------------
-
-def get_timestamp(text):
-	return print(("{0} - {1}").format(datetime.datetime.now().strftime("%H:%M:%S"), text))
-
-def status(current, total, query, proxy = None, color = "green"):
-	text = ("QUERY {0}/{1}: {2}").format(current, total, termcolor.colored(query, color))
-	if proxy:
-		text = ("{0} | PROXY: {1}").format(text, proxy)
-	get_timestamp(text)
-
-def print_ignored(ignored, color = "cyan"):
-	print(("{0} QUERIES IGNORED:").format(len(ignored)))
-	for query in ignored:
-		print(termcolor.colored(query, color))
-
-def get_site(query):
-	return re.search(r"(?<!in|\-)site\:", query, re.IGNORECASE)
-
-def validate_queries(queries, site = None):
-	tmp = []
-	ignored = []
-	const = " "
-	for query in queries:
-		if site:
-			if get_site(query):
-				ignored.append(query)
-				continue
-			query = ("site:{0}{1}({2})").format(site, const, query)
-		if len(query.split(const)) > 32:
-			ignored.append(query)
-			continue
-		tmp.append(query)
-	if ignored:
-		print_ignored(ignored)
-	return unique(tmp)
-
-def wait(minimum, maximum):
-	sec = random.randint(minimum, maximum)
-	print(("Sleeping between requests for {0} seconds...").format(sec))
-	time.sleep(sec)
-
-index = 0
-round_robin = False
-
-def get_proxy(proxies):
-	global index, round_robin
-	proxy = proxies[index]
-	index += 1
-	if index >= len(proxies):
-		index = 0
-		round_robin = True
-	return proxy
-
-def remove_proxy(proxies, proxy, color = "red"):
-	global index
-	proxies.pop(proxies.index(proxy))
-	index -= 1
-	if index < 0:
-		index = 0
-	print(("Proxy '{0}' has been removed due to an error or rate limiting | Proxies left: {1}").format(proxy, len(proxies)))
-	return proxies
-
-def check_blacklist(urls):
-	# exclude security related websites that contain Google Dorks to minimize false positive results
-	blacklist = ["kb.cert.org", "exploit-db.com"]
-	for entry in ["dork", "hack"]:
-		for delimiter in ["", "+", "-", "_", "%20"]:
-			blacklist.append("google" + delimiter + entry)
-	blacklist = ("(?:{0})").format(("|").join([entry.replace(".", "\\.").replace("/", "\\/") for entry in blacklist]))
-	tmp = []
-	for url in urls:
-		if not re.search(blacklist, url, re.IGNORECASE):
-			tmp.append(url)
-	return tmp
-
-def get_tbs(months = None):
-	tmp = "li:1"
-	if months:
-		today = datetime.datetime.today()
-		tmp = nagooglesearch.get_tbs(today, today - relativedelta.relativedelta(months = months))
-	return tmp
-
-def run(queries, tbs = "li:1", total = 100, page = None, min_q = 75, max_q = 125, min_p = 15, max_p = 25, agents = None, proxies = None, sleep = False, debug = False):
-	global round_robin
-	get_timestamp("Searching Google Dorks...")
-	print("Press CTRL + C to exit early - all results will be saved")
-	results = []
-	try:
-		if not sleep:
-			wait(min_q, max_q)
-		count = 0
-		length = len(queries)
-		exit = False
-		for query in queries:
-			count += 1
-			entry = {"query": query, "proxy": None, "urls": None}
-			parameters = {
-				"q": entry["query"],
-				"tbs": tbs,
-				"num": str(page if page else random.randint(75, 100)),
-				"hl": "en",
-				"filter": "0",
-				"safe": "images"
-			}
-			while not exit:
-				if proxies:
-					if round_robin:
-						wait(min_q, max_q)
-						round_robin = False
-					entry["proxy"] = get_proxy(proxies)
-				elif count > 1:
-					wait(min_q, max_q)
-				status(count, length, entry["query"], entry["proxy"])
-				remove = False
-				try:
-					client = nagooglesearch.SearchClient(
-						tld = "com",
-						parameters = parameters,
-						max_results = total,
-						user_agent = agents[random.randint(0, len(agents) - 1)] if agents else nagooglesearch.get_random_user_agent(),
-						proxy = entry["proxy"],
-						min_sleep = min_p,
-						max_sleep = max_p,
-						verbose = debug
-					)
-					entry["urls"] = client.search()
-					if "429_TOO_MANY_REQUESTS" in entry["urls"]:
-						print(termcolor.colored("[ HTTP 429 Too Many Requests ]", "yellow"))
-						entry["urls"].pop(entry["urls"].index("429_TOO_MANY_REQUESTS"))
-						if entry["proxy"]:
-							remove = True
-						else:
-							exit = True
-					if entry["urls"]:
-						if not get_site(entry["query"]):
-							entry["urls"] = check_blacklist(entry["urls"])
-						results.append(entry)
-					if not remove and not exit:
-						break
-				except Exception as ex:
-					if debug:
-						print_error(ex)
-					if entry["proxy"]:
-						remove = True
-					else:
-						exit = True
-				if remove:
-					proxies = remove_proxy(proxies, entry["proxy"])
-					if not proxies:
-						print_error("All proxies has been exhausted!")
-						exit = True
-			if exit:
-				break
-	except KeyboardInterrupt:
-		pass
-	return results
-
-def get_filename(directory, url):
-	url = urllib.parse.urlparse(url)
-	base = os.path.join(directory, url.netloc)
-	if url.path:
-		base = os.path.join(directory, url.path.strip("/").rsplit("/", 1)[-1])
-	count = 0
-	filename = base
-	while os.path.exists(filename):
-		count += 1
-		filename = ("{0} ({1})").format(base, count)
-	return filename
-
-def download(url, headers = None, debug = None):
-	tmp = {"url": url, "data": None}
-	session = requests.Session()
-	session.max_redirects = 10
-	response = None
-	try:
-		response = session.get(url, headers = headers, proxies = None, timeout = 90, verify = False, allow_redirects = True)
-		if response.status_code == 200:
-			tmp["data"] = response.content
-	except (requests.packages.urllib3.exceptions.LocationParseError, requests.exceptions.RequestException) as ex:
-		if debug:
-			print_error(ex)
-	finally:
-		if response is not None:
-			response.close()
-		session.close()
-	return tmp
-
-def get_headers(agents = None):
-	return {
-		"Accept": "*/*",
-		"Accept-Language": "*",
-		"Connection": "keep-alive",
-		"Referer": "https://www.google.com/",
-		# "Upgrade-Insecure-Requests": "1", # because of this request header, some websites might return wrong page content
-		"User-Agent": agents[random.randint(0, len(agents) - 1)] if agents else nagooglesearch.get_random_user_agent()
-	}
-
-def get_urls(results):
-	tmp = []
-	for result in results:
-		tmp.extend(result["urls"])
-	tmp = unique(tmp)
-	random.shuffle(tmp)
-	return tmp
-
-def progress(count, total):
-	print(("Progress: {0}/{1} | {2:.2f}%").format(count, total, (count / total) * 100), end = "\n" if count == total else "\r")
-
-def download_files(results, directory, threads = 5, agents = None, debug = None):
-	get_timestamp("Downloading files... Proxies will be ignored...")
-	results = get_urls(results)
-	count = 0
-	total = len(results)
-	progress(count, total)
-	with concurrent.futures.ThreadPoolExecutor(max_workers = threads) as executor:
-		subprocesses = []
-		for url in results:
-			subprocesses.append(executor.submit(download, url, get_headers(agents), debug))
-		for subprocess in concurrent.futures.as_completed(subprocesses):
-			result = subprocess.result()
-			if result["data"]:
-				write_file_silent(result["data"], get_filename(directory, result["url"]))
-			count += 1
-			progress(count, total)
-
-def main():
-	argc = len(sys.argv) - 1
-
-	if argc == 0:
-		advanced()
-	elif argc == 1:
-		if sys.argv[1] == "-h":
-			basic()
-		elif sys.argv[1] == "--help":
-			advanced()
-		else:
-			error("Incorrect usage", True)
-	elif argc % 2 == 0 and argc <= len(args) * 2:
-		for i in range(1, argc, 2):
-			validate(sys.argv[i], sys.argv[i + 1])
-		if args["queries"] is None or not check(argc, args):
-			error("Missing a mandatory option (-q) and/or optional (-s, -t, -tr, -pr, -min-q, -max-q, -min-p, -max-p, -a, -p, -th, -d, -o, -sos, -dbg)", True)
-	else:
-		error("Incorrect usage", True)
-
-	if proceed:
-		print("#######################################################################")
-		print("#                                                                     #")
-		print("#                              Chad v3.2                              #")
-		print("#                                   by Ivan Sincek                    #")
-		print("#                                                                     #")
-		print("# Search Google Dorks like Chad.                                      #")
-		print("# GitHub repository at github.com/ivan-sincek/chad.                   #")
-		print("# Feel free to donate bitcoin at 1BrZM6T7G9RN8vbabnfXu4M6Lpgztq6Y14.  #")
-		print("#                                                                     #")
-		print("#######################################################################")
-		# --------------------
-		if not args["total"]:
-			args["total"] = 100
-		if not args["min-q"]:
-			args["min-q"] = 75
-		if not args["max-q"] or args["min-q"] > args["max-q"]:
-			args["max-q"] = args["min-q"] + 50
-		if not args["min-p"]:
-			args["min-p"] = 15
-		if not args["max-p"] or args["min-p"] > args["max-p"]:
-			args["max-p"] = args["min-p"] + 10
-		if not args["threads"]:
-			args["threads"] = 5
-		# --------------------
-		get_timestamp("Validating Google Dorks...")
-		print("Google only allows queries up to 32 words in length separated by space")
-		args["queries"] = validate_queries(args["queries"], args["site"])
-		if not args["queries"]:
-			print("No valid queries are left")
-		else:
-			results = run(args["queries"], get_tbs(args["time"]), args["total"], args["page"], args["min-q"], args["max-q"], args["min-p"], args["max-p"], args["agents"], args["proxies"], args["sleep"], args["debug"])
-			if not results:
-				print("No results")
-			else:
-				if args["directory"]:
-					download_files(results, args["directory"], args["threads"], args["agents"], args["debug"])
-				results = jdump(results)
-				print(results)
-				if args["out"]:
-					write_file(results, args["out"])
-		print(("Script has finished in {0}").format(datetime.datetime.now() - start))
-
-if __name__ == "__main__":
-	main()
-
-# ------------------------ TASK END ------------------------
+#!/usr/bin/env python3
+
+import datetime
+import sys
+import os
+import json
+import jq
+import threading
+import random
+import concurrent.futures
+import subprocess
+import asyncio
+from playwright.async_api import async_playwright, TimeoutError as PlaywrightTimeoutError
+from nagooglesearch import nagooglesearch
+import time
+import regex as re
+
+start = datetime.datetime.now()
+
+# -------------------------- INFO --------------------------
+
+def basic():
+	global proceed
+	proceed = False
+	print("Chad Extractor v3.3 ( github.com/ivan-sincek/chad )")
+	print("")
+	print("Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]")
+	print("Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]")
+
+def advanced():
+	basic()
+	print("")
+	print("DESCRIPTION")
+	print("    Extract and validate data from Chad results or plaintext files")
+	print("TEMPLATE")
+	print("    JSON template file with extraction and validation information")
+	print("    -t <template> - template.json | etc.")
+	print("RESULTS DIRECTORY/FILE")
+	print("    Directory containing Chad results or plaintext files, or a single file")
+	print("    -res <results> - results | results.json | urls.txt | etc.")
+	print("PLAINTEXT")
+	print("    Parse files as plaintext")
+	print("    -pt <plaintext> - yes")
+	print("EXCLUDES")
+	print("    File with regular expressions or a single expression to exclude the page content")
+	print("    -e <excludes> - regexes.txt | \"<div id=\\\"seo\\\">.+?<\\/div>\" | etc.")
+	print("THREADS")
+	print("    Number of parallel headless browsers to run")
+	print("    Default: 4")
+	print("    -th <threads> - 10 | etc.")
+	print("RETRIES")
+	print("    Number of retries per URL")
+	print("    Default: 2")
+	print("    -r <retries> - 5 | etc.")
+	print("WAIT")
+	print("    Wait before fetching the page content")
+	print("    Default: 4")
+	print("    -w <wait> - 10 | etc.")
+	print("AGENTS")
+	print("    File with user agents to use")
+	print("    Default: nagooglesearch user agents")
+	print("    -a <agents> - user_agents.txt | etc.")
+	print("OUT")
+	print("    Output file")
+	print("    -o <out> - results_report.json | etc.")
+	print("VERBOSE")
+	print("    Create additional supporting output files")
+	print("    -v <verbose> - yes")
+
+
+# ------------------- MISCELENIOUS BEGIN -------------------
+
+def check_directory_files(directory):
+	tmp = []
+	for file in os.listdir(directory):
+		file = os.path.join(directory, file)
+		if os.path.isfile(file) and os.access(file, os.R_OK) and os.stat(file).st_size > 0:
+			tmp.append(file)
+	return tmp
+
+def unique(sequence, sort = False):
+	seen = set()
+	array = [x for x in sequence if not (x in seen or seen.add(x))]
+	if sort and array:
+		array = sorted(array, key = str.casefold)
+	return array
+
+def read_file(file, sort = False, text = False):
+	flags = "r"
+	encoding = "UTF-8"
+	if text:
+		return open(file, flags, encoding = encoding).read()
+	else:
+		tmp = []
+		with open(file, flags, encoding = encoding) as stream:
+			for line in stream:
+				line = line.strip()
+				if line:
+					tmp.append(line)
+		stream.close()
+		return unique(tmp, sort)
+
+def read_json(file):
+	tmp = []
+	try:
+		tmp = json.loads(open(file, "r", encoding = "UTF-8").read())
+	except json.decoder.JSONDecodeError:
+		pass
+	return tmp
+
+def jquery(obj, query):
+	tmp = []
+	try:
+		tmp = jq.compile(query).input(obj).all()
+	except ValueError:
+		pass
+	return tmp
+
+def jdump(data):
+	return json.dumps(data, indent = 4, ensure_ascii = False)
+
+def write_file(data, out):
+	confirm = "yes"
+	if os.path.isfile(out):
+		print(("'{0}' already exists").format(out))
+		confirm = input("Overwrite the output file (yes): ")
+	if confirm.lower() == "yes":
+		open(out, "w").write(data)
+		print(("Results have been saved to '{0}'").format(out))
+
+def write_file_silent(data, out):
+	open(out, "w").write(data)
+
+# -------------------- MISCELENIOUS END --------------------
+
+# -------------------- VALIDATION BEGIN --------------------
+
+# my own validation algorithm
+
+proceed = True
+
+def print_error(msg):
+	print(("ERROR: {0}").format(msg))
+
+def error(msg, help = False):
+	global proceed
+	proceed = False
+	print_error(msg)
+	if help:
+		print("Use -h for basic and --help for advanced info")
+
+args = {"template": None, "results": None, "plaintext": None, "excludes": None, "threads": None, "retries": None, "wait": None, "agents": None, "out": None, "verbose": None}
+
+def validate(key, value):
+	global args
+	value = value.strip()
+	if len(value) > 0:
+		if key == "-t" and args["template"] is None:
+			args["template"] = value
+			if not os.path.isfile(args["template"]):
+				error("Template file does not exists")
+			elif not os.access(args["template"], os.R_OK):
+				error("Template file does not have read permission")
+			elif not os.stat(args["template"]).st_size > 0:
+				error("Template file is empty")
+			else:
+				args["template"] = read_json(args["template"])
+				if not args["template"]:
+					error("Template file has invalid JSON format")
+		elif key == "-res" and args["results"] is None:
+			args["results"] = value
+			if not os.path.exists(args["results"]):
+				error("Directory containing Chad results or plaintext files, or a single file does not exists")
+			elif os.path.isdir(args["results"]):
+				args["results"] = [file for file in check_directory_files(args["results"]) if not file.endswith(ext)]
+				if not args["results"]:
+					error("No valid Chad results or plaintext files were found")
+			else:
+				if not os.access(args["results"], os.R_OK):
+					error("Chad results or plaintext file does not have read permission")
+				elif not os.stat(args["results"]).st_size > 0:
+					error("Chad results or plaintext file is empty")
+				else:
+					args["results"] = [args["results"]]
+		elif key == "-pt" and args["plaintext"] is None:
+			args["plaintext"] = value.lower()
+			if args["plaintext"] != "yes":
+				error("Specify 'yes' to parse files as plaintext")
+		elif key == "-e" and args["excludes"] is None:
+			args["excludes"] = value
+			if os.path.isdir(args["excludes"]):
+				error("File with regular expressions is a directory")
+			elif os.path.isfile(args["excludes"]):
+				if not os.access(args["excludes"], os.R_OK):
+					error("File with regular expressions does not have read permission")
+				elif not os.stat(args["excludes"]).st_size > 0:
+					error("File with regular expressions is empty")
+				else:
+					args["excludes"] = read_file(args["excludes"])
+					if not args["excludes"]:
+						error("No regular expressions were found")
+			else:
+				args["excludes"] = [args["excludes"]]
+		elif key == "-th" and args["threads"] is None:
+			args["threads"] = value
+			if not args["threads"].isdigit():
+				error("Number of parallel headless browsers must be numeric")
+			else:
+				args["threads"] = int(args["threads"])
+				if args["threads"] < 1:
+					error("Number of parallel headless browsers must be greater than zero")
+		elif key == "-r" and args["retries"] is None:
+			args["retries"] = value
+			if not args["retries"].isdigit():
+				error("Number of retries per URL must be numeric")
+			else:
+				args["retries"] = int(args["retries"])
+				if args["retries"] < 0:
+					error("Number of retries per URL must be greater than or equal to zero")
+		elif key == "-w" and args["wait"] is None:
+			args["wait"] = value
+			if not args["wait"].isdigit():
+				error("Wait before fetching the page content must be numeric")
+			else:
+				args["wait"] = int(args["wait"])
+				if args["wait"] < 0:
+					error("Wait before fetching the page content must be greater than or equal to zero")
+		elif key == "-a" and args["agents"] is None:
+			args["agents"] = value
+			if not os.path.isfile(args["agents"]):
+				error("File with user agents does not exists")
+			elif not os.access(args["agents"], os.R_OK):
+				error("File with user agents does not have read permission")
+			elif not os.stat(args["agents"]).st_size > 0:
+				error("File with user agents is empty")
+			else:
+				args["agents"] = read_file(args["agents"])
+				if not args["agents"]:
+					error("No user agents were found")
+		elif key == "-o" and args["out"] is None:
+			args["out"] = value
+		elif key == "-v" and args["verbose"] is None:
+			args["verbose"] = value.lower()
+			if args["verbose"] != "yes":
+				error("Specify 'yes' to enable verbosity")
+
+def check(argc, args):
+	count = 0
+	for key in args:
+		if args[key] is not None:
+			count += 1
+	return argc - count == argc / 2
+
+# --------------------- VALIDATION END ---------------------
+
+# ----------------- GLOBAL VARIABLES BEGIN -----------------
+
+def get_data():
+	return {
+		"data": [],
+		"lock": threading.Lock()
+	}
+
+data = {
+	"extracted": get_data(),
+	"failed_extraction": get_data(),
+	"validated": get_data(),
+	"failed_validation": get_data()
+}
+
+def extend_data(key, array):
+	global data
+	with data[key]["lock"]:
+		data[key]["data"].extend(array)
+
+queries = {
+	"get_url": ".[].url",
+	"get_urls": ".[].urls[]",
+	"sort_by_url": "sort_by(.url | ascii_downcase)[]",
+	"group_by_url": "group_by(.url) | map((.[0] | del(.file)) + {files: (map(.file) | unique)})[]",
+	"get_file": ".[].file",
+	"get_files": ".[].files[]",
+	"sort_by_file": "sort_by(.file | ascii_downcase)[]",
+	"delete_files": ".[] | del(.files)",
+	"get_results": ".[].results[][]"
+}
+
+ext = ".report.json"
+
+# ------------------ GLOBAL VARIABLES END ------------------
+
+# ----------------------- TASK BEGIN -----------------------
+
+def get_timestamp(text):
+	return print(("{0} - {1}").format(datetime.datetime.now().strftime("%H:%M:%S"), text))
+
+def split(records, threads = 4):
+	if threads > 1:
+		k, m = divmod(len(records), threads)
+		return (records[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(threads))
+	else:
+		return [records]
+
+def parse_response(skey, template, record, response):
+	tmp = {}
+	if skey == "extracted":
+		for key in template:
+			try:
+				matches = re.findall(template[key]["extract"], response, re.MULTILINE | re.IGNORECASE)
+				if matches:
+					if "extract_prepend" in template[key] or "extract_append" in template[key]:
+						prepend = ""
+						if "extract_prepend" in template[key]:
+							prepend = template[key]["extract_prepend"]
+						append = ""
+						if "extract_append" in template[key]:
+							append = template[key]["extract_append"]
+						tmp[key] = []
+						for match in matches:
+							tmp[key].append(prepend + match + append)
+					else:
+						tmp[key] = matches
+					tmp[key] = unique(tmp[key], True)
+			except Exception as ex:
+				print_error(("{0} | {1}").format(key, ex))
+	elif skey == "validated" and re.search(template[record["id"]]["validate"], response, re.MULTILINE | re.IGNORECASE):
+		tmp = True
+	return tmp
+
+async def block(route):
+	await route.abort() if route.request.resource_type in ["stylesheet", "image", "media", "font", "ping"] else await route.continue_()
+
+async def page_get(context, url, excludes = [], wait = 4):
+	tmp = {"response": None, "error": False}
+	page = None
+	try:
+		page = await context.new_page()
+		await page.route("**/*", block) # ignore unnecessary requests
+		await page.goto(url, wait_until = "load")
+		if wait:
+			time.sleep(wait)
+		try:
+			await page.wait_for_load_state(state = "networkidle") # wait until network is idle for 500ms within 30s
+		except PlaywrightTimeoutError: # in case of a live stream, suppress and continue
+			pass
+		tmp["response"] = await page.content()
+		if excludes:
+			for exclude in excludes:
+				tmp["response"] = re.sub(exclude, "", tmp["response"], re.MULTILINE | re.IGNORECASE)
+	except PlaywrightTimeoutError:
+		pass
+	except Exception: # in case of a file or invalid domain, fallback
+		tmp["error"] = True
+	finally:
+		if page:
+			await page.close()
+	return tmp
+
+async def request_get(context, url, excludes = []):
+	tmp = {"response": None, "error": False}
+	try:
+		response = await context.request.get(url)
+		response = await response.body()
+		tmp["response"] = response.decode("ISO-8859-1")
+		if excludes:
+			for exclude in excludes:
+				tmp["response"] = re.sub(exclude, "", tmp["response"], re.MULTILINE | re.IGNORECASE)
+	except PlaywrightTimeoutError:
+		pass
+	except Exception: # in case of an invalid domain, break
+		tmp["error"] = True
+	return tmp
+
+def get_headers(agents = None):
+	return {
+		"Accept": "*/*",
+		"Accept-Language": "*",
+		"Connection": "keep-alive",
+		"Referer": "https://www.google.com/",
+		# "Upgrade-Insecure-Requests": "1", # because of this request header, some websites might return a wrong page content
+		"User-Agent": agents[random.randint(0, len(agents) - 1)] if agents else nagooglesearch.get_random_user_agent()
+	}
+
+async def browser_requests(skey, fkey, template, records, excludes = [], retries = 2, wait = 4, agents = None):
+	succeeded = []
+	failed = []
+	async with async_playwright() as pw:
+		browser = await pw.chromium.launch(headless = True)
+		context = await browser.new_context(ignore_https_errors = True, java_script_enabled = True, accept_downloads = False)
+		# context.set_default_timeout(60000)
+		for record in records:
+			entry = {"files": record["files"], "url": record["url"], "results": {}}
+			count = retries + 1
+			while count > 0:
+				await context.set_extra_http_headers(get_headers(agents)) # anti-bot evasion 2
+				# --------------------
+				tmp = await page_get(context, record["url"], excludes, wait)
+				if tmp["error"]:
+					tmp = await request_get(context, record["url"], excludes)
+					if tmp["error"]:
+						count = 0
+				# --------------------
+				if not tmp["error"] and tmp["response"]:
+					count = 0
+					entry["results"] = parse_response(skey, template, record, tmp["response"])
+					if entry["results"]:
+						succeeded.append(entry)
+				else:
+					count -= 1
+					if count <= 0:
+						failed.append(entry)
+				# --------------------
+				await context.clear_cookies() # anti-bot evasion 3
+		await context.close()
+		await browser.close()
+	extend_data(skey, succeeded)
+	extend_data(fkey, failed)
+
+def proxy_browser_requests(template, records, excludes = [], retries = 2, wait = 4, agents = None, extract = True):
+	skey = "extracted"
+	fkey = "failed_extraction"
+	if not extract:
+		skey = "validated"
+		fkey = "failed_validation"
+	asyncio.run(browser_requests(skey, fkey, template, records, excludes, retries, wait, agents))
+
+def parse_template(template, extract = True):
+	tmp = {}
+	if extract:
+		for key in template:
+			if "extract" in template[key]:
+				tmp[key] = template[key]
+	else:
+		for key in template:
+			if "validate" in template[key]:
+				tmp[key] = template[key]
+	return tmp
+
+def parse_input(template, results, extract = True, plaintext = False):
+	global data
+	tmp = []
+	if extract:
+		for file in results:
+			for url in jquery(read_json(file), queries["get_urls"]):
+				tmp.append({"file": file, "url": url})
+	elif plaintext:
+		for file in results:
+			result = parse_response("extracted", template, None, read_file(file, False, True)) # passing a file content instead of a web content
+			data["extracted"]["data"].append({"file": file, "results": result})
+			for key in result:
+				if key in template:
+					for url in result[key]:
+						tmp.append({"file": file, "url": url, "id": key})
+	else:
+		for result in results:
+			for key in result["results"]:
+				if key in template:
+					for url in result["results"][key]:
+						for file in result["files"]:
+							tmp.append({"file": file, "url": url, "id": key})
+	return jquery(tmp, queries["group_by_url"])
+
+def run(template, results, excludes = [], threads = 4, retries = 2, wait = 4, agents = None, extract = True):
+	get_timestamp(("Number of URLs to be {0}: {1}").format("extracted" if extract else "validated", len(results)))
+	random.shuffle(results) # anti-bot evasion 1
+	with concurrent.futures.ThreadPoolExecutor(max_workers = threads) as executor:
+		subprocesses = []
+		for records in split(results, threads):
+			if wait:
+				time.sleep(wait)
+			subprocesses.append(executor.submit(proxy_browser_requests, template, records, excludes, retries, wait, agents, extract))
+		concurrent.futures.wait(subprocesses)
+
+def get_report(plaintext = False):
+	if plaintext:
+		return {"summary": {"validated": [], "extracted": []}, "failed": {"validation": []}, "results": []}
+	else:
+		return {"summary": {"validated": [], "extracted": []}, "failed": {"validation": [], "extraction": []}, "full": []}
+
+def parse_results(out, verbose = False, plaintext = False):
+	global data
+	# --------------------
+	tmp = get_report(plaintext)
+	# --------------------
+	data["extracted"]["data"] = jquery(data["extracted"]["data"], queries["sort_by_file" if plaintext else "sort_by_url"])
+	tmp["full"] = data["extracted"]["data"] if plaintext else jquery(data["extracted"]["data"], queries["delete_files"])
+	tmp["summary"]["extracted"] = unique(jquery(tmp["full"], queries["get_results"]), True)
+	# --------------------
+	if not plaintext:
+		data["failed_extraction"]["data"] = jquery(data["failed_extraction"]["data"], queries["sort_by_url"])
+		tmp["failed"]["extraction"] = jquery(data["failed_extraction"]["data"], queries["get_url"])
+	# --------------------
+	data["validated"]["data"] = jquery(data["validated"]["data"], queries["sort_by_url"])
+	tmp["summary"]["validated"] = jquery(data["validated"]["data"], queries["get_url"])
+	# --------------------
+	data["failed_validation"]["data"] = jquery(data["failed_validation"]["data"], queries["sort_by_url"])
+	tmp["failed"]["validation"] = jquery(data["failed_validation"]["data"], queries["get_url"])
+	# --------------------
+	write_file(jdump(tmp), out)
+	# --------------------
+	if verbose:
+		for file in unique(jquery(data["extracted"]["data"], queries["get_file" if plaintext else "get_files"])):
+			# --------------------
+			tmp = get_report(plaintext)
+			# --------------------
+			if not plaintext:
+				tmp["full"] = jquery(data["extracted"]["data"], (".[] | select(.files | index(\"{0}\")) | del(.files)").format(file))
+				tmp["summary"]["extracted"] = unique(jquery(tmp["full"], queries["get_results"]), True)
+			else:
+				obj = jquery(data["extracted"]["data"], (".[] | select(.file == \"{0}\") | del(.file)").format(file))
+				tmp["summary"]["extracted"] = unique(jquery(obj, queries["get_results"]), True)
+				tmp["results"] = obj[0]["results"]
+			# --------------------
+			query = (".[] | select(.files | index(\"{0}\")) | .url").format(file)
+			# --------------------
+			if not plaintext:
+				tmp["failed"]["extraction"] = jquery(data["failed_extraction"]["data"], query)
+			# --------------------
+			tmp["summary"]["validated"] = jquery(data["validated"]["data"], query)
+			# --------------------
+			tmp["failed"]["validation"] = jquery(data["failed_validation"]["data"], query)
+			# --------------------
+			write_file_silent(jdump(tmp), file.rsplit(".", 1)[0] + ext)
+			# --------------------
+
+def main():
+	argc = len(sys.argv) - 1
+
+	if argc == 0:
+		advanced()
+	elif argc == 1:
+		if sys.argv[1] == "-h":
+			basic()
+		elif sys.argv[1] == "--help":
+			advanced()
+		else:
+			error("Incorrect usage", True)
+	elif argc % 2 == 0 and argc <= len(args) * 2:
+		for i in range(1, argc, 2):
+			validate(sys.argv[i], sys.argv[i + 1])
+		if args["template"] is None or args["results"] is None or args["out"] is None or not check(argc, args):
+			error("Missing a mandatory option (-t, -res, -o) and/or optional (-pt, -e, -th, -r, -w, -a, -v)", True)
+	else:
+		error("Incorrect usage", True)
+
+	if proceed:
+		print("###########################################################################")
+		print("#                                                                         #")
+		print("#                           Chad Extractor v3.3                           #")
+		print("#                                   by Ivan Sincek                        #")
+		print("#                                                                         #")
+		print("# Extract and validate data from Chad results.                            #")
+		print("# GitHub repository at github.com/ivan-sincek/chad.                       #")
+		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105.  #")
+		print("#                                                                         #")
+		print("###########################################################################")
+		# --------------------
+		if not args["threads"]:
+			args["threads"] = 4
+		if not args["retries"]:
+			args["retries"] = 2
+		if not args["wait"]:
+			args["wait"] = 4
+		# --------------------
+		if args["plaintext"]:
+			args["template"] = parse_template(args["template"], True)
+			if not args["template"]:
+				print("No extraction entries were found in the template file")
+			else:
+				args["results"] = parse_input(args["template"], args["results"], False, True)
+				if not data["extracted"]["data"]:
+					print("No data was extracted")
+				else:
+					args["template"] = parse_template(args["template"], False)
+					if not args["template"]:
+						print("No validation entries were found in the template file")
+					else:
+						run(args["template"], args["results"], args["excludes"], args["threads"], args["retries"], args["wait"], args["agents"], False)
+						if not data["validated"]["data"]:
+							print("No data matched the validation criteria")
+					parse_results(args["out"], args["verbose"], True)
+		else:
+			args["template"] = parse_template(args["template"], True)
+			if not args["template"]:
+				print("No extraction entries were found in the template file")
+			else:
+				args["results"] = parse_input(args["template"], args["results"], True)
+				if not args["results"]:
+					print("No results for data extraction were found")
+				else:
+					run(args["template"], args["results"], args["excludes"], args["threads"], args["retries"], args["wait"], args["agents"], True)
+					if not data["extracted"]["data"]:
+						print("No data was extracted")
+					else:
+						args["template"] = parse_template(args["template"], False)
+						if not args["template"]:
+							print("No validation entries were found in the template file")
+						else:
+							args["results"] = parse_input(args["template"], data["extracted"]["data"], False)
+							if not args["results"]:
+								print("No results for data validation were found")
+							else:
+								run(args["template"], args["results"], args["excludes"], args["threads"], args["retries"], args["wait"], args["agents"], False)
+								if not data["validated"]["data"]:
+									print("No data matched the validation criteria")
+						parse_results(args["out"], args["verbose"])
+		print(("Script has finished in {0}").format(datetime.datetime.now() - start))
+
+if __name__ == "__main__":
+	main()
+
+# ------------------------ TASK END ------------------------
```

### Comparing `google-chad-3.2/src/google_chad.egg-info/PKG-INFO` & `google-chad-3.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,318 +1,305 @@
-Metadata-Version: 2.1
-Name: google-chad
-Version: 3.2
-Summary: Not another Google Dorking tool.
-Author: Ivan Sincek
-Project-URL: Homepage, https://github.com/ivan-sincek/chad
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Chad
-
-Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
-
-Tested on Kali Linux v2023.1 (64-bit).
-
-Made for educational purposes. I hope it will help!
-
-Future plans:
-
-* remove `jq` from Chad Extractor so it can be OS independent.
-
-## Table of Contents
-
-* [How to Install](#how-to-install)
-* [How to Build and Install Manually](#how-to-build-and-install-manually)
-* [Shortest Possible](#shortest-possible)
-* [Basic Example: File Download](#basic-example-file-download)
-* [Chad Extractor](#chad-extractor)
-    * [Extracting and Validating Data)](#extracting-and-validating-data)
-* [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
-    * [Basic Use (Single Domain)](#basic-use-single-domain)
-    * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
-* [Rate Limiting](#rate-limiting)
-* [Usage](#usage)
-
-## How to Install
-
-```bash
-pip3 install google-chad
-
-pip3 install --upgrade google-chad
-
-playwright install chromium
-```
-
-## How to Build and Install Manually
-
-Run the following commands:
-
-```bash
-git clone https://github.com/ivan-sincek/chad && cd chad
-
-python3 -m pip install --upgrade build
-
-python3 -m build
-
-python3 -m pip install dist/google_chad-3.2-py3-none-any.whl
-
-playwright install chromium
-```
-
-## Shortest Possible
-
-```bash
-chad -q 'intitle:"index of /" intext:"parent directory"'
-```
-
-## Basic Example: File Download
-
-Did you say Metagoofil?!
-
-```bash
-mkdir downloads
-
-chad -q "ext:pdf OR ext:docx OR ext:xlsx OR ext:pptx" -s *.example.com -tr 200 -d downloads -sos no
-```
-
-`-s <site>` is optional. For more information, see [Usage](#usage).
-
-Chad's file download feature is based on Python Requests library.
-
-## Chad Extractor
-
-Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
-
-### Extracting and Validating Data
-
-Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag.
-
-## Advanced Example: Social Media Takover
-
-Prepare Google Dorks as `social_media_dorks.txt` file:
-
-```fundamental
-intext:"t.me/"
-intext:"discord.com/invite/"
-intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
-intext:"twitter.com/"
-intext:"instagram.com/"
-intext:"facebook.com/"
-intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
-```
-
-Prepare a template as `social_media_template.json` file:
-
-```json
-{
-   "telegram":{
-      "extract":"t\\.me\\/[\\w\\d\\-\\+]+",
-      "extract_prepend":"https://",
-      "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
-   },
-   "discord":{
-      "extract":"discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"Invite Invalid"
-   },
-   "youtube":{
-      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available\\."
-   },
-   "twitter":{
-      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
-      "extract_prepend":"https://",
-      "validate":"This account doesn.?t exist"
-   },
-   "instagram":{
-      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "extract_append":"/",
-      "validate":"Sorry, this page isn't available\\."
-   },
-   "facebook":{
-      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
-      "extract_prepend":"https://",
-      "validate":"This page isn't available"
-   },
-   "linkedin-company":{
-      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://hr.",
-      "validate":"Page not found"
-   },
-   "linkedin-user":{
-      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
-      "extract_prepend":"https://hr.",
-      "validate":"An exact match for .+ could not be found\\."
-   }
-}
-```
-
-**Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
-
-Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
-
-All regular expression searches are case-insensitive.
-
-Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
-
-To extract data without validating it, omit `validate` attributes from the template file as necessary.
-
-### Basic Use (Single Domain)
-
-```bash
-chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json -sos no
-
-chad-extractor -t social_media_template.json -res results.json -o results_report.json
-```
-
-### Advanced Use (Multiple Domains)
-
-Prepare sites/domains as `sites.txt` file:
-
-```fundamental
-*.example.com
-*.example.com -www
-```
-
-Prepare bot-safe User-Agents as `user_agents.txt` file, where `<your-api-key>` is your API key from [scrapeops.io](https://scrapeops.io):
-
-```python
-python3 -c 'import json, requests; open("user_agents.txt", "w").write(("\n").join(requests.get("http://headers.scrapeops.io/v1/user-agents?api_key=<your-api-key>&num_results=100", verify = False).json()["result"]))'
-```
-
-Automate:
-
-```bash
-mkdir results
-
-IFS=$'\n'; count=0; for site in $(cat sites.txt); do count=$((count+1)); echo "#${count} | ${site}"; chad -q social_media_dorks.txt -s "${site}" -tr 200 -a user_agents.txt -o "results/results_${count}.json"; done
-
-chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
-```
-
-## Rate Limiting
-
-Google's cooling-off period can be from a few hours to a whole day.
-
-To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
-
-Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
-
-## Usage
-
-```fundamental
-Chad v3.2 ( github.com/ivan-sincek/chad )
-
-Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
-Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
-
-DESCRIPTION
-    Search Google Dorks like Chad
-QUERIES
-    File with Google Dorks or a single query to use
-    -q <queries> - queries.txt | intext:password | "ext:tar OR ext:zip" | etc.
-SITE
-    Domain[s] to search
-    -s <site> - example.com | sub.example.com | *.example.com | "*.example.com -www" | etc.
-TIME
-    Get results not older than the specified time in months
-    -t <time> - 6 | 12 | 24 | etc.
-TOTAL RESULTS
-    Total number of unique results
-    Default: 100
-    -tr <total-results> - 200 | etc.
-PAGE RESULTS
-    Number of results per page - capped at 100 by Google
-    Default: randint(75, 100) per page
-    -pr <page-results> - 50 | etc.
-MINIMUM QUERIES
-    Minimum sleep between Google queries
-    Default: 75
-    -min-q <minimum-queries> - 120 | etc.
-MAXIMUM QUERIES
-    Maximum sleep between Google queries
-    Default: minimum + 50
-    -max-q <maximum-queries> - 180 | etc.
-MINIMUM PAGES
-    Minimum sleep between Google pages
-    Default: 15
-    -min-p <minimum-pages> - 30 | etc.
-MAXIMUM PAGES
-    Maximum sleep between Google pages
-    Default: minimum + 10
-    -max-p <maximum-pages> - 60 | etc.
-AGENTS
-    File with user agents to use
-    Default: nagooglesearch user agents
-    -a <agents> - user_agents.txt | etc.
-PROXIES
-    File with proxies to use
-    -p <proxies> - proxies.txt | etc.
-DIRECTORY
-    Downloads directory
-    All downloaded files will be saved in this directory
-    -d <directory> - downloads | etc.
-THREADS
-    Number of parallel files to download
-    Default: 5
-    -th <threads> - 20 | etc.
-OUT
-    Output file
-    -o <out> - results.json | etc.
-SLEEP ON START
-    Safety feature to prevent accidental rate limit triggering
-    -sos <sleep-on-start> - no 
-DEBUG
-    Debug output
-    -dbg <debug> - yes
-```
-
-```fundamental
-Chad Extractor v3.2 ( github.com/ivan-sincek/chad )
-
-Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
-Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
-
-DESCRIPTION
-    Extract and validate data from Chad results or plaintext files
-TEMPLATE
-    JSON template file with extraction and validation information
-    -t <template> - template.json | etc.
-RESULTS DIRECTORY/FILE
-    Directory containing Chad results or plaintext files, or a single file
-    -res <results> - results | results.json | urls.txt | etc.
-PLAINTEXT
-    Parse files as plaintext
-    -pt <plaintext> - yes
-EXCLUDES
-    File with regular expressions or a single expression to exclude the page content
-    -e <excludes> - regexes.txt | "<div id=\"seo\">.+?<\/div>" | etc.
-THREADS
-    Number of parallel headless browsers to run
-    Default: 4
-    -th <threads> - 10 | etc.
-RETRIES
-    Number of retries per URL
-    Default: 2
-    -r <retries> - 5 | etc.
-WAIT
-    Wait before fetching the page content
-    Default: 4
-    -w <wait> - 10 | etc.
-AGENTS
-    File with user agents to use
-    Default: nagooglesearch user agents
-    -a <agents> - user_agents.txt | etc.
-OUT
-    Output file
-    -o <out> - results_report.json | etc.
-VERBOSE
-    Create additional supporting output files
-    -v <verbose> - yes
-```
+# Chad
+
+Search Google Dorks like Chad. Based on [ivan-sincek/nagooglesearch](https://github.com/ivan-sincek/nagooglesearch).
+
+Tested on Kali Linux v2023.1 (64-bit).
+
+Made for educational purposes. I hope it will help!
+
+Future plans:
+
+* remove `jq` from Chad Extractor so it can be OS independent.
+
+## Table of Contents
+
+* [How to Install](#how-to-install)
+* [How to Build and Install Manually](#how-to-build-and-install-manually)
+* [Shortest Possible](#shortest-possible)
+* [Basic Example: File Download](#basic-example-file-download)
+* [Chad Extractor](#chad-extractor)
+    * [Extracting and Validating Data)](#extracting-and-validating-data)
+* [Advanced Example: Social Media Takover](#advanced-example-social-media-takover)
+    * [Basic Use (Single Domain)](#basic-use-single-domain)
+    * [Advanced Use (Multiple Domains)](#advanced-use-multiple-domains)
+* [Rate Limiting](#rate-limiting)
+* [Usage](#usage)
+
+## How to Install
+
+```bash
+pip3 install google-chad
+
+pip3 install --upgrade google-chad
+
+playwright install chromium
+```
+
+## How to Build and Install Manually
+
+Run the following commands:
+
+```bash
+git clone https://github.com/ivan-sincek/chad && cd chad
+
+python3 -m pip install --upgrade build
+
+python3 -m build
+
+python3 -m pip install dist/google_chad-3.3-py3-none-any.whl
+
+playwright install chromium
+```
+
+## Shortest Possible
+
+```bash
+chad -q 'intitle:"index of /" intext:"parent directory"'
+```
+
+## Basic Example: File Download
+
+Did you say Metagoofil?!
+
+```bash
+mkdir downloads
+
+chad -q "ext:pdf OR ext:docx OR ext:xlsx OR ext:pptx" -s *.example.com -tr 200 -d downloads -sos no
+```
+
+`-s <site>` is optional. For more information, see [Usage](#usage).
+
+Chad's file download feature is based on Python Requests library.
+
+## Chad Extractor
+
+Chad Extractor is a powerful tool based on [Playwright](https://playwright.dev/python) Chromium headless browser created to efficiently scrape web; in other words, to compensate for Python Requests library which cannot render JavaScript encoded HTML and is easily blocked by anti-bot solutions.
+
+### Extracting and Validating Data
+
+Chad Extractor was mainly designed to extract and validate data from Chad results files; but, you can also use it to extract and validate data from plaintext files by specifying `-pt yes` flag.
+
+## Advanced Example: Social Media Takover
+
+Prepare Google Dorks as `social_media_dorks.txt` file:
+
+```fundamental
+intext:"t.me/"
+intext:"discord.com/invite/"
+intext:"youtube.com/c/" OR intext:"youtube.com/channel/"
+intext:"twitter.com/"
+intext:"instagram.com/"
+intext:"facebook.com/"
+intext:"linkedin.com/in/" OR intext:"linkedin.com/company/"
+```
+
+Prepare a template as `social_media_template.json` file:
+
+```json
+{
+   "telegram":{
+      "extract":"t\\.me\\/[\\w\\d\\-\\+]+",
+      "extract_prepend":"https://",
+      "validate":"<meta property=\"og:title\" content=\"Telegram: Contact .+?\">"
+   },
+   "discord":{
+      "extract":"discord\\.com\\/invite\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"Invite Invalid"
+   },
+   "youtube":{
+      "extract":"youtube\\.com\\/(?:c|channel)\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available\\."
+   },
+   "twitter":{
+      "extract":"(?<!pic\\.)twitter\\.com\\/(?:(?!(?:hashtag|home|i|intent|share|search|explore)(?:\\/|\\?)[^\\s]+|[\\w]+\\/(?:privacy|tos)|personalization|widgets\\.js)[\\w\\d\\-\\+]+)",
+      "extract_prepend":"https://",
+      "validate":"This account doesn.?t exist"
+   },
+   "instagram":{
+      "extract":"instagram\\.com\\/(?:(?!(?:p|accounts)(?:\\/|\\?)[^\\s]+)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "extract_append":"/",
+      "validate":"Sorry, this page isn't available\\."
+   },
+   "facebook":{
+      "extract":"facebook\\.com\\/(?:(?!(?:about|dialog|gaming|groups|sharer)(?:\\/|\\?)[^\\s]+|share\\.php|terms\\.php)[\\w\\d\\-\\+\\.]+)(?<!\\.)",
+      "extract_prepend":"https://",
+      "validate":"This page isn't available"
+   },
+   "linkedin-company":{
+      "extract":"linkedin\\.com\\/company\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract_prepend":"https://hr.",
+      "validate":"Page not found"
+   },
+   "linkedin-user":{
+      "extract":"linkedin\\.com\\/in\\/[\\w\\d\\-\\+\\.]+(?<!\\.)",
+      "extract_prepend":"https://hr.",
+      "validate":"An exact match for .+ could not be found\\."
+   }
+}
+```
+
+**Make sure your regular expressions return only one capturing group e.g. `[1, 2, 3, 4]`; and not a touple e.g. `[(1, 2), (3, 4)]`.**
+
+Make sure to properly escape regular expression specific symbols in your template file, e.g. make sure to escape dot `.` as `\\.`, and forward slash `/` as `\\/`, etc.
+
+All regular expression searches are case-insensitive.
+
+Web content fetched from the URLs in Chad results will be matched against all the regular expressions (`extract` attributes) in the template file in order to find as much relevant data as possible.
+
+To extract data without validating it, omit `validate` attributes from the template file as necessary.
+
+### Basic Use (Single Domain)
+
+```bash
+chad -q social_media_dorks.txt -s *.example.com -tr 200 -o results.json -sos no
+
+chad-extractor -t social_media_template.json -res results.json -o results_report.json
+```
+
+### Advanced Use (Multiple Domains)
+
+Prepare sites/domains as `sites.txt` file:
+
+```fundamental
+*.example.com
+*.example.com -www
+```
+
+Prepare bot-safe User-Agents as `user_agents.txt` file, where `<your-api-key>` is your API key from [scrapeops.io](https://scrapeops.io):
+
+```python
+python3 -c 'import json, requests; open("user_agents.txt", "w").write(("\n").join(requests.get("http://headers.scrapeops.io/v1/user-agents?api_key=<your-api-key>&num_results=100", verify = False).json()["result"]))'
+```
+
+Automate:
+
+```bash
+mkdir results
+
+IFS=$'\n'; count=0; for site in $(cat sites.txt); do count=$((count+1)); echo "#${count} | ${site}"; chad -q social_media_dorks.txt -s "${site}" -tr 200 -a user_agents.txt -o "results/results_${count}.json"; done
+
+chad-extractor -t social_media_template.json -res results -a user_agents.txt -o results_report.json -v yes
+```
+
+## Rate Limiting
+
+Google's cooling-off period can be from a few hours to a whole day.
+
+To avoid hitting Google's rate limit with Chad, increase the minimum and maximum sleep between Google queries.
+
+Additionally, to avoid hitting e.g. Instagrams's rate limit with Chad Extractor, you might want to isolate it in a separate run, increase the wait time, and use only one thread.
+
+## Usage
+
+```fundamental
+Chad v3.3 ( github.com/ivan-sincek/chad )
+
+Usage:   chad -q queries     [-s site         ] [-a agents         ] [-p proxies    ] [-o out         ]
+Example: chad -q queries.txt [-s *.example.com] [-a user_agents.txt] [-p proxies.txt] [-o results.json]
+
+DESCRIPTION
+    Search Google Dorks like Chad
+QUERIES
+    File with Google Dorks or a single query to use
+    -q <queries> - queries.txt | intext:password | "ext:tar OR ext:zip" | etc.
+SITE
+    Domain[s] to search
+    -s <site> - example.com | sub.example.com | *.example.com | "*.example.com -www" | etc.
+TIME
+    Get results not older than the specified time in months
+    -t <time> - 6 | 12 | 24 | etc.
+TOTAL RESULTS
+    Total number of unique results
+    Default: 100
+    -tr <total-results> - 200 | etc.
+PAGE RESULTS
+    Number of results per page - capped at 100 by Google
+    Default: randint(75, 100) per page
+    -pr <page-results> - 50 | etc.
+MINIMUM QUERIES
+    Minimum sleep between Google queries
+    Default: 75
+    -min-q <minimum-queries> - 120 | etc.
+MAXIMUM QUERIES
+    Maximum sleep between Google queries
+    Default: minimum + 50
+    -max-q <maximum-queries> - 180 | etc.
+MINIMUM PAGES
+    Minimum sleep between Google pages
+    Default: 15
+    -min-p <minimum-pages> - 30 | etc.
+MAXIMUM PAGES
+    Maximum sleep between Google pages
+    Default: minimum + 10
+    -max-p <maximum-pages> - 60 | etc.
+AGENTS
+    File with user agents to use
+    Default: nagooglesearch user agents
+    -a <agents> - user_agents.txt | etc.
+PROXIES
+    File with proxies to use
+    -p <proxies> - proxies.txt | etc.
+DIRECTORY
+    Downloads directory
+    All downloaded files will be saved in this directory
+    -d <directory> - downloads | etc.
+THREADS
+    Number of parallel files to download
+    Default: 5
+    -th <threads> - 20 | etc.
+OUT
+    Output file
+    -o <out> - results.json | etc.
+SLEEP ON START
+    Safety feature to prevent accidental rate limit triggering
+    -sos <sleep-on-start> - no 
+DEBUG
+    Debug output
+    -dbg <debug> - yes
+```
+
+```fundamental
+Chad Extractor v3.3 ( github.com/ivan-sincek/chad )
+
+Usage:   chad-extractor -t template      -res results -o out                 [-th threads] [-r retries] [-w wait] [-a agents         ]
+Example: chad-extractor -t template.json -res results -o results_report.json [-th 10     ] [-r 5      ] [-w 10  ] [-a user_agents.txt]
+
+DESCRIPTION
+    Extract and validate data from Chad results or plaintext files
+TEMPLATE
+    JSON template file with extraction and validation information
+    -t <template> - template.json | etc.
+RESULTS DIRECTORY/FILE
+    Directory containing Chad results or plaintext files, or a single file
+    -res <results> - results | results.json | urls.txt | etc.
+PLAINTEXT
+    Parse files as plaintext
+    -pt <plaintext> - yes
+EXCLUDES
+    File with regular expressions or a single expression to exclude the page content
+    -e <excludes> - regexes.txt | "<div id=\"seo\">.+?<\/div>" | etc.
+THREADS
+    Number of parallel headless browsers to run
+    Default: 4
+    -th <threads> - 10 | etc.
+RETRIES
+    Number of retries per URL
+    Default: 2
+    -r <retries> - 5 | etc.
+WAIT
+    Wait before fetching the page content
+    Default: 4
+    -w <wait> - 10 | etc.
+AGENTS
+    File with user agents to use
+    Default: nagooglesearch user agents
+    -a <agents> - user_agents.txt | etc.
+OUT
+    Output file
+    -o <out> - results_report.json | etc.
+VERBOSE
+    Create additional supporting output files
+    -v <verbose> - yes
+```
```

### Comparing `google-chad-3.2/src/templates/social_media_template.json` & `google-chad-3.3/src/templates/social_media_template.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,109 @@
-00000000: 7b0a 2020 2022 7465 6c65 6772 616d 223a  {.   "telegram":
-00000010: 7b0a 2020 2020 2020 2265 7874 7261 6374  {.      "extract
-00000020: 223a 2274 5c5c 2e6d 655c 5c2f 5b5c 5c77  ":"t\\.me\\/[\\w
-00000030: 5c5c 645c 5c2d 5c5c 2b5d 2b22 2c0a 2020  \\d\\-\\+]+",.  
-00000040: 2020 2020 2265 7874 7261 6374 5f70 7265      "extract_pre
-00000050: 7065 6e64 223a 2268 7474 7073 3a2f 2f22  pend":"https://"
-00000060: 2c0a 2020 2020 2020 2276 616c 6964 6174  ,.      "validat
-00000070: 6522 3a22 3c6d 6574 6120 7072 6f70 6572  e":"<meta proper
-00000080: 7479 3d5c 226f 673a 7469 746c 655c 2220  ty=\"og:title\" 
-00000090: 636f 6e74 656e 743d 5c22 5465 6c65 6772  content=\"Telegr
-000000a0: 616d 3a20 436f 6e74 6163 7420 2e2b 3f5c  am: Contact .+?\
-000000b0: 223e 220a 2020 207d 2c0a 2020 2022 6469  ">".   },.   "di
-000000c0: 7363 6f72 6422 3a7b 0a20 2020 2020 2022  scord":{.      "
-000000d0: 6578 7472 6163 7422 3a22 6469 7363 6f72  extract":"discor
-000000e0: 645c 5c2e 636f 6d5c 5c2f 696e 7669 7465  d\\.com\\/invite
-000000f0: 5c5c 2f5b 5c5c 775c 5c64 5c5c 2d5c 5c2b  \\/[\\w\\d\\-\\+
-00000100: 5c5c 2e5d 2b28 3f3c 215c 5c2e 2922 2c0a  \\.]+(?<!\\.)",.
-00000110: 2020 2020 2020 2265 7874 7261 6374 5f70        "extract_p
-00000120: 7265 7065 6e64 223a 2268 7474 7073 3a2f  repend":"https:/
-00000130: 2f22 2c0a 2020 2020 2020 2276 616c 6964  /",.      "valid
-00000140: 6174 6522 3a22 496e 7669 7465 2049 6e76  ate":"Invite Inv
-00000150: 616c 6964 220a 2020 207d 2c0a 2020 2022  alid".   },.   "
-00000160: 796f 7574 7562 6522 3a7b 0a20 2020 2020  youtube":{.     
-00000170: 2022 6578 7472 6163 7422 3a22 796f 7574   "extract":"yout
-00000180: 7562 655c 5c2e 636f 6d5c 5c2f 283f 3a63  ube\\.com\\/(?:c
-00000190: 7c63 6861 6e6e 656c 295c 5c2f 5b5c 5c77  |channel)\\/[\\w
-000001a0: 5c5c 645c 5c2d 5c5c 2b5c 5c2e 5d2b 283f  \\d\\-\\+\\.]+(?
-000001b0: 3c21 5c5c 2e29 222c 0a20 2020 2020 2022  <!\\.)",.      "
-000001c0: 6578 7472 6163 745f 7072 6570 656e 6422  extract_prepend"
-000001d0: 3a22 6874 7470 733a 2f2f 222c 0a20 2020  :"https://",.   
-000001e0: 2020 2022 7661 6c69 6461 7465 223a 2254     "validate":"T
-000001f0: 6869 7320 7061 6765 2069 736e 2774 2061  his page isn't a
-00000200: 7661 696c 6162 6c65 5c5c 2e22 0a20 2020  vailable\\.".   
-00000210: 7d2c 0a20 2020 2274 7769 7474 6572 223a  },.   "twitter":
-00000220: 7b0a 2020 2020 2020 2265 7874 7261 6374  {.      "extract
-00000230: 223a 2228 3f3c 2170 6963 5c5c 2e29 7477  ":"(?<!pic\\.)tw
-00000240: 6974 7465 725c 5c2e 636f 6d5c 5c2f 283f  itter\\.com\\/(?
-00000250: 3a28 3f21 283f 3a68 6173 6874 6167 7c68  :(?!(?:hashtag|h
-00000260: 6f6d 657c 697c 696e 7465 6e74 7c73 6861  ome|i|intent|sha
-00000270: 7265 7c73 6561 7263 687c 6578 706c 6f72  re|search|explor
-00000280: 6529 283f 3a5c 5c2f 7c5c 5c3f 295b 5e5c  e)(?:\\/|\\?)[^\
-00000290: 5c73 5d2b 7c5b 5c5c 775d 2b5c 5c2f 283f  \s]+|[\\w]+\\/(?
-000002a0: 3a70 7269 7661 6379 7c74 6f73 297c 7065  :privacy|tos)|pe
-000002b0: 7273 6f6e 616c 697a 6174 696f 6e7c 7769  rsonalization|wi
-000002c0: 6467 6574 735c 5c2e 6a73 295b 5c5c 775c  dgets\\.js)[\\w\
-000002d0: 5c64 5c5c 2d5c 5c2b 5d2b 2922 2c0a 2020  \d\\-\\+]+)",.  
-000002e0: 2020 2020 2265 7874 7261 6374 5f70 7265      "extract_pre
-000002f0: 7065 6e64 223a 2268 7474 7073 3a2f 2f22  pend":"https://"
-00000300: 2c0a 2020 2020 2020 2276 616c 6964 6174  ,.      "validat
-00000310: 6522 3a22 5468 6973 2061 6363 6f75 6e74  e":"This account
-00000320: 2064 6f65 736e 2e3f 7420 6578 6973 7422   doesn.?t exist"
-00000330: 0a20 2020 7d2c 0a20 2020 2269 6e73 7461  .   },.   "insta
-00000340: 6772 616d 223a 7b0a 2020 2020 2020 2265  gram":{.      "e
-00000350: 7874 7261 6374 223a 2269 6e73 7461 6772  xtract":"instagr
-00000360: 616d 5c5c 2e63 6f6d 5c5c 2f28 3f3a 283f  am\\.com\\/(?:(?
-00000370: 2128 3f3a 707c 6163 636f 756e 7473 2928  !(?:p|accounts)(
-00000380: 3f3a 5c5c 2f7c 5c5c 3f29 5b5e 5c5c 735d  ?:\\/|\\?)[^\\s]
-00000390: 2b29 5b5c 5c77 5c5c 645c 5c2d 5c5c 2b5c  +)[\\w\\d\\-\\+\
-000003a0: 5c2e 5d2b 2928 3f3c 215c 5c2e 2922 2c0a  \.]+)(?<!\\.)",.
-000003b0: 2020 2020 2020 2265 7874 7261 6374 5f70        "extract_p
-000003c0: 7265 7065 6e64 223a 2268 7474 7073 3a2f  repend":"https:/
-000003d0: 2f22 2c0a 2020 2020 2020 2265 7874 7261  /",.      "extra
-000003e0: 6374 5f61 7070 656e 6422 3a22 2f22 2c0a  ct_append":"/",.
-000003f0: 2020 2020 2020 2276 616c 6964 6174 6522        "validate"
-00000400: 3a22 536f 7272 792c 2074 6869 7320 7061  :"Sorry, this pa
-00000410: 6765 2069 736e 2774 2061 7661 696c 6162  ge isn't availab
-00000420: 6c65 5c5c 2e22 0a20 2020 7d2c 0a20 2020  le\\.".   },.   
-00000430: 2266 6163 6562 6f6f 6b22 3a7b 0a20 2020  "facebook":{.   
-00000440: 2020 2022 6578 7472 6163 7422 3a22 6661     "extract":"fa
-00000450: 6365 626f 6f6b 5c5c 2e63 6f6d 5c5c 2f28  cebook\\.com\\/(
-00000460: 3f3a 283f 2128 3f3a 6162 6f75 747c 6469  ?:(?!(?:about|di
-00000470: 616c 6f67 7c67 616d 696e 677c 6772 6f75  alog|gaming|grou
-00000480: 7073 7c73 6861 7265 7229 283f 3a5c 5c2f  ps|sharer)(?:\\/
-00000490: 7c5c 5c3f 295b 5e5c 5c73 5d2b 7c73 6861  |\\?)[^\\s]+|sha
-000004a0: 7265 5c5c 2e70 6870 7c74 6572 6d73 5c5c  re\\.php|terms\\
-000004b0: 2e70 6870 295b 5c5c 775c 5c64 5c5c 2d5c  .php)[\\w\\d\\-\
-000004c0: 5c2b 5c5c 2e5d 2b29 283f 3c21 5c5c 2e29  \+\\.]+)(?<!\\.)
-000004d0: 222c 0a20 2020 2020 2022 6578 7472 6163  ",.      "extrac
-000004e0: 745f 7072 6570 656e 6422 3a22 6874 7470  t_prepend":"http
-000004f0: 733a 2f2f 222c 0a20 2020 2020 2022 7661  s://",.      "va
-00000500: 6c69 6461 7465 223a 2254 6869 7320 7061  lidate":"This pa
-00000510: 6765 2069 736e 2774 2061 7661 696c 6162  ge isn't availab
-00000520: 6c65 220a 2020 207d 2c0a 2020 2022 6c69  le".   },.   "li
-00000530: 6e6b 6564 696e 2d63 6f6d 7061 6e79 223a  nkedin-company":
-00000540: 7b0a 2020 2020 2020 2265 7874 7261 6374  {.      "extract
-00000550: 223a 226c 696e 6b65 6469 6e5c 5c2e 636f  ":"linkedin\\.co
-00000560: 6d5c 5c2f 636f 6d70 616e 795c 5c2f 5b5c  m\\/company\\/[\
-00000570: 5c77 5c5c 645c 5c2d 5c5c 2b5c 5c2e 5d2b  \w\\d\\-\\+\\.]+
-00000580: 283f 3c21 5c5c 2e29 222c 0a20 2020 2020  (?<!\\.)",.     
-00000590: 2022 6578 7472 6163 745f 7072 6570 656e   "extract_prepen
-000005a0: 6422 3a22 6874 7470 733a 2f2f 6872 2e22  d":"https://hr."
-000005b0: 2c0a 2020 2020 2020 2276 616c 6964 6174  ,.      "validat
-000005c0: 6522 3a22 5061 6765 206e 6f74 2066 6f75  e":"Page not fou
-000005d0: 6e64 220a 2020 207d 2c0a 2020 2022 6c69  nd".   },.   "li
-000005e0: 6e6b 6564 696e 2d75 7365 7222 3a7b 0a20  nkedin-user":{. 
-000005f0: 2020 2020 2022 6578 7472 6163 7422 3a22       "extract":"
-00000600: 6c69 6e6b 6564 696e 5c5c 2e63 6f6d 5c5c  linkedin\\.com\\
-00000610: 2f69 6e5c 5c2f 5b5c 5c77 5c5c 645c 5c2d  /in\\/[\\w\\d\\-
-00000620: 5c5c 2b5c 5c2e 5d2b 283f 3c21 5c5c 2e29  \\+\\.]+(?<!\\.)
-00000630: 222c 0a20 2020 2020 2022 6578 7472 6163  ",.      "extrac
-00000640: 745f 7072 6570 656e 6422 3a22 6874 7470  t_prepend":"http
-00000650: 733a 2f2f 6872 2e22 2c0a 2020 2020 2020  s://hr.",.      
-00000660: 2276 616c 6964 6174 6522 3a22 416e 2065  "validate":"An e
-00000670: 7861 6374 206d 6174 6368 2066 6f72 202e  xact match for .
-00000680: 2b20 636f 756c 6420 6e6f 7420 6265 2066  + could not be f
-00000690: 6f75 6e64 5c5c 2e22 0a20 2020 7d0a 7d0a  ound\\.".   }.}.
+00000000: 7b0d 0a20 2020 2274 656c 6567 7261 6d22  {..   "telegram"
+00000010: 3a7b 0d0a 2020 2020 2020 2265 7874 7261  :{..      "extra
+00000020: 6374 223a 2274 5c5c 2e6d 655c 5c2f 5b5c  ct":"t\\.me\\/[\
+00000030: 5c77 5c5c 645c 5c2d 5c5c 2b5d 2b22 2c0d  \w\\d\\-\\+]+",.
+00000040: 0a20 2020 2020 2022 6578 7472 6163 745f  .      "extract_
+00000050: 7072 6570 656e 6422 3a22 6874 7470 733a  prepend":"https:
+00000060: 2f2f 222c 0d0a 2020 2020 2020 2276 616c  //",..      "val
+00000070: 6964 6174 6522 3a22 3c6d 6574 6120 7072  idate":"<meta pr
+00000080: 6f70 6572 7479 3d5c 226f 673a 7469 746c  operty=\"og:titl
+00000090: 655c 2220 636f 6e74 656e 743d 5c22 5465  e\" content=\"Te
+000000a0: 6c65 6772 616d 3a20 436f 6e74 6163 7420  legram: Contact 
+000000b0: 2e2b 3f5c 223e 220d 0a20 2020 7d2c 0d0a  .+?\">"..   },..
+000000c0: 2020 2022 6469 7363 6f72 6422 3a7b 0d0a     "discord":{..
+000000d0: 2020 2020 2020 2265 7874 7261 6374 223a        "extract":
+000000e0: 2264 6973 636f 7264 5c5c 2e63 6f6d 5c5c  "discord\\.com\\
+000000f0: 2f69 6e76 6974 655c 5c2f 5b5c 5c77 5c5c  /invite\\/[\\w\\
+00000100: 645c 5c2d 5c5c 2b5c 5c2e 5d2b 283f 3c21  d\\-\\+\\.]+(?<!
+00000110: 5c5c 2e29 222c 0d0a 2020 2020 2020 2265  \\.)",..      "e
+00000120: 7874 7261 6374 5f70 7265 7065 6e64 223a  xtract_prepend":
+00000130: 2268 7474 7073 3a2f 2f22 2c0d 0a20 2020  "https://",..   
+00000140: 2020 2022 7661 6c69 6461 7465 223a 2249     "validate":"I
+00000150: 6e76 6974 6520 496e 7661 6c69 6422 0d0a  nvite Invalid"..
+00000160: 2020 207d 2c0d 0a20 2020 2279 6f75 7475     },..   "youtu
+00000170: 6265 223a 7b0d 0a20 2020 2020 2022 6578  be":{..      "ex
+00000180: 7472 6163 7422 3a22 796f 7574 7562 655c  tract":"youtube\
+00000190: 5c2e 636f 6d5c 5c2f 283f 3a63 7c63 6861  \.com\\/(?:c|cha
+000001a0: 6e6e 656c 295c 5c2f 5b5c 5c77 5c5c 645c  nnel)\\/[\\w\\d\
+000001b0: 5c2d 5c5c 2b5c 5c2e 5d2b 283f 3c21 5c5c  \-\\+\\.]+(?<!\\
+000001c0: 2e29 222c 0d0a 2020 2020 2020 2265 7874  .)",..      "ext
+000001d0: 7261 6374 5f70 7265 7065 6e64 223a 2268  ract_prepend":"h
+000001e0: 7474 7073 3a2f 2f22 2c0d 0a20 2020 2020  ttps://",..     
+000001f0: 2022 7661 6c69 6461 7465 223a 2254 6869   "validate":"Thi
+00000200: 7320 7061 6765 2069 736e 2774 2061 7661  s page isn't ava
+00000210: 696c 6162 6c65 5c5c 2e22 0d0a 2020 207d  ilable\\."..   }
+00000220: 2c0d 0a20 2020 2274 7769 7474 6572 223a  ,..   "twitter":
+00000230: 7b0d 0a20 2020 2020 2022 6578 7472 6163  {..      "extrac
+00000240: 7422 3a22 283f 3c21 7069 635c 5c2e 2974  t":"(?<!pic\\.)t
+00000250: 7769 7474 6572 5c5c 2e63 6f6d 5c5c 2f28  witter\\.com\\/(
+00000260: 3f3a 283f 2128 3f3a 6861 7368 7461 677c  ?:(?!(?:hashtag|
+00000270: 686f 6d65 7c69 7c69 6e74 656e 747c 7368  home|i|intent|sh
+00000280: 6172 657c 7365 6172 6368 7c65 7870 6c6f  are|search|explo
+00000290: 7265 2928 3f3a 5c5c 2f7c 5c5c 3f29 5b5e  re)(?:\\/|\\?)[^
+000002a0: 5c5c 735d 2b7c 5b5c 5c77 5d2b 5c5c 2f28  \\s]+|[\\w]+\\/(
+000002b0: 3f3a 7072 6976 6163 797c 746f 7329 7c70  ?:privacy|tos)|p
+000002c0: 6572 736f 6e61 6c69 7a61 7469 6f6e 7c77  ersonalization|w
+000002d0: 6964 6765 7473 5c5c 2e6a 7329 5b5c 5c77  idgets\\.js)[\\w
+000002e0: 5c5c 645c 5c2d 5c5c 2b5d 2b29 222c 0d0a  \\d\\-\\+]+)",..
+000002f0: 2020 2020 2020 2265 7874 7261 6374 5f70        "extract_p
+00000300: 7265 7065 6e64 223a 2268 7474 7073 3a2f  repend":"https:/
+00000310: 2f22 2c0d 0a20 2020 2020 2022 7661 6c69  /",..      "vali
+00000320: 6461 7465 223a 2254 6869 7320 6163 636f  date":"This acco
+00000330: 756e 7420 646f 6573 6e2e 3f74 2065 7869  unt doesn.?t exi
+00000340: 7374 220d 0a20 2020 7d2c 0d0a 2020 2022  st"..   },..   "
+00000350: 696e 7374 6167 7261 6d22 3a7b 0d0a 2020  instagram":{..  
+00000360: 2020 2020 2265 7874 7261 6374 223a 2269      "extract":"i
+00000370: 6e73 7461 6772 616d 5c5c 2e63 6f6d 5c5c  nstagram\\.com\\
+00000380: 2f28 3f3a 283f 2128 3f3a 707c 6163 636f  /(?:(?!(?:p|acco
+00000390: 756e 7473 2928 3f3a 5c5c 2f7c 5c5c 3f29  unts)(?:\\/|\\?)
+000003a0: 5b5e 5c5c 735d 2b29 5b5c 5c77 5c5c 645c  [^\\s]+)[\\w\\d\
+000003b0: 5c2d 5c5c 2b5c 5c2e 5d2b 2928 3f3c 215c  \-\\+\\.]+)(?<!\
+000003c0: 5c2e 2922 2c0d 0a20 2020 2020 2022 6578  \.)",..      "ex
+000003d0: 7472 6163 745f 7072 6570 656e 6422 3a22  tract_prepend":"
+000003e0: 6874 7470 733a 2f2f 222c 0d0a 2020 2020  https://",..    
+000003f0: 2020 2265 7874 7261 6374 5f61 7070 656e    "extract_appen
+00000400: 6422 3a22 2f22 2c0d 0a20 2020 2020 2022  d":"/",..      "
+00000410: 7661 6c69 6461 7465 223a 2253 6f72 7279  validate":"Sorry
+00000420: 2c20 7468 6973 2070 6167 6520 6973 6e27  , this page isn'
+00000430: 7420 6176 6169 6c61 626c 655c 5c2e 220d  t available\\.".
+00000440: 0a20 2020 7d2c 0d0a 2020 2022 6661 6365  .   },..   "face
+00000450: 626f 6f6b 223a 7b0d 0a20 2020 2020 2022  book":{..      "
+00000460: 6578 7472 6163 7422 3a22 6661 6365 626f  extract":"facebo
+00000470: 6f6b 5c5c 2e63 6f6d 5c5c 2f28 3f3a 283f  ok\\.com\\/(?:(?
+00000480: 2128 3f3a 6162 6f75 747c 6469 616c 6f67  !(?:about|dialog
+00000490: 7c67 616d 696e 677c 6772 6f75 7073 7c73  |gaming|groups|s
+000004a0: 6861 7265 7229 283f 3a5c 5c2f 7c5c 5c3f  harer)(?:\\/|\\?
+000004b0: 295b 5e5c 5c73 5d2b 7c73 6861 7265 5c5c  )[^\\s]+|share\\
+000004c0: 2e70 6870 7c74 6572 6d73 5c5c 2e70 6870  .php|terms\\.php
+000004d0: 295b 5c5c 775c 5c64 5c5c 2d5c 5c2b 5c5c  )[\\w\\d\\-\\+\\
+000004e0: 2e5d 2b29 283f 3c21 5c5c 2e29 222c 0d0a  .]+)(?<!\\.)",..
+000004f0: 2020 2020 2020 2265 7874 7261 6374 5f70        "extract_p
+00000500: 7265 7065 6e64 223a 2268 7474 7073 3a2f  repend":"https:/
+00000510: 2f22 2c0d 0a20 2020 2020 2022 7661 6c69  /",..      "vali
+00000520: 6461 7465 223a 2254 6869 7320 7061 6765  date":"This page
+00000530: 2069 736e 2774 2061 7661 696c 6162 6c65   isn't available
+00000540: 220d 0a20 2020 7d2c 0d0a 2020 2022 6c69  "..   },..   "li
+00000550: 6e6b 6564 696e 2d63 6f6d 7061 6e79 223a  nkedin-company":
+00000560: 7b0d 0a20 2020 2020 2022 6578 7472 6163  {..      "extrac
+00000570: 7422 3a22 6c69 6e6b 6564 696e 5c5c 2e63  t":"linkedin\\.c
+00000580: 6f6d 5c5c 2f63 6f6d 7061 6e79 5c5c 2f5b  om\\/company\\/[
+00000590: 5c5c 775c 5c64 5c5c 2d5c 5c2b 5c5c 2e5d  \\w\\d\\-\\+\\.]
+000005a0: 2b28 3f3c 215c 5c2e 2922 2c0d 0a20 2020  +(?<!\\.)",..   
+000005b0: 2020 2022 6578 7472 6163 745f 7072 6570     "extract_prep
+000005c0: 656e 6422 3a22 6874 7470 733a 2f2f 6872  end":"https://hr
+000005d0: 2e22 2c0d 0a20 2020 2020 2022 7661 6c69  .",..      "vali
+000005e0: 6461 7465 223a 2250 6167 6520 6e6f 7420  date":"Page not 
+000005f0: 666f 756e 6422 0d0a 2020 207d 2c0d 0a20  found"..   },.. 
+00000600: 2020 226c 696e 6b65 6469 6e2d 7573 6572    "linkedin-user
+00000610: 223a 7b0d 0a20 2020 2020 2022 6578 7472  ":{..      "extr
+00000620: 6163 7422 3a22 6c69 6e6b 6564 696e 5c5c  act":"linkedin\\
+00000630: 2e63 6f6d 5c5c 2f69 6e5c 5c2f 5b5c 5c77  .com\\/in\\/[\\w
+00000640: 5c5c 645c 5c2d 5c5c 2b5c 5c2e 5d2b 283f  \\d\\-\\+\\.]+(?
+00000650: 3c21 5c5c 2e29 222c 0d0a 2020 2020 2020  <!\\.)",..      
+00000660: 2265 7874 7261 6374 5f70 7265 7065 6e64  "extract_prepend
+00000670: 223a 2268 7474 7073 3a2f 2f68 722e 222c  ":"https://hr.",
+00000680: 0d0a 2020 2020 2020 2276 616c 6964 6174  ..      "validat
+00000690: 6522 3a22 416e 2065 7861 6374 206d 6174  e":"An exact mat
+000006a0: 6368 2066 6f72 202e 2b20 636f 756c 6420  ch for .+ could 
+000006b0: 6e6f 7420 6265 2066 6f75 6e64 5c5c 2e22  not be found\\."
+000006c0: 0d0a 2020 207d 0d0a 7d0d 0a              ..   }..}..
```

