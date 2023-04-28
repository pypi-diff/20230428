# Comparing `tmp/gold-miner-1.0.tar.gz` & `tmp/gold-miner-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gold-miner-1.0.tar", last modified: Wed Apr 19 14:18:12 2023, max compression
+gzip compressed data, was "gold-miner-1.1.tar", last modified: Fri Apr 28 08:55:00 2023, max compression
```

## Comparing `gold-miner-1.0.tar` & `gold-miner-1.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.885742 gold-miner-1.0/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-17 23:16:46.000000 gold-miner-1.0/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      409 2023-04-19 14:18:12.885742 gold-miner-1.0/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        4 2021-11-09 16:49:29.000000 gold-miner-1.0/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.883742 gold-miner-1.0/apropos/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.883742 gold-miner-1.0/apropos/goldmine/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/goldmine/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.884742 gold-miner-1.0/apropos/goldmine/output/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3304 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/goldCurses.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1606 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/goldFsdb.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2099 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/goldHighLowWatermark.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1916 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/goldJson.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1252 2023-02-23 23:23:34.000000 gold-miner-1.0/apropos/goldmine/output/goldOutput.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      531 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/goldTextDump.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      324 2023-02-24 22:11:47.000000 gold-miner-1.0/apropos/goldmine/output/noop.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.884742 gold-miner-1.0/apropos/goldmine/pickaxe/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/goldmine/pickaxe/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)    32567 2023-04-03 15:08:01.000000 gold-miner-1.0/apropos/goldmine/pickaxe/pickaxe.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.884742 gold-miner-1.0/apropos/goldmine/reports/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-18 15:35:54.000000 gold-miner-1.0/apropos/goldmine/reports/__init__.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.884742 gold-miner-1.0/apropos/goldmine/tests/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-06-21 15:48:59.000000 gold-miner-1.0/apropos/goldmine/tests/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1962 2022-06-22 16:13:51.000000 gold-miner-1.0/apropos/goldmine/tests/test_get_spec.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      403 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/goldmine/tests/test_loads.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2117 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/goldmine/tests/test_pickaxe_math.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.885742 gold-miner-1.0/apropos/goldmine/tools/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-02-24 21:57:37.000000 gold-miner-1.0/apropos/goldmine/tools/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2608 2023-02-10 18:34:35.000000 gold-miner-1.0/apropos/goldmine/tools/aggregator.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     8892 2023-04-18 15:22:44.000000 gold-miner-1.0/apropos/goldmine/tools/goldmine.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     5105 2022-06-21 15:38:00.000000 gold-miner-1.0/apropos/goldmine/tools/smelter.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2334 2022-07-12 21:04:32.000000 gold-miner-1.0/apropos/goldmine/tools/trainer.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.885742 gold-miner-1.0/apropos/goldmine/trainer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7390 2023-04-19 13:37:09.000000 gold-miner-1.0/apropos/goldmine/trainer/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3804 2023-04-03 15:07:45.000000 gold-miner-1.0/apropos/goldmine/trainer/widthtrainer.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-19 14:18:12.885742 gold-miner-1.0/gold_miner.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      409 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1104 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      249 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       29 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-19 14:18:12.000000 gold-miner-1.0/gold_miner.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-19 14:18:12.885742 gold-miner-1.0/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1193 2023-04-19 14:18:03.000000 gold-miner-1.0/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1069 2023-04-28 08:32:13.000000 gold-miner-1.1/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-28 08:55:00.498841 gold-miner-1.1/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      810 2023-04-28 08:32:13.000000 gold-miner-1.1/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.495842 gold-miner-1.1/apropos/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.495842 gold-miner-1.1/apropos/goldminer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.496842 gold-miner-1.1/apropos/goldminer/output/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3305 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldCurses.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1607 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldFsdb.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2100 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldHighLowWatermark.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1917 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldJson.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1252 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldOutput.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      532 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/goldTextDump.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      325 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/output/noop.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.496842 gold-miner-1.1/apropos/goldminer/pickaxe/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/pickaxe/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)    32568 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/pickaxe/pickaxe.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/reports/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/reports/__init__.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/tests/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      406 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/test_loads.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2118 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tests/test_pickaxe_math.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.497841 gold-miner-1.1/apropos/goldminer/tools/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       76 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2609 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/aggregator.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     8901 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/goldminer.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5107 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/smelter.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2336 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/tools/trainer.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/apropos/goldminer/trainer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     7390 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/trainer/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3805 2023-04-28 08:30:54.000000 gold-miner-1.1/apropos/goldminer/trainer/widthtrainer.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-04-28 08:55:00.498841 gold-miner-1.1/gold_miner.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1216 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1087 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      258 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       29 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        8 2023-04-28 08:55:00.000000 gold-miner-1.1/gold_miner.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-04-28 08:55:00.498841 gold-miner-1.1/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1203 2023-04-28 08:54:55.000000 gold-miner-1.1/setup.py
```

### Comparing `gold-miner-1.0/LICENSE` & `gold-miner-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldCurses.py` & `gold-miner-1.1/apropos/goldminer/output/goldCurses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import curses
 
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 
 class GoldCurses(GoldOutput):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.win = curses.initscr()
         curses.start_color()
