# Comparing `tmp/gate_drift-0.1.3.tar.gz` & `tmp/gate_drift-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gate_drift-0.1.3.tar", max compression
+gzip compressed data, was "gate_drift-0.1.4.tar", max compression
```

## Comparing `gate_drift-0.1.3.tar` & `gate_drift-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-04-20 19:33:25.531694 gate_drift-0.1.3/LICENSE
--rw-r--r--   0        0        0     1595 2023-04-20 00:23:42.803802 gate_drift-0.1.3/README.md
--rw-r--r--   0        0        0      183 2023-04-19 23:37:10.238460 gate_drift-0.1.3/gate/__init__.py
--rw-r--r--   0        0        0    14182 2023-04-20 19:33:25.546152 gate_drift-0.1.3/gate/drift.py
--rw-r--r--   0        0        0      961 2023-04-20 19:33:25.546362 gate_drift-0.1.3/gate/statistics.py
--rw-r--r--   0        0        0     2357 2023-04-20 00:24:26.178857 gate_drift-0.1.3/gate/summarize.py
--rw-r--r--   0        0        0     7581 2023-04-20 19:33:25.546579 gate_drift-0.1.3/gate/summary.py
--rw-r--r--   0        0        0     1018 2023-04-20 19:34:04.471017 gate_drift-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 gate_drift-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-20 19:33:25.531694 gate_drift-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1965 2023-04-28 01:13:54.722939 gate_drift-0.1.4/README.md
+-rw-r--r--   0        0        0      244 2023-04-27 01:03:41.538087 gate_drift-0.1.4/gate/__init__.py
+-rw-r--r--   0        0        0    21635 2023-04-28 00:57:06.998900 gate_drift-0.1.4/gate/drift.py
+-rw-r--r--   0        0        0     5223 2023-04-27 23:14:25.758176 gate_drift-0.1.4/gate/statistics.py
+-rw-r--r--   0        0        0     4084 2023-04-28 00:57:06.780878 gate_drift-0.1.4/gate/summarize.py
+-rw-r--r--   0        0        0    16145 2023-04-28 00:57:07.107493 gate_drift-0.1.4/gate/summary.py
+-rw-r--r--   0        0        0     1051 2023-04-28 01:20:50.855647 gate_drift-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 gate_drift-0.1.4/PKG-INFO
```

### Comparing `gate_drift-0.1.3/LICENSE` & `gate_drift-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.3/README.md` & `gate_drift-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 [![GATE](https://github.com/dm4ml/gate/workflows/gate/badge.svg)](https://github.com/dm4ml/gate/actions?query=workflow:"gate")
 [![lint (via ruff)](https://github.com/dm4ml/gate/workflows/lint/badge.svg)](https://github.com/dm4ml/gate/actions?query=workflow:"lint")
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 GATE is a Python module that detects drift in partitions of data. GATE computes partition summaries, which are then fed into an anomaly detection algorithm to detect whether a new partition is anomalous. This minimizes false positive alerts when detecting drift in machine learning (ML) pipelines, where there may be many features and prediction columns.
 
+### Support for Embeddings
+
+We now support drift detection on embeddings, in addition to structured data. GATE considers _both_ the structured data and the embeddings when computing partition summaries and detecting drift. Check out the [embeddings page](./embedding) for a walkthrough of how to use GATE with embeddings.
+
 ## Installation
 
 GATE is available on PyPI and can be installed with pip:
 
 ```bash
 pip install gate-drift
 ```
 
+Note that GATE requires Python 3.8 or higher.
+
 ## Usage
 
 GATE is designed to be used with [Pandas](https://pandas.pydata.org/) dataframes. Check out the [documentation](https://dm4ml.github.io/gate/) for a walkthrough of how to use GATE.
 
 ## Research Contributions
 
 GATE was developed and is maintained by researchers at the UC Berkeley [EPIC Lab](https://epic.berkeley.edu/).
```

### Comparing `gate_drift-0.1.3/pyproject.toml` & `gate_drift-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gate-drift"
-version = "0.1.3"
+version = "0.1.4"
 description = "Data drift detection tool for machine learning pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gate"}]
 
 [tool.poetry.dependencies]
@@ -24,14 +24,15 @@
 seaborn = "^0.12.2"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
 mkdocstrings = "^0.21.2"
 pytkdocs = "^0.16.1"
 linkchecker = "^10.2.1"
 mkdocstrings-python = "^0.9.0"
+pytest-rerunfailures = "^11.1.2"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.black]
 max-line-length = 88
 preview = true
```

### Comparing `gate_drift-0.1.3/PKG-INFO` & `gate_drift-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gate-drift
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data drift detection tool for machine learning pipelines.
 License: MIT
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,22 +24,28 @@
 
 [![GATE](https://github.com/dm4ml/gate/workflows/gate/badge.svg)](https://github.com/dm4ml/gate/actions?query=workflow:"gate")
 [![lint (via ruff)](https://github.com/dm4ml/gate/workflows/lint/badge.svg)](https://github.com/dm4ml/gate/actions?query=workflow:"lint")
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 GATE is a Python module that detects drift in partitions of data. GATE computes partition summaries, which are then fed into an anomaly detection algorithm to detect whether a new partition is anomalous. This minimizes false positive alerts when detecting drift in machine learning (ML) pipelines, where there may be many features and prediction columns.
 
+### Support for Embeddings
+
+We now support drift detection on embeddings, in addition to structured data. GATE considers _both_ the structured data and the embeddings when computing partition summaries and detecting drift. Check out the [embeddings page](./embedding) for a walkthrough of how to use GATE with embeddings.
+
 ## Installation
 
 GATE is available on PyPI and can be installed with pip:
 
 ```bash
 pip install gate-drift
 ```
 
+Note that GATE requires Python 3.8 or higher.
+
 ## Usage
 
 GATE is designed to be used with [Pandas](https://pandas.pydata.org/) dataframes. Check out the [documentation](https://dm4ml.github.io/gate/) for a walkthrough of how to use GATE.
 
 ## Research Contributions
 
 GATE was developed and is maintained by researchers at the UC Berkeley [EPIC Lab](https://epic.berkeley.edu/).
```

