# Comparing `tmp/mtrf-1.1.0.tar.gz` & `tmp/mtrf-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtrf-1.1.0.tar", last modified: Mon Jan 30 15:39:41 2023, max compression
+gzip compressed data, was "mtrf-1.2.0.tar", last modified: Fri Apr 28 15:34:26 2023, max compression
```

## Comparing `mtrf-1.1.0.tar` & `mtrf-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-01-30 15:39:41.066919 mtrf-1.1.0/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1515 2022-06-22 19:45:32.000000 mtrf-1.1.0/LICENSE
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     7210 2023-01-30 15:39:41.066919 mtrf-1.1.0/PKG-INFO
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     6730 2023-01-30 15:38:51.000000 mtrf-1.1.0/README.md
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-01-30 15:39:41.062919 mtrf-1.1.0/mtrf/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       59 2023-01-30 15:38:47.000000 mtrf-1.1.0/mtrf/__init__.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     3923 2023-01-30 02:01:32.000000 mtrf-1.1.0/mtrf/crossval.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     5355 2023-01-27 20:24:46.000000 mtrf-1.1.0/mtrf/matrices.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    21710 2023-01-30 14:56:49.000000 mtrf-1.1.0/mtrf/model.py
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-01-30 15:39:41.066919 mtrf-1.1.0/mtrf.egg-info/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     7210 2023-01-30 15:39:41.000000 mtrf-1.1.0/mtrf.egg-info/PKG-INFO
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)      257 2023-01-30 15:39:41.000000 mtrf-1.1.0/mtrf.egg-info/SOURCES.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-01-30 15:39:41.000000 mtrf-1.1.0/mtrf.egg-info/dependency_links.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2022-06-22 21:03:32.000000 mtrf-1.1.0/mtrf.egg-info/not-zip-safe
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       46 2023-01-30 15:39:41.000000 mtrf-1.1.0/mtrf.egg-info/requires.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        5 2023-01-30 15:39:41.000000 mtrf-1.1.0/mtrf.egg-info/top_level.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       38 2023-01-30 15:39:41.066919 mtrf-1.1.0/setup.cfg
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1017 2022-07-28 14:56:16.000000 mtrf-1.1.0/setup.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1515 2023-03-03 16:11:35.000000 mtrf-1.2.0/LICENSE
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 15:34:26.970278 mtrf-1.2.0/PKG-INFO
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1632 2023-03-21 15:29:42.000000 mtrf-1.2.0/README.md
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.966278 mtrf-1.2.0/mtrf/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       59 2023-04-28 15:33:31.000000 mtrf-1.2.0/mtrf/__init__.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     9184 2023-04-25 15:15:02.000000 mtrf-1.2.0/mtrf/matrices.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    31493 2023-04-27 16:29:57.000000 mtrf-1.2.0/mtrf/model.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    10115 2023-04-27 17:12:48.000000 mtrf-1.2.0/mtrf/stats.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/mtrf.egg-info/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/PKG-INFO
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)      345 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/SOURCES.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/dependency_links.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 15:26:52.000000 mtrf-1.2.0/mtrf.egg-info/not-zip-safe
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       46 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/requires.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        5 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/top_level.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       38 2023-04-28 15:34:26.970278 mtrf-1.2.0/setup.cfg
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1017 2023-03-16 20:54:02.000000 mtrf-1.2.0/setup.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/tests/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2824 2023-04-25 14:52:40.000000 mtrf-1.2.0/tests/test_basics.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     3395 2023-04-25 16:38:00.000000 mtrf-1.2.0/tests/test_matlab_examples.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2537 2023-04-25 16:44:01.000000 mtrf-1.2.0/tests/test_model.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1417 2023-04-25 16:48:57.000000 mtrf-1.2.0/tests/test_stats.py
```

### Comparing `mtrf-1.1.0/LICENSE` & `mtrf-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mtrf-1.1.0/mtrf/model.py` & `mtrf-1.2.0/mtrf/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,66 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jul 16 14:42:40 2020
-
-@author: Jin Dou
-"""
 from pathlib import Path
 from itertools import product
 import pickle
 import requests
 from collections.abc import Iterable
 import numpy as np
-from matplotlib import pyplot as plt
-from mtrf.crossval import cross_validate, _progressbar
+from mtrf.stats import cross_validate, _cross_validate, _progressbar, _check_k
 from mtrf.matrices import (
     covariance_matrices,
-    banded_regularization_coefficients,
+    banded_regularization,
     regularization_matrix,
     lag_matrix,
     truncate,
     _check_data,
+    _get_xy,
 )
 
+try:
+    from matplotlib import pyplot as plt
+except ModuleNotFoundError:
+    plt = None
+try:
+    import mne
+except ModuleNotFoundError:
+    mne = None
+
 
 class TRF:
     """
