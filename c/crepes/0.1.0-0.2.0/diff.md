# Comparing `tmp/crepes-0.1.0.tar.gz` & `tmp/crepes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepes-0.1.0.tar", last modified: Tue Jun 28 13:30:55 2022, max compression
+gzip compressed data, was "crepes-0.2.0.tar", last modified: Fri Apr 28 07:58:51 2023, max compression
```

## Comparing `crepes-0.1.0.tar` & `crepes-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2022-06-28 13:30:55.369450 crepes-0.1.0/
--rw-rw-r--   0 henke     (1000) henke     (1000)     1459 2022-06-27 06:33:15.000000 crepes-0.1.0/LICENSE
--rw-rw-r--   0 henke     (1000) henke     (1000)    15016 2022-06-28 13:30:55.369450 crepes-0.1.0/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)    14493 2022-06-28 13:25:06.000000 crepes-0.1.0/README.md
--rw-rw-r--   0 henke     (1000) henke     (1000)      106 2022-06-28 07:30:29.000000 crepes-0.1.0/pyproject.toml
--rw-rw-r--   0 henke     (1000) henke     (1000)       38 2022-06-28 13:30:55.369450 crepes-0.1.0/setup.cfg
--rw-rw-r--   0 henke     (1000) henke     (1000)      865 2022-06-27 06:32:09.000000 crepes-0.1.0/setup.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2022-06-28 13:30:55.369450 crepes-0.1.0/src/
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2022-06-28 13:30:55.369450 crepes-0.1.0/src/crepes/
--rw-rw-r--   0 henke     (1000) henke     (1000)      433 2022-06-28 07:15:47.000000 crepes-0.1.0/src/crepes/__init__.py
--rw-rw-r--   0 henke     (1000) henke     (1000)    27935 2022-06-28 07:16:24.000000 crepes-0.1.0/src/crepes/base.py
--rw-rw-r--   0 henke     (1000) henke     (1000)     6102 2022-06-27 11:48:41.000000 crepes-0.1.0/src/crepes/fillings.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2022-06-28 13:30:55.369450 crepes-0.1.0/src/crepes.egg-info/
--rw-rw-r--   0 henke     (1000) henke     (1000)    15016 2022-06-28 13:30:55.000000 crepes-0.1.0/src/crepes.egg-info/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)      275 2022-06-28 13:30:55.000000 crepes-0.1.0/src/crepes.egg-info/SOURCES.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        1 2022-06-28 13:30:55.000000 crepes-0.1.0/src/crepes.egg-info/dependency_links.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)       13 2022-06-28 13:30:55.000000 crepes-0.1.0/src/crepes.egg-info/requires.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        7 2022-06-28 13:30:55.000000 crepes-0.1.0/src/crepes.egg-info/top_level.txt
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/
+-rw-rw-r--   0 henke     (1000) henke     (1000)     1459 2023-04-28 07:57:14.000000 crepes-0.2.0/LICENSE
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15213 2023-04-28 07:58:51.491480 crepes-0.2.0/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)    14690 2023-04-28 07:32:04.000000 crepes-0.2.0/README.md
+-rw-rw-r--   0 henke     (1000) henke     (1000)      106 2022-06-28 07:30:29.000000 crepes-0.2.0/pyproject.toml
+-rw-rw-r--   0 henke     (1000) henke     (1000)       38 2023-04-28 07:58:51.491480 crepes-0.2.0/setup.cfg
+-rw-rw-r--   0 henke     (1000) henke     (1000)      865 2023-04-12 14:34:32.000000 crepes-0.2.0/setup.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/crepes/
+-rw-rw-r--   0 henke     (1000) henke     (1000)      104 2023-04-12 11:57:09.000000 crepes-0.2.0/src/crepes/__init__.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)    42079 2023-04-27 16:41:21.000000 crepes-0.2.0/src/crepes/base.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)     8365 2023-04-27 15:14:46.000000 crepes-0.2.0/src/crepes/fillings.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-04-28 07:58:51.491480 crepes-0.2.0/src/crepes.egg-info/
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15213 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)      275 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/SOURCES.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        1 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/dependency_links.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)       13 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/requires.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        7 2023-04-28 07:58:51.000000 crepes-0.2.0/src/crepes.egg-info/top_level.txt
```

### Comparing `crepes-0.1.0/LICENSE` & `crepes-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Henrik Boström
+Copyright 2023 Henrik Boström
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `crepes-0.1.0/PKG-INFO` & `crepes-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.1.0
+Version: 0.2.0
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `crepes`: Conformal Regressors and Predictive Systems
+# `crepes`
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with: `pip install crepes`
+Install with:
 
-## Quick start
+```bash
+pip install crepes
+```
+
+## Documentation
+
+For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
+
+## Quickstart
 
 ### Conformal regressors
 
 We first import the main class and two helper functions:
 
 ```python
 from crepes import ConformalRegressor
 from crepes.fillings import sigma_knn, binning
 ```
 
-We will illustrate the above using a dataset from www.openml.org and a `RandomForestRegressor` from `sklearn`:
+We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestRegressor
 
 dataset = fetch_openml(name="house_sales", version=3)
@@ -71,81 +79,81 @@
 ```
 
 We can now apply the conformal regressor to get prediction intervals for the test objects, using the point predictions as input, where the probability of not including the correct target in an interval is 1-confidence:
 ```python
 std_intervals = cr_std.predict(y_hat=y_hat_test, confidence=0.99)
 ```
 
-The output is a NumPy array, specifying the lower and upper bound of each interval:
+The output is a [NumPy](https://numpy.org) array, specifying the lower and upper bound of each interval:
 
 ```numpy
-array([[-353379.  ,  939231.  ],
-       [-251874.3 , 1040735.7 ],
-       [-138329.5 , 1154280.5 ],
+array([[-171902.2 ,  953866.2 ],
+       [-276818.01,  848950.39],
+       [  22679.37, 1148447.77],
        ...,
-       [-389128.68,  903481.32],
-       [-313003.  ,  979607.  ],
-       [ -90551.53, 1202058.47]])
+       [ 242954.02, 1368722.42],
+       [-308093.73,  817674.67],
+       [-227057.4 ,  898711.  ]])
 ```
 
 We may request that the intervals are cut to exclude impossible values, in this case below 0, and if we also rely on the default confidence level (0.95), the output intervals will be a bit tighter:
 
 ```python
 intervals_std = cr_std.predict(y_hat=y_hat_test, y_min=0)
 ```
 
 ```numpy
-array([[  7576.18, 578275.82],
-       [109080.88, 679780.52],
-       [222625.68, 793325.32],
+array([[ 152258.55,  629705.45],
+       [  47342.74,  524789.64],
+       [ 346840.12,  824287.02],
        ...,
-       [     0.  , 542526.14],
-       [ 47952.18, 618651.82],
-       [270403.65, 841103.29]])
+       [ 567114.77, 1044561.67],
+       [  16067.02,  493513.92],
+       [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will here use the helper function `sigma_knn` for this purpose. It estimates the difficulty by the mean absolute errors of the k (default `k=5`) nearest neighbors to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through a (named) argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, residuals=residuals_cal)
+sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the calibration objects and residuals. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
 
 ```python
-sigmas_test = sigma_knn(X=X_cal, residuals=residuals_cal, X_test=X_test)
+sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 645527.3140099 ],
-       [100552.5573358 , 688308.8426642 ],
-       [206605.7263972 , 809345.2736028 ],
+array([[205959.07517616, 576004.92482384],
+       [133206.86035366, 438925.51964634],
+       [291925.81345507, 879201.32654493],
        ...,
-       [ 55388.60029434, 458964.03970566],
-       [252094.62400964, 414509.37599036],
-       [305546.225071  , 805960.714929  ]])
+       [622212.95112744, 989463.48887256],
+       [ 98805.77755066, 410775.16244934],
+       [197248.38670265, 474405.21329735]])
 ```
 
-Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no informatoion on the expected error should instead lead to more uniformly distributed interval sizes.
+Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
 
 ```python
 bins_cal, bin_thresholds = binning(values=sigmas_cal, bins=20)
