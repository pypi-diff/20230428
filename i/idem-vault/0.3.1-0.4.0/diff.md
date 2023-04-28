# Comparing `tmp/idem-vault-0.3.1.tar.gz` & `tmp/idem-vault-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-vault-0.3.1.tar", last modified: Thu Mar 23 14:16:40 2023, max compression
+gzip compressed data, was "idem-vault-0.4.0.tar", last modified: Fri Apr 28 14:32:27 2023, max compression
```

## Comparing `idem-vault-0.3.1.tar` & `idem-vault-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    11338 2023-03-23 14:16:26.000000 idem-vault-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4431 2023-03-23 14:16:40.348000 idem-vault-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3596 2023-03-23 14:16:26.000000 idem-vault-0.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.344000 idem-vault-0.3.1/idem_vault/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/acct/backend/
--rw-r--r--   0 root         (0) root         (0)     2915 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/acct/backend/vault.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/hvac/
--rw-r--r--   0 root         (0) root         (0)      571 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/exec/hvac/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     1257 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/source/
--rw-r--r--   0 root         (0) root         (0)     1221 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/source/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/states/vault/
--rw-r--r--   0 root         (0) root         (0)      173 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/states/vault/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/states/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     5505 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v1/key.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     8035 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault/tool/hvac/
--rw-r--r--   0 root         (0) root         (0)     1148 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/tool/hvac/client.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-03-23 14:16:26.000000 idem-vault-0.3.1/idem_vault/tool/hvac/resolve.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-23 14:16:39.000000 idem-vault-0.3.1/idem_vault/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 14:16:40.348000 idem-vault-0.3.1/idem_vault.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4431 2023-03-23 14:16:40.000000 idem-vault-0.3.1/idem_vault.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      664 2023-03-23 14:16:40.000000 idem-vault-0.3.1/idem_vault.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 14:16:40.000000 idem-vault-0.3.1/idem_vault.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-23 14:16:40.000000 idem-vault-0.3.1/idem_vault.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-23 14:16:40.000000 idem-vault-0.3.1/idem_vault.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-23 14:16:40.348000 idem-vault-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2715 2023-03-23 14:16:26.000000 idem-vault-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11338 2023-04-28 14:32:14.000000 idem-vault-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 14:32:27.894988 idem-vault-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-04-28 14:32:14.000000 idem-vault-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/acct/backend/
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/acct/backend/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/hvac/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/hvac/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/source/
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/source/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     5986 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/key.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     8035 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/hvac/
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/hvac/client.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/hvac/resolve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault/tool/vault/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-04-28 14:32:14.000000 idem-vault-0.4.0/idem_vault/tool/vault/secret.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:32:27.894988 idem-vault-0.4.0/idem_vault.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 14:32:27.000000 idem-vault-0.4.0/idem_vault.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:32:27.898988 idem-vault-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-28 14:32:14.000000 idem-vault-0.4.0/setup.py
```

### Comparing `idem-vault-0.3.1/LICENSE` & `idem-vault-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/PKG-INFO` & `idem-vault-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.3.1
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-vault-0.3.1/README.rst` & `idem-vault-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/acct/backend/vault.py` & `idem-vault-0.4.0/idem_vault/acct/backend/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/conf.py` & `idem-vault-0.4.0/idem_vault/conf.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/exec/hvac/init.py` & `idem-vault-0.4.0/idem_vault/exec/hvac/init.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v1/secret.py` & `idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v1/secret.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,12 +27,15 @@
     """
     result = dict(comment=[], ret=None, result=True)
     read_ret = await hub.exec.hvac.client.secrets.kv.v1.read_secret(ctx=ctx, path=path)
     if not read_ret["result"]:
         result["result"] = False
         result["comment"] += list(read_ret["comment"])
         return result
+    result["changes"] = hub.tool.vault.secret.calculate_changes(
+        new_state=read_ret["ret"]
+    )
     result["ret"] = {
         "path": path,
         "data": dict_tools.data.SafeNamespaceDict(read_ret["ret"]["data"]),
     }
     return result
```

### Comparing `idem-vault-0.3.1/idem_vault/exec/vault/secrets/kv_v2/secret.py` & `idem-vault-0.4.0/idem_vault/exec/vault/secrets/kv_v2/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/source/vault.py` & `idem-vault-0.4.0/idem_vault/source/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v1/key.py` & `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/key.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,25 +79,34 @@
             f"vault.secrets.kv_v1.key '{name}' nothing to be updated.",
         )
         return result
 
     if ctx.get("test", False):
         result["new_state"] = {"name": name, "path": path, "key": key, "value": value}
         result["comment"] = (f"Would {action} vault.secrets.kv_v1.key '{key}'.",)
+        # calculating changes here to show keys that would be updated
+        result["changes"] = hub.tool.vault.secret.calculate_changes(
+            old_state={"data": result["old_state"]},
+            new_state={"data": result["new_state"]},
+        )
         return result
 
     data_to_update[key] = value
     write_ret = await hub.exec.hvac.client.secrets.kv.v1.create_or_update_secret(
         ctx=ctx, path=path, secret=data_to_update
     )
     if not write_ret["result"]:
         result["result"] = False
         result["comment"] = write_ret["comment"]
         return result
     result["new_state"] = {"name": name, "path": path, "key": key, "value": value}
+    # calculating changes here to show keys that would be updated
+    result["changes"] = hub.tool.vault.secret.calculate_changes(
+        old_state={"data": result["old_state"]}, new_state={"data": result["new_state"]}
+    )
     if result["old_state"] is None or "create" == action:
         result["comment"] = (f"Created vault.secrets.kv_v1.key '{key}'.",)
     else:
         result["comment"] = (f"Updated vault.secrets.kv_v1.key '{key}'.",)
     return result
```

### Comparing `idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v1/secret.py` & `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v2/secret.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,211 +1,226 @@
 import copy
-import json
-from json.decoder import JSONDecodeError
 from typing import Dict
 
 import dict_tools.data
 
 
 async def present(
     hub,
     ctx,
     name: str,
     path: str,
-    data: str or Dict,
+    data: Dict,
     disable_read: bool = False,
 ) -> Dict:
     """
