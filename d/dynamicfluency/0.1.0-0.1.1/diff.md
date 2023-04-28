# Comparing `tmp/dynamicfluency-0.1.0.tar.gz` & `tmp/dynamicfluency-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicfluency-0.1.0.tar", last modified: Tue Jan 17 10:55:23 2023, max compression
+gzip compressed data, was "dynamicfluency-0.1.1.tar", last modified: Fri Apr 28 11:43:21 2023, max compression
```

## Comparing `dynamicfluency-0.1.0.tar` & `dynamicfluency-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,45 @@
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.786050 dynamicfluency-0.1.0/
--rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2022-11-14 09:36:37.000000 dynamicfluency-0.1.0/LICENSE
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-01-17 10:55:23.786050 dynamicfluency-0.1.0/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1092 2022-11-15 18:13:09.000000 dynamicfluency-0.1.0/README.md
--rw-r--r--   0 jjw       (1000) jjw       (1000)      827 2023-01-17 10:44:02.000000 dynamicfluency-0.1.0/pyproject.toml
--rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-01-17 10:55:23.786050 dynamicfluency-0.1.0/setup.cfg
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.782050 dynamicfluency-0.1.0/src/
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.782050 dynamicfluency-0.1.0/src/dynamicfluency/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      325 2023-01-17 10:43:53.000000 dynamicfluency-0.1.0/src/dynamicfluency/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1941 2022-11-15 19:42:32.000000 dynamicfluency-0.1.0/src/dynamicfluency/aeneas_conversion.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.786050 dynamicfluency-0.1.0/src/dynamicfluency/helpers/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      536 2022-11-15 16:27:09.000000 dynamicfluency-0.1.0/src/dynamicfluency/helpers/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1188 2022-12-12 13:49:41.000000 dynamicfluency-0.1.0/src/dynamicfluency/helpers/conversions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      307 2022-11-14 11:19:49.000000 dynamicfluency-0.1.0/src/dynamicfluency/helpers/database_extensions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1917 2022-12-13 09:45:38.000000 dynamicfluency-0.1.0/src/dynamicfluency/helpers/textgridtier_extensions.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1798 2022-12-12 15:28:31.000000 dynamicfluency-0.1.0/src/dynamicfluency/pos_tagging.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1669 2022-12-12 15:24:51.000000 dynamicfluency-0.1.0/src/dynamicfluency/repetitions.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.786050 dynamicfluency-0.1.0/src/dynamicfluency/scripts/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2687 2022-11-15 16:29:29.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/add_frequency_dictionairy.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1417 2023-01-15 15:17:19.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      670 2022-11-14 14:58:12.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/download_nltk_requirements.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1883 2023-01-13 22:03:08.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/get_database_columns.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2935 2023-01-15 21:26:46.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_frequencytagged_girds_from_postagged_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1615 2022-12-12 14:15:40.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2079 2022-12-12 13:53:43.000000 dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     2881 2023-01-15 15:18:51.000000 dynamicfluency-0.1.0/src/dynamicfluency/word_frequencies.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-01-17 10:55:23.782050 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-01-17 10:55:23.000000 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1055 2023-01-17 10:55:23.000000 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/SOURCES.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-01-17 10:55:23.000000 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/dependency_links.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)      103 2023-01-17 10:55:23.000000 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/requires.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       15 2023-01-17 10:55:23.000000 dynamicfluency-0.1.0/src/dynamicfluency.egg-info/top_level.txt
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/LICENSE
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1092 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/README.md
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      986 2023-04-16 08:34:15.000000 dynamicfluency-0.1.1/pyproject.toml
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      104 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/requirements.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/setup.cfg
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.027801 dynamicfluency-0.1.1/src/
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.028801 dynamicfluency-0.1.1/src/dynamicfluency/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      325 2023-04-10 14:17:26.000000 dynamicfluency-0.1.1/src/dynamicfluency/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1952 2023-04-10 15:07:55.000000 dynamicfluency-0.1.1/src/dynamicfluency/aeneas_conversion.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency/data/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      248 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/src/dynamicfluency/data/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      122 2023-03-30 11:30:10.000000 dynamicfluency-0.1.1/src/dynamicfluency/data/valid_pos_tags.csv
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency/helpers/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      642 2023-04-16 10:28:22.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1416 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/conversions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      331 2023-04-10 14:16:43.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/database_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      363 2023-04-10 14:16:45.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/filepath_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2071 2023-04-16 20:30:14.000000 dynamicfluency-0.1.1/src/dynamicfluency/helpers/textgridtier_extensions.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1879 2023-04-16 20:50:04.000000 dynamicfluency-0.1.1/src/dynamicfluency/pos_tagging.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2004 2023-04-16 20:50:43.000000 dynamicfluency-0.1.1/src/dynamicfluency/repetitions.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.030801 dynamicfluency-0.1.1/src/dynamicfluency/scripts/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3010 2023-04-28 11:08:32.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/add_frequency_dictionary.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1614 2023-04-28 10:57:56.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      670 2023-04-10 14:16:47.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/download_nltk_requirements.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2111 2023-04-28 11:01:57.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/get_database_columns.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3377 2023-04-28 11:01:32.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2028 2023-04-28 11:02:38.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2401 2023-04-28 11:03:42.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1510 2023-04-28 11:08:07.000000 dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     2054 2023-04-16 20:30:14.000000 dynamicfluency-0.1.1/src/dynamicfluency/syntactic_analysis.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3071 2023-04-16 20:51:26.000000 dynamicfluency-0.1.1/src/dynamicfluency/word_frequencies.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.029801 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1747 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1419 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/SOURCES.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/dependency_links.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      103 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/requires.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       15 2023-04-28 11:43:21.000000 dynamicfluency-0.1.1/src/dynamicfluency.egg-info/top_level.txt
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-28 11:43:21.031801 dynamicfluency-0.1.1/tests/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     4917 2023-04-16 20:33:22.000000 dynamicfluency-0.1.1/tests/test_aeneas.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      588 2023-04-16 12:15:52.000000 dynamicfluency-0.1.1/tests/test_data.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    15320 2023-04-16 20:41:28.000000 dynamicfluency-0.1.1/tests/test_helpers.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    10068 2023-04-16 21:10:06.000000 dynamicfluency-0.1.1/tests/test_sql.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6323 2023-04-25 08:32:12.000000 dynamicfluency-0.1.1/tests/test_tier_generation.py
```

### Comparing `dynamicfluency-0.1.0/LICENSE` & `dynamicfluency-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.0/PKG-INFO` & `dynamicfluency-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicfluency
-Version: 0.1.0
+Version: 0.1.1
 Summary: The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech.
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/bare_python_publish
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/bare_python_publish/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicfluency-0.1.0/README.md` & `dynamicfluency-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.0/pyproject.toml` & `dynamicfluency-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamicfluency"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="JJWRoeloffs", email="jelleroeloffs@gmail.com" },
 ]
 description = "The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.package-data]
