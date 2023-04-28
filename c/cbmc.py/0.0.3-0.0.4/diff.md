# Comparing `tmp/cbmc.py-0.0.3.tar.gz` & `tmp/cbmc.py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmc.py-0.0.3.tar", last modified: Mon Apr 24 20:33:02 2023, max compression
+gzip compressed data, was "cbmc.py-0.0.4.tar", last modified: Fri Apr 28 18:48:49 2023, max compression
```

## Comparing `cbmc.py-0.0.3.tar` & `cbmc.py-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/cbmc/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/cbmc/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/cbmc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 20:33:02.000000 cbmc.py-0.0.3/cbmc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:33:02.429066 cbmc.py-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-24 20:32:51.000000 cbmc.py-0.0.3/tests/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:48:49.615342 cbmc.py-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-28 18:48:49.615342 cbmc.py-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:48:49.611342 cbmc.py-0.0.4/cbmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/cbmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/cbmc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/cbmc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/cbmc/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:48:49.611342 cbmc.py-0.0.4/cbmc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-28 18:48:49.000000 cbmc.py-0.0.4/cbmc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 18:48:49.000000 cbmc.py-0.0.4/cbmc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:48:49.000000 cbmc.py-0.0.4/cbmc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 18:48:49.000000 cbmc.py-0.0.4/cbmc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 18:48:49.000000 cbmc.py-0.0.4/cbmc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:48:49.615342 cbmc.py-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:48:49.615342 cbmc.py-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-28 18:48:37.000000 cbmc.py-0.0.4/tests/test_post.py
```

### Comparing `cbmc.py-0.0.3/LICENSE` & `cbmc.py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.3/PKG-INFO` & `cbmc.py-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: An unofficial 麥塊匿名發文平台 API wrapper.
 Home-page: https://github.com/ItsRqtl/cbmc.py
 Author: ItsRqtl
 Author-email: itsrql@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,16 @@
 
 # cbmc.py
 
 <!-- Add a badge here -->
 
 [![Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen)](https://pypi.org/project/cbmc.py/)
 [![CodeFactor](https://www.codefactor.io/repository/github/itsrqtl/cbmc.py/badge)](https://www.codefactor.io/repository/github/itsrqtl/cbmc.py)
+![GitHub issues](https://img.shields.io/github/issues/itsrqtl/cbmc.py)
+![GitHub pull requests](https://img.shields.io/github/issues-pr/itsrqtl/cbmc.py)
 
 [![PyPI](https://img.shields.io/pypi/v/cbmc.py)](https://pypi.org/project/cbmc.py/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbmc.py)](https://pypi.org/project/cbmc.py/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cbmc.py)](https://pypi.org/project/cbmc.py/)
 
 Unofficial 麥塊匿名發文平台 API Wrapper for Python
 
@@ -36,18 +38,39 @@
 
 ## Usage
 
 ```py
 # Import the library
 from cbmc import AsyncCbmc, SyncCbmc
 
+api = SyncCbmc()
+
 # Obtain post with post id, raise cbmc.NotFound if not found
-SyncCbmc.get_post(1)
+api.get_post(1)
 
 # List recent posts, maximum 300 posts.
-SyncCbmc.get_posts()
+api.get_posts()
+
+# Directly call the method also works
+# Creating an instance is not required, but it is recommended for future updates.
+# (some planned new features will require that)
+SyncCbmc.get_post(1)
 
 # Also available in async
 async def main():
     await AsyncCbmc.get_post(1)
     await AsyncCbmc.get_posts()
 ```
+
+## Documentation
+
+* [Documentation](docs/DOCS.md)
+* [Changelog](CHANGELOG.md)
+
+## Credits
+
+* 麥塊匿名發文平台 API Documents: [CBMC API Docs](https://api.cbmc.club/docs/)
+* Inspired by [HansHans135](https://github.com/hanshans135)'s [cbmc](https://github.com/HansHans135/cbmc) library.
+
+## License
+
+This project is licensed under `MIT License`. See the [LICENSE](LICENSE) for more details.
```

### Comparing `cbmc.py-0.0.3/cbmc/api.py` & `cbmc.py-0.0.4/cbmc/api.py`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.3/cbmc/exception.py` & `cbmc.py-0.0.4/cbmc/exception.py`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.3/cbmc/post.py` & `cbmc.py-0.0.4/cbmc/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,14 +38,35 @@
 
     def __init__(self, data: dict) -> None:
         """
         Initialize the post.
 
         :param data: The data of the post.
         :type data: dict
+
+        :ivar post_id: The post ID of the post.
+        :vartype post_id: int
+        :ivar platform_id: The platform ID of the post.
+        :vartype platform_id: int
+        :ivar type: The post type of the post.
+        :vartype type: str
+        :ivar content: The content of the post.
+        :vartype content: str
+        :ivar photo: The photo url of the post.
+        :vartype photo: str | None
+        :ivar admin_post: Whether the post is an admin post.
+        :vartype admin_post: bool
+        :ivar approve_timestamp: The timestamp of when the post was approved.
+        :vartype approve_timestamp: int | None
+        :ivar approve_time: The time of when the post was approved.
+        :vartype approve_time: datetime.datetime | None
+        :ivar approve_user: The user who approved the post.
+        :vartype approve_user: str | None
+        :ivar fbid: The Facebook ID of the post.
+        :vartype fbid: str | None
         """
         self._post_id = data.get("id", {}).get("post")
         self._platform_id = data.get("id", {}).get("platform")
         self._type = data.get("type")
         self._content = data.get("content")
         self._photo = data.get("photo")
         self._admin_post = data.get("adminPost")
```

### Comparing `cbmc.py-0.0.3/cbmc.py.egg-info/PKG-INFO` & `cbmc.py-0.0.4/cbmc.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbmc.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: An unofficial 麥塊匿名發文平台 API wrapper.
 Home-page: https://github.com/ItsRqtl/cbmc.py
 Author: ItsRqtl
 Author-email: itsrql@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,16 @@
 
 # cbmc.py
 
 <!-- Add a badge here -->
 
 [![Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen)](https://pypi.org/project/cbmc.py/)
 [![CodeFactor](https://www.codefactor.io/repository/github/itsrqtl/cbmc.py/badge)](https://www.codefactor.io/repository/github/itsrqtl/cbmc.py)
+![GitHub issues](https://img.shields.io/github/issues/itsrqtl/cbmc.py)
+![GitHub pull requests](https://img.shields.io/github/issues-pr/itsrqtl/cbmc.py)
 
 [![PyPI](https://img.shields.io/pypi/v/cbmc.py)](https://pypi.org/project/cbmc.py/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbmc.py)](https://pypi.org/project/cbmc.py/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/cbmc.py)](https://pypi.org/project/cbmc.py/)
 
 Unofficial 麥塊匿名發文平台 API Wrapper for Python
 
@@ -36,18 +38,39 @@
 
 ## Usage
 
 ```py
 # Import the library
 from cbmc import AsyncCbmc, SyncCbmc
 
+api = SyncCbmc()
+
 # Obtain post with post id, raise cbmc.NotFound if not found
-SyncCbmc.get_post(1)
+api.get_post(1)
 
 # List recent posts, maximum 300 posts.
-SyncCbmc.get_posts()
+api.get_posts()
+
+# Directly call the method also works
+# Creating an instance is not required, but it is recommended for future updates.
+# (some planned new features will require that)
+SyncCbmc.get_post(1)
 
 # Also available in async
 async def main():
     await AsyncCbmc.get_post(1)
     await AsyncCbmc.get_posts()
 ```
+
+## Documentation
+
+* [Documentation](docs/DOCS.md)
+* [Changelog](CHANGELOG.md)
+
+## Credits
+
+* 麥塊匿名發文平台 API Documents: [CBMC API Docs](https://api.cbmc.club/docs/)
+* Inspired by [HansHans135](https://github.com/hanshans135)'s [cbmc](https://github.com/HansHans135/cbmc) library.
+
+## License
+
+This project is licensed under `MIT License`. See the [LICENSE](LICENSE) for more details.
```

### Comparing `cbmc.py-0.0.3/setup.py` & `cbmc.py-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 setup(
     name="cbmc.py",
     version=VERSION,
     author="ItsRqtl",
     author_email="itsrql@gmail.com",
     description="An unofficial 麥塊匿名發文平台 API wrapper.",
```

### Comparing `cbmc.py-0.0.3/tests/test_api.py` & `cbmc.py-0.0.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cbmc.py-0.0.3/tests/test_post.py` & `cbmc.py-0.0.4/tests/test_post.py`

 * *Files identical despite different names*

