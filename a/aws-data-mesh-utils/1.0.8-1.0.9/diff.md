# Comparing `tmp/aws-data-mesh-utils-1.0.8.tar.gz` & `tmp/aws-data-mesh-utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-data-mesh-utils-1.0.8.tar", last modified: Mon Feb 28 18:52:27 2022, max compression
+gzip compressed data, was "aws-data-mesh-utils-1.0.9.tar", last modified: Tue Mar  1 13:32:07 2022, max compression
```

## Comparing `aws-data-mesh-utils-1.0.8.tar` & `aws-data-mesh-utils-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.127218 aws-data-mesh-utils-1.0.8/
--rw-r--r--   0 meyersi    (504) staff       (20)    10142 2021-11-24 10:46:06.000000 aws-data-mesh-utils-1.0.8/LICENSE
--rw-r--r--   0 meyersi    (504) staff       (20)       37 2021-11-26 15:00:03.000000 aws-data-mesh-utils-1.0.8/MANIFEST.in
--rw-r--r--   0 meyersi    (504) staff       (20)       67 2021-11-24 10:46:06.000000 aws-data-mesh-utils-1.0.8/NOTICE
--rw-r--r--   0 meyersi    (504) staff       (20)    21506 2022-02-28 18:52:27.127755 aws-data-mesh-utils-1.0.8/PKG-INFO
--rw-r--r--   0 meyersi    (504) staff       (20)    20770 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.8/README.md
--rw-r--r--   0 meyersi    (504) staff       (20)      103 2021-11-26 13:41:12.000000 aws-data-mesh-utils-1.0.8/pyproject.toml
--rw-r--r--   0 meyersi    (504) staff       (20)      880 2022-02-28 18:52:27.128587 aws-data-mesh-utils-1.0.8/setup.cfg
--rw-r--r--   0 meyersi    (504) staff       (20)      306 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.8/setup.py
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.104763 aws-data-mesh-utils-1.0.8/src/
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.110696 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/
--rw-r--r--   0 meyersi    (504) staff       (20)    21506 2022-02-28 18:52:26.000000 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/PKG-INFO
--rw-r--r--   0 meyersi    (504) staff       (20)     1277 2022-02-28 18:52:27.000000 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 meyersi    (504) staff       (20)        1 2022-02-28 18:52:26.000000 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 meyersi    (504) staff       (20)       85 2022-02-28 18:52:27.000000 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/requires.txt
--rw-r--r--   0 meyersi    (504) staff       (20)       29 2022-02-28 18:52:27.000000 aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.112029 aws-data-mesh-utils-1.0.8/src/data_mesh_cli/
--rw-r--r--   0 meyersi    (504) staff       (20)    14058 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_cli/DataMeshCli.py
--rw-r--r--   0 meyersi    (504) staff       (20)        0 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_cli/__init__.py
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.116068 aws-data-mesh-utils-1.0.8/src/data_mesh_util/
--rw-r--r--   0 meyersi    (504) staff       (20)    18355 2022-01-18 14:00:27.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshAdmin.py
--rw-r--r--   0 meyersi    (504) staff       (20)     7761 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshConsumer.py
--rw-r--r--   0 meyersi    (504) staff       (20)     1784 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshMacros.py
--rw-r--r--   0 meyersi    (504) staff       (20)    31027 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshProducer.py
--rw-r--r--   0 meyersi    (504) staff       (20)       28 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/__init__.py
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.119606 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/
--rw-r--r--   0 meyersi    (504) staff       (20)    48369 2022-02-28 18:52:14.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/ApiAutomator.py
--rw-r--r--   0 meyersi    (504) staff       (20)    23343 2022-02-28 18:52:14.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/SubscriberTracker.py
--rw-r--r--   0 meyersi    (504) staff       (20)        0 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/__init__.py
--rw-r--r--   0 meyersi    (504) staff       (20)      838 2022-02-28 16:51:20.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/constants.py
--rw-r--r--   0 meyersi    (504) staff       (20)    10106 2022-02-28 18:52:14.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/utils.py
-drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-02-28 18:52:27.126145 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/
--rw-r--r--   0 meyersi    (504) staff       (20)     3448 2021-11-23 09:06:53.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/consumer_account_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)     2690 2021-11-22 18:12:58.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/consumer_mesh_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)     1236 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/data_mesh_read_only_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)      520 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/data_mesh_setup_iam_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)      261 2021-11-17 18:02:02.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/enable_crawler_role.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)      942 2022-02-23 09:50:26.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/lf_cross_account_tbac.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)     1585 2021-11-17 12:14:30.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/producer_account_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)      355 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/producer_bucket_policy.pystache
--rw-r--r--   0 meyersi    (504) staff       (20)     4543 2021-11-24 17:18:58.000000 aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/producer_mesh_policy.pystache
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.292107 aws-data-mesh-utils-1.0.9/
+-rw-r--r--   0 meyersi    (504) staff       (20)    10142 2021-11-24 10:46:06.000000 aws-data-mesh-utils-1.0.9/LICENSE
+-rw-r--r--   0 meyersi    (504) staff       (20)       37 2021-11-26 15:00:03.000000 aws-data-mesh-utils-1.0.9/MANIFEST.in
+-rw-r--r--   0 meyersi    (504) staff       (20)       67 2021-11-24 10:46:06.000000 aws-data-mesh-utils-1.0.9/NOTICE
+-rw-r--r--   0 meyersi    (504) staff       (20)    21506 2022-03-01 13:32:07.292338 aws-data-mesh-utils-1.0.9/PKG-INFO
+-rw-r--r--   0 meyersi    (504) staff       (20)    20770 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.9/README.md
+-rw-r--r--   0 meyersi    (504) staff       (20)      103 2021-11-26 13:41:12.000000 aws-data-mesh-utils-1.0.9/pyproject.toml
+-rw-r--r--   0 meyersi    (504) staff       (20)      880 2022-03-01 13:32:07.293021 aws-data-mesh-utils-1.0.9/setup.cfg
+-rw-r--r--   0 meyersi    (504) staff       (20)      306 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.9/setup.py
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.268404 aws-data-mesh-utils-1.0.9/src/
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.274485 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/
+-rw-r--r--   0 meyersi    (504) staff       (20)    21506 2022-03-01 13:32:07.000000 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 meyersi    (504) staff       (20)     1277 2022-03-01 13:32:07.000000 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 meyersi    (504) staff       (20)        1 2022-03-01 13:32:07.000000 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 meyersi    (504) staff       (20)       85 2022-03-01 13:32:07.000000 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/requires.txt
+-rw-r--r--   0 meyersi    (504) staff       (20)       29 2022-03-01 13:32:07.000000 aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.275646 aws-data-mesh-utils-1.0.9/src/data_mesh_cli/
+-rw-r--r--   0 meyersi    (504) staff       (20)    13679 2022-03-01 13:31:53.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_cli/DataMeshCli.py
+-rw-r--r--   0 meyersi    (504) staff       (20)        0 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_cli/__init__.py
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.279898 aws-data-mesh-utils-1.0.9/src/data_mesh_util/
+-rw-r--r--   0 meyersi    (504) staff       (20)    18355 2022-01-18 14:00:27.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshAdmin.py
+-rw-r--r--   0 meyersi    (504) staff       (20)     7761 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshConsumer.py
+-rw-r--r--   0 meyersi    (504) staff       (20)     1784 2022-02-24 11:26:56.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshMacros.py
+-rw-r--r--   0 meyersi    (504) staff       (20)    31027 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshProducer.py
+-rw-r--r--   0 meyersi    (504) staff       (20)       28 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/__init__.py
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.283959 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/
+-rw-r--r--   0 meyersi    (504) staff       (20)    48369 2022-02-28 18:52:14.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/ApiAutomator.py
+-rw-r--r--   0 meyersi    (504) staff       (20)    23343 2022-02-28 18:52:14.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/SubscriberTracker.py
+-rw-r--r--   0 meyersi    (504) staff       (20)        0 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/__init__.py
+-rw-r--r--   0 meyersi    (504) staff       (20)      838 2022-02-28 16:51:20.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/constants.py
+-rw-r--r--   0 meyersi    (504) staff       (20)    11278 2022-03-01 13:31:53.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/utils.py
+drwxr-xr-x   0 meyersi    (504) staff       (20)        0 2022-03-01 13:32:07.291001 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/
+-rw-r--r--   0 meyersi    (504) staff       (20)     3448 2021-11-23 09:06:53.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/consumer_account_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)     2690 2021-11-22 18:12:58.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/consumer_mesh_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)     1236 2022-02-28 14:53:38.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/data_mesh_read_only_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)      520 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/data_mesh_setup_iam_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)      261 2021-11-17 18:02:02.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/enable_crawler_role.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)      942 2022-02-23 09:50:26.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/lf_cross_account_tbac.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)     1585 2021-11-17 12:14:30.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/producer_account_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)      355 2021-09-29 13:31:36.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/producer_bucket_policy.pystache
+-rw-r--r--   0 meyersi    (504) staff       (20)     4543 2021-11-24 17:18:58.000000 aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/producer_mesh_policy.pystache
```

### Comparing `aws-data-mesh-utils-1.0.8/LICENSE` & `aws-data-mesh-utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/PKG-INFO` & `aws-data-mesh-utils-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-data-mesh-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: The AWS Data Mesh Helper library provides automation around the most common tasks that customers need to perform to implement a data mesh architecture on AWS.
 Home-page: https://github.com/aws-samples/aws-data-mesh-utils
 Author: Ian Meyers
 Author-email: meyersi@amazon.co.uk
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/aws-samples/aws-data-mesh-utils/issues
 Platform: UNKNOWN