+dynamicfluency = ["**/data/*"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 "Homepage" = "https://github.com/JJWRoeloffs/bare_python_publish"
 "Bug Tracker" = "https://github.com/JJWRoeloffs/bare_python_publish/issues"
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/aeneas_conversion.py` & `dynamicfluency-0.1.1/src/dynamicfluency/aeneas_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from pathlib import Path
 from typing import Dict, List
 
 from praatio.utilities.constants import Interval
 from praatio.data_classes.interval_tier import IntervalTier
 
 
 class AeneasIntervaltier(IntervalTier):
@@ -52,14 +53,14 @@
         if force_validity:
             entryList = cls.force_entrylist_validity(entryList)
 
         return cls(name=name, entryList=entryList)
 
 
 def aeneas_tier_from_file(
-    filename: str, name: str, *, force_validity: bool = True
+    file: Path, name: str, *, force_validity: bool = True
 ) -> AeneasIntervaltier:
-    with open(filename, "r") as file:
-        allignment_dict = json.load(file)
+    with file.open("r") as f:
+        allignment_dict = json.load(f)
     return AeneasIntervaltier.from_json(
         allignment_dict, name, force_validity=force_validity
     )
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/helpers/__init__.py` & `dynamicfluency-0.1.1/src/dynamicfluency/helpers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from .database_extensions import connect_to_database
-from .conversions import split_pos_label, pos_tier_to_lemma_tier
+from .database_extensions import get_row_cursor
+from .filepath_extensions import get_local_glob
+from .conversions import split_pos_label, pos_tier_to_word_form_tier
 from .textgridtier_extensions import (
+    get_midpoint,
     replace_label,
     entrylist_labels_to_string,
     set_all_tiers_static,
     set_all_tiers_from_dict,
     make_lowercase_entrylist,
 )
 
 __all__ = (
-    "connect_to_database",
+    "get_midpoint",
+    "get_row_cursor",
+    "get_local_glob",
     "split_pos_label",
-    "pos_tier_to_lemma_tier",
+    "pos_tier_to_word_form_tier",
     "replace_label",
     "entrylist_labels_to_string",
     "set_all_tiers_static",
     "set_all_tiers_from_dict",
     "make_lowercase_entrylist",
 )
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/helpers/conversions.py` & `dynamicfluency-0.1.1/src/dynamicfluency/helpers/conversions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from __future__ import annotations
 
 from itertools import chain
 
 from praatio.data_classes.textgrid_tier import TextgridTier
+from praatio.utilities.constants import Interval
 
 from .textgridtier_extensions import replace_label
 
 
+def get_midpoint(interval: Interval) -> float:
+    return (interval.start + interval.end) / 2
+
+
 def split_pos_label(pos_label: str, *, get_pos: bool = False) -> str:
-    """The lemma split from the full POS tag label.
+    """The word_form split from the full POS tag label.
     This label can have multiple words causing complication.
     It determines the splits by "_" and " ", the form "part_tag part_tag part_tag"
     Example:
     "is_VB" -> "is",
     "is_VB n't_RB" -> "isn't"
     Example for get_pos=True:
     "is_VB" -> "VB",
     "is_VB n't_RB" -> "VB RB"
 
     """
     index = 1 if get_pos else 0
     join = " " if get_pos else ""
 
     split = pos_label.split("_")
-    lemmas_and_tags = chain(*[lemma.split(" ") for lemma in split])
-    lemmas = [lemma for i, lemma in enumerate(lemmas_and_tags) if (i % 2) == index]
-    return join.join(lemmas)
+    word_forms_and_tags = chain(*[word_form.split(" ") for word_form in split])
+    word_forms = [
+        word_form for i, word_form in enumerate(word_forms_and_tags) if (i % 2) == index
+    ]
+    return join.join(word_forms)
 
 
-def pos_tier_to_lemma_tier(
-    pos_tier: TextgridTier, name: str = "Lemmas"
+def pos_tier_to_word_form_tier(
+    pos_tier: TextgridTier, name: str = "WordForms"
 ) -> TextgridTier:
-    """Makes a lemma tier out of a pos_tagging made pos_tier"""
-    lemma_list = [replace_label(entry, split_pos_label) for entry in pos_tier.entryList]
-    return pos_tier.new(name=name, entryList=lemma_list)
+    """Makes a word_form tier out of a pos_tagging made pos_tier"""
+    word_form_list = [
+        replace_label(entry, split_pos_label) for entry in pos_tier.entryList
+    ]
+    return pos_tier.new(name=name, entryList=word_form_list)
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/helpers/textgridtier_extensions.py` & `dynamicfluency-0.1.1/src/dynamicfluency/helpers/textgridtier_extensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from __future__ import annotations
 
 from typing import Callable, List, Dict
 from collections import namedtuple
 
 from praatio.data_classes.textgrid import Textgrid
+from praatio.utilities.constants import Interval
 
 
 def replace_label(entry: namedtuple, f: Callable) -> namedtuple:
     """Returns a new namedtuple with the "label" attribute changed according to passed function."""
     return entry._replace(label=f(entry.label))
 
 
+def get_midpoint(interval: Interval) -> float:
+    return (interval.start + interval.end) / 2
+
+
 def entrylist_labels_to_string(
     entryList: List[namedtuple], *, to_ignore: List[str] = []
 ) -> str:
     """Make a single space-seperated string, out of the labels of an entryList
     Useful to make a "sentence" out of the words in the tier."""
     return " ".join(
         [
             entry.label
             for entry in entryList
-            if entry.label and (not entry.label in to_ignore)
+            if entry.label
+            if not entry.label in to_ignore
         ]
     )
 
 
 def set_all_tiers_static(grid: Textgrid, *, item: str, index: int) -> None:
     """Sets the given index of all tiers' label of given grid to given value"""
     for tier in grid.tierDict:
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/pos_tagging.py` & `dynamicfluency-0.1.1/src/dynamicfluency/pos_tagging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from collections import namedtuple
 from typing import List, Union
 
 import nltk
-from praatio.data_classes.textgrid_tier import TextgridTier
+from praatio.data_classes.interval_tier import IntervalTier
 
 from dynamicfluency.helpers import entrylist_labels_to_string, make_lowercase_entrylist
 
 
-def generate_tags_from_entrylist(entryList: List[namedtuple]) -> List[Union[str, str]]:
-
+def generate_tags_from_entrylist(
+    entryList: List[namedtuple], *, lang: str = "eng"
+) -> List[Union[str, str]]:
     text = entrylist_labels_to_string(entryList)
     tokens: List[str] = nltk.word_tokenize(text)
-    return nltk.pos_tag(tokens)
+    return nltk.pos_tag(tokens=tokens, lang=lang)
 
 
 # Jankyness needed because the NLTK tokenise split sometimes splits words into smaller sub-sections
 def allign_tags(
     tags: List[Union[str, str]], entryList: List[namedtuple]
 ) -> List[namedtuple]:
     """Make an alligned entrylist out of NLTK generated pos_tags and the entryList those were generated from."""
@@ -33,19 +34,21 @@
             word += tags[0][0]
             label = " ".join([label, "_".join(tags[0])])
             tags.pop(0)
         new_entryList.append(entry._replace(label=label.strip()))
     return new_entryList
 
 
-def make_pos_tier(words_tier: TextgridTier, *, name: str = "POStags") -> TextgridTier:
+def make_pos_tier(
+    words_tier: IntervalTier, *, name: str = "POStags", lang: str = "eng"
+) -> IntervalTier:
     """Makes a POS tagged tier from a textgrid tier with alligned words"""
 
     nltk.download("punkt", quiet=True, halt_on_error=True)
     nltk.download("averaged_perceptron_tagger", quiet=True, halt_on_error=True)
 
     lowercase_entryList = make_lowercase_entrylist(words_tier.entryList)
 
-    tags = generate_tags_from_entrylist(lowercase_entryList)
+    tags = generate_tags_from_entrylist(lowercase_entryList, lang=lang)
     tag_entryList = allign_tags(tags, lowercase_entryList)
 
     return words_tier.new(name=name, entryList=tag_entryList)
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/repetitions.py` & `dynamicfluency-0.1.1/src/dynamicfluency/repetitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
-import glob
-import argparse
 from typing import List
 
 import nltk
-from praatio import textgrid as tg
-from praatio.data_classes.textgrid_tier import TextgridTier
+from praatio.data_classes.interval_tier import IntervalTier
 
-from dynamicfluency.helpers import entrylist_labels_to_string
+from dynamicfluency.helpers import entrylist_labels_to_string, split_pos_label
 
 
 def make_repetitions_tier(
-    pos_tier: TextgridTier,
+    pos_tier: IntervalTier,
     *,
     max_cache: int = 100,
     to_ignore: List[str] = [],
     name: str = "Repetitions",
-) -> TextgridTier:
-
+) -> IntervalTier:
     cache = []
     repetitions_list = []
 
     for entry in pos_tier.entryList:
