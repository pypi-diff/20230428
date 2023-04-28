# Comparing `tmp/spatialprompt-0.0.2.tar.gz` & `tmp/spatialprompt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialprompt-0.0.2.tar", last modified: Fri Apr 28 09:22:45 2023, max compression
+gzip compressed data, was "spatialprompt-0.0.3.tar", last modified: Fri Apr 28 16:58:26 2023, max compression
```

## Comparing `spatialprompt-0.0.2.tar` & `spatialprompt-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/
--rw-------   0 asish     (1000) asish     (1000)        0 2022-08-07 15:26:46.000000 spatialprompt-0.0.2/LICENCE.txt
--rw-------   0 asish     (1000) asish     (1000)       30 2022-08-07 15:26:46.000000 spatialprompt-0.0.2/MANIFEST.in
--rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/PKG-INFO
--rw-------   0 asish     (1000) asish     (1000)      108 2023-04-28 09:19:00.000000 spatialprompt-0.0.2/README.md
--rw-rw-r--   0 asish     (1000) asish     (1000)       38 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/setup.cfg
--rw-------   0 asish     (1000) asish     (1000)      841 2023-04-28 09:21:20.000000 spatialprompt-0.0.2/setup.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/spatialprompt/
--rw-------   0 asish     (1000) asish     (1000)    18939 2023-04-28 09:19:06.000000 spatialprompt-0.0.2/spatialprompt/__init__.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/spatialprompt.egg-info/
--rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/PKG-INFO
--rw-rw-r--   0 asish     (1000) asish     (1000)      252 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/SOURCES.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)        1 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/dependency_links.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       83 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/requires.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       14 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/top_level.txt
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/
+-rw-------   0 asish     (1000) asish     (1000)        0 2022-08-07 15:26:46.000000 spatialprompt-0.0.3/LICENCE.txt
+-rw-------   0 asish     (1000) asish     (1000)       30 2022-08-07 15:26:46.000000 spatialprompt-0.0.3/MANIFEST.in
+-rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/PKG-INFO
+-rw-------   0 asish     (1000) asish     (1000)      108 2023-04-28 09:19:00.000000 spatialprompt-0.0.3/README.md
+-rw-rw-r--   0 asish     (1000) asish     (1000)       38 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/setup.cfg
+-rw-------   0 asish     (1000) asish     (1000)      841 2023-04-28 16:57:33.000000 spatialprompt-0.0.3/setup.py
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.547916 spatialprompt-0.0.3/spatialprompt/
+-rw-------   0 asish     (1000) asish     (1000)    19750 2023-04-28 16:57:21.000000 spatialprompt-0.0.3/spatialprompt/__init__.py
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 16:58:26.551916 spatialprompt-0.0.3/spatialprompt.egg-info/
+-rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/PKG-INFO
+-rw-rw-r--   0 asish     (1000) asish     (1000)      252 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/SOURCES.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)        1 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/dependency_links.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)       83 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/requires.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)       14 2023-04-28 16:58:26.000000 spatialprompt-0.0.3/spatialprompt.egg-info/top_level.txt
```

### Comparing `spatialprompt-0.0.2/PKG-INFO` & `spatialprompt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialprompt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
 Home-page: 
 Author: Asish Kumar Swain
 Author-email: swainkasish@gmail.com
 License: MIT
 Keywords: willupdate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spatialprompt-0.0.2/setup.py` & `spatialprompt-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='spatialprompt',
-  version='0.0.2',   #mandatory change
+  version='0.0.3',   #mandatory change
   description='Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics',
   long_description=open('README.md').read() ,
   url='',  
   author='Asish Kumar Swain',
   author_email='swainkasish@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `spatialprompt-0.0.2/spatialprompt/__init__.py` & `spatialprompt-0.0.3/spatialprompt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Tue Jun 28 12:11:26 2022
 @author: swainkasish@gmail.com
-spatialprompt_V 0.0.2
+spatialprompt_V 0.0.3
 """
 #%%
 #%% import libraries 
 import numpy as np
 import pandas as pd 
 import time 
 from sklearn.preprocessing import  StandardScaler,Normalizer,MinMaxScaler
@@ -369,16 +369,29 @@
 
         st_pred_ct = self.__fit_predict__(st_processed,simu_st_arr,simu_ct_prop,return_prop=return_prop)
 
         t2= time.time()
         print(f"Total Time spent: {t2-t1} Sec")
     
         return st_pred_ct
-    
-    
+    def cluster_cell_annotation(self,ct_deconv,cluster_annot,threshold=0.30):
+        dicti_annot = {}
+        cluster_nums = len(np.unique(cluster_annot))
+        for i in range(cluster_nums):
+            clus_temp1_index = cluster_annot == i
+            clus_deconvo = ct_deconv[clus_temp1_index].mean(axis=0)
+            clus_deconvo_major = clus_deconvo[clus_deconvo>threshold]
+            if len(clus_deconvo_major)==0:
+                thres = threshold - 0.10
+                clus_deconvo_major = clus_deconvo[clus_deconvo>thres]
+            dicti_annot[i] = ' / '.join(list(clus_deconvo_major.index))
+            if len(clus_deconvo_major)==0:
+                dicti_annot[i] = "ambiguous"
+        mod_cluster_annot = pd.Categorical([dicti_annot[i]for i in cluster_annot])
+        return dicti_annot,mod_cluster_annot
 #%% 
 class SpatialCluster:
     def __init__(self):
         pass
     def __hvg_detect__(self,df_array,N=1000):
         df_array = np.array(df_array)
         st_vars = df_array.var(axis=0)
@@ -434,10 +447,8 @@
             bar()
             cluster_assignment = self.__kmean_clus__(st_array_hvg_norm_domain,n_clus = n_cluster)
             cluster_assignment = pd.Categorical(cluster_assignment)
             bar()
         t2 = time.time()
         print(f"Executed in {t2-t1} second")
         
-        return cluster_assignment
-
-
+        return cluster_assignment
```

### Comparing `spatialprompt-0.0.2/spatialprompt.egg-info/PKG-INFO` & `spatialprompt-0.0.3/spatialprompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialprompt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
 Home-page: 
 Author: Asish Kumar Swain
 Author-email: swainkasish@gmail.com
 License: MIT
 Keywords: willupdate
 Classifier: Development Status :: 3 - Alpha
```

