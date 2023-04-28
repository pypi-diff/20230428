# Comparing `tmp/spatialprompt-0.0.1.tar.gz` & `tmp/spatialprompt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialprompt-0.0.1.tar", last modified: Fri Apr 28 05:35:15 2023, max compression
+gzip compressed data, was "spatialprompt-0.0.2.tar", last modified: Fri Apr 28 09:22:45 2023, max compression
```

## Comparing `spatialprompt-0.0.1.tar` & `spatialprompt-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 05:35:15.468558 spatialprompt-0.0.1/
--rw-------   0 asish     (1000) asish     (1000)        0 2022-08-07 15:26:46.000000 spatialprompt-0.0.1/LICENCE.txt
--rw-------   0 asish     (1000) asish     (1000)       30 2022-08-07 15:26:46.000000 spatialprompt-0.0.1/MANIFEST.in
--rw-rw-r--   0 asish     (1000) asish     (1000)      557 2023-04-28 05:35:15.468558 spatialprompt-0.0.1/PKG-INFO
--rw-------   0 asish     (1000) asish     (1000)       12 2022-08-07 15:26:46.000000 spatialprompt-0.0.1/README.md
--rw-rw-r--   0 asish     (1000) asish     (1000)       38 2023-04-28 05:35:15.468558 spatialprompt-0.0.1/setup.cfg
--rw-------   0 asish     (1000) asish     (1000)      821 2023-04-28 05:25:02.000000 spatialprompt-0.0.1/setup.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 05:35:15.468558 spatialprompt-0.0.1/spatialprompt/
--rw-------   0 asish     (1000) asish     (1000)    18968 2023-04-28 05:25:17.000000 spatialprompt-0.0.1/spatialprompt/__init__.py
-drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 05:35:15.468558 spatialprompt-0.0.1/spatialprompt.egg-info/
--rw-rw-r--   0 asish     (1000) asish     (1000)      557 2023-04-28 05:35:15.000000 spatialprompt-0.0.1/spatialprompt.egg-info/PKG-INFO
--rw-rw-r--   0 asish     (1000) asish     (1000)      252 2023-04-28 05:35:15.000000 spatialprompt-0.0.1/spatialprompt.egg-info/SOURCES.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)        1 2023-04-28 05:35:15.000000 spatialprompt-0.0.1/spatialprompt.egg-info/dependency_links.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       83 2023-04-28 05:35:15.000000 spatialprompt-0.0.1/spatialprompt.egg-info/requires.txt
--rw-rw-r--   0 asish     (1000) asish     (1000)       14 2023-04-28 05:35:15.000000 spatialprompt-0.0.1/spatialprompt.egg-info/top_level.txt
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/
+-rw-------   0 asish     (1000) asish     (1000)        0 2022-08-07 15:26:46.000000 spatialprompt-0.0.2/LICENCE.txt
+-rw-------   0 asish     (1000) asish     (1000)       30 2022-08-07 15:26:46.000000 spatialprompt-0.0.2/MANIFEST.in
+-rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/PKG-INFO
+-rw-------   0 asish     (1000) asish     (1000)      108 2023-04-28 09:19:00.000000 spatialprompt-0.0.2/README.md
+-rw-rw-r--   0 asish     (1000) asish     (1000)       38 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/setup.cfg
+-rw-------   0 asish     (1000) asish     (1000)      841 2023-04-28 09:21:20.000000 spatialprompt-0.0.2/setup.py
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/spatialprompt/
+-rw-------   0 asish     (1000) asish     (1000)    18939 2023-04-28 09:19:06.000000 spatialprompt-0.0.2/spatialprompt/__init__.py
+drwxrwxr-x   0 asish     (1000) asish     (1000)        0 2023-04-28 09:22:45.161530 spatialprompt-0.0.2/spatialprompt.egg-info/
+-rw-rw-r--   0 asish     (1000) asish     (1000)      653 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/PKG-INFO
+-rw-rw-r--   0 asish     (1000) asish     (1000)      252 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/SOURCES.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)        1 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/dependency_links.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)       83 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/requires.txt
+-rw-rw-r--   0 asish     (1000) asish     (1000)       14 2023-04-28 09:22:45.000000 spatialprompt-0.0.2/spatialprompt.egg-info/top_level.txt
```

### Comparing `spatialprompt-0.0.1/PKG-INFO` & `spatialprompt-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: spatialprompt
-Version: 0.0.1
-Summary: Scalable and efficient Cell type deconvolution and clustering in spatial transcriptomics
+Version: 0.0.2
+Summary: Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
 Home-page: 
 Author: Asish Kumar Swain
 Author-email: swainkasish@gmail.com
 License: MIT
 Keywords: willupdate
 Classifier: Development Status :: 3 - Alpha 
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
-# SpatialCDR
+# SpatialPrompt 
+## Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
```

### Comparing `spatialprompt-0.0.1/setup.py` & `spatialprompt-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='spatialprompt',
-  version='0.0.1',
-  description='Scalable and efficient Cell type deconvolution and clustering in spatial transcriptomics',
+  version='0.0.2',   #mandatory change
+  description='Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics',
   long_description=open('README.md').read() ,
   url='',  
   author='Asish Kumar Swain',
   author_email='swainkasish@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='willupdate', 
   packages=find_packages(),
