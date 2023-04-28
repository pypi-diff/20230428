# Comparing `tmp/langmuir_trough-0.6.0.tar.gz` & `tmp/langmuir_trough-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langmuir_trough-0.6.0.tar", last modified: Thu Mar 30 13:19:07 2023, max compression
+gzip compressed data, was "langmuir_trough-0.7.0.tar", last modified: Fri Apr 28 18:23:38 2023, max compression
```

## Comparing `langmuir_trough-0.6.0.tar` & `langmuir_trough-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-30 13:19:07.898022 langmuir_trough-0.6.0/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-30 13:19:07.894537 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)     9262 2023-03-30 13:19:07.000000 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-03-30 13:19:07.000000 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-03-30 13:19:07.000000 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-03-30 13:19:07.000000 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-03-30 13:19:07.000000 langmuir_trough-0.6.0/Langmuir_Trough.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)     9262 2023-03-30 13:19:07.897858 langmuir_trough-0.6.0/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     8608 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-30 13:19:07.894667 langmuir_trough-0.6.0/Trough/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-30 13:19:07.895597 langmuir_trough-0.6.0/Trough/Trough_Control/
--rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_Control/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_Control/message_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_Control/simulation.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    34195 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_Control/trough_util.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-03-30 13:19:07.897360 langmuir_trough-0.6.0/Trough/Trough_GUI/
--rw-r--r--   0 gutow    (60685682) staff       (20)    29839 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/Collect_data.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    28732 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/Monitor_Calibrate.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     1507 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/calibration_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    16304 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/command_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/conversions.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/Trough_GUI/status_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/Trough/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-03-30 13:19:07.898068 langmuir_trough-0.6.0/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-03-29 22:32:39.000000 langmuir_trough-0.6.0/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.389111 langmuir_trough-0.7.0/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.385300 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9734 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9734 2023-04-28 18:23:38.388951 langmuir_trough-0.7.0/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9080 2023-04-28 18:13:03.000000 langmuir_trough-0.7.0/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.385434 langmuir_trough-0.7.0/Trough/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.386422 langmuir_trough-0.7.0/Trough/Trough_Control/
+-rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/message_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/simulation.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    35561 2023-04-28 17:11:38.000000 langmuir_trough-0.7.0/Trough/Trough_Control/trough_util.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.388455 langmuir_trough-0.7.0/Trough/Trough_GUI/
+-rw-r--r--   0 gutow    (60685682) staff       (20)    29903 2023-04-28 17:39:19.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/Collect_data.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    28732 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/Monitor_Calibrate.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     3017 2023-04-28 14:28:17.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/calibration_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    16304 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/command_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/conversions.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/status_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-28 18:23:38.389159 langmuir_trough-0.7.0/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-04-28 18:13:03.000000 langmuir_trough-0.7.0/setup.py
```

### Comparing `langmuir_trough-0.6.0/Langmuir_Trough.egg-info/PKG-INFO` & `langmuir_trough-0.7.0/Langmuir_Trough.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langmuir-trough
-Version: 0.6.0
+Version: 0.7.0
 Summary: Controls and collects data from Gutow Lab Langmuir Trough.
 Home-page: https://github.com/gutow/Langmuir_Trough.git
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -125,29 +125,38 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.7.0 (Apr. 28, 2023)
+  * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
+    tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
+    `Trough_GUI.newCalculatedColumn()`.
+  * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
+    clobbers an already running notebook that is talking to the trough 
+    A-to-D hardware.
+  * BUG_FIX: Stopping a data collection run now makes sure the barriers are 
+    stopped.
 * 0.6.0 (Mar. 29, 2023)
   * Documentation updates including Gutow Lab Standard Operating Procedures 
     (SOPs).
   * Refactored everything to inside the module `Trough`.
 * 0.5.2 (Mar. 16, 2023) Now works in Jupyter Lab.
   * Adjusted widget updating/clearing to work in Jupyter lab.
   * Added JupyterLab >= 3.6.1 to requirements.
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.6.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
 * Runs don't label graph axes reliably for x-axis units other than cm.
 
 ## Development
