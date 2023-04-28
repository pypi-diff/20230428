# Comparing `tmp/inventronet-0.0.5a0.tar.gz` & `tmp/inventronet-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventronet-0.0.5a0.tar", last modified: Thu Apr 27 07:50:12 2023, max compression
+gzip compressed data, was "inventronet-0.0.6a0.tar", last modified: Thu Apr 27 09:18:47 2023, max compression
```

## Comparing `inventronet-0.0.5a0.tar` & `inventronet-0.0.6a0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.839304 inventronet-0.0.5a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-27 07:50:12.839304 inventronet-0.0.5a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.819303 inventronet-0.0.5a0/inventronet/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.823303 inventronet-0.0.5a0/inventronet/activations/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/activations/tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.823303 inventronet-0.0.5a0/inventronet/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/layers/shape_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.823303 inventronet-0.0.5a0/inventronet/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/losses/mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.827303 inventronet-0.0.5a0/inventronet/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/metrics/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.827303 inventronet-0.0.5a0/inventronet/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/models/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.827303 inventronet-0.0.5a0/inventronet/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/optimizers/stochastic_gradient_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.831303 inventronet-0.0.5a0/inventronet/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/preprocessing/count_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/inventronet/preprocessing/data_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.819303 inventronet-0.0.5a0/inventronet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-27 07:50:12.000000 inventronet-0.0.5a0/inventronet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 07:50:12.000000 inventronet-0.0.5a0/inventronet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 07:50:12.000000 inventronet-0.0.5a0/inventronet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 07:50:12.000000 inventronet-0.0.5a0/inventronet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 07:50:12.000000 inventronet-0.0.5a0/inventronet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 07:50:12.839304 inventronet-0.0.5a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.831303 inventronet-0.0.5a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.831303 inventronet-0.0.5a0/tests/activations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/activations/test_tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.835303 inventronet-0.0.5a0/tests/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/layers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/layers/test_batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/layers/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/layers/test_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.835303 inventronet-0.0.5a0/tests/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/losses/test_binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/losses/test_categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/losses/test_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/losses/test_mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.835303 inventronet-0.0.5a0/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/metrics/test_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.835303 inventronet-0.0.5a0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/models/test_sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.839304 inventronet-0.0.5a0/tests/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/optimizers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/optimizers/test_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/optimizers/test_stochastic_gradient_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 07:50:12.839304 inventronet-0.0.5a0/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/preprocessing/test_count_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 07:49:58.000000 inventronet-0.0.5a0/tests/preprocessing/test_train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.797835 inventronet-0.0.6a0/inventronet/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.801835 inventronet-0.0.6a0/inventronet/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/activations/tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.805835 inventronet-0.0.6a0/inventronet/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/layers/shape_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.805835 inventronet-0.0.6a0/inventronet/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/losses/mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.805835 inventronet-0.0.6a0/inventronet/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/metrics/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/inventronet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/models/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/inventronet/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/optimizers/stochastic_gradient_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/inventronet/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/preprocessing/count_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/inventronet/preprocessing/data_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.801835 inventronet-0.0.6a0/inventronet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-27 09:18:47.000000 inventronet-0.0.6a0/inventronet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 09:18:47.000000 inventronet-0.0.6a0/inventronet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:18:47.000000 inventronet-0.0.6a0/inventronet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-27 09:18:47.000000 inventronet-0.0.6a0/inventronet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:18:47.000000 inventronet-0.0.6a0/inventronet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:18:47.817835 inventronet-0.0.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/tests/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/activations/test_tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.809835 inventronet-0.0.6a0/tests/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/layers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/layers/test_batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/layers/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/layers/test_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/losses/test_binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/losses/test_categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/losses/test_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/losses/test_mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/metrics/test_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/models/test_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/tests/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/optimizers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/optimizers/test_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/optimizers/test_stochastic_gradient_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:47.813835 inventronet-0.0.6a0/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/preprocessing/test_count_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-27 09:18:34.000000 inventronet-0.0.6a0/tests/preprocessing/test_train_test_split.py
```

### Comparing `inventronet-0.0.5a0/LICENSE` & `inventronet-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/PKG-INFO` & `inventronet-0.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 Author-email: haitham.hyder@uni.minerva.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inventronet-0.0.5a0/README.md` & `inventronet-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/activation.py` & `inventronet-0.0.6a0/inventronet/activations/activation.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/leaky_relu.py` & `inventronet-0.0.6a0/inventronet/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/linear.py` & `inventronet-0.0.6a0/inventronet/activations/linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/relu.py` & `inventronet-0.0.6a0/inventronet/activations/relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/sigmoid.py` & `inventronet-0.0.6a0/inventronet/activations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/softmax.py` & `inventronet-0.0.6a0/inventronet/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/activations/tanh.py` & `inventronet-0.0.6a0/inventronet/activations/tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/layers/batch_normalization.py` & `inventronet-0.0.6a0/inventronet/layers/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/layers/dense.py` & `inventronet-0.0.6a0/inventronet/layers/dense.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/layers/dropout.py` & `inventronet-0.0.6a0/inventronet/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/layers/layer.py` & `inventronet-0.0.6a0/inventronet/layers/layer.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/losses/binary_cross_entropy.py` & `inventronet-0.0.6a0/inventronet/losses/binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/losses/categorical_cross_entropy.py` & `inventronet-0.0.6a0/inventronet/losses/categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/losses/loss.py` & `inventronet-0.0.6a0/inventronet/losses/loss.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/losses/mean_absolute_error.py` & `inventronet-0.0.6a0/inventronet/losses/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/losses/mean_squared_error.py` & `inventronet-0.0.6a0/inventronet/losses/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/models/model.py` & `inventronet-0.0.6a0/inventronet/models/model.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/models/sequential.py` & `inventronet-0.0.6a0/inventronet/models/sequential.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/optimizers/adam.py` & `inventronet-0.0.6a0/inventronet/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/preprocessing/count_vectorizer.py` & `inventronet-0.0.6a0/inventronet/preprocessing/count_vectorizer.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet/preprocessing/data_split.py` & `inventronet-0.0.6a0/inventronet/preprocessing/data_split.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/inventronet.egg-info/PKG-INFO` & `inventronet-0.0.6a0/inventronet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 Author-email: haitham.hyder@uni.minerva.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inventronet-0.0.5a0/inventronet.egg-info/SOURCES.txt` & `inventronet-0.0.6a0/inventronet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/setup.py` & `inventronet-0.0.6a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 package_name = "inventronet"
-package_version = "0.0.5-alpha"
+package_version = "0.0.6-alpha"
 package_description = "A package for building and testing neural networks"
 
 # Read the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     package_long_description = f.read()
 
 package_url = "https://github.com/inventrohyder/inventronet"
