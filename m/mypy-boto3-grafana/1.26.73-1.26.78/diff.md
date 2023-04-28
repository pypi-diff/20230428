# Comparing `tmp/mypy-boto3-grafana-1.26.73.tar.gz` & `tmp/mypy-boto3-grafana-1.26.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-grafana-1.26.73.tar", last modified: Thu Feb 16 20:47:25 2023, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
```

## Comparing `mypy-boto3-grafana-1.26.73.tar` & `mypy-boto3-grafana-1.26.78.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.487046 mypy-boto3-grafana-1.26.73/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-02-16 20:47:25.487046 mypy-boto3-grafana-1.26.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.475045 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-02-16 20:47:07.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-02-16 20:47:06.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:47:25.487046 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-16 20:47:25.000000 mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:47:25.487046 mypy-boto3-grafana-1.26.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-16 20:47:05.000000 mypy-boto3-grafana-1.26.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.332421 mypy-boto3-grafana-1.26.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-02-23 20:34:57.328421 mypy-boto3-grafana-1.26.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.324421 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16829 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-02-23 20:34:28.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-02-23 20:34:28.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-02-23 20:34:28.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.328421 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 20:34:57.000000 mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.332421 mypy-boto3-grafana-1.26.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-23 20:34:27.000000 mypy-boto3-grafana-1.26.78/setup.py
```

### Comparing `mypy-boto3-grafana-1.26.73/LICENSE` & `mypy-boto3-grafana-1.26.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/PKG-INFO` & `mypy-boto3-grafana-1.26.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.26.73
-Summary: Type annotations for boto3.ManagedGrafana 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.ManagedGrafana 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.26.73/README.md` & `mypy-boto3-grafana-1.26.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__init__.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__init__.pyi` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.26.73\nVersion:         1.26.73\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.ManagedGrafana 1.26.78\nVersion:         1.26.78\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.73")
+    print("1.26.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -395,14 +395,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/paginator.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.26.73
-Summary: Type annotations for boto3.ManagedGrafana 1.26.73 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.ManagedGrafana 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.26.73](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-grafana-1.26.73/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.26.78/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.26.73/setup.py` & `mypy-boto3-grafana-1.26.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.26.73",
+    version="1.26.78",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedGrafana 1.26.73 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.ManagedGrafana 1.26.78 service generated with"
+        " mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

