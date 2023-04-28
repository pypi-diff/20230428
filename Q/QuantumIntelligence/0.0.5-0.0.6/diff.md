# Comparing `tmp/QuantumIntelligence-0.0.5.tar.gz` & `tmp/QuantumIntelligence-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumIntelligence-0.0.5.tar", last modified: Fri Apr 28 05:21:39 2023, max compression
+gzip compressed data, was "QuantumIntelligence-0.0.6.tar", last modified: Fri Apr 28 05:27:26 2023, max compression
```

## Comparing `QuantumIntelligence-0.0.5.tar` & `QuantumIntelligence-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.676466 QuantumIntelligence-0.0.5/
--rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1763 2023-04-28 05:21:39.675391 QuantumIntelligence-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 05:21:39.676557 QuantumIntelligence-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     8844 2023-04-28 05:06:53.000000 QuantumIntelligence-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.647011 QuantumIntelligence-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.651836 QuantumIntelligence-0.0.5/src/QuantumIntelligence/
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.664937 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/
--rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/__init__.py
--rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
--rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
--rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.669432 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/
--rw-rw-rw-   0        0        0    48902 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Circuit.py
--rw-rw-rw-   0        0        0     9960 2023-04-05 10:35:49.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Gate.py
--rw-rw-rw-   0        0        0    18259 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Simulator.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.674723 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/
--rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/MPSclass.py
--rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TEBD.py
--rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TNclass.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 05:21:39.657170 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/
--rw-rw-rw-   0        0        0     1763 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-28 05:21:39.000000 QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.138677 QuantumIntelligence-0.0.6/
+-rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-04-28 05:27:26.138251 QuantumIntelligence-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 05:27:26.138914 QuantumIntelligence-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     8844 2023-04-28 05:27:11.000000 QuantumIntelligence-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.101615 QuantumIntelligence-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.106491 QuantumIntelligence-0.0.6/src/QuantumIntelligence/
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.117843 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/
+-rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/__init__.py
+-rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
+-rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
+-rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.117843 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/
+-rw-rw-rw-   0        0        0    48902 2023-04-28 05:17:22.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Circuit.py
+-rw-rw-rw-   0        0        0     9960 2023-04-05 10:35:49.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Gate.py
+-rw-rw-rw-   0        0        0    18240 2023-04-28 05:27:11.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Simulator.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.136565 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/
+-rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/MPSclass.py
+-rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TEBD.py
+-rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TNclass.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 05:27:26.111528 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-28 05:27:26.000000 QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/top_level.txt
```

### Comparing `QuantumIntelligence-0.0.5/LICENSE` & `QuantumIntelligence-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/PKG-INFO` & `QuantumIntelligence-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.5
+Version: 0.0.6
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.5/README.md` & `QuantumIntelligence-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/setup.py` & `QuantumIntelligence-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="QuantumIntelligence",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.5",  # Required
+    version="0.0.6",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Developing quantum intelligence.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Circuit.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Circuit.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Gate.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Gate.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/QuantumSimulator/Simulator.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/QuantumSimulator/Simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,14 @@
         for kk in new_state.keys():
             if tc.abs(new_state[kk]) < 1e-8:
                 pop_keys.append(kk)
         for kk in pop_keys:
             new_state.pop(kk)
         self._state = new_state
 
-    @staticmethod
     def sampling(self, n_shots=1024, position=None, if_print=True, rand_seed=None, return_weight=False):
         if rand_seed is None:
             rand_seed = self.rand_seed
         if rand_seed is not None:
             random.seed(rand_seed)
         m_p = len(position)
         population = list()
```

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/MPSclass.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/MPSclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TEBD.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TEBD.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence/TEBD/TNclass.py` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence/TEBD/TNclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/PKG-INFO` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.5
+Version: 0.0.6
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.5/src/QuantumIntelligence.egg-info/SOURCES.txt` & `QuantumIntelligence-0.0.6/src/QuantumIntelligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

