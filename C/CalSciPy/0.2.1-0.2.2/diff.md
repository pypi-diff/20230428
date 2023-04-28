# Comparing `tmp/CalSciPy-0.2.1.tar.gz` & `tmp/CalSciPy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.1.tar", last modified: Wed Apr 26 15:22:00 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.2.tar", last modified: Fri Apr 28 15:08:19 2023, max compression
```

## Comparing `CalSciPy-0.2.1.tar` & `CalSciPy-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:22:00.030279 CalSciPy-0.2.1/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4998 2023-04-26 15:22:00.029279 CalSciPy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.1/README.md
--rw-rw-rw-   0        0        0     2330 2023-04-26 15:21:16.000000 CalSciPy-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 15:22:00.030279 CalSciPy-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.929318 CalSciPy-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.968279 CalSciPy-0.2.1/src/CalSciPy/
--rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.1/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.1/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     2115 2023-04-26 15:19:07.000000 CalSciPy-0.2.1/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.1/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     5129 2023-04-05 15:54:33.000000 CalSciPy-0.2.1/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.1/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.1/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.1/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:21:59.987278 CalSciPy-0.2.1/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      365 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-26 15:21:59.000000 CalSciPy-0.2.1/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:22:00.025280 CalSciPy-0.2.1/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.1/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.1/tests/test_bruker.py
--rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.1/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.1/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.1/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.1/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.1/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.1/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.358989 CalSciPy-0.2.2/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4998 2023-04-28 15:08:19.357988 CalSciPy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.2/README.md
+-rw-rw-rw-   0        0        0     2330 2023-04-28 15:07:52.000000 CalSciPy-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:08:19.358989 CalSciPy-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.311988 CalSciPy-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.332989 CalSciPy-0.2.2/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.2/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.2/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     2388 2023-04-28 15:05:04.000000 CalSciPy-0.2.2/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.2/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     6019 2023-04-28 15:07:33.000000 CalSciPy-0.2.2/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.2/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.2/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.2/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.340989 CalSciPy-0.2.2/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      365 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 15:08:19.000000 CalSciPy-0.2.2/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:08:19.355989 CalSciPy-0.2.2/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.2/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.2/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.2/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.2/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.2/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.2/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.2/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.2/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.1/LICENSE` & `CalSciPy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/PKG-INFO` & `CalSciPy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.1/README.md` & `CalSciPy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/pyproject.toml` & `CalSciPy-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.1"
+version = "0.2.2"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
```

### Comparing `CalSciPy-0.2.1/src/CalSciPy/bruker.py` & `CalSciPy-0.2.2/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy/coloring.py` & `CalSciPy-0.2.2/src/CalSciPy/coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy/event_processing.py` & `CalSciPy-0.2.2/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy/image_processing.py` & `CalSciPy-0.2.2/src/CalSciPy/image_processing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from .misc import generate_blocks
+from .misc import generate_blocks, wrap_cupy_block
 
 try:
     import cupy
     import cupyx.scipy.ndimage
 except ModuleNotFoundError:
     pass
 
@@ -37,23 +37,35 @@
     """
 
     if in_place:
         filtered_images = images
     else:
         filtered_images = images.copy()
 
-    filtered_images = cupy.asarray(filtered_images)
-
     frames = filtered_images.shape[0]
 
     if block_size:
         block_gen = generate_blocks(range(frames), block_size, block_buffer)
         try:
             for block in block_gen:
-                filtered_images[block, :, :] = cupyx.scipy.ndimage.median_filter(filtered_images[block, :, :],
-                                                                                 footprint=mask)
+                filtered_images[block, :, :] = _median_filter(filtered_images[block, :, :], footprint=mask)
         except (RuntimeError, StopIteration):
             pass
     else:
-        filtered_images = cupyx.scipy.ndimage.median_filter(filtered_images, footprint=mask)
+        filtered_images = _median_filter(filtered_images, footprint=mask)
+
+    return filtered_images
 
-    return filtered_images.get()
+
+@wrap_cupy_block
+def _median_filter(images: cupy.ndarray, mask: np.ndarray) -> np.ndarray:
+    """
+    Implementation function of median filter
+
+    :param images: images to be filtered
+    :type images: cupy.ndarray
+    :param mask: mask for filtering
+    :type mask: numpy.ndarray
+    :return: filtered numpy array
+    :rtype: numpy.ndarray
+    """
+    return cupyx.scipy.ndimage.median_filter(images, footprint=mask)
```

### Comparing `CalSciPy-0.2.1/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.2/src/CalSciPy/io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy/misc.py` & `CalSciPy-0.2.2/src/CalSciPy/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from __future__ import annotations
-from typing import Iterable, Iterator, Any
+from typing import Iterable, Iterator, Any, Callable
 from collections import deque
-import numpy as np
 from pathlib import Path
+from numbers import Number
+from functools import wraps
+
+import numpy as np
+
+try:
+    import cupy
+except ModuleNotFoundError:
+    pass
 
 
-def calculate_frames_per_file(y_pixels: int, x_pixels: int, bit_depth: np.dtype = np.uint16, size_cap: float = 3.9) \
+def calculate_frames_per_file(y_pixels: int, x_pixels: int, bit_depth: np.dtype = np.uint16, size_cap: Number = 3.9) \
         -> int:
     """
     Estimates the number of image frames to allocate to each file given some maximum size.
 
     :param y_pixels: number of y_pixels in image
     :type y_pixels: int
     :param x_pixels: number of x_pixels in image
@@ -99,14 +107,33 @@
 
     while len(index) < digits:
         index = "".join(["0", index])
 
     return output_folder.joinpath("".join([base, "_", index, ext]))
 
 
+def wrap_cupy_block(cupy_function: Callable) -> Callable:
+    """
+    Wraps a cupy function such that incoming numpy arrays are converting to cupy arrays and swapped back on return
+
+    :param cupy_function: any cupy function that accepts numpy arrays
+    :type cupy_function: Callable
+    :return: wrapped function
+    :rtype: Callable
+    """
+    @wraps(cupy_function)
+    def decorator(*args, **kwargs) -> Callable:
+        for arg in args:
+            if isinstance(arg, np.ndarray):
+                arg = cupy.asarray(arg, dtype=arg.dtype)  # Not here that I am not ensuring matched to the arrays
+                # memory order. I simply am not sure how...
+        return cupy_function(*args, **kwargs).get()
+    return decorator
+
+
 class PatternMatching:
     def __init__(self, value: Any, comparison_expressions: Iterable[Any]):
         """
         Manual implementation of pattern matching for python < 3.10
 
         Not the most extensible or robust right now, but she works well for the
         current implementations.
```

### Comparing `CalSciPy-0.2.1/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.2/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy/trace_processing.py` & `CalSciPy-0.2.2/src/CalSciPy/trace_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.2/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.1/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.2/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_a_install.py` & `CalSciPy-0.2.2/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_bruker.py` & `CalSciPy-0.2.2/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_coloring.py` & `CalSciPy-0.2.2/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_event_processing.py` & `CalSciPy-0.2.2/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_io_tools.py` & `CalSciPy-0.2.2/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_misc.py` & `CalSciPy-0.2.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_reorganization.py` & `CalSciPy-0.2.2/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.1/tests/test_trace_processing.py` & `CalSciPy-0.2.2/tests/test_trace_processing.py`

 * *Files identical despite different names*

