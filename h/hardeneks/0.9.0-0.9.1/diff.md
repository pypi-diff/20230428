# Comparing `tmp/hardeneks-0.9.0.tar.gz` & `tmp/hardeneks-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardeneks-0.9.0.tar", max compression
+gzip compressed data, was "hardeneks-0.9.1.tar", max compression
```

## Comparing `hardeneks-0.9.0.tar` & `hardeneks-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      927 2023-03-31 18:08:44.740887 hardeneks-0.9.0/LICENSE
--rw-r--r--   0        0        0     6552 2023-03-31 18:08:44.740887 hardeneks-0.9.0/README.md
--rw-r--r--   0        0        0     7046 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
--rw-r--r--   0        0        0     9687 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/reliability/__init__.py
--rw-r--r--   0        0        0     1525 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/scalability/__init__.py
--rw-r--r--   0        0        0     2112 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/scalability/control_plane.py
--rw-r--r--   0        0        0      551 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/scalability/skipped.json
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/__init__.py
--rw-r--r--   0        0        0      874 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/detective_controls.py
--rw-r--r--   0        0        0     3161 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/encryption_secrets.py
--rw-r--r--   0        0        0     5409 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/iam.py
--rw-r--r--   0        0        0     1009 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/image_security.py
--rw-r--r--   0        0        0     2374 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/infrastructure_security.py
--rw-r--r--   0        0        0      760 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/multi_tenancy.py
--rw-r--r--   0        0        0     2558 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/network_security.py
--rw-r--r--   0        0        0     1284 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/cluster_wide/security/pod_security.py
--rw-r--r--   0        0        0     2731 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/config.yaml
--rw-r--r--   0        0        0      728 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/harden.py
--rw-r--r--   0        0        0      544 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/helpers.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/reliability/__init__.py
--rw-r--r--   0        0        0     5859 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/reliability/applications.py
--rw-r--r--   0        0        0        0 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/encryption_secrets.py
--rw-r--r--   0        0        0     8011 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/iam.py
--rw-r--r--   0        0        0     1370 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/network_security.py
--rw-r--r--   0        0        0     5259 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/pod_security.py
--rw-r--r--   0        0        0     1685 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/namespace_based/security/runtime_security.py
--rw-r--r--   0        0        0     2289 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/resources.py
--rw-r--r--   0        0        0     1412 2023-03-31 18:08:44.764887 hardeneks-0.9.0/hardeneks/rules.py
--rw-r--r--   0        0        0     1005 2023-03-31 18:08:44.764887 hardeneks-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7024 1970-01-01 00:00:00.000000 hardeneks-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      927 2023-04-28 16:06:51.608430 hardeneks-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6610 2023-04-28 16:06:51.608430 hardeneks-0.9.1/README.md
+-rw-r--r--   0        0        0     7046 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/__init__.py
+-rw-r--r--   0        0        0     9687 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/reliability/__init__.py
+-rw-r--r--   0        0        0     1525 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/__init__.py
+-rw-r--r--   0        0        0     2112 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/control_plane.py
+-rw-r--r--   0        0        0      551 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/scalability/skipped.json
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/detective_controls.py
+-rw-r--r--   0        0        0     3161 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/encryption_secrets.py
+-rw-r--r--   0        0        0     5409 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/iam.py
+-rw-r--r--   0        0        0     1009 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/image_security.py
+-rw-r--r--   0        0        0     2374 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/infrastructure_security.py
+-rw-r--r--   0        0        0      760 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/multi_tenancy.py
+-rw-r--r--   0        0        0     2558 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/network_security.py
+-rw-r--r--   0        0        0     1222 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/cluster_wide/security/pod_security.py
+-rw-r--r--   0        0        0     2731 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/config.yaml
+-rw-r--r--   0        0        0      728 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/harden.py
+-rw-r--r--   0        0        0      544 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/reliability/__init__.py
+-rw-r--r--   0        0        0     5859 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/reliability/applications.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/__init__.py
+-rw-r--r--   0        0        0     1305 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/encryption_secrets.py
+-rw-r--r--   0        0        0     8011 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/iam.py
+-rw-r--r--   0        0        0     1370 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/network_security.py
+-rw-r--r--   0        0        0     5259 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/pod_security.py
+-rw-r--r--   0        0        0     1685 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/namespace_based/security/runtime_security.py
+-rw-r--r--   0        0        0     2289 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/resources.py
+-rw-r--r--   0        0        0     1412 2023-04-28 16:06:51.616430 hardeneks-0.9.1/hardeneks/rules.py
+-rw-r--r--   0        0        0     1005 2023-04-28 16:06:51.616430 hardeneks-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 hardeneks-0.9.1/PKG-INFO
```

### Comparing `hardeneks-0.9.0/LICENSE` & `hardeneks-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/README.md` & `hardeneks-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 * `--region TEXT`: AWS region of the cluster. Ex: us-east-1
 * `--context TEXT`: K8s context
 * `--cluster TEXT`: EKS Cluster name
 * `--namespace TEXT`: Namespace to be checked (default is all namespaces)
 * `--config TEXT`: Path to a hardeneks config file
 * `--export-txt TEXT`: Export the report in txt format
 * `--export-html TEXT`: Export the report in html format
