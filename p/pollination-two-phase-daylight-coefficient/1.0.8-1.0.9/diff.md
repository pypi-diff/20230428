# Comparing `tmp/pollination-two-phase-daylight-coefficient-1.0.8.tar.gz` & `tmp/pollination-two-phase-daylight-coefficient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.0.8.tar", last modified: Mon Oct 31 14:36:47 2022, max compression
+gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.0.9.tar", last modified: Tue Nov  8 11:09:17 2022, max compression
```

## Comparing `pollination-two-phase-daylight-coefficient-1.0.8.tar` & `pollination-two-phase-daylight-coefficient-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 14:36:04.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 14:36:47.000000 pollination-two-phase-daylight-coefficient-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-10-31 14:35:38.000000 pollination-two-phase-daylight-coefficient-1.0.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      530 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 11:08:27.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 11:09:17.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-08 11:07:58.000000 pollination-two-phase-daylight-coefficient-1.0.9/tests/validation_test.py
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/.github/workflows/ci.yaml` & `pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/.github/workflows/tests.yaml` & `pollination-two-phase-daylight-coefficient-1.0.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/LICENSE` & `pollination-two-phase-daylight-coefficient-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.0.8
+Version: 1.0.9
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/_prepare_folder.py` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/_prepare_folder.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/entry.py` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination/two_phase_daylight_coefficient/two_phase/entry.py` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination/two_phase_daylight_coefficient/two_phase/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.0.8
+Version: 1.0.9
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt` & `pollination-two-phase-daylight-coefficient-1.0.9/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.0.8/setup.py` & `pollination-two-phase-daylight-coefficient-1.0.9/setup.py`

 * *Files identical despite different names*

