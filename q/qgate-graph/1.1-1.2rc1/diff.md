# Comparing `tmp/qgate_graph-1.1.tar.gz` & `tmp/qgate_graph-1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgate_graph-1.1.tar", last modified: Thu Apr 27 20:48:39 2023, max compression
+gzip compressed data, was "qgate_graph-1.2rc1.tar", last modified: Fri Apr 28 10:23:24 2023, max compression
```

## Comparing `qgate_graph-1.1.tar` & `qgate_graph-1.2rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 20:48:39.387559 qgate_graph-1.1/
--rw-rw-rw-   0        0        0      389 2023-04-27 20:48:39.387559 qgate_graph-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 20:48:39.342517 qgate_graph-1.1/qgate_graph/
--rw-rw-rw-   0        0        0        6 2023-04-27 20:17:36.000000 qgate_graph-1.1/qgate_graph/__init__.py
--rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.1/qgate_graph/constant.py
--rw-rw-rw-   0        0        0     7638 2023-04-27 20:17:36.000000 qgate_graph-1.1/qgate_graph/graph.py
-drwxrwxrwx   0        0        0        0 2023-04-27 20:48:39.387559 qgate_graph-1.1/qgate_graph.egg-info/
--rw-rw-rw-   0        0        0      389 2023-04-27 20:48:39.000000 qgate_graph-1.1/qgate_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-27 20:48:39.000000 qgate_graph-1.1/qgate_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 20:48:39.000000 qgate_graph-1.1/qgate_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-27 20:48:39.000000 qgate_graph-1.1/qgate_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 20:48:39.000000 qgate_graph-1.1/qgate_graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 20:48:39.403995 qgate_graph-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-04-27 20:46:12.000000 qgate_graph-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.778486 qgate_graph-1.2rc1/
+-rw-rw-rw-   0        0        0      392 2023-04-28 10:23:24.762730 qgate_graph-1.2rc1/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.731442 qgate_graph-1.2rc1/qgate_graph/
+-rw-rw-rw-   0        0        0        6 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/qgate_graph/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-04-27 20:17:36.000000 qgate_graph-1.2rc1/qgate_graph/constant.py
+-rw-rw-rw-   0        0        0     8131 2023-04-28 10:12:15.000000 qgate_graph-1.2rc1/qgate_graph/graph.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:23:24.762730 qgate_graph-1.2rc1/qgate_graph.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-28 10:23:24.000000 qgate_graph-1.2rc1/qgate_graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 10:23:24.779129 qgate_graph-1.2rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-04-28 10:23:10.000000 qgate_graph-1.2rc1/setup.py
```

### Comparing `qgate_graph-1.1/qgate_graph/constant.py` & `qgate_graph-1.2rc1/qgate_graph/constant.py`

 * *Files identical despite different names*

### Comparing `qgate_graph-1.1/qgate_graph/graph.py` & `qgate_graph-1.2rc1/qgate_graph/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os.path, os
 import matplotlib.pyplot as plt
 import qgate_graph.constant as cns
 import json, datetime
 import logging
 class Graph:
+    """
+    Generate graph based on input data
+    """
     def __init__(self):
         self._markers = ['o','x', '*', '^','X', 'D', 'p', 'H']
         self._marker_point=0
         self._colors=['c', 'm', 'r', 'b', 'g', 'y', 'k', 'w']
         self._color_point=0
 
     def _find_key(self, performance_line: str, keys):
@@ -124,27 +127,39 @@
     def _unife_file_name(self, file_name):
         remove_item=" ,&?"
         for itm in remove_item:
             file_name=file_name.replace(itm,"_")
         file_name=file_name.replace("__","_")
         return file_name
 
-    def generate_from_dir(self, input_dir: str, output_dir: str):
+    def generate_from_dir(self, input_dir: str="input", output_dir: str="output"):
+        """
+        Generate graphs based on input directory
+
+        :param input_dir:       Input directory (default "input")
+        :param output_dir:      Output directory (default "output")
+        """
         for file in os.listdir(input_dir):
             self.generate_from_file(os.path.join(input_dir, file), output_dir)
 
-    def generate_from_file(self, perf_data: str, output_dir: str):
+    def generate_from_file(self, input_file: str, output_dir: str="output"):
+        """
+        Generate graphs based on input input file
+
+        :param input_file:      Input file
+        :param output_dir:      Output directory (default "output")
+        """
         file_name=None
         total_performance={}
         avrg_time={}
         std_deviation={}
         executors={}
 
-        logging.info(f"Processing '{perf_data}' ...")
-        with open(perf_data, "r") as f:
+        logging.info(f"Processing '{input_file}' ...")
+        with open(input_file, "r") as f:
             while True:
                 line=f.readline()
                 if not line:
                     break
                 if line[0]=='#':
                     if file_name:
                         self._show_graph(executors, total_performance, avrg_time, std_deviation,title, file_name,output_dir)
```

### Comparing `qgate_graph-1.1/setup.py` & `qgate_graph-1.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 #with open('HISTORY.md') as history_file:
 #    HISTORY = history_file.read()
 setup_args = dict(
     name='qgate_graph',
-    version='1.1',
+    version='v1.2-rc1',
     description='Generate graphs based on outputs from Quality Gate',
     long_description_content_type="text/markdown",
     long_description=README, # + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Jiri Steuer',
     author_email='steuer.jiri@gmail.com',
```

