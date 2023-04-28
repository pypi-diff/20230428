# Comparing `tmp/pulumiverse_purrl-0.3.1.tar.gz` & `tmp/pulumiverse_purrl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_purrl-0.3.1.tar", last modified: Mon Mar 13 09:22:05 2023, max compression
+gzip compressed data, was "pulumiverse_purrl-0.4.0.tar", last modified: Fri Apr 28 08:19:30 2023, max compression
```

## Comparing `pulumiverse_purrl-0.3.1.tar` & `pulumiverse_purrl-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:22:05.957671 pulumiverse_purrl-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-13 09:22:05.957671 pulumiverse_purrl-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:22:05.957671 pulumiverse_purrl-0.3.1/pulumiverse_purrl/
--rw-------   0 runner    (1001) docker     (123)      606 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8080 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     2713 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/provider.py
--rw-------   0 runner    (1001) docker     (123)       93 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)    26713 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/purrl.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 09:22:05.957671 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 09:22:05.957671 pulumiverse_purrl-0.3.1/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2122 2023-03-13 09:22:05.000000 pulumiverse_purrl-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/pulumiverse_purrl/
+-rw-------   0 runner    (1001) docker     (123)      606 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8080 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     2713 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/provider.py
+-rw-------   0 runner    (1001) docker     (123)       93 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)    26974 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/purrl.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2153 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/setup.py
```

### Comparing `pulumiverse_purrl-0.3.1/PKG-INFO` & `pulumiverse_purrl-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumiverse_purrl
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Pulumi native provider for making API calls
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-purrl
 Keywords: pulumi command category/utility kind/native
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Purrl
 
 [![Go Reference](https://pkg.go.dev/badge/github.com/pulumiverse/pulumi-purrl/sdk.svg)](https://pkg.go.dev/github.com/pulumiverse/pulumi-purrl/sdk)
 
 ![purrl_logo](img/purrl.png)
```

### Comparing `pulumiverse_purrl-0.3.1/README.md` & `pulumiverse_purrl-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.3.1/pulumiverse_purrl/__init__.py` & `pulumiverse_purrl-0.4.0/pulumiverse_purrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.3.1/pulumiverse_purrl/_utilities.py` & `pulumiverse_purrl-0.4.0/pulumiverse_purrl/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.3.1/pulumiverse_purrl/provider.py` & `pulumiverse_purrl-0.4.0/pulumiverse_purrl/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.3.1/pulumiverse_purrl/purrl.py` & `pulumiverse_purrl-0.4.0/pulumiverse_purrl/purrl.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,15 @@
                 raise TypeError("Missing required property 'response_codes'")
             __props__.__dict__["response_codes"] = response_codes
             if url is None and not opts.urn:
                 raise TypeError("Missing required property 'url'")
             __props__.__dict__["url"] = url
             __props__.__dict__["delete_response"] = None
             __props__.__dict__["response"] = None
+            __props__.__dict__["response_code"] = None
         super(Purrl, __self__).__init__(
             'purrl:index:Purrl',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -487,14 +488,15 @@
         __props__.__dict__["delete_url"] = None
         __props__.__dict__["headers"] = None
         __props__.__dict__["insecure_skip_tls_verify"] = None
         __props__.__dict__["key"] = None
         __props__.__dict__["method"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["response"] = None
+        __props__.__dict__["response_code"] = None
         __props__.__dict__["response_codes"] = None
         __props__.__dict__["url"] = None
         return Purrl(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def body(self) -> pulumi.Output[Optional[str]]:
@@ -644,14 +646,19 @@
     def response(self) -> pulumi.Output[str]:
         """
         The response from the API call.
         """
         return pulumi.get(self, "response")
 
     @property
+    @pulumi.getter(name="responseCode")
+    def response_code(self) -> pulumi.Output[int]:
+        return pulumi.get(self, "response_code")
+
+    @property
     @pulumi.getter(name="responseCodes")
     def response_codes(self) -> pulumi.Output[Sequence[str]]:
         """
         The expected response code.
         """
         return pulumi.get(self, "response_codes")
```

### Comparing `pulumiverse_purrl-0.3.1/pulumiverse_purrl.egg-info/PKG-INFO` & `pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumiverse-purrl
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Pulumi native provider for making API calls
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-purrl
 Keywords: pulumi command category/utility kind/native
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Purrl
 
 [![Go Reference](https://pkg.go.dev/badge/github.com/pulumiverse/pulumi-purrl/sdk.svg)](https://pkg.go.dev/github.com/pulumiverse/pulumi-purrl/sdk)
 
 ![purrl_logo](img/purrl.png)
```

### Comparing `pulumiverse_purrl-0.3.1/setup.py` & `pulumiverse_purrl-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.3.1"
-PLUGIN_VERSION = "0.3.1"
+VERSION = "0.4.0"
+PLUGIN_VERSION = "0.4.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'purrl', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "purrl Pulumi Package - Development Version"
 
 
 setup(name='pulumiverse_purrl',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi native provider for making API calls",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