-    Creates or update a secret stored with Vault KV_v1 secret engine.
+    Creates or update a secret stored with Vault KV_v2 secret engine.
 
     Args:
         name(string): An Idem name of the resource.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
-        data(string or dict, optional): Data to be written in the format of a JSON string or a JSON object that can be stringfied.
+        data(string, optional): Data to be written in the format of a JSON object.
         disable_read(bool, optional): Set this field to True if the vault authentication does not have read access.
             However, if the value is True, this Idem state operation is not idempotent, and Idem state comment output
              will always assume it is a "create" operation. Defaults to False.
 
     Request Syntax:
         [vault-secret-name]:
-          vault.secrets.kv_v1.secret.present:
+          vault.secrets.kv_v2.secret.present:
           - path: 'string'
-          - data: 'string or dict'
+          - data: 'string'
           - disable_read: 'boolean'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             my-secret:
-              vault.secrets.kv_v1.secret.present:
+              vault.secrets.kv_v2.secret.present:
                 - path: secret/test
                 - data: '{"my-birthday": "2012-10-17"}'
     """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": (),
     }
-    if isinstance(data, str):
-        try:
-            data = json.loads(data)
-        except JSONDecodeError as e:
-            result[
-                "comment"
-            ] = f"Fail to load data {data} as json object: {e.__class__.__name__}: {e}"
-            result["result"] = False
-            return result
     # data is converted to SafeNamespaceDict to avoid it being converted to string and printed to console.
     data = dict_tools.data.SafeNamespaceDict(data)
     if not disable_read:
-        read_ret = await hub.exec.hvac.client.secrets.kv.v1.read_secret(
+        read_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_version(
             ctx=ctx, path=path
         )
         if not read_ret["result"]:
             if "InvalidPath" not in str(read_ret["comment"]):
                 result["result"] = False
                 result["comment"] = read_ret["comment"]
                 return result
         else:
             result["old_state"] = {
                 "name": name,
                 "path": path,
-                "data": dict_tools.data.SafeNamespaceDict(read_ret["ret"]["data"]),
+                "data": dict_tools.data.SafeNamespaceDict(
+                    read_ret["ret"]["data"]["data"]
+                ),
             }
     else:
-        hub.log.debug(f"vault.secrets.kv_v1.secret '{name}' read has been disabled.")
+        hub.log.debug(f"vault.secrets.kv_v2.secret '{name}' read has been disabled.")
         result["comment"] = (
-            f"vault.secrets.kv_v1.secret '{name}' read has been disabled.",
+            f"vault.secrets.kv_v2.secret '{name}' read has been disabled.",
         )
     if (result["old_state"] is not None) and result["old_state"]["data"] == data:
         result["comment"] = result["comment"] + (
-            f"vault.secrets.kv_v1.secret '{name}' has no property need to be updated.",
+            f"vault.secrets.kv_v2.secret '{name}' has no property need to be updated.",
         )
-        result["new_state"] = copy.deepcopy(result["old_state"])
         return result
     elif result["old_state"] is None:
         if ctx.get("test", False):
-            result["comment"] = (f"Would create vault.secrets.kv_v1.secret '{name}'.",)
+            result["comment"] = (f"Would create vault.secrets.kv_v2.secret '{name}'.",)
             result["new_state"] = {"name": name, "path": path, "data": data}
             return result
     else:
         if ctx.get("test", False):
-            result["comment"] = (f"Would update vault.secrets.kv_v1.secret '{name}'.",)
+            result["comment"] = (f"Would update vault.secrets.kv_v2.secret '{name}'.",)
             result["new_state"] = {"name": name, "path": path, "data": data}
             return result
 
-    write_ret = await hub.exec.hvac.client.secrets.kv.v1.create_or_update_secret(
+    write_ret = await hub.exec.hvac.client.secrets.kv.v2.create_or_update_secret(
         ctx=ctx, path=path, secret=data
     )
     if not write_ret["result"]:
         result["result"] = False
         result["comment"] = write_ret["comment"]
         return result
     result["new_state"] = {"name": name, "path": path, "data": data}
     if result["old_state"] is None:
-        result["comment"] = (f"Created vault.secrets.kv_v1.secret '{name}'.",)
+        result["comment"] = (f"Created vault.secrets.kv_v2.secret '{name}'.",)
     else:
-        result["comment"] = (f"Updated vault.secrets.kv_v1.secret '{name}'.",)
+        result["comment"] = (f"Updated vault.secrets.kv_v2.secret '{name}'.",)
     return result
 
 
 async def absent(
-    hub,
-    ctx,
-    name: str,
-    path: str,
+    hub, ctx, name: str, path: str, delete_all_versions: bool = False
 ) -> Dict:
     """
