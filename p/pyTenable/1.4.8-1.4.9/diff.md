# Comparing `tmp/pyTenable-1.4.8.tar.gz` & `tmp/pyTenable-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTenable-1.4.8.tar", last modified: Tue Sep 20 07:13:23 2022, max compression
+gzip compressed data, was "pyTenable-1.4.9.tar", last modified: Wed Nov  9 08:06:19 2022, max compression
```

## Comparing `pyTenable-1.4.8.tar` & `pyTenable-1.4.9.tar`

### file list

```diff
@@ -1,260 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.816539 pyTenable-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-20 07:13:21.000000 pyTenable-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-20 07:13:21.000000 pyTenable-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-09-20 07:13:23.816539 pyTenable-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-09-20 07:13:21.000000 pyTenable-1.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.796539 pyTenable-1.4.8/pyTenable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4393 2022-09-20 07:13:23.000000 pyTenable-1.4.8/pyTenable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-09-20 07:13:23.000000 pyTenable-1.4.8/pyTenable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 07:13:23.000000 pyTenable-1.4.8/pyTenable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-20 07:13:23.000000 pyTenable-1.4.8/pyTenable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-20 07:13:23.000000 pyTenable-1.4.8/pyTenable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 07:13:23.816539 pyTenable-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-09-20 07:13:21.000000 pyTenable-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/about.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/api_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/attack_types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/attack_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/attack_types/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/attack_types/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/base/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/category/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/category/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/category/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/checker/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/checker_option/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker_option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker_option/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/checker_option/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/dashboard/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/dashboard/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/directories/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/directories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/directories/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/directories/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/infrastructure/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/infrastructure/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/ldap_configuration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/ldap_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/ldap_configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/ldap_configuration/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/lockout_policy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/lockout_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/lockout_policy/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/lockout_policy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/preference/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/preference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/preference/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/preference/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/profiles/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/profiles/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/reason/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/reason/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/reason/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/roles/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/roles/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/roles/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.800539 pyTenable-1.4.8/tenable/ad/saml_configuration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/saml_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3109 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/saml_configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/saml_configuration/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/ad/score/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/score/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/score/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5469 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/ad/topology/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/topology/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/topology/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/ad/users/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/users/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/users/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/ad/widget/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7401 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/widget/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ad/widget/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/base/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/schema/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/base/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/utils/envelope.py
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/base/v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.804539 pyTenable-1.4.8/tenable/dl/
--rw-r--r--   0 runner    (1001) docker     (121)     5081 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/
--rw-r--r--   0 runner    (1001) docker     (121)    11963 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14679 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/access_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    16853 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/access_groups_v2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    15118 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/agent_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13193 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/agent_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     9701 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/agents.py
--rw-r--r--   0 runner    (1001) docker     (121)     9706 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/audit_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/base/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/base/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/base/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/base/schemas/filters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/base/schemas/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/base/schemas/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/base/v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    15634 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/cs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/images.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/cs/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)    13415 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)    16413 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/exclusions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/exports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19217 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/exports/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    11604 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/exports/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/exports/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     7332 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    14464 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/networks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7516 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     9792 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    13097 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/remediation_scans.py
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/scanner_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    10371 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/scanners.py
--rw-r--r--   0 runner    (1001) docker     (121)    59738 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/scans.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/session.py
--rw-r--r--   0 runner    (1001) docker     (121)    28444 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     5263 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/target_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    13356 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/users.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/access_control.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/base/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/endpoints/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/base/iterators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/iterators/explore_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/iterators/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/base/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/base/schema/explore/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/schema/explore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5674 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/schema/explore/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/base/schema/explore/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/explore/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/explore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/explore/assets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/explore/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13819 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/explore/assets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.808539 pyTenable-1.4.8/tenable/io/v3/explore/findings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/explore/findings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15046 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/v3/explore/findings/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    25895 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/io/workbenches.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/nessus/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/agent_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/agents.py
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/nessus/iterators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/iterators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/iterators/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/iterators/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/mail.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/plugin_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6824 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/scanners.py
--rw-r--r--   0 runner    (1001) docker     (121)    13928 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/scans.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/nessus/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/schema/pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/schema/scans.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/schema/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/software_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     3631 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     5086 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/nessus/users.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/ot/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/ot/graphql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6671 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/graphql/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/graphql/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/graphql/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/ot/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.812539 pyTenable-1.4.8/tenable/reports/
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6092 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/reports/nessusv2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 07:13:23.816539 pyTenable-1.4.8/tenable/sc/
--rw-r--r--   0 runner    (1001) docker     (121)    15311 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10044 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/accept_risks.py
--rw-r--r--   0 runner    (1001) docker     (121)    11873 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)    27928 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    33162 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/asset_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)    16387 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/audit_files.py
--rw-r--r--   0 runner    (1001) docker     (121)    12011 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    45191 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/current.py
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     6935 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    24252 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/organizations.py
--rw-r--r--   0 runner    (1001) docker     (121)    12448 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)    18420 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    10132 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)    10519 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/recast_risks.py
--rw-r--r--   0 runner    (1001) docker     (121)    30535 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)    13169 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/roles.py
--rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/scan_instances.py
--rw-r--r--   0 runner    (1001) docker     (121)     5265 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/scan_zones.py
--rw-r--r--   0 runner    (1001) docker     (121)    11736 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/scanners.py
--rw-r--r--   0 runner    (1001) docker     (121)    20754 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/scans.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     6405 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/system.py
--rw-r--r--   0 runner    (1001) docker     (121)    16391 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/sc/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-20 07:13:21.000000 pyTenable-1.4.8/tenable/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.651780 pyTenable-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-09 08:06:17.000000 pyTenable-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-09 08:06:17.000000 pyTenable-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2022-11-09 08:06:19.651780 pyTenable-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2022-11-09 08:06:17.000000 pyTenable-1.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.627780 pyTenable-1.4.9/pyTenable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2022-11-09 08:06:19.000000 pyTenable-1.4.9/pyTenable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6237 2022-11-09 08:06:19.000000 pyTenable-1.4.9/pyTenable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-09 08:06:19.000000 pyTenable-1.4.9/pyTenable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2022-11-09 08:06:19.000000 pyTenable-1.4.9/pyTenable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2022-11-09 08:06:19.000000 pyTenable-1.4.9/pyTenable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-09 08:06:19.651780 pyTenable-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2022-11-09 08:06:17.000000 pyTenable-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.627780 pyTenable-1.4.9/tenable/
+-rw-r--r--   0 runner    (1001) docker     (122)     3031 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.627780 pyTenable-1.4.9/tenable/ad/
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/api_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.627780 pyTenable-1.4.9/tenable/ad/attack_types/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/attack_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/attack_types/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/attack_types/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.627780 pyTenable-1.4.9/tenable/ad/base/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/base/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/category/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/category/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/category/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/checker/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/checker_option/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker_option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3367 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker_option/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/checker_option/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/dashboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/dashboard/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/directories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/directories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6394 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/directories/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/directories/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3770 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/infrastructure/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/infrastructure/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/ldap_configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/ldap_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/ldap_configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/ldap_configuration/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/lockout_policy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/lockout_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/lockout_policy/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/lockout_policy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/preference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/preference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/preference/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/preference/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4932 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/profiles/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/profiles/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/reason/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/reason/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/reason/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/roles/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5687 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/roles/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/roles/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.631780 pyTenable-1.4.9/tenable/ad/saml_configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/saml_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/saml_configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/saml_configuration/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/ad/score/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/score/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/score/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5469 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/ad/topology/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/topology/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/topology/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/ad/users/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/users/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/users/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/ad/widget/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7401 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/widget/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ad/widget/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/base/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3316 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7781 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/base/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/schema/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/utils/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/base/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.635780 pyTenable-1.4.9/tenable/dl/
+-rw-r--r--   0 runner    (1001) docker     (122)     5081 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    11963 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14679 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/access_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16853 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/access_groups_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15118 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/agent_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/agent_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9701 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/agents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9706 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/audit_log.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/base/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/base/schemas/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/base/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/base/schemas/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/base/schemas/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5079 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/base/schemas/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/base/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/cs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3312 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/cs/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13415 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/editor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16413 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/exclusions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/exports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20807 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/exports/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11596 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/exports/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/exports/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7332 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/folders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4333 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14464 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7516 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9792 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/policies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13097 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/remediation_scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7348 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/scanner_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10371 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/scanners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59933 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28444 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5263 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13356 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/users.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7264 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/access_control.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/base/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/base/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5079 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/endpoints/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/base/iterators/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2659 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/iterators/explore_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/iterators/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/base/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.639780 pyTenable-1.4.9/tenable/io/v3/base/schema/explore/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/schema/explore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5674 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/schema/explore/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/base/schema/explore/search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/io/v3/explore/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/explore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/io/v3/explore/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/explore/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13819 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/explore/assets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/io/v3/explore/findings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/explore/findings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15046 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/v3/explore/findings/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25895 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/io/workbenches.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/nessus/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/agent_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/agents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5202 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4835 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/editor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3456 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/folders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3530 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/nessus/iterators/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/iterators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/iterators/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/iterators/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/mail.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/plugin_rules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4974 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/policies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2302 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/scanners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13928 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/scans.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/nessus/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/schema/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/schema/scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/schema/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3170 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5086 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/nessus/users.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.643780 pyTenable-1.4.9/tenable/ot/
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.647780 pyTenable-1.4.9/tenable/ot/graphql/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6353 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.647780 pyTenable-1.4.9/tenable/ot/graphql/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5838 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/schema/assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8797 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/schema/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/graphql/schema/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.647780 pyTenable-1.4.9/tenable/ot/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/schema/assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3660 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/schema/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/schema/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4208 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/ot/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.647780 pyTenable-1.4.9/tenable/reports/
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6092 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/reports/nessusv2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-09 08:06:19.647780 pyTenable-1.4.9/tenable/sc/
+-rw-r--r--   0 runner    (1001) docker     (122)    15311 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10044 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/accept_risks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11873 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27928 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33162 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/asset_lists.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16387 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/audit_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12011 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45191 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/current.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6935 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24252 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12448 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18420 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/policies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10132 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10519 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/recast_risks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30535 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13169 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11803 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/scan_instances.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5265 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/scan_zones.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11736 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/scanners.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20754 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/scans.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6405 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/system.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16391 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/sc/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1431 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2022-11-09 08:06:17.000000 pyTenable-1.4.9/tenable/version.py
```

### Comparing `pyTenable-1.4.8/LICENSE` & `pyTenable-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/PKG-INFO` & `pyTenable-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyTenable
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library to interface into Tenable's products and applications
 Home-page: https://github.com/tenable/pytenable
 Author: Tenable, Inc.
 Author-email: smcgrath@tenable.com
 License: MIT
 Description: Welcome to pyTenable's documentation!
         =====================================
