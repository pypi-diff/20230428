# Comparing `tmp/rils-rols-0.5.tar.gz` & `tmp/rils-rols-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rils-rols-0.5.tar", last modified: Sun Nov 27 18:42:01 2022, max compression
+gzip compressed data, was "dist\rils-rols-1.0.tar", last modified: Fri Apr 28 07:21:39 2023, max compression
```

## Comparing `rils-rols-0.5.tar` & `rils-rols-1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-27 18:42:01.769603 rils-rols-0.5/
--rw-rw-rw-   0        0        0     1079 2022-08-30 22:23:15.000000 rils-rols-0.5/LICENSE
--rw-rw-rw-   0        0        0     2338 2022-11-27 18:42:01.768602 rils-rols-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-27 18:42:01.763604 rils-rols-0.5/rils_rols/
--rw-rw-rw-   0        0        0        0 2022-08-30 22:23:14.000000 rils-rols-0.5/rils_rols/__init__.py
--rw-rw-rw-   0        0        0    17133 2022-11-27 08:16:45.000000 rils-rols-0.5/rils_rols/node.py
--rw-rw-rw-   0        0        0    26035 2022-11-27 09:15:20.000000 rils-rols-0.5/rils_rols/rils_rols.py
--rw-rw-rw-   0        0        0    10930 2022-11-27 08:19:59.000000 rils-rols-0.5/rils_rols/solution.py
--rw-rw-rw-   0        0        0     2089 2022-09-02 18:08:35.000000 rils-rols-0.5/rils_rols/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-27 18:42:01.768602 rils-rols-0.5/rils_rols.egg-info/
--rw-rw-rw-   0        0        0     2338 2022-11-27 18:42:01.000000 rils-rols-0.5/rils_rols.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2022-11-27 18:42:01.000000 rils-rols-0.5/rils_rols.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-27 18:42:01.000000 rils-rols-0.5/rils_rols.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-11-27 18:42:01.000000 rils-rols-0.5/rils_rols.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-11-27 18:42:01.000000 rils-rols-0.5/rils_rols.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-27 18:42:01.769603 rils-rols-0.5/setup.cfg
--rw-rw-rw-   0        0        0      885 2022-11-27 18:41:51.000000 rils-rols-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.819861 rils-rols-1.0/
+-rw-rw-rw-   0        0        0     1079 2022-08-30 22:23:15.000000 rils-rols-1.0/LICENSE
+-rw-rw-rw-   0        0        0     2663 2023-04-28 07:21:39.819861 rils-rols-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.814861 rils-rols-1.0/rils_rols/
+-rw-rw-rw-   0        0        0        0 2022-12-22 15:10:42.000000 rils-rols-1.0/rils_rols/__init__.py
+-rw-rw-rw-   0        0        0    18211 2023-04-11 12:16:34.000000 rils-rols-1.0/rils_rols/node.py
+-rw-rw-rw-   0        0        0    29033 2023-04-28 07:11:52.000000 rils-rols-1.0/rils_rols/rils_rols.py
+-rw-rw-rw-   0        0        0     3633 2023-04-28 06:53:21.000000 rils-rols-1.0/rils_rols/rils_rols_ensemble.py
+-rw-rw-rw-   0        0        0    11918 2023-04-11 12:16:34.000000 rils-rols-1.0/rils_rols/solution.py
+-rw-rw-rw-   0        0        0     2627 2023-04-07 12:50:36.000000 rils-rols-1.0/rils_rols/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:21:39.818861 rils-rols-1.0/rils_rols.egg-info/
+-rw-rw-rw-   0        0        0     2663 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 07:21:39.000000 rils-rols-1.0/rils_rols.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:21:39.820861 rils-rols-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-04-27 11:53:59.000000 rils-rols-1.0/setup.py
```

### Comparing `rils-rols-0.5/LICENSE` & `rils-rols-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rils-rols-0.5/PKG-INFO` & `rils-rols-1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: rils-rols
-Version: 0.5
+Version: 1.0
 Summary: RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares
 Home-page: https://github.com/kartelj/rils-rols
 Author: Aleksandar Kartelj, Marko Đukanović
 Author-email: aleksandar.kartelj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# General