-        if (not entry.label) or (entry.label in to_ignore):
+        if (
+            (not entry.label)
+            or (entry.label in to_ignore)
+            or (split_pos_label(entry.label) in to_ignore)
+        ):
             repetitions_list.append(entry)
             continue
 
         cache.insert(0, entry.label)
         if len(cache) > max_cache:
             cache.pop()
 
@@ -38,24 +38,36 @@
 
         repetitions_list.append(entry._replace(label=repetitions))
 
     return pos_tier.new(name=name, entryList=repetitions_list)
 
 
 def make_freqdist_tier(
-    pos_tier: TextgridTier, *, to_ignore: List[str] = [], name: str = "FreqDist"
-) -> TextgridTier:
+    pos_tier: IntervalTier, *, to_ignore: List[str] = [], name: str = "FreqDist"
+) -> IntervalTier:
     nltk.download("punkt", quiet=True, halt_on_error=True)
 
-    text = entrylist_labels_to_string(pos_tier.entryList, to_ignore=to_ignore)
-    fdist = nltk.FreqDist(nltk.word_tokenize(text))
+    processed_entryList = [
+        interval
+        for interval in pos_tier.entryList
+        if interval.label
+        if not interval.label in to_ignore
+        if not split_pos_label(interval.label) in to_ignore
+    ]
+
+    text = entrylist_labels_to_string(processed_entryList)
+    fdist = nltk.FreqDist(text.split())
     freqdist_list = []
 
     for entry in pos_tier.entryList:
