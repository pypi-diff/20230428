# Comparing `tmp/cnn2snn-2.3.4.tar.gz` & `tmp/cnn2snn-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnn2snn-2.3.4.tar", last modified: Mon Apr 17 08:48:50 2023, max compression
+gzip compressed data, was "dist/cnn2snn-2.3.5.tar", last modified: Fri Apr 28 06:59:14 2023, max compression
```

## Comparing `cnn2snn-2.3.4.tar` & `cnn2snn-2.3.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16847 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    14077 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      882 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     7844 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     7803 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     6342 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     6680 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     5549 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3083 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     9310 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)    11223 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1760 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2023-04-17 08:48:41.000000 cnn2snn-2.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16847 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10739 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    12382 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    14077 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    26028 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)      882 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     8996 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13938 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     6573 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     8073 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     6342 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2023-04-28 06:59:11.000000 cnn2snn-2.3.5/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 06:59:14.000000 cnn2snn-2.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-04-28 06:59:06.000000 cnn2snn-2.3.5/setup.py
```

### Comparing `cnn2snn-2.3.4/LICENSE` & `cnn2snn-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/PKG-INFO` & `cnn2snn-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.4
+Version: 2.3.5
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.4/cnn2snn/__init__.py` & `cnn2snn-2.3.5/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/akida_versions.py` & `cnn2snn-2.3.5/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/calibration/__init__.py` & `cnn2snn-2.3.5/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/calibration/adaround.py` & `cnn2snn-2.3.5/cnn2snn/calibration/adaround.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.3.5/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/calibration/calibration.py` & `cnn2snn-2.3.5/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/cli.py` & `cnn2snn-2.3.5/cnn2snn/cli.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.3.5/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/compatibility_checks.py` & `cnn2snn-2.3.5/cnn2snn/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/converter.py` & `cnn2snn-2.3.5/cnn2snn/converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/min_value_constraint.py` & `cnn2snn-2.3.5/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/model_generator.py` & `cnn2snn-2.3.5/cnn2snn/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantization.py` & `cnn2snn-2.3.5/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantization_layers.py` & `cnn2snn-2.3.5/cnn2snn/quantization_layers.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantization_ops.py` & `cnn2snn-2.3.5/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/__init__.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/activations.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,14 @@
 
     if not out_quantizer:
         if get_akida_version() == AkidaVersion.v1:
             raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer is mandatory.")
         return {'activation': True}
 
     assert isinstance(out_quantizer, OutputQuantizer)
-    if out_quantizer.signed:
-        raise ValueError(f"{lname}: output_quantizer should not be signed")
     bitwidth = out_quantizer.bitwidth
     if get_akida_version() == AkidaVersion.v2:
         bitwidth_param = 'output_bits'
     else:
         bitwidth_param = 'act_bits'
         if out_quantizer._axis == "per-axis":
             raise ValueError(f"{lname}: in AkidaVersion.v1, output_quantizer must be per-tensor.")
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/add.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/attention.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/batchnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,28 +118,53 @@
         prev_layers = _get_inbound_layers(target_layer)
         if len(prev_layers) > 1:
             return True
         if isinstance(target_layer, QuantizedExtractToken):
             return True
         return False
 
-    def _search_block(target_layer):
+    def _search_block_v1(target_layer):
+        # We consider the target is part of one block if there are previous
+        # layers. (Akida v1 doesn't support multi inbound layers)
+        prev_layers = _get_inbound_layers(target_layer)
+        # If it's the first layer return it
+        if len(prev_layers) == 0:
+            return [target_layer]
+
+        # If previous layer has an output quantizer, the blocks end here.
+        next_target = prev_layers[0]
+        out_quantizer = getattr(next_target, "out_quantizer", None)
+        if out_quantizer:
+            if not isinstance(next_target, QuantizedReLU):
+                raise RuntimeError("Model incompatible with akida v1 version. The layer"
+                                   f" {next_target.name} followed by {target_layer.name}"
+                                   " is not valid.")
+            return [target_layer]
+
+        # Otherwise, we continue searching...
+        return _search_block_v1(next_target) + [target_layer]
+
+    def _search_block_v2(target_layer):
         # We consider the target is part of one block if there are previous
         # layers (target is not the model's input), or it's multi-inbound.
         prev_layers = _get_inbound_layers(target_layer)
         if len(prev_layers) != 1:
             return [target_layer]
         # If previous layer has an output quantizer, the blocks end here.
         next_target = prev_layers[0]
         out_quantizer = getattr(next_target, "out_quantizer", None)
         if out_quantizer or _check_single_layer_block(next_target):
             return [target_layer]
 
         # Otherwise, we continue searching...