+
 RILS-ROLS is metaheuristic-based framework to deal with problems of symbolic regression. 
 
 All of its aspects (method description, empirical results, etc.) are explained in the paper named:
 "RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares" by Aleksandar Kartelj and Marko Djukanovic. 
 This paper is currently under review in the Journal of Big Data, Springer. 
 
 All RILS-ROLS resources can be found at https://github.com/kartelj/rils-rols
 
 RILS-ROLS distribution is available as a pip package at https://pypi.org/project/rils-rols
+so it can be easily installed with the following pip command:
+
+```bat
+pip install rils-rols
+```
 
-Minimal working example can be seen bellow:
+# Minimal working example
 ```python
 from rils_rols.rils_rols import RILSROLSRegressor
 from math import sin, log
 
 regr = RILSROLSRegressor()
 ''' regressor parameters:
     1. max_fit_calls=100000         -- maximal number of fitness function calls
@@ -47,8 +54,16 @@
 print("Final model is "+str(regr.model))
 
 # applies the model to a list of input vectors, also well-known predict method
 X_test = [[4, 4], [3, 3]]
 y_test = regr.predict(X_test)
 print(y_test)
 ```
+# Citation
 
+```
+@article{kartelj2022rils,
+  title={RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares},
+  author={Kartelj, Aleksandar and Djukanovi{\'c}, Marko},
+  year={2022}
+}
+```
```

### Comparing `rils-rols-0.5/rils_rols/node.py` & `rils-rols-1.0/rils_rols/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,40 @@
         left_size = 0
         if self.left!=None:
             left_size = self.left.size()
         right_size = 0
         if self.right!=None:
             right_size = self.right.size()
         return 1+left_size+right_size
+    
+    def size_non_linear(self):
+        left_size = 0
+        if self.left!=None:
+            left_size = self.left.size_non_linear()
+        right_size = 0
+        if self.right!=None:
+            right_size = self.right.size_non_linear()
+        # counting the level of non-linearity, so excluding terms and operations plus and minus
+        if type(self)!=type(NodeConstant(0)) and type(self)!=type(NodeVariable(0)) and type(self)!=type(NodePlus) and type(self)!=type(NodeMinus):
+            return 1+left_size+right_size
+        else:
+            return left_size+right_size
+        
+    def size_operators_only(self):
+        left_size = 0
+        if self.left!=None:
+            left_size = self.left.size_operators_only()
+        right_size = 0
+        if self.right!=None:
+            right_size = self.right.size_operators_only()
+        # not counting terms
+        if type(self)!=type(NodeConstant(0)) and type(self)!=type(NodeVariable(0)):
+            return 1+left_size+right_size
+        else:
+            return left_size+right_size
 
     def contains_type(self, search_type):
         if type(self)==search_type:
             return True
         if self.left!=None and self.left.contains_type(search_type):
             return True
         if self.right!=None and self.right.contains_type(search_type):
```

### Comparing `rils-rols-0.5/rils_rols/rils_rols.py` & `rils-rols-1.0/rils_rols/rils_rols.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,42 @@
 import time
 import math
 from random import Random, shuffle
 from sklearn.base import BaseEstimator
 import copy
 from sympy import *
 from .node import Node, NodeConstant, NodeVariable, NodePlus, NodeMinus, NodeMultiply, NodeDivide, NodeSqr, NodeSqrt, NodeLn, NodeExp, NodeSin, NodeCos
-
+from enum import Enum
 import warnings
-
 from .solution import Solution
+
 warnings.filterwarnings("ignore")
 
+
+class FitnessType(Enum):
+    BIC = 1 # bayesian information criterion
+    SRM = 2 # structural risk minimization
+    PENALTY = 3 # penalty based fitness function
+
 class RILSROLSRegressor(BaseEstimator):
 
-    def __init__(self, max_fit_calls=100000, max_seconds=100, complexity_penalty=0.001, error_tolerance=1e-16,random_state=0):
+    def __init__(self, max_fit_calls=100000, max_seconds=100, fitness_type=FitnessType.PENALTY, complexity_penalty=0.001, initial_sample_size=0.01,  
+                 random_perturbations_order = False, verbose=False, random_state=0):
         self.max_seconds = max_seconds
         self.max_fit_calls = max_fit_calls