-        if (not entry.label) or (entry.label in to_ignore):
+        if (
+            (not entry.label)
+            or (entry.label in to_ignore)
+            or (split_pos_label(entry.label) in to_ignore)
+        ):
             freqdist_list.append(entry)
             continue
 
         frequency = str(fdist.freq(entry.label))
         freqdist_list.append(entry._replace(label=frequency))
 
     return pos_tier.new(name=name, entryList=freqdist_list)
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import os
-import glob
 import argparse
+from pathlib import Path
 
 from praatio.data_classes.textgrid import Textgrid
 
 from dynamicfluency.aeneas_conversion import aeneas_tier_from_file
+from dynamicfluency.helpers import get_local_glob
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Processes tokens and phrases .json files generated by aeneas a .TextGrid"
     )
     parser.add_argument(
         "-d",
         "--directory",
         nargs="?",
         default="output",
         help="The directory the tokens and phases is expected in, and the output is saved to",
     )
-    return parser.parse_args()
+    args = parser.parse_args()
+
+    if not Path(args.directory).exists():
+        parser.error(f"{args.directory} does not exist")
+
+    return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
-    word_allignments = glob.glob(f"./{args.directory}/*.tokens.json")
-    phrase_allignments = glob.glob(f"./{args.directory}/*.phrases.json")
+    word_allignments = get_local_glob(args.directory, glob="*.tokens.json")
+    phrase_allignments = get_local_glob(args.directory, glob="*.phrases.json")
 
     for words, phrases in zip(word_allignments, phrase_allignments):
         words_tier = aeneas_tier_from_file(words, "Words")
         phrases_tier = aeneas_tier_from_file(phrases, "Phrases")
 
         allignment_grid = Textgrid()
         allignment_grid.addTier(words_tier)
         allignment_grid.addTier(phrases_tier)
