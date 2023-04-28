# Comparing `tmp/kronbinations-1.6.tar.gz` & `tmp/kronbinations-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kronbinations-1.6.tar", last modified: Thu Apr 27 21:11:01 2023, max compression
+gzip compressed data, was "kronbinations-1.7.tar", last modified: Fri Apr 28 08:21:19 2023, max compression
```

## Comparing `kronbinations-1.6.tar` & `kronbinations-1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/
--rw-rw-rw-   0        0        0     1096 2023-04-27 18:44:03.000000 kronbinations-1.6/LICENSE
--rw-rw-rw-   0        0        0     6252 2023-04-27 21:11:01.290420 kronbinations-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5724 2023-04-27 18:44:03.000000 kronbinations-1.6/README.md
--rw-rw-rw-   0        0        0      523 2023-04-27 21:11:01.306044 kronbinations-1.6/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-04-27 18:44:03.000000 kronbinations-1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.227919 kronbinations-1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.259170 kronbinations-1.6/src/kronbinations/
--rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.6/src/kronbinations/JIT_Array.py
--rw-rw-rw-   0        0        0    17493 2023-04-27 18:49:16.000000 kronbinations-1.6/src/kronbinations/JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.6/src/kronbinations/Kron_Array.py
--rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.6/src/kronbinations/Kron_Fun_Modifier.py
--rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.6/src/kronbinations/__init__.py
--rw-rw-rw-   0        0        0    12896 2023-04-27 18:48:42.000000 kronbinations-1.6/src/kronbinations/kronbinations.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/src/kronbinations.egg-info/
--rw-rw-rw-   0        0        0     6252 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-04-27 21:11:01.000000 kronbinations-1.6/src/kronbinations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-27 21:11:00.000000 kronbinations-1.6/src/kronbinations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 21:11:01.290420 kronbinations-1.6/test/
--rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.6/test/test_JIT_kronbinations.py
--rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.6/test/test_kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:21:19.823191 kronbinations-1.7/
+-rw-rw-rw-   0        0        0     1096 2023-04-28 07:58:36.000000 kronbinations-1.7/LICENSE
+-rw-rw-rw-   0        0        0     6395 2023-04-28 08:21:19.824184 kronbinations-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5867 2023-04-28 07:58:36.000000 kronbinations-1.7/README.md
+-rw-rw-rw-   0        0        0      523 2023-04-28 08:21:19.828184 kronbinations-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-04-28 07:58:37.000000 kronbinations-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:21:19.708087 kronbinations-1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 08:21:19.743256 kronbinations-1.7/src/kronbinations/
+-rw-rw-rw-   0        0        0     9324 2023-04-17 10:40:53.000000 kronbinations-1.7/src/kronbinations/JIT_Array.py
+-rw-rw-rw-   0        0        0    17564 2023-04-28 08:20:21.000000 kronbinations-1.7/src/kronbinations/JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3087 2023-04-17 10:40:45.000000 kronbinations-1.7/src/kronbinations/Kron_Array.py
+-rw-rw-rw-   0        0        0    44564 2023-02-24 16:06:05.000000 kronbinations-1.7/src/kronbinations/Kron_Fun_Modifier.py
+-rw-rw-rw-   0        0        0      241 2023-02-27 13:26:54.000000 kronbinations-1.7/src/kronbinations/__init__.py
+-rw-rw-rw-   0        0        0    12796 2023-04-28 08:20:15.000000 kronbinations-1.7/src/kronbinations/kronbinations.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:21:19.788015 kronbinations-1.7/src/kronbinations.egg-info/
+-rw-rw-rw-   0        0        0     6395 2023-04-28 08:21:19.000000 kronbinations-1.7/src/kronbinations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-04-28 08:21:19.000000 kronbinations-1.7/src/kronbinations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:21:19.000000 kronbinations-1.7/src/kronbinations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 08:21:19.000000 kronbinations-1.7/src/kronbinations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 08:21:19.000000 kronbinations-1.7/src/kronbinations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 08:21:19.820664 kronbinations-1.7/test/
+-rw-rw-rw-   0        0        0     4862 2023-04-17 15:21:41.000000 kronbinations-1.7/test/test_JIT_kronbinations.py
+-rw-rw-rw-   0        0        0     3564 2023-04-17 13:58:07.000000 kronbinations-1.7/test/test_kronbinations.py
```

### Comparing `kronbinations-1.6/LICENSE` & `kronbinations-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kronbinations-1.6/PKG-INFO` & `kronbinations-1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.6
+Version: 1.7
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -84,9 +84,12 @@
 
 k = JIT_kronbinations(a, b, c, func=gridspace, redo=False, progress=True) 
 A = k.zeros()
 B = k.zeros()
 plt.imshow(A.array())
 ```
 
+### Tricks
+You can use `k.tqdm(iterator)` in subloops which will lead to subiterations getting recognized und updated in the progress bar.
+
 ## Authors: 
 By Michael Schilling
```

### Comparing `kronbinations-1.6/README.md` & `kronbinations-1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,9 +70,12 @@
 
 k = JIT_kronbinations(a, b, c, func=gridspace, redo=False, progress=True) 
 A = k.zeros()
 B = k.zeros()
 plt.imshow(A.array())
 ```
 
+### Tricks
+You can use `k.tqdm(iterator)` in subloops which will lead to subiterations getting recognized und updated in the progress bar.
+
 ## Authors: 
 By Michael Schilling
```