```

### Comparing `langmuir_trough-0.6.0/Langmuir_Trough.egg-info/SOURCES.txt` & `langmuir_trough-0.7.0/Langmuir_Trough.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/PKG-INFO` & `langmuir_trough-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langmuir_trough
-Version: 0.6.0
+Version: 0.7.0
 Summary: Controls and collects data from Gutow Lab Langmuir Trough.
 Home-page: https://github.com/gutow/Langmuir_Trough.git
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -125,29 +125,38 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.7.0 (Apr. 28, 2023)
+  * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
+    tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
+    `Trough_GUI.newCalculatedColumn()`.
+  * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
+    clobbers an already running notebook that is talking to the trough 
+    A-to-D hardware.
+  * BUG_FIX: Stopping a data collection run now makes sure the barriers are 
+    stopped.
 * 0.6.0 (Mar. 29, 2023)
   * Documentation updates including Gutow Lab Standard Operating Procedures 
     (SOPs).
   * Refactored everything to inside the module `Trough`.
 * 0.5.2 (Mar. 16, 2023) Now works in Jupyter Lab.
   * Adjusted widget updating/clearing to work in Jupyter lab.
   * Added JupyterLab >= 3.6.1 to requirements.
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.6.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
 * Runs don't label graph axes reliably for x-axis units other than cm.
 
 ## Development
```

### Comparing `langmuir_trough-0.6.0/README.md` & `langmuir_trough-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -108,29 +108,38 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.7.0 (Apr. 28, 2023)
+  * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
+    tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
+    `Trough_GUI.newCalculatedColumn()`.
+  * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
+    clobbers an already running notebook that is talking to the trough 
+    A-to-D hardware.
+  * BUG_FIX: Stopping a data collection run now makes sure the barriers are 
+    stopped.
 * 0.6.0 (Mar. 29, 2023)
   * Documentation updates including Gutow Lab Standard Operating Procedures 
     (SOPs).
   * Refactored everything to inside the module `Trough`.
 * 0.5.2 (Mar. 16, 2023) Now works in Jupyter Lab.
   * Adjusted widget updating/clearing to work in Jupyter lab.
   * Added JupyterLab >= 3.6.1 to requirements.
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.6.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
 * Runs don't label graph axes reliably for x-axis units other than cm.
 
 ## Development
```

### Comparing `langmuir_trough-0.6.0/Trough/Trough_Control/simulation.py` & `langmuir_trough-0.7.0/Trough/Trough_Control/simulation.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/Trough/Trough_Control/trough_util.py` & `langmuir_trough-0.7.0/Trough/Trough_Control/trough_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,44 @@
             result = etol_call(obj,param)
         except RecursionError as f:
             raise RecursionError('Recursion error while trying to recover from '+str(e))
         return result
     else:
         raise TypeError(str(obj) + ' must be a callable object.')
 
+def pid_exists(pid):
+    """Check whether pid exists in the current process table.
+    UNIX only. From this stackoverflow suggestion:
+    https://stackoverflow.com/a/6940314
+    """
+    import os, errno, time
+    if pid < 0:
+        return False
+    if pid == 0:
+        # According to "man 2 kill" PID 0 refers to every process
+        # in the process group of the calling process.
+        # On certain systems 0 is a valid PID but we have no way
+        # to know that in a portable fashion.
+        raise ValueError('invalid PID 0')
+    try:
+        os.kill(pid, 0)
+    except OSError as err:
+        if err.errno == errno.ESRCH:
+            # ESRCH == No such process
+            return False
+        elif err.errno == errno.EPERM:
+            # EPERM clearly means there's a process to deny access to
+            return True
+        else:
+            # According to "man 2 kill" possible error values are
+            # (EINVAL, EPERM, ESRCH)
+            raise
+    else:
+        return True
+
 def is_trough_initialized():
     """Checks for a running Trough process and good connections to it.
     Returns
     -------
     bool
     TRUE if initialized
     """