@@ -167,21 +175,21 @@
 Now we have everything we need to get the prediction intervals:
 
 ```python
 intervals_mond = cr_mond.predict(y_hat=y_hat_test, bins=bins_test, y_min=0)
 ```
 
 ```numpy
-array([[     0.  , 592782.5 ],
-       [146648.15, 642213.25],
-       [260192.95, 755758.05],
+array([[ 206379.7 ,  575584.3 ],
+       [ 144014.65,  428117.73],
+       [  17965.57, 1153161.57],
        ...,
-       [ 38332.66, 476019.98],
-       [198148.5 , 468455.5 ],
-       [329931.17, 781575.77]])
+       [ 653865.22,  957811.22],
+       [ 174264.87,  335316.07],
+       [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
 The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
@@ -212,70 +220,64 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 537757.93618585],
-       [177348.62535049, 655015.98985999],
-       [253618.31669927, 783707.98804461],
+array([[ 226536.76784152,  519404.56955659],
+       [ 170043.51497485,  376524.37491457],
+       [ 192376.08061079,  994115.461665  ],
        ...,
-       [ 73466.09003216, 397289.46238233],
-       [273315.68901744, 405309.55870912],
-       [274035.55188125, 789701.43635318]])
+       [ 594183.11971763, 1010273.54816378],
+       [ 186478.52365968,  308050.53035102],
+       [ 167498.01540504,  485813.1329371 ]])
 ```
 
 We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.3262945 ],
