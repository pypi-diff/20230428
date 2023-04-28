# Comparing `tmp/DecisionTreeClassifier-0.0.6.tar.gz` & `tmp/DecisionTreeClassifier-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DecisionTreeClassifier-0.0.6.tar", last modified: Tue Apr 25 04:50:02 2023, max compression
+gzip compressed data, was "DecisionTreeClassifier-0.0.7.tar", last modified: Fri Apr 28 03:55:52 2023, max compression
```

## Comparing `DecisionTreeClassifier-0.0.6.tar` & `DecisionTreeClassifier-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 04:50:02.248850 DecisionTreeClassifier-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-04-25 04:50:02.239848 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/
-drwxrwxrwx   0        0        0        0 2023-04-25 04:50:02.246850 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/
--rw-rw-rw-   0        0        0      676 2023-04-25 04:50:02.000000 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-25 04:50:02.000000 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 04:50:02.000000 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 04:50:02.000000 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 04:50:02.000000 DecisionTreeClassifier-0.0.6/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-04-21 04:53:44.000000 DecisionTreeClassifier-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0      676 2023-04-25 04:50:02.247850 DecisionTreeClassifier-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-25 04:50:02.248850 DecisionTreeClassifier-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-04-25 04:49:34.000000 DecisionTreeClassifier-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.732710 DecisionTreeClassifier-0.0.7/
+-rw-rw-rw-   0        0        0     1075 2023-04-21 04:53:44.000000 DecisionTreeClassifier-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0     2803 2023-04-28 03:55:52.732710 DecisionTreeClassifier-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-04-28 03:52:27.000000 DecisionTreeClassifier-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.718707 DecisionTreeClassifier-0.0.7/app/
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.722708 DecisionTreeClassifier-0.0.7/app/DecisionTree/
+-rw-rw-rw-   0        0        0       31 2023-04-26 00:14:29.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.728709 DecisionTreeClassifier-0.0.7/app/DecisionTree/src/
+-rw-rw-rw-   0        0        0    25310 2023-04-21 05:19:20.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/src/DecisionTree.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 00:14:08.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/src/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-03-09 20:00:16.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/src/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.731710 DecisionTreeClassifier-0.0.7/app/DecisionTree/test/
+-rw-rw-rw-   0        0        0     2654 2023-04-26 00:13:29.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/test/Full_test.py
+-rw-rw-rw-   0        0        0     7635 2023-04-26 00:13:27.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/test/Testing.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 00:11:45.000000 DecisionTreeClassifier-0.0.7/app/DecisionTree/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 03:55:52.726709 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/
+-rw-rw-rw-   0        0        0     2803 2023-04-28 03:55:52.000000 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-28 03:55:52.000000 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 03:55:52.000000 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 03:55:52.000000 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 03:55:52.000000 DecisionTreeClassifier-0.0.7/app/DecisionTreeClassifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 03:55:52.733710 DecisionTreeClassifier-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-04-28 03:55:47.000000 DecisionTreeClassifier-0.0.7/setup.py
```

### Comparing `DecisionTreeClassifier-0.0.6/LICENCE.txt` & `DecisionTreeClassifier-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

