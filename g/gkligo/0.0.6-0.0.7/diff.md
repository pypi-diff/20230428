# Comparing `tmp/gkligo-0.0.6.tar.gz` & `tmp/gkligo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.6.tar", last modified: Mon Apr 24 16:54:01 2023, max compression
+gzip compressed data, was "gkligo-0.0.7.tar", last modified: Fri Apr 28 12:08:21 2023, max compression
```

## Comparing `gkligo-0.0.6.tar` & `gkligo-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 16:54:01.032847 gkligo-0.0.6/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.6/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.6/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 16:54:01.032340 gkligo-0.0.6/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.6/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 16:54:01.020028 gkligo-0.0.6/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.6/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 16:53:21.000000 gkligo-0.0.6/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 16:54:01.023811 gkligo-0.0.6/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.6/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 16:54:01.031190 gkligo-0.0.6/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.6/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.6/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.6/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.6/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.6/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.6/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.6/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 16:54:01.023094 gkligo-0.0.6/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 16:54:00.000000 gkligo-0.0.6/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 16:54:01.033047 gkligo-0.0.6/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.6/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.588514 gkligo-0.0.7/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.7/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.7/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:08:21.588012 gkligo-0.0.7/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.7/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.576314 gkligo-0.0.7/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.7/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 12:06:33.000000 gkligo-0.0.7/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.580357 gkligo-0.0.7/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.7/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.586823 gkligo-0.0.7/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.7/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.7/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.7/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.7/gkligo/scripts/python/config_reports_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)     8284 2023-04-28 12:05:21.000000 gkligo-0.0.7/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.0.7/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.0.7/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-28 12:08:21.579512 gkligo-0.0.7/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-28 12:08:21.000000 gkligo-0.0.7/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-28 12:08:21.588755 gkligo-0.0.7/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.7/setup.py
```

### Comparing `gkligo-0.0.6/LICENSE` & `gkligo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.6/PKG-INFO` & `gkligo-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.6
+Version: 0.0.7
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.6/README.md` & `gkligo-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.6/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.0.7/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,17 +49,34 @@
 import daemon
 from daemon import pidfile
 import signal
 import os
 import time
 import logging
 
-debug_p = True
+def shutdown(signum, frame):  # signum and frame are mandatory
+    """shutdown.
+
+    Args:
+        signum:
+        frame:
+    """
+    sys.stdout.write("\nOuch...\n")
+    sys.exit(0)
+
 
 def writeMOC(inputFilePointer, outputMOCName, contour, logger):
+    """writeMOC.
+
+    Args:
+        inputFilePointer:
+        outputMOCName:
+        contour:
+        logger:
+    """
     from astropy.table import Table
     from astropy import units as u
     import astropy_healpix as ah
     import numpy as np
     import math
     from ligo.skymap.moc import uniq2pixarea
 
@@ -93,17 +110,22 @@
     skymap = skymap[:i]
     skymap = skymap['UNIQ',]
     logger.info(skymap.info)
     skymap.write(outputMOCName, format='fits', overwrite=True)
     logger.info('MOC file %s written' % outputMOCName)
 
 
-def runLigoDaemon(options):
-    ### This does the "work" of the daemon
+def listen(options):
+    """listen.
 
+    Args:
+        options:
+    """
+    pid = os.getpid()
+    sys.stdout.write("\nListening... PID is %s\n" % pid)
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.INFO)
 
     fh = logging.FileHandler(options.logfile)
     fh.setLevel(logging.INFO)
 
     formatstr = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
@@ -117,27 +139,23 @@
     with open(options.configFile) as yaml_file:
         config = yaml.safe_load(yaml_file)
 
     client_id = config['client_id']
     client_secret = config['client_secret']
     topic = config['topics']
 
-    # Connect as a consumer.
-    # Warning: don't share the client secret with others.
     consumer = Consumer(client_id=client_id,
                         client_secret=client_secret)
 
-    # Subscribe to topics and receive alerts
     consumer.subscribe(['igwn.gwalert'])
 
     while True:
-        for message in consumer.consume():
+        # Non zero timeout is required, otherwise consume blocks termination signals.
+        for message in consumer.consume(timeout=5):
             dataDict = json.loads(message.value().decode('utf-8'))
-            #for k, v in dataDict.items():
-            #    print(k, v)
             try:
                 superEventId = dataDict['superevent_id']
                 alertTimeStamp = dataDict['time_created'].replace(' ','T')
                 alertType = dataDict['alert_type']
                 alertName = superEventId + '_' + alertType + '_' + alertTimeStamp
                 logger.info("Alert Received: %s" % alertName) # Future version of this script will log the output.
                 if dataDict['event'] is not None and options.writeMap:
@@ -157,45 +175,42 @@
 
             except KeyError as e:
                 logger.error(e)
                 pass
             logger.info("")
 
 
