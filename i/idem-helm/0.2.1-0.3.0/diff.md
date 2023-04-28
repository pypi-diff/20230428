# Comparing `tmp/idem-helm-0.2.1.tar.gz` & `tmp/idem-helm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-helm-0.2.1.tar", last modified: Thu Mar 23 20:14:42 2023, max compression
+gzip compressed data, was "idem-helm-0.3.0.tar", last modified: Fri Apr 28 14:35:41 2023, max compression
```

## Comparing `idem-helm-0.2.1.tar` & `idem-helm-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-03-23 20:14:28.000000 idem-helm-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5330 2023-03-23 20:14:42.355701 idem-helm-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4526 2023-03-23 20:14:28.000000 idem-helm-0.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/acct/helm/
--rw-r--r--   0 root         (0) root         (0)      552 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/acct/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/exec/helm/
--rw-r--r--   0 root         (0) root         (0)      169 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/exec/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     3672 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/exec/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/states/helm/
--rw-r--r--   0 root         (0) root         (0)      167 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/states/helm/init.py
--rw-r--r--   0 root         (0) root         (0)    14846 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/states/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm/tool/helm/
--rw-r--r--   0 root         (0) root         (0)     3262 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/tool/helm/command_utils.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/tool/helm/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/tool/helm/release_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-03-23 20:14:28.000000 idem-helm-0.2.1/idem_helm/tool/helm/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-23 20:14:41.000000 idem-helm-0.2.1/idem_helm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 20:14:42.355701 idem-helm-0.2.1/idem_helm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5330 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-23 20:14:42.000000 idem-helm-0.2.1/idem_helm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-23 20:14:42.355701 idem-helm-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2719 2023-03-23 20:14:28.000000 idem-helm-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-04-28 14:35:27.000000 idem-helm-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-28 14:35:41.067172 idem-helm-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-04-28 14:35:27.000000 idem-helm-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/acct/helm/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/acct/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/exec/helm/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/exec/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/exec/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/states/helm/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)    14938 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/tool/helm/
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/command_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/release_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:35:40.000000 idem-helm-0.3.0/idem_helm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:35:41.071172 idem-helm-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-04-28 14:35:27.000000 idem-helm-0.3.0/setup.py
```

### Comparing `idem-helm-0.2.1/LICENSE` & `idem-helm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/PKG-INFO` & `idem-helm-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.2.1
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.2.1/README.rst` & `idem-helm-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/acct/helm/init.py` & `idem-helm-0.3.0/idem_helm/acct/helm/init.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/conf.py` & `idem-helm-0.3.0/idem_helm/conf.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/exec/helm/release.py` & `idem-helm-0.3.0/idem_helm/exec/helm/release.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/states/helm/release.py` & `idem-helm-0.3.0/idem_helm/states/helm/release.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""States module for Helm Release."""
 import copy
 import re
 from typing import Any
 from typing import Dict
 from typing import List
 
 import dict_tools.differ as differ
@@ -32,60 +33,57 @@
     atomic: bool = False,
     devel: bool = False,
     disable_openapi_validation: bool = False,
     no_hooks: bool = False,
     verify: bool = False,
     timeout: str = None,
 ) -> Dict[str, Any]:
-    r"""
-
-    create/update a Helm Release
+    """Create/Update a Helm Release.
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider.
-        chart(Text): Chart name to be installed
-        namespace(Text): namespace scope for helm release
-        repository(Text, optional): chart repository url where to locate the requested chart
-        values(Dict, optional): Specify values in a YAML
-        version(Text, optional): Chart version to install. If this is not specified, the latest version is installed.
-        key_file(Text, optional): The repositories cert key file
-        keyring(Text, optional): location of public keys used for verification (default "~/.gnupg/pubring.gpg")
-        values_files(List, optional): specify values in a YAML file
-        ca_file(Text, optional): verify certificates of HTTPS-enabled servers using this CA bundle
-        cert_file(Text, optional): identify HTTPS client using this SSL certificate file
-        username(Text, optional): chart repository username where to locate the requested chart
-        password(Text, optional): chart repository password where to locate the requested chart
-        dependency_update(Boolean, optional): update dependencies if they are missing before installing the chart
-        create_namespace(Boolean, optional): create the release namespace if not present
-        atomic(Boolean, optional): if True, the installation process deletes the installation on failure.
-        devel(Boolean, optional): use development versions, too. Equivalent to version '>0.0.0-0'. If --version is set, this is ignored
-        disable_openapi_validation(Boolean, optional): if set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema
-        no_hooks(Boolean, optional): prevent hooks from running during install
-        verify(Boolean, optional): verify the package before using it.
-                                    If verify is set, the chart MUST have a provenance file, and the provenance file MUST pass all verification steps.
+        name(str): An Idem name of the resource.
+        chart(str): Chart name to be installed
+        namespace(str): namespace scope for helm release
+        resource_id(str, Optional): An identifier of the resource in the provider.
+        repository(str, Optional): chart repository url where to locate the requested chart
+        values(Dict, Optional): Specify values in a YAML
+        version(str, Optional): Chart version to install. If this is not specified, the latest version is installed.
+        key_file(str, Optional): The repositories cert key file
+        keyring(str, Optional): location of public keys used for verification (default "~/.gnupg/pubring.gpg")
+        values_files(List, Optional): specify values in a YAML file
+        ca_file(str, Optional): verify certificates of HTTPS-enabled servers using this CA bundle
+        cert_file(str, Optional): identify HTTPS client using this SSL certificate file
+        username(str, Optional): chart repository username where to locate the requested chart
+        password(str, Optional): chart repository password where to locate the requested chart
+        dependency_update(bool, Optional): update dependencies if they are missing before installing the chart
+        create_namespace(bool, Optional): create the release namespace if not present
+        atomic(bool, Optional): if True, the installation process deletes the installation on failure.
+        devel(bool, Optional): use development versions, too. Equivalent to version '>0.0.0-0'. If --version is set, this is ignored
+        disable_openapi_validation(bool, Optional): if set, the installation process will not validate rendered templates against the Kubernetes OpenAPI Schema
+        no_hooks(bool, Optional): prevent hooks from running during install
+        verify(bool, Optional): verify the package before using it.
+            If verify is set, the chart MUST have a provenance file, and the provenance file MUST pass all verification steps.
         timeout(str, Optional): time to wait for Kubernetes commands to complete. (Ex-: 100s, 200s, 10m)
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             idem-helm-release-test:
               helm.release.present:
-              - name: idem-redis
-              - resource_id: idem-redis
-              - repository: https://charts.bitnami.com/bitnami
-              - chart: redis
-              - namespace: kube-system
-              - timeout: 200s
-    """
+                - name: idem-redis
+                - resource_id: idem-redis
+                - repository: https://charts.bitnami.com/bitnami
+                - chart: redis
+                - namespace: kube-system
+                - timeout: 200s
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     before = None
     list_release_ret = None
     # Check for existing release by name in namespace
     if resource_id:
         list_release_ret = await hub.exec.helm.release.list_releases(
             ctx, resource_id, namespace
@@ -305,40 +303,37 @@
             else:
                 desire_state[key] = value
 
     return desire_state
 
 
 async def absent(
-    hub, ctx, name: str, namespace: str, resource_id: str = None
+    hub, ctx, name: str, namespace: str = "default", resource_id: str = None
 ) -> Dict[str, Any]:
-    r"""
-
-    delete a helm release
+    """Delete a helm release
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider.
-        namespace(Text): namespace scope for helm release
+        name(str): An Idem name of the resource.
+        namespace(str, Optional): namespace scope for helm release.
+            Defaults to 'default' namespace, in case of value not provided in absent state.
+        resource_id(str, Optional): An identifier of the resource in the provider.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             idem-helm-release-test:
               helm.release.absent:
-              - name: idem-redis
-              - resource_id: idem-redis
-              - namespace: kube-system
+                - name: idem-redis
+                - resource_id: idem-redis
+                - namespace: kube-system
 
     """
-
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     before = None
     if resource_id:
         list_release_ret = await hub.exec.helm.release.list_releases(
             ctx, resource_id, namespace
         )
         if list_release_ret["ret"]:
@@ -369,29 +364,28 @@
         result["comment"] = hub.tool.helm.comment_utils.delete_comment(
             resource_type="helm.release", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
+    """list of helm releases in all namespaces.
 
-    list of helm releases in all namespaces.
-    Repository attributes and other flags are not being persisted as metadata by helm, it will not be set to any value by default.
+    Repository attributes and other flags are not being persisted as metadata by helm,
+    it will not be set to any value by default.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe helm.release
-    """
 
+    """
     list_release_ret = await hub.exec.helm.release.list_releases(ctx)
     if not list_release_ret["result"]:
         hub.log.debug(f"Could not describe helm release {list_release_ret['comment']}")
         return {}
 
     all_releases = list_release_ret["ret"]
     result = {}
```

### Comparing `idem-helm-0.2.1/idem_helm/tool/helm/command_utils.py` & `idem-helm-0.3.0/idem_helm/tool/helm/command_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/tool/helm/comment_utils.py` & `idem-helm-0.3.0/idem_helm/tool/helm/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/tool/helm/release_utils.py` & `idem-helm-0.3.0/idem_helm/tool/helm/release_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm/tool/helm/test_state_utils.py` & `idem-helm-0.3.0/idem_helm/tool/helm/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/idem_helm.egg-info/PKG-INFO` & `idem-helm-0.3.0/idem_helm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.2.1
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.2.1/idem_helm.egg-info/SOURCES.txt` & `idem-helm-0.3.0/idem_helm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-helm-0.2.1/setup.py` & `idem-helm-0.3.0/setup.py`

 * *Files identical despite different names*

