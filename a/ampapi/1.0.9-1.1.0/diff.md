# Comparing `tmp/ampapi-1.0.9.tar.gz` & `tmp/ampapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.0.9.tar", last modified: Sat Apr  8 19:39:26 2023, max compression
+gzip compressed data, was "ampapi-1.1.0.tar", last modified: Fri Apr 28 07:56:03 2023, max compression
```

## Comparing `ampapi-1.0.9.tar` & `ampapi-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1160 2022-12-17 05:17:37.000000 ampapi-1.0.9/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-04-08 19:39:26.373114 ampapi-1.0.9/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4206 2023-03-14 23:17:08.000000 ampapi-1.0.9/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2022-12-17 05:17:37.000000 ampapi-1.0.9/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    44610 2023-04-08 19:34:18.000000 ampapi-1.0.9/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-08 19:39:26.373114 ampapi-1.0.9/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4717 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-08 19:39:26.000000 ampapi-1.0.9/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2022-12-23 22:22:45.000000 ampapi-1.0.9/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-08 19:39:26.373114 ampapi-1.0.9/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 07:56:03.228459 ampapi-1.1.0/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-04-28 07:48:40.000000 ampapi-1.1.0/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-28 07:56:03.228459 ampapi-1.1.0/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3620 2023-04-28 07:47:28.000000 ampapi-1.1.0/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 07:56:03.228459 ampapi-1.1.0/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-04-28 01:28:45.000000 ampapi-1.1.0/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)   159328 2023-04-28 07:55:48.000000 ampapi-1.1.0/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-28 07:56:03.228459 ampapi-1.1.0/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-28 07:56:03.000000 ampapi-1.1.0/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-28 07:56:03.000000 ampapi-1.1.0/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-28 07:56:03.000000 ampapi-1.1.0/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-28 07:56:03.000000 ampapi-1.1.0/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-04-28 01:28:45.000000 ampapi-1.1.0/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-28 07:56:03.228459 ampapi-1.1.0/setup.cfg
```

### Comparing `ampapi-1.0.9/LICENCE` & `ampapi-1.1.0/LICENCE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-A Python port of ampapi-node originally written by Mike from CubeCoders Limited - https://github.com/CubeCoders/ampapi-node
+A Python implementation of the AMPAPI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ampapi-1.0.9/PKG-INFO` & `ampapi-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # ampapi-python
 
-## This implementation is under active development, please feel free to contribute or create an issue if you've found anything that needs fixing
-
 This API allows you to communicate with AMP installations from within Python.
 
 Documentation for available API calls can be found by appending /API to the URL of any existing AMP installation.
 
