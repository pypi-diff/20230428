# Comparing `tmp/mtrf-1.2.0.tar.gz` & `tmp/mtrf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtrf-1.2.0.tar", last modified: Fri Apr 28 15:34:26 2023, max compression
+gzip compressed data, was "mtrf-1.2.1.tar", last modified: Fri Apr 28 18:39:26 2023, max compression
```

## Comparing `mtrf-1.2.0.tar` & `mtrf-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1515 2023-03-03 16:11:35.000000 mtrf-1.2.0/LICENSE
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 15:34:26.970278 mtrf-1.2.0/PKG-INFO
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1632 2023-03-21 15:29:42.000000 mtrf-1.2.0/README.md
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.966278 mtrf-1.2.0/mtrf/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       59 2023-04-28 15:33:31.000000 mtrf-1.2.0/mtrf/__init__.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     9184 2023-04-25 15:15:02.000000 mtrf-1.2.0/mtrf/matrices.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    31493 2023-04-27 16:29:57.000000 mtrf-1.2.0/mtrf/model.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    10115 2023-04-27 17:12:48.000000 mtrf-1.2.0/mtrf/stats.py
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/mtrf.egg-info/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/PKG-INFO
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)      345 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/SOURCES.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/dependency_links.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 15:26:52.000000 mtrf-1.2.0/mtrf.egg-info/not-zip-safe
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       46 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/requires.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        5 2023-04-28 15:34:26.000000 mtrf-1.2.0/mtrf.egg-info/top_level.txt
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       38 2023-04-28 15:34:26.970278 mtrf-1.2.0/setup.cfg
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1017 2023-03-16 20:54:02.000000 mtrf-1.2.0/setup.py
-drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 15:34:26.970278 mtrf-1.2.0/tests/
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2824 2023-04-25 14:52:40.000000 mtrf-1.2.0/tests/test_basics.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     3395 2023-04-25 16:38:00.000000 mtrf-1.2.0/tests/test_matlab_examples.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2537 2023-04-25 16:44:01.000000 mtrf-1.2.0/tests/test_model.py
--rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1417 2023-04-25 16:48:57.000000 mtrf-1.2.0/tests/test_stats.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 18:39:26.579016 mtrf-1.2.1/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1515 2023-03-03 16:11:35.000000 mtrf-1.2.1/LICENSE
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 18:39:26.579016 mtrf-1.2.1/PKG-INFO
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1632 2023-03-21 15:29:42.000000 mtrf-1.2.1/README.md
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 18:39:26.575016 mtrf-1.2.1/mtrf/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       59 2023-04-28 18:27:34.000000 mtrf-1.2.1/mtrf/__init__.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     9217 2023-04-28 18:06:16.000000 mtrf-1.2.1/mtrf/matrices.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    31493 2023-04-28 17:23:03.000000 mtrf-1.2.1/mtrf/model.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)    10197 2023-04-28 17:22:56.000000 mtrf-1.2.1/mtrf/stats.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 18:39:26.575016 mtrf-1.2.1/mtrf.egg-info/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2112 2023-04-28 18:39:26.000000 mtrf-1.2.1/mtrf.egg-info/PKG-INFO
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)      345 2023-04-28 18:39:26.000000 mtrf-1.2.1/mtrf.egg-info/SOURCES.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 18:39:26.000000 mtrf-1.2.1/mtrf.egg-info/dependency_links.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        1 2023-04-28 15:26:52.000000 mtrf-1.2.1/mtrf.egg-info/not-zip-safe
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       46 2023-04-28 18:39:26.000000 mtrf-1.2.1/mtrf.egg-info/requires.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        5 2023-04-28 18:39:26.000000 mtrf-1.2.1/mtrf.egg-info/top_level.txt
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)       38 2023-04-28 18:39:26.579016 mtrf-1.2.1/setup.cfg
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1017 2023-03-16 20:54:02.000000 mtrf-1.2.1/setup.py
+drwxr-xr-x   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)        0 2023-04-28 18:39:26.579016 mtrf-1.2.1/tests/
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2824 2023-04-25 14:52:40.000000 mtrf-1.2.1/tests/test_basics.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     3395 2023-04-25 16:38:00.000000 mtrf-1.2.1/tests/test_matlab_examples.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     2537 2023-04-25 16:44:01.000000 mtrf-1.2.1/tests/test_model.py
+-rw-r--r--   0 obialas@urmc-sh.rochester.edu (1140448484) domain users@urmc-sh.rochester.edu (708800513)     1417 2023-04-25 16:48:57.000000 mtrf-1.2.1/tests/test_stats.py
```

### Comparing `mtrf-1.2.0/LICENSE` & `mtrf-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/PKG-INFO` & `mtrf-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtrf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for modeling brain responses using (multivariate)temporal response functions.
 Home-page: http://github.com/powerfulbean/mTRFpy
 Author: powerfulbean
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mtrf-1.2.0/README.md` & `mtrf-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/mtrf/matrices.py` & `mtrf-1.2.1/mtrf/matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
             If True raise an error if `data` is not a list
         assert_len: bool or int
             If an integer, raise an error if the length of `data` does not
             equal that value.
         unisize: bool
             If True, crop all trials to the length of the shortest one to enforce
             equal size.