```

### Comparing `pyTenable-1.4.8/README.rst` & `pyTenable-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/pyTenable.egg-info/PKG-INFO` & `pyTenable-1.4.9/pyTenable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyTenable
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library to interface into Tenable's products and applications
 Home-page: https://github.com/tenable/pytenable
 Author: Tenable, Inc.
 Author-email: smcgrath@tenable.com
 License: MIT
 Description: Welcome to pyTenable's documentation!
         =====================================
```

### Comparing `pyTenable-1.4.8/pyTenable.egg-info/SOURCES.txt` & `pyTenable-1.4.9/pyTenable.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -169,20 +169,32 @@
 tenable/nessus/iterators/pagination.py
 tenable/nessus/iterators/plugins.py
 tenable/nessus/schema/__init__.py
 tenable/nessus/schema/pagination.py
 tenable/nessus/schema/scans.py
 tenable/nessus/schema/settings.py
 tenable/ot/__init__.py
+tenable/ot/api.py
 tenable/ot/assets.py
+tenable/ot/events.py
+tenable/ot/plugins.py
 tenable/ot/session.py
 tenable/ot/graphql/__init__.py
-tenable/ot/graphql/assets.py
 tenable/ot/graphql/definitions.py
 tenable/ot/graphql/iterators.py
+tenable/ot/graphql/query.py
+tenable/ot/graphql/schema/__init__.py
+tenable/ot/graphql/schema/assets.py
+tenable/ot/graphql/schema/events.py
+tenable/ot/graphql/schema/plugins.py
+tenable/ot/schema/__init__.py
+tenable/ot/schema/assets.py
+tenable/ot/schema/base.py
+tenable/ot/schema/events.py
+tenable/ot/schema/plugins.py
 tenable/reports/__init__.py
 tenable/reports/nessusv2.py
 tenable/sc/__init__.py
 tenable/sc/accept_risks.py
 tenable/sc/alerts.py
 tenable/sc/analysis.py
 tenable/sc/asset_lists.py