+        self.fitness_type = fitness_type
         self.complexity_penalty = complexity_penalty
+        self.initial_sample_size = initial_sample_size
+        self.error_tolerance = 1e-16
+        self.verbose = verbose
+        self.random_perturbations_order = random_perturbations_order
         self.random_state = random_state
-        self.error_tolerance = error_tolerance
 
     def __reset(self):
         self.model = None
-        self.varNames = None
         self.ls_it = 0
         self.main_it = 0
         self.last_improved_it = 0
         self.time_start = 0
         self.time_elapsed = 0
         self.rg = Random(self.random_state)
         Solution.clearStats()
@@ -40,20 +50,21 @@
             self.allowed_nodes.append(NodeVariable(i))
         self.allowed_nodes+=[NodePlus(), NodeMinus(), NodeMultiply(), NodeDivide(), NodeSqr(), NodeSqrt(),NodeLn(), NodeExp(),NodeSin(), NodeCos()]#, NodeArcSin(), NodeArcCos()]
 
     def fit(self, X, y):
         x_all = copy.deepcopy(X)
         y_all = copy.deepcopy(y)
         # take 1% of points or at least 100 points initially 
-        n = int(0.01*len(x_all))
-        if n<100:
-            n=min(100, len(X))
-        print("Taking "+str(n)+" points initially.")
-        X = x_all[:n]
-        y = y_all[:n]
+        self.n = int(self.initial_sample_size*len(x_all))
+        if self.n<100:
+            self.n=min(100, len(X))
+        print("Taking "+str(self.n)+" points initially.")
+        X = x_all[:self.n]
+        y = y_all[:self.n]
+
         size_increased_main_it = 0
 
         self.__reset()
         self.start = time.time()
         if len(X) == 0:
             raise Exception("Input feature data set (X) cannot be empty.")
         if len(X)!=len(y):
@@ -72,33 +83,39 @@
             for pret in all_perturbations: 
                 pret_ols = copy.deepcopy(pret)
                 pret_ols = pret_ols.fit_constants_OLS(X, y)
                 pret_ols_fit = pret_ols.fitness(X, y)
                 pret_fits[pret]=pret_ols_fit[0]
 
             sorted_pret_fits = sorted(pret_fits.items(), key = lambda x: x[1])
+            if self.random_perturbations_order:
+                shuffle(sorted_pret_fits)
+
             impr = False
             p = 0
             for pret, r2Inv in sorted_pret_fits:
                 p+=1
                 self.time_elapsed = time.time()-self.start
                 if self.time_elapsed>self.max_seconds:
                     break
                 if str(pret) in checked_perturbations:
-                    print(str(p)+"/"+str(len(sorted_pret_fits))+". "+str(pret)+" SKIPPED")
+                    if self.verbose:
+                        print(str(p)+"/"+str(len(sorted_pret_fits))+". "+str(pret)+" SKIPPED")
                     continue
                 checked_perturbations.add(str(pret))
-                print(str(p)+"/"+str(len(sorted_pret_fits))+". "+str(pret))
+                if self.verbose:
+                    print(str(p)+"/"+str(len(sorted_pret_fits))+". "+str(pret))
                 new_solution = pret 
                 new_solution.simplify_whole(len(X[0]))
                 new_fitness = new_solution.fitness(X, y)
                 new_solution = self.LS_best(new_solution, X, y)
                 new_fitness = new_solution.fitness(X, y, False)
                 if self.compare_fitness(new_fitness, best_fitness)<0:
-                    print("perturbation "+str(pret)+" produced global improvement.")
+                    if self.verbose:
+                        print("perturbation "+str(pret)+" produced global improvement.")
                     best_solution = copy.deepcopy(new_solution)
                     best_fitness = new_fitness
                     impr = True
                     break
 
             start_solution = copy.deepcopy(best_solution)
             if not impr:
@@ -115,34 +132,36 @@
                     # perform 2-consecutive perturbations -- do not check if this did happen before, it is very small chance for that
                     if len(all_perturbations)>0:
                         perturbation1 = all_perturbations[0]
                         all2_perturbations = self.all_perturbations(perturbation1, len(X[0]))
                         if len(all2_perturbations)>0:
                             start_solution = all2_perturbations[self.rg.randrange(len(all2_perturbations))]
 
