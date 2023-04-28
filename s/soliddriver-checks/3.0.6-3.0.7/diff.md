# Comparing `tmp/soliddriver-checks-3.0.6.tar.gz` & `tmp/soliddriver-checks-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soliddriver-checks-3.0.6.tar", last modified: Fri Dec 30 08:32:16 2022, max compression
+gzip compressed data, was "soliddriver-checks-3.0.7.tar", last modified: Fri Apr 28 12:33:35 2023, max compression
```

## Comparing `soliddriver-checks-3.0.6.tar` & `soliddriver-checks-3.0.7.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.123486 soliddriver-checks-3.0.6/
--rw-r--r--   0 hzzhao     (501) staff       (20)    18091 2022-03-31 07:35:30.000000 soliddriver-checks-3.0.6/LICENSE
--rw-r--r--   0 hzzhao     (501) staff       (20)      111 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/MANIFEST.in
--rw-r--r--   0 hzzhao     (501) staff       (20)     4548 2022-12-30 08:32:16.123347 soliddriver-checks-3.0.6/PKG-INFO
--rw-r--r--   0 hzzhao     (501) staff       (20)     3974 2022-12-21 15:56:00.000000 soliddriver-checks-3.0.6/README.md
--rw-r--r--   0 hzzhao     (501) staff       (20)      107 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/pyproject.toml
--rw-r--r--   0 hzzhao     (501) staff       (20)       38 2022-12-30 08:32:16.123522 soliddriver-checks-3.0.6/setup.cfg
--rw-r--r--   0 hzzhao     (501) staff       (20)     1911 2022-12-29 12:49:50.000000 soliddriver-checks-3.0.6/setup.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.115752 soliddriver-checks-3.0.6/src/
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.117865 soliddriver-checks-3.0.6/src/soliddriver_checks/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-03 10:29:51.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/__init__.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.119523 soliddriver-checks-3.0.6/src/soliddriver_checks/api/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1265 2022-12-29 12:43:30.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/analysis.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     9354 2022-12-30 08:26:33.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/km.py
--rw-r--r--   0 hzzhao     (501) staff       (20)    16550 2022-12-30 08:24:22.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/kmp.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      830 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/raw_data.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.119903 soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1798 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/cmd.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.120130 soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/scripts/
--rwxr-xr-x   0 hzzhao     (501) staff       (20)      857 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/scripts/check-links.sh
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.121527 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     6280 2022-12-29 15:30:57.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/cli.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     6692 2022-12-30 08:16:03.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/km_report.py
--rw-r--r--   0 hzzhao     (501) staff       (20)    14435 2022-12-30 08:10:37.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/kmp_report.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      635 2022-12-29 07:54:18.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/terminal_logs.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     7748 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/cli/xlsx_utils.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.121934 soliddriver-checks-3.0.6/src/soliddriver_checks/config/
--rw-r--r--   0 hzzhao     (501) staff       (20)     6148 2022-12-13 07:54:42.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/.DS_Store
--rw-r--r--   0 hzzhao     (501) staff       (20)     5884 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/soliddriver-checks.conf
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.122700 soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/
--rw-r--r--   0 hzzhao     (501) staff       (20)     6148 2022-12-13 07:54:42.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/.DS_Store
--rw-r--r--   0 hzzhao     (501) staff       (20)     3431 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/km-report.html.jinja
--rw-r--r--   0 hzzhao     (501) staff       (20)     4675 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/kmp-report.html.jinja
--rw-r--r--   0 hzzhao     (501) staff       (20)    13833 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/templates.xlsx
--rw-r--r--   0 hzzhao     (501) staff       (20)     3820 2022-12-15 03:20:21.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/config.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.122936 soliddriver-checks-3.0.6/src/soliddriver_checks/service/
--rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-18 08:10:10.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/service/__init__.py
--rw-r--r--   0 hzzhao     (501) staff       (20)     1632 2022-12-29 07:00:32.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/service/service.py
--rw-r--r--   0 hzzhao     (501) staff       (20)      101 2022-12-30 08:29:15.000000 soliddriver-checks-3.0.6/src/soliddriver_checks/version.py
-drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2022-12-30 08:32:16.118655 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/
--rw-r--r--   0 hzzhao     (501) staff       (20)     4548 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/PKG-INFO
--rw-r--r--   0 hzzhao     (501) staff       (20)     1404 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/SOURCES.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)        1 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/dependency_links.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)      149 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/entry_points.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)      139 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/requires.txt
--rw-r--r--   0 hzzhao     (501) staff       (20)       19 2022-12-30 08:32:16.000000 soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/top_level.txt
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143916 soliddriver-checks-3.0.7/
+-rw-r--r--   0 hzzhao     (501) staff       (20)    18091 2022-03-31 07:35:30.000000 soliddriver-checks-3.0.7/LICENSE
+-rw-r--r--   0 hzzhao     (501) staff       (20)      111 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/MANIFEST.in
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-04-28 12:33:35.143803 soliddriver-checks-3.0.7/PKG-INFO
+-rw-r--r--   0 hzzhao     (501) staff       (20)     4600 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/README.md
+-rw-r--r--   0 hzzhao     (501) staff       (20)      107 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/pyproject.toml
+-rw-r--r--   0 hzzhao     (501) staff       (20)       38 2023-04-28 12:33:35.143947 soliddriver-checks-3.0.7/setup.cfg
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1913 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/setup.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.139144 soliddriver-checks-3.0.7/src/
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.140586 soliddriver-checks-3.0.7/src/soliddriver_checks/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-03 10:29:51.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/__init__.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142042 soliddriver-checks-3.0.7/src/soliddriver_checks/api/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1505 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/analysis.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     9111 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/filter.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     9805 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/km.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)    16773 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/kmp.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      832 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/raw_data.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142259 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1795 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/cmd.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142365 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/
+-rwxr-xr-x   0 hzzhao     (501) staff       (20)      857 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/check-links.sh
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.142999 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-15 01:11:40.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     6407 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/cli.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     6932 2023-02-14 10:22:24.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/km_report.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)    15074 2022-12-30 09:00:29.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/kmp_report.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      611 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/terminal_logs.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     7835 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/cli/xlsx_utils.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143108 soliddriver-checks-3.0.7/src/soliddriver_checks/config/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5884 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/soliddriver-checks.conf
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143453 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     3431 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/km-report.html.jinja
+-rw-r--r--   0 hzzhao     (501) staff       (20)     4675 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/kmp-report.html.jinja
+-rw-r--r--   0 hzzhao     (501) staff       (20)    13833 2022-12-15 01:11:41.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/templates.xlsx
+-rw-r--r--   0 hzzhao     (501) staff       (20)     3720 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/config.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.143652 soliddriver-checks-3.0.7/src/soliddriver_checks/service/
+-rw-r--r--   0 hzzhao     (501) staff       (20)        0 2022-12-18 08:10:10.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/service/__init__.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1646 2022-12-30 08:54:30.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/service/service.py
+-rw-r--r--   0 hzzhao     (501) staff       (20)      101 2023-04-28 12:30:59.000000 soliddriver-checks-3.0.7/src/soliddriver_checks/version.py
+drwxr-xr-x   0 hzzhao     (501) staff       (20)        0 2023-04-28 12:33:35.141371 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/
+-rw-r--r--   0 hzzhao     (501) staff       (20)     5174 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/PKG-INFO
+-rw-r--r--   0 hzzhao     (501) staff       (20)     1351 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/SOURCES.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)        1 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/dependency_links.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)      149 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/entry_points.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)      139 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/requires.txt
+-rw-r--r--   0 hzzhao     (501) staff       (20)       19 2023-04-28 12:33:35.000000 soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/top_level.txt
```

### Comparing `soliddriver-checks-3.0.6/LICENSE` & `soliddriver-checks-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/setup.py` & `soliddriver-checks-3.0.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os.path
 
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+    with codecs.open(os.path.join(here, rel_path), "r") as fp:
         return fp.read()
 
 
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
-        if line.startswith('__VERSION__'):
+        if line.startswith("__VERSION__"):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
@@ -40,24 +40,24 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     include_package_data=True,
     python_requires=">=3.7",
     install_requires=[
-        'bottle>=0.12.23',
-        'click>=8.1.3',
-        'dominate>=2.7.0',
-        'Jinja2>=3.1.2',
-        'openpyxl>=3.0.10',
-        'pandas>=1.5.2',
-        'rich>=12.6.0',
-        'setuptools>=65.4.1',
-        'requests>=2.28.1'
+        "bottle>=0.12.23",
+        "click>=8.1.3",
+        "dominate>=2.7.0",
+        "Jinja2>=3.1.2",
+        "openpyxl>=3.0.10",
+        "pandas>=1.5.2",
+        "rich>=12.6.0",
+        "setuptools>=65.4.1",
+        "requests>=2.28.1",
     ],
     entry_points={
-        'console_scripts': [
-            'soliddriver-checks=soliddriver_checks.cli.cli:run',
-            'soliddriver-checks-service=soliddriver_checks.service.service:run_as_service'
+        "console_scripts": [
+            "soliddriver-checks=soliddriver_checks.cli.cli:run",
+            "soliddriver-checks-service=soliddriver_checks.service.service:run_as_service",
         ]
     },
 )
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/analysis.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .kmp import KMPReader, KMPAnalysis, analysis_kmps_to_dataframe
 from .km import KMReader, KMAnalysis
+from .filter import km_filter
 
 
 def kmps_to_dataframe(path, proc_injector=None):
     reader = KMPReader()
     anls = KMPAnalysis()
     kmps = reader.get_all_kmp_files(path)
     if proc_injector is not None:
@@ -34,19 +35,26 @@
 
 def kmps_to_json(path, proc_injector=None):
     df = kmps_to_dataframe(path, proc_injector)
 
     return df.to_json(orient="records")
 
 
-def kms_to_dataframe():
+def kms_to_dataframe(filter=None):
     reader = KMReader()
     anls = KMAnalysis()
+    df = anls.kms_analysis(reader.get_all_modinfo())
 
-    return anls.kms_analysis(reader.get_all_modinfo())
+    if filter is None:
+        return df
+    else:
+        return km_filter(filter, df)
 
 
-def kms_to_json(df=None):
+def kms_to_json(df=None, filter=None):
     if df is None:
         df = kms_to_dataframe()
 
