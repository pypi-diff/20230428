# Comparing `tmp/forbidden-9.4.tar.gz` & `tmp/forbidden-9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forbidden-9.4.tar", last modified: Sun Apr  9 11:50:09 2023, max compression
+gzip compressed data, was "forbidden-9.5.tar", last modified: Fri Apr 28 13:45:53 2023, max compression
```

## Comparing `forbidden-9.4.tar` & `forbidden-9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 11:50:09.153534 forbidden-9.4/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-08 16:54:53.000000 forbidden-9.4/LICENSE
--rwxrwx---   0 root         (0) root         (0)      112 2023-04-08 16:54:53.000000 forbidden-9.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-09 11:50:09.153534 forbidden-9.4/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)    11959 2023-04-08 17:28:40.000000 forbidden-9.4/README.md
--rwxrwx---   0 root         (0) root         (0)      784 2023-04-08 17:12:01.000000 forbidden-9.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 11:50:09.153534 forbidden-9.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 11:50:09.149532 forbidden-9.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 11:50:09.153534 forbidden-9.4/src/forbidden/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-08 17:10:56.000000 forbidden-9.4/src/forbidden/__init__.py
--rwxrwx---   0 root         (0) root         (0)    43386 2023-04-09 11:50:01.000000 forbidden-9.4/src/forbidden/forbidden.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-08 17:29:14.000000 forbidden-9.4/src/forbidden/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 11:50:09.153534 forbidden-9.4/src/forbidden.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12383 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-09 11:50:09.000000 forbidden-9.4/src/forbidden.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 11:50:09.153534 forbidden-9.4/src/stresser/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-08 17:10:56.000000 forbidden-9.4/src/stresser/__init__.py
--rwxrwx---   0 root         (0) root         (0)    19181 2023-04-09 11:49:19.000000 forbidden-9.4/src/stresser/stresser.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-08 17:29:16.000000 forbidden-9.4/src/stresser/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.365278 forbidden-9.5/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:41:20.000000 forbidden-9.5/LICENSE
+-rwxrwx---   0 root         (0) root         (0)      112 2023-04-28 13:41:20.000000 forbidden-9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-28 13:45:53.365278 forbidden-9.5/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)    12428 2023-04-28 13:42:18.000000 forbidden-9.5/README.md
+-rwxrwx---   0 root         (0) root         (0)      814 2023-04-28 13:41:36.000000 forbidden-9.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:45:53.365278 forbidden-9.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/forbidden/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.5/src/forbidden/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    44708 2023-04-28 13:45:03.000000 forbidden-9.5/src/forbidden/forbidden.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.5/src/forbidden/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.361276 forbidden-9.5/src/forbidden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 13:45:53.000000 forbidden-9.5/src/forbidden.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:45:53.365278 forbidden-9.5/src/stresser/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:41:20.000000 forbidden-9.5/src/stresser/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    19791 2023-04-28 13:44:58.000000 forbidden-9.5/src/stresser/stresser.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-04-28 13:41:20.000000 forbidden-9.5/src/stresser/user_agents.txt
```

### Comparing `forbidden-9.4/LICENSE` & `forbidden-9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `forbidden-9.4/PKG-INFO` & `forbidden-9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forbidden
-Version: 9.4
+Version: 9.5
 Summary: Bypass 4xx HTTP response status codes and more.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -89,15 +89,15 @@
 * [URL Paths](#url-paths)
 * [Results Format](#results-format)
 * [Usage](#usage)
 
 ## How to Install
 
 ```bash
-apt-get install -y libcurl4-gnutls-dev librtmp-dev
+apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 pip3 install forbidden
 
 pip3 install --upgrade forbidden
 ```
 
 ## How to Build and Install Manually
@@ -109,15 +109,15 @@
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.4-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.5-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -346,39 +346,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.4",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.4' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.5",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.4",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.4' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.5",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.4 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.5 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -421,26 +421,26 @@
     Number of parallel threads to run
     More threads make it quicker but can give worse results
     Heavily depends on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.4
+    Default: Forbidden/9.5
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
 ```
 
 ```fundamental
-Stresser v4.4 ( github.com/ivan-sincek/forbidden )
+Stresser v4.5 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -467,15 +467,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.4
+    Default: Stresser/4.5
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.4/README.md` & `forbidden-9.5/src/forbidden.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: forbidden
+Version: 9.5
+Summary: Bypass 4xx HTTP response status codes and more.
+Author: Ivan Sincek
+Project-URL: Homepage, https://github.com/ivan-sincek/forbidden
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Forbidden
 
 Bypass 4xx HTTP response status codes and more. Based on PycURL.
 
 Script uses multithreading and is based on brute forcing, so it might have some false positive results. Script has colored output.
 
 Results will be sorted by HTTP response status code ascending, content length descending, and ID ascending.
@@ -76,15 +89,15 @@
 * [URL Paths](#url-paths)
 * [Results Format](#results-format)
 * [Usage](#usage)
 
 ## How to Install
 
 ```bash
