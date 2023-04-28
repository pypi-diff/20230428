# Comparing `tmp/insights-extractor-0.1.1.tar.gz` & `tmp/insights-extractor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-pq31s1ul/insights-extractor-0.1.1.tar", last modified: Fri Apr 14 04:09:28 2023, max compression
+gzip compressed data, was "/home/runner/work/insights-extractor/insights-extractor/dist/.tmp-sryaqbai/insights-extractor-0.1.2.tar", last modified: Fri Apr 28 14:08:58 2023, max compression
```

## Comparing `insights-extractor-0.1.1.tar` & `insights-extractor-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/dist/insights-extractor-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/dist/insights_extractor-0.1.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/prep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/classification/utils/keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/document/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/ner/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/pre_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/nlp/stopwords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/settings/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/extractlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/extractlib/utils/temp_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/insights_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:09:28.000000 insights-extractor-0.1.1/src/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 04:09:13.000000 insights-extractor-0.1.1/src/requirements/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/dist/insights-extractor-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/dist/insights_extractor-0.1.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/classification/prep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/classification/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/classification/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/classification/utils/keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/document/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/document/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/document/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/document/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/nlp/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/nlp/stopwords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/settings/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/extractlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/extractlib/utils/temp_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/insights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/src/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/src/requirements/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:08:58.000000 insights-extractor-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/tests/pre_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/tests/prep_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-28 14:08:41.000000 insights-extractor-0.1.2/tests/table.py
```

### Comparing `insights-extractor-0.1.1/.github/workflows/python-publish.yml` & `insights-extractor-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.1/LICENSE` & `insights-extractor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.1/PKG-INFO` & `insights-extractor-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
-Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
+Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,22 +20,26 @@
 
 
 ## Dependency Overview
 ### Python Dependency Install
 This project leverages packages 
 <pre>
 nltk == 3.8.1 
+spacy == 3.5.2
 PyMuPDF == 1.21.1 
 camelot-py == 0.11.0 
 opencv-python == 4.7.0.72 
 ghostscript == 0.7
 </pre>
 
 ## manually install supporting binaries
 
+### spacy dependencies
+<pre>python -m spacy download en_core_web_sm</pre>
+
 ### camelot dependencies
 - https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
 
 #### Ubuntu
 <pre>$ apt install ghostscript python3-tk</pre>
 
 #### MacOS
```

### Comparing `insights-extractor-0.1.1/README.md` & `insights-extractor-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 
 
 ## Dependency Overview
 ### Python Dependency Install
 This project leverages packages 
 <pre>
 nltk == 3.8.1 
+spacy == 3.5.2
 PyMuPDF == 1.21.1 
 camelot-py == 0.11.0 
 opencv-python == 4.7.0.72 
 ghostscript == 0.7
 </pre>
 
 ## manually install supporting binaries
 
+### spacy dependencies
+<pre>python -m spacy download en_core_web_sm</pre>
+
 ### camelot dependencies
 - https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
 
 #### Ubuntu
 <pre>$ apt install ghostscript python3-tk</pre>
 
 #### MacOS