-Please Note: This program is directly based on the [ampapi-node](https://github.com/CubeCoders/ampapi-node) implementation and is almost verbatim in most aspects.
-
 ## Installation
 
 ```bash
 pip install ampapi
 ```
 
 or
@@ -33,15 +29,15 @@
 ```bash
 pip install 'ampapi @ git+https://github.com/p0t4t0sandwich/ampapi-python.git'
 ```
 
 You also need the following packages installed:
 
 ```bash
-pip install requests aiohttp json dataclasses
+pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
 from ampapi.ampapi import AMPAPIAsync
@@ -78,54 +74,40 @@
 ```python
 from ampapi.ampapi import AMPAPI
 
 def start() -> None:
     API = AMPAPI("http://localhost:8080/")
 
     try:
-        # Perform first-stage API initialization.
-        APIInitOK = API.init()
-
-        if not APIInitOK:
-            print("API Init failed")
-            return
-
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
-        loginResult = API.Core.Login("admin", "myfancypassword123", "", False)
+        loginResult = API.Core_Login("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
             API.sessionId = loginResult["sessionID"]
 
-            # Perform second-stage API initialization, we only get the full API data once we're logged in.
-            APIInitOK = API.init()
-            if not APIInitOK:
-                print("API Stage 2 Init failed")
-                return
-
             # API call parameters are simply in the same order as shown in the documentation.
-            API.Core.SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
-            currentStatus = API.Core.GetStatus()
+            API.Core_SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
+            currentStatus = API.Core_GetStatus()
             CPUUsagePercent = currentStatus["Metrics"]["CPU Usage"]["Percent"]
             print(f"Current CPU usage is: {CPUUsagePercent}%")
 
         else:
             print("Login failed")
             print(loginResult)
 
     except Exception as err:
         print(err)
 
 start()
 ```
 
-## Additional Notes
-
-As you may have noticed, the async and non-async implementations differ quite a bit. This is due to lambda functions within python being unable to use async methods. Usually this can be solved by manually defining the function, but as that would be cumbersome, I've opted to create a script to grab the API spec from the AMP API and generate all the needed functions (script found under /utils/ampapi_async_gen.py).
+## Notes on generating implementations
 
-Async implementation: `API.Core_LoginAsync()`
+ampapi-python is generated using a script that parses the API spec. The `ampapai_gen.py` script under `/utils` can be used to generate future versions of the API. It requires the `requests` and `json` packages to be installed.
 
-Sync implementation: `API.Core.Login()`
+To generate a new version, set the AMP_URL, AMP_USERNAME, and AMP_PASSWORD environment variables and run the script.
 
-Additonally, unlike other languages, the "Zen of Python" prevents dot/property notation for dictionaries (Think API.Core.Login). I've used dataclasses and some class properties to bypass this, so in the end:
+## Notes on missing methods
 
-`API.Core.Login() == API["Core"]["Login"]()`.
+The generation script only uses the base ADS APISpec of an AMP Network Licence (my current licence). This means any Enterprise methods, methods added by plugins, or module-specific methods are not included. If you find yourself needing these methods frequently, please use the insance's API endpoint with the `ampapai_gen.py` script under `/utils`, then submit a pull request with the generated code.
+If you need a method that is not included, you can use the `AMPAPI.APICall` method to run the method directly.
```

### Comparing `ampapi-1.0.9/README.md` & `ampapi-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # ampapi-python
 
-## This implementation is under active development, please feel free to contribute or create an issue if you've found anything that needs fixing
-
 This API allows you to communicate with AMP installations from within Python.
 
 Documentation for available API calls can be found by appending /API to the URL of any existing AMP installation.
 
-Please Note: This program is directly based on the [ampapi-node](https://github.com/CubeCoders/ampapi-node) implementation and is almost verbatim in most aspects.
-
 ## Installation
 
 ```bash
 pip install ampapi
 ```
 
 or
@@ -19,15 +15,15 @@
 ```bash
 pip install 'ampapi @ git+https://github.com/p0t4t0sandwich/ampapi-python.git'
 ```
 
 You also need the following packages installed:
 
 ```bash
-pip install requests aiohttp json dataclasses
+pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
 from ampapi.ampapi import AMPAPIAsync
@@ -64,54 +60,40 @@
 ```python
 from ampapi.ampapi import AMPAPI
 
 def start() -> None:
     API = AMPAPI("http://localhost:8080/")
 
     try:
-        # Perform first-stage API initialization.
-        APIInitOK = API.init()
-
-        if not APIInitOK:
-            print("API Init failed")
-            return
-
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
-        loginResult = API.Core.Login("admin", "myfancypassword123", "", False)
+        loginResult = API.Core_Login("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
             API.sessionId = loginResult["sessionID"]
 
-            # Perform second-stage API initialization, we only get the full API data once we're logged in.
-            APIInitOK = API.init()
-            if not APIInitOK:
-                print("API Stage 2 Init failed")
-                return
-
             # API call parameters are simply in the same order as shown in the documentation.
-            API.Core.SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
-            currentStatus = API.Core.GetStatus()
+            API.Core_SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
+            currentStatus = API.Core_GetStatus()
             CPUUsagePercent = currentStatus["Metrics"]["CPU Usage"]["Percent"]
             print(f"Current CPU usage is: {CPUUsagePercent}%")
 
         else:
             print("Login failed")
             print(loginResult)
 
     except Exception as err:
         print(err)
 
 start()
 ```
 
-## Additional Notes
-
-As you may have noticed, the async and non-async implementations differ quite a bit. This is due to lambda functions within python being unable to use async methods. Usually this can be solved by manually defining the function, but as that would be cumbersome, I've opted to create a script to grab the API spec from the AMP API and generate all the needed functions (script found under /utils/ampapi_async_gen.py).
+## Notes on generating implementations
 
-Async implementation: `API.Core_LoginAsync()`
+ampapi-python is generated using a script that parses the API spec. The `ampapai_gen.py` script under `/utils` can be used to generate future versions of the API. It requires the `requests` and `json` packages to be installed.
 
-Sync implementation: `API.Core.Login()`
+To generate a new version, set the AMP_URL, AMP_USERNAME, and AMP_PASSWORD environment variables and run the script.
 
-Additonally, unlike other languages, the "Zen of Python" prevents dot/property notation for dictionaries (Think API.Core.Login). I've used dataclasses and some class properties to bypass this, so in the end:
+## Notes on missing methods
 
-`API.Core.Login() == API["Core"]["Login"]()`.
+The generation script only uses the base ADS APISpec of an AMP Network Licence (my current licence). This means any Enterprise methods, methods added by plugins, or module-specific methods are not included. If you find yourself needing these methods frequently, please use the insance's API endpoint with the `ampapai_gen.py` script under `/utils`, then submit a pull request with the generated code.
+If you need a method that is not included, you can use the `AMPAPI.APICall` method to run the method directly.
```

### Comparing `ampapi-1.0.9/ampapi.egg-info/PKG-INFO` & `ampapi-1.1.0/ampapi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.0.9
+Version: 1.1.0
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # ampapi-python
 
-## This implementation is under active development, please feel free to contribute or create an issue if you've found anything that needs fixing
-
 This API allows you to communicate with AMP installations from within Python.
 
 Documentation for available API calls can be found by appending /API to the URL of any existing AMP installation.
 
-Please Note: This program is directly based on the [ampapi-node](https://github.com/CubeCoders/ampapi-node) implementation and is almost verbatim in most aspects.
-
 ## Installation
 
 ```bash
 pip install ampapi
 ```
 
 or
@@ -33,15 +29,15 @@
 ```bash
 pip install 'ampapi @ git+https://github.com/p0t4t0sandwich/ampapi-python.git'
 ```
 
 You also need the following packages installed:
 
 ```bash
-pip install requests aiohttp json dataclasses
+pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
 from ampapi.ampapi import AMPAPIAsync
@@ -78,54 +74,40 @@
 ```python
 from ampapi.ampapi import AMPAPI
 
 def start() -> None:
     API = AMPAPI("http://localhost:8080/")
 
     try:
-        # Perform first-stage API initialization.
-        APIInitOK = API.init()
-
-        if not APIInitOK:
-            print("API Init failed")
-            return
-
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
-        loginResult = API.Core.Login("admin", "myfancypassword123", "", False)
+        loginResult = API.Core_Login("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
             API.sessionId = loginResult["sessionID"]
 
-            # Perform second-stage API initialization, we only get the full API data once we're logged in.
-            APIInitOK = API.init()
-            if not APIInitOK:
-                print("API Stage 2 Init failed")
-                return
-
             # API call parameters are simply in the same order as shown in the documentation.
-            API.Core.SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
-            currentStatus = API.Core.GetStatus()
+            API.Core_SendConsoleMessage("say Hello Everyone, this message was sent from the Python API!")
+            currentStatus = API.Core_GetStatus()
             CPUUsagePercent = currentStatus["Metrics"]["CPU Usage"]["Percent"]
             print(f"Current CPU usage is: {CPUUsagePercent}%")
 
         else:
             print("Login failed")
             print(loginResult)
 
     except Exception as err:
         print(err)
 
 start()
 ```
 
-## Additional Notes
-
-As you may have noticed, the async and non-async implementations differ quite a bit. This is due to lambda functions within python being unable to use async methods. Usually this can be solved by manually defining the function, but as that would be cumbersome, I've opted to create a script to grab the API spec from the AMP API and generate all the needed functions (script found under /utils/ampapi_async_gen.py).
+## Notes on generating implementations
 
-Async implementation: `API.Core_LoginAsync()`
+ampapi-python is generated using a script that parses the API spec. The `ampapai_gen.py` script under `/utils` can be used to generate future versions of the API. It requires the `requests` and `json` packages to be installed.
 
-Sync implementation: `API.Core.Login()`
+To generate a new version, set the AMP_URL, AMP_USERNAME, and AMP_PASSWORD environment variables and run the script.
 
-Additonally, unlike other languages, the "Zen of Python" prevents dot/property notation for dictionaries (Think API.Core.Login). I've used dataclasses and some class properties to bypass this, so in the end:
+## Notes on missing methods
 
-`API.Core.Login() == API["Core"]["Login"]()`.
+The generation script only uses the base ADS APISpec of an AMP Network Licence (my current licence). This means any Enterprise methods, methods added by plugins, or module-specific methods are not included. If you find yourself needing these methods frequently, please use the insance's API endpoint with the `ampapai_gen.py` script under `/utils`, then submit a pull request with the generated code.
+If you need a method that is not included, you can use the `AMPAPI.APICall` method to run the method directly.
```

### Comparing `ampapi-1.0.9/setup.cfg` & `ampapi-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.0.9
+version = 1.1.0
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```

