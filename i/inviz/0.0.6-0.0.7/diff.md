# Comparing `tmp/inviz-0.0.6.tar.gz` & `tmp/inviz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.6.tar", last modified: Thu Apr 27 23:22:14 2023, max compression
+gzip compressed data, was "inviz-0.0.7.tar", last modified: Fri Apr 28 18:14:07 2023, max compression
```

## Comparing `inviz-0.0.6.tar` & `inviz-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.106627 inviz-0.0.6/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-04-27 23:20:02.000000 inviz-0.0.6/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-04-27 23:20:02.000000 inviz-0.0.6/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-27 23:22:14.106627 inviz-0.0.6/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1359 2023-04-27 23:20:02.000000 inviz-0.0.6/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.096627 inviz-0.0.6/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-27 23:22:14.106627 inviz-0.0.6/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       39 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-04-27 23:22:14.000000 inviz-0.0.6/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8826 2023-04-27 23:20:03.000000 inviz-0.0.6/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-04-27 23:22:14.106627 inviz-0.0.6/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1127 2023-04-27 23:20:03.000000 inviz-0.0.6/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-04-27 23:20:02.000000 inviz-0.0.7/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-04-27 23:20:02.000000 inviz-0.0.7/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-28 18:14:07.748636 inviz-0.0.7/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1359 2023-04-27 23:20:02.000000 inviz-0.0.7/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)     9062 2023-04-28 17:14:55.000000 inviz-0.0.7/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-04-28 18:14:07.748636 inviz-0.0.7/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-04-28 17:33:46.000000 inviz-0.0.7/setup.py
```

### Comparing `inviz-0.0.6/LICENSE` & `inviz-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.6/PKG-INFO` & `inviz-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # inviz
 
 This tool helps you explore the results of running MCMC posterior sampling on your cosmological model. Selecting a point on the sample distribution will automatically run CLASS on that sample and display the output.
```

### Comparing `inviz-0.0.6/README.md` & `inviz-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.0.6/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.0.7/inviz/inviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.6
+Version: 0.0.7
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # inviz
 
 This tool helps you explore the results of running MCMC posterior sampling on your cosmological model. Selecting a point on the sample distribution will automatically run CLASS on that sample and display the output.
```

### Comparing `inviz-0.0.6/inviz/inviz.py` & `inviz-0.0.7/inviz/inviz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import holoviews as hv
 from holoviews import dim, opts, streams
-from holoviews.selection import link_selections
-import hvplot.pandas
+# from holoviews.selection import link_selections
+# import hvplot.pandas
 import pandas as pd
 from itertools import combinations
 import numpy as np
 from tqdm import trange, tqdm
 import re
 import panel as pn
 import spatialpandas
 import os
 from bokeh.models import HoverTool
 from classy import Class
 import matplotlib.pyplot as plt
-import copy
+# import copy
 from multiprocessing import Pool
 
+# pn.extension(loading_spinner='dots', loading_color='#00aa41', sizing_mode="stretch_width")
 hv.extension('bokeh')
 # hv.Store.set_current_backend('bokeh')
 # pn.extension('tabulator')
 pn.extension()
 
 # read in the .paramnames file and put it into list format
 def load_params(filename):
@@ -152,18 +153,22 @@
 
         # the Selection1D stream returns an index number. index into the approprate dataframe and turn it into a dictionary for CLASS to read
         selection = data_classy_input.iloc[index]
         selection_CDM = data_classy_CDM.iloc[index]
         sel_dict_list = selection.to_dict('records')
         CDM_dict_list = selection_CDM.to_dict('records')
         
-        # compute stats for user's cosmology and LambdaCDM in parallel
-        if __name__ == '__main__':
-            with Pool() as p:
-                [mycosmo, LambdaCDM] = p.map(run_class, [sel_dict_list[0], CDM_dict_list[0]])
+        # compute stats for user's cosmology and LambdaCDM
+        # in parallel:
+        # if __name__ == '__main__':
+        #     with Pool() as p:
+        #         [mycosmo, LambdaCDM] = p.map(run_class, [sel_dict_list[0], CDM_dict_list[0]])
+        # in serial:
+        mycosmo = run_class(sel_dict_list[0])
+        LambdaCDM = run_class(CDM_dict_list[0])
 
         # compute residuals
         pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
         cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
         cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
 
         plot_pk_residuals = hv.Curve((mycosmo['k'], pk_residuals)).relabel('P(k) Residuals').opts(
```

### Comparing `inviz-0.0.6/setup.py` & `inviz-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
@@ -20,15 +20,14 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=["holoviews==1.15.4",
-                    #   "bokeh==2.4.3",
-                      "spatialpandas==0.4.7"]
-                    #   "numpy<=1.24",
-                    #   "matplotlib==3.7.1"]
+                      "spatialpandas==0.4.7",
+                      "numpy>=1.20, <1.24",
+                      "matplotlib==3.7.1"]
     )
```

