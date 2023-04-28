# Comparing `tmp/unravel-python-1.2.3.tar.gz` & `tmp/unravel-python-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.3.tar", last modified: Mon Apr 24 14:12:09 2023, max compression
+gzip compressed data, was "unravel-python-1.2.4.tar", last modified: Fri Apr 28 13:03:44 2023, max compression
```

## Comparing `unravel-python-1.2.3.tar` & `unravel-python-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-04-24 14:12:10.000000 unravel-python-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 14:12:10.000000 unravel-python-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/unravel/
--rw-rw-rw-   0        0        0      358 2023-04-24 14:11:56.000000 unravel-python-1.2.3/unravel/__init__.py
--rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.3/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.3/unravel/example.py
--rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.3/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.3/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 13:03:44.300000 unravel-python-1.2.4/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-04-28 13:03:46.000000 unravel-python-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 13:03:46.000000 unravel-python-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:03:44.320000 unravel-python-1.2.4/unravel/
+-rw-rw-rw-   0        0        0      358 2023-04-28 13:03:34.000000 unravel-python-1.2.4/unravel/__init__.py
+-rw-rw-rw-   0        0        0    48764 2023-04-28 13:02:26.000000 unravel-python-1.2.4/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.4/unravel/example.py
+-rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.4/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.4/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-04-28 13:03:44.320000 unravel-python-1.2.4/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-04-28 13:03:46.000000 unravel-python-1.2.4/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-28 13:03:46.000000 unravel-python-1.2.4/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 13:03:46.000000 unravel-python-1.2.4/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-28 13:03:46.000000 unravel-python-1.2.4/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 13:03:46.000000 unravel-python-1.2.4/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.3/LICENSE` & `unravel-python-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.3/PKG-INFO` & `unravel-python-1.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UNRAVEL - UtiliziNg tRActography to uncoVEr muLti-fixel microstructure
 
@@ -18,15 +19,15 @@
   <img src="https://user-images.githubusercontent.com/70629561/224088594-7bcbded3-9f68-4389-955b-6141569b3c06.png" width="600" />
 </p>
 
 Welcome to the UNRAVEL's Github repository!
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/unravel-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
 The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
```

### Comparing `unravel-python-1.2.3/README.md` & `unravel-python-1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <img src="https://user-images.githubusercontent.com/70629561/224088594-7bcbded3-9f68-4389-955b-6141569b3c06.png" width="600" />
 </p>
 
 Welcome to the UNRAVEL's Github repository!
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/unravel-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
 The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
```

### Comparing `unravel-python-1.2.3/setup.py` & `unravel-python-1.2.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,13 +25,15 @@
     author_email='nicolas.delinte@uclouvain.be',
     license='GNU General Public License v3.0',
     packages=['unravel'],
     install_requires=['dipy',
                       'nibabel',
                       'numpy',
                       'scipy',
+                      'tqdm',
                       ],
 
-    classifiers=['Development Status :: 3 - Alpha',
+    classifiers=['Development Status :: 4 - Beta',
+                 'Intended Audience :: Science/Research',
                  'Natural Language :: English',
                  'Programming Language :: Python'],
 )
