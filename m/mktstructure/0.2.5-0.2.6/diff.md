# Comparing `tmp/mktstructure-0.2.5.tar.gz` & `tmp/mktstructure-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktstructure-0.2.5.tar", last modified: Fri Mar 24 01:56:37 2023, max compression
+gzip compressed data, was "mktstructure-0.2.6.tar", last modified: Fri Apr 28 01:04:34 2023, max compression
```

## Comparing `mktstructure-0.2.5.tar` & `mktstructure-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:56:37.354948 mktstructure-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-24 01:56:32.000000 mktstructure-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-24 01:56:37.354948 mktstructure-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-24 01:56:32.000000 mktstructure-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:56:37.350948 mktstructure-0.2.5/mktstructure/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/cmd_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/cmd_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/cmd_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/cmd_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:56:37.354948 mktstructure-0.2.5/mktstructure/measures/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/bidask_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/effective_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/price_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/measures/realized_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/request_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/trth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/trth_parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-03-24 01:56:32.000000 mktstructure-0.2.5/mktstructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:56:37.354948 mktstructure-0.2.5/mktstructure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-24 01:56:36.000000 mktstructure-0.2.5/mktstructure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-24 01:56:37.000000 mktstructure-0.2.5/mktstructure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 01:56:36.000000 mktstructure-0.2.5/mktstructure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-24 01:56:36.000000 mktstructure-0.2.5/mktstructure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 01:56:36.000000 mktstructure-0.2.5/mktstructure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-24 01:56:36.000000 mktstructure-0.2.5/mktstructure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 01:56:37.354948 mktstructure-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-24 01:56:32.000000 mktstructure-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 01:04:28.000000 mktstructure-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 01:04:34.166175 mktstructure-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-28 01:04:28.000000 mktstructure-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.162175 mktstructure-0.2.6/mktstructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/cmd_download_mktdepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/mktstructure/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/bidask_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/effective_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/price_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/realized_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/measures/variance_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/request_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/trth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/trth_parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-28 01:04:28.000000 mktstructure-0.2.6/mktstructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:04:34.166175 mktstructure-0.2.6/mktstructure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 01:04:34.000000 mktstructure-0.2.6/mktstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:04:33.000000 mktstructure-0.2.6/mktstructure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:04:34.166175 mktstructure-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 01:04:28.000000 mktstructure-0.2.6/setup.py
```

### Comparing `mktstructure-0.2.5/LICENSE` & `mktstructure-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/PKG-INFO` & `mktstructure-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.5
+Version: 0.2.6
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.5/README.md` & `mktstructure-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/cmd_classify.py` & `mktstructure-0.2.6/mktstructure/cmd_classify.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/cmd_clean.py` & `mktstructure-0.2.6/mktstructure/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/cmd_compute.py` & `mktstructure-0.2.6/mktstructure/cmd_compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
                 continue
 
             path = os.path.join(root, f)
             ric, date = os.path.normpath(path).split(os.sep)[-2:]
             date = dt.fromisoformat(
                 date.removesuffix(".csv")
                 .removesuffix(".csv.gz")
-                .removesuffix(".sorted")
                 .removesuffix(".signed")
+                .removesuffix(".sorted")
             )
 
             # if `--all` flag is set
             if not args.all:
                 if ric not in args.ric:
                     continue
 
@@ -47,16 +47,26 @@
                     _compute(measures.bidask_spread, path, date, ric, df, fout)
                 if args.effective_spread:
                     _compute(measures.effective_spread, path, date, ric, df, fout)
                 if args.realized_spread:
                     _compute(measures.realized_spread, path, date, ric, df, fout)
                 if args.price_impact:
                     _compute(measures.price_impact, path, date, ric, df, fout)
+                if args.variance_ratio:
+                    _compute(measures.variance_ratio, path, date, ric, df, fout)
 
     fout.close()
 
 
 def _compute(measure, path, date, ric, data, fout):
     print(f"Computing {measure.name} for {path}")
     result = measure.estimate(data)
-    result_formated = format_result(date, ric, measure.name, result)
-    print(result_formated, file=fout)
+    # Variance ratio test returns a list of results
+    if measure.name == "LoMacKinlay1988":
+        assert isinstance(result, list)
+        for res in result:
+            for k, v in res.items():
+                formated = format_result(date, ric, k, v)
+                print(formated, file=fout)
+    else:
+        result_formated = format_result(date, ric, measure.name, result)
+        print(result_formated, file=fout)
```

### Comparing `mktstructure-0.2.5/mktstructure/cmd_download.py` & `mktstructure-0.2.6/mktstructure/cmd_download.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/main.py` & `mktstructure-0.2.6/mktstructure/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,19 @@
         description="Choose one from the following. Use `mktstructure subcommand -h` to see help for each sub-command.",
     )
     parser_download = subparsers.add_parser(
         "download",
         description="Download data from Refinitiv Tick History",
         help="Download data from Refinitiv Tick History",
     )