```

### Comparing `aws-data-mesh-utils-1.0.8/README.md` & `aws-data-mesh-utils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/setup.cfg` & `aws-data-mesh-utils-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aws-data-mesh-utils
-version = 1.0.8
+version = 1.0.9
 author = Ian Meyers
 author_email = meyersi@amazon.co.uk
 license = Apache 2.0
 description = The AWS Data Mesh Helper library provides automation around the most common tasks that customers need to perform to implement a data mesh architecture on AWS.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aws-samples/aws-data-mesh-utils
```

### Comparing `aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/PKG-INFO` & `aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-data-mesh-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: The AWS Data Mesh Helper library provides automation around the most common tasks that customers need to perform to implement a data mesh architecture on AWS.
 Home-page: https://github.com/aws-samples/aws-data-mesh-utils
 Author: Ian Meyers
 Author-email: meyersi@amazon.co.uk
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/aws-samples/aws-data-mesh-utils/issues
 Platform: UNKNOWN
```

### Comparing `aws-data-mesh-utils-1.0.8/src/aws_data_mesh_utils.egg-info/SOURCES.txt` & `aws-data-mesh-utils-1.0.9/src/aws_data_mesh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_cli/DataMeshCli.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_cli/DataMeshCli.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,26 +220,14 @@
     :return:
     '''
     constructor = inspect.getattr_static(cls, "__init__")
     constructor_args = inspect.getfullargspec(constructor)
     return _extract_req_opt_params(constructor_args)
 
 
-# load required args for runtimes into sys.argv
-def _load_sysarg(key: str, value: str) -> None:
-    sys.argv.append(f"--{key}")
-    sys.argv.append(value)
-
-
-def _underscore_sysargs() -> None:
-    for i, value in enumerate(sys.argv):
-        if value[:2] == '--':
-            sys.argv[i] = f"--{value[2:].replace('-', '_')}"
-
-
 class DataMeshCli:
     _caller_name = "DataMeshCli"
     _all_commands = None
     _region = None
     _creds = None
     _account_ids = None
 
@@ -271,28 +259,28 @@
         the caller
         :param from_filename:
         :return:
         '''
         self._region, x, self._account_ids, self._creds = utils.load_client_info_from_file(
             from_filename)
 