-    Class for the (multivariate) temporal response function.
-    Can be used as a forward encoding model (stimulus to neural response)
-    or backward decoding model (neural response to stimulus) using time lagged
-    input features as per Crosse et al. (2016).
-    Arguments:
-        direction (int): Direction of the model. Can be 1 to fit a forward
-            model (default) or -1 to fit a backward model.
-        kind (str): Kind of model to fit. Can be 'multi' (default) to fit
-            a multi-lag model using all time lags simulatneously or
-            'single' to fit separate sigle-lag models for each individual lag.
-        zeropad (bool): If True (defaul), pad the outer rows of the design
-            matrix with zeros. If False, delete them.
-        method (str): Regularization method. Can be 'ridge' (default) or
-            'tikhonov' or 'banded'.
-    Attributes:
-       weights (np.ndarray): Model weights which are estimated by fitting the
-           model to the data using the train() method. The weight matrix should
-           have the shape stimulus features x time lags x response features.
-        bias (np.ndarray): Vector containing the bias term for every
-            response feature.
-        times (list): Model time lags, estimated based on the training time
-            window and sampling rate.
+    Temporal response function.
+
+    A (multivariate) regression using time lagged input features which can be used as
+    an encoding model to predict brain responses from stimulus features or as a decoding
+    model to predict stimulus features from brain responses.
+
+    Parameters
+    ----------
+    direction: int
+        If 1, make a forward model using the stimulus as predictor to estimate the
+        response (default). If -1, make a decoding model using the response to estimate
+        the stimulus.
+    kind: str
+        If 'multi' (default), fit a multi-lag model using all time lags simultaneously.
+        If 'single', fit separate single-lag models for each individual lag.
+    zeropad: bool
+        If True (defaul), pad the outer rows of the design matrix with zeros.
+        If False, delete them.
+    method: str
+        Regularization method. Can be 'ridge' (default), 'tikhonov' or 'banded'.
+        See documentation for a detailed explanation.
+
+    Attributes
+    ----------
+    weights: numpy.ndarray
+        Beta coefficients in a three-dimensional inputs-by-lags-by-outputs matrix
+    bias: numpy.ndarray
+        One dimensional array with one bias term per input feature
+    times: list
+        Time lags, depending on training time window and sampling rate.
     """
 
     def __init__(
         self, direction=1, kind="multi", zeropad=True, bias=True, method="ridge"
     ):
         self.weights = None
         self.bias = bias
@@ -91,293 +102,473 @@
 
     def __truediv__(self, num):
         trf_new = self.copy()
         trf_new.weights /= num
         trf_new.bias /= num
         return trf_new
 
-    def fit(
+    def train(
         self,
         stimulus,
         response,
         fs,
         tmin,
         tmax,
         regularization,
+        test=False,
         bands=None,
-        k=5,
+        k=-1,
+        average=True,
         seed=None,
         verbose=True,
     ):
         """