+    parser_download_mktdepth = subparsers.add_parser(
+        "download_mktdepth",
+        description="Download market depth data from Refinitiv Tick History",
+        help="Download market depth data from Refinitiv Tick History",
+    )
     parser_clean = subparsers.add_parser(
         "clean",
         description="Clean the data in the data directory",
         help="Clean downloaded data",
     )
     parser_classify = subparsers.add_parser(
         "classify",
@@ -150,14 +155,77 @@
         "--threads",
         metavar="threads",
         type=int,
         help="number of workers to use",
         default=os.cpu_count(),
     )
 
+    # subparser for `download_mktdepth` subcommand
+    parser_download_mktdepth.add_argument(
+        "-u",
+        metavar="user",
+        help="DataScope username",
+    )
+    parser_download_mktdepth.add_argument(
+        "-p",
+        metavar="password",
+        help="DataScope password",
+    )
+    parser_download_mktdepth.add_argument(
+        "-b",
+        metavar="begin",
+        default="2021-02-15",
+        help="begin UTC date (YYYY-MM-DD)",
+    )
+    parser_download_mktdepth.add_argument(
+        "-e",
+        metavar="end",
+        default="2021-02-28",
+        help="end UTC date (YYYY-MM-DD)",
+    )
+    parser_download_mktdepth.add_argument(
+        "-o",
+        metavar="out",
+        default="out.csv.gz",
+        help="output file path",
+    )
+    parser_download_mktdepth.add_argument(
+        "--ric",
+        nargs="*",
+        default=[],
+        help="RIC of securities to process",
+    )
+    parser_download_mktdepth.add_argument(
+        "--sp500",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, process all S&P500 components (extending RIC list, if any)",
+    )
+    parser_download_mktdepth.add_argument(
+        "--parse",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, parse the downloaded raw data to output data directory",
+    )
+    parser_download_mktdepth.add_argument(
+        "--data_dir",
+        metavar="dir",
+        default="./data",
+        help="output data directory (used when --parse is set)",
+    )
+    parser_download_mktdepth.add_argument(
+        "--compress",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compress parsed data (effective only when --parse is set)",
+    )
+
     # parser for `classify` subcommand
     parser_classify.add_argument(
         "--ric",
         nargs="*",
         default=[],
         help="RIC of securities to clean",
     )
@@ -257,27 +325,39 @@
     parser_compute.add_argument(
         "--price_impact",
         default=False,
         const=True,
         action="store_const",
         help="if set, compute the price impact",
     )
+    parser_compute.add_argument(
+        "--variance_ratio",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compute the variance ratio and test statistics",
+    )
 
     return parser
 
 
 def main():
     parser = init_argparse()
     args = parser.parse_args()
 
     if args.command == "download":
         from .cmd_download import cmd_download
 
         cmd_download(args)
 
+    if args.command == "download_mktdepth":
+        from .cmd_download_mktdepth import cmd_download_mktdepth
+
+        cmd_download_mktdepth(args)
+
     if args.command == "clean":
         from .cmd_clean import cmd_clean
 
         cmd_clean(args)
 
     if args.command == "classify":
         from .cmd_classify import cmd_classify