-        _load_sysarg("region_name", self._region)
+        utils.load_sysarg("region_name", self._region)
         if MESH in self._account_ids:
-            _load_sysarg("data_mesh_account_id", self._account_ids.get(MESH))
+            utils.load_sysarg("data_mesh_account_id", self._account_ids.get(MESH))
 
     def run(self):
         '''
         Main runner method for the CLI class. All parameters are harvested from sys.argv
         :return:
         '''
         if len(sys.argv) == 1:
             _cli_usage("No Valid Arguments Supplied")
 
-        # convert dashed arg names to underscore - annoying for users if we don't do this. all usage will show underscore
-        _underscore_sysargs()
+        # fix sys.argv values which might contain rubbish
+        utils.purify_sysargs()
 
         # create an argument parser with the caller name listed so we get a nice usage string
         parser = argparse.ArgumentParser(prog=self._caller_name)
 
         # add command line arguments to grab credentials information at first
         parser.add_argument("--data_mesh_account_id", required=False)
         parser.add_argument("--credentials_file", required=False)
```

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshAdmin.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshAdmin.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshConsumer.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshConsumer.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshMacros.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshMacros.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/DataMeshProducer.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/DataMeshProducer.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/ApiAutomator.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/ApiAutomator.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/SubscriberTracker.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/SubscriberTracker.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/lib/constants.py` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/lib/constants.py`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/consumer_account_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/consumer_account_policy.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/consumer_mesh_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/consumer_mesh_policy.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/data_mesh_read_only_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/data_mesh_read_only_policy.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/data_mesh_setup_iam_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/data_mesh_setup_iam_policy.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/lf_cross_account_tbac.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/lf_cross_account_tbac.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/producer_account_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/producer_account_policy.pystache`

 * *Files identical despite different names*

### Comparing `aws-data-mesh-utils-1.0.8/src/data_mesh_util/resource/producer_mesh_policy.pystache` & `aws-data-mesh-utils-1.0.9/src/data_mesh_util/resource/producer_mesh_policy.pystache`

 * *Files identical despite different names*

