# Comparing `tmp/wave_train-1.0.7.tar.gz` & `tmp/wave_train-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wave_train-1.0.7.tar", last modified: Fri Feb 10 17:35:13 2023, max compression
+gzip compressed data, was "wave_train-1.0.8.tar", last modified: Thu Apr 27 11:21:32 2023, max compression
```

## Comparing `wave_train-1.0.7.tar` & `wave_train-1.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.449581 wave_train-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-10 17:34:59.000000 wave_train-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-10 17:35:13.449581 wave_train-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-02-10 17:34:59.000000 wave_train-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-10 17:35:13.449581 wave_train-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-10 17:34:59.000000 wave_train-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.441581 wave_train-1.0.7/wave_train/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.445581 wave_train-1.0.7/wave_train/dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/ceom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/class_mech.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/qcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/qu_cl_mech.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/quant_mech.py
--rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/tdse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/dynamics/tise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.445581 wave_train-1.0.7/wave_train/graphics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    40592 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/graphics/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.445581 wave_train-1.0.7/wave_train/hamilton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/hamilton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/hamilton/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/hamilton/coupled.py
--rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/hamilton/exciton.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/hamilton/phonon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.449581 wave_train-1.0.7/wave_train/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/collect3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/collect4_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/collect4_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-10 17:34:59.000000 wave_train-1.0.7/wave_train/io/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:35:13.441581 wave_train-1.0.7/wave_train.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-10 17:35:13.000000 wave_train-1.0.7/wave_train.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-10 17:35:13.000000 wave_train-1.0.7/wave_train.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 17:35:13.000000 wave_train-1.0.7/wave_train.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-10 17:35:13.000000 wave_train-1.0.7/wave_train.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-10 17:35:13.000000 wave_train-1.0.7/wave_train.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.060404 wave_train-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 11:21:21.000000 wave_train-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-27 11:21:32.060404 wave_train-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-27 11:21:21.000000 wave_train-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 11:21:32.060404 wave_train-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-27 11:21:21.000000 wave_train-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.056404 wave_train-1.0.8/wave_train/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.056404 wave_train-1.0.8/wave_train/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/ceom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/class_mech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/qcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/qu_cl_mech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/quant_mech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21543 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/tdse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/dynamics/tise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.060404 wave_train-1.0.8/wave_train/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40592 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/graphics/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.060404 wave_train-1.0.8/wave_train/hamilton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/hamilton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/hamilton/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/hamilton/coupled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/hamilton/exciton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/hamilton/phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.060404 wave_train-1.0.8/wave_train/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/collect3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/collect4_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/collect4_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-27 11:21:21.000000 wave_train-1.0.8/wave_train/io/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:21:32.056404 wave_train-1.0.8/wave_train.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-27 11:21:32.000000 wave_train-1.0.8/wave_train.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-27 11:21:32.000000 wave_train-1.0.8/wave_train.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:21:32.000000 wave_train-1.0.8/wave_train.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 11:21:32.000000 wave_train-1.0.8/wave_train.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 11:21:32.000000 wave_train-1.0.8/wave_train.egg-info/top_level.txt
```

### Comparing `wave_train-1.0.7/LICENSE` & `wave_train-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/PKG-INFO` & `wave_train-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave_train
-Version: 1.0.7
+Version: 1.0.8
 Summary: Numerical quantum mechanics of chain-like systems based on tensor trains
 Author: Jerome Riedel, Patrick Gelß, Burkhard Schmidt
 Author-email: burkhard.schmidt@fu-berlin.de
 License: GNU v3.0
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 fully classical and mixed quantum-classical (Ehrenfest or mean field) dynamics of bipartite 
 ("slow-fast" and/or "heavy-light") systems.
 Moreover, the graphical capabilities allow visualization of quantum dynamics ‘on the fly’, with a choice of 
 several different graphical representations based on reduced density matrices.
 
 ## Full description
 