-apt-get install -y libcurl4-gnutls-dev librtmp-dev
+apt-get -y install libcurl4-gnutls-dev librtmp-dev
 
 pip3 install forbidden
 
 pip3 install --upgrade forbidden
 ```
 
 ## How to Build and Install Manually
@@ -96,15 +109,15 @@
 
 git clone https://github.com/ivan-sincek/forbidden && cd forbidden
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/forbidden-9.4-py3-none-any.whl
+python3 -m pip install dist/forbidden-9.5-py3-none-any.whl
 ```
 
 ## Automation
 
 Bypass `403 Forbidden` HTTP response status code:
 
 ```bash
@@ -333,39 +346,39 @@
       "id":"570-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1"
       ],
       "body":null,
-      "agent":"Forbidden/9.4",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.4' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.5",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    },
    {
       "id":"571-HEADERS-2",
       "url":"https://example.com:443/admin",
       "method":"GET",
       "headers":[
          "Host: 127.0.0.1:443"
       ],
       "body":null,
-      "agent":"Forbidden/9.4",
-      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.4' -X 'GET' 'https://example.com:443/admin'",
+      "agent":"Forbidden/9.5",
+      "command":"curl --connect-timeout 90 -m 180 -iskL --max-redirs 10 --path-as-is -H 'Host: 127.0.0.1:443' -H 'User-Agent: Forbidden/9.5' -X 'GET' 'https://example.com:443/admin'",
       "code":200,
       "length":255408
    }
 ]
 ```
 
 ## Usage
 
 ```fundamental
-Forbidden v9.4 ( github.com/ivan-sincek/forbidden )
+Forbidden v9.5 ( github.com/ivan-sincek/forbidden )
 
 Usage:   forbidden -u url                       -t tests [-f force] [-v values    ] [-p path            ] [-o out         ]
 Example: forbidden -u https://example.com/admin -t all   [-f GET  ] [-v values.txt] [-p /home/index.html] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes and more
 URL
@@ -408,26 +421,26 @@
     Number of parallel threads to run
     More threads make it quicker but can give worse results
     Heavily depends on network bandwidth and server capacity
     Default: 5
     -th <threads> - 200 | etc.
 AGENT
     User agent to use
-    Default: Forbidden/9.4
+    Default: Forbidden/9.5
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
 ```
 
 ```fundamental
-Stresser v4.4 ( github.com/ivan-sincek/forbidden )
+Stresser v4.5 ( github.com/ivan-sincek/forbidden )
 
 Usage:   stresser -u url                        -dir directory -r repeat -th threads [-f force] [-o out         ]
 Example: stresser -u https://example.com/secret -dir results   -r 1000   -th 200     [-f GET  ] [-o results.json]
 
 DESCRIPTION
     Bypass 4xx HTTP response status codes with stress testing
 URL
@@ -454,15 +467,15 @@
 LENGTHS
     Filter out 200 OK false positive results by content lengths
     Specify 'base' to ignore content length of base HTTP response
     Use comma separated values
     -l <lengths> - 12 | base | etc.
 AGENT
     User agent to use
-    Default: Stresser/4.4
+    Default: Stresser/4.5
     -a <agent> - curl/3.30.1 | random[-all] | etc.
 PROXY
     Web proxy to use
     -x <proxy> - 127.0.0.1:8080 | etc.
 OUT
     Output file
     -o <out> - results.json | etc.
```

### Comparing `forbidden-9.4/pyproject.toml` & `forbidden-9.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "forbidden"
-version = "9.4"
-authors = [{ name = "Ivan Sincek" }]
-description = "Bypass 4xx HTTP response status codes and more."
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-	"Programming Language :: Python :: 3",
-	"License :: OSI Approved :: MIT License",
-	"Operating System :: OS Independent"
-]
-dependencies = ["datetime>=5.0", "requests>=2.10.0", "pycurl>=7.45.1", "termcolor>=1.1.0"]
-
-[project.urls]
-"Homepage" = "https://github.com/ivan-sincek/forbidden"
-
-[project.scripts]
-forbidden = "forbidden.forbidden:main"
-stresser = "stresser.stresser:main"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.package-data]
-"*" = ["user_agents.txt"]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "forbidden"
+version = "9.5"
+authors = [{ name = "Ivan Sincek" }]
+description = "Bypass 4xx HTTP response status codes and more."
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [
+	"Programming Language :: Python :: 3",
+	"License :: OSI Approved :: MIT License",
+	"Operating System :: OS Independent"
+]
+dependencies = ["datetime>=5.0", "requests>=2.10.0", "pycurl>=7.45.1", "termcolor>=1.1.0"]
+
+[project.urls]
+"Homepage" = "https://github.com/ivan-sincek/forbidden"
+
+[project.scripts]
+forbidden = "forbidden.forbidden:main"
+stresser = "stresser.stresser:main"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["user_agents.txt"]
```

### Comparing `forbidden-9.4/src/forbidden/user_agents.txt` & `forbidden-9.5/src/forbidden/user_agents.txt`

 * *Files identical despite different names*

### Comparing `forbidden-9.4/src/stresser/user_agents.txt` & `forbidden-9.5/src/stresser/user_agents.txt`

 * *Files identical despite different names*