-        Fit TRF model. If a regularization is just a single scalar, this method
-        will simply call `TRF.train`, when given a list of regularization values,
-        this method will find the best value (i.e. the one that yields the
-        highest prediction accuracy) and train a TRF with the selected regularization value.
-        Arguments:
-            stimulus (list): List where each element is a 2-D samples-by-features array,
-                corresponding to one trial. The second dimension can be omitted if
-                there only is a single stimulus feature (e.g. envelope).
-            response (list): List where each element is a 2-D samples-by-channels array,
-                corresponding to one trial.
-            fs (int): Sample rate of stimulus and response in hertz.
-            tmin (float): Minimum time lag in seconds
-            tmax (float): Maximum time lag in seconds
-            regularization (list, float, int): The regularization paramter
-                (lambda). If a list with multiple values is supplied, the
-                model is fitted separately for each value. The model with the
-                highest accuracy (correlation of prediction and actual output)
-                is selected and the correlation and error for every tested
-                regularization value are returned.
-            bands (list | None): Must only be provided when using banded ridge regression.
-                Size of the features for which a regularization parameter is fitted, in the order
-                they appear in the stimulus matrix. For example, when the stimulus consists of an
-                envelope vector and a 16-band spectrogram, features would be [1, 16].
-                List with indices marking the borders between bands.
-            k (int): Number of data splits for cross validation.
-                     If -1, do leave-one-out cross-validation.
-            seed (int): Seed for the random number generator.
-        Returns:
-            correlation (list): Correlation of prediction and actual output
-                per value when using multiple regularization values.
-            error (list): Error between prediction and output per value
-                when using multiple regularization values.
-        """
-        if not (isinstance(stimulus, list) and isinstance(response, list)):
-            raise ValueError(
-                "Model fitting requires a list of multiple trials for stimulus and response!"
-            )
-        else:
-            stimulus, response = _check_data(stimulus), _check_data(response)
+        Optimize the regularization parameter and optionally test model performance.
 
+        For each value in `regularization`, a model is trained and validated using
+        k-fold cross validation. Then the best regularization value (i.e. the one
+        that results is the lowest mean squared error between the predicted and
+        actual output) is chosen to train the final model.
+
+        Compute a linear mapping between stimulus and response, or vice versa, using
+        regularized regression. This method can compare multiple values for the
+        regularization parameter and select the best one (i.e. the one that yields
+        the highest prediction accuracy).
+
+        Parameters
+        ----------
+        stimulus: list
+            Each element must contain one trial's stimulus in a two-dimensional
+            samples-by-features array (second dimension can be omitted if there is
+            only a single feature.
+        response: list
+            Each element must contain one trial's response in a two-dimensional
+            samples-by-channels array.
+        fs: int
+            Sample rate of stimulus and response in hertz.
+        tmin: float
+            Minimum time lag in seconds.
+        tmax: float
+            Maximum time lag in seconds.
+        regularization: list or float or int
+            Values for the regularization parameter lambda. The model is fitted
+            separately for each value and the one yielding the highest accuracy
+            is chosen (correlation and mean squared error of each model are returned).
+        bands: list or None
+            Must only be provided when using banded ridge regression. Size of the
+            features for which a regularization parameter is fitted, in the order they
+            appear in the stimulus matrix. For example, when the stimulus consists of
+            an envelope vector and a 16-band spectrogram, bands would be [1, 16].
+        k: int
+            Number of data splits for cross validation, defaults to 5.
+            If -1, do leave-one-out cross-validation.
+        average: bool or list or numpy.ndarray
+            If True (default), average correlation and mean squared error across all
+            predictions (e.g. channels in the case of forward modelling). If `average`
+            is an array of integers only average the predicted features at those indices.
+        seed: int
+            Seed for the random number generator.
+        verbose: bool
+            If True (default), show a progress bar during fitting
+
+        Returns
+        -------
+        r : list
+            Correlation of prediction and actual output.
+        mse : list
+            Mean squared error between prediction and actual output.
+        """
+        if average is False:
+            raise ValueError("Average must be True or a list of indices!")
+        if np.isscalar(regularization):
+            min_len = 1
+        else:  # optimizing lambda requires multiple trials
+            min_len = 2
+        stimulus, response, n_trials = _check_data(stimulus, response, min_len=min_len)
+        if not np.isscalar(regularization):
+            k = _check_k(k, n_trials)
+        xs, ys, tmin, tmax = _get_xy(stimulus, response, tmin, tmax, self.direction)
+        lags = list(range(int(np.floor(tmin * fs)), int(np.ceil(tmax * fs)) + 1))
         if self.method == "banded":
-            if bands is None:
-                raise ValueError(
-                    "Must provide band sizes when using banded ridge regression!"
-                )
-            if not sum(bands) == stimulus[0].shape[-1]:
-                raise ValueError(
-                    "Sum of the bands must match the total number of stimulus features!"
-                )
-            n_lags = int(np.ceil(tmax * fs) - np.floor(tmin * fs) + 1)
             coefficients = list(product(regularization, repeat=2))
             regularization = [
-                banded_regularization_coefficients(n_lags, c, bands, self.bias)
+                banded_regularization(len(lags), c, bands, self.bias)
                 for c in coefficients
             ]
         if np.isscalar(regularization):
-            self.train(stimulus, response, fs, tmin, tmax, regularization)
+            self._train(xs, ys, fs, tmin, tmax, regularization)
+            return
         else:  # run cross-validation once per regularization parameter
-            correlation = np.zeros(len(regularization))
-            error = np.zeros(len(regularization))
+            # pre-compute covariance matrices
+            cov_xx, cov_xy = covariance_matrices(xs, ys, lags, self.zeropad, self.bias)
+            r = np.zeros(len(regularization))
+            mse = np.zeros(len(regularization))
             for ir in _progressbar(
-                range(len(regularization)), "Hyperparameter optimization"
+                range(len(regularization)),
+                "Hyperparameter optimization",
+                verbose=verbose,
             ):
