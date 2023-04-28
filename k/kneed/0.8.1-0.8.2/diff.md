# Comparing `tmp/kneed-0.8.1.tar.gz` & `tmp/kneed-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kneed-0.8.1.tar", last modified: Sat Jul 30 19:49:39 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `kneed-0.8.1.tar` & `kneed-0.8.2.tar`

### file list

```diff
@@ -1,23 +1,12 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-07-30 19:49:39.117945 kneed-0.8.1/
--rw-r--r--   0 kevin      (501) staff       (20)     1482 2019-07-21 10:20:30.000000 kneed-0.8.1/LICENSE
--rw-r--r--   0 kevin      (501) staff       (20)      110 2022-07-30 14:12:22.000000 kneed-0.8.1/MANIFEST.in
--rw-r--r--   0 kevin      (501) staff       (20)     5132 2022-07-30 19:49:39.118169 kneed-0.8.1/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     4560 2022-07-30 13:58:36.000000 kneed-0.8.1/README.md
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-07-30 19:49:39.110159 kneed-0.8.1/kneed/
--rw-r--r--   0 kevin      (501) staff       (20)        6 2022-07-30 19:49:19.000000 kneed-0.8.1/kneed/VERSION
--rw-r--r--   0 kevin      (501) staff       (20)      212 2022-07-30 19:36:04.000000 kneed-0.8.1/kneed/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     4571 2020-08-13 00:47:05.000000 kneed-0.8.1/kneed/data_generator.py
--rw-r--r--   0 kevin      (501) staff       (20)    16744 2022-07-30 13:53:15.000000 kneed-0.8.1/kneed/knee_locator.py
--rw-r--r--   0 kevin      (501) staff       (20)      579 2022-07-30 13:53:15.000000 kneed-0.8.1/kneed/shape_detector.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-07-30 19:49:39.115052 kneed-0.8.1/kneed.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)     5132 2022-07-30 19:49:39.000000 kneed-0.8.1/kneed.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)      347 2022-07-30 19:49:39.000000 kneed-0.8.1/kneed.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2022-07-30 19:49:39.000000 kneed-0.8.1/kneed.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)      114 2022-07-30 19:49:39.000000 kneed-0.8.1/kneed.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)        6 2022-07-30 19:49:39.000000 kneed-0.8.1/kneed.egg-info/top_level.txt
--rw-r--r--   0 kevin      (501) staff       (20)       89 2022-07-30 13:53:15.000000 kneed-0.8.1/pyproject.toml
--rw-r--r--   0 kevin      (501) staff       (20)       27 2022-07-30 13:53:15.000000 kneed-0.8.1/requirements.txt
--rw-r--r--   0 kevin      (501) staff       (20)      918 2022-07-30 19:49:39.119104 kneed-0.8.1/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)       70 2022-07-30 13:53:15.000000 kneed-0.8.1/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-07-30 19:49:39.116051 kneed-0.8.1/tests/
--rw-r--r--   0 kevin      (501) staff       (20)    15504 2022-07-30 13:53:15.000000 kneed-0.8.1/tests/test_sample.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kneed-0.8.2/kneed/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kneed-0.8.2/kneed/_version.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 kneed-0.8.2/kneed/data_generator.py
+-rw-r--r--   0        0        0    17683 2020-02-02 00:00:00.000000 kneed-0.8.2/kneed/knee_locator.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 kneed-0.8.2/kneed/shape_detector.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 kneed-0.8.2/tests/test_no_matplotlib.py
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 kneed-0.8.2/tests/test_sample.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 kneed-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 kneed-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 kneed-0.8.2/README.md
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 kneed-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 kneed-0.8.2/PKG-INFO
```

### Comparing `kneed-0.8.1/LICENSE` & `kneed-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kneed-0.8.1/PKG-INFO` & `kneed-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: kneed
-Version: 0.8.1
+Version: 0.8.2
 Summary: Knee-point detection in Python
-Home-page: https://github.com/arvkevi/kneed
-Author: Kevin Arvai
-Author-email: arvkevi@gmail.com
-Maintainer: Kevin Arvai
-License: BSD
-Keywords: knee-detection,system
+Project-URL: Homepage, https://github.com/arvkevi/kneed
+Project-URL: Documentation, https://kneed.readthedocs.io/en/latest/
+Author-email: Kevin Arvai <arvkevi@gmail.com>
+License-File: LICENSE
+Keywords: elbow-method,knee-detection,system
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.5
+Requires-Dist: numpy>=1.14.2
+Requires-Dist: scipy>=1.0.0
 Provides-Extra: plot
+Requires-Dist: matplotlib>=2.2.5; extra == 'plot'
 Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: matplotlib>=2.2.5; extra == 'testing'
