# Comparing `tmp/numalogic_prometheus-0.3.2.tar.gz` & `tmp/numalogic_prometheus-0.3.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.3.2.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.3.2a0.tar", max compression
```

## Comparing `numalogic_prometheus-0.3.2.tar` & `numalogic_prometheus-0.3.2a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-27 23:33:43.486648 numalogic_prometheus-0.3.2/LICENSE
--rw-r--r--   0        0        0      839 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/__init__.py
--rw-r--r--   0        0        0     1395 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/_config.py
--rw-r--r--   0        0        0      561 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0     1316 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/clients/redis.py
--rw-r--r--   0        0        0     1342 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/clients/sentinel.py
--rw-r--r--   0        0        0     2145 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0      382 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/default-configs/pipeline_config.yaml
--rw-r--r--   0        0        0     4483 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/factory.py
--rw-r--r--   0        0        0     8855 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      741 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/filter.py
--rw-r--r--   0        0        0     4148 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6982 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     1887 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     3431 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4321 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     5616 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udsink/train.py
--rw-r--r--   0        0        0     7808 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     5935 2023-04-27 23:33:43.490649 numalogic_prometheus-0.3.2/numaprom/watcher.py
--rw-r--r--   0        0        0     1540 2023-04-27 23:33:43.494649 numalogic_prometheus-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-26 22:19:51.663205 numalogic_prometheus-0.3.2a0/LICENSE
+-rw-r--r--   0        0        0      839 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/__init__.py
+-rw-r--r--   0        0        0     1395 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_config.py
+-rw-r--r--   0        0        0      561 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0     1316 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     1342 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py
+-rw-r--r--   0        0        0     2145 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0      382 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/default-configs/pipeline_config.yaml
+-rw-r--r--   0        0        0     4483 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/factory.py
+-rw-r--r--   0        0        0     8855 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      741 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     4148 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     6982 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     1887 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     3431 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4321 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     5616 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     7808 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5935 2023-04-26 22:19:51.667205 numalogic_prometheus-0.3.2a0/numaprom/watcher.py
+-rw-r--r--   0        0        0     1542 2023-04-26 22:19:51.671205 numalogic_prometheus-0.3.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.2a0/PKG-INFO
```

### Comparing `numalogic_prometheus-0.3.2/LICENSE` & `numalogic_prometheus-0.3.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/__init__.py` & `numalogic_prometheus-0.3.2a0/numaprom/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/_config.py` & `numalogic_prometheus-0.3.2a0/numaprom/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/_constants.py` & `numalogic_prometheus-0.3.2a0/numaprom/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/clients/redis.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/clients/sentinel.py` & `numalogic_prometheus-0.3.2a0/numaprom/clients/sentinel.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/configs/config.yaml` & `numalogic_prometheus-0.3.2a0/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.3.2a0/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/entities.py` & `numalogic_prometheus-0.3.2a0/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/factory.py` & `numalogic_prometheus-0.3.2a0/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/tools.py` & `numalogic_prometheus-0.3.2a0/numaprom/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/filter.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/inference.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/threshold.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/threshold.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udf/window.py` & `numalogic_prometheus-0.3.2a0/numaprom/udf/window.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udsink/train.py` & `numalogic_prometheus-0.3.2a0/numaprom/udsink/train.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.3.2a0/numaprom/udsink/train_rollout.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/numaprom/watcher.py` & `numalogic_prometheus-0.3.2a0/numaprom/watcher.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.3.2/pyproject.toml` & `numalogic_prometheus-0.3.2a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.3.2"
+version = "0.3.2a0"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
```

### Comparing `numalogic_prometheus-0.3.2/PKG-INFO` & `numalogic_prometheus-0.3.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.3.2
+Version: 0.3.2a0
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
```