-                r = regularization[ir]
-                reg_correlation, reg_error = cross_validate(
-                    self.copy(), stimulus, response, fs, tmin, tmax, r, k, seed=seed
+                r[ir], mse[ir] = _cross_validate(
+                    self.copy(),
+                    xs,
+                    ys,
+                    cov_xx,
+                    cov_xy,
+                    lags,
+                    fs,
+                    regularization[ir],
+                    k,
+                    seed=seed,
+                    average=average,
+                    verbose=verbose,
                 )
-                correlation[ir] = reg_correlation
-                error[ir] = reg_error
-            regularization = list(regularization)[np.argmax(correlation)]
-            self.train(stimulus, response, fs, tmin, tmax, regularization)
-            return correlation, error
+            best_regularization = list(regularization)[np.argmin(mse)]
+            self._train(stimulus, response, fs, tmin, tmax, best_regularization)
+            return r, mse
 
-    def train(self, stimulus, response, fs, tmin, tmax, regularization):
-        """
-        Compute the TRF weights that minimze the mean squared error between the
-        actual and predicted neural response.
-        Arguments:
-            stimulus (list | np.ndarray): Either a 2-D samples-by-features array, if
-                the data contains only one trial or a list of such arrays of it
-                contains multiple trials. The second dimension can be omitted if
-                there only is a single stimulus feature (e.g. envelope).
-            response (list | np.ndarray): Either a 2-D samples-by-channels array, if
-                the data contains only one trial or a list of such arrays of it
-                contains multiple trials.
-            fs (int): Sample rate of stimulus and response in hertz.
-            tmin (float): Minimum time lag in seconds
-            tmax (float): Maximum time lag in seconds
-            regularization (float, int): The regularization paramter (lambda).
-        """
+    def _train(self, xs, ys, fs, tmin, tmax, regularization):
         if isinstance(self.bias, np.ndarray):  # reset bias if trf is already trained
             self.bias = True
-        stimulus, response = _check_data(stimulus), _check_data(response)
-        if not len(stimulus) == len(response):
-            ValueError("Respone and stimulus must have the same length!")
-        else:
-            ntrials = len(stimulus)
         if isinstance(regularization, np.ndarray):  # check if matrix is diagonal
             if (
                 np.count_nonzero(regularization - np.diag(np.diagonal(regularization)))
                 > 0
             ):
                 raise ValueError(
                     "Regularization parameter must be a single number or a diagonal matrix!"
                 )
-        delta = 1 / fs
-        self.fs = fs
-        self.regularization = regularization
+        self.fs, self.regularization = fs, regularization
         cov_xx = 0
         cov_xy = 0
-        if self.direction == 1:
-            xs, ys = stimulus, response
-        if self.direction == -1:
-            xs, ys = response, stimulus
-            tmin, tmax = -1 * tmax, -1 * tmin
+        lags = list(range(int(np.floor(tmin * fs)), int(np.ceil(tmax * fs)) + 1))
         for x, y in zip(xs, ys):
             assert x.ndim == 2 and y.ndim == 2
-            lags = list(range(int(np.floor(tmin * fs)), int(np.ceil(tmax * fs)) + 1))
             # sum covariances matrices across observations
             cov_xx_trial, cov_xy_trial = covariance_matrices(
                 x, y, lags, self.zeropad, self.bias
             )
             cov_xx += cov_xx_trial
             cov_xy += cov_xy_trial
-        cov_xx, cov_xy = cov_xx / ntrials, cov_xy / ntrials  # normalize
+        cov_xx, cov_xy = cov_xx / len(xs), cov_xy / len(ys)  # normalize
         regmat = regularization_matrix(cov_xx.shape[1], self.method)
-        regmat *= regularization / delta
-        # calculate reverse correlation:
-        weight_matrix = np.matmul(np.linalg.inv(cov_xx + regmat), cov_xy) / delta
+        regmat *= regularization / (1 / self.fs)
+        weight_matrix = np.matmul(np.linalg.inv(cov_xx + regmat), cov_xy) / (
+            1 / self.fs
+        )
         self.bias = weight_matrix[0:1]
+        if self.bias.ndim == 1:  # add empty dimension for single feature models
+            self.bias = np.expand_dims(self.bias, axis=0)
         self.weights = weight_matrix[1:].reshape(
             (x.shape[1], len(lags), y.shape[1]), order="F"
         )
         self.times = np.array(lags) / fs
         self.fs = fs
 
+    def test(
+        self,
+        stimulus,
+        response,
+        fs,
+        tmin,
+        tmax,
+        regularization,
+        bands=None,
+        k=-1,
+        average=True,
+        seed=None,
+        verbose=True,
+    ):
+        """
+        Unbiased estimate of model accuracy when fitting the regularization parameter.
+
+        This fuction divides the data into k parts and runs two nested
+        cross-validation loops: the outer loop selects k-1 parts to optimize the
+        regularization value and the kth part to test the final model's accuracy.
+        The inner loop uses cross-validation to determine the best regularization
+        value as in the `fit` method. The data are rotated so that each of the
+        k segments is used to test the final model's accuracy once. The average
+        correlation and mean squared error across all folds is an unbiased estimate
+        of the model's accuracy because the test data was not part of the optimization
+        process.
+
+        Parameters
+        ----------
+        stimulus: list
+            Each element must contain one trial's stimulus in a two-dimensional
+            samples-by-features array (second dimension can be omitted if there is
+            only a single feature.
+        response: list
+            Each element must contain one trial's response in a two-dimensional
+            samples-by-channels array.
+        fs: int
+            Sample rate of stimulus and response in hertz.
+        tmin: float
+            Minimum time lag in seconds.
+        tmax: float
+            Maximum time lag in seconds.
+        regularization: list or float or int
+            Values for the regularization parameter lambda. The model is fitted
+            separately for each value and the one yielding the highest accuracy
+            is chosen (correlation and mean squared error of each model are returned).
+        bands: list or None
+            Must only be provided when using banded ridge regression. Size of the
+            features for which a regularization parameter is fitted, in the order they
+            appear in the stimulus matrix. For example, when the stimulus consists of
+            an envelope vector and a 16-band spectrogram, bands would be [1, 16].
+        k: int
+            Number of data splits for cross validation, defaults to 5.
+            If -1, do leave-one-out cross-validation.
+        average: bool or list or numpy.ndarray
+            If True (default), average correlation and mean squared error across all
+            predictions (e.g. channels in the case of forward modelling). If `average`
+            is an array of integers only average the predicted features at those indices.
+        seed: int
+            Seed for the random number generator.
+        verbose: bool
+            If True (default), show a progress bar during fitting
+
+        Returns
+        -------
+        r_test: numpy.ndarray
+            Correlation between actual and predicted output for k test sets
+        mse_test: numpy.ndarray
+            Mean squared error between actual and predicted output for k test sets
+        best_regularization: numpy.ndarray
+            Optimal regularization values for k training sets.
+        """
+        if average is False:
+            raise ValueError("Average must be True or a list of indices!")
+        stimulus, response, n_trials = _check_data(stimulus, response, min_len=2)
+        k = _check_k(k, n_trials)
+        xs, ys, tmin, tmax = _get_xy(stimulus, response, tmin, tmax, self.direction)
+        lags = list(range(int(np.floor(tmin * fs)), int(np.ceil(tmax * fs)) + 1))
+        if self.method == "banded":
+            coefficients = list(product(regularization, repeat=2))
+            regularization = [
+                banded_regularization(len(lags), c, bands, self.bias)
+                for c in coefficients
+            ]
+        cov_xx, cov_xy = covariance_matrices(xs, ys, lags, self.zeropad, self.bias)
+        splits = np.array_split(np.arange(n_trials), k)
+        n_splits = len(splits)
+        r_test, mse_test, best_regularization = [np.zeros(n_splits) for _ in range(3)]
+        for isplit in range(n_splits):
+            idx_test = splits[isplit]
+            idx_train_val = np.concatenate(splits[:isplit] + splits[isplit + 1 :])
+            mse = np.zeros(len(regularization))
+            for ir in _progressbar(
+                range(len(regularization)),
+                "Hyperparameter optimization",
+                verbose=verbose,
+            ):
+                _, mse[ir] = _cross_validate(
+                    self.copy(),
+                    [xs[i] for i in idx_train_val],
+                    [ys[i] for i in idx_train_val],
+                    cov_xx[idx_train_val, :, :],
+                    cov_xy[idx_train_val, :, :],
+                    lags,
+                    fs,
+                    regularization[ir],
+                    k - 1,
+                    seed=seed,
+                    average=average,
+                    verbose=verbose,
+                )
+            best_regularization[isplit] = list(regularization)[np.argmin(mse)]
+            self.train(
+                [stimulus[i] for i in idx_train_val],
+                [response[i] for i in idx_train_val],
+                fs,
+                tmin,
+                tmax,
+                best_regularization[isplit],
+            )
+            _, r_test[isplit], mse_test[isplit] = self.predict(
+                [stimulus[i] for i in idx_test], [response[i] for i in idx_test]
+            )
+        return r_test, mse_test, best_regularization
+
     def predict(
         self,
         stimulus=None,
         response=None,
         lag=None,
         average=True,
     ):
         """
-        Use the trained model to predict the response from the stimulus
-        (or vice versa) and optionally estimate the prediction's accuracy.
-        Arguments:
-            stimulus (None | list | np.ndarray): Either a 2-D samples-by-features
-                array, if the data contains only one trial or a list of such arrays
-                of it contains multiple trials. The second dimension can be omitted if
-                there only is a single stimulus feature (e.g. envelope). When using a
-                forward model, this must be specified. When using a backward model it
-                can be provided to return the prediction's error and correlation with
-                the actual response.
-            response (list | np.ndarray): Either a 2-D samples-by-channels array, if
-                the data contains only one trial or a list of such arrays of it contains
-                multiple trials. When using a forward model it can be provided to
-                return the prediction's error and correlation with the actual response.
-            lag (int | list of int | None): If not None (default), only use the
-                specified lags for prediction. The provided integers are used
-                for indexing the elements in self.times.
-            average (bool): If True (default), average correlation
-                and error across all predictions (e.g. channels in
-                the case of forward modelling) to get a single score.
-        Returns:
-            prediction (np.ndarray): Predicted output. Has the same shape as
-                the input size of the last dimension (i.e. features) is equal
-                to the last dimension in self.weights.
-            correlation (float, np.ndarray): Scalar if average is True,
-                1-dimensioal array otherwise.
-            error (float, np.ndarray):Scalar if average is True, 1-dimensional
-                array otherwise.
+        Predict response from stimulus (or vice versa) using the trained model.
+
+        The matrix of TRF weights is multiplied with the time-lagged input to predict
+        the output. If the actual output is provided, this method will estimate the
+        correlation and mean squared error of the predicted and actual output.
+
+        Parameters
+        ----------
+        stimulus: None or list or numpy.ndarray
+            Either a 2-D samples-by-features array, if the data contains only one trial
+            or a list of such arrays of it contains multiple trials. The second
+            dimension can be omitted if there only is a single stimulus feature
+            (e.g. envelope). When using a forward model, this must be specified.
+        response: None or list or numpy.ndarray
+            Either a 2-D samples-by-channels array, if the data contains only one
+            trial or a list of such arrays of it contains multiple trials. Must be
+            provided when using a backward model.
+        lag: None or in or list
+            If not None (default), only use the specified lags for prediction.
+            The provided values index the elements in self.times.
+        average: bool or list or numpy.ndarray
+            If True (default), average correlation and mean squared error across all
+            predictions (e.g. channels in the case of forward modelling). If `average`
+            is an array of integers only average the predicted features at those indices.
+            If `False`, return each predicted feature's accuracy.
+
+        Returns
+        -------
+        prediction: numpy.ndarray
+            Predicted stimulus or response
+        correlation: float or numpy.ndarray
+            When the actual output is provided, correlation is computed per trial or
+            averaged, depending on the `average` parameter.
+        error: float or numpy.ndarray
+            When the actual output is provided, mean squared error is computed per
+            trial or averaged, depending on the `average` parameter.
         """
         # check that inputs are valid
         if self.weights is None:
             raise ValueError("Can't make predictions with an untrained model!")
         if self.direction == 1 and stimulus is None:
             raise ValueError("Need stimulus to predict with a forward model!")
         elif self.direction == -1 and response is None:
             raise ValueError("Need response to predict with a backward model!")
-        if stimulus is not None:
-            stimulus = _check_data(stimulus)
-            ntrials = len(stimulus)
-        if response is not None:
-            response = _check_data(response)
-            ntrial = len(stimulus)
+        else:
+            stimulus, response, n_trials = _check_data(stimulus, response)
         if stimulus is None:
-            stimulus = [None for _ in range(ntrials)]
+            stimulus = [None for _ in range(n_trials)]
         if response is None:
-            response = [None for _ in range(ntrials)]
-        prediction, correlation, error = [], [], []  # output lists
-        for stim, resp in zip(stimulus, response):
-            if self.direction == 1:
-                x, y = stim, resp
-            elif self.direction == -1:
-                x, y = resp, stim
-            x_samples, x_features = x.shape
-            if y is None:
-                y_samples = x_samples
-                y_features = self.weights.shape[-1]
-            else:
-                y_samples, y_features = y.shape
+            response = [None for _ in range(n_trials)]
 
+        xs, ys = _get_xy(stimulus, response, direction=self.direction)
+        prediction = [np.zeros((x.shape[0], self.weights.shape[-1])) for x in xs]
+        r, mse = [], []  # output lists
+        for i, (x, y) in enumerate(zip(xs, ys)):
             lags = list(
                 range(
                     int(np.floor(self.times[0] * self.fs)),
                     int(np.ceil(self.times[-1] * self.fs)) + 1,
                 )
             )
-            delta = 1 / self.fs
-
             w = self.weights.copy()
             if lag is not None:  # select lag and corresponding weights
                 if not isinstance(lag, Iterable):
                     lag = [lag]
                 lags = list(np.array(lags)[lag])
                 w = w[:, lag, :]
-            w = (
-                np.concatenate(
-                    [
-                        self.bias,
-                        w.reshape(x_features * len(lags), y_features, order="F"),
-                    ]
-                )
-                * delta
-            )
+            w = np.concatenate(
+                [
+                    self.bias,
+                    w.reshape(
+                        x.shape[-1] * len(lags), self.weights.shape[-1], order="F"
+                    ),
+                ]
+            ) * (1 / self.fs)
             x_lag = lag_matrix(x, lags, self.zeropad)
             y_pred = x_lag @ w
             if y is not None:
                 if self.zeropad is False:
                     y = truncate(y, lags[0], lags[-1])
-                err = np.mean((y - y_pred) ** 2, axis=0)
-                r = np.mean((y - y.mean(0)) * (y_pred - y_pred.mean(0)), 0) / (
-                    y.std(0) * y_pred.std(0)
+                mse.append(np.mean((y - y_pred) ** 2, axis=0))
+                r.append(
+                    np.mean((y - y.mean(0)) * (y_pred - y_pred.mean(0)), 0)
+                    / (y.std(0) * y_pred.std(0))
                 )
-                correlation.append(r)
-                error.append(err)
-            prediction.append(y_pred)
-        if y is not None:
-            if average is True:
-                correlation, error = np.mean(correlation), np.mean(error)
-            else:  # only average across trials, not across channels/features
-                correlation, error = np.mean(correlation, axis=0), np.mean(
-                    error, axis=0
-                )
-            return prediction, correlation, error
+            prediction[i][:] = y_pred
+        if ys[0] is not None:
+            r, mse = np.mean(r, axis=0), np.mean(mse, axis=0)  # average across trials
+            if isinstance(average, list) or isinstance(average, np.ndarray):
+                r, mse = r[average], mse[average]  # select a subset of predictions
+            if average is not False:
+                r, mse = np.mean(r), np.mean(mse)
+            return prediction, r, mse
         else:
             return prediction
 
+    def to_forward(self, response):
+        """
+        Transform a backward to a forward model.
+
+        Use the method described in Haufe et al. 2014 to transform the weights of
+        a backward model into coefficients reflecting forward activation patterns
+        which have a clearer physiological interpretation.
+
+        Parameters
+        ----------
+        response: list or numpy.ndarray
+            response data which was used to train the backward model as single
+            trial in a samples-by-channels array or list of multiple trials.
+
+        Returns
+        -------
+        trf: model.TRF
+            New TRF instance with the transformed forward weights
+        """
+        assert self.direction == -1
+
+        _, response, n_trials = _check_data(None, response)
+        stim_pred = self.predict(response=response)
+
+        Cxx = 0
+        Css = 0
+        trf = self.copy()
+        trf.times = np.asarray([-i for i in reversed(trf.times)])
+        trf.direction = 1
+        for i in range(n_trials):
+            Cxx = Cxx + response[i].T @ response[i]
+            Css = Css + stim_pred[i].T @ stim_pred[i]
+        nStimChan = trf.weights.shape[-1]
+        for i in range(nStimChan):
+            trf.weights[..., i] = Cxx @ self.weights[..., i] / Css[i, i]
+
+        trf.weights = np.flip(trf.weights.T, axis=1)
+        trf.bias = np.zeros(trf.weights.shape[-1])  # need to explore
+        return trf
+
     def save(self, path):
+        """
+        Save class instance using the pickle format.
+
+        Parameters
+        ----------
+        path: str or pathlib.Path
+            File destination.
+        """
         path = Path(path)
         if not path.parent.exists():
             raise FileNotFoundError(f"The directory {path.parent} does not exist!")
         with open(path, "wb") as fname:
             pickle.dump(self, fname, pickle.HIGHEST_PROTOCOL)
 
     def load(self, path):
+        """
+        Load pickle file - instance variables will be overwritten with file content.
+
+        Parameters
+        ----------
+        path: str or pathlib.Path
+            File destination.
+        """
         path = Path(path)
         if not path.exists():
             raise FileNotFoundError(f"The file {path} does not exist!")
         with open(path, "rb") as fname:
             trf = pickle.load(fname)
         self.__dict__ = trf.__dict__
 
     def copy(self):
+        """Return a copy of the TRF instance"""
         trf = TRF()
         for k, v in self.__dict__.items():
             value = v
             if getattr(v, "copy", None) is not None:
                 value = v.copy()
             setattr(trf, k, value)
         return trf
@@ -387,37 +578,33 @@
         channel=None,
         feature=None,
         axes=None,
         show=True,
         kind="line",
     ):
         """
-        Plot the weights of the (forward) model across time for
-        a select channel or feature.
+        Plot the weights of the (forward) model across time for a select channel or feature.
+
         Arguments:
-            channel (None | int | str): Channel selection. If None, all channels
-                will be used. If an integer, the channel at that index will be used.
-                If 'avg' or 'gfp' , the average or standard deviation across channels
-                will be computed.
-            feature (None | int | str): Feature selection. If None, all features
-                will be used. If an integer, the feature at that index will be used.
-                If 'avg' , the average across features will be computed.
-            axes (matplotlib.axes.Axes): Axis to plot to. If None is
-                provided (default) generate a new plot.
+            channel (None | int | str): Channel selection. If None, all channels will be used. If an integer, the channel at that index will be used. If 'avg' or 'gfp' , the average or standard deviation across channels will be computed.
+            feature (None | int | str): Feature selection. If None, all features will be used. If an integer, the feature at that index will be used. If 'avg' , the average across features will be computed.
+            axes (matplotlib.axes.Axes): Axis to plot to. If None is provided (default) generate a new plot.
             show (bool): If True (default), show the plot after drawing.
-            kind (str): Type of plot to draw. If 'line' (default), average
-                the weights across all stimulus features, if 'image' draw
-                a features-by-times plot where the weights are color-coded.
+            kind (str): Type of plot to draw. If 'line' (default), average the weights across all stimulus features, if 'image' draw a features-by-times plot where the weights are color-coded.
+
         Returns:
-            fig (matplotlib.figure.Figure): If now axes was provided and
-                a new figure is created, it is returned.
+            fig (matplotlib.figure.Figure): If now axes was provided and a new figure is created, it is returned.
         """
+        if plt is None:
+            raise ModuleNotFoundError("Need matplotlib to plot TRF!")
         if self.direction == -1:
-            # TODO: implement backward to forward transformation
-            raise ValueError("Not implemented for decoding models!")
+            weights = self.weight.T
+            print(
+                "WARNING: decoder weights are hard to interpret, consider using the `to_forward()` method"
+            )
         if axes is None:
             fig, ax = plt.subplots(figsize=(6, 6))
         else:
             fig, ax = None, axes  # dont create a new figure
         weights = self.weights
         # select channel and or feature
         if channel is None and feature is None:
@@ -470,30 +657,113 @@
                 xlim=(self.times.min(), self.times.max()),
             )
         if show is True:
             plt.show()
         if fig is not None:
             return fig
 
