# Comparing `tmp/opendatalab-0.0.4.tar.gz` & `tmp/opendatalab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatalab-0.0.4.tar", last modified: Mon Feb 27 08:09:06 2023, max compression
+gzip compressed data, was "opendatalab-0.0.6.tar", last modified: Fri Apr 28 07:51:06 2023, max compression
```

## Comparing `opendatalab-0.0.4.tar` & `opendatalab-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.623800 opendatalab-0.0.4/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1078 2023-02-23 08:14:20.000000 opendatalab-0.0.4/LICENSE
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6079 2023-02-27 08:09:06.623800 opendatalab-0.0.4/PKG-INFO
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5014 2023-02-23 08:15:29.000000 opendatalab-0.0.4/README.md
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.619800 opendatalab-0.0.4/opendatalab/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      329 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      334 2023-02-27 08:05:39.000000 opendatalab-0.0.4/opendatalab/__version__.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.623800 opendatalab-0.0.4/opendatalab/cli/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      137 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4662 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/cmd.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      762 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/config.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1618 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/custom.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6828 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/get.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3100 2023-02-23 08:15:29.000000 opendatalab-0.0.4/opendatalab/cli/info.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      589 2023-02-23 08:15:29.000000 opendatalab-0.0.4/opendatalab/cli/login.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      620 2023-02-23 08:15:29.000000 opendatalab-0.0.4/opendatalab/cli/logout.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     2378 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/ls.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      150 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/policy.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3599 2023-02-23 08:15:29.000000 opendatalab-0.0.4/opendatalab/cli/search.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4775 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/upgrade.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4940 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/cli/utility.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.623800 opendatalab-0.0.4/opendatalab/client/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      264 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/client/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     7693 2023-02-23 08:20:33.000000 opendatalab-0.0.4/opendatalab/client/api.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1364 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/client/client.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3554 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/client/uaa.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.623800 opendatalab-0.0.4/opendatalab/dataset/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      224 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/dataset/__init__.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3524 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/dataset/dataset.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1416 2023-02-23 08:15:29.000000 opendatalab-0.0.4/opendatalab/exception.py
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       65 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/py.typed
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     2495 2023-02-23 08:14:20.000000 opendatalab-0.0.4/opendatalab/utils.py
-drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-02-27 08:09:06.619800 opendatalab-0.0.4/opendatalab.egg-info/
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6079 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      870 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        1 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       48 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/entry_points.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      102 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/requires.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       12 2023-02-27 08:09:06.000000 opendatalab-0.0.4/opendatalab.egg-info/top_level.txt
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1258 2023-02-27 08:09:06.623800 opendatalab-0.0.4/setup.cfg
--rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      485 2023-02-27 08:06:21.000000 opendatalab-0.0.4/setup.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1078 2023-02-23 08:14:20.000000 opendatalab-0.0.6/LICENSE
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-04-28 07:51:06.074505 opendatalab-0.0.6/PKG-INFO
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5014 2023-04-18 05:57:49.000000 opendatalab-0.0.6/README.md
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/opendatalab/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      295 2023-03-06 07:19:58.000000 opendatalab-0.0.6/opendatalab/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      391 2023-04-28 03:31:03.000000 opendatalab-0.0.6/opendatalab/__version__.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/opendatalab/cli/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      137 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/cli/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4515 2023-03-22 05:51:23.000000 opendatalab-0.0.6/opendatalab/cli/cmd.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      762 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/cli/config.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1618 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/cli/custom.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     5607 2023-04-28 07:50:03.000000 opendatalab-0.0.6/opendatalab/cli/get.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3100 2023-02-23 08:15:29.000000 opendatalab-0.0.6/opendatalab/cli/info.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      589 2023-03-06 10:56:03.000000 opendatalab-0.0.6/opendatalab/cli/login.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      620 2023-02-23 08:15:29.000000 opendatalab-0.0.6/opendatalab/cli/logout.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1986 2023-03-08 08:53:00.000000 opendatalab-0.0.6/opendatalab/cli/ls.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      150 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/cli/policy.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3775 2023-04-20 05:33:58.000000 opendatalab-0.0.6/opendatalab/cli/search.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4776 2023-04-06 08:11:36.000000 opendatalab-0.0.6/opendatalab/cli/upgrade.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     4941 2023-04-11 09:43:56.000000 opendatalab-0.0.6/opendatalab/cli/utility.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/opendatalab/client/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      264 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/client/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    11068 2023-04-20 05:38:34.000000 opendatalab-0.0.6/opendatalab/client/api.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1224 2023-03-06 09:18:13.000000 opendatalab-0.0.6/opendatalab/client/client.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)    13852 2023-04-20 06:16:53.000000 opendatalab-0.0.6/opendatalab/client/downloader.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     3579 2023-03-06 09:57:42.000000 opendatalab-0.0.6/opendatalab/client/uaa.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/opendatalab/dataset/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      224 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/dataset/__init__.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      772 2023-03-06 09:18:08.000000 opendatalab-0.0.6/opendatalab/dataset/dataset.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1416 2023-02-23 08:15:29.000000 opendatalab-0.0.6/opendatalab/exception.py
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       65 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/py.typed
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     2495 2023-02-23 08:14:20.000000 opendatalab-0.0.6/opendatalab/utils.py
+drwxr-xr-x   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        0 2023-04-28 07:51:06.074505 opendatalab-0.0.6/opendatalab.egg-info/
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     6129 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      903 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)        1 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       48 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/entry_points.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      102 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)       12 2023-04-28 07:51:06.000000 opendatalab-0.0.6/opendatalab.egg-info/top_level.txt
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)     1295 2023-04-28 07:51:06.074505 opendatalab-0.0.6/setup.cfg
+-rw-r--r--   0 PJLAB\weixingjian (409471169) PJLAB\domain^users (409469441)      486 2023-03-06 11:46:16.000000 opendatalab-0.0.6/setup.py
```

### Comparing `opendatalab-0.0.4/LICENSE` & `opendatalab-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/PKG-INFO` & `opendatalab-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatalab
-Version: 0.0.4
+Version: 0.0.6
 Summary: OpenDataLab Python SDK
 Home-page: https://github.com/opendatalab/opendatalab-python-sdk
 Author: OpenDataLab
 Author-email: OpenDataLab@pjlab.org.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opendatalab/opendatalab-python-sdk/issues
 Keywords: opendatalab,dataset,test