@@ -84,32 +114,41 @@
     datarcv: the end of the pipe the trough uses to send back data and messages.
 
     Process
     TROUGH: the process handle for the trough.
     """
     from multiprocessing import Process, Pipe
     from Trough.Trough_Control.message_utils import extract_messages
-    import time
+    import time, os
     from sys import exit
 
     cmdsend, cmdrcv = Pipe()
     datasend, datarcv = Pipe()
-    # Check for trough hardware
     trough_exists = True
-    try:
-        from piplates import DAQC2plate
-        del DAQC2plate
-    except Exception as e:
-        print("An issue was encountered while accessing the DAQC2plate:" +
-              str(e))
-        trough_exists = False
+    # Check if another process is monitoring the trough
+    pidpath = '/tmp/troughctl.pid'
+    if os.path.exists(pidpath):
+        file=open(pidpath,'r')
+        pid = int(file.readline())
+        if pid_exists(pid):
+            print("Another process is controlling the Trough.")
+            trough_exists = False
+    # Check for trough hardware
+    if trough_exists:
+        try:
+            from piplates import DAQC2plate
+            del DAQC2plate
+        except Exception as e:
+            print("An issue was encountered while accessing the DAQC2plate:" +
+                  str(e))
+            trough_exists = False
     if trough_exists:
         TROUGH = Process(target=troughctl, args=(cmdrcv, datasend))
     else:
-        print("Unable to find Trough. Using simulation.")
+        print("Unable to access Trough. Using simulation.")
         from Trough.Trough_Control.simulation import simulated_troughctl
         TROUGH = Process(target=simulated_troughctl, args=(cmdrcv, datasend))
     TROUGH.start()
     time.sleep(0.2)
     waiting = True
     while waiting:
         if datarcv.poll():
@@ -118,16 +157,14 @@
             print(str(messages))
             if "ERROR" in messages:
                 exit()
             if "Trough ready" in messages:
                 waiting = False
     return cmdsend, datarcv, TROUGH
 
-
-
 def troughctl(CTLPipe,DATAPipe):
     """
     Will run as separate process taking in commands through a pipe and
     returning data on demand through a second pipe.
     Iteration 1, collects data into a fifo and watches barrier position.
     :param Pipe CTLPipe: pipe commands come in on and messages go out on.
     :param Pipe DATAPipe: pipe data is sent out on
```

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/Collect_data.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/Collect_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,14 +567,16 @@
                     # No updated data, so just pass messages
                     update_dict = {'messages':datapkg[7]}
                 Trough_GUI.status_widgets.update_status(update_dict, cals,
                                                         lastdirection)
                 waiting = False
         if time.time()< min_next_time:
             time.sleep(min_next_time - time.time())
+    # Make sure the barrier stops
+    cmdsend.send(['Stop',''])
     # Release lock and set the shared I'm running flag to False before exiting.
     trough_lock.release()
     updater_running.value = False
     run._end_of_run()
     return
 
 def update_collection(datapkg, cals, lastdirection, run_updater, updater_running, run):
```

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/Monitor_Calibrate.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/Monitor_Calibrate.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/calibration_utils.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/calibration_utils.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/command_widgets.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/command_widgets.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/conversions.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/conversions.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/Trough/Trough_GUI/status_widgets.py` & `langmuir_trough-0.7.0/Trough/Trough_GUI/status_widgets.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.6.0/setup.py` & `langmuir_trough-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="langmuir_trough",
-    version="0.6.0",
+    version="0.7.0",
     description="Controls and collects data from Gutow Lab Langmuir Trough.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gutow/Langmuir_Trough.git",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="",
```

