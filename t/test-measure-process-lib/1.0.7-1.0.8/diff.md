# Comparing `tmp/test_measure_process_lib-1.0.7.tar.gz` & `tmp/test_measure_process_lib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_measure_process_lib-1.0.7.tar", last modified: Sun Feb 26 22:58:56 2023, max compression
+gzip compressed data, was "test_measure_process_lib-1.0.8.tar", last modified: Fri Apr 28 18:42:03 2023, max compression
```

## Comparing `test_measure_process_lib-1.0.7.tar` & `test_measure_process_lib-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-02-26 22:58:56.627693 test_measure_process_lib-1.0.7/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    10273 2021-05-25 23:53:44.000000 test_measure_process_lib-1.0.7/LICENSE.md
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-02-26 22:58:56.627693 test_measure_process_lib-1.0.7/PKG-INFO
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    30554 2023-01-21 14:05:45.000000 test_measure_process_lib-1.0.7/README.md
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      903 2023-02-26 22:51:58.000000 test_measure_process_lib-1.0.7/pyproject.toml
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-02-26 22:58:56.623693 test_measure_process_lib-1.0.7/sandbox/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2023-01-21 13:48:47.000000 test_measure_process_lib-1.0.7/sandbox/set_path_for_notebooks.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       38 2023-02-26 22:58:56.627693 test_measure_process_lib-1.0.7/setup.cfg
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-02-26 22:58:56.623693 test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-02-26 22:58:56.000000 test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/PKG-INFO
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      504 2023-02-26 22:58:56.000000 test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)        1 2023-02-26 22:58:56.000000 test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       51 2023-02-26 22:58:56.000000 test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/top_level.txt
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-02-26 22:58:56.627693 test_measure_process_lib-1.0.7/tmpl/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      509 2023-02-26 22:51:36.000000 test_measure_process_lib-1.0.7/tmpl/__init__.py
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-02-26 22:58:56.627693 test_measure_process_lib-1.0.7/tmpl/examples/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       60 2021-08-01 18:41:18.000000 test_measure_process_lib-1.0.7/tmpl/examples/__init__.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    12475 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.7/tmpl/examples/example_resistor_test.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4947 2021-08-23 12:12:14.000000 test_measure_process_lib-1.0.7/tmpl/examples/resistor_example.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2022-12-21 19:49:01.000000 test_measure_process_lib-1.0.7/tmpl/examples/set_path_for_notebooks.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     9792 2022-10-15 18:40:54.000000 test_measure_process_lib-1.0.7/tmpl/tmp_code_generator.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)   102746 2023-02-26 22:45:55.000000 test_measure_process_lib-1.0.7/tmpl/tmpl_core.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4587 2021-05-25 23:41:52.000000 test_measure_process_lib-1.0.7/tmpl/tmpl_storage.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    16004 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.7/tmpl/tmpl_support.py
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    10273 2021-05-25 23:53:44.000000 test_measure_process_lib-1.0.8/LICENSE.md
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/PKG-INFO
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    30554 2023-01-21 14:05:45.000000 test_measure_process_lib-1.0.8/README.md
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      903 2023-04-28 18:38:19.000000 test_measure_process_lib-1.0.8/pyproject.toml
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/sandbox/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2023-01-21 13:48:47.000000 test_measure_process_lib-1.0.8/sandbox/set_path_for_notebooks.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       38 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/setup.cfg
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      504 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)        1 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       51 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/top_level.txt
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/tmpl/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      509 2023-04-28 18:39:01.000000 test_measure_process_lib-1.0.8/tmpl/__init__.py
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/tmpl/examples/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       60 2021-08-01 18:41:18.000000 test_measure_process_lib-1.0.8/tmpl/examples/__init__.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    12475 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.8/tmpl/examples/example_resistor_test.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4947 2021-08-23 12:12:14.000000 test_measure_process_lib-1.0.8/tmpl/examples/resistor_example.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2022-12-21 19:49:01.000000 test_measure_process_lib-1.0.8/tmpl/examples/set_path_for_notebooks.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     9822 2023-04-28 18:31:02.000000 test_measure_process_lib-1.0.8/tmpl/tmp_code_generator.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)   102795 2023-04-28 18:31:02.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_core.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4587 2021-05-25 23:41:52.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_storage.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    16004 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_support.py
```

### Comparing `test_measure_process_lib-1.0.7/LICENSE.md` & `test_measure_process_lib-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.7/PKG-INFO` & `test_measure_process_lib-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_measure_process_lib
-Version: 1.0.7
+Version: 1.0.8
 Summary: Test, Measure and Process library. Framework for lab experiments.
 Author-email: RedLegJed <rlj_pypi@nym.hush.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test_measure_process_lib-1.0.7/README.md` & `test_measure_process_lib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.7/pyproject.toml` & `test_measure_process_lib-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "test_measure_process_lib"
