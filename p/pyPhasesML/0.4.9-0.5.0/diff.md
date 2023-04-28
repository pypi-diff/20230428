# Comparing `tmp/pyPhasesML-0.4.9.tar.gz` & `tmp/pyPhasesML-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.9.tar", last modified: Sun Apr 16 16:27:15 2023, max compression
+gzip compressed data, was "pyPhasesML-0.5.0.tar", last modified: Fri Apr 28 10:07:37 2023, max compression
```

## Comparing `pyPhasesML-0.4.9.tar` & `pyPhasesML-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.589520 pyPhasesML-0.4.9/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.591520 pyPhasesML-0.4.9/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.592520 pyPhasesML-0.4.9/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    22838 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.590520 pyPhasesML-0.4.9/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 16:27:15.595520 pyPhasesML-0.4.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-16 16:26:49.000000 pyPhasesML-0.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.053188 pyPhasesML-0.5.0/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.056188 pyPhasesML-0.5.0/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.058188 pyPhasesML-0.5.0/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.059188 pyPhasesML-0.5.0/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.060189 pyPhasesML-0.5.0/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19178 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:07:37.055188 pyPhasesML-0.5.0/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-28 10:07:37.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 10:07:36.000000 pyPhasesML-0.5.0/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-28 10:07:11.000000 pyPhasesML-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:07:37.061189 pyPhasesML-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-28 10:07:13.000000 pyPhasesML-0.5.0/setup.py
```

### Comparing `pyPhasesML-0.4.9/LICENSE` & `pyPhasesML-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/PKG-INFO` & `pyPhasesML-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.9
+Version: 0.5.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.9/README.md` & `pyPhasesML-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.5.0/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/DataSet.py` & `pyPhasesML-0.5.0/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.5.0/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/Model.py` & `pyPhasesML-0.5.0/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/ModelManager.py` & `pyPhasesML-0.5.0/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/Plugin.py` & `pyPhasesML-0.5.0/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.5.0/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.5.0/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/config.yaml` & `pyPhasesML-0.5.0/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.5.0/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.5.0/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.9/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.5.0/pyPhasesML/scorer/Scorer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,58 @@
+import itertools
 import numpy as np
-from sklearn.metrics import confusion_matrix
+
+
+def confusion_matrix(true, pred, labels=None):
+    """Compute confusion matrix from truth and prediction"""
+    if labels is None:
+        labels = np.unique(np.concatenate([true, pred]))
+
+    assert true.shape == pred.shape
+
+    size = len(labels)
+    classes = np.arange(size)
+    confmat = np.zeros((size, size))
+
+    for i, j in itertools.product(range(size), range(size)):
+        confmat[i, j] = np.sum((true == classes[i]) & (pred == classes[j]))
+
+    return confmat
 
 
 class Scorer:
     title = "Segmentbasiert"
     cmScaleByClass = 4
 
     metricNameMap = {}
     addedMetrics = {}
 
+    def __init__(self, numClasses=2, classNames=None, trace=False, threshold=None) -> None:
+        self.metrics = ["kappa", "accuracy"]
+        self.ignoreClasses = []
+        self.numClasses = numClasses if classNames is None else len(classNames)
+        self.classNames = list(range(numClasses)) if classNames is None else classNames
+        self.recordResult = {}
+        self.recordIndex = 0
+        self.trace = trace
+        self.possibleValues = None
+        self.addEvents = False
+        self.mapping = None
+        self.threshold = threshold
+
     def getMetricDefinition(self, name):
         metricDefinition = {
             # init value, useAsBest, biggerIsBetter
             "AUC": [0.5, False, True],
             "AP": [0.0, True, True],
             "accuracy": [0.0, False, True],
             "acc": [0.0, False, True],
             "kappa": [-1, True, True],
             "f1": [-1, True, True],
             "CSI": [0, True, True],
-            "loss": [np.inf, True, False],
             "meanSquared": [np.inf, True, False],
             "SNR": [np.inf, False, False],
             "confusion": [np.inf, False, False],
             "auroc": [0.0, False, True],
             "auprc": [0.0, True, True],
             "eventCountDiff": [np.inf, False, False],
             "positiveErrorRatio": [np.inf, True, False],
@@ -46,35 +75,14 @@
         }
 
     def getMetricName(self, metricName):
         if metricName in Scorer.metricNameMap:
             metricName = Scorer.metricNameMap[metricName]
         return metricName
 
