# Comparing `tmp/idem-k8s-0.5.0.tar.gz` & `tmp/idem-k8s-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-k8s-0.5.0.tar", last modified: Mon Mar 20 15:14:52 2023, max compression
+gzip compressed data, was "idem-k8s-0.6.0.tar", last modified: Fri Apr 28 14:35:30 2023, max compression
```

## Comparing `idem-k8s-0.5.0.tar` & `idem-k8s-0.6.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    11336 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7122 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6284 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/acct/k8s/
--rw-r--r--   0 root         (0) root         (0)      547 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/acct/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/autogen/k8s/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/autogen/k8s/init.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/autogen/k8s/openapi_spec_parser.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/autogen/k8s/plugin.py
--rw-r--r--   0 root         (0) root         (0)    10897 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/autogen/k8s/template.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/autogen/k8s/type.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     3837 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)     4356 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/exec/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/exec/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/exec/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     4595 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/states/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)    12998 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/apps/v1/daemon_set.py
--rw-r--r--   0 root         (0) root         (0)    13245 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/apps/v1/deployment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)    10043 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/config_map.py
--rw-r--r--   0 root         (0) root         (0)     9309 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/namespace.py
--rw-r--r--   0 root         (0) root         (0)    10778 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     9695 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/secret.py
--rw-r--r--   0 root         (0) root         (0)    10851 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/service.py
--rw-r--r--   0 root         (0) root         (0)    10289 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/service_account.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)     8549 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py
--rw-r--r--   0 root         (0) root         (0)     9245 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
--rw-r--r--   0 root         (0) root         (0)     9819 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/role_binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/states/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/states/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)    10533 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/k8s/apiregistration_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      653 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/v1/
--rw-r--r--   0 root         (0) root         (0)      905 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     3051 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/client.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/
--rw-r--r--   0 root         (0) root         (0)      714 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/secret_utils.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py
--rw-r--r--   0 root         (0) root         (0)      845 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/service_utils.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/marshaller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/
--rw-r--r--   0 root         (0) root         (0)      692 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/resolve.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s/tool/k8s/storage_k8s_io/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/idem_k8s/tool/k8s/storage_k8s_io/v1/
--rw-r--r--   0 root         (0) root         (0)      848 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/idem_k8s/tool/k8s/waiter_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 15:14:52.710814 idem-k8s-0.5.0/idem_k8s.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7122 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2225 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-20 15:14:52.000000 idem-k8s-0.5.0/idem_k8s.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-20 15:14:52.714814 idem-k8s-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2783 2023-03-20 15:14:39.000000 idem-k8s-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)    11336 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6284 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/acct/k8s/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/acct/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/autogen/k8s/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/init.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/openapi_spec_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/plugin.py
+-rw-r--r--   0 root         (0) root         (0)    10897 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/template.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/autogen/k8s/type.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     3837 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     4595 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)    13115 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/daemon_set.py
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/deployment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)    10073 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/config_map.py
+-rw-r--r--   0 root         (0) root         (0)     9167 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     9756 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/secret.py
+-rw-r--r--   0 root         (0) root         (0)    11114 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service.py
+-rw-r--r--   0 root         (0) root         (0)    10444 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service_account.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)     8356 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py
+-rw-r--r--   0 root         (0) root         (0)     9040 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     9953 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/role_binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)    10373 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/client.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/secret_utils.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py
+-rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/marshaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/resolve.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/idem_k8s/tool/k8s/waiter_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:30.649580 idem-k8s-0.6.0/idem_k8s.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-28 14:35:30.000000 idem-k8s-0.6.0/idem_k8s.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:35:30.653580 idem-k8s-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-04-28 14:35:16.000000 idem-k8s-0.6.0/setup.py
```

### Comparing `idem-k8s-0.5.0/LICENSE` & `idem-k8s-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/PKG-INFO` & `idem-k8s-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 0.5.0
+Version: 0.6.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-k8s-0.5.0/README.rst` & `idem-k8s-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/acct/k8s/init.py` & `idem-k8s-0.6.0/idem_k8s/acct/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/autogen/k8s/init.py` & `idem-k8s-0.6.0/idem_k8s/autogen/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/autogen/k8s/openapi_spec_parser.py` & `idem-k8s-0.6.0/idem_k8s/autogen/k8s/openapi_spec_parser.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/autogen/k8s/plugin.py` & `idem-k8s-0.6.0/idem_k8s/autogen/k8s/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/autogen/k8s/template.py` & `idem-k8s-0.6.0/idem_k8s/autogen/k8s/template.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/autogen/k8s/type.py` & `idem-k8s-0.6.0/idem_k8s/autogen/k8s/type.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-0.6.0/idem_k8s/exec/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/exec/k8s/core/v1/service.py` & `idem-k8s-0.6.0/idem_k8s/exec/k8s/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/exec/k8s/init.py` & `idem-k8s-0.6.0/idem_k8s/exec/k8s/init.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py` & `idem-k8s-0.6.0/idem_k8s/exec/k8s/rbac/v1/role_binding.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/apiregistration_k8s_io/v1/api_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,35 +55,34 @@
             An Idem name of the resource.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         metadata(dict):
             Standard object's metadata.
