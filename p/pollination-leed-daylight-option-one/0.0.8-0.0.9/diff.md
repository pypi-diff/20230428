# Comparing `tmp/pollination-leed-daylight-option-one-0.0.8.tar.gz` & `tmp/pollination-leed-daylight-option-one-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-leed-daylight-option-one-0.0.8.tar", last modified: Tue Nov  8 11:16:13 2022, max compression
+gzip compressed data, was "dist/pollination-leed-daylight-option-one-0.0.9.tar", last modified: Thu Dec 22 11:14:21 2022, max compression
```

## Comparing `pollination-leed-daylight-option-one-0.0.8.tar` & `pollination-leed-daylight-option-one-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination/leed_daylight_option_one/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/pollination/leed_daylight_option_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/pollination/leed_daylight_option_one/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:15:35.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:16:13.000000 pollination-leed-daylight-option-one-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-08 11:15:16.000000 pollination-leed-daylight-option-one-0.0.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination/leed_daylight_option_one/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/pollination/leed_daylight_option_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/pollination/leed_daylight_option_one/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 11:13:41.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 11:14:21.000000 pollination-leed-daylight-option-one-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-22 11:13:19.000000 pollination-leed-daylight-option-one-0.0.9/tests/validation_test.py
```

### Comparing `pollination-leed-daylight-option-one-0.0.8/.github/workflows/ci.yaml` & `pollination-leed-daylight-option-one-0.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-leed-daylight-option-one-0.0.8/.github/workflows/tests.yaml` & `pollination-leed-daylight-option-one-0.0.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-leed-daylight-option-one-0.0.8/LICENSE` & `pollination-leed-daylight-option-one-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-leed-daylight-option-one-0.0.8/PKG-INFO` & `pollination-leed-daylight-option-one-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-leed-daylight-option-one
-Version: 0.0.8
+Version: 0.0.9
 Summary: LEED daylight option I recipe for Pollination.
 Home-page: https://github.com/pollination/leed-daylight-option-one
 Author: pollination
 Author-email: info@pollination.solutions
 Maintainer: mikkel, pollination
 Maintainer-email: mikkel@ladybug.tools, info@pollination.solutions
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-leed-daylight-option-one-0.0.8/pollination/leed_daylight_option_one/entry.py` & `pollination-leed-daylight-option-one-0.0.9/pollination/leed_daylight_option_one/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/PKG-INFO` & `pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-leed-daylight-option-one
-Version: 0.0.8
+Version: 0.0.9
 Summary: LEED daylight option I recipe for Pollination.
 Home-page: https://github.com/pollination/leed-daylight-option-one
 Author: pollination
 Author-email: info@pollination.solutions
 Maintainer: mikkel, pollination
 Maintainer-email: mikkel@ladybug.tools, info@pollination.solutions
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-leed-daylight-option-one-0.0.8/pollination_leed_daylight_option_one.egg-info/SOURCES.txt` & `pollination-leed-daylight-option-one-0.0.9/pollination_leed_daylight_option_one.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-leed-daylight-option-one-0.0.8/setup.py` & `pollination-leed-daylight-option-one-0.0.9/setup.py`

 * *Files identical despite different names*