-                print("RANDOMIZING "+str(best_solution)+" TO "+str(start_solution))
-                if n<len(x_all) and (self.main_it-size_increased_main_it)>=10:
-                    n*=2
-                    if n>len(x_all):
-                        n = len(x_all)
-                    print("Increasing data count to "+str(n))
-                    X = x_all[:n]
-                    y = y_all[:n]
+                if self.verbose:
+                    print("RANDOMIZING "+str(best_solution)+" TO "+str(start_solution))
+                if self.n<len(x_all) and (self.main_it-size_increased_main_it)>=10:
+                    self.n*=2
+                    if self.n>len(x_all):
+                        self.n = len(x_all)
+                    print("Increasing data count to "+str(self.n))
+                    X = x_all[:self.n]
+                    y = y_all[:self.n]
                     size_increased_main_it = self.main_it
                     Node.reset_node_value_cache()
 
             self.time_elapsed = time.time()-self.start
-            print("%d/%d. t=%.1f R2=%.7f RMSE=%.7f size=%d factors=%d mathErr=%d fitCalls=%d fitFails=%d cHits=%d cTries=%d cPerc=%.1f cSize=%d\n                                                                          expr=%s"
-            %(self.main_it,self.ls_it, self.time_elapsed, 1-best_fitness[0], best_fitness[1],best_solution.size(), len(best_solution.factors), Solution.math_error_count, Solution.fit_calls, Solution.fit_fails, Node.cache_hits, Node.cache_tries, Node.cache_hits*100.0/Node.cache_tries, len(Node.node_value_cache), best_solution))
+            print("%d/%d. t=%.1f R2=%.7f RMSE=%.7f size=%d fitFails=%d/%d cPerc=%.1f expr=%s"
+            %(self.main_it,self.ls_it, self.time_elapsed, 1-best_fitness[0], best_fitness[1],best_solution.size(), Solution.fit_fails, Solution.fit_calls,Node.cache_hits*100.0/Node.cache_tries, best_solution))
             self.main_it+=1
             if best_fitness[0]<=self.error_tolerance and best_fitness[1] <= pow(self.error_tolerance, 0.125):
                 break
         self.model_simp = simplify(str(best_solution), ratio=1)
         self.model_simp = self.round_floats(self.model_simp)
         self.model = Solution([Solution.convert_to_my_nodes(self.model_simp)], self.complexity_penalty)
+        return (self.model, self.model_simp)
     
     def round_floats(self, ex1):
         round_digits = int(math.log10(1/self.error_tolerance))
         if round_digits>8:
             round_digits = 8
         #if round_digits<4:
         #    round_digits = 4
@@ -170,20 +189,20 @@
             return str(self.model_simp)
         return ""
 
     def fit_report_string(self, X, y):
         if self.model==None:
             raise Exception("Model is not build yet. First call fit().")
         fitness = self.model.fitness(X,y, False)
-        return "maxTime={0}\tmaxFitCalls={1}\tseed={2}\tsizePenalty={3}\tR2={4:.7f}\tRMSE={5:.7f}\tsize={6}\tsec={7:.1f}\tmainIt={8}\tlsIt={9}\tfitCalls={10}\texpr={11}\texprSimp={12}\terrTol={13}".format(
-            self.max_seconds,self.max_fit_calls,self.random_state,self.complexity_penalty, 1-fitness[0], fitness[1], self.complexity(), self.time_elapsed,self.main_it, self.ls_it,Solution.fit_calls, self.model, self.model_simp, self.error_tolerance)
+        return "maxTime={0}\tmaxFitCalls={1}\tseed={2}\tsizePenalty={3}\tR2={4:.7f}\tRMSE={5:.7f}\tsize={6}\tsec={7:.1f}\tmainIt={8}\tlsIt={9}\tfitCalls={10}\texpr={11}\texprSimp={12}\tfitType={13}\tinitSampleSize={14}\trandomPert={15}".format(
+            self.max_seconds,self.max_fit_calls,self.random_state,self.complexity_penalty, 1-fitness[0], fitness[1], self.complexity(self.model_simp), self.time_elapsed,self.main_it, self.ls_it,Solution.fit_calls, self.model, self.model_simp, self.fitness_type, self.initial_sample_size, self.random_perturbations_order)
 