-        return _search_block(next_target) + [target_layer]
+        return _search_block_v2(next_target) + [target_layer]
+
+    def _search_block(layer):
+        return _search_block_v1(layer) if get_akida_version() == AkidaVersion.v1 \
+            else _search_block_v2(layer)
 
     def _get_layers_before_dequantizer(model):
         # Return layers before the first dequantizer
         layers = []
         last_deq_layer = None
         for layer in model.layers:
             if isinstance(layer, Dequantizer):
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/compatibility_checks.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/compatibility_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # ******************************************************************************
 """Functions to check model compatibility for CNN2SNN conversion.
 """
 from keras import layers
 from quantizeml import layers as qlayers
 
 from .blocks import split_model_into_blocks
+from .padding import check_same_valid_compatibility
 from ..transforms.sequential import _check_layers_data_format, _check_layer_inbounds
 from ..compatibility_checks import _check_reshape_layer
 from ..akida_versions import get_akida_version, AkidaVersion
 
 neural_layers = (qlayers.QuantizedConv2D, qlayers.QuantizedSeparableConv2D,
                  qlayers.QuantizedDense, qlayers.QuantizedDepthwiseConv2D,
                  qlayers.QuantizedConv2DTranspose, qlayers.QuantizedDepthwiseConv2DTranspose)
@@ -96,38 +97,41 @@
 
     It ONLY checks if the model design is compatible with Akida.
 
     Args:
         model (:obj:`tf.keras.Model`): the model to check.
 
     Returns:
-        list: a list of sequences of layers ('blocks').
+        list: a list of sequences of the non_skippable layers ('blocks').
     """
     # Check general rules about model in three steps:
     # 1. Check if model has only one input and one output,
     # 2. Check right data format and
     # 3. Over Akida 1.0, check if model is sequential.
     _check_model_input_output(model)
     _check_layers_data_format(model)
     if get_akida_version() == AkidaVersion.v1:
         _check_layer_inbounds(model)
 
     # Split model into theirs blocks:
     blocks = split_model_into_blocks(model)
 
+    non_skippable_layers = []
     # Evaluate block-by-block integrity
     for block in blocks:
         # Check reshape/flatten layers
         skippable, block = _extract_skippable_layers(block)
         _check_skippable_compatibility(skippable)
         # Check pooling layers
         _check_pooling_compatibility(block)
         # Check other rules
         _check_block_integrity(block)
-    return blocks
+        if len(block) > 0:
+            non_skippable_layers.append(block)
+    return non_skippable_layers
 
 
 def _split_block_into_layer_types(block):
     """Split input block into the following categories:
 
     - neural (processing) layers,
     - activation layers,
@@ -307,18 +311,14 @@
         elif not isinstance(layer, skippable_layers):
             raise RuntimeError(f"Incompatible {layer.name} skippable layer.")
 
 
 def _check_pooling_compatibility(block):
     """Asserts pooling layer is compatible for conversion.
 
-    Two checks are performed here:
-    - a pooling layer must have a Conv2D type as processing layer and
-    - the padding of MaxPool2D must be the same as the padding of neural layer
-
     Args:
         block (list): the layers block.
     """
     errors = CompatibilityBlockError()
     conv_neural_layers = (qlayers.QuantizedConv2D,
                           qlayers.QuantizedSeparableConv2D, qlayers.QuantizedDepthwiseConv2D)
     pool_layer = [ly for ly in block if isinstance(ly, pooling_layers)]
@@ -339,12 +339,12 @@
                     pool_layer)
     # Raise the exceptions(if exist)
     errors()
 
     # Raises error if the padding of MaxPool2D is different from the padding
     # of the neural processing layer.
     conv_layer = conv_layer[0]