```

### Comparing `pyTenable-1.4.8/setup.py` & `pyTenable-1.4.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 from setuptools import setup, find_packages
 import os
 
-with open('tenable/version.py', 'r') as vfile:
+with open("tenable/version.py", "r") as vfile:
     exec(vfile.read())
 
 try:
     long_description = open(
-        os.path.join(
-            os.path.abspath(os.path.dirname(__file__)),
-            'README.rst')).read()
+        os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.rst")
+    ).read()
 except:
-    long_description = 'Please refer to https://pytenable.readthedocs.io'
-    print('! could not read README.rst file.')
+    long_description = "Please refer to https://pytenable.readthedocs.io"
+    print("! could not read README.rst file.")
 
 setup(
-    name='pyTenable',
+    name="pyTenable",
     version=version,  # noqa
-    description=('Python library to interface into Tenable\'s '
-                 'products and applications'
-                 ),
-    author='Tenable, Inc.',
+    description=(
+        "Python library to interface into Tenable's " "products and applications"
+    ),
+    author="Tenable, Inc.",
     long_description=long_description,
-    author_email='smcgrath@tenable.com',
-    url='https://github.com/tenable/pytenable',
-    license='MIT',
+    author_email="smcgrath@tenable.com",
+    url="https://github.com/tenable/pytenable",
+    license="MIT",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Application Frameworks',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
-    keywords='tenable tenable_io securitycenter containersecurity',
-    packages=find_packages(exclude=['docs', 'tests']),
+    keywords="tenable tenable_io securitycenter containersecurity",
+    packages=find_packages(exclude=["docs", "tests"]),
     install_requires=[
-        'requests>=2.26',
-        'python-dateutil>=2.6',
-        'semver>=2.8.1',
-        'restfly>=1.4.5',
-        'marshmallow>=3.6',
-        'python-box>=4.0',
-        'defusedxml>=0.5.0',
-        'urllib3>=1.26.5',
-        'typing-extensions>=4.0.1',
+        "requests>=2.26",
+        "python-dateutil>=2.6",
+        "semver>=2.8.1",
+        "restfly>=1.4.5",
+        "marshmallow>=3.8",
+        "python-box>=4.0",
+        "defusedxml>=0.5.0",
+        "urllib3>=1.26.5",
+        "typing-extensions>=4.0.1",
         'dataclasses>=0.8;python_version=="3.6"',
     ],
 )