```

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldFsdb.py` & `gold-miner-1.1/apropos/goldminer/output/goldFsdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from logging import debug, warning
 import collections
 import pyfsdb
 
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 
 class GoldFsdb(GoldOutput):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.as_percentage = kwargs.get("as_percentage", False)
         self.raw_values = kwargs.get("raw_values", False)
```

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldHighLowWatermark.py` & `gold-miner-1.1/apropos/goldminer/output/goldHighLowWatermark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import warning, debug, info
 
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 
 class GoldHighLowWatermark(GoldOutput):
     """Truncates an output generator to just when values pass a high/low
     watermark.  When an incoming value goes beyond the *high* mark, a
     (single) report is made.  When the value drops below the *low*
     mark afterward, another report is made indicating it dropped below
```

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldJson.py` & `gold-miner-1.1/apropos/goldminer/output/goldJson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import json
 
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 
 class GoldJson(GoldOutput):
     "Outputs results in a list of json dictionaries."
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldOutput.py` & `gold-miner-1.1/apropos/goldminer/output/goldOutput.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.0/apropos/goldmine/output/goldTextDump.py` & `gold-miner-1.1/apropos/goldminer/output/goldTextDump.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from apropos.goldmine.output.goldOutput import GoldOutput
+from apropos.goldminer.output.goldOutput import GoldOutput
 
 
 class GoldTextDump(GoldOutput):
     def __init__(self, seperator="\n"):
         self.seperator = seperator
 
     def output(self, analysis_results, packet_number, tunnel_count, subscriptions):
```

### Comparing `gold-miner-1.0/apropos/goldmine/pickaxe/pickaxe.py` & `gold-miner-1.1/apropos/goldminer/pickaxe/pickaxe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import Counter, defaultdict
 from logging import debug, info, warning, error, critical
 import dpkt
 import numpy as np
 import time
 import pyfsdb
 import pprint
-from apropos.goldmine.output.noop import GoldNoOp
+from apropos.goldminer.output.noop import GoldNoOp
 
 #
 # Analyzer
 #
 last_packet_time = {}
```

### Comparing `gold-miner-1.0/apropos/goldmine/tests/test_pickaxe_math.py` & `gold-miner-1.1/apropos/goldminer/tests/test_pickaxe_math.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 
 class TestPickAxeMath(unittest.TestCase):
     def test_difference_function(self):
-        from apropos.goldmine.pickaxe.pickaxe import PickAxe
+        from apropos.goldminer.pickaxe.pickaxe import PickAxe
 
         a = PickAxe()
 
         # measured, dirty_min, gold_value, dirty_max, expected
         test_cases = [
             [0.2, 0.4, 0.3, 0.8, 0.0],  # measured < gold < min < max
             [0.8, 0.1, 0.7, 0.6, 0.0],  # min < max < gold < measured
```

### Comparing `gold-miner-1.0/apropos/goldmine/tools/aggregator.py` & `gold-miner-1.1/apropos/goldminer/tools/aggregator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import pyfsdb
 import collections
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, FileType
 import logging
 from logging import debug, info, warning, error, critical
-from apropos.goldmine.trainer import GoldMineTrainer
+from apropos.goldminer.trainer import GoldMineTrainer
 
 
 def parse_args():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
         epilog="Exmaple Usage: "
```

### Comparing `gold-miner-1.0/apropos/goldmine/tools/goldmine.py` & `gold-miner-1.1/apropos/goldminer/tools/goldminer.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 import time
 
 try:
     import curses
 except Exception:
     pass
 
-from apropos.goldmine.pickaxe.pickaxe import PickAxe
+from apropos.goldminer.pickaxe.pickaxe import PickAxe
 
 
 def get_parser():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
-        epilog="Exmaple Usage: gold-mine.py -i " + "INTERFACE -g profilename",
+        epilog="Exmaple Usage: gold-miner.py -i " + "INTERFACE -g profilename",
     )
 
     parser.add_argument(
         "-i", "--interface", type=str, help="The interface to monitor for ESP traffic"
     )
 
     parser.add_argument(
@@ -234,54 +234,54 @@
         raise ValueError("either -i or -r is required")
 
     return args
 
 
 def process_arguments(args, axe):
     if args.live_results:
-        from apropos.goldmine.output.goldTextDump import GoldTextDump
+        from apropos.goldminer.output.goldTextDump import GoldTextDump
 
         axe.output = GoldTextDump()
     elif args.curses:
-        from apropos.goldmine.output.goldCurses import GoldCurses
+        from apropos.goldminer.output.goldCurses import GoldCurses
 
         axe.output = GoldCurses(
             as_percentage=args.percentage, parameter_file=args.thresholds
         )
     elif args.output_json or args.output_flattened_json:
-        from apropos.goldmine.output.goldJson import GoldJson
+        from apropos.goldminer.output.goldJson import GoldJson
 
         axe.output = GoldJson(
             as_percentage=args.percentage,
             raw_values=args.raw_values,
             as_list=True,
             parameter_file=args.thresholds,
             flatten=args.output_flattened_json,
         )
     elif args.output_ui:
         try:
-            from apropos.goldmine.output.goldQt import GoldQt
+            from apropos.goldminer.output.goldQt import GoldQt
         except Exception:
-            error("The goldQt module was not found -- please install gold-mine-ui")
+            error("The goldQt module was not found -- please install gold-miner-ui")
             exit(1)
 
         axe.output = GoldQt()
     else:
         # default to FSDB output formatted
-        from apropos.goldmine.output.goldFsdb import GoldFsdb
+        from apropos.goldminer.output.goldFsdb import GoldFsdb
 
         axe.output = GoldFsdb(
             out_file_handle=args.output_file,
             as_percentage=args.percentage,
             raw_values=args.raw_values,
             parameter_file=args.thresholds,
         )
 
     if args.high_low_watermark:
-        from apropos.goldmine.output.goldHighLowWatermark import GoldHighLowWatermark
+        from apropos.goldminer.output.goldHighLowWatermark import GoldHighLowWatermark
 
         highlow = GoldHighLowWatermark(
             high=args.high_low_watermark[0],
             low=args.high_low_watermark[1],
             output=axe.output,
         )
         debug("inserted a high-low process")
```

### Comparing `gold-miner-1.0/apropos/goldmine/tools/smelter.py` & `gold-miner-1.1/apropos/goldminer/tools/smelter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Simplifies gold-mine output into true/false values to reduce numeric confusion"""
+"""Simplifies gold-miner output into true/false values to reduce numeric confusion"""
 
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, FileType
 from logging import debug, info, warning, error, critical
 import logging
 import re
 import sys
 import pyfsdb