-    Delete a secret stored with Vault KV_v1 secret engine.
+    Delete a secret stored with Vault KV_v2 secret engine.
 
     Args:
         name(string): An Idem name of the resource.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
+        delete_all_versions(bool, optional): Set this field to True if the vault authentication does not have read access.
+            However, if the value is True, this Idem state operation is not idempotent. Defaults to False.
 
     Request Syntax:
         [vault-secret-name]:
-          vault.secrets.kv_v1.secret.absent:
+          vault.secrets.kv_v2.secret.absent:
           - path: 'string'
+          - delete_all_versions: 'boolean'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             my-secret:
-              vault.secrets.kv_v1.secret.absent:
+              vault.secrets.kv_v2.secret.absent:
                 - path: secret/test
     """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": (),
     }
-    read_ret = await hub.exec.hvac.client.secrets.kv.v1.read_secret(ctx=ctx, path=path)
-
+    read_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_version(
+        ctx=ctx, path=path
+    )
     if not read_ret["result"]:
         if "InvalidPath" in str(read_ret["comment"]):
             result["comment"] = (
-                f"vault.secrets.kv_v1.secret '{name}' is already absent.",
+                f"vault.secrets.kv_v2.secret '{name}' is already absent.",
             )
         else:
             result["result"] = False
             result["comment"] = read_ret["comment"]
         return result
 
     # "data" is not populated to reduce data exposure.
     result["old_state"] = {"name": name, "path": path}
+    delete_version = [read_ret["ret"]["data"]["metadata"]["version"]]
+    if delete_all_versions:
+        version_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_metadata(
+            ctx=ctx, path=path
+        )
+        if not version_ret["result"]:
+            result["result"] = False
+            result["comment"] = version_ret["comment"]
+            return result
+        delete_version = list(version_ret["ret"]["data"]["versions"].keys())
     if ctx.get("test", False):
-        result["comment"] = (f"Would delete vault.secrets.kv_v1.secret '{name}'.",)
+        if delete_all_versions:
+            result["comment"] = (
+                f"Would delete vault.secrets.kv_v2.secret '{name}' all versions.",
+            )
+        else:
+            result["comment"] = (f"Would delete vault.secrets.kv_v2.secret '{name}'.",)
         return result
-    delete_ret = await hub.exec.hvac.client.secrets.kv.v1.delete_secret(
-        ctx=ctx, path=path
+    delete_ret = await hub.exec.hvac.client.secrets.kv.v2.destroy_secret_versions(
+        ctx=ctx, path=path, versions=delete_version
     )
     if not delete_ret["result"]:
         result["result"] = False
         result["comment"] = read_ret["comment"]
+    elif delete_all_versions:
+        result["comment"] = (
+            f"Deleted vault.secrets.kv_v2.secret '{name}' all versions.",
+        )
     else:
-        result["comment"] = (f"Deleted vault.secrets.kv_v1.secret '{name}'.",)
+        result["comment"] = (f"Deleted vault.secrets.kv_v2.secret '{name}'.",)
     return result
 
 
-async def search(hub, ctx, name, path: str) -> Dict:
+async def search(hub, ctx, name, path: str, version: int = None) -> Dict:
     """