```

### Comparing `insights-extractor-0.1.1/dist/insights-extractor-0.1.0.tar.gz` & `insights-extractor-0.1.2/dist/insights-extractor-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.1/dist/insights_extractor-0.1.0-py3-none-any.whl` & `insights-extractor-0.1.2/dist/insights_extractor-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.1/pyproject.toml` & `insights-extractor-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
+  "spacy == 3.5.2; python_version >= '3.7'",
   "nltk == 3.8.1; python_version >= '3.7'",
   "PyMuPDF == 1.21.1; python_version >= '3.7'",
   "camelot-py == 0.11.0; python_version >= '3.6'",
   "opencv-python == 4.7.0.72; python_version >= '3.6'",
   "ghostscript == 0.7; python_version >= '3.6'"
 ]
 name = "insights-extractor"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Trae Moore", email="trae.dev@gmail.com" },
 ]
 description = "Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities."
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["nltk", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
+keywords = ["nltk", "spaCy", "Pymupdf", "Camelot", "OpenCV", "Ghostscript", "insight-extractor", "pdf extraction", "pdf data extraction", "pdf data", "classification", "keyword extraction"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `insights-extractor-0.1.1/src/extractlib/document/page.py` & `insights-extractor-0.1.2/src/extractlib/document/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,16 +122,14 @@
                     # Add the line to the list of extracted lines
                     collection.append(data)
 
     
 
     # Sort the lines by y-coordinate and then x-coordinate
     sorted_page_elements = sorted(page_lines, key=lambda line: (-line['bbox'][3], line['bbox'][0]))
-    # Sort the table_lines by y-coordinate (top to bottom) and then x-coordinate (left to right)
-    #sorted_table_lines = sorted(table_lines, key=lambda line: (-line['bbox'][1], line['bbox'][0]))
 
     # Return the sorted lines
     return sorted_page_elements, table_lines
 
 
 def _in_table(line, tables):
     """
```

### Comparing `insights-extractor-0.1.1/src/extractlib/document/process.py` & `insights-extractor-0.1.2/src/extractlib/document/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             tables = get_table_data(raw_tables)
 
             # Extract lines from the PDF page
             lines, table_lines = extract_lines(file_path, [Table(table._bbox, table.order)
                                   for table in raw_tables])
 
             tables = corrilate_table_data(table_lines, tables)
-
+            print(json.dumps(tables, indent=4))
             # Cleanse and tag the lines JSON structure
             cleanse_and_tag_json_structure(lines)
 
             images = get_images(file_path)
 
             # Store the extracted data in the dictionary
             data = {
```

### Comparing `insights-extractor-0.1.1/src/extractlib/document/table.py` & `insights-extractor-0.1.2/src/extractlib/document/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 
 
 def corrilate_table_data(table_elements, table_data):
     # Initialize an empty dictionary to store tables
     tables = {}
     
+    if not table_elements or not table_data:
+        raise ValueError('table_elements and table_data cannot be None.')
+
     # Iterate through each table in table_data
     tbl_idx = 0
     while tbl_idx < len(table_data):
         table = table_data[tbl_idx]
 
         # Iterate through each row in the table's JSON data
         row_idx = 0
@@ -115,14 +118,8 @@
             'valid': True,
             'table': idx,
             'json': jsonData,
             'classification_training_data': cleaned
         }
 
         result_tables.append(table)
-    return result_tables
-
-def _col_contains_target(col, target):
-    try:
-        return col.index(target)
-    except Exception:
-        return -1
+    return result_tables
```

### Comparing `insights-extractor-0.1.1/src/extractlib/document/utils.py` & `insights-extractor-0.1.2/src/extractlib/document/utils.py`

 * *Files identical despite different names*

### Comparing `insights-extractor-0.1.1/src/extractlib/ner/__init__.py` & `insights-extractor-0.1.2/src/extractlib/ner/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 
 from nlp.stopwords import get_words
 
 nltk.download('averaged_perceptron_tagger')
 nltk.download('maxent_ne_chunker')
 nltk.download('words')
 
-stopwords = get_words()
-
 def get_entities(content):
     """
     Extract entities from text using NLTK.
 
     Args:
         text (str): The text to extract entities from.
 
     Returns:
         list: A list of entities.
     """
+    stopwords = get_words()
     try:
         entities = []
 
         words = word_tokenize(content)  
         words = [word for word in words if word.lower() not in stopwords]
 
-        for token in nltk.sent_tokenize(content):
+        for token in nltk.sent_tokenize(' '.join(words)):
             for chunk in nltk.ne_chunk(pos_tag(word_tokenize(token))):
                 if hasattr(chunk, 'label'):
                     entities.append((' '.join(c[0] for c in chunk), chunk.label()))
         return entities
     except Exception as e:
         print(f'Error processing: {e}')
         raise e
```

### Comparing `insights-extractor-0.1.1/src/extractlib/nlp/pre_process.py` & `insights-extractor-0.1.2/src/extractlib/nlp/pre_process.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,30 +11,29 @@
         remove_punctuation (bool): Whether to remove punctuation from the text (default=False).
         regex_list (list): A list of regex patterns to match against the input text (default=None).
 
     Returns:
         str: The cleaned text string.
     """
 
+    if regex_list is not None:
+        # Remove any substrings that match a regex pattern
+        for pattern in regex_list:
+            text = re.sub(pattern, '', text)
+
     # Remove all single quotes from the text
-    re.sub(r"'", "", text)
+    result = re.sub(r"'", "", text)
 
     # Remove all new line characters from the text
-    text = re.sub('\n', ' ', text)
-
-    # Remove any extra whitespace from the text
-    text = re.sub('\s+', ' ', text).strip()
+    result = re.sub('\n', ' ', result)
 
     if remove_punctuation:
-        # Remove all punctuation from the text
-        text = text.translate(str.maketrans('', '', string.punctuation))
-
-    if regex_list is not None:
-        # Remove any substrings that match a regex pattern
-        for pattern in regex_list:
-            text = re.sub(pattern, '', text)
+    # Remove all punctuation from the text
+        result = result.translate(str.maketrans('', '', string.punctuation))
 
     # Remove any non-ASCII characters from the text
-    text = text.encode('ascii', 'ignore').decode()
-
+    result = result.encode('ascii', 'ignore').decode()
+    
+    result = re.sub(r'\s+', ' ', result).strip()
+    result = re.sub(r'\t+', ' ', result).strip()
     # Return the cleaned text string
-    return text
+    return result
```

### Comparing `insights-extractor-0.1.1/src/extractlib/utils/json_utils.py` & `insights-extractor-0.1.2/src/extractlib/utils/json_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,74 +21,88 @@
         for item in json_obj:
             extract_json_values(item, result_str)
     else:
         result_str.append(json_obj)
     return ' '.join(result_str).lower()
 
 
-def extract_text_elements(elements, element_valid):
-    result = []
-    for element in elements:
-        if 'text' in element and element_valid(element):
-            result.append(element['text'])
+def extract_text(json, element_valid):
+    # Initialize an empty list to store the text values
+    texts = []
+    
+    # Recursively search the data for 'text' keys and append their values to the 'texts' list
+    def search_for_text(obj):
+        if isinstance(obj, dict):
+            for key, value in obj.items():
+                if key == 'text' and element_valid(obj):
+                    texts.append(value)
+                else:
+                    search_for_text(value)
+        elif isinstance(obj, list):
+            for item in obj:
+                search_for_text(item)
+    
+    # Call the search_for_text function on the parsed data
+    search_for_text(json)
+    
+    # Return the list of text values
+    return texts
 
+
+def extract_text_elements(elements, element_valid):
+    result = extract_text(elements, element_valid)
     return ' '.join(result)
 
 
-def cleanse_and_tag_json_structure(data):
+def cleanse_and_tag_json_structure(data, validation_regexs=[]):
     """
     Evaluate a JSON data structure for invalid content and tag it with validity information.
 
     Args:
         data (dict or list): A dictionary or list containing the JSON data structure to cleanse.
 
     Returns: None
 
-    Example: { "valid": true | false, "item1": ..., "item2": ..., ... }
+    Example: { "item1": {"valid" : true | false }, "item1": ..., "item2": ..., ... }
     """
-
+    regexs = config.invalid_content_regexs if not validation_regexs else list(set(config.invalid_content_regexs + validation_regexs))
+   
     # Check if the data is a dictionary
     if isinstance(data, dict):
-        keys_to_remove = []
-
         # Loop over the dictionary keys and values
-        for key, value in data.items():
+        for key, value in data.items(): 
             # If the value is a string
             if isinstance(value, str):
                 # Check if the string contains any invalid content
-                if test_for_invalid_content(value, config.invalid_content_regexs):
+                if test_for_invalid_content(value, regexs):
                     # If the string contains invalid content, tag the entire data structure as invalid
-                    data["valid"] = False
+                    data.update({"valid": False})
                 else:
                     # Otherwise, clean the string using the clean_text function and update the dictionary value
                     data[key] = clean_text(value, False)
             else:
                 # If the value is not a string, recurse into the data structure to cleanse and tag nested values
-                cleanse_and_tag_json_structure(value)
-
-        # Remove any keys that were flagged for removal during the loop
-        for key in keys_to_remove:
-            del data[key]
+                cleanse_and_tag_json_structure(value, regexs)
 
     # Check if the data is a list
     elif isinstance(data, list):
         # Loop over the list items
         for i, value in enumerate(data):
             # If the list item is a string
             if isinstance(value, str):
                 # Check if the string contains any invalid content
-                if test_for_invalid_content(value, config.invalid_content_regexs):
+                if test_for_invalid_content(value, regexs):
                     # If the string contains invalid content, tag the entire data structure as invalid
                     data["valid"] = False
                 else:
                     # Otherwise, clean the string using the clean_text function and update the list item
                     data[i] = clean_text(value, False)
             else:
                 # If the list item is not a string, recurse into the data structure to cleanse and tag nested values
-                cleanse_and_tag_json_structure(value)
+                cleanse_and_tag_json_structure(value, regexs)
 
 
 def test_for_invalid_content(text, regex_list=[]):
     """
     Check if a string contains any invalid content based on a list of regex statements.
 
     Args:
```

### Comparing `insights-extractor-0.1.1/src/insights_extractor.egg-info/PKG-INFO` & `insights-extractor-0.1.2/src/insights_extractor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: insights-extractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficient PDF analysis, text extraction, preprocessing, and pattern recognition with customizable configurations and utilities.
 Author-email: Trae Moore <trae.dev@gmail.com>
 Project-URL: Homepage, https://github.com/traemoore/insights-extractor
 Project-URL: Tests, https://github.com/traemoore/insights-extractor-test
 Project-URL: Bug Tracker, https://github.com/traemoore/insights-extractor/issues
-Keywords: nltk,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
+Keywords: nltk,spaCy,Pymupdf,Camelot,OpenCV,Ghostscript,insight-extractor,pdf extraction,pdf data extraction,pdf data,classification,keyword extraction
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,22 +20,26 @@
 
 
 ## Dependency Overview
 ### Python Dependency Install
 This project leverages packages 
 <pre>
 nltk == 3.8.1 
+spacy == 3.5.2
 PyMuPDF == 1.21.1 
 camelot-py == 0.11.0 
 opencv-python == 4.7.0.72 
 ghostscript == 0.7
 </pre>
 
 ## manually install supporting binaries
 
+### spacy dependencies
+<pre>python -m spacy download en_core_web_sm</pre>
+
 ### camelot dependencies
 - https://camelot-py.readthedocs.io/en/master/user/install-deps.html#install-deps
 
 #### Ubuntu
 <pre>$ apt install ghostscript python3-tk</pre>
 
 #### MacOS
```

### Comparing `insights-extractor-0.1.1/src/insights_extractor.egg-info/SOURCES.txt` & `insights-extractor-0.1.2/src/insights_extractor.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -27,8 +27,12 @@
 src/extractlib/utils/json_utils.py
 src/extractlib/utils/temp_dir.py
 src/insights_extractor.egg-info/PKG-INFO
 src/insights_extractor.egg-info/SOURCES.txt
 src/insights_extractor.egg-info/dependency_links.txt
 src/insights_extractor.egg-info/requires.txt
 src/insights_extractor.egg-info/top_level.txt
-src/requirements/requirements.txt
+src/requirements/requirements.txt
+tests/__init__.py
+tests/pre_process.py
+tests/prep_utils.py
+tests/table.py
```