-
     Returns
     -------
         data (list): Data in a list of arrays with added singelton dimension if the arrays
             were 1-dimensional.
     """
     for i, data in enumerate([stimulus, response]):
         if isinstance(data, np.ndarray):  # convert array to list
-            if data.ndim == 1:
-                data = np.expand_dims(data, axis=1)
             if data.ndim > 2:
                 raise ValueError("Array cant have more that three dimensions!")
-            data = [data]
+            else:
+                data = [data]
         if data is not None:
-            if len(data) < min_len:  # check length
-                raise ValueError("Data list is too short!")
-            if crop is True:  # crop all trials to same number of samples
-                min_n = min([len(d) for d in data])
-                for i in range(len(data)):
-                    data[i] = data[i][:min_n, :]
             n_trials = len(data)
+            if n_trials < min_len:  # check length
+                raise ValueError("Data list is too short!")
+            min_n = min([len(d) for d in data])
+            for j in range(len(data)):
+                if data[j].ndim == 1:
+                    data[j] = np.expand_dims(data[j], axis=1)
+                if crop is True:  # crop all trials to same number of samples
+                    data[j] = data[j][:min_n, :]
         if i == 0:
             stimulus = data
         else:
             response = data
     if (stimulus is not None) and (response is not None):
         if (not len(stimulus) == len(response)) or (
             not all([s.shape[0] == r.shape[0] for s, r in zip(stimulus, response)])
```

### Comparing `mtrf-1.2.0/mtrf/model.py` & `mtrf-1.2.1/mtrf/model.py`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/mtrf/stats.py` & `mtrf-1.2.1/mtrf/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         idx_train = np.concatenate(splits[:isplit] + splits[isplit + 1 :])  # flatten
         # compute the model for the training set
         cov_xx_hat = cov_xx[idx_train].mean(axis=0)
         cov_xy_hat = cov_xy[idx_train].mean(axis=0)
         w = np.matmul(np.linalg.inv(cov_xx_hat + regmat), cov_xy_hat) / (1 / fs)
         trf = model.copy()
         trf.times, trf.bias, trf.fs = np.array(lags) / fs, w[0:1], fs
+        if trf.bias.ndim == 1:
+            trf.bias = np.expand_dims(trf.bias, 1)
         trf.weights = w[1:].reshape(
             (x[0].shape[-1], len(lags), y[0].shape[-1]), order="F"
         )
         # use the model to predict the test data
         x_test, y_test = [x[i] for i in idx_val], [y[i] for i in idx_val]
         if model.direction == 1:
             _, r_test, mse_test = trf.predict(x_test, y_test, average=average)
```

### Comparing `mtrf-1.2.0/mtrf.egg-info/PKG-INFO` & `mtrf-1.2.1/mtrf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtrf
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for modeling brain responses using (multivariate)temporal response functions.
 Home-page: http://github.com/powerfulbean/mTRFpy
 Author: powerfulbean
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mtrf-1.2.0/setup.py` & `mtrf-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/tests/test_basics.py` & `mtrf-1.2.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/tests/test_matlab_examples.py` & `mtrf-1.2.1/tests/test_matlab_examples.py`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/tests/test_model.py` & `mtrf-1.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `mtrf-1.2.0/tests/test_stats.py` & `mtrf-1.2.1/tests/test_stats.py`

 * *Files identical despite different names*