+    def to_mne_evoked(self, info, include=None, **kwargs):
+        """
+        Output TRF weights as instance(s) of MNE-Python's EvokedArray.
+
+        Create one instance of ``mne.EvokedArray`` for each feature along the first
+        (i.e. input) dimension of ``self.weights``. When using a backward model,
+        the weights are transposed to obtain one EvokedArray per decoded feature.
+        See the MNE-Python documentation for details on the Evoked class.
+
+        Parameters
+        ----------
+        info: mne.Info or mne.channels.montage.DigMontage
+            Either a basic info or montage containing channel locations
+            Information neccessary to build the EvokedArray.
+        include: None or in or list
+            Indices of the stimulus features to include. If None (default),
+            create one Evoked object for each feature.
+        kwargs: dict
+            other parameters for constructing the EvokedArray
+
+        Returns
+        -------
+        evokeds: list
+            One Evoked instance for each included TRF feature.
+        """
+        if mne is False:
+            raise ModuleNotFoundError("To use this function, mne must be installed!")
+        if self.direction == -1:
+            weights = self.weights.T
+        else:
+            weights = self.weights
+        if isinstance(info, mne.channels.montage.DigMontage):
+            kinds = [d["kind"] for d in info.copy().remove_fiducials().dig]
+            ch_types = []
+            for k in kinds:
+                if "eeg" in str(k).lower():
+                    ch_types.append("eeg")
+                if "mag" in str(k).lower():
+                    ch_types.append("mag")
+                if "grad" in str(k).lower():
+                    ch_types.append("grad")
+            mne_info = mne.create_info(info.ch_names, self.fs, ch_types)
+        if isinstance(include, list) or isinstance(include, np.ndarray):
+            weights = weights[np.asarray(include), :, :]
+        evokeds = []
+        for w in weights:
+            evoked = mne.EvokedArray(w.T.copy(), mne_info, tmin=self.times[0], **kwargs)
+            if isinstance(info, mne.channels.montage.DigMontage):
+                evoked.set_montage(info)
+            evokeds.append(evoked)
+        return evokeds
+
 