-    neur_pad = conv_layer.padding
+    neur_pad = conv_layer.padding if not check_same_valid_compatibility(conv_layer) else "same"
     pool_pad = getattr(pool_layer, "padding", "")
     if isinstance(pool_layer, qlayers.QuantizedMaxPool2D) and neur_pad != pool_pad:
         raise RuntimeError(f"Pooling layer {pool_layer.name} (padding: {pool_pad}) must have "
                            f"the same padding as {conv_layer.name} (padding: {neur_pad}).")
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/concatenate.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/conv2d_transpose.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/convolution.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/convolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,19 @@
             layer_ak.variables["threshold"] = -bias
         else:
             # Unshift the bias and store it
             layer_ak.variables["bias"] = (bias >> bias_shift).astype(np.int8)
             # Also store the bias shift
             broadcast_and_set_variable(layer_ak.variables, "bias_shift", bias_shift)
 
+            input_shift = getattr(layer_k, 'input_shift', None)
+            if input_shift is not None:
+                broadcast_and_set_variable(layer_ak.variables, "input_shift",
+                                           input_shift.value.numpy().astype(np.uint8))
+
 
 def _parse_convolutional(layer):
     """Parses a quantizeml.QuantizedConv2D parameters.
 
     Args:
         layer (:obj:`tf.keras.Layer`): the layer to parse.
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/dense.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/dense.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/depthwise_conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/extract_token.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/layer_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     Returns:
         :list: the inbounds layers names.
     """
 
     # The list of supported Keras layers not represented in Akida
     skippable_layers = (qlayers.QuantizedDropout, qlayers.QuantizedFlatten,
                         qlayers.QuantizedReshape, qlayers.QuantizedRescaling,
-                        qlayers.QuantizedReLU,
+                        qlayers.QuantizedReLU, qlayers.QuantizedMaxPool2D,
+                        qlayers.QuantizedGlobalAveragePooling2D,
                         qlayers.QuantizedAddPositionEmbs,
                         qlayers.QuantizedClassToken)
 
     # Get inbound layers names
     in_node = k_layer.inbound_nodes[0]
     inbound_layers = in_node.inbound_layers
     if not isinstance(inbound_layers, list):
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/madnorm.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/madnorm.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/outputs.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/outputs.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/padding.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,8 +40,27 @@
     padding_ak_value = 0
     if getattr(k_layer, "padding_value", None):
         padding_quantize = k_layer.padding_value_quantizer
         assert isinstance(padding_quantize, quantizeml.layers.AlignedWeightQuantizer)
         padding_value = padding_quantize.qweights.value.values.numpy().astype(np.int32)
         padding_shift = padding_quantize.shift.value.numpy().astype(np.uint8)
         padding_ak_value = padding_value >> padding_shift
-    return _get_padding(k_layer.padding), padding_ak_value
+
+    padding = k_layer.padding
+    # If a padding_value value is provided or layer produces same output with 'same' or 'valid',
+    # force the padding to be "same" in Akida.
+    if padding_ak_value != 0 or check_same_valid_compatibility(k_layer):
+        padding = "same"
+    return _get_padding(padding), padding_ak_value
+
+
+def check_same_valid_compatibility(layer):
+    """Check if a layer produces the same output regardless of its padding ('same' or 'valid').
+
+    Args:
+        layer (tf.keras.layers.Layer): Layer to verify
+
+    Returns:
+        bool: same/valid compatibility result.
+    """
+    # Layer produces same output when kernel size == 1
+    return layer.kernel_size == (1, 1)
```

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/pooling.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/separable_convolution.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/separable_convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/shiftmax.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/shiftmax.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.3.5/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/__init__.py` & `cnn2snn-2.3.5/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.3.5/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/clone.py` & `cnn2snn-2.3.5/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/equalization.py` & `cnn2snn-2.3.5/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/reshape.py` & `cnn2snn-2.3.5/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/transforms/sequential.py` & `cnn2snn-2.3.5/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/utils.py` & `cnn2snn-2.3.5/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn/weights_ops.py` & `cnn2snn-2.3.5/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.3.5/cnn2snn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.4
+Version: 2.3.5
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.4/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.3.5/cnn2snn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.4/setup.py` & `cnn2snn-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.3.4',
+    version='2.3.5',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alvaro Moran',
     author_email='amoran@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
     install_requires=[get_tf_dep(), 'keras~=2.10.0',
-        'akida==2.3.4', 'quantizeml~=0.4.1'],
+        'akida==2.3.5', 'quantizeml~=0.4.1'],
 )
```

