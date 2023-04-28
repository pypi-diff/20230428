# Comparing `tmp/stissplice-1.0.2.tar.gz` & `tmp/stissplice-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stissplice-1.0.2.tar", last modified: Tue Apr 25 14:43:44 2023, max compression
+gzip compressed data, was "stissplice-1.0.3.tar", last modified: Fri Apr 28 17:41:57 2023, max compression
```

## Comparing `stissplice-1.0.2.tar` & `stissplice-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-25 14:43:33.000000 stissplice-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:43:44.699745 stissplice-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 14:43:33.000000 stissplice-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:43:44.699745 stissplice-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 14:43:33.000000 stissplice-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/stissplice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32299 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/splicer.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 14:43:33.000000 stissplice-1.0.2/stissplice/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:43:44.699745 stissplice-1.0.2/stissplice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 14:43:44.000000 stissplice-1.0.2/stissplice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 17:41:44.000000 stissplice-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:41:57.794852 stissplice-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-28 17:41:44.000000 stissplice-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:41:57.794852 stissplice-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 17:41:44.000000 stissplice-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/stissplice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32529 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/splicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-28 17:41:44.000000 stissplice-1.0.3/stissplice/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:41:57.794852 stissplice-1.0.3/stissplice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 17:41:57.000000 stissplice-1.0.3/stissplice.egg-info/top_level.txt
```

### Comparing `stissplice-1.0.2/LICENSE` & `stissplice-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.2/PKG-INFO` & `stissplice-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `stissplice-1.0.2/README.md` & `stissplice-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.2/setup.py` & `stissplice-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist upload")
     sys.exit()
 
 setup(
     name="stissplice",
-    version="1.0.2",
+    version="1.0.3",
     author="Leonardo dos Santos",
     author_email="ldsantos@stsci.edu",
     packages=["stissplice"],
     url="https://github.com/ladsantos/stissplice",
     license="MIT",
     description="Splicer of STIS Echelle Spectra from Hubble Space Telescope",
     install_requires=[line.strip() for line in
```

### Comparing `stissplice-1.0.2/stissplice/splicer.py` & `stissplice-1.0.3/stissplice/splicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,19 @@
         else:
             overlap_idx_012 = None
         if idx[2] < idx[1]:
             overlap_idx_12 = np.arange(idx[0], idx[2], 1)
             overlap_idx_123 = None
             unique_idx_2 = np.arange(idx[2], idx[1], 1)
             overlap_idx_23 = np.arange(idx[1], idx[3], 1)
+        elif idx[2] == idx[1]:
+            overlap_idx_12 = np.arange(idx[0], idx[2], 1)
+            overlap_idx_123 = None
+            unique_idx_2 = np.array([idx[2], ])
+            overlap_idx_23 = np.arange(idx[1], idx[3], 1)
         else:
             overlap_idx_12 = np.arange(idx[0], idx[1], 1)
             overlap_idx_123 = np.arange(idx[1], idx[2], 1)
             unique_idx_2 = None
             overlap_idx_23 = np.arange(idx[2], idx[3], 1)
         if idx[3] < 1023:
             overlap_idx_234 = np.arange(idx[3], 1023, 1)
```

### Comparing `stissplice-1.0.2/stissplice/tools.py` & `stissplice-1.0.3/stissplice/tools.py`

 * *Files identical despite different names*

### Comparing `stissplice-1.0.2/stissplice.egg-info/PKG-INFO` & `stissplice-1.0.3/stissplice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stissplice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Splicer of STIS Echelle Spectra from Hubble Space Telescope
 Home-page: https://github.com/ladsantos/stissplice
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