-    def complexity(self):
+    def complexity(self, sm):
         c=0
-        for arg in preorder_traversal(self.model_simp):
+        for arg in preorder_traversal(sm):
             c += 1
         return c
 
     def all_perturbations(self, solution: Solution, var_cnt):
         all = []
         shaked_solution = copy.deepcopy(solution)
         shaked_solution.normalize_constants()
@@ -241,17 +260,19 @@
                 best_solution.simplify_whole(len(X[0]))
                 best_fitness = best_solution.fitness(X, y, False)
                 if self.compare_fitness(best_fitness, old_best_fitness)>=0:
                     impr = False
                     impr2 = False
                     best_solution = old_best_solution
                     best_fitness = old_best_fitness
-                    print("REVERTING back to old best "+str(best_solution))
-                #else:
-                #    print("IMPROVED with LS-change impr="+str(impr)+" impr2="+str(impr2)+" "+str(1-best_fitness[0])+"  "+str(best_solution))
+                    if self.verbose:
+                        print("REVERTING back to old best "+str(best_solution))
+                else:
+                    if self.verbose:
+                        print("IMPROVED with LS-change impr="+str(impr)+" impr2="+str(impr2)+" "+str(1-best_fitness[0])+"  "+str(best_solution))
                 continue  
         return best_solution
 
     def LS_best_change_iteration(self, solution: Solution, X, y, cache, joined=False):
         best_fitness = solution.fitness(X, y, False)
         best_solution = copy.deepcopy(solution)
         if joined:
@@ -470,16 +491,62 @@
                     continue
                 if not is_left_from_parent and not parent.is_allowed_right_argument(c):
                     continue
                 filtered_candidates.append(c)
             candidates = filtered_candidates
         candidates = sorted(candidates, key=lambda x: str(x))
         return candidates
-
+    
     def compare_fitness(self, new_fit, old_fit):
+        if self.fitness_type == FitnessType.BIC:
+            return self.compare_fitness_bic(new_fit, old_fit)
+        elif self.fitness_type == FitnessType.SRM:
+            return self.compare_fitness_srm(new_fit, old_fit)
+        elif self.fitness_type == FitnessType.PENALTY:
+            return self.compare_fitness_penalty(new_fit, old_fit)
+        else:
+            raise Exception("Unrecognized fitness type "+str(self.fitness_type))
+
+    def compare_fitness_bic(self, new_fit, old_fit):
+        if math.isnan(new_fit[0]):
+            return 1
+        # BIC -- see equation (9) in https://www.researchgate.net/profile/Jose-Montana/publication/220743408_Model_selection_in_genetic_programming/links/0c960532776628e069000000/Model-selection-in-genetic-programming.pdf
+        new_mse = new_fit[1]*new_fit[1]
+        old_mse = old_fit[1]*old_fit[1]
+        new_h = new_fit[2]
+        old_h = old_fit[2]
+        new_var = new_fit[3]
+        old_var = old_fit[3]
+        new_tot = new_mse + math.log(self.n)*new_h*new_var/self.n
+        old_tot = old_mse + math.log(self.n)*old_h*old_var/self.n
+        if new_tot<old_tot-0.00000001:
+            return -1
+        if new_tot>old_tot+0.00000001:
+            return 1
+        return 0
+    
+    def compare_fitness_srm(self, new_fit, old_fit):
+        if math.isnan(new_fit[0]):
+            return 1
+        # SRM -- see equation (11) in https://www.researchgate.net/profile/Jose-Montana/publication/220743408_Model_selection_in_genetic_programming/links/0c960532776628e069000000/Model-selection-in-genetic-programming.pdf
+        new_mse = new_fit[1]*new_fit[1]
+        old_mse = old_fit[1]*old_fit[1]
+        new_h = new_fit[4] # non-linear size
+        old_h = old_fit[4]
+        new_p = new_h/self.n
+        old_p = old_h/self.n
+        new_tot = new_mse/(1-math.sqrt(new_p-new_p*math.log(new_p)+math.log(self.n)/(2*self.n)))
+        old_tot = old_mse/(1-math.sqrt(old_p-old_p*math.log(old_p)+math.log(self.n)/(2*self.n)))
+        if new_tot<old_tot-0.00000001:
+            return -1
+        if new_tot>old_tot+0.00000001:
+            return 1
+        return 0
+
+    def compare_fitness_penalty(self, new_fit, old_fit):
         if math.isnan(new_fit[0]):
             return 1
         new_fit_wo_size_pen = (1+new_fit[0])*(1+new_fit[1]) 
         old_fit_wo_size_pen = (1+old_fit[0])*(1+old_fit[1]) 
         if new_fit_wo_size_pen*old_fit_wo_size_pen!=1: # otherwise, if they are both 1 (perfect), code bellow will return better based on the size
             if new_fit_wo_size_pen==1: # if this one is perfrect solution, return it
                 return -1
