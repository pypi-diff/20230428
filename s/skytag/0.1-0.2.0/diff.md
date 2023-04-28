# Comparing `tmp/skytag-0.1.tar.gz` & `tmp/skytag-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytag-0.1.tar", last modified: Thu Apr 27 16:37:42 2023, max compression
+gzip compressed data, was "skytag-0.2.0.tar", last modified: Fri Apr 28 14:57:03 2023, max compression
```

## Comparing `skytag-0.1.tar` & `skytag-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-27 16:37:42.075354 skytag-0.1/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       50 2023-04-27 16:34:12.000000 skytag-0.1/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-27 16:34:12.000000 skytag-0.1/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-27 16:34:12.000000 skytag-0.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3877 2023-04-27 16:37:42.075354 skytag-0.1/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3246 2023-04-27 16:34:12.000000 skytag-0.1/README.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-27 16:37:42.075354 skytag-0.1/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1742 2023-04-27 16:34:12.000000 skytag-0.1/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-27 16:37:42.075354 skytag-0.1/skytag/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-04-27 16:34:12.000000 skytag-0.1/skytag/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       18 2023-04-27 16:34:12.000000 skytag-0.1/skytag/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3897 2023-04-27 16:34:12.000000 skytag-0.1/skytag/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-27 16:37:42.075354 skytag-0.1/skytag/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       47 2023-04-27 16:34:12.000000 skytag-0.1/skytag/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-27 16:34:12.000000 skytag-0.1/skytag/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-04-27 16:34:12.000000 skytag-0.1/skytag/default_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-27 16:34:12.000000 skytag-0.1/skytag/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-04-27 16:34:12.000000 skytag-0.1/skytag/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-27 16:34:12.000000 skytag-0.1/skytag/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-27 16:37:42.075354 skytag-0.1/skytag.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3877 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      476 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-27 16:37:13.000000 skytag-0.1/skytag.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       20 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-27 16:37:41.000000 skytag-0.1/skytag.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.780961 skytag-0.2.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       64 2023-04-28 14:53:42.000000 skytag-0.2.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-28 14:53:42.000000 skytag-0.2.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-28 14:53:42.000000 skytag-0.2.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4311 2023-04-28 14:57:03.780961 skytag-0.2.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3676 2023-04-28 14:53:42.000000 skytag-0.2.0/README.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-28 14:57:03.780961 skytag-0.2.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1807 2023-04-28 14:53:42.000000 skytag-0.2.0/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.776961 skytag-0.2.0/skytag/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        2 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4128 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.780961 skytag-0.2.0/skytag/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       94 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5118 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/prob_at_location.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/default_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      177 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/delete_me.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.776961 skytag-0.2.0/skytag.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4311 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      553 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-28 14:56:27.000000 skytag-0.2.0/skytag.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       57 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/top_level.txt
```

### Comparing `skytag-0.1/LICENSE` & `skytag-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytag-0.1/PKG-INFO` & `skytag-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: skytag
-Version: 0.1
-Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
-Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.1.zip
-Author: David Young
-Author-email: d.r.young@qub.ac.uk
-License: MIT
-Keywords: astronomy
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # skytag
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/pypi/v/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/conda/vn/conda-forge/skytag)](https://anaconda.org/conda-forge/skytag)
@@ -34,27 +17,26 @@
 [![](https://img.shields.io/github/issues/thespacedoctor/skytag/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/skytag/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+) 
 
 *Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.*.
 
 Documentation for skytag is hosted by [Read the Docs](https://skytag.readthedocs.io/en/main/) ([development version](https://skytag.readthedocs.io/en/develop/) and [main version](https://skytag.readthedocs.io/en/main/)). The code lives on [github](https://github.com/thespacedoctor/skytag). Please report any issues you find [here](https://github.com/thespacedoctor/skytag/issues). If you want to contribute, [pull requests](https://github.com/thespacedoctor/skytag/pulls) are welcomed! 
 true
 
-
 ## Features
 
-* 
-
-
+- A command-line tool to report the credibility region a sky-location is found within on a HealPix skymap.  
+- Providing a MJD will also return the time since the map event.  
+- A python interface to provide the same functionality reported above, but can handle large lists of sky-locations or transient events.  
 
 ## Installation
 
 The easiest way to install skytag is to use `conda`:
 
 ``` bash
-conda create -n skytag python=3.9 pip skytag -c conda-forge
+conda create -n skytag python=3.11 pip skytag -c conda-forge
 conda activate skytag
 ```
 
 To upgrade to the latest version of skytag use the command:
 
 ``` bash
 conda upgrade skytag -c conda-forge
@@ -62,30 +44,45 @@
 
 It is also possible to install via pip if required:
 
 ``` bash
 pip install skytag
 ```
 
-Or you can clone the [github repo](https://github.com/thespacedoctor/skytag) and install from a local version of the code:
+To check installation was successful run `skytag -v`. This should return the version number of the install.
 
-``` bash
-git clone git@github.com:thespacedoctor/skytag.git
-cd skytag
-python setup.py install
+## Command-Line 
+
+Here is the command-line usage:
+
+```bash 
+Usage:
+    skytag <ra> <dec> <mapPath>
+    skytag <ra> <dec> <mjd> <mapPath>
 ```
 
-To check installation was successful run `skytag -v`. This should return the version number of the install.
+If you need an example skymap, [download one from here](https://github.com/thespacedoctor/skytag/raw/main/skytag/commonutils/tests/input/bayestar.multiorder.fits).
+
+For example, to find the probability of the location RA=170.343532, Dec=-40.532255 then run:
+
+```bash 
+skytag 170.343532 -40.532255 bayestar.multiorder.fits
+```
 
-## Initialising skytag
+This returns:
 
-Before using skytag you need to use the `init` command to generate a user settings file. Running the following creates a [yaml](https://learnxinyminutes.com/docs/yaml/) settings file in your home folder under `~/.config/skytag/skytag.yaml`:
+> This location is found in the 74.55 credibility region of the map.
 
-```bash
-skytag init
+If you also supply an MJD:
+
+```bash 
+skytag 170.343532 -40.532255 60065.2232 bayestar.multiorder.fits
 ```
 
-The file is initially populated with skytag's default settings which can be adjusted to your preference.
+We get:
+
+> This transient is found in the 74.55 credibility region, and occurred 2.85564 days after the map event.
+
+## Python API
 
-If at any point the user settings file becomes corrupted or you just want to start afresh, simply trash the `skytag.yaml` file and rerun `skytag init`.
+To use skytag in your own Python code, [see here](_autosummary/skytag.commonutils.prob_at_location.html#skytag.commonutils.prob_at_location).
 
-You are now ready to start using skytag.
```

### Comparing `skytag-0.1/setup.py` & `skytag-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 def readme():
     with open(moduleDirectory + '/README.md') as f:
         return f.read()
 
 
 install_requires = [
     'pyyaml',
-    'fundamentals'
+    'fundamentals',
+    'astropy',
+    'astropy-healpix',
+    'numpy',
+    'pandas'
 ]
 
 # READ THE DOCS SERVERS
 exists = os.path.exists("/home/docs/")
 if exists:
     c_exclude_list = ['healpy', 'astropy',
                       'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb']
```

### Comparing `skytag-0.1/skytag/cl_utils.py` & `skytag-0.2.0/skytag/cl_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 Documentation for skytag can be found here: http://skytag.readthedocs.org
 
 Usage:
     skytag init
-    skytag [-s <pathToSettingsFile>]  
+    skytag <ra> <dec> <mapPath>
+    skytag <ra> <dec> <mjd> <mapPath>
 
 Options:
     init                                   setup the skytag settings file for the first time
+    <ra>                                   sky location right-ascension (decimal degrees or sexegesimal)
+    <dec>                                  sky location declination (decimal degrees or sexegesimal)
+    <mjd>                                  a transient event MJD. If supplied, a time delta from the map event is returned alongside probability.
+    <mapPath>                              path to a HealPix skymap
     -h, --help                             show this help message
     -v, --version                          show version
     -s, --settings <pathToSettingsFile>    the settings file
 """
+from subprocess import Popen, PIPE, STDOUT
+from fundamentals import tools, times
+from docopt import docopt
+import pickle
+import glob
+import readline
 import sys
 import os
 os.environ['TERM'] = 'vt100'
-import readline
-import glob
-import pickle
-from docopt import docopt
-from fundamentals import tools, times
-from subprocess import Popen, PIPE, STDOUT
 
 
 def tab_complete(text, state):
     return (glob.glob(text + '*') + [None])[state]
 
 
 def main(arguments=None):
@@ -33,15 +38,15 @@
     *The main function used when `cl_utils.py` is run as a single script from the cl, or when installed as a cl command*
     """
     # setup the command-line util settings
     su = tools(
         arguments=arguments,
         docString=__doc__,
         logLevel="WARNING",
-        options_first=False,
+        options_first=True,
         projectName="skytag",
         defaultSettingsFile=True
     )
     arguments, settings, log, dbConn = su.setup()
 
     # tab completion for raw_input
     readline.set_completer_delims(' \t\n;')
@@ -64,42 +69,14 @@
 
     ## START LOGGING ##
     startTime = times.get_now_sql_datetime()
     log.info(
         '--- STARTING TO RUN THE cl_utils.py AT %s' %
         (startTime,))
 
-    # set options interactively if user requests
-    if "interactiveFlag" in a and a["interactiveFlag"]:
-
-        # load previous settings
-        moduleDirectory = os.path.dirname(__file__) + "/resources"
-        pathToPickleFile = "%(moduleDirectory)s/previousSettings.p" % locals()
-        try:
-            with open(pathToPickleFile):
-                pass
-            previousSettingsExist = True
-        except:
-            previousSettingsExist = False
-        previousSettings = {}
-        if previousSettingsExist:
-            previousSettings = pickle.load(open(pathToPickleFile, "rb"))
-
-        # x-raw-input
-        # x-boolean-raw-input
-        # x-raw-input-with-default-value-from-previous-settings
-
-        # save the most recently used requests
-        pickleMeObjects = []
-        pickleMe = {}
-        theseLocals = locals()
-        for k in pickleMeObjects:
-            pickleMe[k] = theseLocals[k]
-        pickle.dump(pickleMe, open(pathToPickleFile, "wb"))
-
     if a["init"]:
         from os.path import expanduser
         home = expanduser("~")
         filepath = home + "/.config/skytag/skytag.yaml"
         try:
             cmd = """open %(filepath)s""" % locals()
             p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
@@ -108,19 +85,43 @@
         try:
             cmd = """start %(filepath)s""" % locals()
             p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
         except:
             pass
         return
 
-    # CALL FUNCTIONS/OBJECTS
+    if a["mjd"]:
+        from skytag.commonutils import prob_at_location
+        prob, deltas = prob_at_location(
+            log=log,
+            ra=float(a["ra"]),
+            dec=float(a["dec"]),
+            mjd=float(a["mjd"]),
+            mapPath=a["mapPath"]
+        )
+
+        if deltas[0] < 0.:
+            preposition = "before"
+        else:
+            preposition = "after"
+
+        print(f"This transient is found in the {prob[0]} credibility region, and occurred {deltas[0]} days {preposition} the map event.")
+
+    else:
+        # CALL FUNCTIONS/OBJECTS
+        from skytag.commonutils import prob_at_location
+        prob = prob_at_location(
+            log=log,
+            ra=float(a["ra"]),
+            dec=float(a["dec"]),
+            mapPath=a["mapPath"]
+        )[0]
+
+        print(f"This location is found in the {prob} credibility region of the map.")
 
-    if "dbConn" in locals() and dbConn:
-        dbConn.commit()
-        dbConn.close()
     ## FINISH LOGGING ##
     endTime = times.get_now_sql_datetime()
     runningTime = times.calculate_time_difference(startTime, endTime)
     log.info('-- FINISHED ATTEMPT TO RUN THE cl_utils.py AT %s (RUNTIME: %s) --' %
              (endTime, runningTime, ))
 
     return
```

### Comparing `skytag-0.1/skytag/default_settings.yaml` & `skytag-0.2.0/skytag/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.1/skytag/setup.cfg` & `skytag-0.2.0/skytag/setup.cfg`

 * *Files identical despite different names*

### Comparing `skytag-0.1/skytag/test_settings.yaml` & `skytag-0.2.0/skytag/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.1/skytag/utKit.py` & `skytag-0.2.0/skytag/utKit.py`

 * *Files identical despite different names*

### Comparing `skytag-0.1/skytag.egg-info/PKG-INFO` & `skytag-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skytag
-Version: 0.1
+Version: 0.2.0
 Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
 Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.1.zip
+Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.2.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -34,27 +34,26 @@
 [![](https://img.shields.io/github/issues/thespacedoctor/skytag/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/skytag/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+) 
 
 *Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.*.
 
 Documentation for skytag is hosted by [Read the Docs](https://skytag.readthedocs.io/en/main/) ([development version](https://skytag.readthedocs.io/en/develop/) and [main version](https://skytag.readthedocs.io/en/main/)). The code lives on [github](https://github.com/thespacedoctor/skytag). Please report any issues you find [here](https://github.com/thespacedoctor/skytag/issues). If you want to contribute, [pull requests](https://github.com/thespacedoctor/skytag/pulls) are welcomed! 
 true
 
-
 ## Features
 
-* 
-
-
+- A command-line tool to report the credibility region a sky-location is found within on a HealPix skymap.  
+- Providing a MJD will also return the time since the map event.  
+- A python interface to provide the same functionality reported above, but can handle large lists of sky-locations or transient events.  
 
 ## Installation
 
 The easiest way to install skytag is to use `conda`:
 
 ``` bash
-conda create -n skytag python=3.9 pip skytag -c conda-forge
+conda create -n skytag python=3.11 pip skytag -c conda-forge
 conda activate skytag
 ```
 
 To upgrade to the latest version of skytag use the command:
 
 ``` bash
 conda upgrade skytag -c conda-forge
@@ -62,30 +61,45 @@
 
 It is also possible to install via pip if required:
 
 ``` bash
 pip install skytag
 ```
 
-Or you can clone the [github repo](https://github.com/thespacedoctor/skytag) and install from a local version of the code:
+To check installation was successful run `skytag -v`. This should return the version number of the install.
 
-``` bash
-git clone git@github.com:thespacedoctor/skytag.git
-cd skytag
-python setup.py install
+## Command-Line 
+
+Here is the command-line usage:
+
+```bash 
+Usage:
+    skytag <ra> <dec> <mapPath>
+    skytag <ra> <dec> <mjd> <mapPath>
 ```
 
-To check installation was successful run `skytag -v`. This should return the version number of the install.
+If you need an example skymap, [download one from here](https://github.com/thespacedoctor/skytag/raw/main/skytag/commonutils/tests/input/bayestar.multiorder.fits).
+
+For example, to find the probability of the location RA=170.343532, Dec=-40.532255 then run:
+
+```bash 
+skytag 170.343532 -40.532255 bayestar.multiorder.fits
+```
 
-## Initialising skytag
+This returns:
 
-Before using skytag you need to use the `init` command to generate a user settings file. Running the following creates a [yaml](https://learnxinyminutes.com/docs/yaml/) settings file in your home folder under `~/.config/skytag/skytag.yaml`:
+> This location is found in the 74.55 credibility region of the map.
 
-```bash
-skytag init
+If you also supply an MJD:
+
+```bash 
+skytag 170.343532 -40.532255 60065.2232 bayestar.multiorder.fits
 ```
 
-The file is initially populated with skytag's default settings which can be adjusted to your preference.
+We get:
+
+> This transient is found in the 74.55 credibility region, and occurred 2.85564 days after the map event.
+
+## Python API
 
-If at any point the user settings file becomes corrupted or you just want to start afresh, simply trash the `skytag.yaml` file and rerun `skytag init`.
+To use skytag in your own Python code, [see here](_autosummary/skytag.commonutils.prob_at_location.html#skytag.commonutils.prob_at_location).
 
-You are now ready to start using skytag.
```

