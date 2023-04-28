# Comparing `tmp/iterapi-1.2.6.tar.gz` & `tmp/iterapi-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterapi-1.2.6.tar", last modified: Mon Oct  3 04:11:06 2022, max compression
+gzip compressed data, was "iterapi-1.2.7.tar", last modified: Fri Apr 28 13:43:42 2023, max compression
```

## Comparing `iterapi-1.2.6.tar` & `iterapi-1.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:11:06.735116 iterapi-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-03 04:10:54.000000 iterapi-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-03 04:10:54.000000 iterapi-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-10-03 04:11:06.735116 iterapi-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-10-03 04:10:54.000000 iterapi-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:11:06.731116 iterapi-1.2.6/iterapi/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-03 04:10:54.000000 iterapi-1.2.6/iterapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7391 2022-10-03 04:10:54.000000 iterapi-1.2.6/iterapi/iterapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 04:11:06.735116 iterapi-1.2.6/iterapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-10-03 04:11:06.000000 iterapi-1.2.6/iterapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-03 04:11:06.000000 iterapi-1.2.6/iterapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 04:11:06.000000 iterapi-1.2.6/iterapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-03 04:11:06.000000 iterapi-1.2.6/iterapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-03 04:11:06.000000 iterapi-1.2.6/iterapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 04:11:06.735116 iterapi-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-03 04:10:54.000000 iterapi-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:42.010380 iterapi-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 13:43:29.000000 iterapi-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 13:43:29.000000 iterapi-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-28 13:43:42.010380 iterapi-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-28 13:43:29.000000 iterapi-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:42.010380 iterapi-1.2.7/iterapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 13:43:29.000000 iterapi-1.2.7/iterapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-28 13:43:29.000000 iterapi-1.2.7/iterapi/iterapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:43:42.010380 iterapi-1.2.7/iterapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-28 13:43:41.000000 iterapi-1.2.7/iterapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 13:43:41.000000 iterapi-1.2.7/iterapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:43:41.000000 iterapi-1.2.7/iterapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 13:43:41.000000 iterapi-1.2.7/iterapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 13:43:41.000000 iterapi-1.2.7/iterapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:43:42.010380 iterapi-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-28 13:43:29.000000 iterapi-1.2.7/setup.py
```

### Comparing `iterapi-1.2.6/LICENSE` & `iterapi-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iterapi-1.2.6/PKG-INFO` & `iterapi-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterapi
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python API to student portal of ITER
 Home-page: https://github.com/SubhrajitPrusty/iterapi
 Author: Subhrajit Prusty
 Author-email: subhrajit1997@gmail.com
 License: MIT
 Keywords: api ITER development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iterapi-1.2.6/README.md` & `iterapi-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `iterapi-1.2.6/iterapi/iterapi.py` & `iterapi-1.2.7/iterapi/iterapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class Student(object):
     """
     Student Object containing functions to retrieve various student details
     """
 
-    DOMAIN = "http://115.240.101.71:8282"
+    DOMAIN = "http://115.240.101.51:8282"
     LOGIN_URL = DOMAIN+"/CampusPortalSOA/login"
     STUDENTINFO_URL = DOMAIN+"/CampusPortalSOA/studentinfo"
     REGID_URL = DOMAIN+"/CampusPortalSOA/studentSemester/lov"
     STUDENTPHOTO_URL = DOMAIN+"/CampusPortalSOA/image/studentPhoto"  # noqa: E501
     STUDENTRESULT_URL = DOMAIN+"/CampusPortalSOA/stdrst"
     # styno = int(1-8) semester number
     RESULTDETAIL_URL = DOMAIN+"/CampusPortalSOA/rstdtl"
```

### Comparing `iterapi-1.2.6/iterapi.egg-info/PKG-INFO` & `iterapi-1.2.7/iterapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterapi
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python API to student portal of ITER
 Home-page: https://github.com/SubhrajitPrusty/iterapi
 Author: Subhrajit Prusty
 Author-email: subhrajit1997@gmail.com
 License: MIT
 Keywords: api ITER development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iterapi-1.2.6/setup.py` & `iterapi-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with contextlib.suppress(Exception):
         with open('README.md') as f:
             return f.read()
 
 
 setup(
     name='iterapi',
-    version='1.2.6',
+    version='1.2.7',
     description='Python API to student portal of ITER',
 
     long_description=readme(),
     long_description_content_type='text/markdown',
 
     url='https://github.com/SubhrajitPrusty/iterapi',
     author='Subhrajit Prusty',
```

