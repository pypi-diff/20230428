# Comparing `tmp/alacorder-79.8.9.tar.gz` & `tmp/alacorder-79.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.8.9.tar", max compression
+gzip compressed data, was "alacorder-79.9.0.tar", max compression
```

## Comparing `alacorder-79.8.9.tar` & `alacorder-79.9.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.8.9/LICENSE
--rw-r--r--   0        0        0     9801 2023-04-27 23:24:11.886024 alacorder-79.8.9/README.md
--rw-r--r--   0        0        0      697 2023-04-28 01:12:26.214336 alacorder-79.8.9/pyproject.toml
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.8.9/src/alacorder/.python-version
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.8.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   167384 2023-04-28 01:11:07.717891 alacorder-79.8.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   167384 2023-04-28 01:10:59.052060 alacorder-79.8.9/src/alacorder/alac.py
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.8.9/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 alacorder-79.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.9.0/LICENSE
+-rw-r--r--   0        0        0     9801 2023-04-27 23:24:11.886024 alacorder-79.9.0/README.md
+-rw-r--r--   0        0        0      697 2023-04-28 21:55:02.900566 alacorder-79.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-28 21:53:41.054817 alacorder-79.9.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-79.9.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   190051 2023-04-28 21:52:54.246441 alacorder-79.9.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   190051 2023-04-28 21:52:41.293491 alacorder-79.9.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 alacorder-79.9.0/PKG-INFO
```

### Comparing `alacorder-79.8.9/LICENSE` & `alacorder-79.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.9/README.md` & `alacorder-79.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.9/pyproject.toml` & `alacorder-79.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.8.9"
+version = "79.9.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.8.9/src/alacorder/__init__.py` & `alacorder-79.9.0/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.8.9/src/alacorder/__main__.py` & `alacorder-79.9.0/src/alacorder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
- ALACORDER 79
- ┌─┐┌─┐┬─┐┌┬┐┬ ┬┌┬┐┌─┐┬ ┬┌┐┌┌┬┐┌─┐┬┌┐┌
- ├─┘├─┤├┬┘ │ └┬┘││││ ││ ││││ │ ├─┤││││
- ┴  ┴ ┴┴└─ ┴  ┴ ┴ ┴└─┘└─┘┘└┘ ┴ ┴ ┴┴┘└┘
- (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
+ALACORDER --------------------
+╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
+╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
+╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
+(c) 2023 Sam Robson ----------
 
  Dependencies: 
-    python = ^3.9
-    brotli = ^1.0.9
-    click = ^8.1.3
-    polars = ^0.17.6
-    PyMuPDF = ^1.21.1
-    PySimpleGUI = ^4.60.4
-    selenium = ^4.8.3
-    tqdm = ^4.65.0
-    xlsx2csv = ^0.8.1
-    XlsxWriter = ^3.0.9
+    python 3.9 - 3.11
+    brotli 1.0.9
+    click 8.1.3
+    polars 0.17.6
+    PyMuPDF 1.21.1
+    PySimpleGUI 4.60.4
+    selenium 4.8.3
+    tqdm 4.65.0
+    xlsx2csv 0.8.1
+    XlsxWriter 3.0.9
 """
 
 name = "ALACORDER"
-version = "79.8.9"
-long_version = "partymountain"
+long_version = "snowpalace"
+version = "79.9.0"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -127,31 +127,14 @@
     else:
         print(message)
 
 
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
-def pairs(cf):
-    """
-    Create AIS / Unique ID pairs template using configuration object `cf`.
-    """
-    df = read(cf)
-    tp = make_pairs_template(df)
-    if not cf["NO_WRITE"]:
-        write(
-            tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
-        )
-    if cf["LOG"]:
-        print("Created template successfully.")
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("MT-COMPLETE", True)
-    return tp
-
-
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
     plog("Extracting case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
@@ -171,15 +154,15 @@
     img = explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(
             [ca, ch_filing, ch_disposition, fs, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
                 "disposition-charges",
                 "fees",
@@ -212,245 +195,206 @@
     """
     Start cases table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df)
     if not cf["NO_WRITE"]:
-        print("Writing to export...")
+        print("Writing to output path...")
         write(ca, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ca
 
 
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
 
 
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
 
 
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing witnesses...", cf=cf)
     out = explode_witnesses(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
+        print("Completed table export.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
+    return out
+
+
+def cas(cf):
+    """
+    Collect case action summaries using configuration object `cf`.
+    """
+    print("Parsing case action summaries...", cf=cf)
+    q = read(cf["QUEUE"])
+    out = explode_case_action_summary(q)
+    if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
+        write(out, sheet_names=["case-action-summary"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing attorneys...", cf=cf)
     out = explode_attorneys(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
     out = explode_settings(q)
+    print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing images...", cf=cf)
     out = explode_images(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf)
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
-
-def case_action_summary(cf):
-    """
-    Collect case action summaries using configuration object `cf`.
-    """
-    q = read(cf["QUEUE"])
-    out = explode_case_action_summary(q)
-    if not cf["NO_WRITE"]:
-        write(out, sheet_names=["case-action-summary"], cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
     conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-def init(cf):
-    """
-    Start Alacorder using configuration object `cf`.
-    """
-    if cf["FETCH"] == True:
-        ft = fetch(cf=cf)
-        return ft
-    elif cf["ARCHIVE"] == True:
-        ar = archive(cf)
-        return ar
-    elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
-        vr = vrr_summary(cf)
-        return vr
-    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
-        ch = charges_summary(cf)
-        return ch
-    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
-        conv = convictions_summary(cf)
-        return cf
-    elif (
-        cf["TABLE"].lower() in ("charges", "disposition", "filing")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        ch = charges(cf)
-        return ch
-    elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
-        ca = cases(cf)
-        return ca
-    elif (
-        cf["TABLE"].lower() in ("fees", "feesheet", "fines")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        fs = fees(cf)
-        return fs
-    elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
-        out = witnesses(cf)
-        return out
-    elif (
-        cf["TABLE"].lower()
-        in (
-            "case-action-summary",
-            "cas",
-        )
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        out = case_action_summary(cf)
-        return out
-    elif cf["TABLE"].lower() in ("settings", "set") and cf["SUPPORT_SINGLETABLE"]:
-        out = settings(cf)
-        return out
-    elif cf["TABLE"].lower() in ("images", "imgs", "img") and cf["SUPPORT_SINGLETABLE"]:
-        out = images(cf)
-        return out
-    elif cf["TABLE"] in ("attorneys", "att") and cf["SUPPORT_SINGLETABLE"]:
-        out = attorneys(cf)
-        return out
-    elif (
-        cf["TABLE"].lower() in ("all", "", "multi", "multitable")
-        and cf["SUPPORT_MULTITABLE"]
-    ):
-        mult = multi(cf)
-        return mult
-    else:
-        print("Job not specified. Select a mode and reconfigure to start.")
-        return None
-
-
 def archive(cf):
     """
     Write a full text archive from inputs using configuration `cf`.
     """
+    print("Extracting text...", cf=cf)
     a = read(cf)
     write(a, cf=cf)
+    print("Completed archive export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
@@ -905,14 +849,21 @@
             if "AllPagesText" in archive.columns:
                 archive = archive.with_columns(
                     pl.col("AllPagesText")
                     .str.replace_all(r"\n", " ")
                     .alias("AllPagesTextNoNewLine")
                 )
             return archive
+        elif ext == ".txt":
+            with open(cf) as f:
+                text = f.read()
+            return text
+        elif ext == ".pdf":
+            text = extract_text(cf)
+            return text
     else:
         return None
 
 
 def write(outputs, sheet_names=[], cf=None, path=None, overwrite=False):
     """Write `outputs` to output path at `cf['OUTPUT_PATH']` or `path`.
 
@@ -978,15 +929,120 @@
     elif cf["OUTPUT_EXT"] not in ("none", "", "directory", None):
         outputs.write_csv(cf["OUTPUT_PATH"])
     else:
         pass
     return outputs
 
 
-#   #   #   #           TABLE PARSERS           #   #   #   #
+def pairs(cf):
+    """
+    Create AIS / Unique ID pairs template using configuration object `cf`.
+    """
+    print("Creating empty pairs template...", cf=cf)
+    df = read(cf)
+    tp = make_pairs_template(df)
+    if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
+        write(
+            tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+        )
+    print("Created template successfully.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("MT-COMPLETE", True)
+    return tp
+
+
+def init(cf):
+    """
+    Start Alacorder using configuration object `cf`.
+    """
+    if cf["FETCH"] == True:
+        ft = fetch(cf=cf)
+        return ft
+    elif cf["ARCHIVE"] == True:
+        ar = archive(cf)
+        return ar
+    elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
+        vr = vrr_summary(cf)
+        return vr
+    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
+        ch = charges_summary(cf)
+        return ch
+    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
+        conv = convictions_summary(cf)
+        return cf
+    elif (
+        cf["TABLE"].lower() in ("charges", "disposition", "filing")
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        ch = charges(cf)
+        return ch
+    elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
+        ca = cases(cf)
+        return ca
+    elif (
+        cf["TABLE"].lower() in ("fees", "feesheet", "fines")
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        fs = fees(cf)
+        return fs
+    elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
+        out = witnesses(cf)
+        return out
+    elif (
+        cf["TABLE"].lower()
+        in (
+            "case-action-summary",
+            "cas",
+        )
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        out = cas(cf)
+        return out
+    elif cf["TABLE"].lower() in ("settings", "set") and cf["SUPPORT_SINGLETABLE"]:
+        out = settings(cf)
+        return out
+    elif cf["TABLE"].lower() in ("images", "imgs", "img") and cf["SUPPORT_SINGLETABLE"]:
+        out = images(cf)
+        return out
+    elif cf["TABLE"] in ("attorneys", "att") and cf["SUPPORT_SINGLETABLE"]:
+        out = attorneys(cf)
+        return out
+    elif (
+        cf["TABLE"].lower() in ("all", "", "multi", "multitable")
+        and cf["SUPPORT_MULTITABLE"]
+    ):
+        mult = multi(cf)
+        return mult
+    else:
+        print("Job not specified. Select a mode and reconfigure to start.")
+        return None
+
+
+#   #   #   #        PRIVATE / INTERNALS         #   #   #   #
+
+
+def extract_text(path) -> str:
+    """
+    From path, return full text of PDF as string (PyMuPdf engine required!)
+    """
+    try:
+        doc = fitz.open(path)
+    except:
+        return ""
+    text = ""
+    for pg in doc:
+        try:
+            text += " \n ".join(
+                x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
+            )
+        except:
+            pass
+    text = re.sub(r"(<image\:.+?>)", "", text).strip()
+    return text
 
 
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
@@ -2058,15 +2114,14 @@
         "AdminUpdatedBy",
         "TransferDesc",
         "TBNV1",
         "TBNV2",
         "DriverLicenseNo",
         "StateID",
     )
-    cases = cases.sort("CaseNumber")
     return cases, all_charges, all_fees
 
 
 def split_charges(df, debug=False):
     dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
     charges = df.with_columns(
         [
@@ -2295,17 +2350,15 @@
         "PermanentDisqConviction",
         "Filing",
         "Disposition",
         "TotalBalance",
         "PaymentToRestore",
         "ChargesSummary",
     )
-    charges = charges.sort("CaseNumber")
     dlog(charges.columns, charges.shape, cf=debug)
-
     return charges
 
 
 def split_fees(df, debug=False):
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
@@ -3606,15 +3659,14 @@
         elif event == "MT":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
-                debug=False,
                 overwrite=True,
                 window=window,
             )
             threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
@@ -3623,15 +3675,14 @@
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=window["SUM-VRR"].get(),
                 charges_summary=window["SUM-CH"].get(),
                 convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
-                debug=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
             threading.Thread(target=init, args=[cf], daemon=True).start()
             window["SUM"].update(disabled=True)
         elif event == "POPUP":
@@ -3658,15 +3709,14 @@
                     window["TB-INPUTPATH"].get(),
                     window["TB-OUTPUTPATH"].get(),
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
-                    debug=False,
                     archive=False,
                     window=window,
                 )
                 # except:
                 window["TB"].update(disabled=True)
                 threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
@@ -3897,20 +3947,19 @@
     "no_update",
     is_flag=True,
     default=False,
     help="Do not update query template after completion",
 )
 @click.option(
     "--debug",
-    "-d",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug=False):
+def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         listpath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
@@ -3974,15 +4023,15 @@
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print debug logs to console"
+    "--debug",  default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
     input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
@@ -4019,14 +4068,779 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+@main.command(name="multi", help="Export all data tables to .xls/.xlsx")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_multi(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write data tables to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx"):
+        error("File extension must be .xls or .xlsx for multitable export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="all",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = multi(cf)
+    return o
+
+
+@main.command(name="cases", help="Create and export case information table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_cases(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="cases",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+
+@main.command(name="charges", help="Create and export charges table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option("--filing", "-f", is_flag=True, default=False, help="Only export filing charges")
+@click.option("--disposition", is_flag=True, default=False, help="Only export disposition charges")
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_charges(
+    input_path, output_path, filing, disposition, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        filing (bool, optional): Only export filing charges
+        disposition (bool, optional): Only export disposition charges
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    table = "charges" if not filing and not disposition else ""
+    table = "filing" if filing else table
+    table = "disposition" if disposition else table
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table=table,
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="fees", help="Create and export fees table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_cases(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="fees",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="settings", help="Create and export settings table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_settings(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="settings",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="witnesses", help="Create and export witnesses table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_witnesses(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="witnesses",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="case-action-summary", help="Create and export case action summaries")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_case_action_summary(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="case-action-summary",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+
+@main.command(name="images", help="Create and export images table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_images(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="images",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="attorneys", help="Create and export attorneys table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_attorneys(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="attorneys",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
 
 @main.command(name="archive", help="Create full text archive from case PDFs")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
@@ -4070,15 +4884,15 @@
 @click.option(
     "--no-prompt",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def cli_archive(
     input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
 ):
@@ -4105,15 +4919,15 @@
         no_write=False,
         log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if debug:
         click.echo(cf)
-    o = archive(cf, debug=debug)
+    o = archive(cf)
     return o
 
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
 )
@@ -4138,15 +4952,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         debug=debug,
         overwrite=overwrite,
@@ -4188,15 +5002,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_vrr(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         vrr_summary=True,
@@ -4238,15 +5052,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         charges_summary=True,
@@ -4288,49 +5102,29 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return convictions_summary(conf)
 
 
-def extract_text(path) -> str:
-    """
-    From path, return full text of PDF as string (PyMuPdf engine required!)
-    """
-    try:
-        doc = fitz.open(path)
-    except:
-        return ""
-    text = ""
-    for pg in doc:
-        try:
-            text += " \n ".join(
-                x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
-            )
-        except:
-            pass
-    text = re.sub(r"(<image\:.+?>)", "", text).strip()
-    return text
-
-
 if __name__ == "__main__":
     main()
 
 #   #   #   #           GETTER METHODS         #   #   #   #
 
 
 def get_paths(dirpath):
```

### Comparing `alacorder-79.8.9/src/alacorder/alac.py` & `alacorder-79.9.0/src/alacorder/alac.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
- ALACORDER 79
- ┌─┐┌─┐┬─┐┌┬┐┬ ┬┌┬┐┌─┐┬ ┬┌┐┌┌┬┐┌─┐┬┌┐┌
- ├─┘├─┤├┬┘ │ └┬┘││││ ││ ││││ │ ├─┤││││
- ┴  ┴ ┴┴└─ ┴  ┴ ┴ ┴└─┘└─┘┘└┘ ┴ ┴ ┴┴┘└┘
- (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
+ALACORDER --------------------
+╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
+╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
+╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
+(c) 2023 Sam Robson ----------
 
  Dependencies: 
-    python = ^3.9
-    brotli = ^1.0.9
-    click = ^8.1.3
-    polars = ^0.17.6
-    PyMuPDF = ^1.21.1
-    PySimpleGUI = ^4.60.4
-    selenium = ^4.8.3
-    tqdm = ^4.65.0
-    xlsx2csv = ^0.8.1
-    XlsxWriter = ^3.0.9
+    python 3.9 - 3.11
+    brotli 1.0.9
+    click 8.1.3
+    polars 0.17.6
+    PyMuPDF 1.21.1
+    PySimpleGUI 4.60.4
+    selenium 4.8.3
+    tqdm 4.65.0
+    xlsx2csv 0.8.1
+    XlsxWriter 3.0.9
 """
 
 name = "ALACORDER"
-version = "79.8.9"
-long_version = "partymountain"
+long_version = "snowpalace"
+version = "79.9.0"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -127,31 +127,14 @@
     else:
         print(message)
 
 
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
-def pairs(cf):
-    """
-    Create AIS / Unique ID pairs template using configuration object `cf`.
-    """
-    df = read(cf)
-    tp = make_pairs_template(df)
-    if not cf["NO_WRITE"]:
-        write(
-            tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
-        )
-    if cf["LOG"]:
-        print("Created template successfully.")
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("MT-COMPLETE", True)
-    return tp
-
-
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     df = read(cf)
     plog("Extracting case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
@@ -171,15 +154,15 @@
     img = explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(
             [ca, ch_filing, ch_disposition, fs, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
                 "disposition-charges",
                 "fees",
@@ -212,245 +195,206 @@
     """
     Start cases table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df)
     if not cf["NO_WRITE"]:
-        print("Writing to export...")
+        print("Writing to output path...")
         write(ca, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ca
 
 
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
 
 
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
-        print("Writing to export...", cf=cf)
+        print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
 
 
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing witnesses...", cf=cf)
     out = explode_witnesses(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
+        print("Completed table export.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
+    return out
+
+
+def cas(cf):
+    """
+    Collect case action summaries using configuration object `cf`.
+    """
+    print("Parsing case action summaries...", cf=cf)
+    q = read(cf["QUEUE"])
+    out = explode_case_action_summary(q)
+    if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
+        write(out, sheet_names=["case-action-summary"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing attorneys...", cf=cf)
     out = explode_attorneys(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
     out = explode_settings(q)
+    print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
-    q = read(cf["QUEUE"])
+    q = read(cf)
+    print("Parsing images...", cf=cf)
     out = explode_images(q)
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
+        print("Completed table export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf)
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
-
-def case_action_summary(cf):
-    """
-    Collect case action summaries using configuration object `cf`.
-    """
-    q = read(cf["QUEUE"])
-    out = explode_case_action_summary(q)
-    if not cf["NO_WRITE"]:
-        write(out, sheet_names=["case-action-summary"], cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-TB", True)
-    return out
-
-
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
     conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
+        print("Completed table export.", cf=cf)
     if cf["LOG"]:
         print("Created table successfully.")
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-def init(cf):
-    """
-    Start Alacorder using configuration object `cf`.
-    """
-    if cf["FETCH"] == True:
-        ft = fetch(cf=cf)
-        return ft
-    elif cf["ARCHIVE"] == True:
-        ar = archive(cf)
-        return ar
-    elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
-        vr = vrr_summary(cf)
-        return vr
-    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
-        ch = charges_summary(cf)
-        return ch
-    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
-        conv = convictions_summary(cf)
-        return cf
-    elif (
-        cf["TABLE"].lower() in ("charges", "disposition", "filing")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        ch = charges(cf)
-        return ch
-    elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
-        ca = cases(cf)
-        return ca
-    elif (
-        cf["TABLE"].lower() in ("fees", "feesheet", "fines")
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        fs = fees(cf)
-        return fs
-    elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
-        out = witnesses(cf)
-        return out
-    elif (
-        cf["TABLE"].lower()
-        in (
-            "case-action-summary",
-            "cas",
-        )
-        and cf["SUPPORT_SINGLETABLE"]
-    ):
-        out = case_action_summary(cf)
-        return out
-    elif cf["TABLE"].lower() in ("settings", "set") and cf["SUPPORT_SINGLETABLE"]:
-        out = settings(cf)
-        return out
-    elif cf["TABLE"].lower() in ("images", "imgs", "img") and cf["SUPPORT_SINGLETABLE"]:
-        out = images(cf)
-        return out
-    elif cf["TABLE"] in ("attorneys", "att") and cf["SUPPORT_SINGLETABLE"]:
-        out = attorneys(cf)
-        return out
-    elif (
-        cf["TABLE"].lower() in ("all", "", "multi", "multitable")
-        and cf["SUPPORT_MULTITABLE"]
-    ):
-        mult = multi(cf)
-        return mult
-    else:
-        print("Job not specified. Select a mode and reconfigure to start.")
-        return None
-
-
 def archive(cf):
     """
     Write a full text archive from inputs using configuration `cf`.
     """
+    print("Extracting text...", cf=cf)
     a = read(cf)
     write(a, cf=cf)
+    print("Completed archive export.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
@@ -905,14 +849,21 @@
             if "AllPagesText" in archive.columns:
                 archive = archive.with_columns(
                     pl.col("AllPagesText")
                     .str.replace_all(r"\n", " ")
                     .alias("AllPagesTextNoNewLine")
                 )
             return archive
+        elif ext == ".txt":
+            with open(cf) as f:
+                text = f.read()
+            return text
+        elif ext == ".pdf":
+            text = extract_text(cf)
+            return text
     else:
         return None
 
 
 def write(outputs, sheet_names=[], cf=None, path=None, overwrite=False):
     """Write `outputs` to output path at `cf['OUTPUT_PATH']` or `path`.
 
@@ -978,15 +929,120 @@
     elif cf["OUTPUT_EXT"] not in ("none", "", "directory", None):
         outputs.write_csv(cf["OUTPUT_PATH"])
     else:
         pass
     return outputs
 
 
-#   #   #   #           TABLE PARSERS           #   #   #   #
+def pairs(cf):
+    """
+    Create AIS / Unique ID pairs template using configuration object `cf`.
+    """
+    print("Creating empty pairs template...", cf=cf)
+    df = read(cf)
+    tp = make_pairs_template(df)
+    if not cf["NO_WRITE"]:
+        print("Writing to output path...", cf=cf)
+        write(
+            tp, sheet_names=["Pairs"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
+        )
+    print("Created template successfully.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("MT-COMPLETE", True)
+    return tp
+
+
+def init(cf):
+    """
+    Start Alacorder using configuration object `cf`.
+    """
+    if cf["FETCH"] == True:
+        ft = fetch(cf=cf)
+        return ft
+    elif cf["ARCHIVE"] == True:
+        ar = archive(cf)
+        return ar
+    elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
+        vr = vrr_summary(cf)
+        return vr
+    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
+        ch = charges_summary(cf)
+        return ch
+    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
+        conv = convictions_summary(cf)
+        return cf
+    elif (
+        cf["TABLE"].lower() in ("charges", "disposition", "filing")
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        ch = charges(cf)
+        return ch
+    elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
+        ca = cases(cf)
+        return ca
+    elif (
+        cf["TABLE"].lower() in ("fees", "feesheet", "fines")
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        fs = fees(cf)
+        return fs
+    elif cf["TABLE"].lower() in ("witnesses", "witness") and cf["SUPPORT_SINGLETABLE"]:
+        out = witnesses(cf)
+        return out
+    elif (
+        cf["TABLE"].lower()
+        in (
+            "case-action-summary",
+            "cas",
+        )
+        and cf["SUPPORT_SINGLETABLE"]
+    ):
+        out = cas(cf)
+        return out
+    elif cf["TABLE"].lower() in ("settings", "set") and cf["SUPPORT_SINGLETABLE"]:
+        out = settings(cf)
+        return out
+    elif cf["TABLE"].lower() in ("images", "imgs", "img") and cf["SUPPORT_SINGLETABLE"]:
+        out = images(cf)
+        return out
+    elif cf["TABLE"] in ("attorneys", "att") and cf["SUPPORT_SINGLETABLE"]:
+        out = attorneys(cf)
+        return out
+    elif (
+        cf["TABLE"].lower() in ("all", "", "multi", "multitable")
+        and cf["SUPPORT_MULTITABLE"]
+    ):
+        mult = multi(cf)
+        return mult
+    else:
+        print("Job not specified. Select a mode and reconfigure to start.")
+        return None
+
+
+#   #   #   #        PRIVATE / INTERNALS         #   #   #   #
+
+
+def extract_text(path) -> str:
+    """
+    From path, return full text of PDF as string (PyMuPdf engine required!)
+    """
+    try:
+        doc = fitz.open(path)
+    except:
+        return ""
+    text = ""
+    for pg in doc:
+        try:
+            text += " \n ".join(
+                x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
+            )
+        except:
+            pass
+    text = re.sub(r"(<image\:.+?>)", "", text).strip()
+    return text
 
 
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
@@ -2058,15 +2114,14 @@
         "AdminUpdatedBy",
         "TransferDesc",
         "TBNV1",
         "TBNV2",
         "DriverLicenseNo",
         "StateID",
     )
-    cases = cases.sort("CaseNumber")
     return cases, all_charges, all_fees
 
 
 def split_charges(df, debug=False):
     dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
     charges = df.with_columns(
         [
@@ -2295,17 +2350,15 @@
         "PermanentDisqConviction",
         "Filing",
         "Disposition",
         "TotalBalance",
         "PaymentToRestore",
         "ChargesSummary",
     )
-    charges = charges.sort("CaseNumber")
     dlog(charges.columns, charges.shape, cf=debug)
-
     return charges
 
 
 def split_fees(df, debug=False):
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
@@ -3606,15 +3659,14 @@
         elif event == "MT":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
-                debug=False,
                 overwrite=True,
                 window=window,
             )
             threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
@@ -3623,15 +3675,14 @@
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=window["SUM-VRR"].get(),
                 charges_summary=window["SUM-CH"].get(),
                 convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
-                debug=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
             threading.Thread(target=init, args=[cf], daemon=True).start()
             window["SUM"].update(disabled=True)
         elif event == "POPUP":
@@ -3658,15 +3709,14 @@
                     window["TB-INPUTPATH"].get(),
                     window["TB-OUTPUTPATH"].get(),
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
-                    debug=False,
                     archive=False,
                     window=window,
                 )
                 # except:
                 window["TB"].update(disabled=True)
                 threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
@@ -3897,20 +3947,19 @@
     "no_update",
     is_flag=True,
     default=False,
     help="Do not update query template after completion",
 )
 @click.option(
     "--debug",
-    "-d",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug=False):
+def cli_fetch(listpath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         listpath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
@@ -3974,15 +4023,15 @@
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-write", default=False, is_flag=True, help="Do not export to output path"
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print debug logs to console"
+    "--debug",  default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
 def cli_table(
     input_path, output_path, count, table, overwrite, no_write, no_log, no_prompt, debug
 ):
@@ -4019,14 +4068,779 @@
         debug=debug,
     )
     if cf["DEBUG"]:
         print(cf, cf=cf)
     o = init(cf)
     return o
 
+@main.command(name="multi", help="Export all data tables to .xls/.xlsx")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_multi(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write data tables to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx"):
+        error("File extension must be .xls or .xlsx for multitable export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="all",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = multi(cf)
+    return o
+
+
+@main.command(name="cases", help="Create and export case information table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_cases(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="cases",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+
+@main.command(name="charges", help="Create and export charges table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option("--filing", "-f", is_flag=True, default=False, help="Only export filing charges")
+@click.option("--disposition", is_flag=True, default=False, help="Only export disposition charges")
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_charges(
+    input_path, output_path, filing, disposition, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        filing (bool, optional): Only export filing charges
+        disposition (bool, optional): Only export disposition charges
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    table = "charges" if not filing and not disposition else ""
+    table = "filing" if filing else table
+    table = "disposition" if disposition else table
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table=table,
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="fees", help="Create and export fees table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_cases(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="fees",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="settings", help="Create and export settings table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_settings(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="settings",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="witnesses", help="Create and export witnesses table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_witnesses(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="witnesses",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="case-action-summary", help="Create and export case action summaries")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_case_action_summary(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="case-action-summary",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+
+@main.command(name="images", help="Create and export images table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_images(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="images",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
+
+@main.command(name="attorneys", help="Create and export attorneys table")
+@click.option(
+    "--input-path",
+    "-in",
+    required=True,
+    type=click.Path(),
+    prompt="Input Path",
+    show_choices=False,
+)
+@click.option(
+    "--output-path", "-out", required=True, type=click.Path(), prompt="Output Path"
+)
+@click.option(
+    "--count",
+    "-c",
+    default=0,
+    help="Total cases to pull from input",
+    show_default=False,
+)
+@click.option(
+    "--overwrite",
+    "-o",
+    default=False,
+    help="Overwrite existing files at output path",
+    is_flag=True,
+    show_default=False,
+)
+@click.option(
+    "--no-prompt",
+    "-s",
+    default=False,
+    is_flag=True,
+    help="Skip user input / confirmation prompts",
+)
+@click.option(
+    "--no-log",
+    default=False,
+    is_flag=True,
+    help="Do not print logs to console",
+)
+@click.option(
+    "--no-write", default=False, is_flag=True, help="Do not export to output path"
+)
+@click.option(
+    "--debug", default=False, is_flag=True, help="Print debug logs to console"
+)
+@click.version_option(
+    package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
+)
+def cli_attorneys(
+    input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
+):
+    """
+    Write `cases` table to output path from archive or directory input.
+
+    Args:
+        input_path (str): PDF directory or archive input
+        output_path (str): Path to table output
+        count (int): Total cases to pull from input
+        overwrite (bool): Overwrite existing files at output path
+        no_write (bool): Do not export to output path
+        no_log(bool): Do not print logs to console
+        no_prompt (bool): Skip user input / confirmation prompts
+        debug (bool): Print verbose logs to console
+    """
+    log = not no_log
+    if os.path.splitext(output_path)[1] not in (".xls", ".xlsx", ".csv", ".json", ".parquet"):
+        error("File extension must be .xls, .xlsx, .csv, .json, or .parquet for table export.")
+    cf = set(
+        input_path,
+        output_path,
+        count=count,
+        table="attorneys",
+        overwrite=overwrite,
+        no_write=no_write,
+        log=log,
+        no_prompt=no_prompt,
+        debug=debug,
+    )
+    if cf["DEBUG"]:
+        print(cf, cf=cf)
+    o = init(cf)
+    return o
 
 @main.command(name="archive", help="Create full text archive from case PDFs")
 @click.option(
     "--input-path",
     "-in",
     required=True,
     type=click.Path(),
@@ -4070,15 +4884,15 @@
 @click.option(
     "--no-prompt",
     default=False,
     is_flag=True,
     help="Skip user input / confirmation prompts",
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def cli_archive(
     input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
 ):
@@ -4105,15 +4919,15 @@
         no_write=False,
         log=log,
         no_prompt=no_prompt,
         debug=debug,
     )
     if debug:
         click.echo(cf)
-    o = archive(cf, debug=debug)
+    o = archive(cf)
     return o
 
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
 )
@@ -4138,15 +4952,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         debug=debug,
         overwrite=overwrite,
@@ -4188,15 +5002,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_vrr(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         vrr_summary=True,
@@ -4238,15 +5052,15 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         charges_summary=True,
@@ -4288,49 +5102,29 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--debug", "-d", default=False, is_flag=True, help="Print verbose logs to console"
+    "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 def cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
     return convictions_summary(conf)
 
 
-def extract_text(path) -> str:
-    """
-    From path, return full text of PDF as string (PyMuPdf engine required!)
-    """
-    try:
-        doc = fitz.open(path)
-    except:
-        return ""
-    text = ""
-    for pg in doc:
-        try:
-            text += " \n ".join(
-                x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
-            )
-        except:
-            pass
-    text = re.sub(r"(<image\:.+?>)", "", text).strip()
-    return text
-
-
 if __name__ == "__main__":
     main()
 
 #   #   #   #           GETTER METHODS         #   #   #   #
 
 
 def get_paths(dirpath):
```

### Comparing `alacorder-79.8.9/PKG-INFO` & `alacorder-79.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.8.9
+Version: 79.9.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

