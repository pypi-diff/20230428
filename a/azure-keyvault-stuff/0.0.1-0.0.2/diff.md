# Comparing `tmp/azure-keyvault-stuff-0.0.1.tar.gz` & `tmp/azure-keyvault-stuff-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-keyvault-stuff-0.0.1.tar", last modified: Fri Apr 28 13:04:58 2023, max compression
+gzip compressed data, was "azure-keyvault-stuff-0.0.2.tar", last modified: Fri Apr 28 14:05:12 2023, max compression
```

## Comparing `azure-keyvault-stuff-0.0.1.tar` & `azure-keyvault-stuff-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:04:58.505741 azure-keyvault-stuff-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-28 12:59:23.000000 azure-keyvault-stuff-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      747 2023-04-28 13:04:58.504740 azure-keyvault-stuff-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-04-28 12:44:54.000000 azure-keyvault-stuff-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 13:04:58.505741 azure-keyvault-stuff-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1207 2023-04-28 13:01:33.000000 azure-keyvault-stuff-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:04:58.486740 azure-keyvault-stuff-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 13:04:58.502737 azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/
--rw-rw-rw-   0        0        0      747 2023-04-28 13:04:58.000000 azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-28 13:04:58.000000 azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:04:58.000000 azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-28 13:04:58.000000 azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:05:12.823786 azure-keyvault-stuff-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-28 12:59:23.000000 azure-keyvault-stuff-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      747 2023-04-28 14:05:12.820777 azure-keyvault-stuff-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-04-28 12:44:54.000000 azure-keyvault-stuff-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:05:12.823786 azure-keyvault-stuff-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1207 2023-04-28 14:03:32.000000 azure-keyvault-stuff-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:05:12.802776 azure-keyvault-stuff-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:05:12.817776 azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/
+-rw-rw-rw-   0        0        0      747 2023-04-28 14:05:12.000000 azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-28 14:05:12.000000 azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:05:12.000000 azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-28 14:05:12.000000 azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/top_level.txt
```

### Comparing `azure-keyvault-stuff-0.0.1/LICENSE` & `azure-keyvault-stuff-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-keyvault-stuff-0.0.1/PKG-INFO` & `azure-keyvault-stuff-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-stuff
-Version: 0.0.1
+Version: 0.0.2
 Summary: Azure Key Vault Helper Package
 Home-page: https://github.com/george-oconnor/azure-keyvault-stuff
 Author: george.oconnor (George O' Connor)
 Author-email: <george@georgestools.com>
 Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials,azure.identity.DefaultAzureCredential()
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `azure-keyvault-stuff-0.0.1/setup.py` & `azure-keyvault-stuff-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Azure Key Vault Helper Package'
 LONG_DESCRIPTION = 'A package that provides helper functions for interacting with Azure Key Vault.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setting up
```

### Comparing `azure-keyvault-stuff-0.0.1/src/azure_keyvault_stuff.egg-info/PKG-INFO` & `azure-keyvault-stuff-0.0.2/src/azure_keyvault_stuff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-stuff
-Version: 0.0.1
+Version: 0.0.2
 Summary: Azure Key Vault Helper Package
 Home-page: https://github.com/george-oconnor/azure-keyvault-stuff
 Author: george.oconnor (George O' Connor)
 Author-email: <george@georgestools.com>
 Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials,azure.identity.DefaultAzureCredential()
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

