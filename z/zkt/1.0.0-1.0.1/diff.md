# Comparing `tmp/zkt-1.0.0.tar.gz` & `tmp/zkt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkt-1.0.0.tar", last modified: Fri Apr 28 00:49:35 2023, max compression
+gzip compressed data, was "zkt-1.0.1.tar", last modified: Fri Apr 28 00:55:08 2023, max compression
```

## Comparing `zkt-1.0.0.tar` & `zkt-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:49:35.221606 zkt-1.0.0/
--rw-rw-rw-   0        0        0     1957 2023-04-28 00:49:35.222614 zkt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2023-04-28 00:39:30.000000 zkt-1.0.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-28 00:49:35.234817 zkt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-04-28 00:42:54.000000 zkt-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:49:35.152705 zkt-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:49:35.161840 zkt-1.0.0/src/zkt/
--rw-rw-rw-   0        0        0     2549 2023-04-28 00:23:33.000000 zkt-1.0.0/src/zkt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:49:35.201574 zkt-1.0.0/src/zkt/steps/
--rw-rw-rw-   0        0        0     3000 2023-04-28 00:29:38.000000 zkt-1.0.0/src/zkt/steps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:49:35.199574 zkt-1.0.0/src/zkt.egg-info/
--rw-rw-rw-   0        0        0     1957 2023-04-28 00:49:35.000000 zkt-1.0.0/src/zkt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-28 00:49:35.000000 zkt-1.0.0/src/zkt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:49:35.000000 zkt-1.0.0/src/zkt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 00:49:35.000000 zkt-1.0.0/src/zkt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 00:49:35.000000 zkt-1.0.0/src/zkt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 00:55:08.950526 zkt-1.0.1/
+-rw-rw-rw-   0        0        0     1955 2023-04-28 00:55:08.951528 zkt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1600 2023-04-28 00:54:41.000000 zkt-1.0.1/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-28 00:55:08.954036 zkt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      683 2023-04-28 00:54:21.000000 zkt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:55:08.879685 zkt-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 00:55:08.888211 zkt-1.0.1/src/zkt/
+-rw-rw-rw-   0        0        0     2549 2023-04-28 00:23:33.000000 zkt-1.0.1/src/zkt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:55:08.926948 zkt-1.0.1/src/zkt/steps/
+-rw-rw-rw-   0        0        0     3000 2023-04-28 00:29:38.000000 zkt-1.0.1/src/zkt/steps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 00:55:08.924940 zkt-1.0.1/src/zkt.egg-info/
+-rw-rw-rw-   0        0        0     1955 2023-04-28 00:55:08.000000 zkt-1.0.1/src/zkt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-28 00:55:08.000000 zkt-1.0.1/src/zkt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 00:55:08.000000 zkt-1.0.1/src/zkt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 00:55:08.000000 zkt-1.0.1/src/zkt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 00:55:08.000000 zkt-1.0.1/src/zkt.egg-info/top_level.txt
```

### Comparing `zkt-1.0.0/PKG-INFO` & `zkt-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper tool for api test automation
 Home-page: https://github.com/gmyrianthous/example-publish-pypi
 Author: Noé Cruz
 Author-email: contactozurckz@gmail.com
 License: MIT
 Keywords: zurckz test testing
 Platform: UNKNOWN
@@ -55,15 +55,15 @@
 ```python
 
 
 
     test_scenario = Stepexecutor(
         scenario="Create a Generic Order PROD",
         steps=[
-            FullRequestTest("Prepare token request", picker_express),
+            FullRequestTest("Prepare token request", data_request),
             PostHttpRequest("Get Token"),
             HttpResponseVerifier("Tooken Response Verifier"),
             DictValueExtract("Extract Data Tokens", key="result"),
             StoreTransactData("Store Auth Data", key="auth")
         ],
     )
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: zkt Version: 1.0.0 Summary: Helper tool for api
+Metadata-Version: 2.1 Name: zkt Version: 1.0.1 Summary: Helper tool for api
 test automation Home-page: https://github.com/gmyrianthous/example-publish-pypi
 Author: NoÃ© Cruz Author-email: contactozurckz@gmail.com License: MIT Keywords:
 zurckz test testing Platform: UNKNOWN Requires-Python: >=3.6 Description-
 Content-Type: text/markdown
                                    [Zurck'z]
                           Zkt for API Test Automation
 --- # Zkt > Zurck'z Testing Tool This package contains some helpers features
 for api test automation ZPy use the following packages: - zpy-api-core ##
 Requirements - Python 3.10+ ## Installation Use the package manager [pip]
 (https://pip.pypa.io/en/stable/) to install py flask micro service core .
 ```bash pip install zkt ``` ## Features Contains some helper features. - Stage
 - Step ## Basic Usage ```python test_scenario = Stepexecutor( scenario="Create
 a Generic Order PROD", steps=[ FullRequestTest("Prepare token request",
-picker_express), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
+data_request), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
 Response Verifier"), DictValueExtract("Extract Data Tokens", key="result"),
 StoreTransactData("Store Auth Data", key="auth") ], ) result =
 test_scenario.execute() print(result) ``` ## Contributing Pull requests are
 welcome. For major changes, please open an issue first to discuss what you
 would like to change. Please make sure to update tests as appropriate. ##
 License [MIT](https://choosealicense.com/licenses/mit/) ## Authors [NoÃ© Cruz]
 (https://www.linkedin.com/in/zurckz/)
```