```

### Comparing `mktstructure-0.2.5/mktstructure/measures/bidask_spread.py` & `mktstructure-0.2.6/mktstructure/measures/bidask_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/measures/effective_spread.py` & `mktstructure-0.2.6/mktstructure/measures/effective_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/measures/price_impact.py` & `mktstructure-0.2.6/mktstructure/measures/price_impact.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/measures/realized_spread.py` & `mktstructure-0.2.6/mktstructure/measures/realized_spread.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 where q is the trade direction (1 for buys and -1 for sells),
 P is the transaction price, and midpoint_5min is the bid-ask midpoint 5mins later. 
 """
 vars_needed = {"Price", "Volume", "Mid Point", "Direction"}
 
 
 def estimate(data: pd.DataFrame) -> np.ndarray:
-    log_midpt = np.log(data["Mid Point"].to_numpy())
+    midpt = data["Mid Point"].to_numpy()
     price = data["Price"].to_numpy()
     timestamps = np.array(data.index, dtype="datetime64")
     # Find the Quote Mid Point 5 min later than each trade.
     matched_midpt = []
     for idx, ts1 in enumerate(timestamps):
         for i, ts2 in enumerate(timestamps[idx:]):
             if ts2 - ts1 >= np.timedelta64(5, "m"):
-                matched_midpt.append(log_midpt[idx + i])
+                matched_midpt.append(midpt[idx + i])
                 break
     matched = len(matched_midpt)
     rspread = (
         2 * data["Direction"].to_numpy()[:matched] * (price[:matched] - matched_midpt)
     )
     # Daily realized spread is the dollar-volume-weighted average
     # of the realized spread computed over all trades in the day.
```

### Comparing `mktstructure-0.2.5/mktstructure/request_templates.py` & `mktstructure-0.2.6/mktstructure/request_templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,45 @@
         "Range": {
             "Start": "2019-01-01T00:00:00.000Z",
             "End": "2020-01-01T00:00:00.000Z",
         },
     }
 }
 
+INTRADAY_MARKET_DEPTH = {
+    "ExtractionRequest": {
+        "@odata.type": "#DataScope.Select.Api.Extractions.ExtractionRequests.TickHistoryMarketDepthExtractionRequest",
+        "ContentFieldNames": [
+            "Ask Price",
+            "Ask Size",
+            "Bid Price",
+            "Bid Size",
+            "Exchange Time",
+            "Number of Buyers",
+            "Number of Sellers",
+        ],
+        "IdentifierList": {
+            "@odata.type": "#DataScope.Select.Api.Extractions.ExtractionRequests.InstrumentIdentifierList",
+            "InstrumentIdentifiers": [
+                {"Identifier": "AAPL.OQ", "IdentifierType": "Ric"}
+            ],
+            "UseUserPreferencesForValidationOptions": "False",
+        },
+        "Condition": {
+            "View": "NormalizedLL2",
+            "NumberOfLevels": 5,
+            "MessageTimeStampIn": "GmtUtc",
+            "ReportDateRangeType": "Range",
+            "QueryStartDate": "2020-03-01T00:00:00.000Z",
+            "QueryEndDate": "2020-03-03T00:00:00.000Z",
+            "DisplaySourceRIC": "False",
+        },
+    }
+}
+
 INTRADAY_TICKS = {
     "ExtractionRequest": {
         "@odata.type": "#DataScope.Select.Api.Extractions.ExtractionRequests.TickHistoryTimeAndSalesExtractionRequest",
         "ContentFieldNames": [
             "Quote - Bid Price",
             "Quote - Bid Size",
             "Quote - Ask Price",
```

### Comparing `mktstructure-0.2.5/mktstructure/trth.py` & `mktstructure-0.2.6/mktstructure/trth.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/trth_parser.c` & `mktstructure-0.2.6/mktstructure/trth_parser.c`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.5/mktstructure/utils.py` & `mktstructure-0.2.6/mktstructure/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 from typing import List, Dict
 from numba import jit
 import pandas as pd
 import numpy as np
-from .request_templates import INDEX_COMPONENTS, INTRADAY_TICKS
+from .request_templates import INDEX_COMPONENTS, INTRADAY_TICKS, INTRADAY_MARKET_DEPTH
 
 
 SP500_RIC = "0#.SPX"
 NASDAQ_RIC = "0#.NDX"
 NYSE_RIC = "0#.NYA"
 
 
@@ -47,14 +47,24 @@
     request["ExtractionRequest"]["IdentifierList"]["InstrumentIdentifiers"] = [
         {"Identifier": ric, "IdentifierType": "Ric"} for ric in rics
     ]
     request["ExtractionRequest"]["Condition"]["QueryStartDate"] = date_start
     request["ExtractionRequest"]["Condition"]["QueryEndDate"] = date_end
     return request
 
+
+def make_request_tick_history_market_depth(rics: List[str], date_start, date_end):
+    request = INTRADAY_MARKET_DEPTH.copy()
+    request["ExtractionRequest"]["IdentifierList"]["InstrumentIdentifiers"] = [
+        {"Identifier": ric, "IdentifierType": "Ric"} for ric in rics
+    ]
+    request["ExtractionRequest"]["Condition"]["QueryStartDate"] = date_start
+    request["ExtractionRequest"]["Condition"]["QueryEndDate"] = date_end
+    return request
+
 
 def lee_and_ready(df: pd.DataFrame) -> pd.DataFrame:
     # Convert to pd.DatetimeIndex to preserve nanoseconds.
     df["Date-Time"] = pd.DatetimeIndex(df["Date-Time"])
     # Get GMT Offset
     offset = np.timedelta64(df["GMT Offset"].iloc[0], "h")
     # Convert from GMTUTC to local time.
```

### Comparing `mktstructure-0.2.5/mktstructure.egg-info/PKG-INFO` & `mktstructure-0.2.6/mktstructure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.5
+Version: 0.2.6
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.5/mktstructure.egg-info/SOURCES.txt` & `mktstructure-0.2.6/mktstructure.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 mktstructure/__init__.py
 mktstructure/cmd_classify.py
 mktstructure/cmd_clean.py
 mktstructure/cmd_compute.py
 mktstructure/cmd_download.py
+mktstructure/cmd_download_mktdepth.py
 mktstructure/main.py
 mktstructure/request_templates.py
 mktstructure/trth.py
 mktstructure/trth_parser.c
 mktstructure/utils.py
 mktstructure.egg-info/PKG-INFO
 mktstructure.egg-info/SOURCES.txt
@@ -18,8 +19,9 @@
 mktstructure.egg-info/requires.txt
 mktstructure.egg-info/top_level.txt
 mktstructure/measures/__init__.py
 mktstructure/measures/bidask_spread.py
 mktstructure/measures/effective_spread.py
 mktstructure/measures/exceptions.py
 mktstructure/measures/price_impact.py
-mktstructure/measures/realized_spread.py
+mktstructure/measures/realized_spread.py
+mktstructure/measures/variance_ratio.py
```

### Comparing `mktstructure-0.2.5/setup.py` & `mktstructure-0.2.6/setup.py`

 * *Files identical despite different names*

