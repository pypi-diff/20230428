# Comparing `tmp/curriculum_analysis-0.2.4.tar.gz` & `tmp/curriculum_analysis-0.2.5.tar.gz`

## Comparing `curriculum_analysis-0.2.4.tar` & `curriculum_analysis-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/js_exporter.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/keywords.txt
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/data.js
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/index.html
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/index.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/module.html
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/module.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/curriculum_analysis/html/style.css
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/LICENCE
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/README.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/js_exporter.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/keywords.txt
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/data.js
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/module.html
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/module.js
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/style.css
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/LICENCE
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/PKG-INFO
```

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/analysis.py` & `curriculum_analysis-0.2.5/curriculum_analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/corpus.py` & `curriculum_analysis-0.2.5/curriculum_analysis/corpus.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.2.5/curriculum_analysis/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/js_exporter.py` & `curriculum_analysis-0.2.5/curriculum_analysis/js_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.2.5/curriculum_analysis/json_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/main.py` & `curriculum_analysis-0.2.5/curriculum_analysis/main.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.2.5/curriculum_analysis/txt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Details of the structure of txt files, extract data into objects with properties"""
 import logging
 
 log = logging.getLogger(__name__)
 
 def extractData(path, split_string):
-    with path.open('r', encoding='utf8') as f:
+    with path.open('r', encoding='utf8', errors='surrogateescape') as f:
         data = f.read()
         chunks = data.split(split_string)
         chunks = [ch.splitlines() for ch in chunks]
         # chunks = [[line.strip() for line in ch if line.strip()] for ch in chunks]
         chunks[0] = ['deleteme', '', *chunks[0]]
         chunks = [ch[1:] for ch in chunks][:-1]
         for chunk in chunks:
```

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/html/index.html` & `curriculum_analysis-0.2.5/curriculum_analysis/html/index.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/html/index.js` & `curriculum_analysis-0.2.5/curriculum_analysis/html/index.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/html/module.html` & `curriculum_analysis-0.2.5/curriculum_analysis/html/module.html`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/html/module.js` & `curriculum_analysis-0.2.5/curriculum_analysis/html/module.js`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/curriculum_analysis/html/style.css` & `curriculum_analysis-0.2.5/curriculum_analysis/html/style.css`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/LICENCE` & `curriculum_analysis-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/README.md` & `curriculum_analysis-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.4/pyproject.toml` & `curriculum_analysis-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "curriculum_analysis/keywords.txt",
   "curriculum_analysis/html/*",
   "**/*.py",  
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
   { name="Tom Harrison" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `curriculum_analysis-0.2.4/PKG-INFO` & `curriculum_analysis-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
```

