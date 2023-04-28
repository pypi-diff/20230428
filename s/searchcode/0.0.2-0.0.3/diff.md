# Comparing `tmp/searchcode-0.0.2.tar.gz` & `tmp/searchcode-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchcode-0.0.2.tar", last modified: Fri Apr 28 18:40:33 2023, max compression
+gzip compressed data, was "searchcode-0.0.3.tar", last modified: Fri Apr 28 18:47:52 2023, max compression
```

## Comparing `searchcode-0.0.2.tar` & `searchcode-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:40:33.767254 searchcode-0.0.2/
--rw-rw-rw-   0        0        0     1123 2023-04-28 18:40:33.767254 searchcode-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-04-28 18:38:57.000000 searchcode-0.0.2/README.md
--rw-rw-rw-   0        0        0      816 2023-04-28 18:40:11.000000 searchcode-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-28 18:40:33.767254 searchcode-0.0.2/searchcode.egg-info/
--rw-rw-rw-   0        0        0     1123 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 18:40:33.767254 searchcode-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 18:47:52.475041 searchcode-0.0.3/
+-rw-rw-rw-   0        0        0     1170 2023-04-28 18:47:52.475041 searchcode-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-28 18:47:08.000000 searchcode-0.0.3/README.md
+-rw-rw-rw-   0        0        0      816 2023-04-28 18:47:28.000000 searchcode-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-28 18:47:52.475041 searchcode-0.0.3/searchcode.egg-info/
+-rw-rw-rw-   0        0        0     1170 2023-04-28 18:47:52.000000 searchcode-0.0.3/searchcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-28 18:47:52.000000 searchcode-0.0.3/searchcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:47:52.000000 searchcode-0.0.3/searchcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 18:47:52.000000 searchcode-0.0.3/searchcode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:47:52.000000 searchcode-0.0.3/searchcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:47:52.475041 searchcode-0.0.3/setup.cfg
```

### Comparing `searchcode-0.0.2/PKG-INFO` & `searchcode-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dummy package for the SearchCode API wrapper (searchcode-cli)
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 Project-URL: homepage, https://pypi.python.org/pypi/searchcode-cli
 Keywords: searchcode,search-engine,codesearch,api-wrapper
 Classifier: Development Status :: 7 - Inactive
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
@@ -12,8 +12,8 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: 
 Description-Content-Type: text/markdown
 
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
 
-This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is searchcode-cli. This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
+This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is [searchcode-cli](https://pypi.python.org/pypi/searchcode-cli). This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
```

### Comparing `searchcode-0.0.2/pyproject.toml` & `searchcode-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "searchcode"
-version = "0.0.2"
+version = "0.0.3"
 description = "Dummy package for the SearchCode API wrapper (searchcode-cli)"
 readme = "README.md"
 keywords = ["searchcode", "search-engine", "codesearch", "api-wrapper"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
   "Development Status :: 7 - Inactive",
   "Programming Language :: Python :: 3",
```

### Comparing `searchcode-0.0.2/searchcode.egg-info/PKG-INFO` & `searchcode-0.0.3/searchcode.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dummy package for the SearchCode API wrapper (searchcode-cli)
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 Project-URL: homepage, https://pypi.python.org/pypi/searchcode-cli
 Keywords: searchcode,search-engine,codesearch,api-wrapper
 Classifier: Development Status :: 7 - Inactive
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
@@ -12,8 +12,8 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: 
 Description-Content-Type: text/markdown
 
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
 
-This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is searchcode-cli. This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
+This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is [searchcode-cli](https://pypi.python.org/pypi/searchcode-cli). This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
```

