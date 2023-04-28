# Comparing `tmp/alacorder-79.8.8.tar.gz` & `tmp/alacorder-79.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.8.8.tar", max compression
+gzip compressed data, was "alacorder-79.8.9.tar", max compression
```

## Comparing `alacorder-79.8.8.tar` & `alacorder-79.8.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.8.8/LICENSE
--rw-r--r--   0        0        0     9801 2023-04-27 23:24:11.886024 alacorder-79.8.8/README.md
--rw-r--r--   0        0        0      697 2023-04-27 23:25:07.609939 alacorder-79.8.8/pyproject.toml
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.8.8/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.8.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   166065 2023-04-27 23:24:44.915220 alacorder-79.8.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   166065 2023-04-27 23:24:35.455445 alacorder-79.8.8/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.8.8/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 alacorder-79.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.8.9/LICENSE
+-rw-r--r--   0        0        0     9801 2023-04-27 23:24:11.886024 alacorder-79.8.9/README.md
+-rw-r--r--   0        0        0      697 2023-04-28 01:12:26.214336 alacorder-79.8.9/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.8.9/src/alacorder/.python-version
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.8.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   167384 2023-04-28 01:11:07.717891 alacorder-79.8.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   167384 2023-04-28 01:10:59.052060 alacorder-79.8.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.8.9/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 alacorder-79.8.9/PKG-INFO
```

### Comparing `alacorder-79.8.8/LICENSE` & `alacorder-79.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.8/README.md` & `alacorder-79.8.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.8/pyproject.toml` & `alacorder-79.8.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.8.8"
+version = "79.8.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.8.8/src/alacorder/__init__.py` & `alacorder-79.8.9/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.8/src/alacorder/__main__.py` & `alacorder-79.8.9/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     selenium = ^4.8.3
     tqdm = ^4.65.0
     xlsx2csv = ^0.8.1
     XlsxWriter = ^3.0.9
 """
 
 name = "ALACORDER"
-version = "79.8.8"
+version = "79.8.9"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
@@ -144,30 +144,14 @@
     if cf["LOG"]:
         print("Created template successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("MT-COMPLETE", True)
     return tp
 
 
-def vrr(cf):
-    """
-    Summarize voting rights status from pairs using configuration object `cf`.
-    """
-    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
-    if not cf["NO_WRITE"]:
-        write(
-            vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
-        )
-    if cf["LOG"]:
-        print("Created table successfully.")
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
-    return vr
-
-
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
     plog("Extracting case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
@@ -319,49 +303,73 @@
     if not cf["NO_WRITE"]:
         write(out, sheet_names=["images"], cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
+def vrr_summary(cf):
+    """
+    Summarize voting rights status from pairs using configuration object `cf`.
+    """
+    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
+    if not cf["NO_WRITE"]:
+        write(
+            vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+        )
+    if cf["LOG"]:
+        print("Created table successfully.")
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
+    return vr
+
+
 def case_action_summary(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
     q = read(cf["QUEUE"])
     out = explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         write(out, sheet_names=["case-action-summary"], cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
+
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf['DEBUG'])
+    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         write(
-            ch, sheet_names=["ChargesSummary"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+            ch,
+            sheet_names=["ChargesSummary"],
+            path=cf["OUTPUT_PATH"],
+            overwrite=cf["OVERWRITE"],
         )
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
+
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf['DEBUG'])
+    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         write(
-            conv, sheet_names=["ConvictionsSummary"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+            conv,
+            sheet_names=["ConvictionsSummary"],
+            path=cf["OUTPUT_PATH"],
+            overwrite=cf["OVERWRITE"],
         )
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
@@ -373,15 +381,15 @@
     if cf["FETCH"] == True:
         ft = fetch(cf=cf)
         return ft
     elif cf["ARCHIVE"] == True:
         ar = archive(cf)
         return ar
     elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
-        vr = vrr(cf)
+        vr = vrr_summary(cf)
         return vr
     elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
         ch = charges_summary(cf)
         return ch
     elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
         conv = convictions_summary(cf)
         return cf
@@ -1074,116 +1082,122 @@
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     return names
 
+
 def charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
-    ) 
-    ch = src["charges"].filter(  # filter convictions
-        pl.col("Filing")
-    ) 
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
+    )
+    ch = src["charges"].filter(pl.col("Filing"))  # filter convictions
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(ch, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("CaseNumber"),
             pl.col("Alias"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("TypeDescription"),
             pl.col("CERVDisqCharge"),
             pl.col("PardonDisqCharge"),
-            pl.col("PermanentDisqCharge")
+            pl.col("PermanentDisqCharge"),
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("ChargesSummary").arr.lengths().alias("ChargeCount"),
-            pl.col("CERVDisqCharge")
-            .arr.count_match(True)
-            .alias("CERVChargeCount"),
-            pl.col("PardonDisqCharge")
-            .arr.count_match(True)
-            .alias("PardonChargeCount"),
-            pl.col("TypeDescription").arr.count_match("MISDEMEANOR").alias("MisdemeanorChargeCount"),
-            pl.col("TypeDescription").arr.count_match("FELONY").alias("FelonyChargeCount"),
-            pl.col("TypeDescription").arr.count_match("TRAFFIC").alias("TrafficChargeCount"),
+            pl.col("CERVDisqCharge").arr.count_match(True).alias("CERVChargeCount"),
+            pl.col("PardonDisqCharge").arr.count_match(True).alias("PardonChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("MISDEMEANOR")
+            .alias("MisdemeanorChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("FELONY")
+            .alias("FelonyChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("TRAFFIC")
+            .alias("TrafficChargeCount"),
             pl.col("PermanentDisqCharge")
             .arr.count_match(True)
             .alias("PermanentChargeCount"),
             pl.col("ChargesSummary")
             .arr.join(", ")
             .str.replace(r"null", "")
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
+
 def convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
-    ) 
-    conv = src["charges"].filter(  # filter convictions
-        pl.col("Conviction")
-    ) 
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
+    )
+    conv = src["charges"].filter(pl.col("Conviction"))  # filter convictions
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(conv, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("CaseNumber"),
             pl.col("Alias"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("TypeDescription"),
             pl.col("CourtAction"),
             pl.col("CERVDisqConviction"),
             pl.col("PardonDisqConviction"),
             pl.col("PermanentDisqConviction"),
@@ -1192,24 +1206,32 @@
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("ChargesSummary").arr.lengths().alias("ConvictionCount"),
             pl.col("CERVDisqConviction")
             .arr.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
             .arr.count_match(True)
             .alias("PardonConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("MISDEMEANOR").alias("MisdemeanorConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("FELONY").alias("FelonyConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("TRAFFIC").alias("TrafficConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("MISDEMEANOR")
+            .alias("MisdemeanorConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("FELONY")
+            .alias("FelonyConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("TRAFFIC")
+            .alias("TrafficConvictionCount"),
             pl.col("CourtAction").arr.count_match("GUILTY").alias("GuiltyPleaCount"),
             pl.col("PermanentDisqConviction")
             .arr.count_match(True)
             .alias("PermanentConvictionCount"),
             pl.col("TotalBalance").arr.sum(),
             pl.col("PaymentToRestore").arr.sum(),
             pl.col("ChargesSummary")
@@ -1218,48 +1240,51 @@
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
+
 def vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
-    summary = (   # pair AIS to cases sheet
+    summary = (  # pair AIS to cases sheet
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
     )
     disq = src["charges"].filter(  # filter disqualifying convictions
         pl.col("CERVDisqConviction")
         | pl.col("PardonDisqConviction")
         | pl.col("PermanentDisqConviction")
-    ) 
+    )
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(disq, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("CaseNumber"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("Alias"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("CERVDisqConviction"),
             pl.col("PardonDisqConviction"),
             pl.col("PermanentDisqConviction"),
             pl.col("TotalBalance"),
@@ -1267,14 +1292,16 @@
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CERVDisqConviction")
             .arr.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
             .arr.count_match(True)
             .alias("PardonConvictionCount"),
             pl.col("PermanentDisqConviction")
@@ -1341,16 +1368,22 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("RE_Charges")
             .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
             .str.strip()
             .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWTotalBalance")).alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWD999")).alias("TotalD999"),
+            pl.when(pl.col("RAWTotalBalance").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWTotalBalance"))
+            .alias("TotalBalance"),
+            pl.when(pl.col("RAWD999").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWD999"))
+            .alias("TotalD999"),
         ]
     )
 
     dlog(all_charges, all_charges.columns, cf=debug)
     return all_charges
 
 
@@ -1926,16 +1959,22 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("RE_Charges")
             .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
             .str.strip()
             .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWTotalBalance")).alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWD999")).alias("TotalD999"),
+            pl.when(pl.col("RAWTotalBalance").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWTotalBalance"))
+            .alias("TotalBalance"),
+            pl.when(pl.col("RAWD999").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWD999"))
+            .alias("TotalD999"),
         ]
     )
 
     # clean Fees strings
     # explode Fees for table parsing
     all_fees = cases.explode("RE_Fees").select(
         [
@@ -2184,18 +2223,22 @@
                 "CASENONUM"
             ),
         ]
     )
     charges = charges.with_columns(
         [
             pl.col("TotalBalance"),
-            pl.when(pl.col("CERVDisqConviction") | pl.col("PardonDisqConviction") | pl.col("PermanentDisqConviction"))
+            pl.when(
+                pl.col("CERVDisqConviction")
+                | pl.col("PardonDisqConviction")
+                | pl.col("PermanentDisqConviction")
+            )
             .then((pl.col("TotalBalance") - pl.col("TotalD999")))
             .otherwise(None)
-            .alias("PaymentToRestore")
+            .alias("PaymentToRestore"),
         ]
     )
     aggch = charges.groupby("CASENONUM").agg("CaseNumber", "RAWCITE", "RAWDESC")
     aggch = aggch.select(
         [
             pl.col("CASENONUM"),
             pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
@@ -3127,16 +3170,16 @@
             "Default 12",
             True,
             [480, 510],
         )
     elif "Windows" in (plat, psys):  # set Windows element sizes
         HEADER_FONT, LOGO_FONT, ASCII_FONT, BODY_FONT, WINDOW_RESIZE, WINDOW_SIZE = (
             "Default 14",
-            "Courier 12",
             "Courier 13",
+            "Courier 11",
             "Default 10",
             True,
             [500, 540],
         )
         try:
             from ctypes import windll
 
@@ -3148,15 +3191,15 @@
             "Default 15",
             "Courier 12",
             "Courier 13",
             "Default 10",
             True,
             [540, 540],
         )
-    sg.theme("DarkBlack")
+    sg.theme("Black")
     sg.set_options(font=BODY_FONT)
     fetch_layout = [
         [
             sg.Text(
                 """Collect case PDFs in bulk from Alacourt.com.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