```

### Comparing `pyTenable-1.4.8/tenable/__init__.py` & `pyTenable-1.4.9/tenable/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/about.py` & `pyTenable-1.4.9/tenable/ad/about.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/api_keys.py` & `pyTenable-1.4.9/tenable/ad/api_keys.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/attack_types/api.py` & `pyTenable-1.4.9/tenable/ad/attack_types/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/attack_types/schema.py` & `pyTenable-1.4.9/tenable/ad/attack_types/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/base/schema.py` & `pyTenable-1.4.9/tenable/ad/base/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/category/api.py` & `pyTenable-1.4.9/tenable/ad/category/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/checker/api.py` & `pyTenable-1.4.9/tenable/ad/checker/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/checker/schema.py` & `pyTenable-1.4.9/tenable/ad/checker/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/checker_option/api.py` & `pyTenable-1.4.9/tenable/ad/checker_option/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/checker_option/schema.py` & `pyTenable-1.4.9/tenable/ad/checker_option/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/dashboard/api.py` & `pyTenable-1.4.9/tenable/ad/dashboard/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/directories/api.py` & `pyTenable-1.4.9/tenable/ad/directories/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/infrastructure/api.py` & `pyTenable-1.4.9/tenable/ad/infrastructure/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/ldap_configuration/api.py` & `pyTenable-1.4.9/tenable/ad/ldap_configuration/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/ldap_configuration/schema.py` & `pyTenable-1.4.9/tenable/ad/ldap_configuration/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/lockout_policy/api.py` & `pyTenable-1.4.9/tenable/ad/lockout_policy/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/preference/api.py` & `pyTenable-1.4.9/tenable/ad/preference/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/profiles/api.py` & `pyTenable-1.4.9/tenable/ad/profiles/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/reason/api.py` & `pyTenable-1.4.9/tenable/ad/reason/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/roles/api.py` & `pyTenable-1.4.9/tenable/ad/roles/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/roles/schema.py` & `pyTenable-1.4.9/tenable/ad/roles/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/saml_configuration/api.py` & `pyTenable-1.4.9/tenable/ad/saml_configuration/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/saml_configuration/schema.py` & `pyTenable-1.4.9/tenable/ad/saml_configuration/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/score/api.py` & `pyTenable-1.4.9/tenable/ad/score/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/score/schema.py` & `pyTenable-1.4.9/tenable/ad/score/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/session.py` & `pyTenable-1.4.9/tenable/ad/session.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/topology/api.py` & `pyTenable-1.4.9/tenable/ad/topology/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/topology/schema.py` & `pyTenable-1.4.9/tenable/ad/topology/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/users/api.py` & `pyTenable-1.4.9/tenable/ad/users/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/users/schema.py` & `pyTenable-1.4.9/tenable/ad/users/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/widget/api.py` & `pyTenable-1.4.9/tenable/ad/widget/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ad/widget/schema.py` & `pyTenable-1.4.9/tenable/ad/widget/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/base/endpoint.py` & `pyTenable-1.4.9/tenable/base/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/base/platform.py` & `pyTenable-1.4.9/tenable/base/platform.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/base/schema/fields.py` & `pyTenable-1.4.9/tenable/base/schema/fields.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/base/utils/envelope.py` & `pyTenable-1.4.9/tenable/base/utils/envelope.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/base/v1.py` & `pyTenable-1.4.9/tenable/base/v1.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/constants.py` & `pyTenable-1.4.9/tenable/constants.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/dl/__init__.py` & `pyTenable-1.4.9/tenable/dl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/errors.py` & `pyTenable-1.4.9/tenable/errors.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/__init__.py` & `pyTenable-1.4.9/tenable/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/access_groups.py` & `pyTenable-1.4.9/tenable/io/access_groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/access_groups_v2.py` & `pyTenable-1.4.9/tenable/io/access_groups_v2.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/agent_config.py` & `pyTenable-1.4.9/tenable/io/agent_config.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/agent_exclusions.py` & `pyTenable-1.4.9/tenable/io/agent_exclusions.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/agent_groups.py` & `pyTenable-1.4.9/tenable/io/agent_groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/agents.py` & `pyTenable-1.4.9/tenable/io/agents.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/assets.py` & `pyTenable-1.4.9/tenable/io/assets.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/audit_log.py` & `pyTenable-1.4.9/tenable/io/audit_log.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/base/schemas/filters/base.py` & `pyTenable-1.4.9/tenable/io/base/schemas/filters/base.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/base/v1.py` & `pyTenable-1.4.9/tenable/io/base/v1.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/credentials.py` & `pyTenable-1.4.9/tenable/io/credentials.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/cs/api.py` & `pyTenable-1.4.9/tenable/io/cs/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/cs/images.py` & `pyTenable-1.4.9/tenable/io/cs/images.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/cs/iterator.py` & `pyTenable-1.4.9/tenable/io/cs/iterator.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/cs/reports.py` & `pyTenable-1.4.9/tenable/io/cs/reports.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/cs/repositories.py` & `pyTenable-1.4.9/tenable/io/cs/repositories.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/editor.py` & `pyTenable-1.4.9/tenable/io/editor.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/exclusions.py` & `pyTenable-1.4.9/tenable/io/exclusions.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/exports/api.py` & `pyTenable-1.4.9/tenable/io/exports/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,53 @@
 
         Examples:
 
             >>> jobs = tio.exports.jobs('vulns')
         '''
         return self._api.get(f'{export_type}/export/status', box=True).exports
 
+    def initiate_export(self,
+                        export_type: Literal['vulns', 'assets', 'compliance'],
+                        **kwargs):
+        """
+        Initiate an export job of the specified export type, and return the export UUID.
+
+        This method accepts the key-value arguments supported by the methods assets(), vulns(), and compliance()
+        for the matching export_type. For example, when the export_type is "assets", this function will only support the
+        kwargs supported by the assets() method; if export_type is "vulns", the method will accept only those
+        supported by the vulns() method, and so forth.
+
+        Args:
+            export_type (str):
+                The datatype of export to get the jobs for.
+
+        Examples:
+
+            Initiating an assets export with no extra params.
+
+            >>> export_uuid = tio.exports.initiate_export("assets")
+
+            Initiating a vulns export with the params supported by vulns()
+
+            >>> export_uuid = tio.exports.initiate_export("vulns", timeout=10)
+        """
+
+        # Setting the schema for the specified export type.
+        if export_type == "vulns":
+            schema = VulnExportSchema()
+        elif export_type == "assets":
+            schema = AssetExportSchema()
+        elif export_type == "compliance":
+            schema = ComplianceExportSchema()
+
+        payload = schema.dump(schema.load(kwargs))
+
+        # Initiating the export and returning the returned export UUID.
+        return self._api.post(f'{export_type}/export', json=payload, box=True).export_uuid
+
     def _export(self,
                 export_type: Literal['vulns', 'assets', 'compliance'],
                 schema: Schema,
                 **kwargs
                 ) -> Union[ExportsIterator, UUID]:
         '''
         Get the list of jobs for for the specified datatype.