-    KV_v1 secret data-source.
+    KV_v2 secret data-source.
 
     Args:
         name(string): The name of the Idem state.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
+        version(int, optional): The version of the secret to read. If not specified, the latest version will be used.
 
     Request Syntax:
         [Idem-state-name]:
-          vault.secrets.kv_v1.secret.search:
+          vault.secrets.kv_v2.secret.search:
           - path: 'string'
+          - version: 'int'
 
         Examples:
 
             my-secret:
-              vault.secrets.kv_v1.secret.search:
+              vault.secrets.kv_v2.secret.search:
                 - path: secret/test
+                - version: 1
     """
     hub.log.warning(
-        f"vault.secrets.kv_v1.secret.search '{name}' state has been deprecated. Please use exec.run with vault.secrets.kv_v1.secret.get instead."
+        f"vault.secrets.kv_v2.secret.search '{name}' state has been deprecated. Please use exec.run with vault.secrets.kv_v2.secret.get instead."
     )
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
-    ret = await hub.exec.vault.secrets.kv_v1.secret.get(ctx=ctx, path=path)
+    ret = await hub.exec.vault.secrets.kv_v2.secret.get(
+        ctx=ctx, path=path, version=version
+    )
     result["result"] = ret["result"]
     result["comment"] = ret["comment"]
     if result["result"]:
         result["old_state"] = ret["ret"]
         result["old_state"]["name"] = name
         # Populate both "old_state" and "new_state" with the same data
         result["new_state"] = copy.deepcopy(result["old_state"])
```

### Comparing `idem-vault-0.3.1/idem_vault/states/vault/secrets/kv_v2/secret.py` & `idem-vault-0.4.0/idem_vault/states/vault/secrets/kv_v1/secret.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,226 +1,223 @@
 import copy
+import json
+from json.decoder import JSONDecodeError
 from typing import Dict
 
 import dict_tools.data
 
 
 async def present(
     hub,
     ctx,
     name: str,
     path: str,
-    data: Dict,
+    data: str or Dict,
     disable_read: bool = False,
 ) -> Dict:
     """