-For a detailed description of the WaveTrain software, see our article that appeared 2023 at arXiv[^1] 
+For a detailed description of the WaveTrain software, see our article that appeared in February 2023 at arXiv[^1]. To appear in J. Chem. Phys. 
 
 ## Installation
 After downloading and installing the Python tensor train toolbox [scikit\_tt](https://github.com/PGelss/scikit_tt),
 installation of the **WaveTrain** software package is straightforward
 ```
 pip install git+https://github.com/PGelss/scikit_tt
 pip install wave_train
```

### Comparing `wave_train-1.0.7/README.md` & `wave_train-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 fully classical and mixed quantum-classical (Ehrenfest or mean field) dynamics of bipartite 
 ("slow-fast" and/or "heavy-light") systems.
 Moreover, the graphical capabilities allow visualization of quantum dynamics ‘on the fly’, with a choice of 
 several different graphical representations based on reduced density matrices.
 
 ## Full description
 
-For a detailed description of the WaveTrain software, see our article that appeared 2023 at arXiv[^1] 
+For a detailed description of the WaveTrain software, see our article that appeared in February 2023 at arXiv[^1]. To appear in J. Chem. Phys. 
 
 ## Installation
 After downloading and installing the Python tensor train toolbox [scikit\_tt](https://github.com/PGelss/scikit_tt),
 installation of the **WaveTrain** software package is straightforward
 ```
 pip install git+https://github.com/PGelss/scikit_tt
 pip install wave_train
```

### Comparing `wave_train-1.0.7/wave_train/dynamics/ceom.py` & `wave_train-1.0.8/wave_train/dynamics/ceom.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/class_mech.py` & `wave_train-1.0.8/wave_train/dynamics/class_mech.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/mechanics.py` & `wave_train-1.0.8/wave_train/dynamics/mechanics.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/qcmd.py` & `wave_train-1.0.8/wave_train/dynamics/qcmd.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/qu_cl_mech.py` & `wave_train-1.0.8/wave_train/dynamics/qu_cl_mech.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/quant_mech.py` & `wave_train-1.0.8/wave_train/dynamics/quant_mech.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/dynamics/tdse.py` & `wave_train-1.0.8/wave_train/dynamics/tdse.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,15 +375,23 @@
             order = int(self.solver[1])
             self.op_hod = 2 * self.sub_size * self.operator.copy()
             op_tmp = self.operator.copy()
             for k in range(2, order // 2 + 1):
                 op_tmp = op_tmp.dot(self.operator).dot(self.operator)
                 self.op_hod += 2 / np.math.factorial(2 * k - 1) * self.sub_size ** (2 * k - 1) * op_tmp
             self.op_hod = self.op_hod.ortho(threshold=self.threshold)
-
+            
+        # Increase rank of initial quantum state for TDVP
+        if self.solver in ['vp']:
+            psi_tmp = self.psi
+            for i in range(1, self.max_rank):
+                psi_tmp = psi_tmp + self.psi
+            self.psi = psi_tmp.ortho()
+            self.psi = (1/self.psi.norm())*self.psi
+        
     def update_solve(self, i):
 
         with utl.timer() as cputime:
             
             # Propagation for i>0
             if i > 0:
                 
@@ -421,14 +429,18 @@
                                                 number_of_steps=self.sub_steps, threshold=self.threshold,
                                                 max_rank=self.max_rank, normalize=self.normalize)
                 elif self.solver == 'kl':  # Kahan-Li splitting
                     psi = ode.kahan_li_splitting(self.hamilton.S, self.hamilton.L, self.hamilton.I, self.hamilton.M,
                                                 initial_value=self.psi, step_size=self.sub_size,
                                                 number_of_steps=self.sub_steps, threshold=self.threshold,
                                                 max_rank=self.max_rank, normalize=self.normalize)
+                    
+                elif self.solver == 'vp':  # time-dependent variational principle
+                    psi = ode.tdvp(1j*self.operator, initial_value=self.psi, step_size=self.sub_size,
+                                                number_of_steps=self.sub_steps, normalize=self.normalize)
 
                 elif self.solver == 'qe':  # Quasi-exact propagation
                     self.psi = self.propagator @ self.psi
 
                 else:
                     sys.exit('Wrong choice of solver')
```

### Comparing `wave_train-1.0.7/wave_train/dynamics/tise.py` & `wave_train-1.0.8/wave_train/dynamics/tise.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/animation.py` & `wave_train-1.0.8/wave_train/graphics/animation.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/exceptions.py` & `wave_train-1.0.8/wave_train/graphics/exceptions.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/factory.py` & `wave_train-1.0.8/wave_train/graphics/factory.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/helper.py` & `wave_train-1.0.8/wave_train/graphics/helper.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/services.py` & `wave_train-1.0.8/wave_train/graphics/services.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/style.py` & `wave_train-1.0.8/wave_train/graphics/style.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/graphics/visual.py` & `wave_train-1.0.8/wave_train/graphics/visual.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/hamilton/chain.py` & `wave_train-1.0.8/wave_train/hamilton/chain.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/hamilton/coupled.py` & `wave_train-1.0.8/wave_train/hamilton/coupled.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/hamilton/exciton.py` & `wave_train-1.0.8/wave_train/hamilton/exciton.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         print("""
 -------------------------
 Setting up SLIM operators
 -------------------------      
 
 Size of excitonic basis set = {}
         """.format(self.n_dim))
+
         if self.homogen:
             print('shape of S = ', self.S.shape)
             print('shape of L = ', self.L.shape)
             print('shape of I = ', self.I.shape)
             print('shape of M = ', self.M.shape)
 
     def get_exact (self, n_levels):
```

### Comparing `wave_train-1.0.7/wave_train/hamilton/phonon.py` & `wave_train-1.0.8/wave_train/hamilton/phonon.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/io/collect3.py` & `wave_train-1.0.8/wave_train/io/collect3.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/io/collect4_a.py` & `wave_train-1.0.8/wave_train/io/collect4_a.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/io/collect4_b.py` & `wave_train-1.0.8/wave_train/io/collect4_b.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/io/load.py` & `wave_train-1.0.8/wave_train/io/load.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train/io/logging.py` & `wave_train-1.0.8/wave_train/io/logging.py`

 * *Files identical despite different names*

### Comparing `wave_train-1.0.7/wave_train.egg-info/PKG-INFO` & `wave_train-1.0.8/wave_train.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave-train
-Version: 1.0.7
+Version: 1.0.8
 Summary: Numerical quantum mechanics of chain-like systems based on tensor trains
 Author: Jerome Riedel, Patrick Gelß, Burkhard Schmidt
 Author-email: burkhard.schmidt@fu-berlin.de
 License: GNU v3.0
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 fully classical and mixed quantum-classical (Ehrenfest or mean field) dynamics of bipartite 
 ("slow-fast" and/or "heavy-light") systems.
 Moreover, the graphical capabilities allow visualization of quantum dynamics ‘on the fly’, with a choice of 
 several different graphical representations based on reduced density matrices.
 
 ## Full description
 
-For a detailed description of the WaveTrain software, see our article that appeared 2023 at arXiv[^1] 
+For a detailed description of the WaveTrain software, see our article that appeared in February 2023 at arXiv[^1]. To appear in J. Chem. Phys. 
 
 ## Installation
 After downloading and installing the Python tensor train toolbox [scikit\_tt](https://github.com/PGelss/scikit_tt),
 installation of the **WaveTrain** software package is straightforward
 ```
 pip install git+https://github.com/PGelss/scikit_tt
 pip install wave_train
```

### Comparing `wave_train-1.0.7/wave_train.egg-info/SOURCES.txt` & `wave_train-1.0.8/wave_train.egg-info/SOURCES.txt`

 * *Files identical despite different names*