@@ -39,15 +39,15 @@
     )
 
     parser.add_argument(
         "input_file",
         type=FileType("r"),
         nargs="?",
         default=sys.stdin,
-        help="Input file to read generated by gold-mine",
+        help="Input file to read generated by gold-miner",
     )
 
     parser.add_argument(
         "output_file",
         type=FileType("w"),
         nargs="?",
         default=sys.stdout,
```

### Comparing `gold-miner-1.0/apropos/goldmine/tools/trainer.py` & `gold-miner-1.1/apropos/goldminer/tools/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 
 import sys
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, FileType
 import logging
 from logging import debug, info, warning, error, critical
-from apropos.goldmine.trainer import GoldMineTrainer
-from apropos.goldmine.trainer.widthtrainer import GoldMineWidthTrainer
+from apropos.goldminer.trainer import GoldMineTrainer
+from apropos.goldminer.trainer.widthtrainer import GoldMineWidthTrainer
 
 
 def parse_args():
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         description=__doc__,
         epilog="Exmaple Usage: " + "pcap-to-fsdb.py -o output.fsdb input.pcap",
```

### Comparing `gold-miner-1.0/apropos/goldmine/trainer/__init__.py` & `gold-miner-1.1/apropos/goldminer/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `gold-miner-1.0/apropos/goldmine/trainer/widthtrainer.py` & `gold-miner-1.1/apropos/goldminer/trainer/widthtrainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import collections
 import numpy as np
 from logging import debug, info, warning, error, critical
-from apropos.goldmine.trainer import GoldMineBase
+from apropos.goldminer.trainer import GoldMineBase
 
 
 class GoldMineWidthTrainer(GoldMineBase):
     def __init__(self, addresses=None, max_width=10000, max_pkt_size=1500):
         super().__init__(addresses)
         self.packet_data = collections.defaultdict(collections.Counter)
```

### Comparing `gold-miner-1.0/gold_miner.egg-info/SOURCES.txt` & `gold-miner-1.1/gold_miner.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 LICENSE
 README.md
 setup.py
 apropos/__init__.py
-apropos/goldmine/__init__.py
-apropos/goldmine/output/__init__.py
-apropos/goldmine/output/goldCurses.py
-apropos/goldmine/output/goldFsdb.py
-apropos/goldmine/output/goldHighLowWatermark.py
-apropos/goldmine/output/goldJson.py
-apropos/goldmine/output/goldOutput.py
-apropos/goldmine/output/goldTextDump.py
-apropos/goldmine/output/noop.py
-apropos/goldmine/pickaxe/__init__.py
-apropos/goldmine/pickaxe/pickaxe.py
-apropos/goldmine/reports/__init__.py
-apropos/goldmine/tests/__init__.py
-apropos/goldmine/tests/test_get_spec.py
-apropos/goldmine/tests/test_loads.py
-apropos/goldmine/tests/test_pickaxe_math.py
-apropos/goldmine/tools/__init__.py
-apropos/goldmine/tools/aggregator.py
-apropos/goldmine/tools/goldmine.py
-apropos/goldmine/tools/smelter.py
-apropos/goldmine/tools/trainer.py
-apropos/goldmine/trainer/__init__.py
-apropos/goldmine/trainer/widthtrainer.py
+apropos/goldminer/__init__.py
+apropos/goldminer/output/__init__.py
+apropos/goldminer/output/goldCurses.py
+apropos/goldminer/output/goldFsdb.py
+apropos/goldminer/output/goldHighLowWatermark.py
+apropos/goldminer/output/goldJson.py
+apropos/goldminer/output/goldOutput.py
+apropos/goldminer/output/goldTextDump.py
+apropos/goldminer/output/noop.py
+apropos/goldminer/pickaxe/__init__.py
+apropos/goldminer/pickaxe/pickaxe.py
+apropos/goldminer/reports/__init__.py
+apropos/goldminer/tests/__init__.py
+apropos/goldminer/tests/test_loads.py
+apropos/goldminer/tests/test_pickaxe_math.py
+apropos/goldminer/tools/__init__.py
+apropos/goldminer/tools/aggregator.py
+apropos/goldminer/tools/goldminer.py
+apropos/goldminer/tools/smelter.py
+apropos/goldminer/tools/trainer.py
+apropos/goldminer/trainer/__init__.py
+apropos/goldminer/trainer/widthtrainer.py
 gold_miner.egg-info/PKG-INFO
 gold_miner.egg-info/SOURCES.txt
 gold_miner.egg-info/dependency_links.txt
 gold_miner.egg-info/entry_points.txt
 gold_miner.egg-info/requires.txt
 gold_miner.egg-info/top_level.txt
```

### Comparing `gold-miner-1.0/setup.py` & `gold-miner-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gold-miner",
-    version="1.0",
+    version="1.1",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A encrypted tunnel identification research package",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitlab.com/isi-apropos/gold-mine",
+    url="https://gitlab.com/isi-apropos/gold-miner",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
             # migrating to pdb prefixes
-            "gold-mine = apropos.goldmine.tools.goldmine:main",
-            "gold-mine-trainer = apropos.goldmine.tools.trainer:main",
-            "gold-mine-trainer-aggregator = apropos.goldmine.tools.aggregator:main",
-            "gold-mine-smelter = apropos.goldmine.tools.smelter:main",
+            "gold-miner = apropos.goldminer.tools.goldminer:main",
+            "gold-miner-trainer = apropos.goldminer.tools.trainer:main",
+            "gold-miner-trainer-aggregator = apropos.goldminer.tools.aggregator:main",
+            "gold-miner-smelter = apropos.goldminer.tools.smelter:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[
```

