# Comparing `tmp/inventronet-0.0.7a0.tar.gz` & `tmp/inventronet-0.0.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventronet-0.0.7a0.tar", last modified: Fri Apr 28 07:58:42 2023, max compression
+gzip compressed data, was "inventronet-0.0.8a0.tar", last modified: Fri Apr 28 13:19:44 2023, max compression
```

## Comparing `inventronet-0.0.7a0.tar` & `inventronet-0.0.8a0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.702281 inventronet-0.0.7a0/inventronet/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.702281 inventronet-0.0.7a0/inventronet/activations/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/activations/tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/layers/shape_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/losses/mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/metrics/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/models/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/optimizers/stochastic_gradient_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/inventronet/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/preprocessing/count_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/inventronet/preprocessing/data_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.702281 inventronet-0.0.7a0/inventronet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-28 07:58:42.000000 inventronet-0.0.7a0/inventronet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 07:58:42.000000 inventronet-0.0.7a0/inventronet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:58:42.000000 inventronet-0.0.7a0/inventronet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 07:58:42.000000 inventronet-0.0.7a0/inventronet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 07:58:42.000000 inventronet-0.0.7a0/inventronet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/tests/activations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/activations/test_tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.706281 inventronet-0.0.7a0/tests/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/layers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/layers/test_batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/layers/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/layers/test_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/tests/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/losses/test_binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/losses/test_categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/losses/test_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/losses/test_mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/metrics/test_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/models/test_sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/tests/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/optimizers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/optimizers/test_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/optimizers/test_stochastic_gradient_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:42.710281 inventronet-0.0.7a0/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/preprocessing/test_count_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 07:58:31.000000 inventronet-0.0.7a0/tests/preprocessing/test_train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.869126 inventronet-0.0.8a0/inventronet/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/activations/tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/layers/shape_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/losses/mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/metrics/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/models/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.873126 inventronet-0.0.8a0/inventronet/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/optimizers/stochastic_gradient_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/inventronet/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/preprocessing/count_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/inventronet/preprocessing/data_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.869126 inventronet-0.0.8a0/inventronet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-28 13:19:44.000000 inventronet-0.0.8a0/inventronet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 13:19:44.000000 inventronet-0.0.8a0/inventronet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:19:44.000000 inventronet-0.0.8a0/inventronet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 13:19:44.000000 inventronet-0.0.8a0/inventronet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 13:19:44.000000 inventronet-0.0.8a0/inventronet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/activations/test_tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/layers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/layers/test_batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/layers/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/layers/test_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/losses/test_binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/losses/test_categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/losses/test_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/losses/test_mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/metrics/test_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/models/test_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/optimizers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/optimizers/test_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/optimizers/test_stochastic_gradient_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:44.877126 inventronet-0.0.8a0/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/preprocessing/test_count_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 13:19:29.000000 inventronet-0.0.8a0/tests/preprocessing/test_train_test_split.py
```

### Comparing `inventronet-0.0.7a0/LICENSE` & `inventronet-0.0.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/PKG-INFO` & `inventronet-0.0.8a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 Author-email: haitham.hyder@uni.minerva.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inventronet-0.0.7a0/README.md` & `inventronet-0.0.8a0/README.md`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/activation.py` & `inventronet-0.0.8a0/inventronet/activations/activation.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/leaky_relu.py` & `inventronet-0.0.8a0/inventronet/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/linear.py` & `inventronet-0.0.8a0/inventronet/activations/linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/relu.py` & `inventronet-0.0.8a0/inventronet/activations/relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/sigmoid.py` & `inventronet-0.0.8a0/inventronet/activations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/softmax.py` & `inventronet-0.0.8a0/inventronet/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/activations/tanh.py` & `inventronet-0.0.8a0/inventronet/activations/tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/layers/batch_normalization.py` & `inventronet-0.0.8a0/inventronet/layers/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/layers/dense.py` & `inventronet-0.0.8a0/inventronet/layers/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Callable, Dict, Tuple, Type
+from typing import Callable, Dict, Tuple
+
 import numpy as np
 
-from ..activations.activation import Activation
 from .layer import Layer
+from ..activations.activation import Activation
 
 
 class Dense(Layer):
     def __init__(
-        self,
-        input_dim: int,
-        output_dim: int,
-        activation: Type[Activation] = None,
-        use_bias: bool = True,
-        weight_initializer: Callable = np.random.uniform,
-        bias_initializer: Callable = np.zeros,
+            self,
+            input_dim: int,
+            output_dim: int,
+            activation: Activation = None,
+            use_bias: bool = True,
+            weight_initializer: Callable = np.random.uniform,
+            bias_initializer: Callable = np.zeros,
     ) -> None:
         """Initialize the dense layer with the given arguments.
 
         Args:
             input_dim: The dimension of the input features.
             output_dim: The dimension of the output features.
             activation: The activation function for the layer.
```