```

### Comparing `pyTenable-1.4.8/tenable/io/exports/iterator.py` & `pyTenable-1.4.9/tenable/io/exports/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 As exports are asynchronous, pyTenable by default will return an iterator to
 handle the state tracking, data chunking, and presentation of the data in order
-to reduce the amount of boilerplate code that would otherwise hacve to be
-created.  These iterators support both serial iteration as well as threaded
+to reduce the amount of boilerplate code that would otherwise have to be
+created.  These iterators support both serial iteration and threaded
 handling of data depending on how the data is accessed.
 
 .. autoclass:: ExportsIterator
     :members:
 '''
 import time
 from concurrent.futures import ThreadPoolExecutor
```

### Comparing `pyTenable-1.4.8/tenable/io/exports/schema.py` & `pyTenable-1.4.9/tenable/io/exports/schema.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/files.py` & `pyTenable-1.4.9/tenable/io/files.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/filters.py` & `pyTenable-1.4.9/tenable/io/filters.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/folders.py` & `pyTenable-1.4.9/tenable/io/folders.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/groups.py` & `pyTenable-1.4.9/tenable/io/groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/networks.py` & `pyTenable-1.4.9/tenable/io/networks.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/permissions.py` & `pyTenable-1.4.9/tenable/io/permissions.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/plugins.py` & `pyTenable-1.4.9/tenable/io/plugins.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/policies.py` & `pyTenable-1.4.9/tenable/io/policies.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/remediation_scans.py` & `pyTenable-1.4.9/tenable/io/remediation_scans.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/scanner_groups.py` & `pyTenable-1.4.9/tenable/io/scanner_groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/scanners.py` & `pyTenable-1.4.9/tenable/io/scanners.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/scans.py` & `pyTenable-1.4.9/tenable/io/scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -820,38 +820,42 @@
 
         :devportal:`scans: details <scans-details>`
 
         Args:
             scan_id (int or uuid): The unique identifier for the scan.
             history_id (int, optional):
                 The unique identifier for the instance of the scan.
-            history_uuid (uuid, optional):
+            history_uuid (uuid, optional)
                 The UUID for the instance of the scan.
 
         Returns:
             :obj:`dict`:
                 The scan result dictionary.
 
         Examples:
             Retrieve the latest results:
 
-            >>> results = tio.scans.results(1)
+            >>> results = tio.scans.results(419)
 
-            Retrieve a specific instance of the result set:
+            Retrieve a specific instance of the result set using history_id:
+
+            >>> results = tio.scans.results(419, history_id=15184619)
+
+            Retrieve a specific instance of the result set using history_uuid:
+
+            >>> results = tio.scans.results(419, history_uuid="123e4567-e89b-12d3-a456-426614174000")
 
-            >>> results = tio.scans.results(1, 1)
         '''
         params = dict()
 
         if history_id:
             params['history_id'] = self._check('history_id', history_id, int)
 
         if history_uuid:
