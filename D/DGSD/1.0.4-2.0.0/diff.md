# Comparing `tmp/DGSD-1.0.4.tar.gz` & `tmp/DGSD-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DGSD-1.0.4.tar", last modified: Wed Feb 17 13:23:24 2021, max compression
+gzip compressed data, was "dist/DGSD-2.0.0.tar", last modified: Fri Apr 28 18:16:38 2023, max compression
```

## Comparing `DGSD-1.0.4.tar` & `DGSD-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-02-17 13:23:24.590983 DGSD-1.0.4/
-drwxrwxrwx   0        0        0        0 2021-02-17 13:23:24.584574 DGSD-1.0.4/DGSD.egg-info/
--rw-rw-rw-   0        0        0      654 2021-02-17 13:23:24.000000 DGSD-1.0.4/DGSD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2021-02-17 13:23:24.000000 DGSD-1.0.4/DGSD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-17 13:23:24.000000 DGSD-1.0.4/DGSD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2021-02-17 13:23:24.000000 DGSD-1.0.4/DGSD.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-02-17 13:23:24.000000 DGSD-1.0.4/DGSD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       18 2020-02-26 18:46:43.000000 DGSD-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      654 2021-02-17 13:23:24.591968 DGSD-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      838 2021-02-17 11:49:46.000000 DGSD-1.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2021-02-17 13:23:24.589247 DGSD-1.0.4/dgsd/
--rw-rw-rw-   0        0        0      109 2021-02-17 13:21:20.000000 DGSD-1.0.4/dgsd/__init__.py
--rw-rw-rw-   0        0        0     1876 2021-02-17 11:39:50.000000 DGSD-1.0.4/dgsd/main.py
--rw-rw-rw-   0        0        0       87 2021-02-17 13:23:24.594646 DGSD-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      925 2021-02-17 13:22:54.000000 DGSD-1.0.4/setup.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-04-28 18:16:38.000000 DGSD-2.0.0/
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      648 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      222 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/SOURCES.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/dependency_links.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       15 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/requires.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        5 2023-04-28 18:16:38.000000 DGSD-2.0.0/DGSD.egg-info/top_level.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1066 2023-04-27 19:08:44.000000 DGSD-2.0.0/LICENSE.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       18 2023-04-27 19:08:44.000000 DGSD-2.0.0/MANIFEST.in
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      648 2023-04-28 18:16:38.000000 DGSD-2.0.0/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1268 2023-04-27 19:08:44.000000 DGSD-2.0.0/README.rst
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-04-28 18:16:38.000000 DGSD-2.0.0/dgsd/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      107 2023-04-28 18:03:50.000000 DGSD-2.0.0/dgsd/__init__.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1853 2023-04-27 19:06:38.000000 DGSD-2.0.0/dgsd/main.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       80 2023-04-28 18:16:38.000000 DGSD-2.0.0/setup.cfg
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      934 2023-04-28 18:11:03.000000 DGSD-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `DGSD-1.0.4/DGSD.egg-info/PKG-INFO` & `DGSD-2.0.0/DGSD.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
-Name: DGSD
-Version: 1.0.4
-Summary: DGSD: Distributed Graph Representation via Graph Statistical Properties!
-Home-page: https://github.com/Anwar-Said/DGSD
-Author: Anwar Said
-Author-email: anwar.said@itu.edu.pk
-License: MIT
-Download-URL: https://github.com/Anwar-Said/DGSD/archive/v1.0.4.tar.gz
-Description: long_description
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Metadata-Version: 2.1
+Name: DGSD
+Version: 2.0.0
+Summary: DGSD: Distributed Graph Representation via Graph Statistical Properties
+Home-page: https://github.com/Anwar-Said/DGSD
+Download-URL: https://github.com/Anwar-Said/DGSD/releases/download/v2.0.0/DGSD.tar.gz
+Author: Anwar Said
+Author-email: anwar.said@itu.edu.pk
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+License-File: LICENSE.txt
+
+long_description
```

