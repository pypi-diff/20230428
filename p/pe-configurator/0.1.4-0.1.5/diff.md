# Comparing `tmp/pe-configurator-0.1.4.tar.gz` & `tmp/pe-configurator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.4.tar", last modified: Wed Apr 26 09:58:20 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.5.tar", last modified: Fri Apr 28 14:20:28 2023, max compression
```

## Comparing `pe-configurator-0.1.4.tar` & `pe-configurator-0.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.257390 pe-configurator-0.1.4/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.257390 pe-configurator-0.1.4/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.4/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.268223 pe-configurator-0.1.4/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.268223 pe-configurator-0.1.4/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.4/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.268223 pe-configurator-0.1.4/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.268223 pe-configurator-0.1.4/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.268223 pe-configurator-0.1.4/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-26 09:58:20.000000 pe-configurator-0.1.4/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6101 2023-04-26 09:56:59.000000 pe-configurator-0.1.4/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/get_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-26 09:58:20.279056 pe-configurator-0.1.4/tests/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.4/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.820097 pe-configurator-0.1.5/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.820097 pe-configurator-0.1.5/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.5/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.841763 pe-configurator-0.1.5/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.852597 pe-configurator-0.1.5/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.852597 pe-configurator-0.1.5/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.863430 pe-configurator-0.1.5/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6877 2023-04-28 13:12:38.000000 pe-configurator-0.1.5/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.4/PKG-INFO` & `pe-configurator-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.4/README.md` & `pe-configurator-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/data/calibration_files.txt` & `pe-configurator-0.1.5/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/.DS_Store` & `pe-configurator-0.1.5/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190412/test.html` & `pe-configurator-0.1.5/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190412/test.json` & `pe-configurator-0.1.5/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.5/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190521/test.html` & `pe-configurator-0.1.5/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190521/test.json` & `pe-configurator-0.1.5/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.5/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190814/test.html` & `pe-configurator-0.1.5/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190814/test.json` & `pe-configurator-0.1.5/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.5/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW191109/test.html` & `pe-configurator-0.1.5/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW191109/test.json` & `pe-configurator-0.1.5/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.5/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.5/pe_configurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.4/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.5/pe_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/peconfigurator/asimov.py` & `pe-configurator-0.1.5/peconfigurator/asimov.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import os
 import configparser
 import json
 
+import h5py
 from asimov.pipeline import Pipeline
 from asimov import config
 import htcondor
 import yaml
 from asimov.utils import set_directory
 
 class AsimovPipeline(Pipeline):
@@ -27,42 +28,51 @@
             productions = {}
             for production in self.production.event.productions:
                 productions[production.name] = production
             for previous_job in self.production.dependencies:
                 print("assets", productions[previous_job].pipeline.collect_assets())
                 try:
                     if "samples" in productions[previous_job].pipeline.collect_assets():
-                        return productions[previous_job].pipeline.collect_assets()['samples']
+                        posterior_file = productions[previous_job].pipeline.collect_assets()['samples']
+                        if "dataset" not in self.production.meta:
+                            with h5py.File(posterior_file,'r') as f:
+                                keys = list(f.keys())
+                            keys.remove('version')
+                            keys.remove('history')
+                            self.production.meta['dataset'] = keys[0]
+                        return posterior_file
                 except Exception:
                     pass
         else:
             self.logger.error("Could not find an analysis providing the posterior to analyse.")
     
     def build_dag(self, dryrun=False):
         """
         Create a condor submission description.
         """
         name = self.production.name
         ini = self.production.event.repository.find_prods(name,
                                                           self.category)[0]
 
         meta = self.production.meta
+        posterior = self._find_posterior()
+
         executable = f"{os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)}"
         command = ["--dataset", f"{meta['dataset']}",
                    "--output_dir", "results",
                    "--json_file", "recommendations.json",
 	           "--q-min", f"{meta['minimum mass ratio']}",
                    ]
         if "higher modes" in meta['checks']:
             command += ["--HM"]
         if "luminosity distance" in meta['checks']:
             command += ["--include_dL_recommendations"]
         if "no safety" in meta['checks']:
             command += ["--override_safeties"]
-        command += [self._find_posterior()]
+        command += [posterior]
         # To do: Add remaining settings once you've decided where they should go
         full_command = executable + " " + " ".join(command)
         self.logger.info(full_command)
         
         description = {
             "executable": executable,
             "arguments": " ".join(command),
@@ -71,14 +81,17 @@
             "log": f"{name}.log",
             "getenv": "True",
             "request_memory": "4096 MB",
             "request_disk": "100 MB",
             "batch_name": f"{self.name}/{self.production.event.name}/{name}",
             "accounting_group_user": config.get('condor', 'user'),
             "accounting_group": self.production.meta['scheduler']["accounting group"],
+            "request_disk": "8192MB",
+            "+flock_local": "True",
+            "+DESIRED_Sites": htcondor.classad.quote("nogrid"),
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             os.makedirs("results", exist_ok=True)
             
@@ -139,18 +152,20 @@
 
         if 'f_start' in data:
             meta['likelihood']['start frequency'] = data['f_start']
             
         if 'f_ref' in data:
             meta['waveform']['reference frequency'] = data['f_ref']
 
-        if 'seglen' in data:
+        if 'seglen' in data and 'segment length' not in meta['data']:
             meta['data']['segment length'] = data['seglen']
-            meta['likelihood']['window length'] = data['seglen']
-            meta['likelihood']['psd length'] = data['seglen']
+        if 'window length' not in meta['likelihood']:
+            meta['likelihood']['window length'] = meta['data']['segment length']
+        if 'psd length' not in meta['likelihood']:
+            meta['likelihood']['psd length'] = meta['data']['segment length']
 
         if "chirpmass_min" in data:
             if not "chirp mass" in meta['priors']:
                 meta['priors']['chirp mass'] = {}
             meta['priors']['chirp mass']['minimum'] = data['chirpmass_min']
             meta['priors']['chirp mass']['maximum'] = data['chirpmass_max']
         self.production.event.update_data()
```

### Comparing `pe-configurator-0.1.4/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.5/peconfigurator/auxiliary/make_report.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.5/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/peconfigurator/get_settings.py` & `pe-configurator-0.1.5/peconfigurator/get_settings.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/peconfigurator/proc_samples.py` & `pe-configurator-0.1.5/peconfigurator/proc_samples.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.5/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/pyproject.toml` & `pe-configurator-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.4/tests/test_get_settings.py` & `pe-configurator-0.1.5/tests/test_get_settings.py`

 * *Files identical despite different names*