-            params['history_uuid'] = self._check(
-                'history_uuid', history_uuid, 'scanner-uuid')
+            params['history_id'] = self._check('history_uuid', history_uuid, "uuid")
 
         return self._api.get('scans/{}'.format(
             scan_id), params=params).json()
 
     def export(self, scan_id, *filters, stream_hook=None, **kw):
         '''
         Export the scan report.
```

### Comparing `pyTenable-1.4.8/tenable/io/server.py` & `pyTenable-1.4.9/tenable/io/server.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/session.py` & `pyTenable-1.4.9/tenable/io/session.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/tags.py` & `pyTenable-1.4.9/tenable/io/tags.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/target_groups.py` & `pyTenable-1.4.9/tenable/io/target_groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/users.py` & `pyTenable-1.4.9/tenable/io/users.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/__init__.py` & `pyTenable-1.4.9/tenable/io/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/access_control.py` & `pyTenable-1.4.9/tenable/io/v3/access_control.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/base/endpoints/explore.py` & `pyTenable-1.4.9/tenable/io/v3/base/endpoints/explore.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/base/iterators/explore_iterator.py` & `pyTenable-1.4.9/tenable/io/v3/base/iterators/explore_iterator.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/base/schema/explore/filters.py` & `pyTenable-1.4.9/tenable/io/v3/base/schema/explore/filters.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/base/schema/explore/search.py` & `pyTenable-1.4.9/tenable/io/v3/base/schema/explore/search.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/explore/__init__.py` & `pyTenable-1.4.9/tenable/io/v3/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/explore/assets/api.py` & `pyTenable-1.4.9/tenable/io/v3/explore/assets/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/v3/explore/findings/api.py` & `pyTenable-1.4.9/tenable/io/v3/explore/findings/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/io/workbenches.py` & `pyTenable-1.4.9/tenable/io/workbenches.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/agent_groups.py` & `pyTenable-1.4.9/tenable/nessus/agent_groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/agents.py` & `pyTenable-1.4.9/tenable/nessus/agents.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/api.py` & `pyTenable-1.4.9/tenable/nessus/api.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/editor.py` & `pyTenable-1.4.9/tenable/nessus/editor.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/files.py` & `pyTenable-1.4.9/tenable/nessus/files.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/folders.py` & `pyTenable-1.4.9/tenable/nessus/folders.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/groups.py` & `pyTenable-1.4.9/tenable/nessus/groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/iterators/pagination.py` & `pyTenable-1.4.9/tenable/nessus/iterators/pagination.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/iterators/plugins.py` & `pyTenable-1.4.9/tenable/nessus/iterators/plugins.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/mail.py` & `pyTenable-1.4.9/tenable/nessus/mail.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/permissions.py` & `pyTenable-1.4.9/tenable/nessus/permissions.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/plugin_rules.py` & `pyTenable-1.4.9/tenable/nessus/plugin_rules.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/plugins.py` & `pyTenable-1.4.9/tenable/nessus/plugins.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/policies.py` & `pyTenable-1.4.9/tenable/nessus/policies.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/proxy.py` & `pyTenable-1.4.9/tenable/nessus/proxy.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/scanners.py` & `pyTenable-1.4.9/tenable/nessus/scanners.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/scans.py` & `pyTenable-1.4.9/tenable/nessus/scans.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/schema/pagination.py` & `pyTenable-1.4.9/tenable/nessus/schema/pagination.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/schema/scans.py` & `pyTenable-1.4.9/tenable/nessus/schema/scans.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/schema/settings.py` & `pyTenable-1.4.9/tenable/nessus/schema/settings.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/server.py` & `pyTenable-1.4.9/tenable/nessus/server.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/session.py` & `pyTenable-1.4.9/tenable/nessus/session.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/settings.py` & `pyTenable-1.4.9/tenable/nessus/settings.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/software_update.py` & `pyTenable-1.4.9/tenable/nessus/software_update.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/tokens.py` & `pyTenable-1.4.9/tenable/nessus/tokens.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/nessus/users.py` & `pyTenable-1.4.9/tenable/nessus/users.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/ot/assets.py` & `pyTenable-1.4.9/tenable/ot/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-'''
-Assets
+"""
+Events
 ======
 
-Methods described in this section relate to the the assets API.
-These methods can be accessed at ``TenableOT.assets``.
+Methods described in this section relate to the events API.
+These methods can be accessed at ``TenableOT.events``.
 
 .. rst-class:: hide-signature
-.. autoclass:: AssetsAPI
+.. autoclass:: EventsAPI
     :members:
-'''
+"""
 from typing import List, Optional
-from tenable.base.endpoint import APIEndpoint
-from tenable.ot.graphql.assets import (
-    ASSETS_QUERY,
-    ASSETS_QUERY_OBJECT_NAME,
-    AssetsSchema
-)
-from tenable.ot.graphql.definitions import GraphObject
-from tenable.ot.graphql.iterators import OTGraphIterator
 
+from tenable.ot.api import OTAPIBase
+from tenable.ot.graphql.iterators import OTGraphIterator
+from tenable.ot.graphql.query import EVENTS_QUERY
+from tenable.ot.graphql.schema.events import EventsSchema
 
-class AssetsAPI(APIEndpoint):
-    _path = 'assets'
 
-    def list(self,
-             filter: Optional[dict] = None,
-             search: Optional[str] = None,
-             sort: Optional[List[dict]] = None,
-             start_at: Optional[str] = None,
-             limit: Optional[int] = 200,
-             **kwargs):
-        '''
-        Retrieves a list of assets via the GraphQL API.
+class EventsAPI(OTAPIBase):
+    _path = "events"
+    schema_class = EventsSchema
+
+    def list(
+        self,
+        query_filter: Optional[dict] = None,
+        search: Optional[str] = None,
+        sort: Optional[List[dict]] = None,
+        start_at: Optional[str] = None,
+        limit: Optional[int] = 200,
+        **kwargs
+    ) -> OTGraphIterator:
+        """
+        Retrieves a list of events via the GraphQL API.
 
         Args:
-            filter(dict, optional):
+            query_filter(dict, optional):
                 A document as defined by Tenable.ot online documentation.
             search(str, optional):
                 A search string to further limit the response.
-            sort(list[dict], optional):
+            sort(List[dict], optional):
                 A list of order documents, each of which must contain both the
                 ``field`` and ``direction`` keys and may also contain the
                 optional ``function`` key. Default sort is by descending id
                 order. Please refer to Tenable.ot online documentation for more
                 information.
             start_at(str, optional):
                 The cursor to start the scan from (the default is an empty
@@ -52,30 +52,22 @@
                 is 200).
 
         Returns:
             :obj:`OTGraphIterator`:
                 An iterator object that will handle pagination of the data.
 
         Example:
-            >>>     for asset in tot.assets.list(limit=500):
-                        print(asset)
-        '''
+            >>>     for event in tot.events.list(limit=500):
+                        print(event)
+        """
         if not sort:
-            sort = [{'field': 'id', 'direction': 'DescNullLast'}]
+            sort = [{"field": "eventId", "direction": "DescNullLast"}]
 
-        query_variables = {
-            'search': search,
-            'sort': sort,
-            'startAt': start_at,
-            'limit': limit
-        }
-        if filter:
-            query_variables['filter'] = filter
-
-        graph_obj = GraphObject(
-            object_name=ASSETS_QUERY_OBJECT_NAME,
-            query=ASSETS_QUERY,
-            resp_schema=AssetsSchema,
-            query_variables=query_variables
+        return super().list(
+            query=EVENTS_QUERY,
+            query_filter=query_filter,
+            search=search,
+            sort=sort,
+            start_at=start_at,
+            limit=limit,
+            **kwargs
         )
-
-        return OTGraphIterator(self._api, graph_obj, **kwargs)
```

### Comparing `pyTenable-1.4.8/tenable/ot/graphql/iterators.py` & `pyTenable-1.4.9/tenable/ot/graphql/iterators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,81 @@
-'''
+"""
 GraphQL Tenable.ot API iterator.
