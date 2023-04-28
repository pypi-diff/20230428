# Comparing `tmp/best-sort-0.0.8.tar.gz` & `tmp/best-sort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best-sort-0.0.8.tar", last modified: Fri Apr 21 01:09:21 2023, max compression
+gzip compressed data, was "best-sort-0.0.9.tar", last modified: Thu Apr 27 16:54:13 2023, max compression
```

## Comparing `best-sort-0.0.8.tar` & `best-sort-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      130 2023-03-17 22:46:27.922581 best-sort-0.0.8/README.md
--rw-r--r--   0        0        0      825 2023-04-16 17:04:49.991064 best-sort-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-16 17:03:44.081356 best-sort-0.0.8/src/best_sort/__init__.py
--rw-r--r--   0        0        0      160 2023-04-21 01:09:21.516627 best-sort-0.0.8/src/best_sort/_version.py
--rw-r--r--   0        0        0       62 2023-04-09 18:27:39.497791 best-sort-0.0.8/src/best_sort/sort_algos/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.8/src/best_sort/sort_algos/bubble_sort.py
--rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.8/src/best_sort/sort_algos/insertion_sort.py
--rw-r--r--   0        0        0     1017 2023-04-06 00:41:43.248019 best-sort-0.0.8/src/best_sort/sort_algos/selection_sort.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 best-sort-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-04-26 20:41:04.860901 best-sort-0.0.9/README.md
+-rw-r--r--   0        0        0      922 2023-04-27 16:44:31.207587 best-sort-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      148 2023-04-25 00:44:44.166523 best-sort-0.0.9/src/best_sort/__init__.py
+-rw-r--r--   0        0        0      160 2023-04-27 16:54:13.144085 best-sort-0.0.9/src/best_sort/_version.py
+-rw-r--r--   0        0        0       62 2023-04-09 18:27:39.497791 best-sort-0.0.9/src/best_sort/sort_algos/__init__.py
+-rw-r--r--   0        0        0     1060 2023-03-23 02:30:20.768607 best-sort-0.0.9/src/best_sort/sort_algos/bubble_sort.py
+-rw-r--r--   0        0        0     1086 2023-03-31 02:22:50.498076 best-sort-0.0.9/src/best_sort/sort_algos/insertion_sort.py
+-rw-r--r--   0        0        0     1017 2023-04-06 00:41:43.248019 best-sort-0.0.9/src/best_sort/sort_algos/selection_sort.py
+-rw-r--r--   0        0        0       62 2023-04-21 01:15:29.606171 best-sort-0.0.9/src/best_sort/visual_aids/__init__.py
+-rw-r--r--   0        0        0      629 2023-04-27 16:43:17.924903 best-sort-0.0.9/src/best_sort/visual_aids/graph_comparison.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 best-sort-0.0.9/PKG-INFO
```

### Comparing `best-sort-0.0.8/pyproject.toml` & `best-sort-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -19,11 +19,15 @@
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 keywords = ["sorting algorithm", "sorting", "best algorithm"]
-
+dependencies = [
+  "matplotlib >= 3.7.1",
+  "data-science-types >= 0.2.23",
+  "numpy >= 1.24.3"
+]
 [project.urls]
 "Homepage" = "https://git.jharmison.com/JediJoey/best_sort"
 "Bug Tracker" = "https://git.jharmison.com/JediJoey/best_sort/issues"
```

### Comparing `best-sort-0.0.8/src/best_sort/sort_algos/bubble_sort.py` & `best-sort-0.0.9/src/best_sort/sort_algos/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.8/src/best_sort/sort_algos/insertion_sort.py` & `best-sort-0.0.9/src/best_sort/sort_algos/insertion_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.8/src/best_sort/sort_algos/selection_sort.py` & `best-sort-0.0.9/src/best_sort/sort_algos/selection_sort.py`

 * *Files identical despite different names*

### Comparing `best-sort-0.0.8/PKG-INFO` & `best-sort-0.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: best-sort
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to find the best sorting algorithm for given data.
 Keywords: sorting algorithm,sorting,best algorithm
 Author-email: Joey Wheeler <joewheeler2048@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Requires-Dist: matplotlib >= 3.7.1
+Requires-Dist: data-science-types >= 0.2.23
+Requires-Dist: numpy >= 1.24.3
 Project-URL: Bug Tracker, https://git.jharmison.com/JediJoey/best_sort/issues
 Project-URL: Homepage, https://git.jharmison.com/JediJoey/best_sort
 
 # best_sort
 
 A package to find the best sorting algorithm for given data.
```