-        name = words.replace(".tokens.json", ".allignment.TextGrid")
+        name = str(words).replace(".tokens.json", ".allignment.TextGrid")
         allignment_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
 
         os.remove(words)
         os.remove(phrases)
 
 
 if __name__ == "__main__":
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/download_nltk_requirements.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/download_nltk_requirements.py`

 * *Files identical despite different names*

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/get_database_columns.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/get_database_columns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-import os
 import csv
-import glob
 import argparse
+from pathlib import Path
+import sqlite3
 
-from praatio import textgrid as tg
-
-from dynamicfluency.helpers import connect_to_database
+from dynamicfluency.helpers import get_row_cursor
 from dynamicfluency.word_frequencies import get_column_names
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Reads the collumns from an SQLite3 database. Presents the found names inside a .csv in the output directory to allow it to be read by praat"
     )
@@ -32,38 +30,45 @@
     parser.add_argument(
         "-d",
         "--directory",
         nargs="?",
         default="output",
         help="The directory the text file is saved to.",
     )
-    return parser.parse_args()
+
+    args = parser.parse_args()
+
+    if not Path(args.database).exists():
+        parser.error(f"{args.database} does not exist")
+
+    if not Path(args.directory).exists():
+        parser.error(f"{args.directory} does not exist")
+
+    return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
-    filepath = f"./{args.directory}/column_names.csv"
+    filepath = Path().resolve().joinpath(args.directory, "column_names.csv")
 
     # As far as I am aware, there is no good way to send an error message like this back to praat.
-    if os.path.exists(filepath):
-        print(f"{filepath} already exists")
+    if filepath.exists():
+        print(f"{str(filepath)} already exists")
         print("Cannot write anywhere.")
         return
 
-    try:
-        cursor = connect_to_database(args.database)
+    with sqlite3.connect(args.database) as connection:
+        cursor = get_row_cursor(connection)
         names = get_column_names(cursor, table_name=args.table_name)
-    finally:
-        cursor.connection.close()
 
     if not names:
         names = ["#FAIL - Incorrect table name?"]
-    if not "Lemma" in names:
-        names = ['#FAIL - No column "Lemma" found.']
+    if not "WordForm" in names:
+        names = ['#FAIL - No column "WordForm" found.']
 
-    with open(filepath, "w") as f:
+    with filepath.open("w", encoding="utf-8") as f:
         csv.writer(f).writerow(names)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_frequencytagged_girds_from_postagged_grids.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-import glob
 import argparse
+import sqlite3
+from pathlib import Path
 
 from praatio import textgrid as tg
+from praatio.data_classes.interval_tier import IntervalTier
 
-from dynamicfluency.helpers import pos_tier_to_lemma_tier, connect_to_database
+from dynamicfluency.helpers import get_row_cursor, get_local_glob
 from dynamicfluency.word_frequencies import create_frequency_grid
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        description='Reads word frequencies from an SQLite3 database. Assumes lemmas are in a column called "Lemma"'
+        description='Reads word frequencies from an SQLite3 database. Assumes word_forms are in a column called "WordForm"'
     )
     requiredNamed = parser.add_argument_group("Required named arguments")
 
     requiredNamed.add_argument(
         "-t", "--table_name", help="Name of the table to be read from.", required=True
     )
     requiredNamed.add_argument(
@@ -53,45 +55,55 @@
         default="",
         help="The Rows to read from the database table, seperated by commas",
     )
 
     args: argparse.Namespace = parser.parse_args()
     args.to_ignore = args.to_ignore.split(",") if args.to_ignore is not None else None
     args.rows = args.rows.split(",") if args.rows else None
+
+    if not Path(args.database).exists():
+        parser.error(f"{args.database} does not exist")
+
+    if not Path(args.directory).exists():
+        parser.error(f"{args.directory} does not exist")
+
     return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
     if args.allignment == "maus":
         tokentier_name = "ORT-MAU"
     elif args.allignment == "aeneas":
         tokentier_name = "Words"
     else:
         raise ValueError(f"Unknown allignment type found: {args.allignment}")
 
-    allignment_files = glob.glob(f"./{args.directory}/*.allignment.TextGrid")
+    allignment_files = get_local_glob(args.directory, glob="*.allignment.TextGrid")
 
     for file in allignment_files:
-        allignment_grid = tg.openTextgrid(file, includeEmptyIntervals=True)
+        allignment_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
+
+        if not isinstance(
+            tier := allignment_grid.tierDict[tokentier_name], IntervalTier
+        ):
+            raise ValueError("Cannot read Allignment: Not an interval tier")
 
-        try:
-            cursor = connect_to_database(args.database)
+        with sqlite3.connect(args.database) as connection:
+            cursor = get_row_cursor(connection)
             frequency_grid = create_frequency_grid(
-                lemma_tier=allignment_grid.tierDict[tokentier_name],
+                word_form_tier=tier,
                 cursor=cursor,
                 table_name=args.table_name,
                 to_ignore=args.to_ignore,
                 rows=args.rows,
             )
-        finally:
-            cursor.connection.close()
 
-        frequency_grid.removeTier("Lemma")
+        frequency_grid.removeTier("WordForm")
 
-        name = file.replace(".allignment.TextGrid", ".frequencies.TextGrid")
+        name = str(file).replace(".allignment.TextGrid", ".frequencies.TextGrid")
         frequency_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-import glob
+from pathlib import Path
 import argparse
 
 from praatio import textgrid as tg
 from praatio.data_classes.textgrid import Textgrid
+from praatio.data_classes.interval_tier import IntervalTier
 
 from dynamicfluency.pos_tagging import make_pos_tier
+from dynamicfluency.helpers import get_local_glob
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description="Creates a textgrid with a POS-tagged tier from an allignment textgrid"
     )
     parser.add_argument(
@@ -22,35 +24,47 @@
         help="The directory the tokens and phases is expected in, and the output is saved to",
     )
     parser.add_argument(
         "-a",
         "--allignment",
         help="The type of allignment textgrid, either 'maus' or 'aeneas'",
     )
-    return parser.parse_args()
+
+    args = parser.parse_args()
+
+    if not Path(args.directory).exists():
+        parser.error(f"{args.directory} does not exist")
+
+    return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
     if args.allignment == "maus":
         tokentier_name = "ORT-MAU"
     elif args.allignment == "aeneas":
         tokentier_name = "Words"
     else:
         raise ValueError(f"Unknown allignment type found: {args.allignment}")
 
-    allignment_files = glob.glob(f"./{args.directory}/*.allignment.TextGrid")
+    allignment_files = get_local_glob(args.directory, glob="*.allignment.TextGrid")
 
     for file in allignment_files:
-        allignment_grid = tg.openTextgrid(file, includeEmptyIntervals=True)
+        allignment_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
 
-        tagged_tier = make_pos_tier(allignment_grid.tierDict[tokentier_name])
+        if not isinstance(
+            tier := allignment_grid.tierDict[tokentier_name], IntervalTier
+        ):
+            raise ValueError("Cannot read Allignment: Not an interval tier")
+
+        tagged_tier = make_pos_tier(tier)
 
         tag_grid = Textgrid()
         tag_grid.addTier(tagged_tier)
-        name = file.replace(".allignment.TextGrid", ".pos_tags.TextGrid")
+
+        name = str(file).replace(".allignment.TextGrid", ".pos_tags.TextGrid")
         tag_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py` & `dynamicfluency-0.1.1/src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,52 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-import glob
 import argparse
+from pathlib import Path
 
 from praatio import textgrid as tg
-from praatio.data_classes.textgrid import Textgrid
+from praatio.data_classes.interval_tier import IntervalTier
 
-from dynamicfluency.repetitions import make_repetitions_tier, make_freqdist_tier
+from dynamicfluency.helpers import get_local_glob
+from dynamicfluency.syntactic_analysis import make_syntax_grid
 
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        description="Processes alligned pos_tags .TextGrid files generated by pos_tagging.py to a .TextGrid with reptition information in it."
+        description="Creates textgrid with syntactic information already present in pos tags"
     )
     parser.add_argument(
         "-d",
         "--directory",
         nargs="?",
         default="output",
-        help="The directory the pos_tags .TextGrid is expected in, and the output is saved to",
-    )
-    parser.add_argument(
-        "-m",
-        "--max_read",
-        nargs="?",
-        default=300,
-        type=int,
-        help="The maximum amount of words the detector reads back to check for repetitions",
-    )
-    parser.add_argument(
-        "-i",
-        "--to_ignore",
-        nargs="?",
-        help="The words to ignore and not assign any value, seperated by commas.",
+        help="The directory the tokens and phases is expected in, and the output is saved to",
     )
 
-    args: argparse.Namespace = parser.parse_args()
-    args.to_ignore.split(",")
+    args = parser.parse_args()
+
+    if not Path(args.directory).exists():
+        parser.error(f"{args.directory} does not exist")
+
     return args
 
 
 def main():
     args: argparse.Namespace = parse_arguments()
 
-    tagged_files = glob.glob(f"./{args.directory}/*.pos_tags.TextGrid")
+    tagged_files = get_local_glob(args.directory, glob="*.pos_tags.TextGrid")
+
     for file in tagged_files:
-        tagged_grid = tg.openTextgrid(file, includeEmptyIntervals=True)
+        tagged_grid = tg.openTextgrid(str(file), includeEmptyIntervals=True)
+
+        if not isinstance(tier := tagged_grid.tierDict["POStags"], IntervalTier):
+            raise ValueError("Cannot read POStags: Not an interval tier")
 
-        repetition_tier = make_repetitions_tier(
-            pos_tier=tagged_grid.tierDict["POStags"],
-            max_cache=args.max_read,
-            to_ignore=args.to_ignore,
-        )
-        freqdist_tier = make_freqdist_tier(
-            pos_tier=tagged_grid.tierDict["POStags"], to_ignore=args.to_ignore
-        )
-
-        repetition_grid = Textgrid()
-        repetition_grid.addTier(repetition_tier)
-        repetition_grid.addTier(freqdist_tier)
+        syntax_grid = make_syntax_grid(pos_tier=tier)
 
-        name = file.replace(".pos_tags.TextGrid", ".repetitions.TextGrid")
-        repetition_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
+        name = str(file).replace(".pos_tags.TextGrid", ".syntax.TextGrid")
+        syntax_grid.save(name, format="long_textgrid", includeBlankSpaces=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency.egg-info/PKG-INFO` & `dynamicfluency-0.1.1/src/dynamicfluency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicfluency
-Version: 0.1.0
+Version: 0.1.1
 Summary: The base python package for DynamicFluency: Monitor and understand the dynamicity of linguistic aspects in (L2) speech.
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/bare_python_publish
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/bare_python_publish/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicfluency-0.1.0/src/dynamicfluency.egg-info/SOURCES.txt` & `dynamicfluency-0.1.1/src/dynamicfluency.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 src/dynamicfluency/__init__.py
 src/dynamicfluency/aeneas_conversion.py
 src/dynamicfluency/pos_tagging.py
 src/dynamicfluency/repetitions.py
+src/dynamicfluency/syntactic_analysis.py
 src/dynamicfluency/word_frequencies.py
 src/dynamicfluency.egg-info/PKG-INFO
 src/dynamicfluency.egg-info/SOURCES.txt
 src/dynamicfluency.egg-info/dependency_links.txt
 src/dynamicfluency.egg-info/requires.txt
 src/dynamicfluency.egg-info/top_level.txt
+src/dynamicfluency/data/__init__.py
+src/dynamicfluency/data/valid_pos_tags.csv
 src/dynamicfluency/helpers/__init__.py
 src/dynamicfluency/helpers/conversions.py
 src/dynamicfluency/helpers/database_extensions.py
+src/dynamicfluency/helpers/filepath_extensions.py
 src/dynamicfluency/helpers/textgridtier_extensions.py
-src/dynamicfluency/scripts/add_frequency_dictionairy.py
+src/dynamicfluency/scripts/add_frequency_dictionary.py
 src/dynamicfluency/scripts/convert_aeneas_to_textgrids.py
 src/dynamicfluency/scripts/download_nltk_requirements.py
 src/dynamicfluency/scripts/get_database_columns.py
-src/dynamicfluency/scripts/make_frequencytagged_girds_from_postagged_grids.py
+src/dynamicfluency/scripts/make_frequencytagged_girds_from_alligned_grids.py
 src/dynamicfluency/scripts/make_postagged_grids_from_alligned_grids.py
-src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
+src/dynamicfluency/scripts/make_repetitionstagged_grids_from_postagged_grids.py
+src/dynamicfluency/scripts/make_syntax_grids_from_postagged_grids.py
+tests/test_aeneas.py
+tests/test_data.py
+tests/test_helpers.py
+tests/test_sql.py
+tests/test_tier_generation.py
```