```

### Comparing `rils-rols-0.5/rils_rols/solution.py` & `rils-rols-1.0/rils_rols/solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import copy
 from math import e, inf
 import math
 from .node import NodeAbs, NodeArcCos, NodeArcSin, NodeArcTan, NodeCeil, NodeConstant, NodeCos, NodeExp, NodeFloor, NodeLn, NodeMax, NodeMin, NodeMultiply, NodePlus, NodePow, NodeSgn, NodeSin, NodeTan, NodeVariable
-from .utils import R2, RMSE
+from .utils import R2, RMSE, ResidualVariance
 from sympy import *
 from sympy.core.numbers import ImaginaryUnit
 from sympy.core.symbol import Symbol
 import numpy as np
 import statsmodels.api as sma
+import hashlib
 
 class Solution:
 
     math_error_count = 0
     fit_calls = 0
     fit_fails = 0
 
@@ -24,39 +25,60 @@
     def __init__(self, factors, complexity_penalty):
         # factors are basically subexpressions that enter linear combination, e.g. 2*x+3y*sin(x*y) --> factors = [2x, 3y*sin(x*y)]
         self.factors =  copy.deepcopy(factors)
         self.complexity_penalty = complexity_penalty
 
     def __str__(self) -> str:
         return "+".join([str(x) for x in self.factors])
-
+    
+    def __eq__(self, other):
+        return str(self) == str(other)
+    
+    def __hash__(self):
+        # Stable hash (same for different runs, unlike standard hash() method)
+        h = hashlib.sha1(str(self).encode("ascii"))
+        return int(h.hexdigest(), 16)
+        #return hash(str(self))
+    
     def evaluate_all(self,X, cache):
         yp = np.zeros(len(X))
         for fact in self.factors:
             fyp = fact.evaluate_all(X, cache)
             for i in range(len(fyp)):
                 yp[i]+=fyp[i]
         return yp
 
     def fitness(self, X, y, cache=True):
         try:
             Solution.fit_calls+=1
             yp = self.evaluate_all(X, cache) 
-            return (1-R2(y, yp), RMSE(y, yp), self.size())
+            return (1-R2(y, yp), RMSE(y, yp), self.size(), ResidualVariance(y, yp, self.size()), self.size_non_linear(), self.size_operators_only())
         except Exception as e:
             #print(e)
             Solution.math_error_count+=1
             Solution.fit_fails+=1
-            return (inf, inf, inf)
+            return (inf, inf, inf, inf, inf, inf)
 
     def size(self):
         totSize = len(self.factors) 
         for fact in self.factors:
             totSize+=fact.size()
         return totSize
+    
+    def size_non_linear(self):
+        totSize = 1
+        for fact in self.factors:
+            totSize+=fact.size_non_linear()
+        return totSize
+    
+    def size_operators_only(self):
+        totSize = len(self.factors)
+        for fact in self.factors:
+            totSize+=fact.size_operators_only()
+        return totSize
 
     def fit_constants_OLS(self, X, y):
         new_factors = []
         for fact in self.factors:
             if fact.contains_type(type(NodeVariable(0))):
                 new_factors.append(copy.deepcopy(fact))
         Xnew = np.zeros((len(X), len(new_factors)))