-'''
+"""
+import json
+import typing
+from typing import Type
+
 from marshmallow.utils import EXCLUDE
 from restfly.iterator import APIIterator
+
 from tenable.ot.graphql.definitions import (
     GraphqlErrorSchema,
-    GraphqlParsingError
+    GraphqlParsingError,
+    GraphObject,
+    NodesSchema,
 )
 
+if typing.TYPE_CHECKING:
+    from tenable.ot.session import TenableOT
 
-class OTGraphIterator(APIIterator):
-    '''
-    Iterator class over Tenable.ot GraphQL connetions.
-    '''
 
-    def __init__(self, api, graph_object, **kwargs):
+class OTGraphIterator(APIIterator):
+    """
+    Iterator class over Tenable.ot GraphQL connections.
+    """
+
+    def __init__(
+        self,
+        api: "Type[TenableOT]",
+        graph_object: GraphObject,
+        **kwargs,
+    ):
         self._graph_object = graph_object
-        super().__init__(api, **kwargs)
+        self.api = api
+        super().__init__(
+            api=api,
+            **kwargs,
+        )
 
-    def _get_page(self):
-        '''
+    def _get_page(self) -> Type[NodesSchema]:
+        """
         Retrieves the next page of data.
-        '''
+        """
         graph_full_object = {
-            'query': self._graph_object.query,
-            'variables': self._graph_object.query_variables
+            "query": self._graph_object.query,
+            "variables": json.dumps(self._graph_object.query_variables),
         }
+        graphql_response_object = self._perform_request(graph_full_object)
+
+        self.page = self._graph_object.resp_schema().load(
+            graphql_response_object, unknown=EXCLUDE
+        )
+        if graphql_response_object.get("pageInfo"):
+            self._graph_object.query_variables["startAt"] = graphql_response_object[
+                "pageInfo"
+            ].get("endCursor", None)
 
-        resp = self._api.graphql(**graph_full_object)
-        if 'error' in resp:
+        return self.page
+
+    def _perform_request(
+        self,
+        graph_full_object: dict,
+    ) -> dict:
+        resp = self.api.graphql(**graph_full_object)
+        if "error" in resp:
             errors = GraphqlErrorSchema(many=True).load(
-                resp['error']['errors'], unknown=EXCLUDE)
+                resp["error"].get("errors", None), unknown=EXCLUDE
+            )
             raise errors[0]
-        if 'data' not in resp:
+        if "data" not in resp:
             raise GraphqlParsingError(
-                'graphql data field was not returned but no error occurred')
+                "graphql data field was not returned but no error occurred"
+            )
 
-        connection_object = resp['data'][self._graph_object.object_name]
-        if connection_object is None:
+        graphql_response_object = resp["data"][self._graph_object.object_name]
+        if graphql_response_object is None:
             raise GraphqlParsingError(
-                f'user requested object {self._graph_object.object_name}' +
-                ' was not returned')
-
-        self.page = self._graph_object.resp_schema().load(
-            connection_object, unknown=EXCLUDE)
-
-        self._graph_object.query_variables['startAt'] = connection_object[
-            'pageInfo'].get('endCursor', None)
+                f"user requested object {self._graph_object.object_name} was not returned"
+            )
 
-        return self.page
+        return graphql_response_object
```

### Comparing `pyTenable-1.4.8/tenable/ot/session.py` & `pyTenable-1.4.9/tenable/ot/session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-'''
+"""
 Tenable.ot
 ==========
 
 This package covers the Tenable.ot interface.
 
 .. autoclass:: TenableOT
     :members:
 
 
 .. toctree::
     :hidden:
     :glob:
 
     assets
-'''
+    events
+    plugins
+"""
 import os
 import warnings
+
 from tenable.base.platform import APIPlatform
 from tenable.ot.assets import AssetsAPI
+from tenable.ot.events import EventsAPI
+from tenable.ot.plugins import PluginsAPI
 
 
 class TenableOT(APIPlatform):
-    '''
+    """
     The Tenable.ot object is the primary interaction point for users to
-    interface with Tenable.io via the pyTenable library.  All of the API
+    interface with Tenable.OT via the pyTenable library.  All the API
     endpoint classes that have been written will be grafted onto this class.
 
     Args:
         api_key (str, optional):
             The user's API key for Tenable.ot.  If an api key isn't specified,
             then the library will attempt to read the environment variable
             ``TOT_API_KEY`` to acquire the key.
         url (str, optional):
             The base URL used to connect to the Tenable.ot application.  If a
-            url isn't specified, then the library will attempt to read the
+            URL isn't specified, then the library will attempt to read the
             environment variable ``TOT_URL`` to acquire the URL.
 
         **kwargs:
             arguments passed to :class:`tenable.base.platform.APIPlatform` for
             connection management.
 
 
     Examples:
         Basic Example:
 
         >>> from tenable.ot import TenableOT
