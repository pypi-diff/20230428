# Comparing `tmp/docmaptools-0.6.0.tar.gz` & `tmp/docmaptools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmaptools-0.6.0.tar", last modified: Tue Apr 18 22:51:52 2023, max compression
+gzip compressed data, was "docmaptools-0.7.0.tar", last modified: Fri Apr 28 01:29:28 2023, max compression
```

## Comparing `docmaptools-0.6.0.tar` & `docmaptools-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-04-18 22:51:22.000000 docmaptools-0.6.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-04-18 22:51:22.000000 docmaptools-0.6.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-18 22:51:52.379190 docmaptools-0.6.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-04-18 22:51:22.000000 docmaptools-0.6.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/docmaptools/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5293 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/parse.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/docmaptools.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-04-18 22:51:22.000000 docmaptools-0.6.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-04-18 22:51:52.379190 docmaptools-0.6.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-04-18 22:51:22.000000 docmaptools-0.6.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_init.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    24022 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-04-28 01:28:58.000000 docmaptools-0.7.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-04-28 01:28:58.000000 docmaptools-0.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-28 01:29:28.692159 docmaptools-0.7.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-04-28 01:28:58.000000 docmaptools-0.7.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/docmaptools/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8128 2023-04-28 01:28:58.000000 docmaptools-0.7.0/docmaptools/parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/docmaptools.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-04-28 01:29:28.000000 docmaptools-0.7.0/docmaptools.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-04-28 01:28:58.000000 docmaptools-0.7.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-04-28 01:29:28.692159 docmaptools-0.7.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-04-28 01:28:58.000000 docmaptools-0.7.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-28 01:29:28.692159 docmaptools-0.7.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_init.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    28557 2023-04-28 01:28:58.000000 docmaptools-0.7.0/tests/test_parse.py
```

### Comparing `docmaptools-0.6.0/LICENSE` & `docmaptools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docmaptools-0.6.0/PKG-INFO` & `docmaptools-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.6.0
+Version: 0.7.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.6.0/docmaptools/__init__.py` & `docmaptools-0.7.0/docmaptools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
 
 
 def configure_logging(filename, level=logging.INFO, format_string=None):
```

### Comparing `docmaptools-0.6.0/docmaptools/convert.py` & `docmaptools-0.7.0/docmaptools/convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.6.0/docmaptools.egg-info/PKG-INFO` & `docmaptools-0.7.0/docmaptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.6.0
+Version: 0.7.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.6.0/setup.py` & `docmaptools-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.6.0/tests/test_convert.py` & `docmaptools-0.7.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.6.0/tests/test_init.py` & `docmaptools-0.7.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.6.0/tests/test_parse.py` & `docmaptools-0.7.0/tests/test_parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -150,14 +150,39 @@
                 "type": "preprint",
                 "identifier": "85111",
                 "versionIdentifier": "2",
                 "doi": "10.7554/eLife.85111.2",
             },
         )
 
+    def test_docmap_preprint_history(self):
+        "list of preprint history event data"
+        result = parse.docmap_preprint_history(self.d_json)
+        expected = [
+            {
+                "type": "preprint",
+                "doi": "10.1101/2022.11.08.515698",
+                "versionIdentifier": "2",
+                "date": "2022-11-22",
+            },
+            {
+                "type": "reviewed-preprint",
+                "doi": "10.7554/eLife.85111.1",
+                "versionIdentifier": "1",
+                "date": "2022-11-28T11:30:05+00:00",
+            },
+            {
+                "type": "reviewed-preprint",
+                "doi": "10.7554/eLife.85111.2",
+                "versionIdentifier": "2",
+                "date": "2023-04-14T13:42:25.781585+00:00",
+            },
+        ]
+        self.assertEqual(result, expected)
+
     def test_step_actions(self):
         "get actions from the last step"
         step_2 = parse.next_step(
             self.d_json,
             parse.next_step(self.d_json, parse.docmap_first_step(self.d_json)),
         )
         result = parse.step_actions(step_2)
@@ -435,20 +460,39 @@
     def test_docmap_latest_preprint(self):
         "preprint data from the most recent step inputs"
         result = parse.docmap_latest_preprint(self.d_json)
         self.assertDictEqual(
             result,
             {
                 "identifier": "84364",
-                "versionIdentifier": "",
+                "versionIdentifier": "1",
                 "type": "preprint",
-                "doi": "10.7554/eLife.84364",
+                "doi": "10.7554/eLife.84364.1",
             },
         )
 
