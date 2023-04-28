# Comparing `tmp/behave_odoo-0.1.0.tar.gz` & `tmp/behave_odoo-14.0.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave_odoo-0.1.0.tar", last modified: Thu Apr 27 23:18:54 2023, max compression
+gzip compressed data, was "behave_odoo-14.0.1.0.0.tar", last modified: Fri Apr 28 00:37:46 2023, max compression
```

## Comparing `behave_odoo-0.1.0.tar` & `behave_odoo-14.0.1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:18:54.933476 behave_odoo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-04-27 23:18:41.000000 behave_odoo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-27 23:18:54.933476 behave_odoo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-27 23:18:41.000000 behave_odoo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:18:54.933476 behave_odoo-0.1.0/behave_odoo/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-27 23:18:41.000000 behave_odoo-0.1.0/behave_odoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-27 23:18:41.000000 behave_odoo-0.1.0/behave_odoo/behave_odoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:18:54.933476 behave_odoo-0.1.0/behave_odoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-27 23:18:54.000000 behave_odoo-0.1.0/behave_odoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-27 23:18:54.000000 behave_odoo-0.1.0/behave_odoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:18:54.000000 behave_odoo-0.1.0/behave_odoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 23:18:54.000000 behave_odoo-0.1.0/behave_odoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 23:18:54.000000 behave_odoo-0.1.0/behave_odoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:18:54.933476 behave_odoo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 23:18:41.000000 behave_odoo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:46.740896 behave_odoo-14.0.1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-04-28 00:37:28.000000 behave_odoo-14.0.1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-28 00:37:46.740896 behave_odoo-14.0.1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-28 00:37:28.000000 behave_odoo-14.0.1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:46.736896 behave_odoo-14.0.1.0.0/behave_odoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 00:37:28.000000 behave_odoo-14.0.1.0.0/behave_odoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-28 00:37:28.000000 behave_odoo-14.0.1.0.0/behave_odoo/behave_odoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:37:46.740896 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-28 00:37:46.000000 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 00:37:46.000000 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:37:46.000000 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 00:37:46.000000 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 00:37:46.000000 behave_odoo-14.0.1.0.0/behave_odoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:37:46.740896 behave_odoo-14.0.1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-28 00:37:28.000000 behave_odoo-14.0.1.0.0/setup.py
```

### Comparing `behave_odoo-0.1.0/LICENSE` & `behave_odoo-14.0.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `behave_odoo-0.1.0/PKG-INFO` & `behave_odoo-14.0.1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: behave_odoo
-Version: 0.1.0
+Version: 14.0.1.0.0
 Summary: Helper functions for simplifying the process of writing behave tests for Odoo
 Home-page: https://github.com/coopdevs/behave_odoo
 Author: Coopdevs
 Author-email: pelayo.garcia@coopdevs.org
 License: AGPLv3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Odoo
+Classifier: Framework :: Odoo :: 14.0
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: Software Development :: Testing :: BDD
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `behave_odoo`
 
-behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo applications. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
+behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo 14. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
 
 ## Installation
 
-To install behave_odoo, use pip:
+To install behave_odoo, use [pip](https://pypi.org/project/behave-odoo/):
 
 ```shell
-pip install behave_odoo
+pip install behave-odoo
 ```
 
 ## Usage
 
 To use the behave_odoo in your project, simply import the functions you need:
 
 ```python
```

### Comparing `behave_odoo-0.1.0/README.md` & `behave_odoo-14.0.1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # `behave_odoo`
 
-behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo applications. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
+behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo 14. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
 
 ## Installation
 
-To install behave_odoo, use pip:
+To install behave_odoo, use [pip](https://pypi.org/project/behave-odoo/):
 
 ```shell
-pip install behave_odoo
+pip install behave-odoo
 ```
 
 ## Usage
 
 To use the behave_odoo in your project, simply import the functions you need:
 
 ```python
```

### Comparing `behave_odoo-0.1.0/behave_odoo/__init__.py` & `behave_odoo-14.0.1.0.0/behave_odoo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-`behave_odoo` is a Python package that provides a collection of helper functions designed to simplify the process of writing behave tests for Odoo applications. 
+`behave_odoo` is a Python package that provides a collection of helper functions designed to simplify the process of writing behave tests for Odoo 14. 
 
 The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
 
 
 ```python
 import behave_odoo as bodoo
```

### Comparing `behave_odoo-0.1.0/behave_odoo/behave_odoo.py` & `behave_odoo-14.0.1.0.0/behave_odoo/behave_odoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-`behave_odoo` is a Python package that provides a collection of helper functions designed to simplify the process of writing behave tests for Odoo applications. 
+`behave_odoo` is a Python package that provides a collection of helper functions designed to simplify the process of writing behave tests for Odoo 14. 
 
 The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
 
 
 ```python
 import behave_odoo as bodoo
```

### Comparing `behave_odoo-0.1.0/behave_odoo.egg-info/PKG-INFO` & `behave_odoo-14.0.1.0.0/behave_odoo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: behave-odoo
-Version: 0.1.0
+Version: 14.0.1.0.0
 Summary: Helper functions for simplifying the process of writing behave tests for Odoo
 Home-page: https://github.com/coopdevs/behave_odoo
 Author: Coopdevs
 Author-email: pelayo.garcia@coopdevs.org
 License: AGPLv3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Odoo
+Classifier: Framework :: Odoo :: 14.0
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: Software Development :: Testing :: BDD
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `behave_odoo`
 
-behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo applications. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
+behave_odoo is a Python package that provides a collection of helper functions designed to simplify the process of writing [behave](https://github.com/behave) tests for Odoo 14. The package includes functions for navigating the Odoo interface, interacting with form fields, and performing common actions within the Odoo environment.
 
 ## Installation
 
-To install behave_odoo, use pip:
+To install behave_odoo, use [pip](https://pypi.org/project/behave-odoo/):
 
 ```shell
-pip install behave_odoo
+pip install behave-odoo
 ```
 
 ## Usage
 
 To use the behave_odoo in your project, simply import the functions you need:
 
 ```python
```