+* `--export-json TEXT`: Export the report in json format
 * `--insecure-skip-tls-verify`: Skip TLS verification
 * `--help`: Show this message and exit.
 
 
 - <b>K8S_CONTEXT<b> 
   
     You can get the contexts by running:
```

### Comparing `hardeneks-0.9.0/hardeneks/__init__.py` & `hardeneks-0.9.1/hardeneks/__init__.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/cluster_autoscaling/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/reliability/applications.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/scalability/control_plane.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/scalability/control_plane.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/scalability/skipped.json` & `hardeneks-0.9.1/hardeneks/cluster_wide/scalability/skipped.json`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/detective_controls.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/detective_controls.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/encryption_secrets.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/iam.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/iam.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/image_security.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/image_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/infrastructure_security.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/infrastructure_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/multi_tenancy.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/multi_tenancy.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/network_security.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/cluster_wide/security/pod_security.py` & `hardeneks-0.9.1/hardeneks/cluster_wide/security/pod_security.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,22 +11,24 @@
     message = "Namespaces should have psa modes."
     url = "https://aws.github.io/aws-eks-best-practices/security/docs/pods/#pod-security-standards-pss-and-pod-security-admission-psa"
 
     def check(self, resources: Resources):
         offenders = []
 
         namespaces = kubernetes.client.CoreV1Api().list_namespace().items
+        psa_labels = [
+            "pod-security.kubernetes.io/enforce",
+            "pod-security.kubernetes.io/warn",
+            "pod-security.kubernetes.io/audit",
+        ]
+
         for namespace in namespaces:
-            if namespace.metadata.name not in resources.namespaces:
+            if namespace.metadata.name in resources.namespaces:
                 labels = namespace.metadata.labels.keys()
-                if "pod-security.kubernetes.io/enforce" not in labels:
-                    offenders.append(namespace.metadata.name)
-                elif "pod-security.kubernetes.io/warn" not in labels:
-                    offenders.append(namespace.metadata.name)
-                elif not labels:
+                if not any(i in labels for i in psa_labels):
                     offenders.append(namespace.metadata.name)
 
         self.result = Result(status=True, resource_type="Namespace")
         if offenders:
             self.result = Result(
                 status=False, resource_type="Namespace", resources=offenders
             )
```

### Comparing `hardeneks-0.9.0/hardeneks/config.yaml` & `hardeneks-0.9.1/hardeneks/config.yaml`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/harden.py` & `hardeneks-0.9.1/hardeneks/harden.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/helpers.py` & `hardeneks-0.9.1/hardeneks/helpers.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/reliability/applications.py` & `hardeneks-0.9.1/hardeneks/namespace_based/reliability/applications.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/security/encryption_secrets.py` & `hardeneks-0.9.1/hardeneks/namespace_based/security/encryption_secrets.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/security/iam.py` & `hardeneks-0.9.1/hardeneks/namespace_based/security/iam.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/security/network_security.py` & `hardeneks-0.9.1/hardeneks/namespace_based/security/network_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/security/pod_security.py` & `hardeneks-0.9.1/hardeneks/namespace_based/security/pod_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/namespace_based/security/runtime_security.py` & `hardeneks-0.9.1/hardeneks/namespace_based/security/runtime_security.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/resources.py` & `hardeneks-0.9.1/hardeneks/resources.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/hardeneks/rules.py` & `hardeneks-0.9.1/hardeneks/rules.py`

 * *Files identical despite different names*

### Comparing `hardeneks-0.9.0/pyproject.toml` & `hardeneks-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardeneks"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Doruk Ozturk <dozturk@amazon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typer = {extras = ["all"], version = "^0.6.1"}
@@ -37,15 +37,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.9.0"
+version = "0.9.1"
 version_files = [
   "pyproject.toml:[tool.commitizen]\nversion",
   "pyproject.toml:[tool.poetry]\nname = \"commitizen\"\nversion",
   "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 [build-system]
```

### Comparing `hardeneks-0.9.0/PKG-INFO` & `hardeneks-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardeneks
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Doruk Ozturk
 Author-email: dozturk@amazon.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -50,14 +50,15 @@
 * `--region TEXT`: AWS region of the cluster. Ex: us-east-1
 * `--context TEXT`: K8s context
 * `--cluster TEXT`: EKS Cluster name
 * `--namespace TEXT`: Namespace to be checked (default is all namespaces)
 * `--config TEXT`: Path to a hardeneks config file
 * `--export-txt TEXT`: Export the report in txt format
 * `--export-html TEXT`: Export the report in html format
+* `--export-json TEXT`: Export the report in json format
 * `--insecure-skip-tls-verify`: Skip TLS verification
 * `--help`: Show this message and exit.
 
 
 - <b>K8S_CONTEXT<b> 
   
     You can get the contexts by running:
```