-    return df.to_json(orient="records")
+    if filter is None:
+        return df.to_json(orient="records")
+    else:
+        return km_filter(filter, df).to_json(orient="records")
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/km.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/km.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,64 +4,79 @@
 from ..config import SDCConf
 from enum import Enum, unique
 from .utils.cmd import run_cmd
 import requests
 
 
 @unique
-class KMEvaluation (Enum):
+class KMEvaluation(Enum):
     PASS = 1
     WARNING = 2
     ERROR = 3
 
     def __str__(self):
         return self.name
 
     def __int__(self):
         return self.value
 
     def to_json(self):
-        return {'level': self.name, 'value': self.value}
+        return {"level": self.name, "value": self.value}
 
 
 class KMAnalysis:
     def __init__(self):
         conf = SDCConf()
         self._valid_licenses = conf.get_valid_licenses()
-        self._valid_licenses = [i.get('name', '') for i in self._valid_licenses]
+        self._valid_licenses = [i.get("name", "") for i in self._valid_licenses]
 
     def kms_analysis(self, kms):
         row_level = []
         df = pd.DataFrame()
         for filename in kms:
-            lev_name, name = self._km_module_name_analysis(kms[filename].get("name", ""))
-            row_level.append(lev_name['value'])
-            lev_fn, filename = self._km_filename_analysis(filename, kms[filename].get("weak-updates", 0))
-            row_level.append(lev_fn['value'])
-            lev_spd, supported = self._km_supported_analysis(kms[filename].get("supported", ""))
-            row_level.append(lev_spd['value'])
-            lev_lic, license = self._km_license_analysis(kms[filename].get("license", ""))
-            row_level.append(lev_lic['value'])
-            lev_sig, signature = self._km_signature_analysis(kms[filename].get("signature", ""))
-            row_level.append(lev_sig['value'])
+            lev_name, name = self._km_module_name_analysis(
+                kms[filename].get("name", "")
+            )
+            row_level.append(lev_name["value"])
+            lev_fn, filename = self._km_filename_analysis(
+                filename, kms[filename].get("weak-updates", 0)
+            )
+            row_level.append(lev_fn["value"])
+            lev_spd, supported = self._km_supported_analysis(
+                kms[filename].get("supported", "")
+            )
+            row_level.append(lev_spd["value"])
+            lev_lic, license = self._km_license_analysis(
+                kms[filename].get("license", "")
+            )
+            row_level.append(lev_lic["value"])
+            lev_sig, signature = self._km_signature_analysis(
+                kms[filename].get("signature", "")
+            )
+            row_level.append(lev_sig["value"])
             lev_r, running = self._km_running_analysis(kms[filename].get("running", ""))
-            row_level.append(lev_r['value'])
+            row_level.append(lev_r["value"])
             lev_kmp, kmp = self._km_kmp_analysis(kms[filename].get("kmp", None))
-            row_level.append(lev_kmp['value'])
+            row_level.append(lev_kmp["value"])
 
-            row = pd.Series({
-                             "level": KMEvaluation(max(row_level)).to_json(),
-                             "modulename": {"level": lev_name, "value": name},
-                             "filename": {"level": lev_fn, "value": filename},
-                             "license": {"level": lev_lic, "value": license},
-                             "signature": {"level": lev_sig, "value": signature},
-                             "supported": {"level": lev_spd, "value": " ".join(supported).strip()},
-                             "running": {"level": lev_r, "value": running},
-                             "kmp": {"level": lev_kmp, "value": kmp}
-                             })
+            row = pd.Series(
+                {
+                    "level": KMEvaluation(max(row_level)).to_json(),
+                    "modulename": {"level": lev_name, "value": name},
+                    "filename": {"level": lev_fn, "value": filename},
+                    "license": {"level": lev_lic, "value": license},
+                    "signature": {"level": lev_sig, "value": signature},
+                    "supported": {
+                        "level": lev_spd,
+                        "value": " ".join(supported).strip(),
+                    },
+                    "running": {"level": lev_r, "value": running},
+                    "kmp": {"level": lev_kmp, "value": kmp},
+                }
+            )
 
             df = pd.concat([df, row.to_frame().T], ignore_index=True)
 
         return df
 
     def _km_module_name_analysis(self, name):
         return KMEvaluation.PASS.to_json(), name
@@ -77,29 +92,34 @@
 
         return lev.to_json(), filename
 
     def _km_supported_analysis(self, supported):
         sps = supported.splitlines()
         lev = KMEvaluation.PASS
         # no supported flag or 1 supported flag but the value is not yes(supported by SUSE) or supported (supported by others).
-        if len(sps) == 0 or (len(sps) == 1 and sps[0] != "yes" and sps[0] != "no" and sps[0] != "external"):
+        if len(sps) == 0 or (
+            len(sps) == 1
+            and sps[0] != "yes"
+            and sps[0] != "no"
+            and sps[0] != "external"
+        ):
             lev = KMEvaluation.ERROR
         elif len(sps) > 1:
             lev = KMEvaluation.WARNING
             for v in sps:
                 if v != "yes" and v != "no" and v != "external":
                     lev = KMEvaluation.ERROR
                     break
 
         return lev.to_json(), sps
 
     def _km_license_analysis(self, license):
         lev = KMEvaluation.PASS
 
-        lics = license.split('\n')
+        lics = license.split("\n")
         for i in lics:
             if i not in self._valid_licenses:
                 lev = KMEvaluation.WARNING
                 break
 
         return lev.to_json(), license
 
@@ -110,15 +130,15 @@
             return KMEvaluation.WARNING.to_json(), "No"
 
     def _km_running_analysis(self, running):
         return KMEvaluation.PASS.to_json(), running
 
     def _km_kmp_analysis(self, kmp):
         if kmp is None:
-            return KMEvaluation.PASS.to_json(), {"name": "", "signature": ""} 
+            return KMEvaluation.PASS.to_json(), {"name": "", "signature": ""}
 
         name = kmp["name"]
         signature = kmp["signature"]
 
         if name.endswith("is not owned by any package"):
             return KMEvaluation.WARNING.to_json(), "Not owned by any package"
         elif signature == "":
@@ -133,35 +153,43 @@
         files_no = len(files)
         output = ""
         step = 300
         for i in range(0, files_no, step):
             curr_slip = step
             if i + step > files_no:
                 curr_slip = files_no - i
-            str_files = " ".join(files[i:i+curr_slip])
+            str_files = " ".join(files[i : i + curr_slip])
             output += run_cmd(cmd % str_files)
 
         return output
 
     def get_all_modinfo(self):
-        running_kms = run_cmd("/usr/sbin/modinfo $(cat /proc/modules | awk '{print $1}') | grep filename | awk '{print$2}'").splitlines()
+        running_kms = run_cmd(
+            "/usr/sbin/modinfo $(cat /proc/modules | awk '{print $1}') | grep filename | awk '{print$2}'"
+        ).splitlines()
         # Have to remove the invalid running kernel module, like it's running inside container.
         # But it always can't get rpm information if it's running inside container.
-        running_kms = [file for file in running_kms if not file.startswith("modinfo: ERROR:")]
-        lm_kms = run_cmd("find /lib/modules/ -regex \".*\.\(ko\|ko.xz\|ko.zst\)$\"").splitlines()
+        running_kms = [
+            file for file in running_kms if not file.startswith("modinfo: ERROR:")
+        ]
+        lm_kms = run_cmd(
+            'find /lib/modules/ -regex ".*\.\(ko\|ko.xz\|ko.zst\)$"'
+        ).splitlines()
 
         files = list(set(running_kms + lm_kms))
         # we don't need the entire signature, so add grep to ignore the details in other lines.
-        kms_info = self._split_cmd_args(files, '/usr/sbin/modinfo %s | grep -E "^([a-z]|[A-Z])" 2>&1')
+        kms_info = self._split_cmd_args(
+            files, '/usr/sbin/modinfo %s | grep -E "^([a-z]|[A-Z])" 2>&1'
+        )
         kms_info = kms_info.split("filename:")
         if len(kms_info) == 0:
             return {}
 
         kms = {}
-        kmps = self._split_cmd_args(files, 'rpm -qf %s')
+        kmps = self._split_cmd_args(files, "rpm -qf %s")
         kmps = kmps.splitlines()
         kmps_sig_pair = self._get_kmps_signature(kmps)
         # Here's something needs to be take care of if you split all the modinfo output by "filename",
         # If the kernel module is an invalid link, the output is:
         # modinfo: ERROR: Module invalid-link.ko not found.
         # If the kernel module is not a link but a broken kernel module, the output is:
         # filename:       /full/path/to/broken.ko
@@ -169,29 +197,36 @@
         # so if you want to match the KMP search index with the modinfo output index, you have to
         # take care of above. This is what I am doing.
         kmp_index = 0
         for km_info in kms_info[1:]:  # first one is empty.
             lines = km_info.splitlines()
             info = {}
             filename = lines[0].strip()
-            for line in lines[1:]:  # first line is filename, and filename is the key for info.
+            for line in lines[
+                1:
+            ]:  # first line is filename, and filename is the key for info.
                 vs = line.split(":")
                 k, v = vs[0].strip(), ":".join(vs[1:]).strip()
                 if "modinfo" == k:  # invalid kernel module found
                     if "not found." in v:  # invalid kernel module link found
-                        file = files[kmp_index]  # the full file path only can be found in files. The orders are the same.
+                        file = files[
+                            kmp_index
+                        ]  # the full file path only can be found in files. The orders are the same.
                         kmps[file]["rpm"] = {"name": kmps[kmp_index], "signature": ""}
                         kmp_index += 1
                 elif info.get(k, None) is not None:  # if already exist
                     info[k] = info[k] + "\n" + v
                 else:
                     info[k] = v
-            kms[filename]            = info
+            kms[filename] = info
             kms[filename]["running"] = filename in running_kms
-            kms[filename]["kmp"]     = {"name": kmps[kmp_index], "signature": kmps_sig_pair.get(kmps[kmp_index], "")}
+            kms[filename]["kmp"] = {
+                "name": kmps[kmp_index],
+                "signature": kmps_sig_pair.get(kmps[kmp_index], ""),
+            }
             kmp_index += 1
 
         self._check_weak_links(kms)
 
         return kms
 
     def _check_weak_links(self, kms):