-    def beforeLoss(self, x, y):
-        """can be overwritten to tranform for a required format for the loss function"""
-        return x, y
-
-    def __init__(self, numClasses=None, classNames=None, trace=False, threshold=None) -> None:
-        if numClasses is None and classNames is None:
-            raise Exception("number of classes or list of classnames are required for scoring")
-
-        self.metrics = ["kappa", "accuracy"]
-        self.ignoreClasses = []
-        self.numClasses = numClasses if classNames is None else len(classNames)
-        self.classNames = [i for i in range(numClasses)] if classNames is None else classNames
-        self.recordResult = {}
-        self.recordIndex = 0
-        self.trace = trace
-        self.possibleValues = None
-        self.lossF = None
-        self.addEvents = False
-        self.mapping = None
-        self.threshold = threshold
-
     def prepareInput(self, inputArray):
         """can be overwritten to tranform tensors to numpy"""
         return inputArray
 
     def preparePrediction(self, inputArray):
         # for classification task the shape can be (recordcount?, predictions, classCount)
         isOneHotEncode = inputArray.shape[-1] == self.numClasses
@@ -169,15 +177,14 @@
             # given the above
             self.results["neg_values"] = self.results["all_values"] - self.results["pos_values"] - self.results["ign_values"]
             auroc, auprc, _, _, _ = self._auc(self.results["pos_values"], self.results["neg_values"])
             self.results["auprc"] = np.sum(auprc)
             self.results["auroc"] = np.sum(auroc)
         elif metricName in [
             "meanSquared",
-            "loss",
             "rootMeanSquared",
             "prd",
             "eventCountDiff",
             "countTruth",
             "countPred",
             "overlappingCount",
             "positiveErrorRatio",
@@ -280,14 +287,15 @@
         if useThreshold:
             return self.getClassPrediction(prediction)
 
         if self.isHotEncoded(prediction):
             prediction = prediction.argmax(-1)
         else:
             threshhold = self.threshold if useThreshold is None else 0.5
+            prediction = prediction.reshape(-1)
             if self.numClasses > 2:
                 return prediction
             else:
                 prediction[prediction >= threshhold] = 1
                 prediction[prediction < threshhold] = 0
         return prediction
 
@@ -317,32 +325,33 @@
             confusion = self.scoreMetric("confusion", truth, prediction)
             k, acc = self.calculateKappaAccFromConfusion(confusion)
             self.results["accuracy"] = acc
             self.results["kappa"] = k
         elif metricName in ["f1"]:
             f1s = []
             confusion = self.scoreMetric("confusion", truth, prediction)
-            for i in range(self.numClasses):
+            startAt = 1 if self.numClasses == 2 else 0
+            for i in range(startAt, self.numClasses):
                 # first = truth, second = predicted
                 tp = confusion[i][i]
                 fp = sum(confusion[i, :]) - tp
                 fn = sum(confusion[:, i]) - tp
                 f1 = tp / (tp + 0.5 * (fp + fn))
                 self.results["f1-%i" % i] = f1
                 f1s.append(f1)
-                self.results["f1"] = np.mean(f1s)
+            self.results["f1"] = np.mean(f1s)
         elif metricName == "confusion":
             prediction = self.flattenPrediction(prediction, threshold=self.threshold)
             result = confusion_matrix(
                 truth, prediction, labels=range(self.numClasses)
             )  # , labels=range(self.numClasses) # HPC comp
         elif metricName in ["auprc", "auroc"]:
             classLikelyhood = self.getClassLikelyhood(prediction)
 
-            scale = 10**3
+            scale = 10 ** 3
             b = scale + 1
             r = (-0.5 / scale, 1.0 + 0.5 / scale)
 
             self.results["all_values"] = np.histogram(classLikelyhood, bins=b, range=r)[0]
 
             pred_pos = classLikelyhood[truth > 0]
             self.results["pos_values"] = np.histogram(pred_pos, bins=b, range=r)[0]
@@ -353,21 +362,20 @@
 
             # Compute the histogram of probabilities in non-arousal regions,
             # given the above
             self.results["neg_values"] = self.results["all_values"] - self.results["pos_values"] - self.results["ign_values"]
             auroc, auprc, _, _, _ = self._auc(self.results["pos_values"], self.results["neg_values"])
             self.results["auprc"] = np.sum(auprc)
             self.results["auroc"] = np.sum(auroc)
-        elif metricName in ["loss"]:
-            truth, prediction = self.beforeLoss(truth, self.flattenPrediction(prediction))
-            self.results["loss"] = self.lossF(truth, prediction)
         elif metricName in ["meanSquared", "rootMeanSquared", "prd"]:
-            if len(prediction.shape) > 1:
+            if prediction.shape[1] > 1:
                 diag = np.eye(self.numClasses)
                 truth = diag[truth]
+            else:
+                prediction = self.getClassLikelyhood(prediction)
             squared = np.square(truth - prediction)
             meanSquared = squared.mean() if len(truth) > 0 else 0
             if metricName == "meanSquared":  # MS
                 self.results[metricName] = meanSquared
             elif metricName == "rootMeanSquared":  # RMS
                 self.results[metricName] = np.sqrt(meanSquared)
             elif metricName == "prd":  # Percentage RMS Difference
@@ -419,104 +427,14 @@
 
             self.results[metricName] = np.sqrt(ppv * tpr)
         if result is not None:
             self.results[metricName] = result
 
         return self.results[metricName]
 
-    def getValuesFromClasses(self):
-        if self.possibleValues is None:
-            values = []
-            for id in range(self.numClasses**2):
-                trueValue, preditedValue = (id // self.numClasses, id % self.numClasses)
-                values.append("%s as %s" % (self.classNames[trueValue], self.classNames[preditedValue]))
-            self.possibleValues = values
-
-        return self.possibleValues
-
-    # def getValidationEvents(self, truth, prediction, recordName=None):
-
-    #     validationSignal = self.numClasses * truth + prediction
-    #     validationSignal[truth == -1] = -1
-
-    #     values = self.getValuesFromClasses()
-
-    #     em = EventManager(None)
-    #     return em.getEventsFromSignal(validationSignal, values, owner=recordName)
-
-    # def confusionMatrix(self, resultEntry, labels=None, title="confusion matrix"):
-    #     confusion = resultEntry["confusion"]
-    #     labels = self.classNames
-
-    #     label_list = [labels[i] for i in range(len(labels))]
-    #     df_cm = pd.DataFrame(confusion, index=label_list, columns=label_list)
-
-    #     blue = cm.get_cmap("Blues", 256)
-    #     darkencolor = blue(np.linspace(0.3, 1, 256))
-    #     newcmp = ListedColormap(darkencolor, name="DarkenBlue")
-    #     figSize = self.numClasses * Scorer.cmScaleByClass
-    #     return pp_matrix(df_cm, title=title, figsize=[figSize, figSize], cmap=newcmp, cbar=False)
-
-    # def confusionMatrixTrailor(self, resultEntry, labels=None, title="sub confusion matrix", rowsSplit=slice(0,2), colSplit=slice(None), colNames = None, rowNames=None):
-    #     #remove NoneRow
-    #     colNames = self.classNames if colNames is None else colNames
-    #     rowNames = self.classNames if rowNames is None else rowNames
-    #     confusion = resultEntry["confusion"][colSplit, rowsSplit]
-    #     labelsCol = np.array(colNames)[colSplit]
-    #     labelsRow = np.array(rowNames)[rowsSplit]
-    #     df_cm = pd.DataFrame(confusion, index=labelsCol, columns=labelsRow)
-
-    #     blue = cm.get_cmap("Blues", 256)
-    #     darkencolor = blue(np.linspace(0.3, 1, 256))
-    #     newcmp = ListedColormap(darkencolor, name="DarkenBlue")
-    #     figSizeL = (len(labelsCol) + 1 ) * Scorer.cmScaleByClass
-    #     figSizeH = (len(labelsRow) +  1) * Scorer.cmScaleByClass
-    #     return pp_matrix(df_cm, title=title, figsize=[figSizeL, figSizeH], cmap=newcmp, cbar=False)
-
-    # def prCurve(self, resultEntry, title="ROC"):
-    #     _, _, precision, _, recall = self._auc(resultEntry["pos_values"], resultEntry["neg_values"])
-    #     fig = plt.figure(figsize=(6, 6))
-    #     lw = 2
-    #     plt.plot(
-    #         recall,
-    #         precision,
-    #         color="darkorange",
-    #         lw=lw,
-    #         label=title,
-    #     )
-    #     plt.xlim([0.0, 1.0])
-    #     plt.ylim([0.0, 1.05])
-    #     plt.xlabel("Recall")
-    #     plt.ylabel("Precision")
-    #     plt.title("Precision/Recall Curve")
-    #     plt.legend(loc="lower right")
-
-    #     return fig
-
-    # def rocCurve(self, resultEntry, title="ROC"):
-    #     _, _, tpr, fpr, _ = self._auc(resultEntry["pos_values"], resultEntry["neg_values"])
-
-    #     fig = plt.figure(figsize=(6, 6))
-    #     lw = 2
-    #     plt.plot(
-    #         fpr,
-    #         tpr,
-    #         color="darkorange",
-    #         lw=lw,
-    #         label=title,
-    #     )
-    #     plt.plot([0, 1], [0, 1], color="navy", lw=lw, linestyle="--")
-    #     plt.xlim([0.0, 1.0])
-    #     plt.ylim([0.0, 1.05])
-    #     plt.xlabel("False Positive Rate")
-    #     plt.ylabel("True Positive Rate")
-    #     plt.title("Receiver operating characteristic")
-    #     plt.legend(loc="lower right")
-    #     return fig
-
     def _auc(self, pos_values, neg_values):
         # Calculate areas under the ROC and PR curves by iterating
         # over the possible threshold values.
 
         # At the minimum threshold value, all samples are classified as
         # positive, and thus TPR = 1 and TNR = 0.
         tp = np.sum(pos_values)
```

### Comparing `pyPhasesML-0.4.9/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.5.0/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.9
+Version: 0.5.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.9/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.5.0/pyPhasesML.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pyPhasesML/DataAugmentation.py
 pyPhasesML/DataSet.py
+pyPhasesML/DataversionManager.py
 pyPhasesML/FeatureExtraction.py
 pyPhasesML/Model.py
 pyPhasesML/ModelManager.py
 pyPhasesML/Plugin.py
 pyPhasesML/SignalPreprocessing.py
 pyPhasesML/__init__.py
 pyPhasesML/config.yaml
@@ -17,14 +18,19 @@
 pyPhasesML.egg-info/dependency_links.txt
 pyPhasesML.egg-info/requires.txt
 pyPhasesML.egg-info/top_level.txt
 pyPhasesML/adapter/ModelKerasAdapter.py
 pyPhasesML/adapter/ModelTf1Adapter.py
 pyPhasesML/adapter/ModelTorchAdapter.py
 pyPhasesML/adapter/__init__.py
+pyPhasesML/datapipes/Augmentor.py
+pyPhasesML/datapipes/DatasetXY.py
+pyPhasesML/datapipes/FoldMapper.py
+pyPhasesML/datapipes/RecordMap.py
+pyPhasesML/datapipes/__init__.py
 pyPhasesML/exporter/MemmapRecordExporter.py
 pyPhasesML/exporter/ModelExporter.py
 pyPhasesML/exporter/__init__.py
 pyPhasesML/scorer/Scorer.py
 pyPhasesML/scorer/ScorerTF.py
 pyPhasesML/scorer/ScorerTorch.py
 pyPhasesML/scorer/__init__.py
```

### Comparing `pyPhasesML-0.4.9/setup.py` & `pyPhasesML-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.9"[1:],
+    version="v0.5.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
     package_data={"": ["*.yaml"]},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pyPhases", "scikit-learn", "typeguard"],
+    install_requires=["pyPhases", "typeguard"],
     python_requires=">=3.5",
 )
```