### Comparing `inventronet-0.0.7a0/inventronet/layers/dropout.py` & `inventronet-0.0.8a0/inventronet/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/layers/layer.py` & `inventronet-0.0.8a0/inventronet/layers/layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from abc import ABC, abstractmethod
-from typing import Tuple, Type
+from typing import Tuple
 
 import numpy as np
 
 from ..activations.activation import Activation
 
 
 class Layer(ABC):
 
     @abstractmethod
     def __init__(
             self,
             input_dim: int,
             output_dim: int,
-            activation: Type[Activation],
+            activation: Activation,
     ) -> None:
         """Initialize the layer with the given arguments.
 
         Args:
             input_dim: The dimension of the input features.
             output_dim: The dimension of the output features.
             activation: The activation function for the layer.
         """
         self.input_dim: int = input_dim
         self.output_dim: int = output_dim
-        self.activation: Type[Activation] = activation
+        self.activation: Activation = activation
         self.parameters = None
         self.gradients = None
 
         self.previous_layer_output = None
 
     @abstractmethod
     def forward(self, inputs: np.ndarray, training: bool = False) -> np.ndarray:
```

### Comparing `inventronet-0.0.7a0/inventronet/losses/binary_cross_entropy.py` & `inventronet-0.0.8a0/inventronet/losses/binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/losses/categorical_cross_entropy.py` & `inventronet-0.0.8a0/inventronet/losses/categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/losses/loss.py` & `inventronet-0.0.8a0/inventronet/losses/loss.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/losses/mean_absolute_error.py` & `inventronet-0.0.8a0/inventronet/losses/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/losses/mean_squared_error.py` & `inventronet-0.0.8a0/inventronet/losses/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/models/model.py` & `inventronet-0.0.8a0/inventronet/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         """
         raise NotImplementedError("The add method must be implemented.")
 
     # Define an abstract method for compiling the model with a loss
     # function and a metric
     @abstractmethod
     def compile(
-            self, loss: Loss, optimizer: Optimizer, metrics: List[Type[Metric]]
+            self, loss: Loss, optimizer: Optimizer, metrics: List[Metric]
     ) -> None:
         """Compile the model with a loss function and a metric.
 
         Args:
             loss (Loss): The loss function to be used.
             optimizer (Optimizer): The optimizer to be used.
             metrics (Metric): The metrics to be used.
```

### Comparing `inventronet-0.0.7a0/inventronet/models/sequential.py` & `inventronet-0.0.8a0/inventronet/models/sequential.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Define a class for a sequential model
 import math
-from typing import List, Tuple, Type
+from typing import List, Tuple
 
 import numpy as np
 from tqdm import tqdm
 
 from .model import Model
 from ..layers.layer import Layer
 from ..losses.loss import Loss
@@ -23,17 +23,17 @@
 
 class Sequential(Model):
     # Define the initialization method
     def __init__(self) -> None:
         """Call the superclass constructor."""
         # Call the superclass constructor
         super().__init__()
-        self.metrics: List[Type[Metric]] = None
-        self.optimizer: Type[Optimizer] = None
-        self.loss: Type[Loss] = None
+        self.metrics: List[Metric] = None
+        self.optimizer: Optimizer = None
+        self.loss: Loss = None
         # Attributes for early stopping
         self.patience: int = None
         self.min_delta: float = None
         self.wait: int = 0
         self.best_loss: float = np.inf
 
         # Attribute for history