-    Creates or update a secret stored with Vault KV_v2 secret engine.
+    Creates or update a secret stored with Vault KV_v1 secret engine.
 
     Args:
         name(string): An Idem name of the resource.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
-        data(string, optional): Data to be written in the format of a JSON object.
+        data(string or dict, optional): Data to be written in the format of a JSON string or a JSON object that can be stringfied.
         disable_read(bool, optional): Set this field to True if the vault authentication does not have read access.
             However, if the value is True, this Idem state operation is not idempotent, and Idem state comment output
              will always assume it is a "create" operation. Defaults to False.
 
     Request Syntax:
         [vault-secret-name]:
-          vault.secrets.kv_v2.secret.present:
+          vault.secrets.kv_v1.secret.present:
           - path: 'string'
-          - data: 'string'
+          - data: 'string or dict'
           - disable_read: 'boolean'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             my-secret:
-              vault.secrets.kv_v2.secret.present:
+              vault.secrets.kv_v1.secret.present:
                 - path: secret/test
                 - data: '{"my-birthday": "2012-10-17"}'
     """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": (),
     }
+    if isinstance(data, str):
+        try:
+            data = json.loads(data)
+        except JSONDecodeError as e:
+            result[
+                "comment"
+            ] = f"Fail to load data {data} as json object: {e.__class__.__name__}: {e}"
+            result["result"] = False
+            return result
     # data is converted to SafeNamespaceDict to avoid it being converted to string and printed to console.
     data = dict_tools.data.SafeNamespaceDict(data)
     if not disable_read:
-        read_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_version(
+        read_ret = await hub.exec.hvac.client.secrets.kv.v1.read_secret(
             ctx=ctx, path=path
         )
         if not read_ret["result"]:
             if "InvalidPath" not in str(read_ret["comment"]):
                 result["result"] = False
                 result["comment"] = read_ret["comment"]
                 return result
         else:
             result["old_state"] = {
                 "name": name,
                 "path": path,
-                "data": dict_tools.data.SafeNamespaceDict(
-                    read_ret["ret"]["data"]["data"]
-                ),
+                "data": dict_tools.data.SafeNamespaceDict(read_ret["ret"]["data"]),
             }
     else:
-        hub.log.debug(f"vault.secrets.kv_v2.secret '{name}' read has been disabled.")
+        hub.log.debug(f"vault.secrets.kv_v1.secret '{name}' read has been disabled.")
         result["comment"] = (
-            f"vault.secrets.kv_v2.secret '{name}' read has been disabled.",
+            f"vault.secrets.kv_v1.secret '{name}' read has been disabled.",
         )
     if (result["old_state"] is not None) and result["old_state"]["data"] == data:
         result["comment"] = result["comment"] + (
-            f"vault.secrets.kv_v2.secret '{name}' has no property need to be updated.",
+            f"vault.secrets.kv_v1.secret '{name}' has no property need to be updated.",
         )
+        result["new_state"] = copy.deepcopy(result["old_state"])
         return result
     elif result["old_state"] is None:
         if ctx.get("test", False):
-            result["comment"] = (f"Would create vault.secrets.kv_v2.secret '{name}'.",)
+            result["comment"] = (f"Would create vault.secrets.kv_v1.secret '{name}'.",)
             result["new_state"] = {"name": name, "path": path, "data": data}
+            # calculating changes here to show keys that would be updated
+            result["changes"] = hub.tool.vault.secret.calculate_changes(
+                old_state=result["old_state"], new_state=result["new_state"]
+            )
             return result
     else:
         if ctx.get("test", False):
-            result["comment"] = (f"Would update vault.secrets.kv_v2.secret '{name}'.",)
+            result["comment"] = (f"Would update vault.secrets.kv_v1.secret '{name}'.",)
             result["new_state"] = {"name": name, "path": path, "data": data}
+            # calculating changes here to show keys that would be updated
+            result["changes"] = hub.tool.vault.secret.calculate_changes(
+                old_state=result["old_state"], new_state=result["new_state"]
+            )
             return result
 
-    write_ret = await hub.exec.hvac.client.secrets.kv.v2.create_or_update_secret(
+    write_ret = await hub.exec.hvac.client.secrets.kv.v1.create_or_update_secret(
         ctx=ctx, path=path, secret=data
     )
     if not write_ret["result"]:
         result["result"] = False
         result["comment"] = write_ret["comment"]
         return result
     result["new_state"] = {"name": name, "path": path, "data": data}
+    # calculating changes here to show keys that are updated
+    result["changes"] = hub.tool.vault.secret.calculate_changes(
+        old_state=result["old_state"], new_state=result["new_state"]
+    )
     if result["old_state"] is None:
-        result["comment"] = (f"Created vault.secrets.kv_v2.secret '{name}'.",)
+        result["comment"] = (f"Created vault.secrets.kv_v1.secret '{name}'.",)
     else:
-        result["comment"] = (f"Updated vault.secrets.kv_v2.secret '{name}'.",)
+        result["comment"] = (f"Updated vault.secrets.kv_v1.secret '{name}'.",)
     return result
 
 
 async def absent(
-    hub, ctx, name: str, path: str, delete_all_versions: bool = False
+    hub,
+    ctx,
+    name: str,
+    path: str,
 ) -> Dict:
     """
