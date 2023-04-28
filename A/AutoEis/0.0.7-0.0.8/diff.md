# Comparing `tmp/AutoEis-0.0.7.tar.gz` & `tmp/AutoEis-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\Beta_AutoEis\dist\.tmp-1sxvbsyq\AutoEis-0.0.7.tar", last modified: Fri Apr 28 20:27:06 2023, max compression
+gzip compressed data, was "D:\Personal Document\Studying in Canada\UOT-courses\Beta_AutoEis\dist\.tmp-8id36hxb\AutoEis-0.0.8.tar", last modified: Fri Apr 28 21:04:36 2023, max compression
```

## Comparing `AutoEis-0.0.7.tar` & `AutoEis-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.898256 AutoEis-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.881256 AutoEis-0.0.7/AutoEis/
--rw-rw-rw-   0        0        0    72563 2023-04-28 18:58:01.000000 AutoEis-0.0.7/AutoEis/AutoEIS.py
--rw-rw-rw-   0        0        0      288 2023-04-28 19:04:43.000000 AutoEis-0.0.7/AutoEis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 20:27:06.894256 AutoEis-0.0.7/AutoEis.egg-info/
--rw-rw-rw-   0        0        0      645 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 20:27:06.000000 AutoEis-0.0.7/AutoEis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-28 19:52:59.000000 AutoEis-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      645 2023-04-28 20:27:06.897256 AutoEis-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.7/README.md
--rw-rw-rw-   0        0        0       86 2023-04-28 20:17:09.000000 AutoEis-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 20:27:06.898256 AutoEis-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1717 2023-04-28 19:35:47.000000 AutoEis-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.163001 AutoEis-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.138842 AutoEis-0.0.8/AutoEis/
+-rw-rw-rw-   0        0        0    72648 2023-04-28 20:58:38.000000 AutoEis-0.0.8/AutoEis/AutoEIS.py
+-rw-rw-rw-   0        0        0      289 2023-04-28 21:04:01.000000 AutoEis-0.0.8/AutoEis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 21:04:36.157853 AutoEis-0.0.8/AutoEis.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 21:04:36.000000 AutoEis-0.0.8/AutoEis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-28 19:52:59.000000 AutoEis-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-04-28 21:04:36.161982 AutoEis-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2022-07-21 02:14:53.000000 AutoEis-0.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-28 20:17:09.000000 AutoEis-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 21:04:36.163001 AutoEis-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1717 2023-04-28 21:03:26.000000 AutoEis-0.0.8/setup.py
```

### Comparing `AutoEis-0.0.7/AutoEis/AutoEIS.py` & `AutoEis-0.0.8/AutoEis/AutoEIS.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,30 +253,32 @@
         folder_name = dirStr.split('\\')[-1]
         mkdir(folder_name)
         with open(f'{folder_name}\\ohmic_resistance = {round(ohmic_resistance, 4)}.txt', 'w') as f:
             f.write(f"ohmic resistance = {ohmic_resistance}")
     return ohmic_resistance
 
 
-
-def pre_processing(impedance: 'np.array', freq: 'np.array',
-                   threshold: 'float') -> 'Returns: pd.DataFrame / float / float':
+def pre_processing(impedance: 'np.array', freq: 'np.array', threshold: 'float',
+                   data_path: 'str') -> 'Returns: pd.DataFrame / float / float':
     """ Pre-process impedance data by deleting data with positive imaginary part at high-freq range, and by kk validation
 
         Parameters:
         ----------
         impedance: np.array of complex numbers
             the impedance data
 
         freq: np.array of float
             the frequencies of EIS data points
 
         threshold: float
             the parameter that controls the filtering effect of KK validation
 
+        data_path:string
+            the storage path
+
         Returns:
         --------
         Zdf_mask: pd.DataFrame with 3 columns
             the impedance data after pre-processing
 
         ohmic_resistance: float
             the ohmic resistance of impedance data
@@ -1927,15 +1929,15 @@
         Return:
         -------
         results: pd.DataFrame
             the dataframe that stored effective ECMs after filtering and corresponding BI results (12 columns)
     """
 
     # preprocessing + store preprocessed data
-    data_processed, ohmic_resistance = pre_processing(impedance, freq, 0.05)
+    data_processed, ohmic_resistance = pre_processing(impedance, freq, 0.05, data_path)
     path_data_preprocessed = save_processed_data(input_name=data_path, data_stored=data_processed)
 
     # call julia program
     run_julia = j.include('test_julia.jl')
 
     # load the results
     path_results = "df_results.csv"
```

### Comparing `AutoEis-0.0.7/AutoEis.egg-info/PKG-INFO` & `AutoEis-0.0.8/AutoEis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoEis
-Version: 0.0.7
+Version: 0.0.8
 Summary: A demo package to assist EIS analysis by automatically proposing statistically plausible ECM
 Home-page: 
 Author: Runze zhang, Robert Black, Jason Hattrick-Simpers*
 Author-email: runzee.zhang@mail.utoronto.ca
 Keywords: Electrochemical impedance spectroscopy,equivalent circuit models,Bayesian inference,evolutionary algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AutoEis-0.0.7/PKG-INFO` & `AutoEis-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoEis
-Version: 0.0.7
+Version: 0.0.8
 Summary: A demo package to assist EIS analysis by automatically proposing statistically plausible ECM
 Home-page: 
 Author: Runze zhang, Robert Black, Jason Hattrick-Simpers*
 Author-email: runzee.zhang@mail.utoronto.ca
 Keywords: Electrochemical impedance spectroscopy,equivalent circuit models,Bayesian inference,evolutionary algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AutoEis-0.0.7/setup.py` & `AutoEis-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A demo package to assist EIS analysis by automatically proposing statistically plausible ECM'
 LONG_DESCRIPTION = 'AutoEIS is a novel tool designed to aid EIS analysis by automatically prioritizing statistically optimal ECM by combining evolutionary algorithms and Bayesian inference.'
 
 # Setting up
 setup(
     name="AutoEis",
     version= VERSION,
```