-       [0.12184386],
-       [0.82948135],
+array([[0.98298087],
+       [0.90125379],
+       [0.41770673],
        ...,
-       [0.75042278],
-       [0.61815831],
-       [0.70252814]])
+       [0.04659288],
+       [0.07914733],
+       [0.31090332]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
                              bins=bins_test,
                              return_cpds=True)
 ```
 
 The resulting vector of arrays is not displayed here, but we instead provide a plot for the CPD of a random test instance:
 
-![cpd](https://user-images.githubusercontent.com/7838741/176182669-1cb739dc-dc38-4c30-80b1-624c2f6b4b83.png)
+![cpd](https://user-images.githubusercontent.com/7838741/235081969-328d7a23-26c9-4799-a246-8c35fd7ac88e.png)
 
 ## Examples
 
-For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/crepes.ipynb).
-
-## Documentation
-
-For documentation of the `crepes` package, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.html).
-
-For documentation of the `crepes.fillings` module, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.fillings.html).
+For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [the documentation](https://crepes.readthedocs.io/en/latest/) and [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/docs/crepes_nb.ipynb).
 
 ## Citing crepes
 
 If you use `crepes` for a scientific publication, you may cite the following paper:
 
-Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179.
+Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179. [Link](https://copa-conference.com/papers/COPA2022_paper_11.pdf)
 
 Bibtex entry:
 
 ```bibtex
 @InProceedings{crepes,
   title = 	 {crepes: a Python Package for Generating Conformal Regressors and Predictive Systems},
   author =       {Bostr\"om, Henrik},
@@ -300,12 +302,15 @@
 
 <a id="5">[5]</a> Boström, H. and Johansson, U., 2020. Mondrian conformal regressors. In Conformal and Probabilistic Prediction and Applications. PMLR, 128, pp. 114-133. [Link](https://proceedings.mlr.press/v128/bostrom20a.html)
 
 <a id="6">[6]</a> Vovk, V., Petej, I., Nouretdinov, I., Manokhin, V. and Gammerman, A., 2020. Computationally efficient versions of conformal predictive distributions. Neurocomputing, 397, pp.292-308. [Link](https://www.aminer.org/pub/5e09aac9df1a9c0c416c9b70/computationally-efficient-versions-of-conformal-predictive-distributions)
 
 <a id="7">[7]</a> Boström, H., Johansson, U. and Löfström, T., 2021. Mondrian conformal predictive distributions. In Conformal and Probabilistic Prediction and Applications. PMLR, 152, pp. 24-38. [Link](https://proceedings.mlr.press/v152/bostrom21a.html)
 
+<a id="8">[8]</a> Vovk, V., 2022. Universal predictive systems. Pattern Recognition. 126: pp. 108536 [Link](https://dl.acm.org/doi/abs/10.1016/j.patcog.2022.108536)
+
+
 - - -
 
 Author: Henrik Boström (bostromh@kth.se)
-Copyright 2022 Henrik Boström
+Copyright 2023 Henrik Boström
 License: BSD 3 clause
```

### Comparing `crepes-0.1.0/README.md` & `crepes-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-# `crepes`: Conformal Regressors and Predictive Systems
+# `crepes`
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with: `pip install crepes`
+Install with:
 
-## Quick start
+```bash
+pip install crepes
+```
+
+## Documentation
+
+For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
+
+## Quickstart
 
 ### Conformal regressors
 
 We first import the main class and two helper functions:
 
 ```python
 from crepes import ConformalRegressor
 from crepes.fillings import sigma_knn, binning
 ```
 
-We will illustrate the above using a dataset from www.openml.org and a `RandomForestRegressor` from `sklearn`:
+We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestRegressor
 
 dataset = fetch_openml(name="house_sales", version=3)
@@ -56,81 +64,81 @@
 ```
 
 We can now apply the conformal regressor to get prediction intervals for the test objects, using the point predictions as input, where the probability of not including the correct target in an interval is 1-confidence:
 ```python
 std_intervals = cr_std.predict(y_hat=y_hat_test, confidence=0.99)
 ```
 
-The output is a NumPy array, specifying the lower and upper bound of each interval:
+The output is a [NumPy](https://numpy.org) array, specifying the lower and upper bound of each interval:
 
 ```numpy
-array([[-353379.  ,  939231.  ],
-       [-251874.3 , 1040735.7 ],
-       [-138329.5 , 1154280.5 ],
+array([[-171902.2 ,  953866.2 ],
+       [-276818.01,  848950.39],
+       [  22679.37, 1148447.77],
        ...,
-       [-389128.68,  903481.32],
-       [-313003.  ,  979607.  ],
-       [ -90551.53, 1202058.47]])
+       [ 242954.02, 1368722.42],
+       [-308093.73,  817674.67],
+       [-227057.4 ,  898711.  ]])
 ```
 
 We may request that the intervals are cut to exclude impossible values, in this case below 0, and if we also rely on the default confidence level (0.95), the output intervals will be a bit tighter:
 
 ```python
 intervals_std = cr_std.predict(y_hat=y_hat_test, y_min=0)
 ```
 
 ```numpy
-array([[  7576.18, 578275.82],
-       [109080.88, 679780.52],
-       [222625.68, 793325.32],
+array([[ 152258.55,  629705.45],
+       [  47342.74,  524789.64],
+       [ 346840.12,  824287.02],
        ...,
-       [     0.  , 542526.14],
-       [ 47952.18, 618651.82],
-       [270403.65, 841103.29]])
+       [ 567114.77, 1044561.67],
+       [  16067.02,  493513.92],
+       [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will here use the helper function `sigma_knn` for this purpose. It estimates the difficulty by the mean absolute errors of the k (default `k=5`) nearest neighbors to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through a (named) argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, residuals=residuals_cal)
+sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the calibration objects and residuals. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
 
 ```python
-sigmas_test = sigma_knn(X=X_cal, residuals=residuals_cal, X_test=X_test)
+sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 645527.3140099 ],
-       [100552.5573358 , 688308.8426642 ],
-       [206605.7263972 , 809345.2736028 ],
+array([[205959.07517616, 576004.92482384],
+       [133206.86035366, 438925.51964634],
+       [291925.81345507, 879201.32654493],
        ...,
-       [ 55388.60029434, 458964.03970566],
-       [252094.62400964, 414509.37599036],
-       [305546.225071  , 805960.714929  ]])
+       [622212.95112744, 989463.48887256],
+       [ 98805.77755066, 410775.16244934],
+       [197248.38670265, 474405.21329735]])
 ```
 
-Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no informatoion on the expected error should instead lead to more uniformly distributed interval sizes.
+Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
 
 ```python
 bins_cal, bin_thresholds = binning(values=sigmas_cal, bins=20)
@@ -152,21 +160,21 @@
 Now we have everything we need to get the prediction intervals:
 
 ```python
 intervals_mond = cr_mond.predict(y_hat=y_hat_test, bins=bins_test, y_min=0)
 ```
 
 ```numpy
-array([[     0.  , 592782.5 ],
-       [146648.15, 642213.25],
-       [260192.95, 755758.05],
+array([[ 206379.7 ,  575584.3 ],
+       [ 144014.65,  428117.73],
+       [  17965.57, 1153161.57],
        ...,
-       [ 38332.66, 476019.98],
-       [198148.5 , 468455.5 ],
-       [329931.17, 781575.77]])
+       [ 653865.22,  957811.22],
+       [ 174264.87,  335316.07],
+       [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
 The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
@@ -197,70 +205,64 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 537757.93618585],
-       [177348.62535049, 655015.98985999],
-       [253618.31669927, 783707.98804461],
+array([[ 226536.76784152,  519404.56955659],
+       [ 170043.51497485,  376524.37491457],
+       [ 192376.08061079,  994115.461665  ],
        ...,
-       [ 73466.09003216, 397289.46238233],
-       [273315.68901744, 405309.55870912],
-       [274035.55188125, 789701.43635318]])
+       [ 594183.11971763, 1010273.54816378],
+       [ 186478.52365968,  308050.53035102],
+       [ 167498.01540504,  485813.1329371 ]])
 ```
 
 We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.3262945 ],
-       [0.12184386],
-       [0.82948135],
+array([[0.98298087],
+       [0.90125379],
+       [0.41770673],
        ...,
-       [0.75042278],
-       [0.61815831],
-       [0.70252814]])
+       [0.04659288],
+       [0.07914733],
+       [0.31090332]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
                              bins=bins_test,
                              return_cpds=True)
 ```
 
 The resulting vector of arrays is not displayed here, but we instead provide a plot for the CPD of a random test instance:
 
-![cpd](https://user-images.githubusercontent.com/7838741/176182669-1cb739dc-dc38-4c30-80b1-624c2f6b4b83.png)
+![cpd](https://user-images.githubusercontent.com/7838741/235081969-328d7a23-26c9-4799-a246-8c35fd7ac88e.png)
 
 ## Examples
 
-For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/crepes.ipynb).
-
-## Documentation
-
-For documentation of the `crepes` package, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.html).
-
-For documentation of the `crepes.fillings` module, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.fillings.html).
+For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [the documentation](https://crepes.readthedocs.io/en/latest/) and [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/docs/crepes_nb.ipynb).
 
 ## Citing crepes
 
 If you use `crepes` for a scientific publication, you may cite the following paper:
 
-Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179.
+Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179. [Link](https://copa-conference.com/papers/COPA2022_paper_11.pdf)
 
 Bibtex entry:
 
 ```bibtex
 @InProceedings{crepes,
   title = 	 {crepes: a Python Package for Generating Conformal Regressors and Predictive Systems},
   author =       {Bostr\"om, Henrik},
@@ -285,12 +287,15 @@
 
 <a id="5">[5]</a> Boström, H. and Johansson, U., 2020. Mondrian conformal regressors. In Conformal and Probabilistic Prediction and Applications. PMLR, 128, pp. 114-133. [Link](https://proceedings.mlr.press/v128/bostrom20a.html)
 
 <a id="6">[6]</a> Vovk, V., Petej, I., Nouretdinov, I., Manokhin, V. and Gammerman, A., 2020. Computationally efficient versions of conformal predictive distributions. Neurocomputing, 397, pp.292-308. [Link](https://www.aminer.org/pub/5e09aac9df1a9c0c416c9b70/computationally-efficient-versions-of-conformal-predictive-distributions)
 
 <a id="7">[7]</a> Boström, H., Johansson, U. and Löfström, T., 2021. Mondrian conformal predictive distributions. In Conformal and Probabilistic Prediction and Applications. PMLR, 152, pp. 24-38. [Link](https://proceedings.mlr.press/v152/bostrom21a.html)
 
+<a id="8">[8]</a> Vovk, V., 2022. Universal predictive systems. Pattern Recognition. 126: pp. 108536 [Link](https://dl.acm.org/doi/abs/10.1016/j.patcog.2022.108536)
+
+
 - - -
 
 Author: Henrik Boström (bostromh@kth.se)
-Copyright 2022 Henrik Boström
+Copyright 2023 Henrik Boström
 License: BSD 3 clause
```

### Comparing `crepes-0.1.0/setup.py` & `crepes-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crepes",
-    version="0.1.0",
+    version="0.2.0",
     author="Henrik Boström",
     author_email="bostromh@kth.se",
     description="Conformal regressors and predictive systems (crepes)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henrikbostrom/crepes",
     project_urls={
```

### Comparing `crepes-0.1.0/src/crepes/base.py` & `crepes-0.2.0/src/crepes/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,51 +2,48 @@
 
 Classes implementing conformal regressors and conformal predictive
 systems, which transform point predictions into prediction intervals
 and cumulative distribution functions, respectively.
 
 Author: Henrik Boström (bostromh@kth.se)
 
-Copyright 2022 Henrik Boström
+Copyright 2023 Henrik Boström
 
 License: BSD 3 clause
 """
 
 import numpy as np
 import pandas as pd
 import time
+import warnings
 
-__version__ = "0.1.0"
+warnings.simplefilter("always", UserWarning)
+
+__version__ = "0.2.0"
 
 class ConformalPredictor():
     """
-    Conformal Predictor.
-
     The class contains two sub-classes: ConformalRegressor 
     and ConformalPredictiveSystem.
-    
     """
     
     def __init__(self):
         self.alphas = None
         self.fitted = False
         self.normalized = None
         self.mondrian = None
         self.time_fit = None
         self.time_predict = None
         self.time_evaluate = None
 
         
 class ConformalRegressor(ConformalPredictor):
     """
-    Conformal Regressor.
-
     A conformal regressor transforms point predictions (regression 
-    values) into prediction intervals, for a certain confidence level.  
-    
+    values) into prediction intervals, for a certain confidence level.
     """
     
     def __repr__(self):
         if self.fitted:
             return (f"ConformalRegressor(fitted={self.fitted}, "
                     f"normalized={self.normalized}, "
                     f"mondrian={self.mondrian})")
@@ -56,26 +53,68 @@
     def fit(self, residuals=None, sigmas=None, bins=None):
         """
         Fit conformal regressor.
 
         Parameters
         ----------
         residuals : array-like of shape (n_values,), default=None
-            actual values - predicted values
+            true values - predicted values
         sigmas: array-like of shape (n_values,), default=None
             difficulty estimates
         bins : array-like of shape (n_values,), default=None
             Mondrian categories
 
         Returns
         -------
         self : object
             Fitted ConformalRegressor.
-        """
 
+        Examples
+        --------
+        Assuming that ``y_cal`` and ``y_hat_cal`` are vectors with true
+        and predicted targets for some calibration set, then a standard
+        conformal regressor can be formed from the residuals:
+
+        .. code-block:: python
+
+           residuals_cal = y_cal - y_hat_cal
+
+           from crepes import ConformalRegressor
+
+           cr_std = ConformalRegressor() 
+
+           cr_std.fit(residuals_cal) 
+
+        Assuming that ``sigmas_cal`` is a vector with difficulty estimates,
+        then a normalized conformal regressor can be fitted in the following
+        way:
+
+        .. code-block:: python
+
+           cr_norm = ConformalRegressor()
+           cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
+
+        Assuming that ``bins_cals`` is a vector with Mondrian categories 
+        (bin labels), then a Mondrian conformal regressor can be fitted in the
+        following way:
+
+        .. code-block:: python
+
+           cr_mond = ConformalRegressor()
+           cr_mond.fit(residuals=residuals_cal, bins=bins_cal)
+
+        A normalized Mondrian conformal regressor can be fitted in the 
+        following way:
+
+        .. code-block:: python
+
+           cr_norm_mond = ConformalRegressor()
+           cr_norm_mond.fit(residuals=residuals_cal, sigmas=sigmas_cal, 
+                            bins=bins_cal)
+        """
         tic = time.time()
         abs_residuals = np.abs(residuals)
         if bins is None:
             self.mondrian = False
             if sigmas is None:
                 self.normalized = False
                 self.alphas = np.sort(abs_residuals)[::-1]
@@ -110,25 +149,59 @@
             predicted values
         sigmas : array-like of shape (n_values,), default=None
             difficulty estimates
         bins : array-like of shape (n_values,), default=None
             Mondrian categories
         confidence : float in range (0,1), default=0.95
             confidence level
-        y_min : float or int, default=-np.inf
+        y_min : float or int, default=-numpy.inf
             minimum value to include in prediction intervals
-        y_max : float or int, default=np.inf
+        y_max : float or int, default=numpy.inf
             maximum value to include in prediction intervals
 
         Returns
         -------
         intervals : ndarray of shape (n_values, 2)
             prediction intervals
-        """
 
+        Examples
+        --------
+        Assuming that ``y_hat_test`` is a vector with predicted targets for a
+        test set and ``cr_std`` a fitted standard conformal regressor, then 
+        prediction intervals at the 99% confidence level can be obtained by:
+
+        .. code-block:: python
+
+           intervals = cr_std.predict(y_hat=y_hat_test, confidence=0.99)
+
+        Assuming that ``sigmas_test`` is a vector with difficulty estimates for
+        the test set and ``cr_norm`` a fitted normalized conformal regressor, 
+        then prediction intervals at the default (95%) confidence level can be
+        obtained by:
+
+        .. code-block:: python
+
+           intervals = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test)
+
+        Assuming that ``bins_test`` is a vector with Mondrian categories (bin 
+        labels) for the test set and ``cr_mond`` a fitted Mondrian conformal 
+        regressor, then the following provides prediction intervals at the 
+        default confidence level, where the intervals are lower-bounded by 0:
+
+        .. code-block:: python
+
+           intervals = cr_mond.predict(y_hat=y_hat_test, bins=bins_test, 
+                                       y_min=0)
+
+        Note
+        ----
+        In case the specified confidence level is too high in relation to the 
+        size of the calibration set, a warning will be issued and the output
+        intervals will be of maximum size.
+        """
         tic = time.time()
         intervals = np.zeros((len(y_hat),2))
         if not self.mondrian:
             alpha_index = int((1-confidence)*(len(self.alphas)+1))-1
             if alpha_index >= 0:
                 alpha = self.alphas[alpha_index]
                 if self.normalized:
@@ -136,25 +209,40 @@
                     intervals[:,1] = y_hat+alpha*sigmas
                 else:
                     intervals[:,0] = y_hat-alpha
                     intervals[:,1] = y_hat+alpha
             else:
                 intervals[:,0] = -np.inf 
                 intervals[:,1] = np.inf
-                # If the no. of calibration examples is too small for
-                # the chosen confidence level, then the intervals will
-                # be of maximum size
+                warnings.warn("the no. of calibration examples is too few" \
+                              "for the chosen confidence level; the " \
+                              "intervals will be of maximum size")
         else:           
             bin_values, bin_alphas = self.alphas
-            bin_indexes = [np.argwhere(bins == b).T[0] for b in bin_values]
-            alpha_indexes = [int((1-confidence)*(len(bin_alphas[b])+1))-1
-                             for b in range(len(bin_values))]
-            bin_alpha = [bin_alphas[b][alpha_indexes[b]]
+            bin_indexes = [np.argwhere(bins == b).T[0]
+                           for b in bin_values]
+            alpha_indexes = np.array(
+                [int((1-confidence)*(len(bin_alphas[b])+1))-1
+                 for b in range(len(bin_values))])
+            too_small_bins = np.argwhere(alpha_indexes < 0)
+            if len(too_small_bins) > 0:
+                if len(too_small_bins[:,0]) < 11:
+                    bins_to_show = " ".join([str(bin_values[i]) for i in
+                                             too_small_bins[:,0]])
+                else:
+                    bins_to_show = " ".join([str(bin_values[i]) for i in
+                                             too_small_bins[:10,0]]+['...'])
+                warnings.warn("the no. of calibration examples is too " \
+                              "small for the chosen confidence level " \
+                              f"in the following bins: {bins_to_show}; "\
+                              "the corresponding intervals will be of " \
+                              "maximum size") 
+            bin_alpha = np.array([bin_alphas[b][alpha_indexes[b]]
                          if alpha_indexes[b]>=0 else np.inf
-                         for b in range(len(bin_values))]
+                         for b in range(len(bin_values))])
             if self.normalized:
                 for b in range(len(bin_values)):
                     intervals[bin_indexes[b],0] = y_hat[bin_indexes[b]] \
                         - bin_alpha[b]*sigmas[bin_indexes[b]]
                     intervals[bin_indexes[b],1] = y_hat[bin_indexes[b]] \
                         + bin_alpha[b]*sigmas[bin_indexes[b]]
             else:
@@ -182,57 +270,70 @@
             predicted values
         sigmas : array-like of shape (n_values,), default=None
             difficulty estimates
         bins : array-like of shape (n_values,), default=None
             Mondrian categories
         confidence : float in range (0,1), default=0.95
             confidence level
-        y_min : float or int, default=-np.inf
+        y_min : float or int, default=-numpy.inf
             minimum value to include in prediction intervals
-        y_max : float or int, default=np.inf
+        y_max : float or int, default=numpy.inf
             maximum value to include in prediction intervals
         metrics : a string or a list of strings, 
                   default=list of all metrics, i.e., 
-                  ["error", "efficiency", "time_fit", "time_evaluate"]
+                  ["error", "eff_mean", "eff_med", "time_fit", "time_evaluate"]
         
         Returns
         -------
         results : dictionary with a key for each selected metric 
             estimated performance using the metrics
-        """
 
+        Examples
+        --------
+        Assuming that ``y_hat_test`` and ``y_test`` are vectors with predicted
+        and true targets for a test set, ``sigmas_test`` and ``bins_test`` are
+        vectors with difficulty estimates and Mondrian categories (bin labels) 
+        for the test set, and ``cr_norm_mond`` is a fitted normalized Mondrian
+        conformal regressor, then the latter can be evaluated at the default
+        confidence level with respect to error and mean efficiency (interval 
+        size) by:
+
+        .. code-block:: python
+
+           results = cr_norm_mond.evaluate(y_hat=y_hat_test, y=y_test, 
+                                           sigmas=sigmas_test, bins=bins_test,
+                                           metrics=["error", "eff_mean"])
+        """
         tic = time.time()
         if metrics is None:
-            metrics = ["error","efficiency","time_fit","time_evaluate"]
+            metrics = ["error","eff_mean","eff_med","time_fit","time_evaluate"]
         test_results = {}
         intervals = self.predict(y_hat, sigmas, bins, confidence, y_min, y_max)
         if "error" in metrics:
             test_results["error"] = 1-np.mean(
                 np.logical_and(intervals[:,0]<=y,y<=intervals[:,1]))
-        if "efficiency" in metrics:            
-            test_results["efficiency"] = np.mean(intervals[:,1]-intervals[:,0])
+        if "eff_mean" in metrics:            
+            test_results["eff_mean"] = np.mean(intervals[:,1]-intervals[:,0])
+        if "eff_med" in metrics:            
+            test_results["eff_med"] = np.median(intervals[:,1]-intervals[:,0])
         if "time_fit" in metrics:
             test_results["time_fit"] = self.time_fit
         toc = time.time()
         self.time_evaluate = toc-tic
         if "time_evaluate" in metrics:
             test_results["time_evaluate"] = self.time_evaluate
         return test_results
     
 class ConformalPredictiveSystem(ConformalPredictor):
     """
-    Conformal Predictive System.
-
     A conformal predictive system transforms point predictions 
-    (regression values) into cumulative distributions (conformal 
-    predictive distributions).
-    
+    (regression values) into cumulative distribution functions 
+    (conformal predictive distributions).
     """
     
-
     def __repr__(self):
         if self.fitted:
             return (f"ConformalPredictiveSystem(fitted={self.fitted}, "
                     f"normalized={self.normalized}, "
                     f"mondrian={self.mondrian})")
         else:
             return f"ConformalPredictiveSystem(fitted={self.fitted})"
@@ -250,14 +351,57 @@
         bins : array-like of shape (n_values,), default=None
             Mondrian categories
 
         Returns
         -------
         self : object
             Fitted ConformalPredictiveSystem.
+
+        Examples
+        --------
+        Assuming that ``y_cal`` and ``y_hat_cal`` are vectors with true and
+        predicted targets for some calibration set, then a standard conformal
+        predictive system can be formed from the residuals:
+
+        .. code-block:: python
+
+           residuals_cal = y_cal - y_hat_cal
+
+           from crepes import ConformalPredictiveSystem
+
+           cps_std = ConformalPredictiveSystem() 
+
+           cps_std.fit(residuals_cal) 
+
+        Assuming that ``sigmas_cal`` is a vector with difficulty estimates,
+        then a normalized conformal predictive system can be fitted in the 
+        following way:
+
+        .. code-block:: python
+
+           cps_norm = ConformalPredictiveSystem()
+           cps_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
+
+        Assuming that ``bins_cals`` is a vector with Mondrian categories (bin
+        labels), then a Mondrian conformal predictive system can be fitted in
+        the following way:
+
+        .. code-block:: python
+
+           cps_mond = ConformalPredictiveSystem()
+           cps_mond.fit(residuals=residuals_cal, bins=bins_cal)
+
+        A normalized Mondrian conformal predictive system can be fitted in the
+        following way:
+
+        .. code-block:: python
+
+           cps_norm_mond = ConformalPredictiveSystem()
+           cps_norm_mond.fit(residuals=residuals_cal, sigmas=sigmas_cal, 
+                             bins=bins_cal)
         """
 
         tic = time.time()
         if bins is None:
             self.mondrian = False
             if sigmas is None:
                 self.normalized = False
@@ -293,26 +437,26 @@
         y_hat : array-like of shape (n_values,), default=None
             predicted values
         sigmas : array-like of shape (n_values,), default=None
             difficulty estimates
         bins : array-like of shape (n_values,), default=None
             Mondrian categories
         y : float, int or array-like of shape (n_values,), default=None
-            values for which cumulative probabilities should be returned
+            values for which p-values should be returned
         lower_percentiles : array-like of shape (l_values,), default=None
             percentiles for which a lower value will be output 
             in case a percentile lies between two values
             (similar to `interpolation="lower"` in `numpy.percentile`)
         higher_percentiles : array-like of shape (h_values,), default=None
             percentiles for which a higher value will be output 
             in case a percentile lies between two values
             (similar to `interpolation="higher"` in `numpy.percentile`)
-        y_min : float or int, default=-np.inf
+        y_min : float or int, default=-numpy.inf
             The minimum value to include in prediction intervals.
-        y_max : float or int, default=np.inf
+        y_max : float or int, default=numpy.inf
             The maximum value to include in prediction intervals.
         return_cpds : Boolean, default=False
             specifies whether conformal predictive distributions (cpds)
             should be output or not
         cpds_by_bins : Boolean, default=False
             specifies whether the output cpds should be grouped by bin or not; 
             only applicable when bins is not None and return_cpds = True
@@ -332,14 +476,94 @@
             return_cpds == True. If bins is None, the distributions are
             represented by a single array, where the number of columns
             (c_values) is determined by the number of residuals of the fitted
             conformal predictive system. Otherwise, the distributions
             are represented by a vector of arrays, if cpds_by_bins = False,
             or a list of arrays, with one element for each bin, if 
             cpds_by_bins = True.
+
+        Examples
+        --------
+        Assuming that ``y_hat_test`` and ``y_test`` are vectors with predicted
+        and true targets, respectively, for a test set and ``cps_std`` a fitted
+        standard conformal predictive system, the p-values for the true targets 
+        can be obtained by:
+
+        .. code-block:: python
+
+           p_values = cps_std.predict(y_hat=y_hat_test, y=y_test)
+
+        The p-values with respect to some specific value, e.g., 37, can be
+        obtained by:
+
+        .. code-block:: python
+
+           p_values = cps_std.predict(y_hat=y_hat_test, y=37)
+
+        Assuming that ``sigmas_test`` is a vector with difficulty estimates for
+        the test set and ``cps_norm`` a fitted normalized conformal predictive 
+        system, then the 90th and 95th percentiles can be obtained by:
+
+        .. code-block:: python
+
+           percentiles = cps_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test,
+                                          higher_percentiles=[90,95])
+
+        In the above example, the nearest higher value is returned, if there is
+        no value that corresponds exactly to the requested percentile. If we
+        instead would like to retrieve the nearest lower value, we should 
+        write:
+
+        .. code-block:: python
+
+           percentiles = cps_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test,
+                                          lower_percentiles=[90,95])
+
+        Assuming that ``bins_test`` is a vector with Mondrian categories (bin 
+        labels) for the test set and ``cps_mond`` a fitted Mondrian conformal 
+        regressor, then the following returns prediction intervals at the 
+        95% confidence level, where the intervals are lower-bounded by 0:
+
+        .. code-block:: python
+
+           intervals = cps_mond.predict(y_hat=y_hat_test, bins=bins_test,
+                                        lower_percentiles=2.5,
+                                        higher_percentiles=97.5,
+                                        y_min=0)
+
+        If we would like to obtain the conformal distributions, we could write
+        the following:
+
+        .. code-block:: python
+
+           cpds = cps_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test,
+                                   return_cpds=True)
+
+        The output of the above will be an array with a row for each test
+        instance and a column for each calibration instance (residual).
+        For a Mondrian conformal predictive system, the above will instead
+        result in a vector, in which each element is a vector, as the number
+        of calibration instances may vary between categories. If we instead
+        would like an array for each category, this can be obtained by:
+
+        .. code-block:: python
+
+           cpds = cps_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test,
+                                   return_cpds=True, cpds_by_bins=True)
+
+        Note
+        ----
+        Setting ``cpds_by_bins`` has an effect only for Mondrian conformal 
+        predictive systems.
+
+        Note
+        ----
+        In case the calibration set is too small for the specified lower and
+        higher percentiles, a warning will be issued and the output will be 
+        ``y_min`` and ``y_max``, respectively.
         """
 
         tic = time.time()
         if not self.mondrian:
                 if self.normalized:
                     cpds = np.array([y_hat[i]+sigmas[i]*self.alphas
                                      for i in range(len(y_hat))])
@@ -354,30 +578,30 @@
                                   for i in bin_indexes[b]])
                         for b in range(len(bin_values))]
             else:
                 cpds = [np.array([y_hat[i]+bin_alphas[b] for
                                   i in bin_indexes[b]])
                         for b in range(len(bin_values))]
         no_prec_result_cols = 0
-        if type(lower_percentiles) in [int, float]:
+        if isinstance(lower_percentiles, (int, float, np.integer, np.floating)):
             lower_percentiles = [lower_percentiles]
-        if type(higher_percentiles) in [int, float]:
+        if isinstance(higher_percentiles, (int, float, np.integer, np.floating)):
             higher_percentiles = [higher_percentiles]
         if lower_percentiles is None:
             lower_percentiles = []
         if higher_percentiles is None:
             higher_percentiles = []
         no_result_columns = \
             (y is not None) + len(lower_percentiles) + len(higher_percentiles)
         if no_result_columns > 0:
             result = np.zeros((len(y_hat),no_result_columns))
         if y is not None:
             no_prec_result_cols += 1
             gammas = np.random.rand(len(y_hat))
-            if type(y) in [int, float]:
+            if isinstance(y, (int, float, np.integer, np.floating)):
                 if not self.mondrian:
                     result[:,0] = np.array([(len(np.argwhere(cpds[i]<y)) \
                                              + gammas[i])/(len(cpds[i])+1)
                                             for i in range(len(cpds))])
                 else:
                     for b in range(len(bin_values)):
                         result[bin_indexes[b],0] = np.array(
@@ -399,36 +623,63 @@
                                       for i in range(len(cpds[b]))])
             else:
                 raise ValueError(("y must either be a single int, float or"
                                   "a list/numpy array of the same length as "
                                   "the residuals"))
         if len(lower_percentiles) > 0:
                 if not self.mondrian:
-                    lower_indexes = [int(lower_percentile/100 \
+                    lower_indexes = np.array([int(lower_percentile/100 \
                                          * (len(self.alphas)+1))-1
-                                     for lower_percentile in lower_percentiles]
+                                     for lower_percentile in lower_percentiles])
+                    too_low_indexes = np.argwhere(lower_indexes < 0)
+                    if len(too_low_indexes) > 0:
+                        lower_indexes[too_low_indexes[:,0]] = 0
                     result[:,no_prec_result_cols:no_prec_result_cols \
                            + len(lower_percentiles)] = cpds[:,lower_indexes]
-                    y_min_columns = [no_prec_result_cols+i
-                                     for i in range(len(lower_indexes))
-                                     if lower_indexes[i]<0]
-                    result[:,y_min_columns] = y_min
+                    if len(too_low_indexes) > 0:
+                        percentiles_to_show = " ".join([
+                            str(lower_percentiles[i])
+                            for i in too_low_indexes[:,0]])
+                        warnings.warn("the no. of calibration examples is " \
+                                      "too few for the following lower " \
+                                      f"percentiles: {percentiles_to_show}; "\
+                                      "the corresponding values are " \
+                                      "set to y_min")
+                        y_min_columns = [no_prec_result_cols+i
+                                         for i in too_low_indexes[:,0]]
+                        result[:,y_min_columns] = y_min
                 else:
+                    too_small_bins = []
                     for b in range(len(bin_values)):
-                        lower_indexes = [int(lower_percentile/100 \
+                        lower_indexes = np.array([int(lower_percentile/100 \
                                              * (len(bin_alphas[b])+1))-1
                                          for lower_percentile
-                                         in lower_percentiles]                
+                                         in lower_percentiles])
+                        too_low_indexes = np.argwhere(lower_indexes < 0)
+                        if len(too_low_indexes) > 0:
+                            lower_indexes[too_low_indexes[:,0]] = 0
+                            too_small_bins.append(str(bin_values[b]))                            
                         result[bin_indexes[b],
                                no_prec_result_cols:no_prec_result_cols \
                                + len(lower_indexes)] = cpds[b][:,lower_indexes]
-                    y_min_columns = [no_prec_result_cols+i
-                                     for i in range(len(lower_indexes))
-                                     if lower_indexes[i]<0]
-                    result[:,y_min_columns] = y_min                    
+                        if len(too_low_indexes) > 0:
+                            for i in too_low_indexes[:,0]:
+                                result[bin_indexes[b],no_prec_result_cols+i] = y_min
+                    if len(too_small_bins) > 0:
+                        if len(too_small_bins) < 11:
+                            bins_to_show = " ".join(too_small_bins)
+                        else:
+                            bins_to_show = " ".join(
+                                too_small_bins[:10]+['...'])
+                        warnings.warn("the no. of calibration examples is " \
+                                      "too few for some lower percentile" \
+                                      "in the following bins:" \
+                                      f"{bins_to_show}; "\
+                                      "the corresponding values are " \
+                                      "set to y_min")
         if y_min > -np.inf:
             result[:,
                    no_prec_result_cols:no_prec_result_cols \
                    + len(lower_percentiles)]\
                    [result[:,no_prec_result_cols:no_prec_result_cols \
                            + len(lower_percentiles)]<y_min] = y_min
         no_prec_result_cols += len(lower_percentiles)
@@ -438,28 +689,58 @@
                         [int(np.ceil(higher_percentile/100 \
                                      * (len(self.alphas)+1)))-1
                          for higher_percentile in higher_percentiles],
                         dtype=int)
                     too_high_indexes = np.array(
                         [i for i in range(len(higher_indexes))
                          if higher_indexes[i] > len(self.alphas)-1], dtype=int)
+                    if len(too_high_indexes) > 0:
+                        percentiles_to_show = " ".join(
+                            [str(higher_percentiles[i])
+                             for i in too_high_indexes])
+                        warnings.warn("the no. of calibration examples is " \
+                                      "too few for the following higher " \
+                                      f"percentiles: {percentiles_to_show}; "\
+                                      "the corresponding values are " \
+                                      "set to y_max") 
                     higher_indexes[too_high_indexes] = len(self.alphas)-1
                     result[:,no_prec_result_cols:no_prec_result_cols \
                            + len(higher_indexes)] = cpds[:,higher_indexes]
                     result[:,no_prec_result_cols+too_high_indexes] = y_max
                 else:
+                    too_small_bins = []
                     for b in range(len(bin_values)):
-                        higher_indexes = [
+                        higher_indexes = np.array([
                             int(np.ceil(higher_percentile/100 \
                                         * (len(bin_alphas[b])+1)))-1
-                            for higher_percentile in higher_percentiles]
+                            for higher_percentile in higher_percentiles])
+                        too_high_indexes = np.array(
+                            [i for i in range(len(higher_indexes))
+                             if higher_indexes[i] > len(bin_alphas[b])-1], dtype=int)
+                        if len(too_high_indexes) > 0:
+                            higher_indexes[too_high_indexes] = -1
+                            too_small_bins.append(str(bin_values[b]))                            
                         result[bin_indexes[b],
                                no_prec_result_cols:no_prec_result_cols \
-                               + len(higher_indexes)] = cpds[b]\
-                                   [:,higher_indexes]
+                               + len(higher_indexes)] = cpds[b][:,higher_indexes]
+                        if len(too_high_indexes) > 0:
+                            for i in too_high_indexes:
+                                result[bin_indexes[b],no_prec_result_cols+i] = y_max
+                    if len(too_small_bins) > 0:
+                        if len(too_small_bins) < 11:
+                            bins_to_show = " ".join(too_small_bins)
+                        else:
+                            bins_to_show = " ".join(
+                                too_small_bins[:10]+['...'])
+                        warnings.warn("the no. of calibration examples is " \
+                                      "too few for some higher percentile" \
+                                      "in the following bins:" \
+                                      f"{bins_to_show}; "\
+                                      "the corresponding values are " \
+                                      "set to y_max")
         if y_max < np.inf:
             result[:,no_prec_result_cols:no_prec_result_cols\
                    + len(higher_percentiles)]\
                    [result[:,no_prec_result_cols:no_prec_result_cols \
                            + len(higher_percentiles)]>y_max] = y_max
         toc = time.time()
         self.time_predict = toc-tic            
@@ -497,31 +778,50 @@
             correct target values
         sigmas : array-like of shape (n_values,), default=None,
             difficulty estimates
         bins : array-like of shape (n_values,), default=None,
             Mondrian categories
         confidence : float in range (0,1), default=0.95
             confidence level
-        y_min : float or int, default=-np.inf
+        y_min : float or int, default=-numpy.inf
             minimum value to include in prediction intervals
-        y_max : float or int, default=np.inf
+        y_max : float or int, default=numpy.inf
             maximum value to include in prediction intervals
         metrics : a string or a list of strings, default=list of all 
-            metrics; ["error", "efficiency", "CRPS", "time_fit", 
+            metrics; ["error", "eff_mean","eff_med", "CRPS", "time_fit",
                       "time_evaluate"]
         
         Returns
         -------
         results : dictionary with a key for each selected metric 
             estimated performance using the metrics
+
+        Examples
+        --------
+        Assuming that ``y_hat_test`` and ``y_test`` are vectors with predicted
+        and true targets for a test set, ``sigmas_test`` and ``bins_test`` are
+        vectors with difficulty estimates and Mondrian categories (bin labels) 
+        for the test set, and ``cps_norm_mond`` is a fitted normalized Mondrian
+        conformal predictive system, then the latter can be evaluated at the 
+        default confidence level with respect to error, mean and median 
+        efficiency (interval size, given the default confidence level) and 
+        continuous-ranked probability score (CRPS) by:
+
+        .. code-block:: python
+
+           results = cps_norm_mond.evaluate(y_hat=y_hat_test, y=y_test, 
+                                            sigmas=sigmas_test, bins=bins_test,
+                                            metrics=["error", "eff_mean", 
+                                                     "eff_med", "CRPS"])
         """
 
         tic = time.time()
         if metrics is None:
-            metrics = ["error","efficiency","CRPS","time_fit","time_evaluate"]
+            metrics = ["error","eff_mean","eff_med","CRPS","time_fit",
+                       "time_evaluate"]
         lower_percentile = (1-confidence)/2*100
         higher_percentile = (confidence+(1-confidence)/2)*100
         test_results = {}
         if "CRPS" in metrics:
             results, cpds = self.predict(y_hat, sigmas=sigmas, bins=bins, y=y,
                                          lower_percentiles=lower_percentile,
                                          higher_percentiles=higher_percentile,
@@ -557,16 +857,18 @@
                                      lower_percentiles=lower_percentile,
                                      higher_percentiles=higher_percentile,
                                      y_min=y_min, y_max=y_max,
                                      return_CRPS=False)
         if "error" in metrics:
             test_results["error"] = 1-np.mean(np.logical_and(
                 intervals[:,0]<=y,y<=intervals[:,1]))
-        if "efficiency" in metrics:            
-            test_results["efficiency"] = np.mean(intervals[:,1]-intervals[:,0])
+        if "eff_mean" in metrics:            
+            test_results["eff_mean"] = np.mean(intervals[:,1]-intervals[:,0])
+        if "eff_med" in metrics:            
+            test_results["eff_med"] = np.median(intervals[:,1]-intervals[:,0])
         if "CRPS" in metrics:
             test_results["CRPS"] = crps
         if "time_fit" in metrics:
             test_results["time_fit"] = self.time_fit
         toc = time.time()
         self.time_evaluate = toc-tic
         if "time_evaluate" in metrics:
```

### Comparing `crepes-0.1.0/src/crepes.egg-info/PKG-INFO` & `crepes-0.2.0/src/crepes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.1.0
+Version: 0.2.0
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `crepes`: Conformal Regressors and Predictive Systems
+# `crepes`
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
 The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
 
 ## Installation
 
-Install with: `pip install crepes`
+Install with:
 
-## Quick start
+```bash
+pip install crepes
+```
+
+## Documentation
+
+For complete documentation of the `crepes` package, see [here](https://crepes.readthedocs.io/en/latest/).
+
+## Quickstart
 
 ### Conformal regressors
 
 We first import the main class and two helper functions:
 
 ```python
 from crepes import ConformalRegressor
 from crepes.fillings import sigma_knn, binning
 ```
 
-We will illustrate the above using a dataset from www.openml.org and a `RandomForestRegressor` from `sklearn`:
+We will illustrate the above using a dataset from [www.openml.org](https://www.openml.org) and a `RandomForestRegressor` from [sklearn](https://scikit-learn.org):
 
 ```python
 from sklearn.datasets import fetch_openml
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestRegressor
 
 dataset = fetch_openml(name="house_sales", version=3)
@@ -71,81 +79,81 @@
 ```
 
 We can now apply the conformal regressor to get prediction intervals for the test objects, using the point predictions as input, where the probability of not including the correct target in an interval is 1-confidence:
 ```python
 std_intervals = cr_std.predict(y_hat=y_hat_test, confidence=0.99)
 ```
 
-The output is a NumPy array, specifying the lower and upper bound of each interval:
+The output is a [NumPy](https://numpy.org) array, specifying the lower and upper bound of each interval:
 
 ```numpy
-array([[-353379.  ,  939231.  ],
-       [-251874.3 , 1040735.7 ],
-       [-138329.5 , 1154280.5 ],
+array([[-171902.2 ,  953866.2 ],
+       [-276818.01,  848950.39],
+       [  22679.37, 1148447.77],
        ...,
-       [-389128.68,  903481.32],
-       [-313003.  ,  979607.  ],
-       [ -90551.53, 1202058.47]])
+       [ 242954.02, 1368722.42],
+       [-308093.73,  817674.67],
+       [-227057.4 ,  898711.  ]])
 ```
 
 We may request that the intervals are cut to exclude impossible values, in this case below 0, and if we also rely on the default confidence level (0.95), the output intervals will be a bit tighter:
 
 ```python
 intervals_std = cr_std.predict(y_hat=y_hat_test, y_min=0)
 ```
 
 ```numpy
-array([[  7576.18, 578275.82],
-       [109080.88, 679780.52],
-       [222625.68, 793325.32],
+array([[ 152258.55,  629705.45],
+       [  47342.74,  524789.64],
+       [ 346840.12,  824287.02],
        ...,
-       [     0.  , 542526.14],
-       [ 47952.18, 618651.82],
-       [270403.65, 841103.29]])
+       [ 567114.77, 1044561.67],
+       [  16067.02,  493513.92],
+       [  97103.35,  574550.25]])
 ```
 
 The above intervals are not normalized, i.e., they are all of the same size (at least before they are cut). We could make the intervals more informative through normalization using difficulty estimates; more difficult instances will be assigned wider intervals.
 
-We will here use the helper function `sigma_knn` for this purpose. It estimates the difficulty by the mean absolute errors of the k (default `k=5`) nearest neighbors to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through a (named) argument to the function; below we just use the default, i.e., `beta=0.01`.
+We will use the helper function `sigma_knn` for this purpose. Here it estimates the difficulty by the standard deviation of the target of the k (default `k=25`) nearest neighbors in the proper training set to each instance in the calibration set. A small value (beta) is added to the estimates, which may be given through an argument to the function; below we just use the default, i.e., `beta=0.01`.
 
 ```python
-sigmas_cal = sigma_knn(X=X_cal, residuals=residuals_cal)
+sigmas_cal = sigma_knn(X=X_cal, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 The difficulty estimates and residuals of the calibration examples can now be used to form a normalized conformal regressor:
 
 ```python
 cr_norm = ConformalRegressor()
 cr_norm.fit(residuals=residuals_cal, sigmas=sigmas_cal)
 ```
 
-To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the calibration objects and residuals. 
+To generate prediction intervals for the test set using the normalized conformal regressor, we need difficulty estimates for the test set too, which we get using the same helper function. 
 
 ```python
-sigmas_test = sigma_knn(X=X_cal, residuals=residuals_cal, X_test=X_test)
+sigmas_test = sigma_knn(X=X_test, X_ref=X_prop_train, y_ref=y_prop_train)
 ```
 
 Now we can obtain the prediction intervals, using the point predictions and difficulty estimates for the test set:
 
 ```python
 intervals_norm = cr_norm.predict(y_hat=y_hat_test, sigmas=sigmas_test, 
                                  y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 645527.3140099 ],
-       [100552.5573358 , 688308.8426642 ],
-       [206605.7263972 , 809345.2736028 ],
+array([[205959.07517616, 576004.92482384],
+       [133206.86035366, 438925.51964634],
+       [291925.81345507, 879201.32654493],
        ...,
-       [ 55388.60029434, 458964.03970566],
-       [252094.62400964, 414509.37599036],
-       [305546.225071  , 805960.714929  ]])
+       [622212.95112744, 989463.48887256],
+       [ 98805.77755066, 410775.16244934],
+       [197248.38670265, 474405.21329735]])
 ```
 
-Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no informatoion on the expected error should instead lead to more uniformly distributed interval sizes.
+Depending on the employed difficulty estimator, the normalized intervals may sometimes be unreasonably large, in the sense that they may be several times larger than any previously observed error. Moreover, if the difficulty estimator is not very informative, e.g., completely random, the varying interval sizes may give a false impression of that we can expect lower prediction errors for instances with tighter intervals. Ideally, a difficulty estimator providing little or no information on the expected error should instead lead to more uniformly distributed interval sizes.
 
 A Mondrian conformal regressor can be used to address these problems, by dividing the object space into non-overlapping so-called Mondrian categories, and forming a (standard) conformal regressor for each category. The category membership of the objects can be provided as an additional argument, named `bins`, for the `fit` method.
 
 Here we will use the helper function `binning` to form Mondrian categories by equal-sized binning of the difficulty estimates; the function will return labels for the calibration objects as well as thresholds for the bins, which are later to be used when binning the test objects:
 
 ```python
 bins_cal, bin_thresholds = binning(values=sigmas_cal, bins=20)
@@ -167,21 +175,21 @@
 Now we have everything we need to get the prediction intervals:
 
 ```python
 intervals_mond = cr_mond.predict(y_hat=y_hat_test, bins=bins_test, y_min=0)
 ```
 
 ```numpy
-array([[     0.  , 592782.5 ],
-       [146648.15, 642213.25],
-       [260192.95, 755758.05],
+array([[ 206379.7 ,  575584.3 ],
+       [ 144014.65,  428117.73],
+       [  17965.57, 1153161.57],
        ...,
-       [ 38332.66, 476019.98],
-       [198148.5 , 468455.5 ],
-       [329931.17, 781575.77]])
+       [ 653865.22,  957811.22],
+       [ 174264.87,  335316.07],
+       [ 140587.46,  531066.14]])
 ```
 
 ### Conformal predictive systems
 
 The interface to a `ConformalPredictiveSystem` is very similar to that of a conformal regressor; by providing just the residuals, we get a standard conformal predictive system, by providing also difficulty estimates, we get a normalized conformal predictive system and by providing labels for Mondrian categories (bins), we get a Mondrian conformal predictive system.
 
 The main difference to conformal regressors concerns the output; instead of prediction intervals, conformal predictive systems produce complete cumulative distribution functions (conformal predictive distributions). From these we can generate prediction intervals, but we can also obtain calibrated point predictions, as well as p values for given target values.
@@ -212,70 +220,64 @@
                                   bins=bins_test,
                                   lower_percentiles=2.5,
                                   higher_percentiles=97.5,
                                   y_min=0)
 ```
 
 ```numpy
-array([[     0.        , 537757.93618585],
-       [177348.62535049, 655015.98985999],
-       [253618.31669927, 783707.98804461],
+array([[ 226536.76784152,  519404.56955659],
+       [ 170043.51497485,  376524.37491457],
+       [ 192376.08061079,  994115.461665  ],
        ...,
-       [ 73466.09003216, 397289.46238233],
-       [273315.68901744, 405309.55870912],
-       [274035.55188125, 789701.43635318]])
+       [ 594183.11971763, 1010273.54816378],
+       [ 186478.52365968,  308050.53035102],
+       [ 167498.01540504,  485813.1329371 ]])
 ```
 
 We can also get the p values for the true target values; they should be uniformly distributed, if the test objects are drawn from the same underlying distribution as the calibration examples.
 
 ```python
 p_values = cps_mond_norm.predict(y_hat=y_hat_test,
                                  sigmas=sigmas_test,
                                  bins=bins_test,
                                  y=y_test)
 ```
 
 ```numpy
-array([[0.3262945 ],
-       [0.12184386],
-       [0.82948135],
+array([[0.98298087],
+       [0.90125379],
+       [0.41770673],
        ...,
-       [0.75042278],
-       [0.61815831],
-       [0.70252814]])
+       [0.04659288],
+       [0.07914733],
+       [0.31090332]])
 ```
 
 We may request that the predict method returns the full conformal predictive distribution (CPD) for each test instance, as defined by the threshold values, by setting `return_cpds=True`. The format of the distributions vary with the type of conformal predictive system; for a standard and normalized CPS, the output is an array with a row for each test instance and a column for each calibration instance (residual), while for a Mondrian CPS, the default output is a vector containing one CPD per test instance, since the number of values may vary between categories.
 
 ```python
 cpds = cps_mond_norm.predict(y_hat=y_hat_test,
                              sigmas=sigmas_test,
                              bins=bins_test,
                              return_cpds=True)
 ```
 
 The resulting vector of arrays is not displayed here, but we instead provide a plot for the CPD of a random test instance:
 
-![cpd](https://user-images.githubusercontent.com/7838741/176182669-1cb739dc-dc38-4c30-80b1-624c2f6b4b83.png)
+![cpd](https://user-images.githubusercontent.com/7838741/235081969-328d7a23-26c9-4799-a246-8c35fd7ac88e.png)
 
 ## Examples
 
-For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/crepes.ipynb).
-
-## Documentation
-
-For documentation of the `crepes` package, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.html).
-
-For documentation of the `crepes.fillings` module, see [here](http://htmlpreview.github.io/?https://github.com/henrikbostrom/crepes/blob/main/docs/crepes.fillings.html).
+For additional examples of how to use the package and module, including how to use out-of-bag predictions rather than having to rely on dividing the training set into a proper training and calibration set, see [the documentation](https://crepes.readthedocs.io/en/latest/) and [this Jupyter notebook](https://github.com/henrikbostrom/crepes/blob/main/docs/crepes_nb.ipynb).
 
 ## Citing crepes
 
 If you use `crepes` for a scientific publication, you may cite the following paper:
 
-Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179.
+Boström, H., 2022. crepes: a Python Package for Generating Conformal Regressors and Predictive Systems. In Conformal and Probabilistic Prediction and Applications. PMLR, 179. [Link](https://copa-conference.com/papers/COPA2022_paper_11.pdf)
 
 Bibtex entry:
 
 ```bibtex
 @InProceedings{crepes,
   title = 	 {crepes: a Python Package for Generating Conformal Regressors and Predictive Systems},
   author =       {Bostr\"om, Henrik},
@@ -300,12 +302,15 @@
 
 <a id="5">[5]</a> Boström, H. and Johansson, U., 2020. Mondrian conformal regressors. In Conformal and Probabilistic Prediction and Applications. PMLR, 128, pp. 114-133. [Link](https://proceedings.mlr.press/v128/bostrom20a.html)
 
 <a id="6">[6]</a> Vovk, V., Petej, I., Nouretdinov, I., Manokhin, V. and Gammerman, A., 2020. Computationally efficient versions of conformal predictive distributions. Neurocomputing, 397, pp.292-308. [Link](https://www.aminer.org/pub/5e09aac9df1a9c0c416c9b70/computationally-efficient-versions-of-conformal-predictive-distributions)
 
 <a id="7">[7]</a> Boström, H., Johansson, U. and Löfström, T., 2021. Mondrian conformal predictive distributions. In Conformal and Probabilistic Prediction and Applications. PMLR, 152, pp. 24-38. [Link](https://proceedings.mlr.press/v152/bostrom21a.html)
 
+<a id="8">[8]</a> Vovk, V., 2022. Universal predictive systems. Pattern Recognition. 126: pp. 108536 [Link](https://dl.acm.org/doi/abs/10.1016/j.patcog.2022.108536)
+
+
 - - -
 
 Author: Henrik Boström (bostromh@kth.se)
-Copyright 2022 Henrik Boström
+Copyright 2023 Henrik Boström
 License: BSD 3 clause
```