-  install_requires=['pandas>=2.0.1',
+  install_requires=['pandas>=1.3.5',
         'numpy>=1.21.6',
-        'scikit-learn>=1.2.2',
-        "alive_progress>=3.1.1",
-        "scipy>=1.9.1"] 
+        'scikit-learn>=1.0.2',
+        "alive_progress>=3.0.1",
+        "scipy>=1.7.3"] 
 )
```

### Comparing `spatialprompt-0.0.1/spatialprompt/__init__.py` & `spatialprompt-0.0.2/spatialprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Created on Tue Jun 28 12:11:26 2022
-
 @author: swainkasish@gmail.com
-spatialCDR version : 0.0.8
+spatialprompt_V 0.0.2
 """
 #%%
 #%% import libraries 
 import numpy as np
 import pandas as pd 
 import time 
 from sklearn.preprocessing import  StandardScaler,Normalizer,MinMaxScaler
 from sklearn.decomposition import PCA,TruncatedSVD
 from sklearn.neighbors import KNeighborsRegressor
 from alive_progress import alive_bar
 from scipy.spatial import cKDTree
 from  scipy.spatial.distance import cdist
 from sklearn.cluster import KMeans,AgglomerativeClustering
 from sklearn.linear_model import Ridge,RidgeCV
+
 #%%
 class SpatialDeconvolution:
     def __init__(self):
         pass
     
     def __preprocessing__(self,sc_array,st_array,sc_genes,st_genes,n_hvgs=1000):
         
@@ -262,21 +262,21 @@
     def __domain_neighbor_index__(self,expr_matrix,x_cor,y_cor,n_neighbor=50):
         x_cor,y_cor = np.array(x_cor),np.array(y_cor)
         cor_mat = np.array([x_cor,y_cor],dtype=np.float32).T
         tree = cKDTree(cor_mat)    
         distances, nei_indexes = tree.query(cor_mat, k=n_neighbor)
         nei_indexes = nei_indexes[:,1:]
         n_spot,n_gene = expr_matrix.shape
-        domain_index = np.zeros([n_spot,int(n_neighbor/3)])
+        domain_index = np.zeros([n_spot,int(n_neighbor/2)])
         for i in range(n_spot):
             own_expression = expr_matrix[i,:]
             spot_nei_index = nei_indexes[i]
             nei_expression = expr_matrix[spot_nei_index,:]
             similarity  = 1-cdist(own_expression.reshape(1,-1),nei_expression,'cosine')[0]
-            spot_dom_index = spot_nei_index[np.argsort(similarity)[::-1][0:int(n_neighbor/3)]]
+            spot_dom_index = spot_nei_index[np.argsort(similarity)[::-1][0:int(n_neighbor/2)]]
             domain_index[i,:] = spot_dom_index
         domain_index = np.array(domain_index,dtype=np.int32)
         return domain_index
     
     def __domain_inspired__(self,expr_matrx,domain_index,n_itr=3,W=0.3):
         n_spot,n_gene = expr_matrx.shape
         expr_spatial_neighbor = np.array([expr_matrx[domain_index[i,:],:].mean(axis=0) for i in range(n_spot)],dtype=np.float32)
@@ -352,15 +352,15 @@
 
         return predict
     
     
     def predict_cell_prop(self,sc_array,st_array,
                           sc_genes,st_genes,sc_labels,
                           x_cord,y_cord,
-                          n_hvgs=1000,min_cell=10,max_cell=15,return_prop=True,spot_ratio= [0.33,0.33,0.33],n_neighbor=40,n_itr=3):
+                          n_hvgs=1000,min_cell=10,max_cell=15,return_prop=True,spot_ratio= [0.33,0.33,0.33],n_neighbor=45,n_itr=3):
         t1 = time.time()
         sc_processed,st_processed = self.__preprocessing__(sc_array, st_array,
                                                            sc_genes, st_genes,n_hvgs=n_hvgs) 
 
         simu_st_arr,simu_ct_prop = self.__simulate_st_spots__(sc_processed,sc_labels,min_cell=min_cell,
                                                                max_cell=max_cell,spot_ratio=spot_ratio)
         
@@ -390,15 +390,15 @@
         # std = StandardScaler()
         std = MinMaxScaler()
         pca =   TruncatedSVD(n_components=50)
         st_df_graph_std = std.fit_transform(df)
         st_df_graph_pca = pca.fit_transform(st_df_graph_std)
         if n_clus=="auto":
             n_clus = self.__auto_k_find__(st_df_graph_pca)
-        kmean = KMeans(n_clusters=n_clus,init ="k-means++",n_init=1)
+        kmean = KMeans(n_clusters=n_clus)
         kmean.fit(st_df_graph_pca)
         labels = np.array(kmean.labels_)
         return labels
     
     def __auto_k_find__(self,data):
         n_row,_ = data.shape
         random_row = np.random.choice(n_row,5000)
@@ -415,15 +415,15 @@
         df_row_sum = df.sum(axis=1)    #tpm
         df = df.div(df_row_sum,axis=0)* 10**6
         df = df.fillna(0)   
         minmax= MinMaxScaler()
         df = minmax.fit_transform(df)
         return np.array(df)
     
-    def fit_predict(self,st_array,x_cor,y_cor,n_neighbor=30,n_itr=3,n_cluster="auto",W=0.4,n_hvg=1000):
+    def fit_predict(self,st_array,x_cor,y_cor,n_neighbor=20,n_itr=3,n_cluster="auto",W=0.4,n_hvg=1000):
         t1 = time.time()
         with alive_bar(5,title="Spatial clustering: ") as bar:
             st_array_hvg = self.__hvg_detect__(st_array,N=n_hvg)
             bar()
             st_array_hvg_norm = self.__normalisation3__(st_array_hvg)
             deconv_class = SpatialDeconvolution()
             domain_index = deconv_class.__domain_neighbor_index__(st_array_hvg_norm, x_cor, y_cor,n_neighbor=n_neighbor)
@@ -434,8 +434,10 @@
             bar()
             cluster_assignment = self.__kmean_clus__(st_array_hvg_norm_domain,n_clus = n_cluster)
             cluster_assignment = pd.Categorical(cluster_assignment)
             bar()
         t2 = time.time()
         print(f"Executed in {t2-t1} second")
         
-        return cluster_assignment
+        return cluster_assignment
+
+
```

### Comparing `spatialprompt-0.0.1/spatialprompt.egg-info/PKG-INFO` & `spatialprompt-0.0.2/spatialprompt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: spatialprompt
-Version: 0.0.1
-Summary: Scalable and efficient Cell type deconvolution and clustering in spatial transcriptomics
+Version: 0.0.2
+Summary: Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
 Home-page: 
 Author: Asish Kumar Swain
 Author-email: swainkasish@gmail.com
 License: MIT
 Keywords: willupdate
 Classifier: Development Status :: 3 - Alpha 
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
-# SpatialCDR
+# SpatialPrompt 
+## Scalable and efficient cell type deconvolution and clustering in spatial transcriptomics
```

