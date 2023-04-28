# Comparing `tmp/tantaroba-0.4.0.tar.gz` & `tmp/tantaroba-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tantaroba-0.4.0.tar", max compression
+gzip compressed data, was "tantaroba-0.4.1.tar", max compression
```

## Comparing `tantaroba-0.4.0.tar` & `tantaroba-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      900 2023-03-15 11:26:35.248634 tantaroba-0.4.0/LICENSE
--rw-r--r--   0        0        0      199 2023-03-15 11:26:35.248634 tantaroba-0.4.0/README.md
--rw-r--r--   0        0        0     1984 2023-03-15 11:26:35.249634 tantaroba-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 11:26:35.249634 tantaroba-0.4.0/tantaroba/__init__.py
--rw-r--r--   0        0        0       22 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/__version__.py
--rw-r--r--   0        0        0      499 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/dynamic_import.py
--rw-r--r--   0        0        0      641 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/iterator_helpers.py
--rw-r--r--   0        0        0      936 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/log.py
--rw-r--r--   0        0        0      683 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/profile.py
--rw-r--r--   0        0        0       88 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/scripts/script.py
--rw-r--r--   0        0        0      691 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/strings.py
--rw-r--r--   0        0        0      528 2023-03-15 11:26:35.250634 tantaroba-0.4.0/tantaroba/yaml.py
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 tantaroba-0.4.0/setup.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 tantaroba-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-04-28 10:08:47.277778 tantaroba-0.4.1/LICENSE
+-rw-r--r--   0        0        0      199 2023-04-28 10:08:47.277778 tantaroba-0.4.1/README.md
+-rw-r--r--   0        0        0     1985 2023-04-28 10:08:47.278778 tantaroba-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/__version__.py
+-rw-r--r--   0        0        0      499 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/dynamic_import.py
+-rw-r--r--   0        0        0      641 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/iterator_helpers.py
+-rw-r--r--   0        0        0      936 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/log.py
+-rw-r--r--   0        0        0      683 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/profile.py
+-rw-r--r--   0        0        0       88 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/scripts/script.py
+-rw-r--r--   0        0        0      691 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/strings.py
+-rw-r--r--   0        0        0      528 2023-04-28 10:08:47.278778 tantaroba-0.4.1/tantaroba/yaml.py
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 tantaroba-0.4.1/setup.py
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 tantaroba-0.4.1/PKG-INFO
```

### Comparing `tantaroba-0.4.0/LICENSE` & `tantaroba-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/pyproject.toml` & `tantaroba-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "tantaroba"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python package template"
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/tantardini/tantaroba"
 keywords = ["utils", "postgresql", "yaml"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
-pandas = "^1.5.3"
+pandas = ">=1.5.3"
 numpy = "^1.24.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 commitizen = "^2.35.0"
 python-semantic-release = "^7.32.1"
 pytest = "^7.1.3"
```

### Comparing `tantaroba-0.4.0/tantaroba/iterator_helpers.py` & `tantaroba-0.4.1/tantaroba/iterator_helpers.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/tantaroba/log.py` & `tantaroba-0.4.1/tantaroba/log.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/tantaroba/profile.py` & `tantaroba-0.4.1/tantaroba/profile.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/tantaroba/strings.py` & `tantaroba-0.4.1/tantaroba/strings.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/tantaroba/yaml.py` & `tantaroba-0.4.1/tantaroba/yaml.py`

 * *Files identical despite different names*

### Comparing `tantaroba-0.4.0/setup.py` & `tantaroba-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['tantaroba', 'tantaroba.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['loguru>=0.6.0,<0.7.0', 'numpy>=1.24.2,<2.0.0', 'pandas>=1.5.3,<2.0.0']
+['loguru>=0.6.0,<0.7.0', 'numpy>=1.24.2,<2.0.0', 'pandas>=1.5.3']
 
 setup_kwargs = {
     'name': 'tantaroba',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Python package template',
     'long_description': '# tantaroba\n\nCollection of miscellanoeus utilities commonly used across different projects.\n\n## Installation\n```\npip install tantaroba\n```\n\n## Usage\nDescribe how to launch and use tantaroba project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tantardini/tantaroba',
```

### Comparing `tantaroba-0.4.0/PKG-INFO` & `tantaroba-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tantaroba
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package template
 Home-page: https://gitlab.com/tantardini/tantaroba
 Keywords: utils,postgresql,yaml
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=1.5.3)
 Project-URL: Repository, https://gitlab.com/tantardini/tantaroba
 Description-Content-Type: text/markdown
 
 # tantaroba
 
 Collection of miscellanoeus utilities commonly used across different projects.
```

