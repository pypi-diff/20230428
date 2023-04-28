# Comparing `tmp/gkligo-0.0.8.tar.gz` & `tmp/gkligo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.8.tar", last modified: Fri Apr 28 12:20:12 2023, max compression
+gzip compressed data, was "gkligo-0.0.9.tar", last modified: Fri Apr 28 13:12:21 2023, max compression
```

## Comparing `gkligo-0.0.8.tar` & `gkligo-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.890464 gkligo-0.0.8/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.8/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.8/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:20:12.889986 gkligo-0.0.8/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.8/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.882553 gkligo-0.0.8/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.8/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:19:09.000000 gkligo-0.0.8/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.885733 gkligo-0.0.8/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.8/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.889200 gkligo-0.0.8/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.8/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.8/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.8/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.8/gkligo/scripts/python/config_reports_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)     8348 2023-04-28 12:18:55.000000 gkligo-0.0.8/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.8/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.8/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:20:12.885320 gkligo-0.0.8/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 12:20:12.000000 gkligo-0.0.8/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 12:20:12.890636 gkligo-0.0.8/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.8/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.209688 gkligo-0.0.9/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.9/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.9/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 13:12:21.209123 gkligo-0.0.9/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.9/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.199647 gkligo-0.0.9/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.9/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:33:16.000000 gkligo-0.0.9/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.203371 gkligo-0.0.9/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.9/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.208300 gkligo-0.0.9/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.9/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:33:16.000000 gkligo-0.0.9/gkligo/scripts/python/__version__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.9/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.9/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.9/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     8999 2023-04-28 13:09:16.000000 gkligo-0.0.9/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.9/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.9/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 13:12:21.202732 gkligo-0.0.9/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      623 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 13:12:21.000000 gkligo-0.0.9/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 13:12:21.209890 gkligo-0.0.9/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.9/setup.py
```

### Comparing `gkligo-0.0.8/LICENSE` & `gkligo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.8/PKG-INFO` & `gkligo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.8
+Version: 0.0.9
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.8/README.md` & `gkligo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.8/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.0.9/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 mocpy
 
 Usage:
   %s <configFile> <action> [--writeMap] [--writeMOC] [--directory=<directory>] [--contours=<contours>] [--pidfile=<pidfile>] [--logfile=<logfile>] [--daemonErrFile=<deamonErrFile>] [--daemonOutFile=<deamonOutFile>] [--terminal]
   %s (-h | --help)
   %s --version
 
-where action is start|stop|restart
+where action is start|stop|restart|listen
+
+If action is listen, start in non-daemon mode. Otherwise use daemon mode.
 
 Options:
   -h --help                         Show this screen.
   --version                         Show version.
   --writeMap                        Write the Map file
   --writeMOC                        Write the MOC file (selected contour)
   --directory=<directory>           Directory to where the maps and MOCs will be written [default: /tmp].
@@ -36,14 +38,15 @@
   %s config.yaml start --writeMap --writeMOC --directory=/tmp --contours=90
   %s config.yaml start --writeMOC --directory=/tmp --contours=90,50,10
 
 """
 import sys
 __doc__ = __doc__ % (sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0])
 from docopt import docopt
+from __version__ import __version__
 
 from gcn_kafka import Consumer
 import json
 import base64
 from gkutils.commonutils import Struct, cleanOptions
 from io import BytesIO
 import daemon
@@ -203,41 +206,52 @@
         ) as context:
         listen(options)
 
 
 def main():
     """main.
     """
-    opts = docopt(__doc__, version='0.1')
+    opts = docopt(__doc__, version=__version__)
     opts = cleanOptions(opts)
 
     # Use utils.Struct to convert the dict into an object for compatibility with old optparse code.
     options = Struct(**opts)
 
 
-    if options.action not in ['start', 'stop', 'restart']:
-        sys.stderr.write('Valid options for action are start|stop|restart\n')
+    if options.action not in ['start', 'stop', 'restart', 'listen']:
+        sys.stderr.write('Valid options for action are start|stop|restart|listen\n')
         sys.exit(1)
 
+    # First check that the listen option has been chosen. If so, start listening to the Kafka
+    # stream immediately, without daemonisation.
+
+    if options.action == 'listen':
+        if os.path.exists(options.pidfile):
+            with open(options.pidfile, mode='r') as f:
+                pid = f.read().strip()
+                sys.stderr.write("\nDaemon is already running (PID = %s). Kill the existing daemon first. E.g. use the stop option.\n" % pid)
+        else:
+            listen(options)
+    
     if options.action == 'start':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
-                sys.stderr.write("Daemon is already running (PID = %s). Stop and restart if you want to restart it.\n" % pid)
+                sys.stderr.write("\nDaemon is already running (PID = %s). Stop and restart if you want to restart it.\n" % pid)
         else:
             startDaemon(options)
 
     if options.action == 'stop':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
             print("Stopping daemon (PID = %s)." % pid)
             os.kill(int(pid), signal.SIGTERM)
         else:
-            sys.stderr.write("Daemon is not running.\n")
+            sys.stderr.write("\nDaemon is not running.\n")
 
 
     if options.action == 'restart':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
             print("Stopping daemon (PID = %s)." % pid)
```

### Comparing `gkligo-0.0.8/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.0.9/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.8/gkligo/scripts/python/testDaemon.py` & `gkligo-0.0.9/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.8/gkligo.egg-info/PKG-INFO` & `gkligo-0.0.9/gkligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.8
+Version: 0.0.9
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.8/gkligo.egg-info/SOURCES.txt` & `gkligo-0.0.9/gkligo.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 gkligo.egg-info/SOURCES.txt
 gkligo.egg-info/dependency_links.txt
 gkligo.egg-info/entry_points.txt
 gkligo.egg-info/requires.txt
 gkligo.egg-info/top_level.txt
 gkligo/scripts/__init__.py
 gkligo/scripts/python/__init__.py
+gkligo/scripts/python/__version__.py
 gkligo/scripts/python/config_download_example.yaml
 gkligo/scripts/python/config_reports.yaml
 gkligo/scripts/python/config_reports_example.yaml
 gkligo/scripts/python/downloadGWAlerts.py
 gkligo/scripts/python/generateGWReports.py
 gkligo/scripts/python/testDaemon.py
```

### Comparing `gkligo-0.0.8/setup.py` & `gkligo-0.0.9/setup.py`

 * *Files identical despite different names*