-            More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
 
         spec(dict):
             Spec contains information for locating and communicating with a server.
+            More info: `Kubernetes spec reference <https://github.com/kubernetes/community/blob/master/contributors/devel/sig-architecture/api-conventions.md#spec-and-status>`_
 
     Request Syntax:
-
         .. code-block:: sls
 
-            [api_service-name]:
+           [api_service-name]:
               k8s.apiregistration_k8s_io.v1.api_service.present:
                 - name: 'string'
                 - metadata: Dict
                 - spec: Dict
                 - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.apiregistration_k8s_io.v1.api_service.present:
                 - name: 'test-api-service'
                 - metadata:
                     labels:
@@ -96,15 +95,14 @@
                     service:
                       name: metrics-server
                       namespace: kube-system
                     version: v1beta1
                     version_priority: 100
 
     """
-
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Check for existing api_service by name
     before = None
     if resource_id:
         api_service = await hub.exec.k8s.apiregistration_k8s_io.v1.api_service.get(
             ctx, name=name, resource_id=resource_id
@@ -207,42 +205,40 @@
     ctx,
     name: str,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes an APIService.
 
     Args:
-        name(str):
+        name(str, Optional):
             An Idem name of the resource.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Request Syntax:
-
         .. code-block:: sls
 
-            [api-service-name]:
+           [api-service-name]:
               k8s.apiregistration_k8s_io.v1.api_service.absent:
                 - name: 'string'
                 - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.apiregistration_k8s_io.v1.api_service.absent:
                 - name: "test-api-service"
                 - resource_id: "test-api-service"
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     before = None
     if resource_id:
         api_service = await hub.exec.k8s.apiregistration_k8s_io.v1.api_service.get(
             ctx, name=name, resource_id=resource_id
         )
@@ -274,25 +270,23 @@
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     """Describes the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     list or watch objects of kind APIService.
 
-
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: bash
 
