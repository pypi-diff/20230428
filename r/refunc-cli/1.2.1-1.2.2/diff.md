# Comparing `tmp/refunc-cli-1.2.1.tar.gz` & `tmp/refunc-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refunc-cli-1.2.1.tar", last modified: Tue Apr 25 06:30:34 2023, max compression
+gzip compressed data, was "refunc-cli-1.2.2.tar", last modified: Fri Apr 28 05:23:23 2023, max compression
```

## Comparing `refunc-cli-1.2.1.tar` & `refunc-cli-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-23 02:26:55.000000 refunc-cli-1.2.1/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-23 09:58:14.000000 refunc-cli-1.2.1/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.556407 refunc-cli-1.2.1/refunc_cli.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-25 06:30:34.000000 refunc-cli-1.2.1/refunc_cli.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-24 06:30:18.000000 refunc-cli-1.2.1/requirements.txt
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/rfctl/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-23 02:02:22.000000 refunc-cli-1.2.1/rfctl/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-24 02:41:18.000000 refunc-cli-1.2.1/rfctl/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-24 02:58:19.000000 refunc-cli-1.2.1/rfctl/awslocal.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-25 06:26:50.000000 refunc-cli-1.2.1/rfctl/build.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/rfctl/client/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-24 06:37:09.000000 refunc-cli-1.2.1/rfctl/client/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1425 2023-04-24 06:31:46.000000 refunc-cli-1.2.1/rfctl/client/client.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      841 2023-04-25 06:27:25.000000 refunc-cli-1.2.1/rfctl/create.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-23 07:21:11.000000 refunc-cli-1.2.1/rfctl/create_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-23 07:14:35.000000 refunc-cli-1.2.1/rfctl/delete.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-23 07:21:59.000000 refunc-cli-1.2.1/rfctl/delete_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-23 07:28:56.000000 refunc-cli-1.2.1/rfctl/get.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-23 07:28:47.000000 refunc-cli-1.2.1/rfctl/get_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-24 06:51:06.000000 refunc-cli-1.2.1/rfctl/init.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-25 06:20:52.000000 refunc-cli-1.2.1/rfctl/init_source.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-23 03:35:02.000000 refunc-cli-1.2.1/rfctl/schema.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-25 06:27:08.000000 refunc-cli-1.2.1/rfctl/update_code.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-23 07:17:30.000000 refunc-cli-1.2.1/rfctl/update_config.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-25 06:30:34.564407 refunc-cli-1.2.1/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-25 06:21:17.000000 refunc-cli-1.2.1/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.499520 refunc-cli-1.2.2/refunc_cli.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-28 05:23:23.000000 refunc-cli-1.2.2/refunc_cli.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/requirements.txt
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/rfctl/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/awslocal.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/build.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/rfctl/client/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/client/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1449 2023-04-28 05:20:56.000000 refunc-cli-1.2.2/rfctl/client/client.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      841 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/create.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/create_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/delete.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/delete_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/get.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/get_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3152 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/init.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/init_source.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/schema.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/update_code.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-28 05:17:10.000000 refunc-cli-1.2.2/rfctl/update_config.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-28 05:23:23.507520 refunc-cli-1.2.2/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-28 05:22:41.000000 refunc-cli-1.2.2/setup.py
```

### Comparing `refunc-cli-1.2.1/refunc_cli.egg-info/SOURCES.txt` & `refunc-cli-1.2.2/refunc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/__main__.py` & `refunc-cli-1.2.2/rfctl/__main__.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/awslocal.py` & `refunc-cli-1.2.2/rfctl/awslocal.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/build.py` & `refunc-cli-1.2.2/rfctl/build.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/client/client.py` & `refunc-cli-1.2.2/rfctl/client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class LambdaClient:
     def __init__(self, region_name):
         self.lambda_client = boto3.client('lambda',
                                           region_name=region_name,
                                           endpoint_url=os.environ.get("AWS_DEFAULT_ENDPOINT"),
                                           use_ssl=False,
-                                          aws_access_key_id=os.environ.get('AWS_ACCESS_KEY_ID'),
-                                          aws_secret_access_key=os.environ.get('AWS_SECRET_ACCESS_KEY'))
+                                          aws_access_key_id=os.environ.get('AWS_ACCESS_KEY_ID', "__none__"),
+                                          aws_secret_access_key=os.environ.get('AWS_SECRET_ACCESS_KEY', "__none__"))
 
     def invoke_function(self, function_name, function_params, get_log=False):
         response = self.lambda_client.invoke(FunctionName=function_name, Payload=json.dumps(function_params), LogType='Tail' if get_log else 'None')
         metadata = response["ResponseMetadata"]
         payload = response["Payload"]
         if get_log:
             headers = metadata["HTTPHeaders"]
```

### Comparing `refunc-cli-1.2.1/rfctl/create.py` & `refunc-cli-1.2.2/rfctl/create.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/init.py` & `refunc-cli-1.2.2/rfctl/init.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/init_source.py` & `refunc-cli-1.2.2/rfctl/init_source.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/schema.py` & `refunc-cli-1.2.2/rfctl/schema.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/update_code.py` & `refunc-cli-1.2.2/rfctl/update_code.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/rfctl/update_config.py` & `refunc-cli-1.2.2/rfctl/update_config.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.2.1/setup.py` & `refunc-cli-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='refunc-cli',
-    version='1.2.1',
+    version='1.2.2',
     description='refunc command line tools',
     author='arvin',
     license='MIT',
     url='https://github.com/refunc/refunc-cli',
     author_email='arvintian8@gamil.com',
     packages=find_packages(),
     include_package_data=True,
```

