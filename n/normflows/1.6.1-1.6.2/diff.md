# Comparing `tmp/normflows-1.6.1.tar.gz` & `tmp/normflows-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/normflows-1.6.1.tar", last modified: Fri Feb 24 11:03:20 2023, max compression
+gzip compressed data, was "dist/normflows-1.6.2.tar", last modified: Fri Apr 28 14:53:22 2023, max compression
```

## Comparing `normflows-1.6.1.tar` & `normflows-1.6.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.6.1/LICENSE
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.6.1/MANIFEST.in
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-02-24 11:03:20.000000 normflows-1.6.1/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13434 2023-02-24 10:54:07.000000 normflows-1.6.1/README.md
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-02-24 09:05:36.000000 normflows-1.6.1/normflows/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15220 2023-01-23 14:38:51.000000 normflows-1.6.1/normflows/core.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7500 2023-01-23 14:38:51.000000 normflows-1.6.1/normflows/core_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/distributions/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      659 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/distributions/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    21576 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4508 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/distributions/decoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/decoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/distribution_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/encoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/encoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/distributions/linear_interpolation.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/distributions/mh_proposal.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.6.1/normflows/distributions/prior.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/prior_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4930 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/distributions/target.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      844 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/distributions/target_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/flows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/flows/__init__.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/flows/affine/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/flows/affine/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/flows/affine/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/affine/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/flows/affine/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/flows/affine/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/affine/glow.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/affine/glow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/flows/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/flow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/mixing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/mixing_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/flows/neural_spline/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/flows/neural_spline/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/wrapper.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/neural_spline/wrapper_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/flows/normalization.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/flows/periodic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/periodic_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/planar.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/planar_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/flows/radial.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/radial_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/flows/reshape.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.6.1/normflows/flows/residual.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.6.1/normflows/flows/residual_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/stochastic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/flows/stochastic_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/nets/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/nets/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/nets/cnn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/nets/lipschitz.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/nets/made.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/nets/made_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/nets/mlp.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/nets/resnet.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/sampling/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/sampling/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/sampling/hais.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/transforms.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.6.1/normflows/transforms_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows/utils/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/utils/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/utils/eval.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/utils/masks.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.6.1/normflows/utils/nn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/utils/optim.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.6.1/normflows/utils/preprocessing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.6.1/normflows/utils/splines.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.6.1/normflows/utils/splines_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/SOURCES.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/dependency_links.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/requires.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-02-24 11:03:20.000000 normflows-1.6.1/normflows.egg-info/top_level.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.6.1/requirements.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-02-24 11:03:20.000000 normflows-1.6.1/setup.cfg
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-02-24 09:04:20.000000 normflows-1.6.1/setup.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.6.2/LICENSE
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.6.2/MANIFEST.in
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-04-28 14:53:22.000000 normflows-1.6.2/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13434 2023-04-28 14:51:39.000000 normflows-1.6.2/README.md
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-04-28 14:51:39.000000 normflows-1.6.2/normflows/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15220 2023-04-28 14:51:17.000000 normflows-1.6.2/normflows/core.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7502 2023-04-28 14:51:17.000000 normflows-1.6.2/normflows/core_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/distributions/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      659 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/distributions/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    21489 2023-02-25 15:05:55.000000 normflows-1.6.2/normflows/distributions/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4508 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/distributions/decoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/decoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/distribution_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/encoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/encoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/linear_interpolation.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/mh_proposal.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.6.2/normflows/distributions/prior.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/prior_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4930 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/distributions/target.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      844 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/distributions/target_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/__init__.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/affine/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/affine/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/affine/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/affine/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/affine/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/glow.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/affine/glow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/flows/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/flow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/mixing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/mixing_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/flows/neural_spline/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/flows/neural_spline/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/wrapper.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/neural_spline/wrapper_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/normalization.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/periodic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/periodic_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/planar.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/planar_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/flows/radial.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/radial_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/flows/reshape.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.6.2/normflows/flows/residual.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.6.2/normflows/flows/residual_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/stochastic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/flows/stochastic_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/nets/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/nets/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/cnn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/lipschitz.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/nets/made.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/made_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/nets/mlp.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/nets/resnet.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/sampling/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/sampling/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/sampling/hais.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/transforms.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.6.2/normflows/transforms_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows/utils/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/utils/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/eval.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/masks.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.6.2/normflows/utils/nn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/optim.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.6.2/normflows/utils/preprocessing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.6.2/normflows/utils/splines.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.6.2/normflows/utils/splines_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14023 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/requires.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-04-28 14:53:22.000000 normflows-1.6.2/normflows.egg-info/top_level.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.6.2/requirements.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-04-28 14:53:22.000000 normflows-1.6.2/setup.cfg
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-04-28 14:51:39.000000 normflows-1.6.2/setup.py
```

### Comparing `normflows-1.6.1/LICENSE` & `normflows-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/PKG-INFO` & `normflows-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normflows
-Version: 1.6.1
+Version: 1.6.2
 Summary: Pytorch implementation of normalizing flows
 Home-page: https://github.com/VincentStimper/normalizing-flows
 Author: Vincent Stimper
 Author-email: vincent.stimper@tuebingen.mpg.de
 License: MIT
 Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.1-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.6.1 Summary: Pytorch