@@ -224,14 +246,18 @@
                 try:
                     index = int(str(sympy_node).replace("x",""))
                     return NodeVariable(index)
                 except Exception as ex:
                     print(sympy_node)
                     print(ex)
             else:
+                if str(sympy_node)=="1/2":
+                    return NodeConstant(0.5)
+                elif str(sympy_node)=="1/10":
+                    return NodeConstant(0.1)
                 return NodeConstant(float(str(sympy_node)))
 
         if len(sympy_node.args)==1:
             if type(sympy_node)==exp:
                 new = NodeExp()
             elif type(sympy_node)==cos:
                 new = NodeCos()
```

### Comparing `rils-rols-0.5/rils_rols/utils.py` & `rils-rols-1.0/rils_rols/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,89 @@
-from math import nan, sqrt
-from statistics import mean
-from numpy.random import RandomState
-
-# described in Apendix 4 of paper Contemporary Symbolic Regression Methods and their Relative Performance
-def noisefy(y, noise_level, random_state):
-    yRMSE = 0
-    for i in range(len(y)):
-        yRMSE+=(y[i]*y[i])
-    yRMSE=sqrt(yRMSE/len(y))
-    yRMSE_noise_SD = noise_level*yRMSE
-    rg = RandomState(random_state)
-    noise = rg.normal(0, yRMSE_noise_SD, len(y))
-    y_n = []
-    for i in range(len(y)):
-        y_n.append(y[i]+noise[i])
-    return y_n
-
-def RMSE(yt, yp):
-    if len(yp)!=len(yt):
-        raise Exception("Vectors of predicted and true y values should be of same size.")
-    try:
-        rmse = 0.0
-        for i in range(len(yp)):
-            err = yp[i]-yt[i]
-            err*=err
-            if err == nan:
-                return nan
-            rmse+=err
-        rmse = sqrt(rmse/len(yp))
-        return rmse
-    except OverflowError:
-       return nan
-
-def percentile_abs_error(yt, yp, percentile):
-    if len(yp)!=len(yt):
-        raise Exception("Vectors of predicted and true y values should be of same size.")
-    try:
-        errors = []
-        for i in range(len(yp)):
-            err = yp[i]-yt[i]
-            if err<0:
-                err*=-1
-            if err == nan:
-                return nan
-            errors.append(err)
-        errors.sort()
-        idx = int(percentile*(len(yp)-1)/100)
-        return errors[idx]
-    except OverflowError:
-        return nan
-
-def R2(yt, yp):
-    if len(yp)!=len(yt):
-        raise Exception("Vectors of predicted and true y values should be of same size.")
-    try:
-        yt_mean = mean(yt)
-        ss_res = 0
-        ss_tot = 0
-        for i in range(len(yp)):
-            err = yp[i]-yt[i]
-            err*=err
-            if err == nan:
-                return nan
-            ss_res+=err
-            var_err = yt_mean-yt[i]
-            var_err*=var_err
-            ss_tot+=var_err
-        if ss_tot<0.000000000001:
-            ss_tot=1
-        return 1-ss_res/ss_tot
-    except OverflowError:
+from math import nan, sqrt
+from statistics import mean
+from numpy.random import RandomState
+
+# described in Apendix 4 of paper Contemporary Symbolic Regression Methods and their Relative Performance
+def noisefy(y, noise_level, random_state):
+    yRMSE = 0
+    for i in range(len(y)):
+        yRMSE+=(y[i]*y[i])
+    yRMSE=sqrt(yRMSE/len(y))
+    yRMSE_noise_SD = noise_level*yRMSE
+    rg = RandomState(random_state)
+    noise = rg.normal(0, yRMSE_noise_SD, len(y))
+    y_n = []
+    for i in range(len(y)):
+        y_n.append(y[i]+noise[i])
+    return y_n
+
+def RMSE(yt, yp):
+    if len(yp)!=len(yt):
+        raise Exception("Vectors of predicted and true y values should be of same size.")
+    try:
+        rmse = 0.0
+        for i in range(len(yp)):
+            err = yp[i]-yt[i]
+            err*=err
+            if err == nan:
+                return nan
+            rmse+=err
+        rmse = sqrt(rmse/len(yp))
+        return rmse
+    except OverflowError:
+       return nan
+    
+def ResidualVariance(yt, yp, complexity):
+    if len(yp)!=len(yt):
+        raise Exception("Vectors of predicted and true y values should be of same size.")
+    try:
+        var = 0.0
+        for i in range(len(yp)):
+            err = yp[i]-yt[i]
+            err*=err
+            if err == nan:
+                return nan
+            var+=err
+        var = var/(len(yp)-complexity)
+        return var
+    except OverflowError:
+       return nan
+
+def percentile_abs_error(yt, yp, percentile):
+    if len(yp)!=len(yt):
+        raise Exception("Vectors of predicted and true y values should be of same size.")
+    try:
+        errors = []
+        for i in range(len(yp)):
+            err = yp[i]-yt[i]
+            if err<0:
+                err*=-1
+            if err == nan:
+                return nan
+            errors.append(err)
+        errors.sort()
+        idx = int(percentile*(len(yp)-1)/100)
+        return errors[idx]
+    except OverflowError:
+        return nan
+
+def R2(yt, yp):
+    if len(yp)!=len(yt):
+        raise Exception("Vectors of predicted and true y values should be of same size.")
+    try:
+        yt_mean = mean(yt)
+        ss_res = 0
+        ss_tot = 0
+        for i in range(len(yp)):
+            err = yp[i]-yt[i]
+            err*=err
+            if err == nan:
+                return nan
+            ss_res+=err
+            var_err = yt_mean-yt[i]
+            var_err*=var_err
+            ss_tot+=var_err
+        if ss_tot<0.000000000001:
+            ss_tot=1
+        return 1-ss_res/ss_tot
+    except OverflowError:
         return nan
