# Comparing `tmp/luscioustwitch-0.3.8.tar.gz` & `tmp/luscioustwitch-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luscioustwitch-0.3.8.tar", last modified: Tue Apr 11 04:28:45 2023, max compression
+gzip compressed data, was "luscioustwitch-0.3.9.tar", last modified: Fri Apr 28 05:18:13 2023, max compression
```

## Comparing `luscioustwitch-0.3.8.tar` & `luscioustwitch-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 04:28:45.870251 luscioustwitch-0.3.8/
--rw-rw-rw-   0        0        0    35823 2023-02-18 18:00:33.000000 luscioustwitch-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      618 2023-04-11 04:28:45.869752 luscioustwitch-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-03-08 02:46:28.000000 luscioustwitch-0.3.8/README.md
--rw-rw-rw-   0        0        0      649 2023-04-11 04:28:29.000000 luscioustwitch-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 04:28:45.870752 luscioustwitch-0.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 04:28:45.839751 luscioustwitch-0.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 04:28:45.860251 luscioustwitch-0.3.8/src/luscioustwitch/
--rw-rw-rw-   0        0        0       64 2023-03-23 03:59:45.000000 luscioustwitch-0.3.8/src/luscioustwitch/__init__.py
--rw-rw-rw-   0        0        0    18768 2023-04-11 04:28:23.000000 luscioustwitch-0.3.8/src/luscioustwitch/api.py
--rw-rw-rw-   0        0        0     7610 2023-03-24 01:09:26.000000 luscioustwitch-0.3.8/src/luscioustwitch/events.py
--rw-rw-rw-   0        0        0     5189 2023-04-02 22:11:33.000000 luscioustwitch-0.3.8/src/luscioustwitch/gql.py
--rw-rw-rw-   0        0        0      810 2023-03-26 21:25:10.000000 luscioustwitch-0.3.8/src/luscioustwitch/saferequests.py
--rw-rw-rw-   0        0        0     3859 2023-03-24 01:48:54.000000 luscioustwitch-0.3.8/src/luscioustwitch/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-11 04:28:45.869252 luscioustwitch-0.3.8/src/luscioustwitch.egg-info/
--rw-rw-rw-   0        0        0      618 2023-04-11 04:28:45.000000 luscioustwitch-0.3.8/src/luscioustwitch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-04-11 04:28:45.000000 luscioustwitch-0.3.8/src/luscioustwitch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 04:28:45.000000 luscioustwitch-0.3.8/src/luscioustwitch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 04:28:45.000000 luscioustwitch-0.3.8/src/luscioustwitch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 05:18:13.528901 luscioustwitch-0.3.9/
+-rw-rw-rw-   0        0        0    35823 2023-02-18 18:00:33.000000 luscioustwitch-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      618 2023-04-28 05:18:13.528401 luscioustwitch-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-03-08 02:46:28.000000 luscioustwitch-0.3.9/README.md
+-rw-rw-rw-   0        0        0      649 2023-04-28 05:18:01.000000 luscioustwitch-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 05:18:13.528901 luscioustwitch-0.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 05:18:13.486401 luscioustwitch-0.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 05:18:13.519901 luscioustwitch-0.3.9/src/luscioustwitch/
+-rw-rw-rw-   0        0        0       64 2023-03-23 03:59:45.000000 luscioustwitch-0.3.9/src/luscioustwitch/__init__.py
+-rw-rw-rw-   0        0        0    18933 2023-04-28 05:17:47.000000 luscioustwitch-0.3.9/src/luscioustwitch/api.py
+-rw-rw-rw-   0        0        0     7610 2023-03-24 01:09:26.000000 luscioustwitch-0.3.9/src/luscioustwitch/events.py
+-rw-rw-rw-   0        0        0     5189 2023-04-02 22:11:33.000000 luscioustwitch-0.3.9/src/luscioustwitch/gql.py
+-rw-rw-rw-   0        0        0      810 2023-03-26 21:25:10.000000 luscioustwitch-0.3.9/src/luscioustwitch/saferequests.py
+-rw-rw-rw-   0        0        0     3859 2023-03-24 01:48:54.000000 luscioustwitch-0.3.9/src/luscioustwitch/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:18:13.527901 luscioustwitch-0.3.9/src/luscioustwitch.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-04-28 05:18:13.000000 luscioustwitch-0.3.9/src/luscioustwitch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-04-28 05:18:13.000000 luscioustwitch-0.3.9/src/luscioustwitch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 05:18:13.000000 luscioustwitch-0.3.9/src/luscioustwitch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 05:18:13.000000 luscioustwitch-0.3.9/src/luscioustwitch.egg-info/top_level.txt
```

### Comparing `luscioustwitch-0.3.8/LICENSE` & `luscioustwitch-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `luscioustwitch-0.3.8/PKG-INFO` & `luscioustwitch-0.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luscioustwitch
-Version: 0.3.8
+Version: 0.3.9
 Summary: Twitch API Wrapper
 Author-email: Charlie Coleman <me@charlie-coleman.com>
 Project-URL: Homepage, https://github.com/charlie-coleman/luscioustwitch
 Project-URL: Bug Tracker, https://github.com/charlie-coleman/luscioustwitch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `luscioustwitch-0.3.8/pyproject.toml` & `luscioustwitch-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "luscioustwitch"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="Charlie Coleman", email="me@charlie-coleman.com" },
 ]
 description = "Twitch API Wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch/api.py` & `luscioustwitch-0.3.9/src/luscioustwitch/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,24 +145,29 @@
     r : requests.Response = self.rlrequests.get(url = url, headers = self.DEFAULT_HEADERS)
     
     if r.status_code == 200:
       return r.json()['data'][0]
     else:
       self.__raise_req_error(r)
       
-  def get_category_info(self, category_name : str) -> dict:
+  def get_category_info(self, category_specifier : str, is_name = True) -> dict:
     """Get category information from category name
 
     Args:
         category_name (string): Category name
+        category_id (str): Category ID
 
     Returns:
         dict: Category information
     """
-    url = f"{self.API_URL}/games?name={category_name}"
+    if is_name:
+      url = f"{self.API_URL}/games?name={category_specifier}"
+    else:
+      url = f"{self.API_URL}/games?id={category_specifier}"
+      
     r : requests.Response = self.rlrequests.get(url = url, headers = self.DEFAULT_HEADERS)
     
     if r.status_code == 200:
       return r.json()["data"][0]
     else:
       self.__raise_req_error(r)
```

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch/events.py` & `luscioustwitch-0.3.9/src/luscioustwitch/events.py`

 * *Files identical despite different names*

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch/gql.py` & `luscioustwitch-0.3.9/src/luscioustwitch/gql.py`

 * *Files identical despite different names*

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch/saferequests.py` & `luscioustwitch-0.3.9/src/luscioustwitch/saferequests.py`

 * *Files identical despite different names*

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch/websocket.py` & `luscioustwitch-0.3.9/src/luscioustwitch/websocket.py`

 * *Files identical despite different names*

### Comparing `luscioustwitch-0.3.8/src/luscioustwitch.egg-info/PKG-INFO` & `luscioustwitch-0.3.9/src/luscioustwitch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luscioustwitch
-Version: 0.3.8
+Version: 0.3.9
 Summary: Twitch API Wrapper
 Author-email: Charlie Coleman <me@charlie-coleman.com>
 Project-URL: Homepage, https://github.com/charlie-coleman/luscioustwitch
 Project-URL: Bug Tracker, https://github.com/charlie-coleman/luscioustwitch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