### Comparing `DGSD-1.0.4/PKG-INFO` & `DGSD-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 1.1
-Name: DGSD
-Version: 1.0.4
-Summary: DGSD: Distributed Graph Representation via Graph Statistical Properties!
-Home-page: https://github.com/Anwar-Said/DGSD
-Author: Anwar Said
-Author-email: anwar.said@itu.edu.pk
-License: MIT
-Download-URL: https://github.com/Anwar-Said/DGSD/archive/v1.0.4.tar.gz
-Description: long_description
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Metadata-Version: 2.1
+Name: DGSD
+Version: 2.0.0
+Summary: DGSD: Distributed Graph Representation via Graph Statistical Properties
+Home-page: https://github.com/Anwar-Said/DGSD
+Download-URL: https://github.com/Anwar-Said/DGSD/releases/download/v2.0.0/DGSD.tar.gz
+Author: Anwar Said
+Author-email: anwar.said@itu.edu.pk
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+License-File: LICENSE.txt
+
+long_description
```

### Comparing `DGSD-1.0.4/dgsd/main.py` & `DGSD-2.0.0/dgsd/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-import multiprocessing as mp
-import time
-import networkx as nx
-import numpy as np
-from itertools import repeat
-import csv
-import math
-import sys
-
-class DGSD:
-    def __init__(self):
-        self.graph = None
-    def get_descriptor(self, graph, bins = 50, workers=1):
-        p = mp.Pool(workers)
-        self.graph = nx.convert_node_labels_to_integers(graph)
-        nodes = list(self.graph.nodes())
-        if workers<len(nodes):
-            batches = np.array_split(nodes, workers)
-        else:
-            workers = len(nodes)
-            batches = np.array_split(nodes, workers)
-        emb = p.starmap(self.Generate_Embeddings, zip(batches, repeat(bins)))
-        embeddings = np.sum(np.array(emb),axis = 0)
-        return embeddings
-
-    def Generate_Embeddings(self, batch, nbins):
-        total_nodes = self.get_nodes()
-        d = []
-        for v in batch:
-            N_v = self.request_neighbors(v)
-            d_v = len(N_v)
-            for u in range(total_nodes):
-                if u == v:
-                    d.append(0)
-                    continue
-                N_u = self.request_neighbors(u)
-                delta = 0
-                if u in N_v:
-                    delta = 1
-                else:
-                    delta = 0
-                d_u = len(N_u)
-                common = len(list(set(N_u) & set(N_v)))
-                dist = 0
-                if (((d_u + d_v) + common + delta))>0:
-                    dist = (d_u + d_v) / ((d_u + d_v) + common + delta)
-                delta = 0
-                d.append(dist)
-        hist, bin_edges = np.histogram(d, range=(0, 1), bins=nbins)
-        return hist
-
-    def request_neighbors(self, node):
-        N_i = list(self.graph.neighbors(node))
-        return N_i
-
-    def get_nodes(self):
-        return self.graph.number_of_nodes()
-    
+import multiprocessing as mp
+import time
+import networkx as nx
+import numpy as np
+from itertools import repeat
+import csv
+import math
+import sys
+
+class DGSD:
+    def __init__(self):
+        self.graph = None
+    def get_descriptor(self, graph, bins = 50, workers=1):
+        p = mp.Pool(workers)
+        self.graph = nx.convert_node_labels_to_integers(graph)
+        nodes = list(self.graph.nodes())
+        if workers<len(nodes):
+            batches = np.array_split(nodes, workers)
+        else:
+            workers = len(nodes)
+            batches = np.array_split(nodes, workers)
+        emb = p.starmap(self.Generate_Embeddings, zip(batches, repeat(bins)))
+        embeddings = np.sum(np.array(emb),axis = 0)
+        p.close()
+        p.join()
+        return embeddings
+
+    def Generate_Embeddings(self, batch, nbins):
+        total_nodes = self.get_nodes()
+        d = []
+        for v in batch:
+            N_v = self.request_neighbors(v)
+            d_v = len(N_v)
+            for u in range(total_nodes):
+                if u == v:
+                    d.append(0)
+                    continue
+                N_u = self.request_neighbors(u)
+                delta = 0
+                if u in N_v:
+                    delta = 1
+                else:
+                    delta = 0
+                d_u = len(N_u)
+                common = len(list(set(N_u) & set(N_v)))
+                dist = 0
+                if (((d_u + d_v) + common + delta))>0:
+                    dist = (d_u + d_v) / ((d_u + d_v) + common + delta)
+                delta = 0
+                d.append(dist)
+        hist, bin_edges = np.histogram(d, range=(0, 1), bins=nbins)
+        return hist
+
+    def request_neighbors(self, node):
+        N_i = list(self.graph.neighbors(node))
+        return N_i
+
+    def get_nodes(self):
+        return self.graph.number_of_nodes()
+
```

### Comparing `DGSD-1.0.4/setup.py` & `DGSD-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='DGSD',
-    version='v1.0.4',
+    version='v2.0.0',
     author='Anwar Said',
     author_email='anwar.said@itu.edu.pk',
-    description='DGSD: Distributed Graph Representation via Graph Statistical Properties!',
+    description='DGSD: Distributed Graph Representation via Graph Statistical Properties',
     long_description='long_description',
     packages=['dgsd',],
     url='https://github.com/Anwar-Said/DGSD',
-    download_url = 'https://github.com/Anwar-Said/DGSD/archive/v1.0.4.tar.gz',
+    download_url = 'https://github.com/Anwar-Said/DGSD/releases/download/v2.0.0/DGSD.tar.gz',
     license='MIT',
     install_requires=[
         'numpy',
-        'networkx==2.5'
+        'networkx'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
 )
```

