# Comparing `tmp/gkligo-0.0.7.tar.gz` & `tmp/gkligo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.7.tar", last modified: Fri Apr 28 12:08:21 2023, max compression
+gzip compressed data, was "gkligo-0.0.8.tar", last modified: Fri Apr 28 12:20:12 2023, max compression
```

## Comparing `gkligo-0.0.7.tar` & `gkligo-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.588514 gkligo-0.0.7/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.7/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.7/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:08:21.588012 gkligo-0.0.7/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.7/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.576314 gkligo-0.0.7/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.7/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:06:33.000000 gkligo-0.0.7/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.580357 gkligo-0.0.7/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.7/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.586823 gkligo-0.0.7/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.7/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.7/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.7/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.7/gkligo/scripts/python/config_reports_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)     8284 2023-04-28 12:05:21.000000 gkligo-0.0.7/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.7/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.7/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.579512 gkligo-0.0.7/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 12:08:21.588755 gkligo-0.0.7/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.7/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.890464 gkligo-0.0.8/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.8/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.8/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:20:12.889986 gkligo-0.0.8/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.8/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.882553 gkligo-0.0.8/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.8/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:19:09.000000 gkligo-0.0.8/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.885733 gkligo-0.0.8/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.8/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.889200 gkligo-0.0.8/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.8/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.8/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.8/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.8/gkligo/scripts/python/config_reports_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)     8348 2023-04-28 12:18:55.000000 gkligo-0.0.8/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.8/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.8/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.885320 gkligo-0.0.8/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 12:20:12.890636 gkligo-0.0.8/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.8/setup.py
```

### Comparing `gkligo-0.0.7/LICENSE` & `gkligo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.7/PKG-INFO` & `gkligo-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.7
+Version: 0.0.8
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.7/README.md` & `gkligo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.7/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.0.8/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,17 @@
 
 
     if options.action == 'restart':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
             print("Stopping daemon (PID = %s)." % pid)
-            os.kill(pid, signal.SIGTERM)
+            os.kill(int(pid), signal.SIGTERM)
+            time.sleep(5)
+            startDaemon(options)
         else:
             startDaemon(options)
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gkligo-0.0.7/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.0.8/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.7/gkligo/scripts/python/testDaemon.py` & `gkligo-0.0.8/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.7/gkligo.egg-info/PKG-INFO` & `gkligo-0.0.8/gkligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.7
+Version: 0.0.8
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.7/gkligo.egg-info/SOURCES.txt` & `gkligo-0.0.8/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.7/setup.py` & `gkligo-0.0.8/setup.py`

 * *Files identical despite different names*