-    Delete a secret stored with Vault KV_v2 secret engine.
+    Delete a secret stored with Vault KV_v1 secret engine.
 
     Args:
         name(string): An Idem name of the resource.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
-        delete_all_versions(bool, optional): Set this field to True if the vault authentication does not have read access.
-            However, if the value is True, this Idem state operation is not idempotent. Defaults to False.
 
     Request Syntax:
         [vault-secret-name]:
-          vault.secrets.kv_v2.secret.absent:
+          vault.secrets.kv_v1.secret.absent:
           - path: 'string'
-          - delete_all_versions: 'boolean'
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
         .. code-block:: sls
 
             my-secret:
-              vault.secrets.kv_v2.secret.absent:
+              vault.secrets.kv_v1.secret.absent:
                 - path: secret/test
     """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": (),
     }
-    read_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_version(
-        ctx=ctx, path=path
-    )
+    read_ret = await hub.exec.hvac.client.secrets.kv.v1.read_secret(ctx=ctx, path=path)
+
     if not read_ret["result"]:
         if "InvalidPath" in str(read_ret["comment"]):
             result["comment"] = (
-                f"vault.secrets.kv_v2.secret '{name}' is already absent.",
+                f"vault.secrets.kv_v1.secret '{name}' is already absent.",
             )
         else:
             result["result"] = False
             result["comment"] = read_ret["comment"]
         return result
 
     # "data" is not populated to reduce data exposure.
     result["old_state"] = {"name": name, "path": path}
-    delete_version = [read_ret["ret"]["data"]["metadata"]["version"]]
-    if delete_all_versions:
-        version_ret = await hub.exec.hvac.client.secrets.kv.v2.read_secret_metadata(
-            ctx=ctx, path=path
-        )
-        if not version_ret["result"]:
-            result["result"] = False
-            result["comment"] = version_ret["comment"]
-            return result
-        delete_version = list(version_ret["ret"]["data"]["versions"].keys())
     if ctx.get("test", False):
-        if delete_all_versions:
-            result["comment"] = (
-                f"Would delete vault.secrets.kv_v2.secret '{name}' all versions.",
-            )
-        else:
-            result["comment"] = (f"Would delete vault.secrets.kv_v2.secret '{name}'.",)
+        result["comment"] = (f"Would delete vault.secrets.kv_v1.secret '{name}'.",)
         return result
-    delete_ret = await hub.exec.hvac.client.secrets.kv.v2.destroy_secret_versions(
-        ctx=ctx, path=path, versions=delete_version
+    delete_ret = await hub.exec.hvac.client.secrets.kv.v1.delete_secret(
+        ctx=ctx, path=path
     )
     if not delete_ret["result"]:
         result["result"] = False
         result["comment"] = read_ret["comment"]
-    elif delete_all_versions:
-        result["comment"] = (
-            f"Deleted vault.secrets.kv_v2.secret '{name}' all versions.",
-        )
     else:
-        result["comment"] = (f"Deleted vault.secrets.kv_v2.secret '{name}'.",)
+        result["comment"] = (f"Deleted vault.secrets.kv_v1.secret '{name}'.",)
     return result
 
 
-async def search(hub, ctx, name, path: str, version: int = None) -> Dict:
+async def search(hub, ctx, name, path: str) -> Dict:
     """