+Requires-Dist: pytest-cov>=3.0.0; extra == 'testing'
+Requires-Dist: pytest>=5.0.1; extra == 'testing'
+Description-Content-Type: text/markdown
 
 # kneed
  Knee-point detection in Python
 
 [![Downloads](https://pepy.tech/badge/kneed)](https://pepy.tech/project/kneed) [![Downloads](https://pepy.tech/badge/kneed/week)](https://pepy.tech/project/kneed) ![Dependents](https://badgen.net/github/dependents-repo/arvkevi/kneed/?icon=github) [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/arvkevi/ikneed/main/ikneed.py) [![Build Status](https://travis-ci.com/arvkevi/kneed.svg?branch=master)](https://travis-ci.com/arvkevi/kneed) [![codecov](https://codecov.io/gh/arvkevi/kneed/branch/master/graph/badge.svg)](https://codecov.io/gh/arvkevi/kneed)[![DOI](https://zenodo.org/badge/113799037.svg)](https://zenodo.org/badge/latestdoi/113799037)
```

### Comparing `kneed-0.8.1/README.md` & `kneed-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `kneed-0.8.1/kneed/data_generator.py` & `kneed-0.8.2/kneed/data_generator.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.1/kneed/knee_locator.py` & `kneed-0.8.2/kneed/knee_locator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     _has_matplotlib = True
 
 class KneeLocator(object):
     """
     Once instantiated, this class attempts to find the point of maximum
     curvature on a line. The knee is accessible via the `.knee` attribute.
 
-    :param x: x values.
-    :type x: array-like
-    :param y: y values.
-    :type y: array-like
+    :param x: x values, must be the same length as y.
+    :type x: 1D array of shape (`number_of_y_values`,) or list
+    :param y: y values, must be the same length as x.
+    :type y: 1D array of shape (`number_of_y_values`,) or list
     :param S: Sensitivity, original paper suggests default of 1.0
     :type S: float
     :param curve: If 'concave', algorithm will detect knees. If 'convex', it
         will detect elbows.
     :type curve: str
     :param direction: one of {"increasing", "decreasing"}
     :type direction: str
@@ -309,29 +309,39 @@
 
         if self.all_knees == set():
             warnings.warn("No knee/elbow found")
             return None, None
 
         return knee, norm_knee
 
-    def plot_knee_normalized(self, figsize: Optional[Tuple[int, int]] = None):
+    def plot_knee_normalized(self, figsize: Optional[Tuple[int, int]] = None, title: str = "Normalized Knee Point", xlabel: Optional[str] = None, ylabel: Optional[str] = None):
         """Plot the normalized curve, the difference curve (x_difference, y_normalized) and the knee, if it exists.
 
         :param figsize: Optional[Tuple[int, int]
             The figure size of the plot. Example (12, 8)
+        :param title: str
+            Title of the visualization, defaults to "Normalized Knee Point"
+        :param xlabel: Optional[str]
+            X-axis label
+        :param ylabel: Optional[str]
+            y-axis label
         :return: NoReturn
         """
         if not _has_matplotlib:
             raise _matplotlib_not_found_err
 
         if figsize is None:
             figsize = (6, 6)
 
         plt.figure(figsize=figsize)
-        plt.title("Normalized Knee Point")
+        plt.title(title)
+        if xlabel:
+            plt.xlabel(xlabel)
+        if ylabel:
+            plt.ylabel(ylabel)
         plt.plot(self.x_normalized, self.y_normalized, "b", label="normalized curve")
         plt.plot(self.x_difference, self.y_difference, "r", label="difference curve")
         plt.xticks(
             np.arange(self.x_normalized.min(), self.x_normalized.max() + 0.1, 0.1)
         )
         plt.yticks(
             np.arange(self.y_difference.min(), self.y_normalized.max() + 0.1, 0.1)
@@ -342,30 +352,40 @@
             plt.ylim()[0],
             plt.ylim()[1],
             linestyles="--",
             label="knee/elbow",
         )
         plt.legend(loc="best")
 
-    def plot_knee(self, figsize: Optional[Tuple[int, int]] = None):
+    def plot_knee(self, figsize: Optional[Tuple[int, int]] = None, title: str = "Knee Point", xlabel: Optional[str] = None, ylabel: Optional[str] = None):
         """
         Plot the curve and the knee, if it exists
 
         :param figsize: Optional[Tuple[int, int]
             The figure size of the plot. Example (12, 8)
+        :param title: str
+            Title of the visualization, defaults to "Knee Point"
+        :param xlabel: Optional[str]
+            X-axis label
+        :param ylabel: Optional[str]
+            y-axis label
         :return: NoReturn
         """
         if not _has_matplotlib:
             raise _matplotlib_not_found_err
 
         if figsize is None:
             figsize = (6, 6)
 
         plt.figure(figsize=figsize)
-        plt.title("Knee Point")
+        plt.title(title)
+        if xlabel:
+            plt.xlabel(xlabel)
+        if ylabel:
+            plt.ylabel(ylabel)
         plt.plot(self.x, self.y, "b", label="data")
         plt.vlines(
             self.knee, plt.ylim()[0], plt.ylim()[1], linestyles="--", label="knee/elbow"
         )
         plt.legend(loc="best")
 
     # Niceties for users working with elbows rather than knees
```

### Comparing `kneed-0.8.1/kneed/shape_detector.py` & `kneed-0.8.2/kneed/shape_detector.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.1/tests/test_sample.py` & `kneed-0.8.2/tests/test_sample.py`

 * *Files identical despite different names*