```

### Comparing `unravel-python-1.2.3/unravel/core.py` & `unravel-python-1.2.4/unravel/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 Created on Fri Mar 11 11:05:25 2022
 
 @author: DELINTE  Nicolas
 
 """
 
 import os
+import math
 import warnings
 import numpy as np
 import nibabel as nib
+from tqdm import tqdm
 from dipy.io.streamline import load_tractogram
 
 
 def deltas_to_D(dx: float, dy: float, dz: float, lamb=np.diag([1, 0, 0]),
                 vec_len: float = 500):
     '''
     Function creating a diffusion tensor from three orthogonal components.
@@ -112,16 +114,17 @@
     if voxDis == 0:  # Trying to gain time
         voxList[tuple(np.floor(position1))] = 1
 
         return voxList
 
     subseg = np.linspace(position1, position2, subparts)
 
-    for i in subseg:
-        xyz = tuple(np.floor(i))
+    voxels = np.floor(subseg)
+    for i in voxels:
+        xyz = tuple(i)
         if xyz not in voxList:
             voxList[xyz] = 1/subparts
         else:
             voxList[xyz] += (1/subparts)
 
     return voxList
 
@@ -271,21 +274,22 @@
 
     v1n = v1/np.linalg.norm(v1)
     v2n = v2/np.linalg.norm(v2)
 
     if (v1n == v2n).all():
         return 0
 
-    if sum(v1n*v2n) > 1:
-        return 0
-
-    if sum(v1n*v2n) < -1:
-        return 180
+    dot = np.dot(v1n, v2n)
 
-    ang = np.arccos(sum(v1n*v2n))*180/np.pi
+    if dot > 1:
+        ang = 0
+    if dot < -1:
+        ang = 180
+    else:
+        ang = math.acos(dot)*180/math.pi
 
     if ang > 90 and not direction:
         ang = 180-ang
 
     return ang
 
 
@@ -306,18 +310,20 @@
     Returns
     -------
     ang_coef : list
         List of the k coefficients
 
     '''
 
-    if len(vList) == 1:
+    K = len(vList)
+
+    if K == 1:
         return [1]
 
-    if len(vList)-sum(nList) <= 1:
+    if K-sum(nList) <= 1:
         return [1-i for i in list(map(int, nList))]
 
     angle_diffList = []
 
     for i, v in enumerate(vList):
         if nList[i]:
             angle_diffList.append(0)
@@ -329,15 +335,15 @@
     ang_coef = []
 
     for i, angle_diff in enumerate(angle_diffList):
         if nList[i]:
             ang_coef.append(0)
         else:
             coef = 1-angle_diff/sum_diff
-            coef = coef/(len(vList)-1-sum(nList))
+            coef = coef/(K-1-sum(nList))
             ang_coef.append(coef)
 
     return ang_coef
 
 
 def closest_fixel_only(vs, vList: list, nList: list):
     '''
@@ -356,18 +362,20 @@
     Returns
     -------
     ang_coef : list
         List of the k coefficients
 
     '''
 
-    if len(vList) == 1:
+    K = len(vList)
+
+    if K == 1:
         return [1]
 
-    if len(vList)-sum(nList) <= 1:
+    if K-sum(nList) <= 1:
         return [1-i for i in list(map(int, nList))]
 
     angle_diffList = []
 
     for k, v in enumerate(vList):
         if nList[k]:
             angle_diffList.append(1000)
@@ -408,18 +416,20 @@
     Returns
     -------
     ang_coef : list
         List of the k coefficients
 
     '''
 
-    if len(vList) == 1:
+    K = len(vList)
+
+    if K == 1:
         return [1]
 
-    if len(vList)-sum(nList) <= 1:
+    if K-sum(nList) <= 1:
         return [1-i for i in list(map(int, nList))]
 
     ang_coef = []
 
     for k, v in enumerate(vList):
         if nList[k]:
             ang_coef.append(0)
@@ -459,15 +469,15 @@
     Returns
     -------
     t : 5-D array
         Tensor array of shape (x,y,z,1,6).
 
     '''
 
-    t = np.zeros(peaks.shape[:3]+(1, 6))
+    t = np.zeros(peaks.shape[:3]+(1, 6), dtype='float32')
 
     scaleFactor = 1000 / min(pixdim)
 
     for xyz in np.ndindex(peaks.shape[:3]):
 
         if peaks[xyz].all() == 0:
             continue
@@ -693,15 +703,16 @@
 
             fList.append(fk)
 
     return get_fixel_weight(trk, tList, method, streamList, fList)
 
 
 def get_fixel_weight(trk, tList: list, method: str = 'ang',
-                     streamList: list = [], fList: list = []):
+                     streamList: list = [], fList: list = [],
+                     return_phi: bool = False, speed_up: bool = False):
     '''
     Get the fixel weights from a tract specified in trk_file.
 
     Parameters
     ----------
     trk : tractogram
         Content of a .trk file
@@ -715,14 +726,21 @@
         The default is 'ang'.
     streamList : list, optional
         Plots every streamline corresponding to the number (int) in the list.
         The default is [].
     fList : list, optional
         List of 3D arrays (x,y,z) containing the fraction of each fiber
         population. Only used with 'vol' method. The default is [].
+    return_phi : bool, optional
+        If True, returns the phi_maps used for the angular agreement. Currently
+        slows down the code. The default is False.
+    speed_up : bool, optional
+        If True, divides streamline segments into a fixed number of subsegments
+        instead of comptuing exact voxel border crossings. Decreases computation
+        time. The default is False.
 
     Returns
     -------
     fixelWeights : 4-D array of shape (x,y,z,K)
         Array containing the relative weights of the K fixels in each voxel.
     phi_maps : dict
         Dictionnary containing the lists of the relative contribution and
@@ -739,34 +757,36 @@
     '''
 
     assert method in ['ang', 'cfo', 'vol'], ("Unknown method : "+method)
 
     phi_maps = {}
     K = len(tList)
     # t10=np.zeros(tList[0].shape)
-    fixelWeights = np.zeros(tList[0].shape[0:3]+(K,))
+    fixelWeights = np.zeros(tList[0].shape[0:3]+(K,), dtype='float32')
 
     sList = tract_to_streamlines(trk)
 
     outputVoxelStream = []
     outputSegmentStream = []
 
-    for h, streamline in enumerate(sList):
+    for h, streamline in enumerate(tqdm(sList, desc='Following streamlines')):
 
         voxelStream = {}
         segmentStream = []
 
         previous_point = streamline[0, :]
 
         for i in range(1, streamline.shape[0]):
 
             point = streamline[i, :]
 
-            # voxList=voxels_from_segment(point,previous_point)
-            voxList = compute_subsegments(previous_point, point)
+            if speed_up:
+                voxList = voxels_from_segment(previous_point, point)
+            else:
+                voxList = compute_subsegments(previous_point, point)
 
             vs = (point-previous_point)   # Tract deltas
 
             for x, y, z in voxList:
 
                 x, y, z = (int(x), int(y), int(z))
 
@@ -786,46 +806,47 @@
                     if fList[k][x, y, z] == 0:
                         nList[k] = True
 
                 if all(nList):       # If no tensor in voxel
                     # t10[x,y,z,:]=np.zeros(3)
                     continue
 
-                if (x, y, z) not in phi_maps:       # Never been to this voxel
-                    phi_maps[(x, y, z)] = [[], []]
-
-                # !!! Computed twice (also in angular_weighting/cfo)
-                aList = []    # angle list
-                for k, v in enumerate(vList):
-                    if nList[k]:
-                        aList.append(1000)
-                    else:
-                        aList.append(angle_difference(vs, v))
-
-                min_k = np.argmin(aList)
-                phi_maps[(x, y, z)][0].append(aList[min_k])
-
                 if method == 'cfo':     # Closest-fixel-only
                     coefList = closest_fixel_only(vs, vList, nList)
                 elif method == 'vol':   # Relative volume fraction
-                    if len(vList) != len(fList):
+                    if K != len(fList):
                         warnings.warn("Warning : The number of fixels ("
-                                      + str(len(vList))
+                                      + str(K)
                                       + ") does not correspond to the number "
                                       + " of fractions given ("+str(len(fList))
                                       + ").")
                     coefList = fraction_weighting(
                         (x, y, z), vList, nList, fList)
                 else:   # Angular weighting
                     coefList = angular_weighting(vs, vList, nList)
 
                 for k, coef in enumerate(coefList):
                     fixelWeights[x, y, z, k] += voxList[(x, y, z)]*coef
-                phi_maps[(x, y, z)][1].append(
-                    voxList[(x, y, z)]*coefList[min_k])
+
+                if return_phi:
+                    if (x, y, z) not in phi_maps:     # Never been to this voxel
+                        phi_maps[(x, y, z)] = [[], []]
+
+                    # !!! Computed twice (also in angular_weighting/cfo)
+                    aList = []    # angle list
+                    for k, v in enumerate(vList):
+                        if nList[k]:
+                            aList.append(1000)
+                        else:
+                            aList.append(angle_difference(vs, v))
+
+                    min_k = np.argmin(aList)
+                    phi_maps[(x, y, z)][0].append(aList[min_k])
+                    phi_maps[(x, y, z)][1].append(voxList[(x, y, z)]
+                                                  * coefList[min_k])
 
                 if h in streamList:
 
                     s = []
                     for coef in coefList:
                         s.append(voxList[(x, y, z)]*coef)
                     segmentStream.append([(x, y, z)]+s)
@@ -870,15 +891,15 @@
     Returns
     -------
     mainFixelMap : 3-D array of shape (x,y,z).
         The array contains int values representing the most aligned fixel.
 
     '''
 
-    mainFixelMap = np.zeros(fixelWeights.shape[0:3])
+    mainFixelMap = np.zeros(fixelWeights.shape[0:3], dtype='float32')
     mainFixelMap[fixelWeights[:, :, :, 0] > fixelWeights[:, :, :, 1]] = 1
     mainFixelMap[fixelWeights[:, :, :, 0] < fixelWeights[:, :, :, 1]] = 2
 
     return mainFixelMap
 
 
 def tract_to_streamlines(trk) -> list:
@@ -985,22 +1006,14 @@
                 if len(fList) > 0:    # If fractions available and ==0
                     if fList[k][x, y, z] == 0:
                         nList[k] = True
 
             if all(nList):       # If no tensor in voxel
                 continue
 
-            # !!! Computed twice (also in angular_weighting/cfo)
-            aList = []    # angle list
-            for k, v in enumerate(vList):
-                if nList[k]:
-                    aList.append(1000)
-                else:
-                    aList.append(angle_difference(vs, v))
-
             for j, method in enumerate(method_list):
 
                 if method == 'cfo':     # Closest-fixel-only
                     coefList = closest_fixel_only(vs, vList, nList)
                 elif method == 'vol':   # Relative volume fraction
                     if len(vList) != len(fList):
                         warnings.warn("Warning : The number of fixels ("
@@ -1355,17 +1368,17 @@
     phi : float
         Angular agreement index.
     phi_map : 3-D array of shape (x,y,z)
         Voxel-wise angular agreement index.
 
     '''
 
-    phi_sum = np.zeros(volume_shape[:3])
-    phi_map = np.zeros(volume_shape[:3])
-    w = np.zeros(volume_shape[:3])
+    phi_sum = np.zeros(volume_shape[:3], dtype='float32')
+    phi_map = np.zeros(volume_shape[:3], dtype='float32')
+    w = np.zeros(volume_shape[:3], dtype='float32')
 
     for (x, y, z) in phi_maps:
         lista = np.array(phi_maps[(x, y, z)][0]) * \
             np.array(phi_maps[(x, y, z)][1])
         phi_sum[x, y, z] = round(np.sum(lista), 3)
         w[x, y, z] = sum(phi_maps[(x, y, z)][1])
 
@@ -1409,15 +1422,15 @@
     Returns
     -------
     microMap : 3-D array of shape (x,y,z)
         Array containing the microstructure map
 
     '''
 
-    microMap = np.zeros(metricMapList[0].shape)
+    microMap = np.zeros(metricMapList[0].shape, dtype='float32')
     total_weight = np.sum(fixelWeights, axis=len(fixelWeights.shape)-1)
 
     for k, metricMap in enumerate(metricMapList):
         slic = tuple([slice(None)]*(len(fixelWeights.shape)-1))+(k,)
         microMap += metricMap*fixelWeights[slic]
 
     microMap[total_weight != 0] /= total_weight[total_weight != 0]
@@ -1449,15 +1462,15 @@
         Weighted sum.
 
     '''
 
     tsl = total_segment_length(fixel_weights)
 
     if weighting == 'roi':
-        weighted_map = np.zeros(tsl.shape)
+        weighted_map = np.zeros(tsl.shape, dtype='float32')
         weighted_map[tsl != 0] = 1
     else:
         weighted_map = tsl
 
     if np.sum(weighted_map) == 0:
         return 0, 0
 
@@ -1494,22 +1507,22 @@
         Total length map.
     M : int
         Number of non-zero pixels in both metric maps.
 
     '''
 
     K = len(metricMapList)
-    fixelWeightSum = np.zeros(fixelWeightList[0].shape)
+    fixelWeightSum = np.zeros(fixelWeightList[0].shape, dtype='float32')
     M = 0
 
     for fixelWeight in fixelWeightList:
         fixelWeightSum += fixelWeight
         M += np.count_nonzero(fixelWeight)
 
-    weightedMetricSum = np.zeros(metricMapList[0].shape)
+    weightedMetricSum = np.zeros(metricMapList[0].shape, dtype='float32')
 
     for k in range(K):
         weightedMetricSum += metricMapList[k]*fixelWeightList[k]
 
     return weightedMetricSum, fixelWeightSum, M
```

### Comparing `unravel-python-1.2.3/unravel/example.py` & `unravel-python-1.2.4/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.3/unravel/utils.py` & `unravel-python-1.2.4/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.3/unravel/viz.py` & `unravel-python-1.2.4/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.3/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.4/unravel_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.3
+Version: 1.2.4
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UNRAVEL - UtiliziNg tRActography to uncoVEr muLti-fixel microstructure
 
@@ -18,15 +19,15 @@
   <img src="https://user-images.githubusercontent.com/70629561/224088594-7bcbded3-9f68-4389-955b-6141569b3c06.png" width="600" />
 </p>
 
 Welcome to the UNRAVEL's Github repository!
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/unravel-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
 The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
```

