# Comparing `tmp/ta_sites-0.4.4.tar.gz` & `tmp/ta_sites-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-qh4up5mt/ta_sites-0.4.4.tar", last modified: Fri Mar 17 15:26:06 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-kfgtcee9/ta_sites-0.4.5.tar", last modified: Fri Apr 28 11:04:51 2023, max compression
```

## Comparing `ta_sites-0.4.4.tar` & `ta_sites-0.4.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-03-17 15:25:44.000000 ta_sites-0.4.4/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-03-17 15:25:44.000000 ta_sites-0.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-03-17 15:26:06.020761 ta_sites-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-03-17 15:25:44.000000 ta_sites-0.4.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-03-17 15:26:06.020761 ta_sites-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-03-17 15:25:44.000000 ta_sites-0.4.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.016761 ta_sites-0.4.4/ta_sites/
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.016761 ta_sites-0.4.4/ta_sites/always_care/
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/always_care/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/always_care/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9569 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/always_care/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/ta_sites/basic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/basic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4304 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/basic/core.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/basic/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/ta_sites/central_reach/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/central_reach/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17159 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/central_reach/core.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/central_reach/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9608 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/central_reach/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/ta_sites/quickbooks/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/quickbooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25674 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/quickbooks/core.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/quickbooks/grouped_row.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/ta_sites/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2654 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/salesforce/core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.020761 ta_sites-0.4.4/ta_sites/versant/
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/versant/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/versant/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10568 2023-03-17 15:25:44.000000 ta_sites-0.4.4/ta_sites/versant/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 15:26:06.016761 ta_sites-0.4.4/ta_sites.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-03-17 15:26:05.000000 ta_sites-0.4.4/ta_sites.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-03-17 15:26:06.000000 ta_sites-0.4.4/ta_sites.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-17 15:26:05.000000 ta_sites-0.4.4/ta_sites.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-17 15:26:05.000000 ta_sites-0.4.4/ta_sites.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-17 15:26:05.000000 ta_sites-0.4.4/ta_sites.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-03-17 15:26:06.000000 ta_sites-0.4.4/ta_sites.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-28 11:04:30.000000 ta_sites-0.4.5/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-28 11:04:30.000000 ta_sites-0.4.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-28 11:04:50.997998 ta_sites-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-04-28 11:04:30.000000 ta_sites-0.4.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-28 11:04:50.997998 ta_sites-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-28 11:04:30.000000 ta_sites-0.4.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites/always_care/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9569 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/always_care/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/basic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4304 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/basic/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/central_reach/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17159 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9652 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/central_reach/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/quickbooks/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25674 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/quickbooks/grouped_row.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/salesforce/core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.997998 ta_sites-0.4.5/ta_sites/versant/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10568 2023-04-28 11:04:30.000000 ta_sites-0.4.5/ta_sites/versant/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-28 11:04:50.993998 ta_sites-0.4.5/ta_sites.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-28 11:04:50.000000 ta_sites-0.4.5/ta_sites.egg-info/top_level.txt
```

### Comparing `ta_sites-0.4.4/LICENSE` & `ta_sites-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/PKG-INFO` & `ta_sites-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta_sites
-Version: 0.4.4
+Version: 0.4.5
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ta_sites-0.4.4/setup.py` & `ta_sites-0.4.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
     name="ta_sites",
-    version="0.4.4",
+    version="0.4.5",
     packages=[
         "ta_sites",
         "ta_sites.central_reach",
         "ta_sites.basic",
         "ta_sites.quickbooks",
         "ta_sites.salesforce",
         "ta_sites.versant",
```

### Comparing `ta_sites-0.4.4/ta_sites/__init__.py` & `ta_sites-0.4.5/ta_sites/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/always_care/requests_core.py` & `ta_sites-0.4.5/ta_sites/always_care/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/basic/core.py` & `ta_sites-0.4.5/ta_sites/basic/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/central_reach/__init__.py` & `ta_sites-0.4.5/ta_sites/central_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/central_reach/core.py` & `ta_sites-0.4.5/ta_sites/central_reach/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/central_reach/exceptions.py` & `ta_sites-0.4.5/ta_sites/central_reach/exceptions.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/central_reach/requests_core.py` & `ta_sites-0.4.5/ta_sites/central_reach/requests_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """
         Prepare header object for request.
 
         :param is_json (bool): True if content-type should be json, else False.
         :param add_headers (dict): dictionary with key-values that should be added to headers.
         :param put_token (bool): True if 'csrf-token' should be added to headers, else False.
         """
-        headers = {}
+        headers = {"origin": "https://members.centralreach.com"}
         if is_json:
             headers["content-type"] = "application/json; charset=UTF-8"
 
         if put_token:
             headers["x-csrf-token"] = self._session_csrf_token
 
         if add_headers:
```

### Comparing `ta_sites-0.4.4/ta_sites/quickbooks/core.py` & `ta_sites-0.4.5/ta_sites/quickbooks/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/quickbooks/grouped_row.py` & `ta_sites-0.4.5/ta_sites/quickbooks/grouped_row.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/salesforce/core.py` & `ta_sites-0.4.5/ta_sites/salesforce/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites/versant/requests_core.py` & `ta_sites-0.4.5/ta_sites/versant/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.4/ta_sites.egg-info/PKG-INFO` & `ta_sites-0.4.5/ta_sites.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ta-sites
-Version: 0.4.4
+Version: 0.4.5
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ta_sites-0.4.4/ta_sites.egg-info/SOURCES.txt` & `ta_sites-0.4.5/ta_sites.egg-info/SOURCES.txt`

 * *Files identical despite different names*