+Metadata-Version: 2.1 Name: normflows Version: 1.6.2 Summary: Pytorch
 implementation of normalizing flows Home-page: https://github.com/
 VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
 vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
 VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
@@ -11,15 +11,15 @@
 workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
 flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
 actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
 raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
 coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
 MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
 img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.1-blue.svg)](https:/
+2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https:/
 /pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
```

### Comparing `normflows-1.6.1/README.md` & `normflows-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.1-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 badge.svg)](https://vincentstimper.github.io/normalizing-flows/) ![unit-tests]
 (https://github.com/VincentStimper/normalizing-flows/actions/workflows/
 pytest.yaml/badge.svg) ![code coverage](https://raw.githubusercontent.com/
 VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true) [!
 [License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://
 opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-
 2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) [![PyPI](https://
-img.shields.io/badge/PyPI-1.6.1-blue.svg)](https://pypi.org/project/normflows/
+img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/
 ) [![Downloads](https://static.pepy.tech/personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
```

### Comparing `normflows-1.6.1/normflows/core.py` & `normflows-1.6.2/normflows/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Returns:
           Batch in the space of the target distribution,
           log determinant of the Jacobian
         """
         log_det = torch.zeros(len(z), device=z.device)
         for flow in self.flows:
             z, log_d = flow(z)
-            log_det -= log_d
+            log_det += log_d
         return z, log_det
 
     def inverse(self, x):
         """Transforms flow variable x to the latent variable z
 
         Args:
           x: Batch in the space of the target distribution
```

### Comparing `normflows-1.6.1/normflows/core_test.py` & `normflows-1.6.2/normflows/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         latent_size = 2
         for n_layers in [2, 5]:
             with self.subTest(n_layers=n_layers):
                 # Construct flow model
                 layers = []
                 for i in range(n_layers):
                     b = torch.Tensor([j if i % 2 == j % 2 else 0 for j in range(latent_size)])
-                    s = MLP([latent_size, 2 * latent_size, latent_size], init_zeros=True)
-                    t = MLP([latent_size, 2 * latent_size, latent_size], init_zeros=True)
+                    s = MLP([latent_size, 2 * latent_size, latent_size], init_zeros=False)
+                    t = MLP([latent_size, 2 * latent_size, latent_size], init_zeros=False)
                     layers.append(MaskedAffineFlow(b, t, s))
                 base = DiagGaussian(latent_size)
                 target = CircularGaussianMixture()
                 model = NormalizingFlow(base, layers, target)
                 # Test log prob and sampling
                 inputs = torch.randn((batch_size, latent_size))
                 log_q = model.log_prob(inputs)
```

### Comparing `normflows-1.6.1/normflows/distributions/__init__.py` & `normflows-1.6.2/normflows/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/base.py` & `normflows-1.6.2/normflows/distributions/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,17 +441,14 @@
         )
         # Apply transform
         if self.class_cond:
             z, log_det = self.transform(z, y)
         else:
             z, log_det = self.transform(z)
         log_p -= log_det
-        print(y)
-        print(eps)
-        print(z)
         return z, log_p
 
     def log_prob(self, z, y=None):
         # Perpare onehot encoding of class if needed
         if self.class_cond:
             if y.dim() == 1:
                 y_onehot = torch.zeros(
@@ -473,16 +470,14 @@
         z = z / np.exp(log_scale)
         log_p = (
             log_p
             - self.d * log_scale
             - 0.5 * self.d * np.log(2 * np.pi)
             - 0.5 * torch.sum(torch.pow(z, 2), dim=self.sum_dim)
         )
-        print(y)
-        print(z)
         return log_p
 
 
 class GaussianMixture(BaseDistribution):
     """
     Mixture of Gaussians with diagonal covariance matrix
     """
```

### Comparing `normflows-1.6.1/normflows/distributions/base_test.py` & `normflows-1.6.2/normflows/distributions/base_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/decoder.py` & `normflows-1.6.2/normflows/distributions/decoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/decoder_test.py` & `normflows-1.6.2/normflows/distributions/decoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/distribution_test.py` & `normflows-1.6.2/normflows/distributions/distribution_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/encoder.py` & `normflows-1.6.2/normflows/distributions/encoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/encoder_test.py` & `normflows-1.6.2/normflows/distributions/encoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/linear_interpolation.py` & `normflows-1.6.2/normflows/distributions/linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/mh_proposal.py` & `normflows-1.6.2/normflows/distributions/mh_proposal.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/prior.py` & `normflows-1.6.2/normflows/distributions/prior.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/prior_test.py` & `normflows-1.6.2/normflows/distributions/prior_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/target.py` & `normflows-1.6.2/normflows/distributions/target.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/distributions/target_test.py` & `normflows-1.6.2/normflows/distributions/target_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/__init__.py` & `normflows-1.6.2/normflows/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/autoregressive.py` & `normflows-1.6.2/normflows/flows/affine/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/autoregressive_test.py` & `normflows-1.6.2/normflows/flows/affine/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/coupling.py` & `normflows-1.6.2/normflows/flows/affine/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/coupling_test.py` & `normflows-1.6.2/normflows/flows/affine/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/glow.py` & `normflows-1.6.2/normflows/flows/affine/glow.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/affine/glow_test.py` & `normflows-1.6.2/normflows/flows/affine/glow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/base.py` & `normflows-1.6.2/normflows/flows/base.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/base_test.py` & `normflows-1.6.2/normflows/flows/base_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/flow_test.py` & `normflows-1.6.2/normflows/flows/flow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/mixing.py` & `normflows-1.6.2/normflows/flows/mixing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/mixing_test.py` & `normflows-1.6.2/normflows/flows/mixing_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/autoregressive.py` & `normflows-1.6.2/normflows/flows/neural_spline/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/autoregressive_test.py` & `normflows-1.6.2/normflows/flows/neural_spline/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/coupling.py` & `normflows-1.6.2/normflows/flows/neural_spline/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/coupling_test.py` & `normflows-1.6.2/normflows/flows/neural_spline/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/wrapper.py` & `normflows-1.6.2/normflows/flows/neural_spline/wrapper.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/neural_spline/wrapper_test.py` & `normflows-1.6.2/normflows/flows/neural_spline/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/normalization.py` & `normflows-1.6.2/normflows/flows/normalization.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/periodic.py` & `normflows-1.6.2/normflows/flows/periodic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/periodic_test.py` & `normflows-1.6.2/normflows/flows/periodic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/planar.py` & `normflows-1.6.2/normflows/flows/planar.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/planar_test.py` & `normflows-1.6.2/normflows/flows/planar_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/radial.py` & `normflows-1.6.2/normflows/flows/radial.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/reshape.py` & `normflows-1.6.2/normflows/flows/reshape.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/residual.py` & `normflows-1.6.2/normflows/flows/residual.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/residual_test.py` & `normflows-1.6.2/normflows/flows/residual_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/stochastic.py` & `normflows-1.6.2/normflows/flows/stochastic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/flows/stochastic_test.py` & `normflows-1.6.2/normflows/flows/stochastic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/cnn.py` & `normflows-1.6.2/normflows/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/lipschitz.py` & `normflows-1.6.2/normflows/nets/lipschitz.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/made.py` & `normflows-1.6.2/normflows/nets/made.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/made_test.py` & `normflows-1.6.2/normflows/nets/made_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/mlp.py` & `normflows-1.6.2/normflows/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/nets/resnet.py` & `normflows-1.6.2/normflows/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/sampling/hais.py` & `normflows-1.6.2/normflows/sampling/hais.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/transforms.py` & `normflows-1.6.2/normflows/transforms.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/transforms_test.py` & `normflows-1.6.2/normflows/transforms_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/eval.py` & `normflows-1.6.2/normflows/utils/eval.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/masks.py` & `normflows-1.6.2/normflows/utils/masks.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/nn.py` & `normflows-1.6.2/normflows/utils/nn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/optim.py` & `normflows-1.6.2/normflows/utils/optim.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/preprocessing.py` & `normflows-1.6.2/normflows/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/splines.py` & `normflows-1.6.2/normflows/utils/splines.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows/utils/splines_test.py` & `normflows-1.6.2/normflows/utils/splines_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/normflows.egg-info/PKG-INFO` & `normflows-1.6.2/normflows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normflows
-Version: 1.6.1
+Version: 1.6.2
 Summary: Pytorch implementation of normalizing flows
 Home-page: https://github.com/VincentStimper/normalizing-flows
 Author: Vincent Stimper
 Author-email: vincent.stimper@tuebingen.mpg.de
 License: MIT
 Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
 Platform: UNKNOWN
@@ -18,15 +18,15 @@
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
 [![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.6.1-blue.svg)](https://pypi.org/project/normflows/)
+[![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
 is available as well. A more detailed description of this package is given in out accompanying
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.6.1 Summary: Pytorch
+Metadata-Version: 2.1 Name: normflows Version: 1.6.2 Summary: Pytorch
 implementation of normalizing flows Home-page: https://github.com/
 VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
 vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
 VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
@@ -11,15 +11,15 @@
 workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
 flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
 actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
 raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
 coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
 MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
 img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.1-blue.svg)](https:/
+2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.6.2-blue.svg)](https:/
 /pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
 personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
```

### Comparing `normflows-1.6.1/normflows.egg-info/SOURCES.txt` & `normflows-1.6.2/normflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `normflows-1.6.1/setup.py` & `normflows-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