-    KV_v2 secret data-source.
+    KV_v1 secret data-source.
 
     Args:
         name(string): The name of the Idem state.
         path(string): The full logical path to write the data. This should be prefixed 'with secret/'.
-        version(int, optional): The version of the secret to read. If not specified, the latest version will be used.
 
     Request Syntax:
         [Idem-state-name]:
-          vault.secrets.kv_v2.secret.search:
+          vault.secrets.kv_v1.secret.search:
           - path: 'string'
-          - version: 'int'
 
         Examples:
 
             my-secret:
-              vault.secrets.kv_v2.secret.search:
+              vault.secrets.kv_v1.secret.search:
                 - path: secret/test
-                - version: 1
     """
     hub.log.warning(
-        f"vault.secrets.kv_v2.secret.search '{name}' state has been deprecated. Please use exec.run with vault.secrets.kv_v2.secret.get instead."
+        f"vault.secrets.kv_v1.secret.search '{name}' state has been deprecated. Please use exec.run with vault.secrets.kv_v1.secret.get instead."
     )
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
-    ret = await hub.exec.vault.secrets.kv_v2.secret.get(
-        ctx=ctx, path=path, version=version
-    )
+    ret = await hub.exec.vault.secrets.kv_v1.secret.get(ctx=ctx, path=path)
     result["result"] = ret["result"]
     result["comment"] = ret["comment"]
     if result["result"]:
         result["old_state"] = ret["ret"]
         result["old_state"]["name"] = name
         # Populate both "old_state" and "new_state" with the same data
         result["new_state"] = copy.deepcopy(result["old_state"])
```

### Comparing `idem-vault-0.3.1/idem_vault/tool/hvac/client.py` & `idem-vault-0.4.0/idem_vault/tool/hvac/client.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault/tool/hvac/resolve.py` & `idem-vault-0.4.0/idem_vault/tool/hvac/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.3.1/idem_vault.egg-info/PKG-INFO` & `idem-vault-0.4.0/idem_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.3.1
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-vault-0.3.1/idem_vault.egg-info/SOURCES.txt` & `idem-vault-0.4.0/idem_vault.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 idem_vault/exec/vault/secrets/kv_v2/secret.py
 idem_vault/source/vault.py
 idem_vault/states/vault/init.py
 idem_vault/states/vault/secrets/kv_v1/key.py
 idem_vault/states/vault/secrets/kv_v1/secret.py
 idem_vault/states/vault/secrets/kv_v2/secret.py
 idem_vault/tool/hvac/client.py
-idem_vault/tool/hvac/resolve.py
+idem_vault/tool/hvac/resolve.py
+idem_vault/tool/vault/secret.py
```

### Comparing `idem-vault-0.3.1/setup.py` & `idem-vault-0.4.0/setup.py`

 * *Files identical despite different names*

