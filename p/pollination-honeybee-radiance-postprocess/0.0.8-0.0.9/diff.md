# Comparing `tmp/pollination-honeybee-radiance-postprocess-0.0.8.tar.gz` & `tmp/pollination-honeybee-radiance-postprocess-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-radiance-postprocess-0.0.8.tar", last modified: Wed Sep 28 07:16:48 2022, max compression
+gzip compressed data, was "dist/pollination-honeybee-radiance-postprocess-0.0.9.tar", last modified: Mon Oct 10 15:51:36 2022, max compression
```

## Comparing `pollination-honeybee-radiance-postprocess-0.0.8.tar` & `pollination-honeybee-radiance-postprocess-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/leed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/post_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 07:16:00.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-09-28 07:16:48.000000 pollination-honeybee-radiance-postprocess-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-09-28 07:15:36.000000 pollination-honeybee-radiance-postprocess-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/leed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/sky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/translate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/two_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 15:50:46.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-10 15:51:36.000000 pollination-honeybee-radiance-postprocess-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-10 15:50:23.000000 pollination-honeybee-radiance-postprocess-0.0.9/setup.py
```

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/.github/workflows/ci.yaml` & `pollination-honeybee-radiance-postprocess-0.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/.github/workflows/dependency-release.yaml` & `pollination-honeybee-radiance-postprocess-0.0.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/LICENSE` & `pollination-honeybee-radiance-postprocess-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/PKG-INFO` & `pollination-honeybee-radiance-postprocess-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-radiance-postprocess
-Version: 0.0.8
+Version: 0.0.9
 Summary: Honeybee Radiance Post Process plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-honeybee-radiance-postprocess
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/__init__.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/grid.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/grid.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/leed.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/leed.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/post_process.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/post_process.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/sky.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/sky.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination/honeybee_radiance_postprocess/translate.py` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination/honeybee_radiance_postprocess/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/PKG-INFO` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-radiance-postprocess
-Version: 0.0.8
+Version: 0.0.9
 Summary: Honeybee Radiance Post Process plugin for Pollination.
 Home-page: https://github.com/pollination/pollination-honeybee-radiance-postprocess
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/pollination_honeybee_radiance_postprocess.egg-info/SOURCES.txt` & `pollination-honeybee-radiance-postprocess-0.0.9/pollination_honeybee_radiance_postprocess.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 .github/workflows/dependency-release.yaml
 pollination/honeybee_radiance_postprocess/__init__.py
 pollination/honeybee_radiance_postprocess/grid.py
 pollination/honeybee_radiance_postprocess/leed.py
 pollination/honeybee_radiance_postprocess/post_process.py
 pollination/honeybee_radiance_postprocess/sky.py
 pollination/honeybee_radiance_postprocess/translate.py
+pollination/honeybee_radiance_postprocess/two_phase.py
 pollination_honeybee_radiance_postprocess.egg-info/PKG-INFO
 pollination_honeybee_radiance_postprocess.egg-info/SOURCES.txt
 pollination_honeybee_radiance_postprocess.egg-info/dependency_links.txt
 pollination_honeybee_radiance_postprocess.egg-info/not-zip-safe
 pollination_honeybee_radiance_postprocess.egg-info/requires.txt
 pollination_honeybee_radiance_postprocess.egg-info/top_level.txt
```

### Comparing `pollination-honeybee-radiance-postprocess-0.0.8/setup.py` & `pollination-honeybee-radiance-postprocess-0.0.9/setup.py`

 * *Files identical despite different names*