@@ -70,15 +70,15 @@
                 assert (
                         layer.input_dim == previous_layer.output_dim
                 ), "Layer input dimension does not match previous layer output dimension"
         # Append the layer to the list of layers
         self.layers.append(layer)
 
     def compile(
-            self, loss: Type[Loss], optimizer: Type[Optimizer], metrics: List[Type[Metric]]
+            self, loss: Loss, optimizer: Optimizer, metrics: List[Metric]
     ) -> None:
         """Compile the model with a loss function, an optimizer, and metrics.
 
         Args:
             loss (Loss): The loss function to be used.
             optimizer (Optimizer): The optimizer to be used.
             metrics (List[Metric]): The metrics to be used.
@@ -146,32 +146,19 @@
                         layer.previous_layer_output
                         if layer.previous_layer_output is not None
                         else x_batch
                     )
                     layer_error = layer.backward(layer_error, prev_output=layer_input)
 
                     # Check shapes before updating the optimizer
-                    for key in layer.parameters.keys():
-                        assert layer.parameters[key].shape == layer.gradients[
-                            key].shape, f"Parameter shape {layer.parameters[key].shape} does not match gradient shape {layer.gradients[key].shape}"
-
-                    self.optimizer.update(len(self.layers) - 1 - layer_index, layer.parameters, layer.gradients)
-
-                # Check for early stopping
-                if self.patience is not None and self.min_delta is not None:
-                    if loss_value < self.best_loss - self.min_delta:
-                        self.best_loss = loss_value
-                        self.wait = 0
-                    else:
-                        self.wait += 1
-
-                    if self.wait >= self.patience:
-                        progress_bar.close()
-                        print(f"Early stopping on epoch {epoch + 1}")
-                        break
+                    if layer.parameters is not None:
+                        for key in layer.parameters.keys():
+                            assert layer.parameters[key].shape == layer.gradients[
+                                key].shape, f"Parameter shape {layer.parameters[key].shape} does not match gradient shape {layer.gradients[key].shape}"
+                        self.optimizer.update(len(self.layers) - 1 - layer_index, layer.parameters, layer.gradients)
 
             # Calculate the average loss and metrics for the current epoch
             avg_epoch_loss = epoch_loss / batch_count
             avg_epoch_metric_values = [
                 m_value / batch_count for m_value in epoch_metric_values
             ]
 
@@ -210,14 +197,29 @@
                 progress_bar.set_description(
                     f"Epoch {epoch + 1}, Loss: {avg_epoch_loss:.4f}, {metrics_str}, Val Loss: {val_loss_value:.4f}, {val_metrics_str}"
                 )
 
             else:
                 progress_bar.set_description(f"Epoch {epoch + 1}, Loss: {avg_epoch_loss:.4f}, {metrics_str}")
 
+            # Check for early stopping
+            if self.patience is not None and self.min_delta is not None:
+                current_val_loss = self.history["val_loss"][-1] if validation_split is not None else avg_epoch_loss
+
+                if current_val_loss < self.best_loss - self.min_delta:
+                    self.best_loss = current_val_loss
+                    self.wait = 0
+                else:
+                    self.wait += 1
+
+                if self.wait >= self.patience:
+                    progress_bar.close()
+                    print(f"Early stopping on epoch {epoch + 1}")
+                    break
+
     def predict(self, x_test: np.ndarray) -> np.ndarray:
         # Forward pass the input data through the network
         layer_output = x_test
         for layer in self.layers:
             layer_output = layer.forward(layer_output)
         # Return the final output
         return layer_output
```

### Comparing `inventronet-0.0.7a0/inventronet/optimizers/adam.py` & `inventronet-0.0.8a0/inventronet/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet/preprocessing/count_vectorizer.py` & `inventronet-0.0.8a0/inventronet/preprocessing/count_vectorizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from typing import List, Dict, Union
 import re
 from collections import Counter
+from typing import List, Dict, Union, Optional
 
 from scipy.sparse import csr_matrix
 
 
 class CountVectorizer:
-    def __init__(self, lowercase: bool = True, token_pattern: str = r'\b\w+\b'):
+    def __init__(
+            self,
+            lowercase: bool = True,
+            token_pattern: str = r'\b\w+\b',
+            max_features: Optional[int] = None,
+    ):
         self.lowercase: bool = lowercase
         self.token_pattern: str = token_pattern
         self.vocabulary_: Union[Dict[str, int], None] = None
+        self.max_features = max_features
 
     def _preprocess(self, doc: str) -> str:
         if self.lowercase:
             doc = doc.lower()
         return doc
 
     def _tokenize(self, doc: str) -> List[str]:
@@ -22,15 +28,19 @@
     def fit(self, documents: List[str]) -> None:
         word_counts = Counter()
         for doc in documents:
             doc = self._preprocess(doc)
             tokens = self._tokenize(doc)
             word_counts.update(tokens)
 
-        self.vocabulary_ = {word: idx for idx, word in enumerate(word_counts.keys())}
+        if self.max_features is not None:
+            word_counts = word_counts.most_common(self.max_features)
+            self.vocabulary_ = {word: idx for idx, (word, _) in enumerate(word_counts)}
+        else:
+            self.vocabulary_ = {word: idx for idx, word in enumerate(word_counts.keys())}
 
     def transform(self, documents: List[str]) -> csr_matrix:
         if self.vocabulary_ is None:
             raise RuntimeError("You need to call fit() before calling transform().")
 
         indptr = [0]
         indices = []
```

### Comparing `inventronet-0.0.7a0/inventronet/preprocessing/data_split.py` & `inventronet-0.0.8a0/inventronet/preprocessing/data_split.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/inventronet.egg-info/PKG-INFO` & `inventronet-0.0.8a0/inventronet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.7a0
+Version: 0.0.8a0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 Author-email: haitham.hyder@uni.minerva.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inventronet-0.0.7a0/inventronet.egg-info/SOURCES.txt` & `inventronet-0.0.8a0/inventronet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/setup.py` & `inventronet-0.0.8a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 package_name = "inventronet"
-package_version = "0.0.7-alpha"
+package_version = "0.0.8-alpha"
 package_description = "A package for building and testing neural networks"
 
 # Read the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     package_long_description = f.read()
 
 package_url = "https://github.com/inventrohyder/inventronet"
```

### Comparing `inventronet-0.0.7a0/tests/activations/test_leaky_relu.py` & `inventronet-0.0.8a0/tests/activations/test_leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/activations/test_linear.py` & `inventronet-0.0.8a0/tests/activations/test_linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/activations/test_relu.py` & `inventronet-0.0.8a0/tests/activations/test_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/activations/test_sigmoid.py` & `inventronet-0.0.8a0/tests/activations/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/activations/test_softmax.py` & `inventronet-0.0.8a0/tests/activations/test_softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/activations/test_tanh.py` & `inventronet-0.0.8a0/tests/activations/test_tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/layers/conftest.py` & `inventronet-0.0.8a0/tests/layers/conftest.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/layers/test_batch_normalization.py` & `inventronet-0.0.8a0/tests/layers/test_batch_normalization.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/layers/test_dense.py` & `inventronet-0.0.8a0/tests/layers/test_dense.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/layers/test_dropout.py` & `inventronet-0.0.8a0/tests/layers/test_dropout.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/losses/test_binary_cross_entropy.py` & `inventronet-0.0.8a0/tests/losses/test_binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/losses/test_categorical_cross_entropy.py` & `inventronet-0.0.8a0/tests/losses/test_categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/losses/test_mean_absolute_error.py` & `inventronet-0.0.8a0/tests/losses/test_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/losses/test_mean_squared_error.py` & `inventronet-0.0.8a0/tests/losses/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/metrics/test_accuracy.py` & `inventronet-0.0.8a0/tests/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/metrics/test_precision.py` & `inventronet-0.0.8a0/tests/metrics/test_precision.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/models/test_sequential.py` & `inventronet-0.0.8a0/tests/models/test_sequential.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import numpy as np
 import pytest
 from _pytest.fixtures import SubRequest
 
 import inventronet.losses as losses_module
 import inventronet.metrics as metrics_module
 import inventronet.optimizers as optimizers_module
-from inventronet.layers import Dense
+from inventronet.activations import ReLU, Sigmoid
+from inventronet.layers import Dense, Dropout
 from inventronet.losses.loss import Loss
 from inventronet.metrics.metric import Metric
 from inventronet.models import Sequential
+from inventronet.optimizers import StochasticGradientDescent
 from inventronet.optimizers.optimizer import Optimizer
 
 # Get all classes in the metrics module that are subclasses of Metric
 all_metrics = [
     metric
     for _, metric in inspect.getmembers(metrics_module, inspect.isclass)
     if issubclass(metric, Metric) and metric != Metric
@@ -98,14 +100,77 @@
 
 
 @pytest.fixture(scope="module")
 def y(xy: Tuple[np.ndarray, np.ndarray]) -> np.ndarray:
     yield xy[1]
 
 
+@pytest.fixture
+def sequential_model_with_dropout(x: np.ndarray, y: np.ndarray, loss: Loss, optimizer: Optimizer,
+                                  metric: Metric) -> Sequential:
+    # Define the input and output data
+    input_data = x
+    output_data = y
+
+    # Define the neural network with two dense layers and a dropout layer
+    model = Sequential()
+    model.add(Dense(input_dim=3, output_dim=4, activation=ReLU()))
+    model.add(Dropout(0.5, input_dim=4))
+    model.add(Dense(input_dim=4, output_dim=1, activation=Sigmoid()))
+
+    # Compile the model with the loss function, optimizer, and metric
+    model.compile(loss, optimizer, metrics=[metric])
+
+    # Fit the model on the training data
+    model.fit(input_data, output_data, epochs=10)
+
+    return model
+
+
+def test_sequential_model_with_dropout_loss_history_length(sequential_model_with_dropout):
+    # Assert that the training didn't raise any errors and completed successfully
+    assert len(sequential_model_with_dropout.history["loss"]) == 10
+
+
+def test_sequential_model_with_dropout_accuracy_history_length(sequential_model_with_dropout, metric: Metric):
+    # Assert that the training didn't raise any errors and completed successfully
+    assert len(sequential_model_with_dropout.history[metric.__class__.__name__]) == 10
+
+
+# Define a simple model
+def create_model():
+    model = Sequential()
+    model.add(Dense(input_dim=2, output_dim=2, activation=Sigmoid()))
+    model.add(Dense(input_dim=2, output_dim=1, activation=Sigmoid()))
+    return model
+
+
+# Test early stopping
+@pytest.mark.parametrize("patience, min_delta, expected_epochs", [
+    (2, 0.1, 3),
+    (4, 0.05, 5)
+])
+def test_early_stopping(patience, min_delta, expected_epochs, loss: Loss, optimizer: Optimizer, metric: Metric):
+    model = create_model()
+    optimizer = StochasticGradientDescent(learning_rate=0.1)
+
+    model.compile(loss, optimizer, metrics=[metric])
+    model.set_early_stopping(patience=patience, min_delta=min_delta)
+
+    # Define a simple dataset
+    input_data = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
+    output_data = np.array([[0], [1], [1], [0]])
+
+    # Train the model
+    model.fit(input_data, output_data, epochs=1000)
+
+    # Check if the training stopped at the expected epoch
+    assert len(model.history["loss"]) == expected_epochs
+
+
 def test_add(dummy_sequential_model: Sequential):
     """Test the add method of the sequential model."""
     # Try to add a layer with input dimension 4 and output dimension 2
     with pytest.raises(AssertionError):
         dummy_sequential_model.add(Dense(4, 2))
     # Check that the model still has two layers
     assert len(dummy_sequential_model.layers) == 2
```

### Comparing `inventronet-0.0.7a0/tests/optimizers/conftest.py` & `inventronet-0.0.8a0/tests/optimizers/conftest.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/optimizers/test_adam.py` & `inventronet-0.0.8a0/tests/optimizers/test_adam.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/optimizers/test_stochastic_gradient_descent.py` & `inventronet-0.0.8a0/tests/optimizers/test_stochastic_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.7a0/tests/preprocessing/test_count_vectorizer.py` & `inventronet-0.0.8a0/tests/preprocessing/test_count_vectorizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -84,7 +84,37 @@
     vectorizer = CountVectorizer()
     vectorizer.fit_transform(documents)
 
     vectorizer_no_lowercase = CountVectorizer(lowercase=False)
     vectorizer_no_lowercase.fit_transform(documents)
 
     assert len(vectorizer_no_lowercase.vocabulary_) > len(vectorizer.vocabulary_)
+
+
+def test_count_vectorizer_max_features_vocabulary_size(documents):
+    vectorizer = CountVectorizer(max_features=5)
+    vectorizer.fit_transform(documents)
+
+    assert len(vectorizer.vocabulary_) == 5
+
+
+def test_count_vectorizer_max_features_output(documents):
+    vectorizer = CountVectorizer(max_features=5)
+    X = vectorizer.fit_transform(documents)
+
+    assert X.shape == (3, 5)
+
+
+def test_count_vectorizer_max_features_vocabulary_size(documents):
+    max_features = 5
+    vectorizer = CountVectorizer(max_features=max_features)
+    vectorizer.fit_transform(documents)
+
+    assert len(vectorizer.vocabulary_) == max_features
+
+
+def test_count_vectorizer_max_features_output_shape(documents):
+    max_features = 5
+    vectorizer = CountVectorizer(max_features=max_features)
+    X = vectorizer.fit_transform(documents)
+
+    assert X.shape == (3, max_features)
```

### Comparing `inventronet-0.0.7a0/tests/preprocessing/test_train_test_split.py` & `inventronet-0.0.8a0/tests/preprocessing/test_train_test_split.py`

 * *Files identical despite different names*