```

### Comparing `rils-rols-0.5/rils_rols.egg-info/PKG-INFO` & `rils-rols-1.0/rils_rols.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 Metadata-Version: 2.1
 Name: rils-rols
-Version: 0.5
+Version: 1.0
 Summary: RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares
 Home-page: https://github.com/kartelj/rils-rols
 Author: Aleksandar Kartelj, Marko Đukanović
 Author-email: aleksandar.kartelj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# General
+
 RILS-ROLS is metaheuristic-based framework to deal with problems of symbolic regression. 
 
 All of its aspects (method description, empirical results, etc.) are explained in the paper named:
 "RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares" by Aleksandar Kartelj and Marko Djukanovic. 
 This paper is currently under review in the Journal of Big Data, Springer. 
 
 All RILS-ROLS resources can be found at https://github.com/kartelj/rils-rols
 
 RILS-ROLS distribution is available as a pip package at https://pypi.org/project/rils-rols
+so it can be easily installed with the following pip command:
+
+```bat
+pip install rils-rols
+```
 
-Minimal working example can be seen bellow:
+# Minimal working example
 ```python
 from rils_rols.rils_rols import RILSROLSRegressor
 from math import sin, log
 
 regr = RILSROLSRegressor()
 ''' regressor parameters:
     1. max_fit_calls=100000         -- maximal number of fitness function calls
@@ -47,8 +54,16 @@
 print("Final model is "+str(regr.model))
 
 # applies the model to a list of input vectors, also well-known predict method
 X_test = [[4, 4], [3, 3]]
 y_test = regr.predict(X_test)
 print(y_test)
 ```
+# Citation
 
+```
+@article{kartelj2022rils,
+  title={RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares},
+  author={Kartelj, Aleksandar and Djukanovi{\'c}, Marko},
+  year={2022}
+}
+```
```

### Comparing `rils-rols-0.5/setup.py` & `rils-rols-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='rils-rols',
-    version='0.5',
+    version='1.0',
     description='RILS-ROLS: Robust Symbolic Regression via Iterated Local Search and Ordinary Least Squares',
     long_description= long_description,
     long_description_content_type  = "text/markdown",
     author='Aleksandar Kartelj, Marko Đukanović',
     author_email='aleksandar.kartelj@gmail.com',
     url='https://github.com/kartelj/rils-rols',
     packages = find_packages(),
```