@@ -12,20 +12,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenDataLab Python SDK
 
 
 [![Downloads](https://pepy.tech/badge/opendatalab/month)](https://pepy.tech/project/opendatalab)
@@ -79,15 +80,15 @@
   search   Search dataset info.
   version  Show opendatalab version.
 ```
 
 ### Version
 ```cmd
 $ odl version
-odl version, current: 0.0.2, svc: 1.8
+odl version, current: 0.0.6, svc: 1.8
 ```
 
 ### Login
 Login with opendatalab username and password. If you haven't an opendatalab account，please register with link: https://opendatalab.org.cn/
 
 ```cmd
 $ odl login
```

### Comparing `opendatalab-0.0.4/README.md` & `opendatalab-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   search   Search dataset info.
   version  Show opendatalab version.
 ```
 
 ### Version
 ```cmd
 $ odl version
-odl version, current: 0.0.2, svc: 1.8
+odl version, current: 0.0.6, svc: 1.8
 ```
 
 ### Login
 Login with opendatalab username and password. If you haven't an opendatalab account，please register with link: https://opendatalab.org.cn/
 
 ```cmd
 $ odl login
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/cmd.py` & `opendatalab-0.0.6/opendatalab/cli/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """Definitions of OpenDataLab Command-line Interface commands."""
 import sys
 from functools import partial
 
 import click
 
-from opendatalab.__version__ import __version__, __url__, __svc__
+from opendatalab.__version__ import __svc__, __url__, __version__
 from opendatalab.cli.custom import CustomCommand
 from opendatalab.cli.utility import ContextInfo
 
 
 @click.group(context_settings={"help_option_names": ("-h", "--help")})
 @click.version_option(__version__)
 @click.option("-u", "--url", type=str, default=__url__, help="The login url.", hidden=True)
@@ -87,17 +87,15 @@
         username (str): account username
         password (str): account password
     """
     from opendatalab.cli.login import implement_login
     implement_login(obj, username, password)
 
 
-@command(synopsis=(
-        "$ odl ls dataset              # list dataset files",
-        "$ odl ls dataset/sub_dir      # list dataset/sub_dir files",))
+@command(synopsis=("$ odl ls dataset              # list dataset files",))
 @click.argument("name", nargs=1)
 @click.pass_obj
 def ls(obj: ContextInfo, name: str) -> None:
     """List files of the dataset.\f
 
     Args:
         obj (ContextInfo): context info
@@ -117,15 +115,15 @@
         obj (ContextInfo): context info
         keywords (str): dataset keywords
     """
     from opendatalab.cli.search import implement_search
     implement_search(obj, keywords)
 
 
-@command(synopsis=("$ odl info dataset_name      # show dataset info.",))
+@command(synopsis=("$ odl info dataset_name      # show dataset info",))
 @click.argument("name", nargs=1)
 @click.pass_obj
 def info(obj: ContextInfo, name):
     """Print dataset info.\f
     Args:
         obj (ContextInfo): context info
         name (str): dataset name
@@ -133,37 +131,34 @@
     from opendatalab.cli.info import implement_info
     implement_info(obj, name)
 
 
 @command(synopsis=("$ odl get dataset_name      # get dataset files into local",))
 @click.argument("name", nargs=1)
 @click.option(
-    "--thread",
-    "-t",
-    default=8,
-    help="Number of thread for download",
-    show_default=True,
+    "--dest",
+    "-d",
+    default='',
+    help="Desired dataset store path",
+    show_default=True
 )
 @click.option(
-    "--limit_speed",
-    "-l",
-    default=0,
-    help="Download limit speed: KB/s, 0 is unlimited",
-    show_default=True,
+    "--workers",
+    "-w",
+    default = 8,
+    help= "number of workers",
+    show_default = True
 )
 @click.pass_obj
-def get(obj: ContextInfo, name, thread, limit_speed):
+def get(obj: ContextInfo, name, dest, workers):
     """Get(Download) dataset files into local path.\f
-
     Args:
         obj (ContextInfo): context info\f
         name (str): dataset name\f
-        thread (int): multi-thread number\f
-        limit_speed (int): limit download speed, for not limit set value to 0
+        destination(str): desired dataset store path\f
+        wokers(str): number of workers\f
     """
-
+    
     from opendatalab.cli.get import implement_get
-    implement_get(obj, name, thread, limit_speed)
-
-
+    implement_get(obj, name, dest, workers)
 if __name__ == "__main__":
     cli()
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/config.py` & `opendatalab-0.0.6/opendatalab/cli/config.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab/cli/custom.py` & `opendatalab-0.0.6/opendatalab/cli/custom.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab/cli/info.py` & `opendatalab-0.0.6/opendatalab/cli/info.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab/cli/login.py` & `opendatalab-0.0.6/opendatalab/cli/login.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
 import sys
+
 from opendatalab.cli.utility import ContextInfo, exception_handler
 
 
 @exception_handler
 def implement_login(obj: ContextInfo, username: str, password: str) -> None:
     try:
         client = obj.get_client()
@@ -14,8 +15,7 @@
         obj.update_config(config_json)
 
     except Exception as e:
         print(f"Login failure with account {username}")
         sys.exit(-1)
 
     print(f"Login successfully as {username}")
-
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/logout.py` & `opendatalab-0.0.6/opendatalab/cli/logout.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab/cli/ls.py` & `opendatalab-0.0.6/opendatalab/cli/ls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
 import sys
 
-import oss2
 from rich import box
+from rich import print as rprint
 from rich.console import Console
 from rich.table import Table
 
 from opendatalab.cli.utility import ContextInfo, exception_handler
 from opendatalab.exception import OdlAccessDeniedError
 from opendatalab.utils import bytes2human
 
 
 @exception_handler
-def implement_ls(obj: ContextInfo, dataset: str) -> None:
+def implement_ls(obj: ContextInfo, dataset: str):
     """
     implementation for show dataset files
     Args:
         obj (ContextInfo):
         dataset (str): dataset name
 
     Returns:
@@ -29,45 +29,36 @@
         dataset_name = ds_split[0]
         sub_dir = "/".join(ds_split[1:])
     else:
         dataset_name = dataset
         sub_dir = ""
 
     client = obj.get_client()
-    info_data_name = client.get_api().get_info(dataset_name)['name']
-    dataset_instance = client.get_dataset(dataset_name=info_data_name)
-
-    bucket = dataset_instance.get_oss_bucket()
-    prefix = dataset_instance.get_object_key_prefix(compressed=True)
+    info_dataset_name = client.get_api().get_info(dataset_name)['name']
+    dataset_instance = client.get_dataset(dataset_name=info_dataset_name)
 
+    dataset_res_dict = client.get_api().get_dataset_files(dataset_name=info_dataset_name, prefix = sub_dir)
+    
+    # generate output info dict
     object_info_dict = {}
     total_files, total_size = 0, 0
-    for info in oss2.ObjectIteratorV2(bucket, prefix):
-        if not info.is_prefix() and not info.key.endswith("/"):
-            file_name = "/".join(info.key.split("/")[2:])
-            if not sub_dir:
-                object_info_dict[file_name] = bytes2human(info.size)
-                total_files = total_files + 1
-                total_size = total_size + info.size
-            elif sub_dir and file_name.startswith(sub_dir):
-                object_info_dict[file_name] = bytes2human(info.size)
-                total_files = total_files + 1
-                total_size = total_size + info.size
-            else:
-                pass
+    total_files = dataset_res_dict['total']
+    for info in dataset_res_dict['list']:
+        object_info_dict[info['path']] = bytes2human(info['size'])
+        total_size += info['size']
+
 
     if len(object_info_dict) == 0:
         raise OdlAccessDeniedError()
         sys.exit(-1)
 
     sorted_object_info_dict = dict(sorted(object_info_dict.items(), key=lambda x: x[0], reverse=True))
 
     console = Console()
     table = Table(show_header=True, header_style='bold cyan', box=box.ASCII2)  # ROUNDED
     table.add_column("File Name", min_width=20, justify='left')
     table.add_column("Size", width=12, justify='left')
 
-    print(f"total: {total_files}, size: {bytes2human(total_size)}")
+    print(f"Total file count: {total_files}, Size: {bytes2human(total_size)}")
     for key, val in sorted_object_info_dict.items():
         table.add_row(key, val, end_section=True)
-
     console.print(table)
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/search.py` & `opendatalab-0.0.6/opendatalab/cli/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
 import re
+import time
+
 from rich import box
 from rich.console import Console
 from rich.table import Table
+
 from opendatalab.cli.utility import ContextInfo, exception_handler
 from opendatalab.utils import bytes2human
 
 
 def rich_content_str(keywords: str, content: str):
     keywords = keywords.strip()
     len_keywords = len(keywords)
@@ -44,16 +47,19 @@
         keywords (str):
 
     Returns:
 
     """
     client = obj.get_client()
     odl_api = client.get_api()
+    import time
+    time_start =time.time()
     result_list = odl_api.search_dataset(keywords)
-
+    time_end = time.time()
+    # print('-------------time_consuming--------', time_end - time_start, 's')
     console = Console()
     table = Table(show_header=True, header_style='bold cyan', box=box.ASCII2)
     table.add_column("Name", min_width=10, justify='left', overflow='fold')
     table.add_column("DataType", min_width=8, justify='left', overflow='fold')
     table.add_column("FileByte", min_width=8, overflow='fold')
     table.add_column("FileCount", min_width=8, overflow='fold')
     table.add_column("TaskType", min_width=8, justify='left', overflow='fold')
@@ -67,16 +73,16 @@
             ds_name = res['name']
             ds_name_rich = rich_content_str(keywords=keywords, content=ds_name)
             ds_view_count = res['viewCount']
             ds_desc = res['introduction']['en'][:97] + '...'
             ds_desc_rich = rich_content_str(keywords=keywords, content=ds_desc)
 
             ds_attr_info = res['attrs']
-            ds_file_byte = bytes2human(ds_attr_info['fileBytes'])
-            ds_file_count = ds_attr_info['fileCount']
+            ds_file_byte = bytes2human(ds_attr_info.get('fileBytes', 0))
+            ds_file_count = ds_attr_info.get('fileCount',0)
 
             ds_data_types = _get_complex_types_str(ds_attr_info, 'mediaTypes')
             ds_task_types = _get_complex_types_str(ds_attr_info, 'taskTypes')
             ds_label_types = _get_complex_types_str(ds_attr_info, 'labelTypes')
 
             ds_task_types_rich = rich_content_str(keywords=keywords, content=ds_task_types)
             ds_label_types_rich = rich_content_str(keywords=keywords, content=ds_label_types)
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/upgrade.py` & `opendatalab-0.0.6/opendatalab/cli/upgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
-import sys
 import operator
+import sys
+
 import click
 
 from opendatalab.__version__ import __version__
 from opendatalab.cli.utility import ContextInfo, exception_handler
 
 
 @exception_handler
```

### Comparing `opendatalab-0.0.4/opendatalab/cli/utility.py` & `opendatalab-0.0.6/opendatalab/cli/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
 
 """OpenDataLab CLI utility functions."""
-import sys
 import json
+import sys
 from functools import wraps
 from typing import Any, Callable, TypeVar
+
 import click
-from opendatalab.__version__ import __version__
 
+from opendatalab.__version__ import __version__
 from opendatalab.cli.config import config as client_config
 from opendatalab.client import Client
-from opendatalab.utils import UUID
 from opendatalab.exception import OpenDataLabError
+from opendatalab.utils import UUID
 
 _Callable = TypeVar("_Callable", bound=Callable[..., None])
 
 
 class ContextInfo:
     """This class contains command context."""
```

### Comparing `opendatalab-0.0.4/opendatalab/client/api.py` & `opendatalab-0.0.6/opendatalab/client/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,111 @@
 
 
 class OpenDataLabAPI(object):
     def __init__(self, host, token, odl_cookie):
         self.host = host
         self.token = token
         self.odl_cookie = odl_cookie
+        
+    def get_dataset_files(self, dataset_name:str, prefix:str):
+        """ https request retrieve dataset files
+        Args:
+            dataset (str): dataset name
+            
+        Returns:
+            result_dict: 2 keys:
+                  dict['list']:contain list of files 
+                  dict['total']:files count.
+        """
+        
+        header_dict = {"X-OPENDATALAB-API-TOKEN": self.token,
+                "Cookie": f"opendatalab_session={self.odl_cookie}",
+                "User-Agent": UUID,
+                "accept" : "application/json"
+                }
+        data = {"recursive": True,
+                "prefix":prefix}
+        resp = requests.get(
+            url = f"{self.host}/api/datasets/{dataset_name}/files",
+            params = data,
+            headers = header_dict
+        )
+        if resp.status_code != 200:
+            if resp.status_code == 404:
+                raise OdlDataNotExistsError()
+            elif resp.status_code == 401:
+                raise OdlAuthError()
+            elif resp.status_code == 403:
+                raise OdlAccessDeniedError()
+            elif resp.status_code == 412:
+                raise OdlAccessCdnError()
+            elif resp.status_code == 500:
+                raise OdlAccessDeniedError()
+            else:
+                raise RespError(resp_code=resp.status_code, error_msg=resp.reason)
+        
+        result_dict = resp.json()['data']
+        
+        return result_dict
+    
+    def get_dataset_download_urls(self, dataset_id:int, dataset_list:list):
+        """get Dataset segments downloadable url
+
+        Args:
+            dataset (str): dataset name
+            dataset_list (list): list of dict contain segment size and name
+            
+        Returns:
+            download_url_list: list of dict contain segment name and executable url.
+        """
+        resp = requests.post(
+            f"{self.host}/api/track/datasets/download/{dataset_id}",
+            data = json.dumps(dataset_list),
+            headers={
+                    "Content-Type": "application/json",
+                    "Cookie": f"opendatalab_session={self.odl_cookie}",
+                    "User-Agent": f"opendatalab-python-sdk/{__version__}",
+                    "accept": "application/json"
+            }
+        )
+        if resp.status_code != 200:
+            print(f"{OpenDataLabError(resp.status_code, resp.text)}")
+            sys.exit(-1)
+        
+        download_url_list = resp.json()['data']
+        if not download_url_list:
+            click.secho(f"No datasets matched!", fg='red')
+            sys.exit(-1)
+        
+        return download_url_list
+   
+    def get_auth_status(self, dataset_id:int):
+        """Get Dataset authentication status.
 
+        Args:
+            dataset_id (int): dataset id
+        """
+        resp = requests.get(
+            f"{self.host}/api/datasets/{dataset_id}/downloadAuth",
+            headers= {
+                "X-OPENDATALAB-API-TOKEN": self.token,
+                "Cookie": f"opendatalab_session={self.odl_cookie}",
+                "User-Agent": UUID,
+                "accept" : "application/json"
+            }
+        )
+        if resp.status_code != 200:
+            click.echo(f"{OpenDataLabError(resp.status_code, resp.text)}")
+            sys.exit(-1)
+
+        result_status = resp.json()['data']
+        
+        return result_status
+    
+    
     def get_dataset_sts(self, dataset, expires=900):
         """Get dataset sts by dataset_name
         Args:
             expires (int): expire timeout unit seconds
             dataset (string): dataset_name
 
         Raises:
@@ -69,14 +165,15 @@
             data=json.dumps({
                 "backend": False,
                 "keywords": keywords,
                 "pageSize": 25,
                 "state": ["online"],
             })
         )
+        print(resp.status_code, resp.url)
         if resp.status_code != 200:
             print(f"{OpenDataLabError(resp.status_code, resp.text)}")
             sys.exit(-1)
 
         result_list = resp.json()["data"]["list"]
         if not result_list:
             click.secho(f"No datasets matched!", fg='red')
@@ -91,15 +188,14 @@
             headers={"X-OPENDATALAB-API-TOKEN": self.token,
                      "Cookie": f"opendatalab_session={self.odl_cookie}",
                      "User-Agent": f"opendatalab-python-sdk/{__version__}",
                      "Content-Type": "application/json"
                      },
         )
         if resp.status_code != 200:
-            # print(f"{(resp.status_code, resp.text)}")
             sys.exit(-1)
 
         data = resp.json()['data']
         return data
 
     def get_info(self, dataset):
         resp = requests.get(
@@ -190,15 +286,14 @@
         data = json.dumps(data)
 
         resp = requests.post(
             f"{self.host}/api/users/auth",
             data=data,
             headers={"Content-Type": "application/json"},
         )
-
         if resp.status_code != 200:
             raise OdlAuthError(resp.status_code, resp.text)
 
         odl_token = resp.json()["data"]["token"]
         config_json = {
             'user.email': account,
             'user.token': odl_token,
```

### Comparing `opendatalab-0.0.4/opendatalab/client/client.py` & `opendatalab-0.0.6/opendatalab/client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 #
 # Copyright 2022 Shanghai AI Lab. Licensed under MIT License.
 #
+from opendatalab.__version__ import __url__
 from opendatalab.client.api import OpenDataLabAPI
 from opendatalab.dataset.dataset import Dataset
 from opendatalab.utils import get_api_token_from_env
-from opendatalab.__version__ import __url__
 
 
 class Client:
     def __init__(self, host: str = __url__, token: str = "", odl_cookie: str = ""):
         """opendatalab client
 
         Args:
@@ -27,14 +27,10 @@
 
     def get_dataset(self, dataset_name: str) -> Dataset:
         if dataset_name not in self.dataset_map:
             self.dataset_map[dataset_name] = Dataset(
                 f"{self.host}/datasets/{dataset_name}", self.token, self.odl_cookie)
         return self.dataset_map[dataset_name]
 
-    def get(self, dataset_name: int, filepath: str):
-        dataset = self.get_dataset(dataset_name)
-        return dataset.get(filepath)
-
     def get_api(self):
         self.odl_api = OpenDataLabAPI(self.host, self.token, self.odl_cookie)
         return self.odl_api
```

### Comparing `opendatalab-0.0.4/opendatalab/client/uaa.py` & `opendatalab-0.0.6/opendatalab/client/uaa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import json
 import sys
+import time
+from base64 import b64decode, b64encode
 
 import click
 import requests
-import json
-import time
-from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5
-from base64 import b64encode, b64decode
+from Crypto.PublicKey import RSA
 
-from opendatalab.__version__ import uaa_url_prefix, odl_clientId
+from opendatalab.__version__ import odl_clientId, uaa_url_prefix
 
 api_login = "/api/v1/login/byClientSdk"
 api_public_key = "/api/v1/cipher/getPubKey"
 api_user_info = "/api/v1/login/getUserInfo"
 api_auth = "/api/v1/internal/auth"
 
 
@@ -117,11 +117,12 @@
 def get_odl_token(account, password):
     authorization, sso_uid = get_account(account=account, password=password)
     auth_code = None
     if sso_uid:
         auth_code = get_auth_code(sso_uid=sso_uid)
 
     if not auth_code:
+        print(auth_code)
         click.secho(f"Error: Auth failure with account: {account}", err=True, fg="red")
         sys.exit(1)
 
     return auth_code
```

### Comparing `opendatalab-0.0.4/opendatalab/exception.py` & `opendatalab-0.0.6/opendatalab/exception.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab/utils.py` & `opendatalab-0.0.6/opendatalab/utils.py`

 * *Files identical despite different names*

### Comparing `opendatalab-0.0.4/opendatalab.egg-info/PKG-INFO` & `opendatalab-0.0.6/opendatalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendatalab
-Version: 0.0.4
+Version: 0.0.6
 Summary: OpenDataLab Python SDK
 Home-page: https://github.com/opendatalab/opendatalab-python-sdk
 Author: OpenDataLab
 Author-email: OpenDataLab@pjlab.org.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opendatalab/opendatalab-python-sdk/issues
 Keywords: opendatalab,dataset,test
@@ -12,20 +12,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OpenDataLab Python SDK
 
 
 [![Downloads](https://pepy.tech/badge/opendatalab/month)](https://pepy.tech/project/opendatalab)
@@ -79,15 +80,15 @@
   search   Search dataset info.
   version  Show opendatalab version.
 ```
 
 ### Version
 ```cmd
 $ odl version
-odl version, current: 0.0.2, svc: 1.8
+odl version, current: 0.0.6, svc: 1.8
 ```
 
 ### Login
 Login with opendatalab username and password. If you haven't an opendatalab account，please register with link: https://opendatalab.org.cn/
 
 ```cmd
 $ odl login
```

### Comparing `opendatalab-0.0.4/opendatalab.egg-info/SOURCES.txt` & `opendatalab-0.0.6/opendatalab.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 opendatalab/cli/policy.py
 opendatalab/cli/search.py
 opendatalab/cli/upgrade.py
 opendatalab/cli/utility.py
 opendatalab/client/__init__.py
 opendatalab/client/api.py
 opendatalab/client/client.py
+opendatalab/client/downloader.py
 opendatalab/client/uaa.py
 opendatalab/dataset/__init__.py
 opendatalab/dataset/dataset.py
```

### Comparing `opendatalab-0.0.4/setup.cfg` & `opendatalab-0.0.6/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Typing :: Typed
 
 [options]
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.7
 install_requires = 
+	pycryptodome
 	click >= 7.0.0
 	requests >= 2.4.2
-	tqdm >= 4.14.0
-	oss2
+	tqdm
 	colorama
 	rich
 	pywin32; platform_system == "Windows"
 
 [options.packages.find]
 include = opendatalab*
 exclude = *.tests
```