@@ -209,15 +244,17 @@
         invalid_kmps = []
         for kmp in uniq_kmps:
             if kmp.endswith("is not owned by any package"):
                 invalid_kmps.append(kmp)
         for ik in invalid_kmps:
             uniq_kmps.remove(ik)
         # example: Signature   : RSA/SHA256, Wed 12 Oct 2022 06:57:49 PM CST, Key ID 70af9e8139db7c82
-        signatures = run_cmd(f'rpm -q --info {" ".join(uniq_kmps)} | grep -E "^Signature"').splitlines()
+        signatures = run_cmd(
+            f'rpm -q --info {" ".join(uniq_kmps)} | grep -E "^Signature"'
+        ).splitlines()
 
         kmp_sig_pairs = {}
         uniq_kmps = list(uniq_kmps)
         for i in range(0, len(uniq_kmps)):
             kmp_sig_pairs[uniq_kmps[i]] = signatures[i].split(":")[1:]
 
         return kmp_sig_pairs
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/kmp.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/kmp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,109 @@
-
 from pathlib import Path
 import pandas as pd
 import re
 from collections import namedtuple
 import tempfile
 import fnmatch
 from ..config import SDCConf
 from enum import Enum, unique
 from .utils.cmd import run_cmd
 
 
 def raw_kmp_to_series(data):
-    return pd.Series({
-        "name"            : data["name"],
-        "path"            : data["path"],
-        "vendor"          : data["vendor"],
-        "signature"       : data["signature"],
-        "license"         : data["license"],
-        "wm2_invoked"     : data["wm2_invoked"],
-        "km_info"         : data["km_info"]
-        })
+    return pd.Series(
+        {
+            "name": data["name"],
+            "path": data["path"],
+            "vendor": data["vendor"],
+            "signature": data["signature"],
+            "license": data["license"],
+            "wm2_invoked": data["wm2_invoked"],
+            "km_info": data["km_info"],
+        }
+    )
 
 
 def analysis_kmps_to_dataframe(data):
     df = pd.DataFrame()
 
     for item in data:
-        new_row = pd.Series({
-        "level"           : item["level"],
-        "name"            : item["name"],
-        "path"            : item["path"],
-        "vendor"          : item["vendor"],
-        "signature"       : item["signature"],
-        "license"         : item["license"],
-        "wm2_invoked"     : item["wm2_invoked"],
-        "supported_flag"  : item["km"]["supported"],
-        "km_signatures"   : item["km"]["signature"],
-        "km_licenses"     : item["km"]["license"],
-        "symbols"         : item["km"]["symbols"],
-        "modalias"        : item["km"]["alias"]
-        })
+        new_row = pd.Series(
+            {
+                "level": item["level"],
+                "name": item["name"],
+                "path": item["path"],
+                "vendor": item["vendor"],
+                "signature": item["signature"],
+                "license": item["license"],
+                "wm2_invoked": item["wm2_invoked"],
+                "supported_flag": item["km"]["supported"],
+                "km_signatures": item["km"]["signature"],
+                "km_licenses": item["km"]["license"],
+                "symbols": item["km"]["symbols"],
+                "modalias": item["km"]["alias"],
+            }
+        )
         df = pd.concat([df, new_row.to_frame().T], ignore_index=True)
 
     return df
 
 
 @unique
-class KMPEvaluation (Enum):
+class KMPEvaluation(Enum):
     PASS = 1
     WARNING = 2
     ERROR = 3
 
     def __str__(self):
         return self.name
 
     def __int__(self):
         return self.value
 
     def to_json(self):
-        return {'level': self.name, 'value': self.value}
+        return {"level": self.name, "value": self.value}
 
 
 class KMPAnalysis:
     def __init__(self):
         conf = SDCConf()
         self._valid_licenses = conf.get_valid_licenses()
 
     def kmp_analysis(self, data):
         ana_level = []
         name_lev, name_anls = self._kmp_name_analysis(data["name"])
-        ana_level.append(name_lev['value'])
+        ana_level.append(name_lev["value"])
         path_lev, path_anls = self._kmp_path_analysis(data["path"])
-        ana_level.append(path_lev['value'])
+        ana_level.append(path_lev["value"])
         ven_lev, vendor_anls = self._kmp_vendor_analysis(data["vendor"])
-        ana_level.append(ven_lev['value'])
+        ana_level.append(ven_lev["value"])
         sig_lev, sig_anls = self._kmp_vendor_analysis(data["signature"])
-        ana_level.append(ven_lev['value'])
+        ana_level.append(ven_lev["value"])
         lic_lev, license_anls = self._licenses_analysis([data["license"]])
-        ana_level.append(lic_lev['value'])
-        wm2_lev, wm2_invoked_anls = self._kmp_wm2_invoked_analysis(data["wm2_invoked"], data["name"])
-        ana_level.append(wm2_lev['value'])
-        km_lev, km_anls = self._kmp_km_analysis(data["reqs"], data["modalias"], data["km_info"])
-        ana_level.append(km_lev['value'])
+        ana_level.append(lic_lev["value"])
+        wm2_lev, wm2_invoked_anls = self._kmp_wm2_invoked_analysis(
+            data["wm2_invoked"], data["name"]
+        )
+        ana_level.append(wm2_lev["value"])
+        km_lev, km_anls = self._kmp_km_analysis(
+            data["reqs"], data["modalias"], data["km_info"]
+        )
+        ana_level.append(km_lev["value"])
 
         row_eval = KMPEvaluation(max(ana_level))
         return {
-            "level"      : row_eval.to_json(),
-            "name"       : {"level": name_lev, "value": name_anls},
-            "path"       : {"level": path_lev, "value": path_anls},
-            "vendor"     : {"level": ven_lev,  "value": vendor_anls},
-            "signature"  : {"level": sig_lev,  "value": sig_anls},
-            "license"    : {"level": lic_lev,  "value": license_anls},
-            "wm2_invoked": {"level": wm2_lev,  "value": wm2_invoked_anls},
-            "km"         : km_anls
+            "level": row_eval.to_json(),
+            "name": {"level": name_lev, "value": name_anls},
+            "path": {"level": path_lev, "value": path_anls},
+            "vendor": {"level": ven_lev, "value": vendor_anls},
+            "signature": {"level": sig_lev, "value": sig_anls},
+            "license": {"level": lic_lev, "value": license_anls},
+            "wm2_invoked": {"level": wm2_lev, "value": wm2_invoked_anls},
+            "km": km_anls,
         }
 
     def _kmp_name_analysis(self, name):
         return KMPEvaluation.PASS.to_json(), name
 
     def _kmp_path_analysis(self, path):
         return KMPEvaluation.PASS.to_json(), path
@@ -122,68 +129,79 @@
             for lic in invlics:
                 if lic == vlic.get("name"):
                     invlics.remove(lic)
 
         if len(invlics) == 0:
             return KMPEvaluation.PASS.to_json(), " ".join(licenses)
 
-        return KMPEvaluation.WARNING.to_json(), "Invalid or non Opensource license found: %s" % " ".join(invlics)
+        return (
+            KMPEvaluation.WARNING.to_json(),
+            "Invalid or non Opensource license found: %s" % " ".join(invlics),
+        )
 
     def _kmp_wm2_invoked_analysis(self, wm2, kmp_name):
-        if wm2 or "debuginfo" in kmp_name: # currently we ignore wm2 check for debuginfo package.
+        if (
+            wm2 or "debuginfo" in kmp_name
+        ):  # currently we ignore wm2 check for debuginfo package.
             return KMPEvaluation.PASS.to_json(), wm2
 
         return KMPEvaluation.ERROR.to_json(), wm2
 
     def _kmp_km_ana_summary(self, km_info, flavor):
         summary = {"level": KMPEvaluation.PASS.to_json(), "value": ""}
         values = []
         for km_path in km_info:
             km_data = km_info.get(km_path)
             level = km_data[flavor].get("level")
             msg = km_data[flavor].get("value")
 
-            summary["level"] = KMPEvaluation(max(summary["level"]['value'], level['value'])).to_json()
+            summary["level"] = KMPEvaluation(
+                max(summary["level"]["value"], level["value"])
+            ).to_json()
             values.append(msg)
 
         summary["value"] = " ".join(set(values))
 
         return summary
 
     def _kmp_km_analysis(self, kmp_reqs, kmp_modalias, km_info):
         km_analysis = {}
         ana_level = []
         for km_path in km_info:
             km_analysis[km_path] = {}
             eval, msg = self._licenses_analysis(km_info.get(km_path)["license"])
             km_analysis[km_path]["license"] = {"level": eval, "value": msg}
-            ana_level.append(eval['value'])
+            ana_level.append(eval["value"])
 
             eval, msg = self._km_supported_analysis(km_info.get(km_path)["supported"])
-            if eval['value'] != KMPEvaluation.PASS:
+            if eval["value"] != KMPEvaluation.PASS:
                 msg = f"{Path(km_path).name}: {msg}"
             km_analysis[km_path]["supported"] = {"level": eval, "value": msg}
-            ana_level.append(eval['value'])
+            ana_level.append(eval["value"])
 
             eval, msg = self._km_signature_analysis(km_info.get(km_path)["signature"])
             km_analysis[km_path]["signature"] = {"level": eval, "value": msg}
-            ana_level.append(eval['value'])
+            ana_level.append(eval["value"])
 
-            eval, msg = self._kms_symbols_analysis(kmp_reqs, km_info.get(km_path)["symbols"])
+            eval, msg = self._kms_symbols_analysis(
+                kmp_reqs, km_info.get(km_path)["symbols"]
+            )
             km_analysis[km_path]["symbols"] = {"level": eval, "value": msg}
-            ana_level.append(eval['value'])
+            ana_level.append(eval["value"])
 
         eval, alaias_msg = self._kms_modalias_analysis(kmp_modalias, km_info)
-        ana_level.append(eval['value'])
+        ana_level.append(eval["value"])
 