### Comparing `zkt-1.0.0/README.md` & `zkt-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ```python
 
 
 
     test_scenario = Stepexecutor(
         scenario="Create a Generic Order PROD",
         steps=[
-            FullRequestTest("Prepare token request", picker_express),
+            FullRequestTest("Prepare token request", data_request),
             PostHttpRequest("Get Token"),
             HttpResponseVerifier("Tooken Response Verifier"),
             DictValueExtract("Extract Data Tokens", key="result"),
             StoreTransactData("Store Auth Data", key="auth")
         ],
     )
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 --- # Zkt > Zurck'z Testing Tool This package contains some helpers features
 for api test automation ZPy use the following packages: - zpy-api-core ##
 Requirements - Python 3.10+ ## Installation Use the package manager [pip]
 (https://pip.pypa.io/en/stable/) to install py flask micro service core .
 ```bash pip install zkt ``` ## Features Contains some helper features. - Stage
 - Step ## Basic Usage ```python test_scenario = Stepexecutor( scenario="Create
 a Generic Order PROD", steps=[ FullRequestTest("Prepare token request",
-picker_express), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
+data_request), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
 Response Verifier"), DictValueExtract("Extract Data Tokens", key="result"),
 StoreTransactData("Store Auth Data", key="auth") ], ) result =
 test_scenario.execute() print(result) ``` ## Contributing Pull requests are
 welcome. For major changes, please open an issue first to discuss what you
 would like to change. Please make sure to update tests as appropriate. ##
 License [MIT](https://choosealicense.com/licenses/mit/) ## Authors [NoÃ© Cruz]
 (https://www.linkedin.com/in/zurckz/)
```

### Comparing `zkt-1.0.0/setup.py` & `zkt-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="zkt",
-    version="1.0.0",
+    version="1.0.1",
     license="MIT",
     author="Noé Cruz",
     author_email="contactozurckz@gmail.com",
     description="Helper tool for api test automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages("src"),
```

### Comparing `zkt-1.0.0/src/zkt/__init__.py` & `zkt-1.0.1/src/zkt/__init__.py`

 * *Files identical despite different names*

### Comparing `zkt-1.0.0/src/zkt/steps/__init__.py` & `zkt-1.0.1/src/zkt/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `zkt-1.0.0/src/zkt.egg-info/PKG-INFO` & `zkt-1.0.1/src/zkt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper tool for api test automation
 Home-page: https://github.com/gmyrianthous/example-publish-pypi
 Author: Noé Cruz
 Author-email: contactozurckz@gmail.com
 License: MIT
 Keywords: zurckz test testing
 Platform: UNKNOWN
@@ -55,15 +55,15 @@
 ```python
 
 
 
     test_scenario = Stepexecutor(
         scenario="Create a Generic Order PROD",
         steps=[
-            FullRequestTest("Prepare token request", picker_express),
+            FullRequestTest("Prepare token request", data_request),
             PostHttpRequest("Get Token"),
             HttpResponseVerifier("Tooken Response Verifier"),
             DictValueExtract("Extract Data Tokens", key="result"),
             StoreTransactData("Store Auth Data", key="auth")
         ],
     )
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: zkt Version: 1.0.0 Summary: Helper tool for api
+Metadata-Version: 2.1 Name: zkt Version: 1.0.1 Summary: Helper tool for api
 test automation Home-page: https://github.com/gmyrianthous/example-publish-pypi
 Author: NoÃ© Cruz Author-email: contactozurckz@gmail.com License: MIT Keywords:
 zurckz test testing Platform: UNKNOWN Requires-Python: >=3.6 Description-
 Content-Type: text/markdown
                                    [Zurck'z]
                           Zkt for API Test Automation
 --- # Zkt > Zurck'z Testing Tool This package contains some helpers features
 for api test automation ZPy use the following packages: - zpy-api-core ##
 Requirements - Python 3.10+ ## Installation Use the package manager [pip]
 (https://pip.pypa.io/en/stable/) to install py flask micro service core .
 ```bash pip install zkt ``` ## Features Contains some helper features. - Stage
 - Step ## Basic Usage ```python test_scenario = Stepexecutor( scenario="Create
 a Generic Order PROD", steps=[ FullRequestTest("Prepare token request",
-picker_express), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
+data_request), PostHttpRequest("Get Token"), HttpResponseVerifier("Tooken
 Response Verifier"), DictValueExtract("Extract Data Tokens", key="result"),
 StoreTransactData("Store Auth Data", key="auth") ], ) result =
 test_scenario.execute() print(result) ``` ## Contributing Pull requests are
 welcome. For major changes, please open an issue first to discuss what you
 would like to change. Please make sure to update tests as appropriate. ##
 License [MIT](https://choosealicense.com/licenses/mit/) ## Authors [NoÃ© Cruz]
 (https://www.linkedin.com/in/zurckz/)
```

