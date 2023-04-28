# Comparing `tmp/complex-network-link-prediction-1.0.tar.gz` & `tmp/complex-network-link-prediction-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex-network-link-prediction-1.0.tar", last modified: Fri Apr 28 15:39:16 2023, max compression
+gzip compressed data, was "complex-network-link-prediction-1.0.1.tar", last modified: Fri Apr 28 19:55:19 2023, max compression
```

## Comparing `complex-network-link-prediction-1.0.tar` & `complex-network-link-prediction-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.989191 complex-network-link-prediction-1.0/cnlp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.989191 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-28 15:39:16.000000 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 15:39:16.000000 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:39:16.000000 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 15:39:16.000000 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 15:39:16.000000 complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/cnlp/other_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/other_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/other_methods/information_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/cnlp/probabilistic_methods/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/probabilistic_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/probabilistic_methods/sbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/cnlp/similarity_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/similarity_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/similarity_methods/global_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/similarity_methods/local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/cnlp/similarity_methods/quasi_local_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 15:39:16.993191 complex-network-link-prediction-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-28 15:39:15.000000 complex-network-link-prediction-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/dimensionality_reduction_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/other_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/other_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/other_methods/information_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/sbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/global_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/similarity_methods/quasi_local_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/cnlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 19:55:19.000000 complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 19:55:19.631379 complex-network-link-prediction-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 19:55:18.000000 complex-network-link-prediction-1.0.1/setup.py
```

### Comparing `complex-network-link-prediction-1.0/LICENSE` & `complex-network-link-prediction-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/PKG-INFO` & `complex-network-link-prediction-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-network-link-prediction
-Version: 1.0
+Version: 1.0.1
 Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
 Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
 License: MIT
 Keywords: Link Prediction,Social Network,Complex Network Analisys
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `complex-network-link-prediction-1.0/README.md` & `complex-network-link-prediction-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/PKG-INFO` & `complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-network-link-prediction
-Version: 1.0
+Version: 1.0.1
 Home-page: https://github.com/Typing-Monkeys/social-network-link-prediction
 Author: Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani
 License: MIT
 Keywords: Link Prediction,Social Network,Complex Network Analisys
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `complex-network-link-prediction-1.0/cnlp/complex_network_link_prediction.egg-info/SOURCES.txt` & `complex-network-link-prediction-1.0.1/complex_network_link_prediction.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
-cnlp/complex_network_link_prediction.egg-info/PKG-INFO
-cnlp/complex_network_link_prediction.egg-info/SOURCES.txt
-cnlp/complex_network_link_prediction.egg-info/dependency_links.txt
-cnlp/complex_network_link_prediction.egg-info/requires.txt
-cnlp/complex_network_link_prediction.egg-info/top_level.txt
+cnlp/__init__.py
+cnlp/dimensionality_reduction_methods.py
+cnlp/utils.py
 cnlp/other_methods/__init__.py
 cnlp/other_methods/information_theory.py
 cnlp/probabilistic_methods/__init__.py
 cnlp/probabilistic_methods/sbm.py
 cnlp/similarity_methods/__init__.py
 cnlp/similarity_methods/global_similarity.py
 cnlp/similarity_methods/local_similarity.py
-cnlp/similarity_methods/quasi_local_similarity.py
+cnlp/similarity_methods/quasi_local_similarity.py
+complex_network_link_prediction.egg-info/PKG-INFO
+complex_network_link_prediction.egg-info/SOURCES.txt
+complex_network_link_prediction.egg-info/dependency_links.txt
+complex_network_link_prediction.egg-info/requires.txt
+complex_network_link_prediction.egg-info/top_level.txt
```

### Comparing `complex-network-link-prediction-1.0/cnlp/other_methods/information_theory.py` & `complex-network-link-prediction-1.0.1/cnlp/other_methods/information_theory.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/probabilistic_methods/sbm.py` & `complex-network-link-prediction-1.0.1/cnlp/probabilistic_methods/sbm.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/similarity_methods/__init__.py` & `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/similarity_methods/global_similarity.py` & `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/global_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/similarity_methods/local_similarity.py` & `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/local_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/cnlp/similarity_methods/quasi_local_similarity.py` & `complex-network-link-prediction-1.0.1/cnlp/similarity_methods/quasi_local_similarity.py`

 * *Files identical despite different names*

### Comparing `complex-network-link-prediction-1.0/setup.py` & `complex-network-link-prediction-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='complex-network-link-prediction',
-    version='1.0',
+    version='1.0.1',
     license='MIT',
     author=
     "Cristian Cosci, Fabrizio Fagiolo, Nicolò Vescera, Nicolò Posta, Tommaso Romani",
-    packages=find_packages('cnlp'),
-    package_dir={'': 'cnlp'},
+    packages=find_packages(where='.', include=['cnlp*']),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Typing-Monkeys/social-network-link-prediction',
     keywords='Link Prediction, Social Network, Complex Network Analisys',
     install_requires=[
         'networkx',
         'scipy',
```