-def start_daemon(options):
-    ### This launches the daemon in its context
-
-    global debug_p
-
-    if debug_p:
-        print("eg_daemon: entered run()")
-        print("eg_daemon: pidfile = {}    logfile = {}".format(options.pidfile, options.logfile))
-        print("eg_daemon: about to start daemonization")
+def startDaemon(options):
+    """startDaemon.
 
+    Args:
+        options:
+    """
 
     if options.terminal:
         err = sys.stderr
         out = sys.stdout
     else:
         out = open(options.daemonOutFile, 'w')
         err = open(options.daemonErrFile, 'w')
 
-    ### XXX pidfile is a context
     with daemon.DaemonContext(
         working_directory='/tmp',
         umask=0o002,
         pidfile=pidfile.TimeoutPIDLockFile(options.pidfile),
         stdout=out,
-        stderr=err
+        stderr=err,
+        signal_map={ signal.SIGTERM: shutdown }
         ) as context:
-        runLigoDaemon(options)
-
+        listen(options)
 
 
 def main():
+    """main.
+    """
     opts = docopt(__doc__, version='0.1')
     opts = cleanOptions(opts)
 
     # Use utils.Struct to convert the dict into an object for compatibility with old optparse code.
     options = Struct(**opts)
 
 
@@ -205,53 +220,32 @@
 
     if options.action == 'start':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
                 sys.stderr.write("Daemon is already running (PID = %s). Stop and restart if you want to restart it.\n" % pid)
         else:
-            start_daemon(options)
-            # Give the daemon a few seconds to start
-            time.sleep(2)
-            with open(options.pidfile, mode='r') as f:
-                pid = f.read().strip()
-                print("Starting Daemon. PID = %s" % pid)
+            startDaemon(options)
 
     if options.action == 'stop':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
             print("Stopping daemon (PID = %s)." % pid)
-            os.kill(int(pid), signal.SIGKILL)
-            time.sleep(2)
-            if os.path.exists(options.pidfile):
-                os.remove(options.pidfile)
+            os.kill(int(pid), signal.SIGTERM)
         else:
             sys.stderr.write("Daemon is not running.\n")
 
 
     if options.action == 'restart':
         if os.path.exists(options.pidfile):
             with open(options.pidfile, mode='r') as f:
                 pid = f.read().strip()
             print("Stopping daemon (PID = %s)." % pid)
-            os.kill(pid, signal.SIGKILL)
-            time.sleep(2)
-            if os.path.exists(options.pidfile):
-                os.remove(options.pidfile)
+            os.kill(pid, signal.SIGTERM)
         else:
-            start_daemon(options)
-            time.sleep(2)
-            if os.path.exists(options.pidfile):
-                with open(options.pidfile, mode='r') as f:
-                    pid = f.read().strip()
-                print("Starting Daemon. PID = %s" % pid)
-            else:
-                print ("Daemon not started.")
-
-
-
+            startDaemon(options)
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `gkligo-0.0.6/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.0.7/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.6/gkligo/scripts/python/testDaemon.py` & `gkligo-0.0.7/gkligo/scripts/python/testDaemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import os
 import time
 import logging
 import daemon
 from daemon import pidfile
 from gkutils.commonutils import cleanOptions, Struct
-
+import signal
 debug_p = True
 
 def do_something(options):
     ### This does the "work" of the daemon
 
     logger = logging.getLogger('eg_daemon')
     logger.setLevel(logging.INFO)
@@ -49,30 +49,40 @@
     while True:
         logger.debug("this is a DEBUG message")
         logger.info("this is an INFO message")
         logger.error("this is an ERROR message")
         time.sleep(5)
 
 
+def shutdown(signum, frame):  # signum and frame are mandatory
+    sys.stdout.write("Ah ballix...\n")
+    sys.exit(0)
+
 def start_daemon(options):
     ### This launches the daemon in its context
 
     global debug_p
 
     if debug_p:
         print("eg_daemon: entered run()")
         print("eg_daemon: pidf = {}    logf = {}".format(options.pidfile, options.logfile))
         print("eg_daemon: about to start daemonization")
         print(type(options.pidfile), type(options.logfile))
 
+    out = sys.stdout
+    err = sys.stderr
+
     ### XXX pidfile is a context
     with daemon.DaemonContext(
-        working_directory='/tmp/eg_daemon',
+        working_directory='/tmp',
         umask=0o002,
         pidfile=pidfile.TimeoutPIDLockFile(options.pidfile),
+        signal_map={ signal.SIGTERM: shutdown },
+        stdout=out,
+        stderr=err,
         ) as context:
         do_something(options)
 
 
 if __name__ == "__main__":
     opts = docopt(__doc__, version='0.1')
     opts = cleanOptions(opts)
```

### Comparing `gkligo-0.0.6/gkligo.egg-info/PKG-INFO` & `gkligo-0.0.7/gkligo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.6
+Version: 0.0.7
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.6/gkligo.egg-info/SOURCES.txt` & `gkligo-0.0.7/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.6/setup.py` & `gkligo-0.0.7/setup.py`

 * *Files identical despite different names*