### Comparing `kronbinations-1.6/setup.py` & `kronbinations-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "kronbinations",
-    version            = "1.6",
+    version             = "1.7",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "kronbinations is used to remove nested loops and perform parameter sweeps.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz",
+    url = "https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.7.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `kronbinations-1.6/src/kronbinations/JIT_Array.py` & `kronbinations-1.7/src/kronbinations/JIT_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.6/src/kronbinations/JIT_kronbinations.py` & `kronbinations-1.7/src/kronbinations/JIT_kronbinations.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,16 @@
                 self.array_vars_all[i] = np.array([arr])
         # only relevant values in array_directions
         self.array_vars = [arr for arr in self.array_vars_all if len(arr) > 1]
         if isinstance(values, dict):
             self.array_vars_names = [name for name, arr in zip(self.array_vars_all_names, self.array_vars_all) if len(arr) > 1]
         # add index values of the array vars 
         self.array_vars_indexes = [i for i, arr in enumerate(self.array_vars_all) if len(arr) > 1] 
-
+        self.weights = [w for i, w in enumerate(self.all_weights) if i in self.array_vars_indexes]
+        
         if self.return_as_dict:
             self.curr_vals = {key: arr[0] for key, arr in zip(self.array_vars_all_names, self.array_vars_all)}
         else:
             self.curr_vals = [arr[0] for arr in self.array_vars_all]
 
         self.array_lengths_all = [len(arr) for arr in self.array_vars_all]
         self.array_lengths = [len(arr) for arr in self.array_vars]
@@ -271,15 +272,15 @@
             self.last_indexes_all = self.indexes_all
             self.changed_var = changed_var
         return self.last_values, self.last_indexes, self.changed_var
 
     def kronprod(self, **args):
         self.set(**args)
         if self.do_tqdm and self.total_length > 1:
-            self.pbar.init(np.array(list(itertools.product(*self.index_list))))
+            self.pbar.init(self.indexes)
         if self.do_index:
             if self.do_change:
                 for n in range(self.total_length):
                     v,i,c = next(self)
                     yield tuple(i), v, c
                     if self.do_tqdm and self.total_length > 1:
                         self.pbar.increment()
@@ -303,17 +304,17 @@
                     if self.do_tqdm and self.total_length > 1:
                         self.pbar.increment()
         if self.do_tqdm and self.total_length > 1:
             self.pbar.close()
             
     def tqdm(self, iterator, weights=None, name='', **kwargs):
         if self.do_tqdm:
-            yield self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
+            return self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
         else:
-            yield weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
+            return weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
 
     def changed(self, elem=None):
         if elem is None:
             return self.changed_var
         elif isinstance(elem, int):
             if self.return_as_dict:
                 string = self.array_vars_all_names[elem]
```

### Comparing `kronbinations-1.6/src/kronbinations/Kron_Array.py` & `kronbinations-1.7/src/kronbinations/Kron_Array.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.6/src/kronbinations/Kron_Fun_Modifier.py` & `kronbinations-1.7/src/kronbinations/Kron_Fun_Modifier.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.6/src/kronbinations/kronbinations.py` & `kronbinations-1.7/src/kronbinations/kronbinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,17 @@
                         self.pbar.increment()
         if self.do_tqdm:
             self.pbar.close()
         self.setup_iterator()
         
     def tqdm(self, iterator, weights=None, name='', **kwargs):
         if self.do_tqdm:
-            yield self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
+            return self.pbar.sub_tqdm(iterator, weights=weights, name=name, **kwargs)
         else:
-            yield weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
+            return weighted_tqdm(iterator, weights=weights, name=name, **kwargs)
 
     def changed(self, elem=None):
         if elem is None:
             return self.changed_var
         elif isinstance(elem, int):
             if self.return_as_dict:
                 string = self.array_vars_all_names[elem]
@@ -281,25 +281,8 @@
         # loop over all combinations
         for i, v in self.kronprod(change=False):
             for j in range(self.ndim_all):
                 array_vars_all[j][i] = v[j]
         return array_vars_all
     
     
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-
```

### Comparing `kronbinations-1.6/src/kronbinations.egg-info/PKG-INFO` & `kronbinations-1.7/src/kronbinations.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kronbinations
-Version: 1.6
+Version: 1.7
 Summary: kronbinations is used to remove nested loops and perform parameter sweeps.
-Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.6.tar.gz
+Home-page: https://github.com/Ntropic/kronbinations/archive/refs/tags/v1.7.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -84,9 +84,12 @@
 
 k = JIT_kronbinations(a, b, c, func=gridspace, redo=False, progress=True) 
 A = k.zeros()
 B = k.zeros()
 plt.imshow(A.array())
 ```
 
+### Tricks
+You can use `k.tqdm(iterator)` in subloops which will lead to subiterations getting recognized und updated in the progress bar.
+
 ## Authors: 
 By Michael Schilling
```

### Comparing `kronbinations-1.6/test/test_JIT_kronbinations.py` & `kronbinations-1.7/test/test_JIT_kronbinations.py`

 * *Files identical despite different names*

### Comparing `kronbinations-1.6/test/test_kronbinations.py` & `kronbinations-1.7/test/test_kronbinations.py`

 * *Files identical despite different names*

