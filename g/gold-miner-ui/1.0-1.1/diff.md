# Comparing `tmp/gold-miner-ui-1.0.tar.gz` & `tmp/gold-miner-ui-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gold-miner-ui-1.0.tar", last modified: Wed Apr 19 14:23:33 2023, max compression
+gzip compressed data, was "gold-miner-ui-1.1.tar", last modified: Fri Apr 28 08:58:09 2023, max compression
```

## Comparing `gold-miner-ui-1.0.tar` & `gold-miner-ui-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.385154 gold-miner-ui-1.0/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-17 23:17:21.000000 gold-miner-ui-1.0/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      656 2023-04-19 14:23:33.385154 gold-miner-ui-1.0/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      228 2023-04-17 23:05:25.000000 gold-miner-ui-1.0/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.383154 gold-miner-ui-1.0/apropos/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-17 22:59:26.000000 gold-miner-ui-1.0/apropos/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.383154 gold-miner-ui-1.0/apropos/goldmine/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-17 22:59:39.000000 gold-miner-ui-1.0/apropos/goldmine/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.383154 gold-miner-ui-1.0/apropos/goldmine/output/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-17 22:59:05.000000 gold-miner-ui-1.0/apropos/goldmine/output/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     4329 2023-04-17 23:05:50.000000 gold-miner-ui-1.0/apropos/goldmine/output/goldQt.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.384154 gold-miner-ui-1.0/apropos/goldmine/reports/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-18 15:35:03.000000 gold-miner-ui-1.0/apropos/goldmine/reports/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1832 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/cancel.svg
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1808 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/check.svg
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     8410 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/hardhat.svg
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       63 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/header.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      796 2023-02-24 21:57:37.000000 gold-miner-ui-1.0/apropos/goldmine/reports/navbar-summary.html
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1118 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/navbar.html
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      567 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/report.css
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      639 2023-02-10 18:34:35.000000 gold-miner-ui-1.0/apropos/goldmine/reports/summary-template.md
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3020 2022-08-09 03:07:12.000000 gold-miner-ui-1.0/apropos/goldmine/reports/template.html
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3356 2023-03-21 18:38:46.000000 gold-miner-ui-1.0/apropos/goldmine/reports/template.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.384154 gold-miner-ui-1.0/apropos/goldmine/tools/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-18 15:31:49.000000 gold-miner-ui-1.0/apropos/goldmine/tools/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7479 2023-04-12 20:36:54.000000 gold-miner-ui-1.0/apropos/goldmine/tools/auditor.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     9310 2023-02-10 18:34:35.000000 gold-miner-ui-1.0/apropos/goldmine/tools/fingerprinter.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)    37599 2023-04-19 13:49:34.000000 gold-miner-ui-1.0/apropos/goldmine/tools/tande.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:23:33.385154 gold-miner-ui-1.0/gold_miner_ui.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      656 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      931 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      192 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       75 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-19 14:23:33.000000 gold-miner-ui-1.0/gold_miner_ui.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-19 14:23:33.385154 gold-miner-ui-1.0/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1542 2023-04-19 14:19:06.000000 gold-miner-ui-1.0/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      287 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.015945 gold-miner-ui-1.1/apropos/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.015945 gold-miner-ui-1.1/apropos/goldminer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.016945 gold-miner-ui-1.1/apropos/goldminer/output/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/output/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     4331 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/output/goldQt.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/apropos/goldminer/reports/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1832 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/cancel.svg
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     1808 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/check.svg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     8410 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/hardhat.svg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       63 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/header.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      796 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/navbar-summary.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1118 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/navbar.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      567 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/report.css
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      639 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/summary-template.md
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3020 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/template.html
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3356 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/reports/template.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/apropos/goldminer/tools/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7479 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/auditor.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     9310 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/fingerprinter.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    37608 2023-04-28 08:40:21.000000 gold-miner-ui-1.1/apropos/goldminer/tools/tande.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:58:09.017945 gold-miner-ui-1.1/gold_miner_ui.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      705 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      949 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      198 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       75 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-28 08:58:08.000000 gold-miner-ui-1.1/gold_miner_ui.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-28 08:58:09.018945 gold-miner-ui-1.1/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1539 2023-04-28 08:57:56.000000 gold-miner-ui-1.1/setup.py
```

### Comparing `gold-miner-ui-1.0/LICENSE` & `gold-miner-ui-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/output/goldQt.py` & `gold-miner-ui-1.1/apropos/goldminer/output/goldQt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import json
 import multiprocessing
 import threading
 import time
 import queue
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 from PyQt5.QtCore import QDateTime, Qt, QTimer
 from PyQt5.QtWidgets import (
     QApplication,
     QCheckBox,
     QComboBox,
     QDateTimeEdit,
@@ -47,15 +47,15 @@
 
         # create a graph
         self.graph = PlotWidget()
         vertLayout.addWidget(self.graph)
 
         # set styles
         self.graph.setBackground("w")
-        self.graph.setTitle("gold-mine analysis")
+        self.graph.setTitle("gold-miner analysis")
         self.pen = pg.mkPen(color=(0, 0, 255))
 
         # a container for storing data by identifier
         self.data = {}
 
         # create a label strip # TODO: make a table
         horizLayout = QHBoxLayout()
```

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/cancel.svg` & `gold-miner-ui-1.1/apropos/goldminer/reports/cancel.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/check.svg` & `gold-miner-ui-1.1/apropos/goldminer/reports/check.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/hardhat.svg` & `gold-miner-ui-1.1/apropos/goldminer/reports/hardhat.svg`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/navbar-summary.html` & `gold-miner-ui-1.1/apropos/goldminer/reports/navbar-summary.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/navbar.html` & `gold-miner-ui-1.1/apropos/goldminer/reports/navbar.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/report.css` & `gold-miner-ui-1.1/apropos/goldminer/reports/report.css`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/summary-template.md` & `gold-miner-ui-1.1/apropos/goldminer/reports/summary-template.md`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/template.html` & `gold-miner-ui-1.1/apropos/goldminer/reports/template.html`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/reports/template.md` & `gold-miner-ui-1.1/apropos/goldminer/reports/template.md`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/tools/auditor.py` & `gold-miner-ui-1.1/apropos/goldminer/tools/auditor.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/tools/fingerprinter.py` & `gold-miner-ui-1.1/apropos/goldminer/tools/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `gold-miner-ui-1.0/apropos/goldmine/tools/tande.py` & `gold-miner-ui-1.1/apropos/goldminer/tools/tande.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 from rich import print
 from rich.console import Console
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, FileType
 from logging import debug, info, warning, error, critical
 from concurrent.futures import ProcessPoolExecutor
 
 # our modules
-from apropos.goldmine.trainer import GoldMineTrainer
-from apropos.goldmine.pickaxe.pickaxe import PickAxe
-from apropos.goldmine.tools.aggregator import aggregate_results
-from apropos.goldmine.tools.auditor import calculate_similarities, plot_similarities
+from apropos.goldminer.trainer import GoldMineTrainer
+from apropos.goldminer.pickaxe.pickaxe import PickAxe
+from apropos.goldminer.tools.aggregator import aggregate_results
+from apropos.goldminer.tools.auditor import calculate_similarities, plot_similarities
 
 
 def parse_args():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
         epilog="Exmaple Usage: ",
@@ -165,19 +165,19 @@
             return plan[config_name]
 
         return default
 
     def get_dist_file(self, filename, output_directory):
         "Copies a FILENAME found either local path or distribution install to OUTPUT_DIRECTORY"
         output_file = os.path.join(output_directory, filename)
-        local_file = os.path.join("apropos/goldmine/reports", filename)
+        local_file = os.path.join("apropos/goldminer/reports", filename)
         if os.path.exists(local_file):
             shutil.copy(local_file, output_file)
         else:
-            source_stream = pkgutil.get_data("apropos.goldmine.reports", filename)
+            source_stream = pkgutil.get_data("apropos.goldminer.reports", filename)
             f = open(output_file, "wb")
             f.write(source_stream)
             f.close()
         return output_file
 
     def maybe_create_filtered_pcap(self, plan, plantype, spec):
         pkt_filter = self.get_spec(plan, spec, "filter", plantype, "")
@@ -395,15 +395,15 @@
                 test["file"],
                 old_suffix=".pcap",
                 new_suffix=f".test.{test_num}.fsdb",
                 output_directory=output_directory,
             )
         debug(f"  output results:  {test['file']} => {output_file}")
         # default to FSDB output formatted
-        from apropos.goldmine.output.goldFsdb import GoldFsdb
+        from apropos.goldminer.output.goldFsdb import GoldFsdb
 
         axe.output = GoldFsdb(out_file=output_file, save_values=True)
 
         packet_count = self.get_spec(plan, test, "packet_count", testing_token, 0)
         axe.three_tuple_only = self.get_spec(
             plan, test, "three_tuple_only", testing_token, False
         )
@@ -918,27 +918,27 @@
             "--include-before-body",
             f"{output_directory}/{navbar}",
             "--standalone",
             "--toc",
             "--toc-depth",
             "2",
             "--metadata",
-            "title=gold-mine-report",
+            "title=gold-miner-report",
         ]
         debug("running: " + " ".join(cmd))
         subprocess.run(["bash", "-c", " ".join(cmd)])
 
         # filter resulting html
         with open(tmpfile) as inh:
             with open(f"{output_directory}/{output_file}", "w") as outh:
                 for line in inh:
                     if line.startswith("<p><img"):
                         line = line.replace("<img ", '<img class="img-fluid" ')
                     line = line.replace(
-                        "gold-mine-report", "Gold-Mine Test and Evaluation Report"
+                        "gold-miner-report", "Gold-Mine Test and Evaluation Report"
                     )
                     outh.write(line)
 
         os.unlink(tmpfile)
         info(f"creating {output_directory}/{output_file}")
 
     def dump_algorithm_results(
```

### Comparing `gold-miner-ui-1.0/gold_miner_ui.egg-info/SOURCES.txt` & `gold-miner-ui-1.1/gold_miner_ui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE
 README.md
 setup.py
 apropos/__init__.py
-apropos/goldmine/__init__.py
-apropos/goldmine/output/__init__.py
-apropos/goldmine/output/goldQt.py
-apropos/goldmine/reports/__init__.py
-apropos/goldmine/reports/cancel.svg
-apropos/goldmine/reports/check.svg
-apropos/goldmine/reports/hardhat.svg
-apropos/goldmine/reports/header.html
-apropos/goldmine/reports/navbar-summary.html
-apropos/goldmine/reports/navbar.html
-apropos/goldmine/reports/report.css
-apropos/goldmine/reports/summary-template.md
-apropos/goldmine/reports/template.html
-apropos/goldmine/reports/template.md
-apropos/goldmine/tools/__init__.py
-apropos/goldmine/tools/auditor.py
-apropos/goldmine/tools/fingerprinter.py
-apropos/goldmine/tools/tande.py
+apropos/goldminer/__init__.py
+apropos/goldminer/output/__init__.py
+apropos/goldminer/output/goldQt.py
+apropos/goldminer/reports/__init__.py
+apropos/goldminer/reports/cancel.svg
+apropos/goldminer/reports/check.svg
+apropos/goldminer/reports/hardhat.svg
+apropos/goldminer/reports/header.html
+apropos/goldminer/reports/navbar-summary.html
+apropos/goldminer/reports/navbar.html
+apropos/goldminer/reports/report.css
+apropos/goldminer/reports/summary-template.md
+apropos/goldminer/reports/template.html
+apropos/goldminer/reports/template.md
+apropos/goldminer/tools/__init__.py
+apropos/goldminer/tools/auditor.py
+apropos/goldminer/tools/fingerprinter.py
+apropos/goldminer/tools/tande.py
 gold_miner_ui.egg-info/PKG-INFO
 gold_miner_ui.egg-info/SOURCES.txt
 gold_miner_ui.egg-info/dependency_links.txt
 gold_miner_ui.egg-info/entry_points.txt
 gold_miner_ui.egg-info/requires.txt
 gold_miner_ui.egg-info/top_level.txt
```

### Comparing `gold-miner-ui-1.0/setup.py` & `gold-miner-ui-1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gold-miner-ui",
-    version="1.0",
+    version="1.1",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
-    description="A UI (alpha) plugin that produces a live graph when using gold-mine",
+    description="A UI plugin that adds graphical extensions to gold-miner",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitlab.com/isi-apropos/gold-mine-ui",
+    url="https://gitlab.com/isi-apropos/gold-miner-ui",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "gold-miner",
@@ -25,24 +25,24 @@
         "multikeygraph",
         "jinja2",
         "roc_utils",
         "pyaml",
     ],
     entry_points={
         "console_scripts": [
-            "gold-mine-auditor = apropos.goldmine.tools.auditor:main",
-            "gold-mine-tande = apropos.goldmine.tools.tande:main",
-            "gold-mine-fingerprint = apropos.goldmine.tools.fingerprinter:main",
+            "gold-miner-auditor = apropos.goldminer.tools.auditor:main",
+            "gold-miner-tande = apropos.goldminer.tools.tande:main",
+            "gold-miner-fingerprint = apropos.goldminer.tools.fingerprinter:main",
         ]
     },
     python_requires=">=3.6",
     test_suite="nose.collector",
     tests_require=["nose"],
     package_data={
-        "apropos.goldmine.reports": [
+        "apropos.goldminer.reports": [
             "template.md",
             "summary-template.md",
             "template.html",
             "header.html",
             "navbar.html",
             "navbar-summary.html",
             "report.css",
```