@@ -3324,69 +3367,74 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]  # "AA"
-    vrr_layout = [
+    sum_layout = [
         [
             sg.Text(
-                """Pair cases by AIS number to create\na voting rights status summary.""",
+                """Pair cases by AIS number to create a\npaired summary table.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To make a voting rights status summary table, start by creating an\nAIS / Unique ID pair template, fill the template with AIS numbers or\nanother identifier to match names in common, then enter the\ntemplate path and case input path below.""",
+                """To make a charges summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another\nidentifier to match names in common, then enter the template path and\ncase input path below.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[31, 10],
-                key="VRR-INPUTPATH",
+                key="SUM-INPUTPATH",
                 focus=True,
             ),
             sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
         ],
         [
             sg.Text("Pairs: "),
             sg.InputText(
                 tooltip="Destination full text archive (.parquet, .json, .csv)",
                 size=[32, 10],
-                key="VRR-PAIRS",
+                key="SUM-PAIRS",
             ),
             sg.Button(
                 button_text="Make Template", button_color=("white", "black"), key="MT"
             ),
         ],
         [
             sg.Text("Output Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[40, 10],
-                key="VRR-OUTPUTPATH",
+                key="SUM-OUTPUTPATH",
                 focus=True,
             ),
         ],
         [
+            sg.Radio("Charges", "SUMMARY", key="SUM-CH", default=True),
+            sg.Radio("Convictions", "SUMMARY", key="SUM-CONV", default=False),
+            sg.Radio("Voting Rights", "SUMMARY", key="SUM-VRR", default=False),
+        ],
+        [
             sg.Button(
                 "Create Summary",
-                key="VRR",
+                key="SUM",
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
-    ]  # VRR
+    ]  # "SUM"
     table_layout = [
         [
             sg.Text(
                 """Export data tables from a case archive\nor PDF directory.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
@@ -3478,15 +3526,15 @@
         size=[0, 0],
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
-            [sg.Tab("voting", layout=vrr_layout, pad=(2, 2))],
+            [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(fshort_name, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -3535,15 +3583,15 @@
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
-            window["VRR"].update(disabled=False)
+            window["SUM"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -3553,42 +3601,43 @@
                     sg.popup("Alacorder created query template.")
                 else:
                     sg.popup(
                         "Enter valid path with .xlsx extension in Input Path box and try again."
                     )
         elif event == "MT":
             cf = set(
-                window["VRR-INPUTPATH"].get(),
-                window["VRR-PAIRS"].get(),
-                pairs=window["VRR-PAIRS"].get(),
-                vrr=False,
+                window["SUM-INPUTPATH"].get(),
+                window["SUM-PAIRS"].get(),
+                pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
                 debug=False,
                 overwrite=True,
                 window=window,
             )
             threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
-        elif event == "VRR":
+        elif event == "SUM":
             cf = set(
-                window["VRR-INPUTPATH"].get(),
-                window["VRR-OUTPUTPATH"].get(),
-                pairs=window["VRR-PAIRS"].get(),
-                vrr=True,
+                window["SUM-INPUTPATH"].get(),
+                window["SUM-OUTPUTPATH"].get(),
+                pairs=window["SUM-PAIRS"].get(),
+                vrr_summary=window["SUM-VRR"].get(),
+                charges_summary=window["SUM-CH"].get(),
+                convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
                 debug=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
-            threading.Thread(target=vrr, args=[cf], daemon=True).start()
-            window["VRR"].update(disabled=True)
+            threading.Thread(target=init, args=[cf], daemon=True).start()
+            window["SUM"].update(disabled=True)
         elif event == "POPUP":
             sg.popup(values["POPUP"])
         elif event == "TB":
             table = ""
             table = "all" if window["TB-ALL"].get() else table
             table = "charges" if window["TB-CHARGES"].get() else table
             table = "fees" if window["TB-FEES"].get() else table
@@ -4095,26 +4144,25 @@
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
-        vrr_summary=False,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     p = pairs(conf)
     print("Created pair template at output path.")
     return p
 
 
 @main.command(
-    name="vrr", help="Create voting rights summary from input cases and pairs"
+    name="vrr-pairs", help="Create voting rights summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
     required=True,
     type=click.Path(),
@@ -4154,14 +4202,15 @@
         vrr_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return vrr(conf)
 
+
 @main.command(
     name="charge-pairs", help="Create charges summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
@@ -4203,14 +4252,15 @@
         charges_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return charges_summary(conf)
 
+
 @main.command(
     name="conv-pairs", help="Create convictions summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
@@ -4252,14 +4302,15 @@
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return convictions_summary(conf)
 
+
 def extract_text(path) -> str:
     """
     From path, return full text of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
```

### Comparing `alacorder-79.8.8/src/alacorder/alac.py` & `alacorder-79.8.9/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     selenium = ^4.8.3
     tqdm = ^4.65.0
     xlsx2csv = ^0.8.1
     XlsxWriter = ^3.0.9
 """
 
 name = "ALACORDER"
-version = "79.8.8"
+version = "79.8.9"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
@@ -144,30 +144,14 @@
     if cf["LOG"]:
         print("Created template successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("MT-COMPLETE", True)
     return tp
 
 
-def vrr(cf):
-    """
-    Summarize voting rights status from pairs using configuration object `cf`.
-    """
-    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
-    if not cf["NO_WRITE"]:
-        write(
-            vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
-        )
-    if cf["LOG"]:
-        print("Created table successfully.")
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
-    return vr
-
-
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
     plog("Extracting case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
@@ -319,49 +303,73 @@
     if not cf["NO_WRITE"]:
         write(out, sheet_names=["images"], cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
+def vrr_summary(cf):
+    """
+    Summarize voting rights status from pairs using configuration object `cf`.
+    """
+    vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
+    if not cf["NO_WRITE"]:
+        write(
+            vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+        )
+    if cf["LOG"]:
+        print("Created table successfully.")
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
+    return vr
+
+
 def case_action_summary(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
     q = read(cf["QUEUE"])
     out = explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         write(out, sheet_names=["case-action-summary"], cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
+
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf['DEBUG'])
+    ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         write(
-            ch, sheet_names=["ChargesSummary"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+            ch,
+            sheet_names=["ChargesSummary"],
+            path=cf["OUTPUT_PATH"],
+            overwrite=cf["OVERWRITE"],
         )
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
+
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
-    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf['DEBUG'])
+    conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         write(
-            conv, sheet_names=["ConvictionsSummary"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+            conv,
+            sheet_names=["ConvictionsSummary"],
+            path=cf["OUTPUT_PATH"],
+            overwrite=cf["OVERWRITE"],
         )
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
@@ -373,15 +381,15 @@
     if cf["FETCH"] == True:
         ft = fetch(cf=cf)
         return ft
     elif cf["ARCHIVE"] == True:
         ar = archive(cf)
         return ar
     elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
-        vr = vrr(cf)
+        vr = vrr_summary(cf)
         return vr
     elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
         ch = charges_summary(cf)
         return ch
     elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
         conv = convictions_summary(cf)
         return cf
@@ -1074,116 +1082,122 @@
                 pl.col("CaseNumber").arr.join(", ").alias("Cases"),
             ]
         )
     )
     names = names.sort("Name")
     return names
 
+
 def charges_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
-    ) 
-    ch = src["charges"].filter(  # filter convictions
-        pl.col("Filing")
-    ) 
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
+    )
+    ch = src["charges"].filter(pl.col("Filing"))  # filter convictions
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(ch, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("CaseNumber"),
             pl.col("Alias"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("TypeDescription"),
             pl.col("CERVDisqCharge"),
             pl.col("PardonDisqCharge"),
-            pl.col("PermanentDisqCharge")
+            pl.col("PermanentDisqCharge"),
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("ChargesSummary").arr.lengths().alias("ChargeCount"),
-            pl.col("CERVDisqCharge")
-            .arr.count_match(True)
-            .alias("CERVChargeCount"),
-            pl.col("PardonDisqCharge")
-            .arr.count_match(True)
-            .alias("PardonChargeCount"),
-            pl.col("TypeDescription").arr.count_match("MISDEMEANOR").alias("MisdemeanorChargeCount"),
-            pl.col("TypeDescription").arr.count_match("FELONY").alias("FelonyChargeCount"),
-            pl.col("TypeDescription").arr.count_match("TRAFFIC").alias("TrafficChargeCount"),
+            pl.col("CERVDisqCharge").arr.count_match(True).alias("CERVChargeCount"),
+            pl.col("PardonDisqCharge").arr.count_match(True).alias("PardonChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("MISDEMEANOR")
+            .alias("MisdemeanorChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("FELONY")
+            .alias("FelonyChargeCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("TRAFFIC")
+            .alias("TrafficChargeCount"),
             pl.col("PermanentDisqCharge")
             .arr.count_match(True)
             .alias("PermanentChargeCount"),
             pl.col("ChargesSummary")
             .arr.join(", ")
             .str.replace(r"null", "")
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
+
 def convictions_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
     summary = (
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
-    ) 
-    conv = src["charges"].filter(  # filter convictions
-        pl.col("Conviction")
-    ) 
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
+    )
+    conv = src["charges"].filter(pl.col("Conviction"))  # filter convictions
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(conv, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("CaseNumber"),
             pl.col("Alias"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("TypeDescription"),
             pl.col("CourtAction"),
             pl.col("CERVDisqConviction"),
             pl.col("PardonDisqConviction"),
             pl.col("PermanentDisqConviction"),
@@ -1192,24 +1206,32 @@
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("ChargesSummary").arr.lengths().alias("ConvictionCount"),
             pl.col("CERVDisqConviction")
             .arr.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
             .arr.count_match(True)
             .alias("PardonConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("MISDEMEANOR").alias("MisdemeanorConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("FELONY").alias("FelonyConvictionCount"),
-            pl.col("TypeDescription").arr.count_match("TRAFFIC").alias("TrafficConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("MISDEMEANOR")
+            .alias("MisdemeanorConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("FELONY")
+            .alias("FelonyConvictionCount"),
+            pl.col("TypeDescription")
+            .arr.count_match("TRAFFIC")
+            .alias("TrafficConvictionCount"),
             pl.col("CourtAction").arr.count_match("GUILTY").alias("GuiltyPleaCount"),
             pl.col("PermanentDisqConviction")
             .arr.count_match(True)
             .alias("PermanentConvictionCount"),
             pl.col("TotalBalance").arr.sum(),
             pl.col("PaymentToRestore").arr.sum(),
             pl.col("ChargesSummary")
@@ -1218,48 +1240,51 @@
             .alias("ChargesSummary"),
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
+
 def vrr_summary_from_pairs(src, pairs, debug=False):
     if isinstance(src, str):
         arc = read(src)
         src = cf(arc, table="all", no_write=True, now=True)
     if isinstance(pairs, str):
         pairs = read(pairs)
-    summary = (   # pair AIS to cases sheet
+    summary = (  # pair AIS to cases sheet
         src["cases"]
         .join(pairs, on="Name", how="inner")
         .groupby("AIS / Unique ID")
-        .agg(
-            "Name", "Alias", "DOB", "CaseNumber"
-        )
+        .agg("Name", "Alias", "DOB", "CaseNumber", "Race", "Sex")
     )
     disq = src["charges"].filter(  # filter disqualifying convictions
         pl.col("CERVDisqConviction")
         | pl.col("PardonDisqConviction")
         | pl.col("PermanentDisqConviction")
-    ) 
+    )
     summary = summary.select(  # prepare summary for join w/ convictions
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.get(0).alias("Name"),
             pl.col("Alias").arr.get(0).alias("Alias"),
             pl.col("DOB").arr.get(0),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CaseNumber").arr.join(", "),
         ]
     )
     summary = summary.join(disq, on="Name", how="outer")  # join cases, convictions
     summary = summary.groupby("Name").agg(
         [
             pl.col("AIS / Unique ID"),
             pl.col("DOB"),
             pl.col("CaseNumber"),
+            pl.col("Race"),
+            pl.col("Sex"),
             pl.col("Alias"),
             pl.col("Cite"),
             pl.col("ChargesSummary"),
             pl.col("CERVDisqConviction"),
             pl.col("PardonDisqConviction"),
             pl.col("PermanentDisqConviction"),
             pl.col("TotalBalance"),
@@ -1267,14 +1292,16 @@
         ]
     )
     summary = summary.select(
         [
             pl.col("AIS / Unique ID").arr.get(0).cast(pl.Utf8).alias("AIS / Unique ID"),
             pl.col("Name"),
             pl.col("DOB").arr.get(0).alias("DOB"),
+            pl.col("Race").arr.get(0),
+            pl.col("Sex").arr.get(0),
             pl.col("CERVDisqConviction")
             .arr.count_match(True)
             .alias("CERVConvictionCount"),
             pl.col("PardonDisqConviction")
             .arr.count_match(True)
             .alias("PardonConvictionCount"),
             pl.col("PermanentDisqConviction")
@@ -1341,16 +1368,22 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("RE_Charges")
             .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
             .str.strip()
             .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWTotalBalance")).alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWD999")).alias("TotalD999"),
+            pl.when(pl.col("RAWTotalBalance").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWTotalBalance"))
+            .alias("TotalBalance"),
+            pl.when(pl.col("RAWD999").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWD999"))
+            .alias("TotalD999"),
         ]
     )
 
     dlog(all_charges, all_charges.columns, cf=debug)
     return all_charges
 
 
@@ -1926,16 +1959,22 @@
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("RE_Charges")
             .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
             .str.strip()
             .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWTotalBalance")).alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null()).then(pl.lit(0.0)).otherwise(pl.col("RAWD999")).alias("TotalD999"),
+            pl.when(pl.col("RAWTotalBalance").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWTotalBalance"))
+            .alias("TotalBalance"),
+            pl.when(pl.col("RAWD999").is_null())
+            .then(pl.lit(0.0))
+            .otherwise(pl.col("RAWD999"))
+            .alias("TotalD999"),
         ]
     )
 
     # clean Fees strings
     # explode Fees for table parsing
     all_fees = cases.explode("RE_Fees").select(
         [
@@ -2184,18 +2223,22 @@
                 "CASENONUM"
             ),
         ]
     )
     charges = charges.with_columns(
         [
             pl.col("TotalBalance"),
-            pl.when(pl.col("CERVDisqConviction") | pl.col("PardonDisqConviction") | pl.col("PermanentDisqConviction"))
+            pl.when(
+                pl.col("CERVDisqConviction")
+                | pl.col("PardonDisqConviction")
+                | pl.col("PermanentDisqConviction")
+            )
             .then((pl.col("TotalBalance") - pl.col("TotalD999")))
             .otherwise(None)
-            .alias("PaymentToRestore")
+            .alias("PaymentToRestore"),
         ]
     )
     aggch = charges.groupby("CASENONUM").agg("CaseNumber", "RAWCITE", "RAWDESC")
     aggch = aggch.select(
         [
             pl.col("CASENONUM"),
             pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
@@ -3127,16 +3170,16 @@
             "Default 12",
             True,
             [480, 510],
         )
     elif "Windows" in (plat, psys):  # set Windows element sizes
         HEADER_FONT, LOGO_FONT, ASCII_FONT, BODY_FONT, WINDOW_RESIZE, WINDOW_SIZE = (
             "Default 14",
-            "Courier 12",
             "Courier 13",
+            "Courier 11",
             "Default 10",
             True,
             [500, 540],
         )
         try:
             from ctypes import windll
 
@@ -3148,15 +3191,15 @@
             "Default 15",
             "Courier 12",
             "Courier 13",
             "Default 10",
             True,
             [540, 540],
         )
-    sg.theme("DarkBlack")
+    sg.theme("Black")
     sg.set_options(font=BODY_FONT)
     fetch_layout = [
         [
             sg.Text(
                 """Collect case PDFs in bulk from Alacourt.com.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
@@ -3324,69 +3367,74 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]  # "AA"
-    vrr_layout = [
+    sum_layout = [
         [
             sg.Text(
-                """Pair cases by AIS number to create\na voting rights status summary.""",
+                """Pair cases by AIS number to create a\npaired summary table.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To make a voting rights status summary table, start by creating an\nAIS / Unique ID pair template, fill the template with AIS numbers or\nanother identifier to match names in common, then enter the\ntemplate path and case input path below.""",
+                """To make a charges summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another\nidentifier to match names in common, then enter the template path and\ncase input path below.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[31, 10],
-                key="VRR-INPUTPATH",
+                key="SUM-INPUTPATH",
                 focus=True,
             ),
             sg.FileBrowse(button_text="Select File", button_color=("white", "black")),
         ],
         [
             sg.Text("Pairs: "),
             sg.InputText(
                 tooltip="Destination full text archive (.parquet, .json, .csv)",
                 size=[32, 10],
-                key="VRR-PAIRS",
+                key="SUM-PAIRS",
             ),
             sg.Button(
                 button_text="Make Template", button_color=("white", "black"), key="MT"
             ),
         ],
         [
             sg.Text("Output Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[40, 10],
-                key="VRR-OUTPUTPATH",
+                key="SUM-OUTPUTPATH",
                 focus=True,
             ),
         ],
         [
+            sg.Radio("Charges", "SUMMARY", key="SUM-CH", default=True),
+            sg.Radio("Convictions", "SUMMARY", key="SUM-CONV", default=False),
+            sg.Radio("Voting Rights", "SUMMARY", key="SUM-VRR", default=False),
+        ],
+        [
             sg.Button(
                 "Create Summary",
-                key="VRR",
+                key="SUM",
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
-    ]  # VRR
+    ]  # "SUM"
     table_layout = [
         [
             sg.Text(
                 """Export data tables from a case archive\nor PDF directory.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
@@ -3478,15 +3526,15 @@
         size=[0, 0],
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
-            [sg.Tab("voting", layout=vrr_layout, pad=(2, 2))],
+            [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(fshort_name, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -3535,15 +3583,15 @@
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
-            window["VRR"].update(disabled=False)
+            window["SUM"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -3553,42 +3601,43 @@
                     sg.popup("Alacorder created query template.")
                 else:
                     sg.popup(
                         "Enter valid path with .xlsx extension in Input Path box and try again."
                     )
         elif event == "MT":
             cf = set(
-                window["VRR-INPUTPATH"].get(),
-                window["VRR-PAIRS"].get(),
-                pairs=window["VRR-PAIRS"].get(),
-                vrr=False,
+                window["SUM-INPUTPATH"].get(),
+                window["SUM-PAIRS"].get(),
+                pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
                 debug=False,
                 overwrite=True,
                 window=window,
             )
             threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
-        elif event == "VRR":
+        elif event == "SUM":
             cf = set(
-                window["VRR-INPUTPATH"].get(),
-                window["VRR-OUTPUTPATH"].get(),
-                pairs=window["VRR-PAIRS"].get(),
-                vrr=True,
+                window["SUM-INPUTPATH"].get(),
+                window["SUM-OUTPUTPATH"].get(),
+                pairs=window["SUM-PAIRS"].get(),
+                vrr_summary=window["SUM-VRR"].get(),
+                charges_summary=window["SUM-CH"].get(),
+                convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
                 debug=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
-            threading.Thread(target=vrr, args=[cf], daemon=True).start()
-            window["VRR"].update(disabled=True)
+            threading.Thread(target=init, args=[cf], daemon=True).start()
+            window["SUM"].update(disabled=True)
         elif event == "POPUP":
             sg.popup(values["POPUP"])
         elif event == "TB":
             table = ""
             table = "all" if window["TB-ALL"].get() else table
             table = "charges" if window["TB-CHARGES"].get() else table
             table = "fees" if window["TB-FEES"].get() else table
@@ -4095,26 +4144,25 @@
 @click.option(
     "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
-        vrr_summary=False,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     p = pairs(conf)
     print("Created pair template at output path.")
     return p
 
 
 @main.command(
-    name="vrr", help="Create voting rights summary from input cases and pairs"
+    name="vrr-pairs", help="Create voting rights summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
     required=True,
     type=click.Path(),
@@ -4154,14 +4202,15 @@
         vrr_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return vrr(conf)
 
+
 @main.command(
     name="charge-pairs", help="Create charges summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
@@ -4203,14 +4252,15 @@
         charges_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return charges_summary(conf)
 
+
 @main.command(
     name="conv-pairs", help="Create convictions summary from input cases and pairs"
 )
 @click.option(
     "--input-path",
     "-in",
     "input_path",
@@ -4252,14 +4302,15 @@
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return convictions_summary(conf)
 
+
 def extract_text(path) -> str:
     """
     From path, return full text of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
```

### Comparing `alacorder-79.8.8/PKG-INFO` & `alacorder-79.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.8.8
+Version: 79.8.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