-            $ idem describe k8s.apiregistration_k8s_io.v1.api_service
-    """
+           $ idem describe k8s.apiregistration_k8s_io.v1.api_service
 
+    """
     result = {}
     ret = await hub.exec.k8s.apiregistration_k8s_io.v1.api_service.list(
         ctx, name="k8s.apiregistration_k8s_io.v1.api_service.describe"
     )
     if not ret["result"]:
         hub.log.debug(
             f"Could not describe k8s.apiregistration_k8s_io.v1.api_service {ret['comment']}"
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/apps/v1/daemon_set.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/daemon_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-apps/v1/DaemonSet
-"""
+"""State module for managing Kubernetes DaemonSet."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 from dict_tools import differ
 
@@ -18,37 +14,34 @@
     ctx,
     name: str,
     metadata: Dict,
     spec: Dict,
     resource_id: str = None,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    Create a DaemonSet.
+    """Create a DaemonSet.
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        spec(Dict): The desired behavior of this daemon set. More info:
-            https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-
-            status.
-        timeout(Dict, optional): Timeout configuration for resource creation.
-            * create (Dict) -- Timeout configuration for resource creation
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        spec(dict): The desired behavior of this daemon set. More info:
+            More info: `Kubernetes spec reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-
+            status.>`_
+        timeout(dict, Optional): Timeout configuration for resource creation.
+
+           * create(dict) -- Timeout configuration for resource creation
+              * delay(int, Optional) -- The amount of time in seconds to wait between attempts. Defaults to 15
+              * max_attempts(int, Optional) -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.apps.v1.daemon_set.present:
                 - name: daemon_set_1
                 - metadata: value
                 - spec: value
@@ -81,16 +74,16 @@
                             memory: 200Mi
                           requests:
                             cpu: 100m
                             memory: 200Mi
                         termination_message_path: /dev/termination-log
                         termination_message_policy: File
                       restart_policy: Always
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing daemon_set by name in namespace
@@ -221,45 +214,48 @@
     ] = hub.tool.k8s.apps.v1.daemon_set_utils.convert_raw_daemon_set_to_present(
         daemon_set=after
     )
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None, timeout: Dict = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
+    timeout: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    Delete a DaemonSet.
+    """Delete a DaemonSet.
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        timeout(Dict, optional): Timeout configuration for resource deletion.
-            * delete (Dict) -- Timeout configuration for resource deletion
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40. Defaults to None.
+        name(str, Optional): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        timeout(dict, Optional): Timeout configuration for resource deletion.
+
+            * delete(dict) -- Timeout configuration for resource deletion
+                * delay(int, Optional) -- The amount of time in seconds to wait between attempts. Defaults to 15
+                * max_attempts(int, Optional) -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.apps.v1.daemon_set.absent:
                 - name: value
                 - metadata: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         daemon_set = await hub.exec.k8s.client.AppsV1Api.read_namespaced_daemon_set(
@@ -331,33 +327,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.apps.v1.daemon_set", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
-
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     list or watch objects of kind DaemonSet.
 
-
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.apps.v1.daemon_set
-    """
 
+    """
     ret = await hub.exec.k8s.client.AppsV1Api.list_daemon_set_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe daemon_set {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/apps/v1/deployment.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/apps/v1/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-apps/v1/Deployment
-"""
+"""State module for managing Kubernetes Deployment."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 from dict_tools import differ
 
@@ -18,35 +14,32 @@
     ctx,
     name: str,
     metadata: Dict,
     spec: Dict,
     resource_id: str = None,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create/update a Deployment
+    """create/update a Deployment
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        spec(Dict): Specification of the desired behavior of the Deployment.
-        timeout(Dict, optional): Timeout configuration for resource creation.
-            * create (Dict) -- Timeout configuration for resource creation
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        spec(dict): Specification of the desired behavior of the Deployment.
+        timeout(dict, Optional): Timeout configuration for resource creation.
+
+          * create (dict) -- Timeout configuration for resource creation
+                * delay(int, Optional) -- The amount of time in seconds to wait between attempts. Defaults to 15
+                * max_attempts(int, Optional)  -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.apps.v1.deployment.present:
               - metadata:
                   name: nginx-deployment
                   namespace: default
@@ -71,16 +64,16 @@
                         name: nginx
                         ports:
                         - container_port: 80
                           protocol: TCP
                         termination_message_path: /dev/termination-log
                         termination_message_policy: File
                       restart_policy: Always
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing deployment by name in namespace
@@ -231,44 +224,47 @@
     ] = hub.tool.k8s.apps.v1.deployment_utils.convert_raw_deployment_to_present(
         deployment=after
     )
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None, timeout: Dict = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
+    timeout: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a Deployment
+    """Delete a Deployment
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        timeout(Dict, optional): Timeout configuration for resource deletion.
-            * delete (Dict) -- Timeout configuration for resource deletion
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        timeout(dict, Optional): Timeout configuration for resource deletion.
+
+            * delete(dict) -- Timeout configuration for resource deletion
+                * delay(int, Optional) -- The amount of time in seconds to wait between attempts. Defaults to 15
+                * max_attempts(int, Optional) -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.apps.v1.deployment.absent:
                 - name: value
                 - metadata: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         deployment = await hub.exec.k8s.client.AppsV1Api.read_namespaced_deployment(
@@ -340,33 +336,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.apps.v1.deployment", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list objects of kind Deployment in all namespaces
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List objects of kind Deployment in all namespaces
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.apps.v1.deployment
-    """
 
+    """
     ret = await hub.exec.k8s.client.AppsV1Api.list_deployment_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe deployment {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/config_map.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/config_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-v1/ConfigMap
-"""
+"""State module for managing Kubernetes ConfigMap."""
 import copy
 from typing import Any
 from typing import Dict
 
 from dict_tools import differ
 
 __contracts__ = ["resource"]
@@ -18,42 +14,38 @@
     name: str,
     metadata: Dict,
     immutable: bool = False,
     data: Dict = None,
     binary_data: Dict = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a ConfigMap
+    """Create a ConfigMap
 
     Args:
-        name(Text): An Idem name of the resource.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        binary_data(Dict, Optional): BinaryData contains the binary data. Each key must consist of alphanumeric characters, '-', '_'
+        name(str): An Idem name of the resource.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        binary_data(dict, Optional): BinaryData contains the binary data. Each key must consist of alphanumeric characters, '-', '_'
             or '.'. BinaryData can contain byte sequences that are not in the UTF-8 range. The keys stored
             in BinaryData must not overlap with the ones in the Data field, this is enforced during
             validation process. Using this field will require 1.10+ apiserver and kubelet.
-        data(Dict, Optional): Data contains the configuration data. Each key must consist of alphanumeric characters, '-', '_'
+        data(dict, Optional): Data contains the configuration data. Each key must consist of alphanumeric characters, '-', '_'
             or '.'. Values with non-UTF-8 byte sequences must use the BinaryData field. The keys stored in
             Data must not overlap with the keys in the BinaryData field, this is enforced during validation
             process.
         immutable(bool, Optional): Immutable, if set to true, ensures that data stored in the ConfigMap cannot be updated (only
             object metadata can be modified). If not set to true, the field can be modified at any time.
             Defaulted to nil.
 
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.config_map.present:
                 - name: idem-config-map-test
                 - data:
                       adminRoles: test-admin
@@ -65,16 +57,16 @@
                         meta.helm.sh/release-namespace: test-release-default
                       labels:
                         app: test-app
                         environment: test-environment
                         product: test-product
                       name: idem-config-map-test
                       namespace: default
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing config_map by name in namespace
@@ -182,40 +174,41 @@
     ] = hub.tool.k8s.core.v1.config_map_utils.convert_raw_config_map_to_present(
         config_map=after
     )
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a ConfigMap
+    """Delete a ConfigMap
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.config_map.absent:
                 - name: value
                 - metadata: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         config_map = await hub.exec.k8s.client.CoreV1Api.read_namespaced_config_map(
@@ -249,33 +242,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.core.v1.config_map", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind ConfigMap
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind ConfigMap
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.config_map
-    """
 
+    """
     ret = await hub.exec.k8s.client.CoreV1Api.list_config_map_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe config_map {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/namespace.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/namespace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,44 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-v1/Namespace
-"""
+"""State module for managing Kubernetes Namespace."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 from dict_tools import differ
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub, ctx, name: str, metadata: Dict, resource_id: str = None
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a Namespace
+    """Create a Namespace
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.namespace.present:
               - name: idem-test
               - metadata:
                   name: idem-test
                   labels:
                     example-label-name: example-label-value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Check for existing namespace by name
     before = None
     if resource_id:
         namespace = await hub.exec.k8s.client.CoreV1Api.read_namespace(
             ctx, name=resource_id
@@ -145,40 +137,37 @@
     )
     return result
 
 
 async def absent(
     hub, ctx, name: str, resource_id: str = None, timeout: Dict = None
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a Namespace
+    """Delete a Namespace
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        timeout(Dict, optional): Timeout configuration for resource deletion.
-            * delete (Dict) -- Timeout configuration for resource deletion
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        timeout(dict, Optional): Timeout configuration for resource deletion.
+
+            * delete (dict) -- Timeout configuration for resource deletion
+                * delay(int, Optional) -- The amount of time in seconds to wait between attempts. Defaults to 15
+                * max_attempts(int, Optional) -- Customized timeout configuration containing delay and max attempts. Defaults to 40.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.namespace.absent:
                 - name: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     before = None
     if resource_id:
         namespace = await hub.exec.k8s.client.CoreV1Api.read_namespace(
             ctx, name=resource_id
         )
@@ -248,33 +237,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.core.v1.namespace", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind Namespace
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind Namespace.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.namespace
-    """
 
+    """
     ret = await hub.exec.k8s.client.CoreV1Api.list_namespace(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe namespace {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/persistent_volume_claim.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,36 +69,35 @@
             An Idem name of the resource.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         metadata(dict):
             Standard object's metadata.
-            More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
 
         spec(dict):
             Spec defines the desired characteristics of a volume requested by a pod author.
-            More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims.
+            More info: `Kubernetes spec reference <https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims.>`_
 
-    Request Syntax:
 
+    Request Syntax:
         .. code-block:: sls
 
             [pvc-name]:
               k8s.core.v1.persistent_volume_claim.present:
                 - name: 'string'
                 - metadata: Dict
                 - spec: Dict
                 - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.persistent_volume_claim.present:
                 - name: "pvc-1"
                 - metadata:
                     name: "pvc-1"
@@ -110,15 +109,14 @@
                     access_modes:
                       - ReadWriteMany
                     resources:
                       requests:
                         storage: 1Mi
 
     """
-
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing persistent_volume_claim by name in namespace
@@ -217,55 +215,54 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    metadata: Dict,
+    metadata: Dict = dict(namespace="default"),
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes a PersistentVolumeClaim.
 
     Args:
         name(str):
             An Idem name of the resource.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
-        metadata(dict):
+        metadata(dict, Optional):
             Standard object's metadata.
-            More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
 
     Request Syntax:
-
         .. code-block:: sls
 
             [service-name]:
               k8s.core.v1.service.absent:
                 - name: 'string'
                 - metadata: Dict
                 - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.persistent_volume_claim.absent:
                 - name: "pvc-1"
                 - resource_id: "pvc-1"
                 - metadata:
                     namespace: "default"
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         persistent_volume_claim = (
@@ -301,20 +298,18 @@
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     """Describes the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     list or watch objects of kind PersistentVolumeClaim.
 
-
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.persistent_volume_claim
 
     """
     result = {}
     ret = await hub.exec.k8s.core.v1.persistent_volume_claim.list(
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/secret.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/secret.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-v1/Secret
-"""
+"""State module for managing Kubernetes Secret."""
 import base64
 import copy
 from typing import Any
 from typing import Dict
 
 from dict_tools import differ
 
@@ -20,58 +16,54 @@
     metadata: Dict,
     type: str,
     data: Dict = None,
     immutable: bool = False,
     string_data: Dict = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a Secret
+    """Create a Secret
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        data(Dict, optional): Data contains the secret data. Each key must consist of alphanumeric characters, '-', '_' or
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        data(dict, Optional): Data contains the secret data. Each key must consist of alphanumeric characters, '-', '_' or
             '.'. The serialized form of the secret data is a base64 encoded string, representing the
             arbitrary (possibly non-string) data value here. Described in
             https://tools.ietf.org/html/rfc4648#section-4.
-        immutable(bool, optional): Immutable, if set to true, ensures that data stored in the Secret cannot be updated (only object
+        immutable(bool, Optional): Immutable, if set to true, ensures that data stored in the Secret cannot be updated (only object
             metadata can be modified). If not set to true, the field can be modified at any time. Defaulted
             to nil.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        string_data(Dict, optional): stringData allows specifying non-binary secret data in string form. It is provided as a write-
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata.>`_
+        string_data(dict, Optional): stringData allows specifying non-binary secret data in string form. It is provided as a write-
             only input field for convenience. All keys and values are merged into the data field on write,
             overwriting any existing values. The stringData field is never output when reading from the API.
-        type(Text): Used to facilitate programmatic handling of secret data. More info:
-            https://kubernetes.io/docs/concepts/configuration/secret/#secret-types.
+        type(str): Used to facilitate programmatic handling of secret data.
+            More info: `Secret Types <https://kubernetes.io/docs/concepts/configuration/secret/#secret-types.>`_
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.secret.present:
                 - name: idem-test-secret
                 - data:
                     username: YWRtaW4=
                     password: MWYyZDFlMmU2N2Rm
                 - metadata:
                    name: idem-test-secret
                    namespace: default
                    annotations:
                     kubernetes.io/service-account.name: test-account
                 - type: Opaque
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing secret by name in namespace
@@ -177,40 +169,42 @@
     result[
         "new_state"
     ] = hub.tool.k8s.core.v1.secret_utils.convert_raw_secret_to_present(secret=after)
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a Secret
+    """Delete a Secret
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.secret.absent:
                 - name: value
                 - metadata: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         secret = await hub.exec.k8s.client.CoreV1Api.read_namespaced_secret(
@@ -244,33 +238,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.core.v1.secret", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind Secret
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind Secret.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.secret
-    """
 
+    """
     ret = await hub.exec.k8s.client.CoreV1Api.list_secret_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe secret {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/service.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-core/v1/Service
-"""
+"""State module for managing Kubernetes Service."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import Tuple
 
 from dict_tools import differ
 
@@ -18,45 +14,48 @@
     ctx,
     name: str,
     metadata: Dict,
     spec: Dict,
     resource_id: str = None,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
-    r"""create a Service
+    """create a Service
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        spec(Dict): Spec defines the behavior of a service. https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#spec-and-status.
-        timeout(Dict, optional): Timeout configuration for resource creation.
-            * create (Dict) -- Timeout configuration for resource creation
-                * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
-                * max_attempts -- Customized timeout configuration containing delay and max attempts. Defaults to 40. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
+        spec(dict): Spec defines the behavior of a service.
+            More info: `Kubernetes Spec reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#spec-and-status.>`_
+        timeout(dict, Optional): Timeout configuration for resource creation.
+
+            * create (dict) -- Timeout configuration for resource creation
+                * delay(int, Optional) -- The amount of time in seconds to wait between attempts.
+                  Defaults to 15 in case of None.
+                * max_attempts(int, Optional) -- Customized timeout configuration containing delay and max attempts.
+                  Defaults to 40 in case of None.
 
     Request Syntax:
-
         .. code-block:: sls
 
             [service-name]:
               k8s.core.v1.service.present:
                 - name: "string"
                 - metadata: "Dict"
                 - spec: "Dict"
                 - resource_id: "string"
                 - timeout: "Dict"
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.service.present:
                 - name: idem-test-service
                 - metadata:
                     name: idem-test-secret
@@ -65,16 +64,16 @@
                     type: NodePort
                     selector:
                       app: echo-hostname
                     ports:
                       - nodePort: 30163
                         port: 8080
                         targetPort: 80
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing service by name in namespace
@@ -214,45 +213,51 @@
         return result
     after = service["ret"]
     result["new_state"] = after
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
 ) -> Dict[str, Any]:
     """delete a Service
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
 
     Request Syntax:
       .. code-block:: sls
+
            [service-name]:
               k8s.core.v1.service.absent:
                 - name: 'string'
                 - metadata: 'Dict'
                 - resource_id: 'string'
 
     Returns:
       Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.service.absent:
                 - name: value
                 - metadata: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         service = await hub.exec.k8s.core.v1.service.get(
@@ -283,32 +288,27 @@
             result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
                 resource_type="k8s.core.v1.service", name=name
             )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-
-    list or watch objects of kind Service
+    List or watch objects of kind Service
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.service
-    """
 
+    """
     ret = await hub.exec.k8s.client.CoreV1Api.list_service_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe service {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/core/v1/service_account.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/core/v1/service_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-core/v1/ServiceAccount
-"""
+"""State module for managing Kubernetes ServiceAccount."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import List
 
 from dict_tools import differ
 
@@ -19,52 +15,51 @@
     name: str,
     metadata: Dict,
     automount_service_account_token: bool = True,
     image_pull_secrets: List = None,
     secrets: List = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a ServiceAccount
+    """Create a ServiceAccount
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        automount_service_account_token(bool, optional): AutomountServiceAccountToken indicates whether pods running as this service account should have
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        automount_service_account_token(bool, Optional):
+            AutomountServiceAccountToken indicates whether pods running as this service account should have
             an API token automatically mounted. Can be overridden at the pod level.
-        image_pull_secrets(List, optional): ImagePullSecrets is a list of references to secrets in the same namespace to use for pulling any
+        image_pull_secrets(list, Optional):
+            ImagePullSecrets is a list of references to secrets in the same namespace to use for pulling any
             images in pods that reference this ServiceAccount. ImagePullSecrets are distinct from Secrets
             because Secrets can be mounted in the pod, but ImagePullSecrets are only accessed by the
-            kubelet. More info: https://kubernetes.io/docs/concepts/containers/images/#specifying-
-            imagepullsecrets-on-a-pod.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        secrets(List, optional): Secrets is the list of secrets allowed to be used by pods running using this ServiceAccount.
-            More info: https://kubernetes.io/docs/concepts/configuration/secret.
+            kubelet. More info: `Kubernetes reference <https://kubernetes.io/docs/concepts/containers/images/#specifying-
+            imagepullsecrets-on-a-pod>`_.
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_.
+        secrets(list, Optional): Secrets is the list of secrets allowed to be used by pods running using this ServiceAccount.
+            More info: `Kubernetes secret reference <https://kubernetes.io/docs/concepts/configuration/secret.>`_.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.core.v1.service_account.present:
                 - name: value
                 - metadata:
                   name: idem-service-account-test
                   namespace: default
                   labels:
                     example-label-name: example-label-value
                 - automount_service_account_token: false
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
     metadata["namespace"] = namespace
 
     # Check for existing service_account by name in namespace
@@ -179,41 +174,43 @@
     ] = hub.tool.k8s.core.v1.service_account_utils.convert_raw_service_account_to_present(
         service_account=after
     )
     return result
 
 
 async def absent(
-    hub, ctx, name: str, metadata: Dict, resource_id: str = None
+    hub,
+    ctx,
+    name: str,
+    metadata: Dict = dict(namespace="default"),
+    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a ServiceAccount
+    """Delete a ServiceAccount
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict, Optional): Standard object's metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            More info: `Kubernetes metadata reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.core.v1.service_account.absent:
                 - name: value
                 - metadata: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     namespace = metadata.get("namespace") if "namespace" in metadata else "default"
 
     before = None
     if resource_id:
         service_account = (
@@ -249,33 +246,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.core.v1.service_account", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind ServiceAccount
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind ServiceAccount.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.core.v1.service_account
-    """
 
+    """
     ret = await hub.exec.k8s.client.CoreV1Api.list_service_account_for_all_namespaces(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe service_account {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-rbac.authorization.k8s.io/v1/ClusterRole
-"""
+"""State module for managing Kubernetes ClusterRole."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import List
 
 from dict_tools import differ
 
@@ -18,33 +14,30 @@
     ctx,
     name: str,
     metadata: Dict,
     aggregation_rule: Dict = None,
     rules: List = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a ClusterRole
+    """Create a ClusterRole
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        aggregation_rule(Dict, optional): AggregationRule is an optional field that describes how to build the Rules for this ClusterRole.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        aggregation_rule(dict, Optional):
+            AggregationRule is an optional field that describes how to build the Rules for this ClusterRole.
             If AggregationRule is set, then the Rules are controller managed and direct changes to Rules
             will be stomped by the controller.
-        metadata(Dict): Standard object's metadata.
-        rules(List. optional): Rules holds all the PolicyRules for this ClusterRole.
+        metadata(dict): Standard object's metadata.
+        rules(list, Optional): Rules holds all the PolicyRules for this ClusterRole.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.rbac.v1.cluster_role.present:
               - name: value
               - metadata:
                   name: idem-test-cluster-role
@@ -53,16 +46,16 @@
                   - test.com
                   resources:
                   - vaconfigs
                   verbs:
                   - get
                   - list
                   - watch
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Check for existing cluster_role by name
     before = None
     if resource_id:
         cluster_role = (
             await hub.exec.k8s.client.RbacAuthorizationV1Api.read_cluster_role(
@@ -168,36 +161,32 @@
     ] = hub.tool.k8s.rbac.v1.cluster_role_utils.convert_raw_cluster_role_to_present(
         cluster_role=after
     )
     return result
 
 
 async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a ClusterRole
+    """Delete a ClusterRole
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.rbac.v1.cluster_role.absent:
                 - name: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     before = None
     if resource_id:
         cluster_role = (
             await hub.exec.k8s.client.RbacAuthorizationV1Api.read_cluster_role(
                 ctx, name=resource_id
@@ -231,33 +220,27 @@
         result["comment"] = hub.tool.k8s.comment_utils.delete_comment(
             resource_type="k8s.rbac.v1.cluster_role", name=name
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind ClusterRole
+    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind ClusterRole.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.rbac.v1.cluster_role
-    """
 
+    """
     ret = await hub.exec.k8s.client.RbacAuthorizationV1Api.list_cluster_role(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe cluster_role {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/cluster_role_binding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-rbac.authorization.k8s.io/v1/ClusterRoleBinding
-"""
+"""State module for managing Kubernetes ClusterRoleBinding."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import List
 
 from dict_tools import differ
 
@@ -18,31 +14,28 @@
     ctx,
     name: str,
     metadata: Dict,
     role_ref: Dict,
     subjects: List,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    create a ClusterRoleBinding
+    """Create a ClusterRoleBinding
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        metadata(Dict): Standard object's metadata.
-        role_ref(Dict): RoleRef can only reference a ClusterRole in the global namespace. If the RoleRef cannot be
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        metadata(dict): Standard object's metadata.
+        role_ref(dict): RoleRef can only reference a ClusterRole in the global namespace. If the RoleRef cannot be
             resolved, the Authorizer must return an error.
-        subjects(List): Subjects holds references to the objects the role applies to.
+        subjects(list): Subjects holds references to the objects the role applies to.
+
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.rbac.v1.cluster_role_binding.present:
                   - name: idem-test-cluster-role-binding
                   - metadata:
                       annotations:
@@ -54,16 +47,16 @@
                       api_group: rbac.authorization.k8s.io
                       kind: ClusterRole
                       name: idem-test-cluster-role-binding
                   - subjects:
                     - api_group: rbac.authorization.k8s.io
                       kind: User
                       name: idem-test-cluster-role-binding
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Check for existing cluster_role_binding by name
     before = None
     if resource_id:
         cluster_role_binding = (
             await hub.exec.k8s.client.RbacAuthorizationV1Api.read_cluster_role_binding(
@@ -171,36 +164,32 @@
     ] = hub.tool.k8s.rbac.v1.cluster_role_binding_utils.convert_raw_cluster_role_binding_to_present(
         cluster_role_binding=after
     )
     return result
 
 
 async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    delete a ClusterRoleBinding
+    """Delete a ClusterRoleBinding
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.rbac.v1.cluster_role_binding.absent:
                 - name: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     before = None
     if resource_id:
         cluster_role_binding = (
             await hub.exec.k8s.client.RbacAuthorizationV1Api.read_cluster_role_binding(
                 ctx, name=resource_id
@@ -237,33 +226,27 @@
             resource_type="k8s.rbac.v1.cluster_role_binding",
             name=name,
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
+    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
     list or watch objects of kind ClusterRoleBinding
 
-
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.rbac.v1.cluster_role_binding
-    """
 
+    """
     ret = await hub.exec.k8s.client.RbacAuthorizationV1Api.list_cluster_role_binding(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe cluster_role_binding {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/rbac/v1/role_binding.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/rbac/v1/role_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,29 +56,27 @@
         role_ref(dict):
             RoleRef can reference a Role in the current namespace or a ClusterRole in the global namespace.
             If the RoleRef cannot be resolved, the Authorizer must return an error.
         subjects(list):
             Subjects holds references to the objects the role applies to.
 
     Request Syntax:
-
         .. code-block:: sls
 
             [unmanaged_resource]:
               k8s.rbac.v1.role_binding.present:
                 - name: 'string'
                 - metadata: 'dict'
                 - role_ref: 'dict'
                 - subjects: 'dict'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.rbac.v1.role_binding.present:
                   - resource_id: system:controller:token-cleaner
                   - metadata:
                       annotations:
@@ -90,16 +88,17 @@
                   - role_ref:
                       api_group: rbac.authorization.k8s.io
                       kind: Role
                       name: system:controller:token-cleaner
                   - subjects:
                     - kind: ServiceAccount
                       name: token-cleaner
-                      namespace: kube-system"""
+                      namespace: kube-system
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Get namespace
     namespace = metadata.get("namespace", "default")
 
     # Check for existing role_binding by name in namespace
     before = None
@@ -215,39 +214,39 @@
 
     Args:
         name(str):
             An Idem name of the resource.
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
         metadata(dict, Optional):
-            Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
+            Defaults to metadata with 'default' namespace, in case of value not provided in absent state.
+            Standard object's metadata. More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
 
     Returns:
         Dict[str, Any]
 
     Request Syntax:
-
         .. code-block:: sls
 
             [k8s.rbac.v1.role_binding.name]:
               k8s.rbac.v1.role_binding.absent:
                 - resource_id: 'string'
                 - name: 'string'
                 - metadata: 'dict'
-    Examples:
 
+    Examples:
         .. code-block:: sls
 
             resource_is_absent:
               k8s.rbac.v1.role_binding.absent:
                 - resource_id: 'k8s.rbac.v1.role_binding.id'
                 - name: 'role_binding_name'
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     namespace = "default"
     if metadata:
         namespace = metadata.get("namespace", "default")
     before = None
     if resource_id:
         role_binding = await hub.exec.k8s.rbac.v1.role_binding.get(
```

### Comparing `idem-k8s-0.5.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py` & `idem-k8s-0.6.0/idem_k8s/states/k8s/storage_k8s_io/v1/storage_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Autogenerated using `pop-create-idem <https://gitlab.com/saltstack/pop/pop-create-idem>`__
-
-storage.k8s.io/v1/StorageClass
-"""
+"""State module for managing Kubernetes StorageClass."""
 import copy
 from typing import Any
 from typing import Dict
 from typing import List
 
 from dict_tools import differ
 
@@ -23,47 +19,44 @@
     allowed_topologies: List = None,
     mount_options: List = None,
     parameters: Dict = None,
     reclaim_policy: str = None,
     volume_binding_mode: str = "Immediate",
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    Create a StorageClass.
+    """Create a StorageClass.
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
-        allow_volume_expansion(bool, optional): AllowVolumeExpansion shows whether the storage class allow volume
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        allow_volume_expansion(bool, Optional): AllowVolumeExpansion shows whether the storage class allow volume
             expand.
-        allowed_topologies(List, optional): Restrict the node topologies where volumes can be dynamically provisioned.
+        allowed_topologies(list, Optional): Restrict the node topologies where volumes can be dynamically provisioned.
             Each volume plugin defines its own supported topology specifications.
             An empty TopologySelectorTerm list means there is no topology restriction.
             This field is only honored by servers that enable the VolumeScheduling feature.
-        metadata(Dict): Standard object's metadata. More info: https://git.k8s.io/community/contributors/devel/sig-
-            architecture/api-conventions.md#metadata.
-        mount_options(List, optional): Dynamically provisioned PersistentVolumes of this storage class are created with
+        metadata(dict): Standard object's metadata.
+            More info: `Kubernetes reference <https://git.k8s.io/community/contributors/devel/sig-
+            architecture/api-conventions.md#metadata.>`_
+        mount_options(list, Optional): Dynamically provisioned PersistentVolumes of this storage class are created with
             these mountOptions, e.g. ["ro", "soft"]. Not validated - mount of the PVs will simply fail if one is
             invalid.
-        parameters(Dict, optional): Parameters holds the parameters for the provisioner that should create volumes of
+        parameters(dict, Optional): Parameters holds the parameters for the provisioner that should create volumes of
             this storage class.
-        provisioner(Text): Provisioner indicates the type of the provisioner.
-        reclaim_policy(Text, optional): Dynamically provisioned PersistentVolumes of this storage class are created with
+        provisioner(str): Provisioner indicates the type of the provisioner.
+        reclaim_policy(str, Optional): Dynamically provisioned PersistentVolumes of this storage class are created with
             this reclaimPolicy. Defaults to Delete.
-        volume_binding_mode(Text, optional): VolumeBindingMode indicates how PersistentVolumeClaims should be
+        volume_binding_mode(str, Optional): VolumeBindingMode indicates how PersistentVolumeClaims should be
             provisioned and bound. When unset, VolumeBindingImmediate is used. This field is only honored by servers
             that enable the VolumeScheduling feature.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_present:
               k8s.storage_k8s_io.v1.storage_class.present:
                 - name: storage_class_1
                 - allow_volume_expansion: true
                 - allowed_topologies:
@@ -75,16 +68,16 @@
                 - mount_options: ["soft"]
                 - parameters:
                     type: "gp2"
                     iopsPerGB: "10"
                 - provisioner: "kubernetes.io/aws-ebs"
                 - reclaim_policy: "Retain"
                 - volume_binding_mode: "WaitForFirstConsumer"
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # Check for existing storage_class by name
     before = None
     if resource_id:
         storage_class = await hub.exec.k8s.client.StorageV1Api.read_storage_class(
             ctx, name=resource_id
@@ -191,36 +184,32 @@
     ] = hub.tool.k8s.storage_k8s_io.v1.storage_class_utils.convert_raw_storage_class_to_present(
         storage_class=after
     )
     return result
 
 
 async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
-    r"""
-    **Autogenerated function**
-
-    Delete a StorageClass.
+    """Delete a StorageClass.
 
     Args:
-        name(Text): An Idem name of the resource.
-        resource_id(Text, optional): An identifier of the resource in the provider. Defaults to None.
+        name(str): An Idem name of the resource.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             resource_is_absent:
               k8s.storage_k8s_io.v1.storage_class.absent:
                 - name: value
                 - resource_id: value
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     before = None
     if resource_id:
         storage_class = await hub.exec.k8s.client.StorageV1Api.read_storage_class(
             ctx, name=resource_id
         )
@@ -252,33 +241,27 @@
             if result["result"]
             else ret["comment"]
         )
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
-    **Autogenerated function**
-
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
-
-
-    list or watch objects of kind StorageClass
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
+    List or watch objects of kind StorageClass.
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe k8s.storage_k8s_io.v1.storage_class
-    """
 
+    """
     ret = await hub.exec.k8s.client.StorageV1Api.list_storage_class(
         ctx,
     )
     if not ret["result"]:
         hub.log.debug(f"Could not describe storage_class {ret['comment']}")
         return {}
```

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/apiregistration_k8s_io/v1/api_service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/daemon_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/apps/v1/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/client.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/client.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/comment_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/config_map_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/namespace_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/persistent_volume_claim_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/secret_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/secret_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_account_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/core/v1/service_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/core/v1/service_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/custom_waiter.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/marshaller.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/marshaller.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/cluster_role_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/rbac/v1/role_binding_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/resolve.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/state_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/storage_k8s_io/v1/storage_class_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/test_state_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s/tool/k8s/waiter_utils.py` & `idem-k8s-0.6.0/idem_k8s/tool/k8s/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/idem_k8s.egg-info/PKG-INFO` & `idem-k8s-0.6.0/idem_k8s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-k8s
-Version: 0.5.0
+Version: 0.6.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Naresh
 Author-email: nkumar5@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-k8s-0.5.0/idem_k8s.egg-info/SOURCES.txt` & `idem-k8s-0.6.0/idem_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-k8s-0.5.0/setup.py` & `idem-k8s-0.6.0/setup.py`

 * *Files identical despite different names*