@@ -16,14 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 package_keywords = "neural network, machine learning, artificial intelligence"
 package_install_requires = [
     "numpy",
+    "tqdm",
 ]
 
 package_extras_require = {
     "test": ["pytest", "pytest-cov"],
     "docs": ["sphinx", "sphinx-rtd-theme"],
     "lint": ["flake8", "ruff", "black"],
 }
```

### Comparing `inventronet-0.0.5a0/tests/activations/test_leaky_relu.py` & `inventronet-0.0.6a0/tests/activations/test_leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/activations/test_linear.py` & `inventronet-0.0.6a0/tests/activations/test_linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/activations/test_relu.py` & `inventronet-0.0.6a0/tests/activations/test_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/activations/test_sigmoid.py` & `inventronet-0.0.6a0/tests/activations/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/activations/test_softmax.py` & `inventronet-0.0.6a0/tests/activations/test_softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/activations/test_tanh.py` & `inventronet-0.0.6a0/tests/activations/test_tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/layers/conftest.py` & `inventronet-0.0.6a0/tests/layers/conftest.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/layers/test_batch_normalization.py` & `inventronet-0.0.6a0/tests/layers/test_batch_normalization.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/layers/test_dense.py` & `inventronet-0.0.6a0/tests/layers/test_dense.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/layers/test_dropout.py` & `inventronet-0.0.6a0/tests/layers/test_dropout.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/losses/test_binary_cross_entropy.py` & `inventronet-0.0.6a0/tests/losses/test_binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/losses/test_categorical_cross_entropy.py` & `inventronet-0.0.6a0/tests/losses/test_categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/losses/test_mean_absolute_error.py` & `inventronet-0.0.6a0/tests/losses/test_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/losses/test_mean_squared_error.py` & `inventronet-0.0.6a0/tests/losses/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/metrics/test_accuracy.py` & `inventronet-0.0.6a0/tests/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/metrics/test_precision.py` & `inventronet-0.0.6a0/tests/metrics/test_precision.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/models/test_sequential.py` & `inventronet-0.0.6a0/tests/models/test_sequential.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/optimizers/conftest.py` & `inventronet-0.0.6a0/tests/optimizers/conftest.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/optimizers/test_adam.py` & `inventronet-0.0.6a0/tests/optimizers/test_adam.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/optimizers/test_stochastic_gradient_descent.py` & `inventronet-0.0.6a0/tests/optimizers/test_stochastic_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/preprocessing/test_count_vectorizer.py` & `inventronet-0.0.6a0/tests/preprocessing/test_count_vectorizer.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.5a0/tests/preprocessing/test_train_test_split.py` & `inventronet-0.0.6a0/tests/preprocessing/test_train_test_split.py`

 * *Files identical despite different names*

