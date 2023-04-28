# Comparing `tmp/searchcode-0.0.1.tar.gz` & `tmp/searchcode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchcode-0.0.1.tar", last modified: Fri Apr 28 13:50:28 2023, max compression
+gzip compressed data, was "searchcode-0.0.2.tar", last modified: Fri Apr 28 18:40:33 2023, max compression
```

## Comparing `searchcode-0.0.1.tar` & `searchcode-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:50:28.332752 searchcode-0.0.1/
--rw-rw-rw-   0        0        0     1147 2023-04-28 13:50:28.332752 searchcode-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-28 13:38:18.000000 searchcode-0.0.1/README.md
--rw-rw-rw-   0        0        0      981 2023-04-28 13:44:47.000000 searchcode-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-28 13:50:28.332752 searchcode-0.0.1/searchcode.egg-info/
--rw-rw-rw-   0        0        0     1147 2023-04-28 13:50:28.000000 searchcode-0.0.1/searchcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-04-28 13:50:28.000000 searchcode-0.0.1/searchcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:50:28.000000 searchcode-0.0.1/searchcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-28 13:50:28.000000 searchcode-0.0.1/searchcode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:50:28.000000 searchcode-0.0.1/searchcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 13:50:28.332752 searchcode-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 18:40:33.767254 searchcode-0.0.2/
+-rw-rw-rw-   0        0        0     1123 2023-04-28 18:40:33.767254 searchcode-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-04-28 18:38:57.000000 searchcode-0.0.2/README.md
+-rw-rw-rw-   0        0        0      816 2023-04-28 18:40:11.000000 searchcode-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-28 18:40:33.767254 searchcode-0.0.2/searchcode.egg-info/
+-rw-rw-rw-   0        0        0     1123 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 18:40:33.000000 searchcode-0.0.2/searchcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 18:40:33.767254 searchcode-0.0.2/setup.cfg
```

### Comparing `searchcode-0.0.1/PKG-INFO` & `searchcode-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: searchcode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dummy package for the SearchCode API wrapper (searchcode-cli)
 Author-email: Richard Mwewa <rly0nheart@duck.com>
-Project-URL: homepage, https://github.com/rly0nheart/searchcode-cli
-Project-URL: documentation, https://github.com/rly0nheart/searchcode-cli/wiki
-Project-URL: repository, https://github.com/rly0nheart/searchcode-cli.git
+Project-URL: homepage, https://pypi.python.org/pypi/searchcode-cli
 Keywords: searchcode,search-engine,codesearch,api-wrapper
 Classifier: Development Status :: 7 - Inactive
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: 
 Description-Content-Type: text/markdown
 
+![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
+
 This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is searchcode-cli. This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
```

### Comparing `searchcode-0.0.1/pyproject.toml` & `searchcode-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "searchcode"
-version = "0.0.1"
+version = "0.0.2"
 description = "Dummy package for the SearchCode API wrapper (searchcode-cli)"
 readme = "README.md"
-license = {file = "LICENSE"}
 keywords = ["searchcode", "search-engine", "codesearch", "api-wrapper"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
   "Development Status :: 7 - Inactive",
   "Programming Language :: Python :: 3",
   "Intended Audience :: Information Technology",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Natural Language :: English",
   ""
 ]
 dependencies = ["searchcode-cli"]
 
 [project.urls]
-homepage = "https://github.com/rly0nheart/searchcode-cli"
-documentation = "https://github.com/rly0nheart/searchcode-cli/wiki"
-repository = "https://github.com/rly0nheart/searchcode-cli.git"
+homepage = "https://pypi.python.org/pypi/searchcode-cli"
```

### Comparing `searchcode-0.0.1/searchcode.egg-info/PKG-INFO` & `searchcode-0.0.2/searchcode.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: searchcode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dummy package for the SearchCode API wrapper (searchcode-cli)
 Author-email: Richard Mwewa <rly0nheart@duck.com>
-Project-URL: homepage, https://github.com/rly0nheart/searchcode-cli
-Project-URL: documentation, https://github.com/rly0nheart/searchcode-cli/wiki
-Project-URL: repository, https://github.com/rly0nheart/searchcode-cli.git
+Project-URL: homepage, https://pypi.python.org/pypi/searchcode-cli
 Keywords: searchcode,search-engine,codesearch,api-wrapper
 Classifier: Development Status :: 7 - Inactive
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: 
 Description-Content-Type: text/markdown
 
+![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
+
 This is a dummy package managed by the developer of the SearchCode API wrapper to prevent name squatting. The official name of PyPI’s SearchCode API wrapper Python package is searchcode-cli. This package ensures that if you type `pip install searchcode` by mistake you will end up with `searchcode-cli`.
```

