# Comparing `tmp/Quid-2.4.0.tar.gz` & `tmp/Quid-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quid-2.4.0.tar", last modified: Wed Apr 26 11:35:57 2023, max compression
+gzip compressed data, was "Quid-2.4.1.tar", last modified: Fri Apr 28 09:06:11 2023, max compression
```

## Comparing `Quid-2.4.0.tar` & `Quid-2.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2023-04-26 11:32:23.000000 Quid-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13106 2023-04-26 11:35:57.016539 Quid-2.4.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/Quid.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13106 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2023-04-26 11:35:57.000000 Quid-2.4.0/Quid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-26 11:35:56.000000 Quid-2.4.0/Quid.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    12374 2023-04-26 11:32:23.000000 Quid-2.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-26 11:32:23.000000 Quid-2.4.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/quid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.008539 Quid-2.4.0/quid/cli/
--rw-rw-rw-   0 root         (0) root         (0)    28626 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/cli/QuidCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/core/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/BestMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/InternalMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/InternalMatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)    17263 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Quid.py
--rw-rw-rw-   0 root         (0) root         (0)    17822 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/QuidMatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    14310 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/QuidMerger.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Text.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/core/Token.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/helper/
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/helper/Decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/helper/Loader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.012539 Quid-2.4.0/quid/match/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/match/Match.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/match/MatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/quid/passager/
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/AnalyzedWork.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/CitationSource.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/CitationSourceLink.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/Location.py
--rw-rw-rw-   0 root         (0) root         (0)    28856 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/Passager.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/SourceSegment.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetLocation.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetLocationSelection.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetText.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TargetTextLocationLink.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/passager/TextWithMatches.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/passager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:57.016539 Quid-2.4.0/quid/visualization/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Info.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Markup.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/MarkupSpan.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/TargetHtml.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/TargetTextWithContent.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Visualization.py
--rw-rw-rw-   0 root         (0) root         (0)    12304 2023-04-26 11:32:23.000000 Quid-2.4.0/quid/visualization/Visualizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 11:35:30.000000 Quid-2.4.0/quid/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-26 11:35:57.020539 Quid-2.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.326522 Quid-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2023-04-26 11:32:23.000000 Quid-2.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13106 2023-04-28 09:06:11.326522 Quid-2.4.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/Quid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13106 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-28 09:06:11.000000 Quid-2.4.1/Quid.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    12374 2023-04-26 11:32:23.000000 Quid-2.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-26 11:32:23.000000 Quid-2.4.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/quid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/quid/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    28626 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/cli/QuidCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/quid/core/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/BestMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/InternalMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/InternalMatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)    17263 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/Quid.py
+-rw-rw-rw-   0 root         (0) root         (0)    17822 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/QuidMatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    14310 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/QuidMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/Text.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/core/Token.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/quid/helper/
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/helper/Decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/helper/Loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.322522 Quid-2.4.1/quid/match/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/match/Match.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/match/MatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.326522 Quid-2.4.1/quid/passager/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/AnalyzedWork.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/CitationSource.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/CitationSourceLink.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/Location.py
+-rw-rw-rw-   0 root         (0) root         (0)    28856 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/Passager.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/SourceSegment.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TargetLocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TargetLocationSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TargetMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TargetText.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TargetTextLocationLink.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/passager/TextWithMatches.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/passager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:06:11.326522 Quid-2.4.1/quid/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/Info.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/Markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/MarkupSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/TargetHtml.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/TargetTextWithContent.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/Visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12304 2023-04-26 11:32:23.000000 Quid-2.4.1/quid/visualization/Visualizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 09:05:46.000000 Quid-2.4.1/quid/visualization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-28 09:06:11.330523 Quid-2.4.1/setup.cfg
```

### Comparing `Quid-2.4.0/LICENSE` & `Quid-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/PKG-INFO` & `Quid-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quid
-Version: 2.4.0
+Version: 2.4.1
 Summary: Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 Home-page: https://hu.berlin/quid
 Author: Frederik Arnold
 Author-email: frederik.arnold@hu-berlin.de
 Project-URL: Source, https://hu.berlin/quid
 Keywords: quotation detection,quotation identification,literal citation extraction,key passages,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Quid-2.4.0/Quid.egg-info/PKG-INFO` & `Quid-2.4.1/Quid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quid
-Version: 2.4.0
+Version: 2.4.1
 Summary: Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 Home-page: https://hu.berlin/quid
 Author: Frederik Arnold
 Author-email: frederik.arnold@hu-berlin.de
 Project-URL: Source, https://hu.berlin/quid
 Keywords: quotation detection,quotation identification,literal citation extraction,key passages,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Quid-2.4.0/Quid.egg-info/SOURCES.txt` & `Quid-2.4.1/Quid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/README.md` & `Quid-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/cli/QuidCLI.py` & `Quid-2.4.1/quid/cli/QuidCLI.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/core/Quid.py` & `Quid-2.4.1/quid/core/Quid.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/core/QuidMatcher.py` & `Quid-2.4.1/quid/core/QuidMatcher.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/core/QuidMerger.py` & `Quid-2.4.1/quid/core/QuidMerger.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/helper/Decoder.py` & `Quid-2.4.1/quid/helper/Decoder.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/helper/Loader.py` & `Quid-2.4.1/quid/helper/Loader.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/passager/AnalyzedWork.py` & `Quid-2.4.1/quid/passager/AnalyzedWork.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/passager/CitationSource.py` & `Quid-2.4.1/quid/passager/CitationSource.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/passager/Passager.py` & `Quid-2.4.1/quid/passager/Passager.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/passager/SourceSegment.py` & `Quid-2.4.1/quid/passager/SourceSegment.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/passager/TargetText.py` & `Quid-2.4.1/quid/passager/TargetText.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/quid/visualization/Visualizer.py` & `Quid-2.4.1/quid/visualization/Visualizer.py`

 * *Files identical despite different names*

### Comparing `Quid-2.4.0/setup.cfg` & `Quid-2.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Quid
-version = 2.4.0
+version = 2.4.1
 author = Frederik Arnold
 author_email = frederik.arnold@hu-berlin.de
 description = Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = quotation detection, quotation identification, literal citation extraction, key passages, natural language processing, nlp, text reuse
 url = https://hu.berlin/quid
```