+    def test_docmap_preprint_history(self):
+        "list of preprint history event data"
+        result = parse.docmap_preprint_history(self.d_json)
+        expected = [
+            {
+                "type": "preprint",
+                "doi": "10.1101/2022.10.17.512253",
+                "versionIdentifier": "1",
+                "date": "2022-10-17",
+            },
+            {
+                "type": "reviewed-preprint",
+                "doi": "10.7554/eLife.84364.1",
+                "versionIdentifier": "1",
+                "date": "2022-11-08T07:01:52+00:00",
+            },
+        ]
+        self.assertEqual(result, expected)
+
     def test_step_actions(self):
         "get actions from the last step"
         step_2 = parse.next_step(
             self.d_json,
             parse.next_step(self.d_json, parse.docmap_first_step(self.d_json)),
         )
         result = parse.step_actions(step_2)
@@ -505,14 +549,100 @@
                     ),
                 ]
             ),
         ]
         self.assertEqual(result, expected)
 
 
+class TestPreprintEventOutput(unittest.TestCase):
+    def setUp(self):
+        self.output_type = "preprint"
+        self.output_doi = "10.7554/eLife.85111.1"
+        self.output_version_identifier = "1"
+        self.output_date_string = "2023-04-27T15:30:00+00:00"
+        self.step_json = {"assertions": [{"happened": self.output_date_string}]}
+
+    def test_not_found(self):
+        "test if first preprint is not yet found"
+        found_first_preprint = False
+        output_json = {
+            "type": self.output_type,
+            "doi": self.output_doi,
+            "versionIdentifier": self.output_version_identifier,
+            "published": self.output_date_string,
+        }
+        expected = {
+            "type": self.output_type,
+            "doi": self.output_doi,
+            "versionIdentifier": self.output_version_identifier,
+            "date": self.output_date_string,
+        }
+        result = parse.preprint_event_output(
+            output_json, self.step_json, found_first_preprint
+        )
+        self.assertDictEqual(result, expected)
+
+    def test_found(self):
+        "test if first preprint is already found"
+        found_first_preprint = True
+        output_json = {
+            "type": self.output_type,
+            "doi": self.output_doi,
+            "versionIdentifier": self.output_version_identifier,
+            "date": self.output_date_string,
+        }
+        expected = {
+            "type": "reviewed-preprint",
+            "doi": self.output_doi,
+            "versionIdentifier": self.output_version_identifier,
+            "date": self.output_date_string,
+        }
+        result = parse.preprint_event_output(
+            output_json, self.step_json, found_first_preprint
+        )
+        self.assertDictEqual(result, expected)
+
+
+class TestPreprintHappenedDate(unittest.TestCase):
+    def test_preprint_happened_date(self):
+        date_string = "2023-04-27T15:30:00+00:00"
+        step_json = {"assertions": [{"happened": date_string}]}
+        self.assertEqual(parse.preprint_happened_date(step_json), date_string)
+
+    def test_none(self):
+        step_json = None
+        self.assertEqual(parse.preprint_happened_date(step_json), None)
+
+
+class TestPreprintAlternateDate(unittest.TestCase):
+    def test_preprint_alternate_date(self):
+        date_string = "2023-04-27T15:30:00+00:00"
+        step_json = {
+            "actions": [
+                {
+                    "outputs": [
+                        {
+                            "type": "evaluation-summary",
+                            "published": date_string,
+                        }
+                    ]
+                }
+            ]
+        }
+        self.assertEqual(parse.preprint_alternate_date(step_json), date_string)
+
+    def test_no_outputs(self):
+        step_json = {"actions": [{"outputs": []}]}
+        self.assertEqual(parse.preprint_alternate_date(step_json), None)
+
+    def test_none(self):
+        step_json = None
+        self.assertEqual(parse.preprint_alternate_date(step_json), None)
+
+
 class TestContentStep(unittest.TestCase):
     def test_content_step_none(self):
         d_json = None
         self.assertEqual(parse.content_step(d_json), None)
 
     def test_content_step_empty(self):
         d_json = {}
```