-        ana_summary = {"license"  : self._kmp_km_ana_summary(km_analysis, "license"),
-                       "supported": self._kmp_km_ana_summary(km_analysis, "supported"),
-                       "signature": self._kmp_km_ana_summary(km_analysis, "signature"),
-                       "symbols"  : {"level": eval, "value": alaias_msg},
-                       "alias"    : self._kmp_km_ana_summary(km_analysis, "symbols")}
+        ana_summary = {
+            "license": self._kmp_km_ana_summary(km_analysis, "license"),
+            "supported": self._kmp_km_ana_summary(km_analysis, "supported"),
+            "signature": self._kmp_km_ana_summary(km_analysis, "signature"),
+            "symbols": {"level": eval, "value": alaias_msg},
+            "alias": self._kmp_km_ana_summary(km_analysis, "symbols"),
+        }
 
         return KMPEvaluation(max(ana_level)).to_json(), ana_summary
 
     def _kms_symbols_analysis(self, kmp_reqs, km_syms):
         syms = {}
         syms["unfound"] = []
         syms["checksum-mismatch"] = []
@@ -213,16 +231,21 @@
         if mismatched > 0:
             msg = msg + f"Number of symbols checksum does not match: {mismatched}"
 
         return KMPEvaluation.ERROR.to_json(), msg.strip()
 
     def _kms_modalias_analysis(self, kmp_modalias, km_info):
         for a in kmp_modalias:
-            if a == "*":  # "use default-kernel:* to match all the devices is always a bad idea."
-                return KMPEvaluation.ERROR.to_json(), "KMP can match all the devices! Highly not recommended!"
+            if (
+                a == "*"
+            ):  # "use default-kernel:* to match all the devices is always a bad idea."
+                return (
+                    KMPEvaluation.ERROR.to_json(),
+                    "KMP can match all the devices! Highly not recommended!",
+                )
 
         kms_alias = []
         for km_path in km_info:
             kms_alias += km_info.get(km_path)["alias"]
         kms_alias = set(kms_alias)
         unmatched_ker_alias = []
         unmatched_kmp_alias = kmp_modalias.copy()
@@ -258,24 +281,27 @@
 
         return KMPEvaluation.ERROR.to_json(), msg
 
     def _km_signature_analysis(self, signature):
         if str(signature) != "":
             return KMPEvaluation.PASS.to_json(), "Exist"
 
-        return KMPEvaluation.WARNING.to_json(), "No signature found"        
+        return KMPEvaluation.WARNING.to_json(), "No signature found"
 
     def _km_supported_analysis(self, values):
         if len(values) < 1:
             return KMPEvaluation.ERROR.to_json(), "No 'supported' flag found"
 
         if len(values) == 1 and values[0] == "external":
             return KMPEvaluation.PASS.to_json(), ""
 
-        return KMPEvaluation.ERROR.to_json(), "Multiple values found, they're %s" % " ".join(values)
+        return (
+            KMPEvaluation.ERROR.to_json(),
+            "Multiple values found, they're %s" % " ".join(values),
+        )
 
 
 class KMPReader:
     def get_all_kmp_files(self, path):
         cmd = "find %s -regextype sed -regex '.*-kmp-.*\.rpm$'" % path
         kmps = run_cmd(cmd)
 
@@ -284,23 +310,25 @@
     def collect_kmp_data(self, path):
         base_info = self._get_kmp_info(path)
         wm2_invoked = self._check_kmp_wm2_invoked(path)
         reqs = self._get_kmp_requires(path)
         modalias = self._get_kmp_modalias(path)
         km_info = self._get_km_all_info(path)
 
-        return {"name"         : base_info.get("Name"),
-                "path"         : path,
-                "vendor"       : base_info.get("Vendor"),
-                "signature"    : base_info.get("Signature"),
-                "license"      : base_info.get("License"),
-                "wm2_invoked"  : wm2_invoked,
-                "reqs"         : reqs,
-                "modalias"     : modalias,
-                "km_info"      : km_info}
+        return {
+            "name": base_info.get("Name"),
+            "path": path,
+            "vendor": base_info.get("Vendor"),
+            "signature": base_info.get("Signature"),
+            "license": base_info.get("License"),
+            "wm2_invoked": wm2_invoked,
+            "reqs": reqs,
+            "modalias": modalias,
+            "km_info": km_info,
+        }
 
     def _get_km_symbols(self, path):
         cmd = "/usr/sbin/modprobe --dump-modversions %s" % path
         symbols = run_cmd(cmd)
 
         lines = symbols.splitlines()
         symver = {}
@@ -362,48 +390,54 @@
         tmp.cleanup()
 
         return result
 
     def _check_kmp_manifest(self, cmd_output):
         lines = cmd_output.splitlines()
 
-        if len(lines) < 1: # no output also means good.
+        if len(lines) < 1:  # no output also means good.
             return True, []
 
         items = lines[0].split(":")
-        if len(items) < 3:  # example: error: ./tmp/a.rpm: not an rpm package (or package manifest)
+        if (
+            len(items) < 3
+        ):  # example: error: ./tmp/a.rpm: not an rpm package (or package manifest)
             return True, []
 
         if items[0].strip() == "error":
-             return False, items
+            return False, items
 
         return True, []
 
     def _get_kmp_modalias(self, path):
         cmd = "".join("rpm -q --nosignature --supplements %s" % path)
         supplements = run_cmd(cmd)
 
         success, err_info = self._check_kmp_manifest(supplements)
         if not success:
             print(err_info)
             return []
 
         # modalias = namedtuple("modalias", "kernel_flavor pci_re")
-        ml_pci_re = re.compile(r"modalias\((.*):(.*\:.*)\)")  # example: modalias(kernel-default:pci:v000019A2d00000712sv*sd*bc*sc*i*)
-        ml_all_re = re.compile(r"modalias\((.*):(.*)\)")      # example: packageand(kernel-default:primergy-be2iscsi)
+        ml_pci_re = re.compile(
+            r"modalias\((.*):(.*\:.*)\)"
+        )  # example: modalias(kernel-default:pci:v000019A2d00000712sv*sd*bc*sc*i*)
+        ml_all_re = re.compile(
+            r"modalias\((.*):(.*)\)"
+        )  # example: packageand(kernel-default:primergy-be2iscsi)
 
         alias_re = []
         for line in supplements.splitlines():
             pci_rst = ml_pci_re.match(line)
             all_rst = ml_all_re.match(line)
             if pci_rst:
                 __, pci = pci_rst.groups()
-                if "pci:" in pci: # only check PCI devices
+                if "pci:" in pci:  # only check PCI devices
                     alias_re.append(pci)
-            elif all_rst: # match all (*) should not be allowed
+            elif all_rst:  # match all (*) should not be allowed
                 __, rst = all_rst.groups()
                 if rst == "*":
                     alias_re.append(rst)
 
         return alias_re
 
     def _check_kmp_wm2_invoked(self, path):
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/raw_data.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/raw_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
     return df
 
 
 def kmps_to_json(path, proc_injector=None):
     pass
 
+
 def km_to_dataframe(proc_injector=None):
     pass
 
+
 def km_to_json():
     pass
 
+
 def remote_km_to_json(remote_info, proc_injector=None):
     pass
-
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/cmd.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess
 
 
 def get_max_args():
     return int(run_cmd("getconf ARG_MAX"))
 
+
 def async_run_cmd(
     cmd, line_handler, line_handler_arg, start, end, condition, sshClient=None
 ):
     if sshClient is not None:
         __, stdout, __ = sshClient.exec_command(cmd)
 
         lines = stdout.read().decode().splitlines()