-        >>> ot = TenableOT(secret_key='SECRET_KEY',
+        >>> ot = TenableOT(api_key='SECRET_KEY',
         ..                 url='https://ot.example.com')
 
         Example with proper identification:
 
-        >>> ot = TenableOT(secret_key='SECRET_KEY',
+        >>> ot = TenableOT(api_key='SECRET_KEY',
         ...                url='https://ot.example.com',
         ...                vendor='Company Name',
         ...                product='My Awesome Widget',
         ...                build='1.0.0')
 
         Example with proper identification leveraging environment variables for
         the connection parameters:
 
         >>> ot = TenableOT(vendor='Company', product='Widget', build='1.0.0')
-    '''
-    _env_base = 'TOT'
+    """
+
+    _env_base = "TOT"
     _ssl_verify = False
     _conv_json = True
 
     def _session_auth(self, **kwargs):  # noqa: PLW0221,PLW0613
-        msg = 'Session Auth isn\'t supported with the Tenable.ot APIs'
+        msg = "Session Auth isn't supported with the Tenable.ot APIs"
         warnings.warn(msg)
         self._log.warning(msg)
 
     def _key_auth(self, api_key, **kwargs):  # noqa: PLW0221,PLW0613
-        self._session.headers.update({
-            'X-APIKeys': f'key={api_key}'
-        })
-        self._auth_mech = 'keys'
+        self._session.headers.update({"X-APIKeys": f"key={api_key}"})
+        self._auth_mech = "keys"
 
     def _authenticate(self, **kwargs):
-        kwargs['_key_auth_dict'] = kwargs.get('_key_auth_dict', {
-            'api_key': kwargs.get('api_key',
-                                  os.getenv(f'{self._env_base}_API_KEY')
-                                  )
-        })
+        kwargs["_key_auth_dict"] = kwargs.get(
+            "_key_auth_dict",
+            {"api_key": kwargs.get("api_key", os.getenv(f"{self._env_base}_API_KEY"))},
+        )
         super()._authenticate(**kwargs)
 
     def graphql(self, **kwargs):
-        '''
+        """
         GraphQL Endpoint
 
         This singular method exposes the GraphQL API to the library.  As all
         keyword arguments are passed directly to the JSON body, it allows for a
         freeform interface into the GraphQL API.
 
         Args:
@@ -107,17 +110,33 @@
             ...                 type
             ...                 name
             ...                 criticality
             ...                 location
             ...             }
             ...         }
             ... \'\'\')
-        '''
-        return self.post('graphql', json=kwargs)
+        """
+        return self.post("graphql", json=kwargs)
 
     @property
     def assets(self):
-        '''
+        """
         The interface object for the
         :doc:`Tenable.ot Assets APIs <assets>`.
-        '''
+        """
         return AssetsAPI(self)
+
+    @property
+    def events(self):
+        """
+        The interface object for the
+        :doc:`Tenable.ot Events APIs <events>`.
+        """
+        return EventsAPI(self)
+
+    @property
+    def plugins(self):
+        """
+        The interface object for the
+        :doc:`Tenable.ot Plugins APIs <plugins>`.
+        """
+        return PluginsAPI(self)
```

### Comparing `pyTenable-1.4.8/tenable/reports/__init__.py` & `pyTenable-1.4.9/tenable/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/reports/nessusv2.py` & `pyTenable-1.4.9/tenable/reports/nessusv2.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/__init__.py` & `pyTenable-1.4.9/tenable/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/accept_risks.py` & `pyTenable-1.4.9/tenable/sc/accept_risks.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/alerts.py` & `pyTenable-1.4.9/tenable/sc/alerts.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/analysis.py` & `pyTenable-1.4.9/tenable/sc/analysis.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/asset_lists.py` & `pyTenable-1.4.9/tenable/sc/asset_lists.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/audit_files.py` & `pyTenable-1.4.9/tenable/sc/audit_files.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/base.py` & `pyTenable-1.4.9/tenable/sc/base.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/credentials.py` & `pyTenable-1.4.9/tenable/sc/credentials.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/current.py` & `pyTenable-1.4.9/tenable/sc/current.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/feeds.py` & `pyTenable-1.4.9/tenable/sc/feeds.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/files.py` & `pyTenable-1.4.9/tenable/sc/files.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/groups.py` & `pyTenable-1.4.9/tenable/sc/groups.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/organizations.py` & `pyTenable-1.4.9/tenable/sc/organizations.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/plugins.py` & `pyTenable-1.4.9/tenable/sc/plugins.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/policies.py` & `pyTenable-1.4.9/tenable/sc/policies.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/queries.py` & `pyTenable-1.4.9/tenable/sc/queries.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/recast_risks.py` & `pyTenable-1.4.9/tenable/sc/recast_risks.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/repositories.py` & `pyTenable-1.4.9/tenable/sc/repositories.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/roles.py` & `pyTenable-1.4.9/tenable/sc/roles.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/scan_instances.py` & `pyTenable-1.4.9/tenable/sc/scan_instances.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/scan_zones.py` & `pyTenable-1.4.9/tenable/sc/scan_zones.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/scanners.py` & `pyTenable-1.4.9/tenable/sc/scanners.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/scans.py` & `pyTenable-1.4.9/tenable/sc/scans.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/status.py` & `pyTenable-1.4.9/tenable/sc/status.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/system.py` & `pyTenable-1.4.9/tenable/sc/system.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/sc/users.py` & `pyTenable-1.4.9/tenable/sc/users.py`

 * *Files identical despite different names*

### Comparing `pyTenable-1.4.8/tenable/utils.py` & `pyTenable-1.4.9/tenable/utils.py`

 * *Files identical despite different names*