-version = "1.0.7"
+version = "1.0.8"
 description = "Test, Measure and Process library. Framework for lab experiments."
 readme = "README.md"
 authors = [{ name = "RedLegJed", email = "rlj_pypi@nym.hush.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `test_measure_process_lib-1.0.7/test_measure_process_lib.egg-info/PKG-INFO` & `test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-measure-process-lib
-Version: 1.0.7
+Version: 1.0.8
 Summary: Test, Measure and Process library. Framework for lab experiments.
 Author-email: RedLegJed <rlj_pypi@nym.hush.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test_measure_process_lib-1.0.7/tmpl/examples/example_resistor_test.py` & `test_measure_process_lib-1.0.8/tmpl/examples/example_resistor_test.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.7/tmpl/examples/resistor_example.py` & `test_measure_process_lib-1.0.8/tmpl/examples/resistor_example.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.7/tmpl/tmp_code_generator.py` & `test_measure_process_lib-1.0.8/tmpl/tmp_code_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 TestManager classes:
 <MANAGER_CLASSES>
 
 
 
 This module is based on the "Test, Measure, Process Library" (TMPL)
 framework for organising measurement code.
-See: https://github.com/redlegjed/test_measure_process_lib
+See: https://pypi.org/project/test-measure-process-lib/
 
 \"\"\"
 
 #================================================================
 \#%% Imports
 #================================================================
 # Standard library
@@ -233,28 +233,28 @@
     str
         text of class definition code
     """
     txt = copy.deepcopy(TEMPLATE_MANAGER)
     txt = txt.replace('<MANAGER_NAME>',name)
 
     # Make conditions lines
-    cond_txt = [f'        self.add_condition({c})' for c in conditions]
+    cond_txt = [f'        self.add_setup_condition({c})' for c in conditions]
     
     # Make conditions lines
     meas_txt = [f'        self.add_measurement({m})' for m in meas]
 
     txt = txt.replace('<CONDITION_DEFINITIONS>','\n'.join(cond_txt))
     txt = txt.replace('<MEASUREMENT_DEFINITIONS>','\n'.join(meas_txt))
 
     return txt
 
 
-def make_module(filename,conditions=['DefaultCondition'],
+def make_module(filename='',conditions=['DefaultCondition'],
                     meas=['DefaultMeasurement'],
-                    seq=['DefaultSeq'],return_text=False):
+                    seq=['DefaultSeq']):
     """
     Make a module file with auto-generated code for TMPL classes.
 
     Specifiy the names of the SetupConditions, Measurement and TestManager
     classes in the input arguments. A code template for each class will be
     added to the module file.
 
@@ -274,27 +274,30 @@
 
     Name of module file (full paths supported as well)
     >>> name = 'BigExperiment2.py'
 
     Generate module file
     >>> make_module(name,conditions=cond,meas=meas,seq=seq)
 
+    Return text string only
+    >>> make_module(conditions=cond,meas=meas,seq=seq)
+
+
     Parameters
     ----------
     filename : str
         full filename for module file to be created
+        If this is empty or not specified then the function returns a 
+        text string with the code documentation.
     conditions : list, optional
         List of names of SetupCondition classes, by default ['DefaultCondition']
     meas : list, optional
         List of names of Measurement classes, by default ['DefaultMeasurement']
     seq : list, optional
         List of names of TestManager classes, by default ['DefaultSeq']
-    return_text : bool, optional
-        If True then the text of the module is returned as a string
-        otherwise the text is save to a file, by default False
 
     Returns
     -------
     str or None
         text string if return_text is True otherwise None
     """
 
@@ -337,15 +340,15 @@
     rep_txt = [make_manager(s,conditions=conditions,meas=meas) for s in seq]
     txt = txt.replace('<MANAGER_TEXT>','\n'.join(rep_txt))
 
     # Have to escape the #%% because VSCode thinks it's a notebook
     # - undo this here
     txt = txt.replace(r'\#','#')
     
-    if return_text:
+    if filename=='':
         return txt
 
     file.write_text(txt)
 
 
 #================================================================
 #%% Classes
```

### Comparing `test_measure_process_lib-1.0.7/tmpl/tmpl_core.py` & `test_measure_process_lib-1.0.8/tmpl/tmpl_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
     @test_time
     def myfunction(self)
 
     It will time how long the function takes and display it.
     """                                                                                                   
                                                                                                                           
     def wrapper(self,*arg,**kwargs):                                                                                                      
+        """
+        Wrapper function
+        """
         t = time.time()            
         self.log('<'*40)
         self.log(f'Running {self.name}')
 
         res = func(self,*arg,**kwargs)  
 
         self.test_time_s = time.time()-t
```

### Comparing `test_measure_process_lib-1.0.7/tmpl/tmpl_storage.py` & `test_measure_process_lib-1.0.8/tmpl/tmpl_storage.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.7/tmpl/tmpl_support.py` & `test_measure_process_lib-1.0.8/tmpl/tmpl_support.py`

 * *Files identical despite different names*

