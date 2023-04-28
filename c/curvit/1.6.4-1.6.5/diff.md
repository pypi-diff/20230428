# Comparing `tmp/curvit-1.6.4.tar.gz` & `tmp/curvit-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.6.4.tar", last modified: Fri Apr 28 06:18:26 2023, max compression
+gzip compressed data, was "curvit-1.6.5.tar", last modified: Fri Apr 28 13:37:19 2023, max compression
```

## Comparing `curvit-1.6.4.tar` & `curvit-1.6.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.017010 curvit-1.6.4/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.4/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 06:18:26.017010 curvit-1.6.4/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.4/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.015010 curvit-1.6.4/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.4/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.4/curvit/check_curvit_variability_V.0.4.py
--rwxrwxr-x   0 prajwel   (1000) prajwel   (1000)    79824 2023-04-28 06:10:59.000000 curvit-1.6.4/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.4/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.4/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 06:18:26.016010 curvit-1.6.4/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-04-28 06:18:26.000000 curvit-1.6.4/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-28 06:18:26.017010 curvit-1.6.4/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-04-28 06:11:41.000000 curvit-1.6.4/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.231493 curvit-1.6.5/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.5/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 13:37:19.231493 curvit-1.6.5/PKG-INFO
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.5/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.230493 curvit-1.6.5/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      133 2023-03-19 15:24:32.000000 curvit-1.6.5/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.5/curvit/check_curvit_variability_V.0.4.py
+-rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    79693 2023-04-28 13:32:33.000000 curvit-1.6.5/curvit/curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      355 2021-06-25 20:52:41.000000 curvit-1.6.5/curvit/profile_curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1003 2022-12-10 20:44:29.000000 curvit-1.6.5/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-04-28 13:37:19.230493 curvit-1.6.5/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       63 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-04-28 13:37:19.000000 curvit-1.6.5/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-04-28 13:37:19.231493 curvit-1.6.5/setup.cfg
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      894 2023-04-28 13:32:52.000000 curvit-1.6.5/setup.py
```

### Comparing `curvit-1.6.4/LICENSE` & `curvit-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.6.4/PKG-INFO` & `curvit-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.4
+Version: 1.6.5
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.4 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.5 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.4/README.md` & `curvit-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `curvit-1.6.4/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.6.5/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.4/curvit/curvit.py` & `curvit-1.6.5/curvit/curvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -414,32 +414,79 @@
     elif aperture_correction == 'nuv':
         CPF = CPF / nuv_ratio_function(radius)
         CPF_err = CPF_err / nuv_ratio_function(radius)
     return CPF, CPF_err
     
     
 def apply_saturation_correction(CPF5, CPF5_err):
-            
+    
+    CPF_original = CPF5
+    CPF5_err_original = CPF5_err
+    
+    CPF5 = CPF5 * 0.97
+    CPF5_err = CPF5_err * 0.97    
+    
     if np.sum(CPF5 >= 0.6) != 0:
         print("\nCounts per frame exeeds 0.6; saturation correction cannot be applied")
         return
 
     ICPF5 = -1 * np.log(1 - CPF5)
     ICPF5_err = CPF5_err / CPF5
 
     ICORR = ICPF5 - CPF5
     ICORR_err = np.sqrt((ICPF5_err ** 2) + (CPF5_err ** 2))
 
     RCORR = ICORR * (0.89 - (0.30 * (ICORR ** 2)))
     RCORR_err = RCORR * np.sqrt((ICORR_err ** 2) + ((0.30 * 2 * ICORR * ICORR_err) ** 2))
 
-    CPF5 = CPF5 + RCORR
-    CPF5_err = np.sqrt((CPF5_err ** 2) + (RCORR_err ** 2))       
+    CPF5 = CPF_original + RCORR
+    CPF5_err = np.sqrt((CPF5_err_original ** 2) + (RCORR_err ** 2))       
     return CPF5, CPF5_err  
     
+def compute_CPF(mcounts, frames_in_bin, bg_CPS, bg_CPS_e,
+                weighted_mcounts, saturation_correction,
+                aperture_correction, radius,
+                framecount_per_sec):                      
+                      
+    if saturation_correction == True:
+        if aperture_correction is None:
+            raise ValueError("If saturation_correction parameter is True, "
+                             "then aperture_correction parameter should not be None!")
+
+        CPF = mcounts / frames_in_bin
+        CPF_err = np.sqrt(mcounts) / frames_in_bin
+
+        # Background subtraction.
+        CPF = CPF - (bg_CPS / framecount_per_sec)
+        CPF_err = np.sqrt(CPF_err ** 2 + (bg_CPS_e / framecount_per_sec) ** 2)   
+
+        CPF, CPF_err = apply_aperture_correction(CPF, 
+                                                 CPF_err, 
+                                                 radius, 
+                                                 aperture_correction)
+
+        CPF, CPF_err = apply_saturation_correction(CPF, CPF_err)
+        
+        # Applying flat-field correction.               
+        flat_field_array = weighted_mcounts / mcounts                      
+        CPF = CPF * flat_field_array
+    else:
+        CPF = weighted_mcounts / frames_in_bin
+        CPF_err = np.sqrt(mcounts) / frames_in_bin
+
+        # Background subtraction.
+        CPF = CPF - (bg_CPS / framecount_per_sec)
+        CPF_err = np.sqrt(CPF_err ** 2 + (bg_CPS_e / framecount_per_sec) ** 2)   
+
+        CPF, CPF_err = apply_aperture_correction(CPF, CPF_err, 
+                                                 radius, 
+                                                 aperture_correction)
+                      
+    return CPF, CPF_err
+    
     
 def makecurves(events_list = events_list,
                radius = radius,
                detection_method = detection_method,
                threshold = threshold,
                how_many = how_many,
                bwidth = bwidth,
@@ -714,33 +761,18 @@
             weighted_mcounts = weighted_counts[count_mask]
             mcounts = counts[count_mask]
             frames_in_bin = u_counts[count_mask]
         else:
             print('No counts for the source at %s' %uaxy)
             continue
 
-        CPF = weighted_mcounts / frames_in_bin
-        CPF_err = np.sqrt(mcounts) / frames_in_bin
-        
-        # Background subtraction.
-        CPF = CPF - (bg_CPS / framecount_per_sec)
-        CPF_err = np.sqrt(CPF_err ** 2 + (bg_CPS_e / framecount_per_sec) ** 2)   
-
-        if saturation_correction == True:
-            CPF, CPF_err = apply_aperture_correction(mcounts / frames_in_bin, 
-                                                     CPF_err, 
-                                                     radius, 
-                                                     aperture_correction)
-            flat_field_array = weighted_mcounts / mcounts
-            CPF, CPF_err = apply_saturation_correction(CPF, CPF_err)
-            CPF = CPF * flat_field_array
-        else:
-            CPF, CPF_err = apply_aperture_correction(CPF, CPF_err, 
-                                                     radius, 
-                                                     aperture_correction)
+        CPF, CPF_err = compute_CPF(mcounts, frames_in_bin, bg_CPS, bg_CPS_e,
+                                   weighted_mcounts, saturation_correction,
+                                   aperture_correction, radius,
+                                   framecount_per_sec)
         
         CPS = CPF * framecount_per_sec
         CPS_err = CPF_err * framecount_per_sec
 
         plt.scatter(mcentres, CPS)
         plt.errorbar(mcentres, CPS, yerr = CPS_err, linestyle = "None")
         empty_space = (till_here - time_start) / 25.0
@@ -1016,33 +1048,18 @@
         mcentres =  bin_centres[count_mask]
         weighted_mcounts = weighted_counts[count_mask]
         mcounts = counts[count_mask]
         frames_in_bin = u_counts[count_mask]
     else:
         print('No counts inside the aperture!')
 
-    CPF = weighted_mcounts / frames_in_bin
-    CPF_err = np.sqrt(mcounts) / frames_in_bin
-    
-    # Background subtraction.
-    CPF = CPF - (bg_CPS / framecount_per_sec)
-    CPF_err = np.sqrt(CPF_err ** 2 + (bg_CPS_e / framecount_per_sec) ** 2)    
-
-    if saturation_correction == True:
-        CPF, CPF_err = apply_aperture_correction(mcounts / frames_in_bin, 
-                                                 CPF_err, 
-                                                 radius, 
-                                                 aperture_correction)
-        flat_field_array = weighted_mcounts / mcounts
-        CPF, CPF_err = apply_saturation_correction(CPF, CPF_err)
-        CPF = CPF * flat_field_array
-    else:
-        CPF, CPF_err = apply_aperture_correction(CPF, CPF_err, 
-                                                 radius, 
-                                                 aperture_correction)
+    CPF, CPF_err = compute_CPF(mcounts, frames_in_bin, bg_CPS, bg_CPS_e,
+                               weighted_mcounts, saturation_correction,
+                               aperture_correction, radius,
+                               framecount_per_sec)
     
     CPS = CPF * framecount_per_sec
     CPS_err = CPF_err * framecount_per_sec
 
     # Let us get on with the plot. 
     plt.scatter(mcentres, CPS)
     plt.errorbar(mcentres, CPS, yerr = CPS_err, linestyle = "None")
@@ -1331,35 +1348,20 @@
 
     if np.sum(count_mask) != 0:
         mcentres =  bin_centres[count_mask]
         weighted_mcounts = weighted_counts[count_mask]
         mcounts = counts[count_mask]
         frames_in_bin = u_counts[count_mask]
     else:
-        print('No counts inside the aperture!')
+        print('No counts inside the aperture!') 
 
-    CPF = weighted_mcounts / frames_in_bin
-    CPF_err = np.sqrt(mcounts) / frames_in_bin
-    
-    # Background subtraction.
-    CPF = CPF - (bg_CPS / framecount_per_sec)
-    CPF_err = np.sqrt(CPF_err ** 2 + (bg_CPS_e / framecount_per_sec) ** 2)    
-
-    if saturation_correction == True:
-        CPF, CPF_err = apply_aperture_correction(mcounts / frames_in_bin, 
-                                                 CPF_err, 
-                                                 radius, 
-                                                 aperture_correction)
-        flat_field_array = weighted_mcounts / mcounts
-        CPF, CPF_err = apply_saturation_correction(CPF, CPF_err)
-        CPF = CPF * flat_field_array
-    else:
-        CPF, CPF_err = apply_aperture_correction(CPF, CPF_err, 
-                                                 radius, 
-                                                 aperture_correction)
+    CPF, CPF_err = compute_CPF(mcounts, frames_in_bin, bg_CPS, bg_CPS_e,
+                               weighted_mcounts, saturation_correction,
+                               aperture_correction, radius,
+                               framecount_per_sec)
     
     CPS = CPF * framecount_per_sec
     CPS_err = CPF_err * framecount_per_sec
 
     # Let us get on with the plot. 
     plt.scatter(mcentres, CPS)
     plt.errorbar(mcentres, CPS, yerr = CPS_err, linestyle = "None")
```

### Comparing `curvit-1.6.4/curvit/test_curvit.py` & `curvit-1.6.5/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.4/curvit.egg-info/PKG-INFO` & `curvit-1.6.5/curvit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.4
+Version: 1.6.5
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.4 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.5 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.4/setup.py` & `curvit-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit", 
-    version="1.6.4",
+    version="1.6.5",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```