-def load_sample_data(path=None):
+def load_sample_data(path=None, n_segments=1, normalize=True):
     """
-    Load the sample data containing a small snippet of brain responses to naturalstic
-    speech and the 16-band spectrogram of that speech. The data will be
-    automatically downloaded the first time.
-    Arguments:
-        path (str | inst of Path | None): Full path to the folder where the sample
-            data will be stored. If None (default), a folder called mtrf_data in the
-            users home directory is assumed and created if it does not exist.
+    Load sample of brain responses to naturalistic speech.
+
+    If no path is provided, the data is assumed to be in a folder called mtrf_data
+    in the users home directory and will be downloaded and stored there if it can't
+    be found. The data contains about 2 minutes of brain responses to naturalistic
+    speech, recorded with a 128-channel Biosemi EEG system and the 16-band spectrogram
+    of that speech.
+
+    Parameters
+    ----------
+    path: str or pathlib.Path
+        Destination where the sample data is stored or will be downloaded to. If None
+        (default), a folder called mtrf_data in the users home directory is assumed
+        and created if it does not exist.
+
+    Returns
+    -------
+    stimulus: numpy.ndarray
+        Samples-by-features array of the presented speech's spectrogram.
+    response : numpy.ndarray
+        Samples-by-channels array of the recorded neural response.
+    fs: int
+        Sampling rate of stimulus and response in Hz.
     """
     if path == None:  # use default path
         path = Path.home() / "mtrf_data"
         if not path.exists():
             path.mkdir()
     else:
         path = Path(path)
     if not (path / "speech_data.npy").exists():  # download the data
         url = "https://github.com/powerfulbean/mTRFpy/raw/master/tests/data/speech_data.npy"
         response = requests.get(url, allow_redirects=True)
         open(path / "speech_data.npy", "wb").write(response.content)
     data = np.load(str(path / "speech_data.npy"), allow_pickle=True).item()
-    return data["stimulus"], data["response"], data["samplerate"][0]
+    stimulus, response, fs = (
+        data["stimulus"],
+        data["response"],
+        data["samplerate"][0][0],
+    )
+    stimulus = np.array_split(stimulus, n_segments)
+    response = np.array_split(response, n_segments)
+    if normalize:
+        for i in range(len(stimulus)):
+            stimulus[i] = (stimulus[i] - stimulus[i].mean(axis=0)) / stimulus[i].std(
+                axis=0
+            )
+            response[i] = (response[i] - response[i].mean(axis=0)) / response[i].std(
+                axis=0
+            )
+    return stimulus, response, fs
```

### Comparing `mtrf-1.1.0/setup.py` & `mtrf-1.2.0/setup.py`

 * *Files identical despite different names*