@@ -49,8 +50,7 @@
         return str(result, "utf-8")
     else:
         cmd_runner = subprocess.Popen(
             cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         result, __ = cmd_runner.communicate()
         return str(result, "utf-8")
-
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/api/utils/scripts/check-links.sh` & `soliddriver-checks-3.0.7/src/soliddriver_checks/api/utils/scripts/check-links.sh`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/cli/cli.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
             target = "system"
 
         self._target = target
 
     @property
     def system(self):
         target = Path(self._target)
-        return target.name == "system" and not (
-            target.is_file() or target.is_dir()
-        )
+        return target.name == "system" and not (target.is_file() or target.is_dir())
 
     @property
     def rpm(self):
         # need better check than this
         target = Path(self._target)
         if target.is_file() and target.name.endswith(".rpm"):
             return target
@@ -87,22 +85,22 @@
         exporter.to_html(check_result, dst)
     elif out_format == "xlsx":
         exporter.to_xlsx(check_result, dst)
     elif out_format == "json":
         exporter.to_json(check_result, dst)
 
 
-def km_export(exporter, label, check_result, out_format, dst):
+def km_export(exporter, label, check_result, filter, out_format, dst):
     dst = with_format_suffix(dst, out_format)
     if out_format == "html":
-        exporter.to_html(label, check_result, dst)
+        exporter.to_html(label, check_result, filter, dst)
     elif out_format == "xlsx":
-        exporter.to_xlsx(label, check_result, dst)
+        exporter.to_xlsx(label, check_result, filter, dst)
     elif out_format == "json":
-        exporter.to_json(label, check_result, dst)
+        exporter.to_json(label, check_result, filter, dst)
 
 
 def dst_is_ok(dst, out_format):
     def check(dst):
         if dst.is_file():
             if not os.access(dst, os.W_OK):
                 raise Exception("Cannot write to %s" % dst)
@@ -128,15 +126,21 @@
 @click.argument("check_target", default="system")
 @click.option(
     "--format",
     "-f",
     "out_format",
     type=click.Choice(FORMAT_TYPES),
     default="json",
-    help="Specify output format (PDF is in Beta)",
+    help="Specify output format",
+)
+@click.option(
+    "--filter",
+    "-i",
+    default="",
+    help="Filter kernel module to report (Beta)",
 )
 @click.option(
     "--output",
     "-o",
     default=".",
     help="Output destination. Target can be filename or point "
     "existing directory "
@@ -144,15 +148,15 @@
     "using a autmatically generated filename. If target "
     "is not an existing directory, file name is assumed "
     "and output files will use the path and file name "
     "specified. In either case, the file extension will "
     "be automatically appended matching on the output format",
 )
 @click.option("--version", is_flag=True)
-def run(check_target, output, out_format, version):
+def run(check_target, output, out_format, filter, version):
     """Run checks against CHECK_TARGET.
 
     \b
     CHECK_TARGET can be:
       KMP file
       directory containing KMP files
       "system" to check locally installed kernel modules
@@ -212,15 +216,16 @@
         except socket.gaierror as e:
             logger.warning(f"Get ip by hostname: {hostname} failed: {e}")
             ip = "127.0.0.1"
 
         label = "%s (%s)" % (hostname, ip)
         logger.info("Retrieving kernel module data for %s" % label)
         reporter = KMReporter()
-        km_export(reporter, label, None, out_format, dst)
+        km_export(reporter, label, None, filter, out_format, dst)
     elif target.url:
         df = read_remote_json(target.url)
         reporter = KMReporter()
-        km_export(reporter, target.url_host, df, out_format, dst)
+        km_export(reporter, target.url_host, df, filter, out_format, dst)
+
 
 if __name__ == "__main__":
     run()
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/cli/km_report.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/km_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,137 +37,167 @@
             elif int(KMEvaluation.ERROR) == cell_level:
                 style = f"background-color:{cri_bgcolor} color:{cri_color}"
 
             return style
 
         return [
             "",  # level style, no need for this.
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row["Module Name"]["level"]["value"])),
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row["File"]["level"]["value"])),
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row["License"]["level"]["value"])),
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row["Signature"]["level"]["value"])),
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row['"supported" Flag']["level"]["value"])),
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row["Module Name"]["level"]["value"]),
+            ),
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row["File"]["level"]["value"]),
+            ),
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row["License"]["level"]["value"]),
+            ),
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row["Signature"]["level"]["value"]),
+            ),
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row['"supported" Flag']["level"]["value"]),
+            ),
             "",  # running style, no need for this.
-            _get_cell_style(KMEvaluation(row["level"]["value"]), KMEvaluation(row["KMP"]["level"]["value"]))
+            _get_cell_style(
+                KMEvaluation(row["level"]["value"]),
+                KMEvaluation(row["KMP"]["level"]["value"]),
+            ),
         ]
 
     def _format_columns(self, df):
         return df.rename(
-            columns = {
-                "modulename" : "Module Name",
-                "filename"   : "File",
-                "license"    : "License",
-                "signature"  : "Signature",
-                "supported"  : '"supported" Flag',
-                "running"    : "Running",
-                "kmp"        : "KMP"
+            columns={
+                "modulename": "Module Name",
+                "filename": "File",
+                "license": "License",
+                "signature": "Signature",
+                "supported": '"supported" Flag',
+                "running": "Running",
+                "kmp": "KMP",
             }
         )
 
-    def to_html(self, sys_info, df_format, file):
+    def to_html(self, sys_info, df_format, filter, file):
         pkg_path = os.path.dirname(__file__)
         jinja_tmpl = f"{pkg_path}/../config/templates"
         file_loader = FileSystemLoader(jinja_tmpl)
         env = Environment(loader=file_loader)
 
         km_tmpl = env.get_template("km-report.html.jinja")
 
         if df_format is None:
-            df_format = kms_to_dataframe()  # read from local system.
+            df_format = kms_to_dataframe(filter)  # read from local system.
 
         kms_in_total = len(df_format.index)
-        failed_kms_in_total = len([f for f in df_format["level"].to_list() if f['value'] != int(KMEvaluation.PASS)])
+        failed_kms_in_total = len(
+            [
+                f
+                for f in df_format["level"].to_list()
+                if f["value"] != int(KMEvaluation.PASS)
+            ]
+        )
 
         df_format = self._format_columns(df_format)
-        ts = df_format.style.hide(axis="index").hide([('level')], axis="columns").set_table_attributes('class="table_center"').apply(self._row_style_in_html, axis=1).format(self._format_cell)
+        ts = (
+            df_format.style.hide(axis="index")
+            .hide([("level")], axis="columns")
+            .set_table_attributes('class="table_center"')
+            .apply(self._row_style_in_html, axis=1)
+            .format(self._format_cell)
+        )
 
         # df["running"].loc[df.running == True] = "&#9989;"
         # df["running"].loc[df.running == False] = "&#9940;"
         # df["running"].loc[df.running == ""] = "N/A"
 
         # Will be easier to get the value if run this after reformat the values.
-        external_kms_in_total = len([sf for sf in df_format['"supported" Flag'].to_list() if sf == "external"])
+        external_kms_in_total = len(
+            [sf for sf in df_format['"supported" Flag'].to_list() if sf == "external"]
+        )
 
         kms_buffer = km_tmpl.render(
-            version               = get_version(),
-            timestamp             = generate_timestamp(),
-            sysinfo               = sys_info,
-            kms_in_total          = kms_in_total,
-            external_kms_in_total = external_kms_in_total,
-            failed_kms_in_total   = failed_kms_in_total,
-            kms_table             = ts.to_html()
-            )
+            version=get_version(),
+            timestamp=generate_timestamp(),
+            sysinfo=sys_info,
+            kms_in_total=kms_in_total,
+            external_kms_in_total=external_kms_in_total,
+            failed_kms_in_total=failed_kms_in_total,
+            kms_table=ts.to_html(),
+        )
 
         with open(file, "w") as f:
             f.write(kms_buffer)
 
     def _create_xlsx_overview(self, ws):
         et = XlsxTemplate()
         et.set_km_overview(ws)
 
     def _create_xlsx_sheet(self, wb, sys_info, df):
         ws = wb.create_sheet(sys_info)
 
         df_values = df.copy()
         df_values = self._format_columns(df_values)
-        df_values = df_values.drop(['level'], axis=1)
+        df_values = df_values.drop(["level"], axis=1)
         df_values = df_values.applymap(lambda v: v.get("value", ""))
         # fill the values
         df_values = df_values.astype(str)
         for row in dataframe_to_rows(df_values, index=False, header=True):
             ws.append(row)
 
         # format table
         render = KMXlsxStyler()
         # format header
         for cell in ws[1]:
             render.set_header(cell)
 
         # format data
-        pair = {'A' : "modulename",
-        'B' : "filename",
-        'C' : "license",
-        'D' : "signature",
-        'E' : 'supported',
-        'F' : "running",
-        'G' : 'kmp'}
+        pair = {
+            "A": "modulename",
+            "B": "filename",
+            "C": "license",
+            "D": "signature",
+            "E": "supported",
+            "F": "running",
+            "G": "kmp",
+        }
 
         data_start_row = 2
         row_count = len(df.index) + data_start_row
         for i in range(data_start_row, row_count):
             # TODO: add row level style.
-            row_level = df.at[i-data_start_row, 'level']
+            row_level = df.at[i - data_start_row, "level"]
             for cell in ws[i]:
-                v = df.at[i-data_start_row, pair[cell.column_letter]]
-                lev = v.get('level')
-                if lev['value'] == int(KMEvaluation.PASS):
+                v = df.at[i - data_start_row, pair[cell.column_letter]]
+                lev = v.get("level")
+                if lev["value"] == int(KMEvaluation.PASS):
                     render.normal(cell)
-                elif lev['value'] == int(KMEvaluation.WARNING):
+                elif lev["value"] == int(KMEvaluation.WARNING):
                     render.warning(cell)
-                elif lev['value'] == int(KMEvaluation.ERROR):
+                elif lev["value"] == int(KMEvaluation.ERROR):
                     render.error(cell)
 
-        render.set_column_width(ws, {'A': 25,
-                                     'B': 90,
-                                     'C': 18,
-                                     'D': 10,
-                                     'E': 15,
-                                     'F': 10,
-                                     'G': 30})
+        render.set_column_width(
+            ws, {"A": 25, "B": 90, "C": 18, "D": 10, "E": 15, "F": 10, "G": 30}
+        )
 
-    def to_xlsx(self, sys_info, df_format, file):
+    def to_xlsx(self, sys_info, df_format, filter, file):
         wb = Workbook()
         self._create_xlsx_overview(wb.active)
 
         if df_format is None:
-            df_format = kms_to_dataframe()
+            df_format = kms_to_dataframe(filter)
 
         self._create_xlsx_sheet(wb, sys_info, df_format)
 
         wb.save(file)
 
-    def to_json(self, sys_info, df_format, file):
+    def to_json(self, sys_info, df_format, filter, file):
         buffer = kms_to_json(df_format)
 
         # TODO: add sys_info to json output.
         with open(file, "w") as fp:
             json.dump(json.loads(buffer), fp)
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/cli/kmp_report.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/kmp_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,54 +12,57 @@
 
 class KMPReporter:
     def __init__(self):
         self._style = SDCConf()
 
     def _summary(self, df):
         summary = df.copy()
-        for i, row in summary.iterrows():  # we need to do this for unique() since unhashable type: 'dict'.
+        # we need to do this for unique() since unhashable type: 'dict'.
+        for i, row in summary.iterrows():
             row["vendor"] = row["vendor"]["value"]
 
         def failed_len(col):
             counter = 0
             for v in col:
                 eval = v.get("level")
-                if eval['value'] != int(KMPEvaluation.PASS):
+                if eval["value"] != int(KMPEvaluation.PASS):
                     counter += 1
             return counter
 
         def format_cell(number, total):
             return f"{number} ({number/total * 100:.2f}%)"
 
         vendors = summary["vendor"].unique()
         sum_table = pd.DataFrame()
         for v in vendors:
-            vendor_df          = summary.loc[summary["vendor"] == v]
-            total              = len(vendor_df.index)
-            sig_failed         = failed_len(vendor_df["signature"])
-            license_failed     = failed_len(vendor_df["license"])
-            supported_failed   = failed_len(vendor_df["supported_flag"])
+            vendor_df = summary.loc[summary["vendor"] == v]
+            total = len(vendor_df.index)
+            sig_failed = failed_len(vendor_df["signature"])
+            license_failed = failed_len(vendor_df["license"])
+            supported_failed = failed_len(vendor_df["supported_flag"])
             wm2_invoked_failed = failed_len(vendor_df["wm2_invoked"])
-            km_sigs_failed     = failed_len(vendor_df["km_signatures"])
-            km_license_failed  = failed_len(vendor_df["km_licenses"])
-            symbols_failed     = failed_len(vendor_df["symbols"])
-            alias_failed       = failed_len(vendor_df["modalias"])
-
-            new_row = pd.Series({
-                "Vendor"             : v,
-                "Total KMPs"         : total,
-                "License"            : format_cell(license_failed, total),
-                "KMP Signature"      : format_cell(sig_failed, total),
-                "Weak Module Invoked": format_cell(wm2_invoked_failed, total),
-                "Supported Flag"     : format_cell(supported_failed, total),
-                "KM Signatures"      : format_cell(km_sigs_failed, total),
-                "KM Licenses"        : format_cell(km_license_failed, total),
-                "Symbols"            : format_cell(symbols_failed, total),
-                "Modalias"           : format_cell(alias_failed, total),
-            })
+            km_sigs_failed = failed_len(vendor_df["km_signatures"])
+            km_license_failed = failed_len(vendor_df["km_licenses"])
+            symbols_failed = failed_len(vendor_df["symbols"])
+            alias_failed = failed_len(vendor_df["modalias"])
+
+            new_row = pd.Series(
+                {
+                    "Vendor": v,
+                    "Total KMPs": total,
+                    "License": format_cell(license_failed, total),
+                    "KMP Signature": format_cell(sig_failed, total),
+                    "Weak Module Invoked": format_cell(wm2_invoked_failed, total),
+                    "Supported Flag": format_cell(supported_failed, total),
+                    "KM Signatures": format_cell(km_sigs_failed, total),
+                    "KM Licenses": format_cell(km_license_failed, total),
+                    "Symbols": format_cell(symbols_failed, total),
+                    "Modalias": format_cell(alias_failed, total),
+                }
+            )
 
             sum_table = pd.concat([sum_table, new_row.to_frame().T], ignore_index=True)
 
         return sum_table
 
     def _summary_to_html(self, df):
         tb = table()
@@ -158,45 +161,79 @@
 
     def _detail_to_html(self, df):
         def _create_cell(ana_val):
             level, value = ana_val.get("level"), ana_val.get("value")
             if value is None:
                 value = ""
 
-            if level['value'] == int(KMPEvaluation.PASS):
+            if level["value"] == int(KMPEvaluation.PASS):
                 return td(value)
-            elif level['value'] == int(KMPEvaluation.WARNING):
+            elif level["value"] == int(KMPEvaluation.WARNING):
                 return td(value).set_attribute("class", "important_failed")
-            elif level['value'] == int(KMPEvaluation.ERROR):
+            elif level["value"] == int(KMPEvaluation.ERROR):
                 return td(value).set_attribute("class", "critical_failed")
 
         tb = table()
         with tb:
             tb.set_attribute("class", "table_center")
             with tr():
                 th("KMP Checks", colspan=6).set_attribute("class", f"detail_rpm")
-                th("Kernel Module Checks", colspan=5).set_attribute("class", f"detail_kernel_module")
+                th("Kernel Module Checks", colspan=5).set_attribute(
+                    "class", f"detail_kernel_module"
+                )
             with tr():
                 th("Name").set_attribute("class", f"detail_0")
                 th("Path").set_attribute("class", f"detail_1")
                 th("Vendor").set_attribute("class", f"detail_2")
-                th(raw("Signature<span class=\"tooltiptext\">Only check there's a signature or not.</span>")).set_attribute("class", f"detail_3 tooltip")
-                th(raw("License<span class=\"tooltiptext\">KMP and it's kernel modules should use open source licenses.</span>")).set_attribute("class", f"detail_4 tooltip")
-                th(raw("Weak Module Invoked<span class=\"tooltiptext\">Weak Module is necessary to make 3rd party kernel modules installed for one kernel available to KABI-compatible kernels. </span>")).set_attribute("class", f"detail_5 tooltip")
-                th(raw("Licenses<span class=\"tooltiptext\">KMP and it's kernel modules should use open source licenses.</span>")).set_attribute("class", f"detail_6 tooltip")
-                th(raw("Signatures<span class=\"tooltiptext\">\"supported\" flag: <br/>  \"yes\": Only supported by SUSE<br/>  \"external\": supported by both SUSE and vendor</span>")).set_attribute("class", f"detail_6 tooltip")
-                th(raw("Supported Flag<span class=\"tooltiptext\">\"supported\" flag: <br/>  \"yes\": Only supported by SUSE<br/>  \"external\": supported by both SUSE and vendor</span>")).set_attribute("class", f"detail_6 tooltip")
-                th(raw("Symbols<span class=\"tooltiptext\">Symbols check is to check whether the symbols in kernel modules matches the symbols in its package.</span>")).set_attribute("class", f"detail_7 tooltip")
-                th(raw("Modalias<span class=\"tooltiptext\">Modalias check is to check whether the modalias in kernel modules matches the modalias in its package.</span>")).set_attribute("class", f"detail_8 tooltip")
+                th(
+                    raw(
+                        'Signature<span class="tooltiptext">Only check there\'s a signature or not.</span>'
+                    )
+                ).set_attribute("class", f"detail_3 tooltip")
+                th(
+                    raw(
+                        'License<span class="tooltiptext">KMP and it\'s kernel modules should use open source licenses.</span>'
+                    )
+                ).set_attribute("class", f"detail_4 tooltip")
+                th(
+                    raw(
+                        'Weak Module Invoked<span class="tooltiptext">Weak Module is necessary to make 3rd party kernel modules installed for one kernel available to KABI-compatible kernels. </span>'
+                    )
+                ).set_attribute("class", f"detail_5 tooltip")
+                th(
+                    raw(
+                        'Licenses<span class="tooltiptext">KMP and it\'s kernel modules should use open source licenses.</span>'
+                    )
+                ).set_attribute("class", f"detail_6 tooltip")
+                th(
+                    raw(
+                        'Signatures<span class="tooltiptext">"supported" flag: <br/>  "yes": Only supported by SUSE<br/>  "external": supported by both SUSE and vendor</span>'
+                    )
+                ).set_attribute("class", f"detail_6 tooltip")
+                th(
+                    raw(
+                        'Supported Flag<span class="tooltiptext">"supported" flag: <br/>  "yes": Only supported by SUSE<br/>  "external": supported by both SUSE and vendor</span>'
+                    )
+                ).set_attribute("class", f"detail_6 tooltip")
+                th(
+                    raw(
+                        'Symbols<span class="tooltiptext">Symbols check is to check whether the symbols in kernel modules matches the symbols in its package.</span>'
+                    )
+                ).set_attribute("class", f"detail_7 tooltip")
+                th(
+                    raw(
+                        'Modalias<span class="tooltiptext">Modalias check is to check whether the modalias in kernel modules matches the modalias in its package.</span>'
+                    )
+                ).set_attribute("class", f"detail_8 tooltip")
 
             for __, row in df.iterrows():
                 with tr() as r:
-                    if row["level"]['value'] == int(KMPEvaluation.WARNING):
+                    if row["level"]["value"] == int(KMPEvaluation.WARNING):
                         r.set_attribute("class", "important_failed_row")
-                    elif row["level"]['value'] == int(KMPEvaluation.ERROR):
+                    elif row["level"]["value"] == int(KMPEvaluation.ERROR):
                         r.set_attribute("class", "critical_failed_row")
 
                     _create_cell(row["name"])
                     _create_cell(row["path"])
                     _create_cell(row["vendor"])
                     _create_cell(row["signature"])
                     _create_cell(row["license"])
@@ -213,15 +250,17 @@
         pkg_path = os.path.dirname(__file__)
         jinja_tmpl = f"{pkg_path}/../config/templates"
         file_loader = FileSystemLoader(jinja_tmpl)
         env = Environment(loader=file_loader)
 
         kmp_tmpl = env.get_template("kmp-report.html.jinja")
 
-        kmp_checks = kmp_tmpl.render(version=get_version(), timestamp=generate_timestamp(),
+        kmp_checks = kmp_tmpl.render(
+            version=get_version(),
+            timestamp=generate_timestamp(),
             summary_table=self._summary_to_html(df),
             rpm_details=self._detail_to_html(df),
         )
 
         with open(file, "w") as f:
             f.write(kmp_checks)
 
@@ -237,15 +276,15 @@
         render = KMPXlsxStyler()
         render.render_summary(ws)
 
     def _detail_to_xlsx(self, wb, df):
         ws = wb.create_sheet("KMP Detail")
         df_values = df.copy()
         # format value
-        df_values = df_values.drop(['level'], axis=1)
+        df_values = df_values.drop(["level"], axis=1)
         df_values = df_values.applymap(lambda v: v.get("value", ""))
         # fill the values
         df_values = df_values.astype(str)
         for row in dataframe_to_rows(df_values, index=False, header=False):
             ws.append(row)
 
         ws.insert_rows(1, amount=2)
@@ -253,71 +292,79 @@
         render = KMPXlsxStyler()
         # create header
         def set_header(pairs):
             for loc in pairs:
                 ws[loc] = pairs[loc]
                 render.set_header(ws[loc])
 
-        set_header({
-            'A1': 'KMP Checks',
-            'G1': 'Kernel Module Checks',
-            'A2': 'Name',
-            'B2': 'Path',
-            'C2': 'Vendor',
-            'D2': 'Signature',
-            'E2': 'License',
-            'F2': 'Weak Module Invoked',
-            'G2': 'Licenses',
-            'H2': 'Signatures',
-            'I2': 'Supported Flag',
-            'J2': 'Symbols',
-            'K2': 'Modalias'
-        })
-        ws.merge_cells('A1:F1')
-        ws.merge_cells('G1:K1')
-
-        pair = {'A' : "name",
-        'B' : "path",
-        'C' : "vendor",
-        'D' : "signature",
-        'E' : 'license',
-        'F' : "wm2_invoked",
-        'G' : "km_licenses",
-        'H' : "km_signatures",
-        'I' : "supported_flag",
-        'J' : "symbols",
-        'K' : "modalias",
+        set_header(
+            {
+                "A1": "KMP Checks",
+                "G1": "Kernel Module Checks",
+                "A2": "Name",
+                "B2": "Path",
+                "C2": "Vendor",
+                "D2": "Signature",
+                "E2": "License",
+                "F2": "Weak Module Invoked",
+                "G2": "Licenses",
+                "H2": "Signatures",
+                "I2": "Supported Flag",
+                "J2": "Symbols",
+                "K2": "Modalias",
+            }
+        )
+        ws.merge_cells("A1:F1")
+        ws.merge_cells("G1:K1")
+
+        pair = {
+            "A": "name",
+            "B": "path",
+            "C": "vendor",
+            "D": "signature",
+            "E": "license",
+            "F": "wm2_invoked",
+            "G": "km_licenses",
+            "H": "km_signatures",
+            "I": "supported_flag",
+            "J": "symbols",
+            "K": "modalias",
         }
 
         data_start_row = 3
         row_count = len(df.index) + data_start_row
         for i in range(data_start_row, row_count):
             # TODO: add row level style.
-            row_level = df.at[i-data_start_row, 'level']
+            row_level = df.at[i - data_start_row, "level"]
             for cell in ws[i]:
-                v = df.at[i-data_start_row, pair[cell.column_letter]]
-                lev = v.get('level')
-                if lev['value'] == int(KMPEvaluation.PASS):
+                v = df.at[i - data_start_row, pair[cell.column_letter]]
+                lev = v.get("level")
+                if lev["value"] == int(KMPEvaluation.PASS):
                     render.normal(cell)
-                elif lev['value'] == int(KMPEvaluation.WARNING):
+                elif lev["value"] == int(KMPEvaluation.WARNING):
                     render.warning(cell)
-                elif lev['value'] == int(KMPEvaluation.ERROR):
+                elif lev["value"] == int(KMPEvaluation.ERROR):
                     render.error(cell)
 
-        render.set_column_width(ws, {'A': 25,
-                                     'B': 90,
-                                     'C': 18,
-                                     'D': 30,
-                                     'E': 15,
-                                     'F': 10,
-                                     'G': 20,
-                                     'H': 10,
-                                     'I': 30,
-                                     'J': 60,
-                                     'K': 40})
+        render.set_column_width(
+            ws,
+            {
+                "A": 25,
+                "B": 90,
+                "C": 18,
+                "D": 30,
+                "E": 15,
+                "F": 10,
+                "G": 20,
+                "H": 10,
+                "I": 30,
+                "J": 60,
+                "K": 40,
+            },
+        )
 
     def to_xlsx(self, df, file):
         wb = Workbook()
         self._create_xlsx_overview(wb.active)
 
         sum_table = self._summary(df)
         self._summary_to_xlsx(wb, sum_table)
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/cli/xlsx_utils.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/cli/xlsx_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,209 @@
 import os
 from copy import copy
 from openpyxl import load_workbook
 from ..config import SDCConf, get_version, generate_timestamp
 from openpyxl.formatting.rule import Rule
 from openpyxl.styles.differential import DifferentialStyle
 
+
 class XlsxStyler:
     def __init__(self):
         self._styler = SDCConf()
         self._header = {}
         self._data_pass = {}
         self._data_warning = {}
         self._data_error = {}
 
     def set_header(self, cell):
-        cell.font   = copy(self._header['font'])
-        cell.border = copy(self._header['border'])
-        cell.fill   = copy(self._header['fill'])
-    
+        cell.font = copy(self._header["font"])
+        cell.border = copy(self._header["border"])
+        cell.fill = copy(self._header["fill"])
+
     def normal(self, cell):
-        cell.font   = copy(self._data_pass['font'])
-        cell.border = copy(self._data_pass['border'])
-        cell.fill   = copy(self._data_pass['fill'])
-        
+        cell.font = copy(self._data_pass["font"])
+        cell.border = copy(self._data_pass["border"])
+        cell.fill = copy(self._data_pass["fill"])
+
     def warning(self, cell):
-        cell.font   = copy(self._data_warning['font'])
-        cell.border = copy(self._data_warning['border'])
-        cell.fill   = copy(self._data_warning['fill'])
-    
+        cell.font = copy(self._data_warning["font"])
+        cell.border = copy(self._data_warning["border"])
+        cell.fill = copy(self._data_warning["fill"])
+
     def error(self, cell):
-        cell.font   = copy(self._data_error['font'])
-        cell.border = copy(self._data_error['border'])
-        cell.fill   = copy(self._data_error['fill'])
-    
+        cell.font = copy(self._data_error["font"])
+        cell.border = copy(self._data_error["border"])
+        cell.fill = copy(self._data_error["fill"])
+
     def set_column_width(self, ws, columns):
         for key in columns:
             ws.column_dimensions[key].width = columns[key]
 
 
 class KMXlsxStyler(XlsxStyler):
     def __init__(self):
         super().__init__()
-        
-        (self._header['font'], 
-         self._header['border'],
-         self._header['fill']) = self._styler.get_km_header()
-        
-        (
-            self._data_pass['font'],
-            self._data_pass['border'],
-            self._data_pass['fill']
+
+        (
+            self._header["font"],
+            self._header["border"],
+            self._header["fill"],
+        ) = self._styler.get_km_header()
+
+        (
+            self._data_pass["font"],
+            self._data_pass["border"],
+            self._data_pass["fill"],
         ) = self._styler.get_km_normal()
-        
+
         (
-            self._data_warning['font'],
-            self._data_warning['border'],
-            self._data_warning['fill']
+            self._data_warning["font"],
+            self._data_warning["border"],
+            self._data_warning["fill"],
         ) = self._styler.get_km_warning()
-        
+
         (
-            self._data_error['font'],
-            self._data_error['border'],
-            self._data_error['fill']
+            self._data_error["font"],
+            self._data_error["border"],
+            self._data_error["fill"],
         ) = self._styler.get_km_error()
 
 
 class KMPXlsxStyler(XlsxStyler):
     def __init__(self):
         super().__init__()
         (
-            self._header['font'], 
-            self._header['border'], 
-            self._header['fill']
+            self._header["font"],
+            self._header["border"],
+            self._header["fill"],
         ) = self._styler.get_kmp_header()
-        
+
         (
-            self._data_pass['font'],
-            self._data_pass['border'],
-            self._data_pass['fill']
+            self._data_pass["font"],
+            self._data_pass["border"],
+            self._data_pass["fill"],
         ) = self._styler.get_kmp_normal()
-        
+
         (
-            self._data_warning['font'],
-            self._data_warning['border'],
-            self._data_warning['fill']
+            self._data_warning["font"],
+            self._data_warning["border"],
+            self._data_warning["fill"],
         ) = self._styler.get_kmp_warning()
-        
+
         (
-            self._data_error['font'],
-            self._data_error['border'],
-            self._data_error['fill']
+            self._data_error["font"],
+            self._data_error["border"],
+            self._data_error["fill"],
         ) = self._styler.get_kmp_error()
         self._row_pass = {}
         (
-            self._row_pass['font'],
-            self._row_pass['border'],
-            self._row_pass['fill']
+            self._row_pass["font"],
+            self._row_pass["border"],
+            self._row_pass["fill"],
         ) = self._styler.get_kmp_row_pass()
-    
+
     def render_summary(self, ws):
         # format header
         for cell in ws[1]:
-            cell.font = self._header['font']
-            cell.border = self._header['border']
-            cell.fill = self._header['fill']
-        
+            cell.font = self._header["font"]
+            cell.border = self._header["border"]
+            cell.fill = self._header["fill"]
+
         # format all the cells
         for row in range(2, ws.max_row + 1):
             for cell in ws[row]:
-                cell.font = self._data_pass['font']
-                cell.border = self._data_pass['border']
-                cell.fill = self._data_pass['fill']
-        
-        row_pass = Rule(type='expression', dxf=DifferentialStyle(
-            font=self._row_pass['font'],
-            border=self._row_pass['border'],
-            fill=self._row_pass['fill'],
-        ))
-        row_pass.formula = ['AND($A2 <> "", VALUE(LEFT($C2, FIND(" ",$C2)-1))=0, VALUE(LEFT($D2, FIND(" ", $D2) - 1)) = 0, VALUE(LEFT($E2, FIND(" ", $E2) - 1)) = 0, VALUE(LEFT($F2, FIND(" ", $F2)-1))=0, VALUE(LEFT($G2, FIND(" ", $G2) - 1))=0, VALUE(LEFT($H2, FIND(" ", $H2) - 1))=0, VALUE(LEFT($I2, FIND(" ", $I2) - 1))=0, VALUE(LEFT($J2, FIND(" ", $J2) - 1))=0)']
+                cell.font = self._data_pass["font"]
+                cell.border = self._data_pass["border"]
+                cell.fill = self._data_pass["fill"]
+
+        row_pass = Rule(
+            type="expression",
+            dxf=DifferentialStyle(
+                font=self._row_pass["font"],
+                border=self._row_pass["border"],
+                fill=self._row_pass["fill"],
+            ),
+        )
+        row_pass.formula = [
+            'AND($A2 <> "", VALUE(LEFT($C2, FIND(" ",$C2)-1))=0, VALUE(LEFT($D2, FIND(" ", $D2) - 1)) = 0, VALUE(LEFT($E2, FIND(" ", $E2) - 1)) = 0, VALUE(LEFT($F2, FIND(" ", $F2)-1))=0, VALUE(LEFT($G2, FIND(" ", $G2) - 1))=0, VALUE(LEFT($H2, FIND(" ", $H2) - 1))=0, VALUE(LEFT($I2, FIND(" ", $I2) - 1))=0, VALUE(LEFT($J2, FIND(" ", $J2) - 1))=0)'
+        ]
         ws.conditional_formatting.add(f"A2:J{ws.max_row}", row_pass)
-        
+
         def get_warning_rule():
-            return Rule(type='expression', dxf=DifferentialStyle(
-                font=self._data_warning['font'],
-                border = self._data_warning['border'],
-                fill=self._data_warning['fill']
-            ))
+            return Rule(
+                type="expression",
+                dxf=DifferentialStyle(
+                    font=self._data_warning["font"],
+                    border=self._data_warning["border"],
+                    fill=self._data_warning["fill"],
+                ),
+            )
+
         warning = get_warning_rule()
         warning.formula = ['$A2 = ""']
         ws.conditional_formatting.add(f"A2:A{ws.max_row}", warning)
-        
+
         warning = get_warning_rule()
         warning.formula = ['VALUE(LEFT($C2, FIND(" ", $C2) - 1)) <> 0']
         ws.conditional_formatting.add(f"C2:C{ws.max_row}", warning)
-        
+
         warning = get_warning_rule()
         warning.formula = ['VALUE(LEFT($D2, FIND(" ", $D2) - 1)) <> 0']
         ws.conditional_formatting.add(f"D2:D{ws.max_row}", warning)
-        
+
         warning = get_warning_rule()
         warning.formula = ['VALUE(LEFT($E2, FIND(" ", $E2) - 1)) <> 0']
         ws.conditional_formatting.add(f"E2:E{ws.max_row}", warning)
-        
+
         warning = get_warning_rule()
         warning.formula = ['VALUE(LEFT($G2, FIND(" ", $G2) - 1)) <> 0']
         ws.conditional_formatting.add(f"G2:G{ws.max_row}", warning)
-        
+
         warning = get_warning_rule()
         warning.formula = ['VALUE(LEFT($H2, FIND(" ", $H2) - 1)) <> 0']
         ws.conditional_formatting.add(f"H2:H{ws.max_row}", warning)
-        
+
         def get_error_rule():
-            return Rule(type='expression', dxf=DifferentialStyle(
-                font=self._data_error['font'],
-                border=self._data_error['border'],
-                fill=self._data_error['fill'],
-            ))
-        
+            return Rule(
+                type="expression",
+                dxf=DifferentialStyle(
+                    font=self._data_error["font"],
+                    border=self._data_error["border"],
+                    fill=self._data_error["fill"],
+                ),
+            )
+
         error = get_error_rule()
         error.formula = ['VALUE(LEFT($F2, FIND(" ", $F2) - 1)) <> 0']
         ws.conditional_formatting.add(f"F2:F{ws.max_row}", error)
-        
+
         error = get_error_rule()
         error.formula = ['VALUE(LEFT($I2, FIND(" ", $I2) - 1)) <> 0']
         ws.conditional_formatting.add(f"I2:I{ws.max_row}", error)
-        
+
         error = get_error_rule()
         error.formula = ['VALUE(LEFT($J2, FIND(" ", $J2) - 1)) <> 0']
         ws.conditional_formatting.add(f"J2:J{ws.max_row}", error)
-        
-        self.set_column_width(ws, {
-            'A': 40,
-            'B': 15,
-            'C': 15,
-            'D': 15,
-            'E': 15,
-            'F': 15,
-            'G': 15,
-            'H': 15,
-            'I': 15,
-            'J': 15
-        })
+
+        self.set_column_width(
+            ws,
+            {
+                "A": 40,
+                "B": 15,
+                "C": 15,
+                "D": 15,
+                "E": 15,
+                "F": 15,
+                "G": 15,
+                "H": 15,
+                "I": 15,
+                "J": 15,
+            },
+        )
+
 
 class XlsxTemplate:
     def __init__(self):
         pkg_path = os.path.dirname(__file__)
         self._cfg_path = f"{pkg_path}/../config/templates/templates.xlsx"
 
     def set_km_overview(self, ws):
@@ -193,21 +212,21 @@
     def set_kmp_overview(self, ws):
         self._copy_work_sheep("kmp-report-overview", ws)
 
     def _copy_work_sheep(self, title, ws):
         tmpl = load_workbook(filename=self._cfg_path)
         cover = tmpl[title]
         ws.title = "Overview"
-        
+
         for row in cover.rows:
             for cell in row:
-                ws[cell.coordinate].value     = copy(cell.value)
-                ws[cell.coordinate].style     = copy(cell.style)
-                ws[cell.coordinate].font      = copy(cell.font)
-                ws[cell.coordinate].border    = copy(cell.border)
-                ws[cell.coordinate].fill      = copy(cell.fill)
+                ws[cell.coordinate].value = copy(cell.value)
+                ws[cell.coordinate].style = copy(cell.style)
+                ws[cell.coordinate].font = copy(cell.font)
+                ws[cell.coordinate].border = copy(cell.border)
+                ws[cell.coordinate].fill = copy(cell.fill)
                 ws[cell.coordinate].alignment = copy(cell.alignment)
 
         ws["A5"].value = get_version()
         ws["A6"].value = generate_timestamp()
-        ws.column_dimensions['A'].width = 200
-        ws.page_setup.fitToHeight = 1
+        ws.column_dimensions["A"].width = 200
+        ws.page_setup.fitToHeight = 1
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/config/soliddriver-checks.conf` & `soliddriver-checks-3.0.7/src/soliddriver_checks/config/soliddriver-checks.conf`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/km-report.html.jinja` & `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/km-report.html.jinja`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/kmp-report.html.jinja` & `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/kmp-report.html.jinja`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/config/templates/templates.xlsx` & `soliddriver-checks-3.0.7/src/soliddriver_checks/config/templates/templates.xlsx`

 * *Files identical despite different names*

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/config.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         font = Font(
             name=conf["font"]["family"],
             size=conf["font"]["size"],
             bold=conf["font"]["bold"],
             color=conf["font"]["color"],
         )
         sd = Side(
-            border_style=conf["side"]["border_style"],
-            color=conf["side"]["color"]
+            border_style=conf["side"]["border_style"], color=conf["side"]["color"]
         )
         bd = Border(top=sd, left=sd, right=sd, bottom=sd)
         fill = PatternFill(
             start_color=conf["fill"]["bgcolor"],
             end_color=conf["fill"]["bgcolor"],
             fill_type="solid",
         )
@@ -58,44 +57,36 @@
     def get_kmp_header(self):
         return self._get_xlsx_info("kmp", "xlsx", "table", "header")
 
     def get_kmp_normal(self):
         return self._get_xlsx_info("kmp", "xlsx", "table", "data", "normal")
 
     def get_kmp_warning(self):
-        return self._get_xlsx_info(
-            "kmp", "xlsx", "table", "data", "warning"
-        )
+        return self._get_xlsx_info("kmp", "xlsx", "table", "data", "warning")
 
     def get_kmp_error(self):
-        return self._get_xlsx_info(
-            "kmp", "xlsx", "table", "data", "error"
-        )
+        return self._get_xlsx_info("kmp", "xlsx", "table", "data", "error")
 
     def get_kmp_row_pass(self):
         return self._get_xlsx_info("kmp", "xlsx", "table", "row", "pass")
 
     def get_km_sig_keys(self):
         return self._conf["km"]["sig-keys"]
 
     def get_km_header(self):
         return self._get_xlsx_info("km", "xlsx", "table", "header")
 
     def get_km_normal(self):
         return self._get_xlsx_info("km", "xlsx", "table", "data", "normal")
 
     def get_km_warning(self):
-        return self._get_xlsx_info(
-            "km", "xlsx", "table", "data", "warning"
-        )
+        return self._get_xlsx_info("km", "xlsx", "table", "data", "warning")
 
     def get_km_error(self):
-        return self._get_xlsx_info(
-            "km", "xlsx", "table", "data", "error"
-        )
+        return self._get_xlsx_info("km", "xlsx", "table", "data", "error")
 
     def get_km_warn_row(self):
         return self._get_xlsx_info("km", "xlsx", "table", "row", "warn")
 
     def get_km_html_warning(self):
         return self._conf["km"]["html"]["warning"]
 
@@ -126,8 +117,8 @@
                 ws[cell.coordinate].font = copy(cell.font)
                 ws[cell.coordinate].border = copy(cell.border)
                 ws[cell.coordinate].fill = copy(cell.fill)
                 ws[cell.coordinate].alignment = copy(cell.alignment)
 
         ws["A5"].value = get_version()
         ws["A6"].value = generate_timestamp()
-        ws.column_dimensions['A'].width = 200
+        ws.column_dimensions["A"].width = 200
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks/service/service.py` & `soliddriver-checks-3.0.7/src/soliddriver_checks/service/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,30 +35,32 @@
         new_data = kms_to_json()
         with self._data_lock:
             self._info = new_data
         logging.info("data refreshing is completed!")
 
 
 def run_as_service(host="0.0.0.0", port=8080):
-    logging.basicConfig(format='%(asctime)s : %(levelname)s : %(message)s', level=logging.INFO)
+    logging.basicConfig(
+        format="%(asctime)s : %(levelname)s : %(message)s", level=logging.INFO
+    )
     logging.info("soliddriver-checks-service version: %s" % __VERSION__)
 
     interval = os.getenv("REFRESH_INTERVAL")
     interval = int(interval) if interval is not None else 1
     logging.info("refresh interval: %s hour(s)" % interval)
 
     global kms
     kms = KMInfo(interval)
 
     run(host=host, port=port, quiet=True)
 
 
-@get('/kms_info')
+@get("/kms_info")
 def kms_info():
-    response.content_type = 'application/json'
+    response.content_type = "application/json"
     info = kms.data
     logging.info("GET /kms_info HTTP/1.1")
 
     return info
 
 
 if __name__ == "__main__":
```

### Comparing `soliddriver-checks-3.0.6/src/soliddriver_checks.egg-info/SOURCES.txt` & `soliddriver-checks-3.0.7/src/soliddriver_checks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 src/soliddriver_checks.egg-info/SOURCES.txt
 src/soliddriver_checks.egg-info/dependency_links.txt
 src/soliddriver_checks.egg-info/entry_points.txt
 src/soliddriver_checks.egg-info/requires.txt
 src/soliddriver_checks.egg-info/top_level.txt
 src/soliddriver_checks/api/__init__.py
 src/soliddriver_checks/api/analysis.py
+src/soliddriver_checks/api/filter.py
 src/soliddriver_checks/api/km.py
 src/soliddriver_checks/api/kmp.py
 src/soliddriver_checks/api/raw_data.py
 src/soliddriver_checks/api/utils/__init__.py
 src/soliddriver_checks/api/utils/cmd.py
 src/soliddriver_checks/api/utils/scripts/check-links.sh
 src/soliddriver_checks/cli/__init__.py
 src/soliddriver_checks/cli/cli.py
 src/soliddriver_checks/cli/km_report.py
 src/soliddriver_checks/cli/kmp_report.py
 src/soliddriver_checks/cli/terminal_logs.py
 src/soliddriver_checks/cli/xlsx_utils.py
-src/soliddriver_checks/config/.DS_Store
 src/soliddriver_checks/config/soliddriver-checks.conf
-src/soliddriver_checks/config/templates/.DS_Store
 src/soliddriver_checks/config/templates/km-report.html.jinja
 src/soliddriver_checks/config/templates/kmp-report.html.jinja
 src/soliddriver_checks/config/templates/templates.xlsx
 src/soliddriver_checks/service/__init__.py
 src/soliddriver_checks/service/service.py
```

