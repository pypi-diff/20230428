# Comparing `tmp/linearmodels-4.8.tar.gz` & `tmp/linearmodels-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linearmodels-4.8.tar", last modified: Fri May 18 12:37:07 2018, max compression
+gzip compressed data, was "dist/linearmodels-4.9.tar", last modified: Wed Aug 29 15:12:30 2018, max compression
```

## Comparing `linearmodels-4.8.tar` & `linearmodels-4.9.tar`

### file list

```diff
@@ -1,256 +1,262 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5902 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6589 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/iv_using-formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    18212 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/iv_advanced-examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22351 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/iv_basic-examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8798 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_three-stage-ls.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35002 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_correct-greene-table-10-1.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    17212 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_correct-greene-table-10-2.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5945 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/panel_using-formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15372 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/panel_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12515 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/asset-pricing_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    24856 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5084 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/asset-pricing_formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8244 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/panel_data-formats.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    31657 2018-05-18 12:29:16.000000 linearmodels-4.8/examples/system_correct-greene-table-10-3.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4739 2018-05-18 12:29:16.000000 linearmodels-4.8/README.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4264 2018-05-18 12:29:16.000000 linearmodels-4.8/README.md
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      928 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/formula.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/compat/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1256 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/compat/pandas.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/compat/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      375 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/compat/numpy.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      469 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/compat/statsmodels.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/panel/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    20319 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/panel/data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      297 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/panel/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    26812 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/panel/results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    20637 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/panel/covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    76850 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/panel/model.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/birthweight/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      962 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/birthweight/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/jobtraining/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1635 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/jobtraining/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/french/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1353 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/french/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      221 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/meps/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1042 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/meps/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/mroz/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1032 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/mroz/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/munnell/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      517 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/munnell/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/wage_panel/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      789 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/wage_panel/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/fertility/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1025 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/fertility/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/fringe/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2042 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/fringe/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/wage/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1022 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/wage/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/datasets/card/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1991 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/datasets/card/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/iv/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13520 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/gmm.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5666 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      112 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    48114 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5100 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    18872 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    40903 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/iv/model.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2150 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      495 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/_version.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      621 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/conftest.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/system/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9612 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/gmm.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      107 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    19565 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8459 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    16715 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    62975 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/system/model.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5257 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/test_utility.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/panel/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4551 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_simulated_against_stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5929 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_panel_covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5432 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    26678 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7952 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_formula.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    11113 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_between_ols.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2608 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_random_effects.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5849 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_model.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3375 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_fama_macbeth.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7401 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_pooled_ols.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6760 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_firstdifference_ols.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4863 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_cluster_input_formats.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    40265 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_panel_ols.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/panel/results/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1957 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/parse_stata_results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1508 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/generate-panel-data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    65624 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/stata-panel-simulated-results.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)   578091 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/simulated-panel.dta
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3504 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/results/execute-stata-simulated-data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5458 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/panel/test_results.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/datasets/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/datasets/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      598 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/datasets/test_datasets.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1441 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/test_examples.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/iv/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10592 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_gmm.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7661 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_against_stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12050 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1349 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8419 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2783 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_missing_data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10682 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_model.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8553 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_formulas.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4505 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_postestimation.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/iv/results/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13232 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/stata-iv-housing-results.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2533 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/execute-stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    97696 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/simulated-data.dta
--rw-r--r--   0 kevin     (1000) kevin     (1000)   547258 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/stata-iv-simulated-results.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3331 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/read_stata_results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2170 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/simulated-test-data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4111 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/execute-stata-simulated-data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5777 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/results/housing.csv
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2946 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/iv/test_results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/system/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5691 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13629 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_gmm.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2471 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_3sls_against_stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4888 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_sur_against_stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9273 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_3sls.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9841 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12313 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5409 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_formulas.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1618 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_equivalence.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22521 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/test_sur.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/system/results/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2636 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/parse_stata_3sls_results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3607 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/execute-stata.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3350 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/parse_stata_results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    55085 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/simulated-sur.dta
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2618 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/execute-stata-3sls.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1558 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/generate_data.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    32162 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/stata-sur-results.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)    50504 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/simulated-3sls.dta
--rw-r--r--   0 kevin     (1000) kevin     (1000)    85208 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/system/results/stata-3sls-results.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2023 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/test_covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1557 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/_utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7205 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/test_model.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3133 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/test_formulas.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3240 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    11627 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/tests/asset_pricing/test_linear_factor_model.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels/asset_pricing/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      188 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/asset_pricing/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9238 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/asset_pricing/results.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9222 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/asset_pricing/covariance.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    34468 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/asset_pricing/model.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    16073 2018-05-18 12:29:16.000000 linearmodels-4.8/linearmodels/utility.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)       61 2018-05-18 12:29:16.000000 linearmodels-4.8/requirements.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4098 2018-05-18 12:29:16.000000 linearmodels-4.8/setup.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6941 2018-05-18 12:37:07.000000 linearmodels-4.8/PKG-INFO
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/panel/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      394 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/convert-lyx.cmd
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9282 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/mathematical-detail.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/panel/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8244 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/panel/examples/data-formats.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5945 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/panel/examples/using-formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15372 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/panel/examples/examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1209 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/covariance.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    15701 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/mathematical-detail.lyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7696 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/pandas.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      651 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/results.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1417 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/faq.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      233 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/data.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)       71 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/mathematical-formula.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1578 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/index.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5721 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/introduction.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      749 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/models.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      162 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/panel/reference.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/iv/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      291 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/convert-lyx.cmd
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/iv/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6589 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/iv/examples/using-formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22351 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/iv/examples/basic-examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    18212 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/iv/examples/advanced-examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)      742 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/covariance.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      473 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/results.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      390 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/methods.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      252 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/mathematical-formula.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    34614 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/estimators.lyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1190 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/index.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8668 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/introduction.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      533 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/gmm.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      157 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/reference.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    21745 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/iv/estimators.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      744 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/contributing.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      422 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/convert-lyx.cmd
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13225 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/mathematical-detail.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5902 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    24856 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    35002 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-1.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)    17212 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-2.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8798 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/three-stage-ls.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    31657 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-3.png
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1450 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/covariance.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      371 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/gmm-weights.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    21447 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/mathematical-detail.lyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)      414 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/results.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      161 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/mathematical-formula.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3828 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/index.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      629 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/models.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      176 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/system/reference.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     7267 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/conf.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2015 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/plan.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/_templates/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      213 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/_templates/layout.html
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2253 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/index.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      240 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/utility.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1409 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/changes.rst
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/_static/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/_static/css/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1323 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/_static/css/overrides.css
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/asset-pricing/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      422 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/convert-lyx.cmd
--rw-r--r--   0 kevin     (1000) kevin     (1000)     8882 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/mathematical-detail.txt
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/asset-pricing/examples/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5084 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/asset-pricing/examples/formulas.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12515 2018-05-18 12:37:07.000000 linearmodels-4.8/doc/source/asset-pricing/examples/examples.ipynb
--rw-r--r--   0 kevin     (1000) kevin     (1000)      585 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/covariance.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)    22515 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/mathematical-detail.lyx
--rw-r--r--   0 kevin     (1000) kevin     (1000)      255 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/results.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      173 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/mathematical-formula.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2689 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/index.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3610 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/introduction.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      655 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/models.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      161 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/asset-pricing/reference.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2063 2018-05-18 12:29:16.000000 linearmodels-4.8/doc/source/references.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      399 2018-05-18 12:29:16.000000 linearmodels-4.8/MANIFEST.in
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)       60 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6941 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12677 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2018-05-18 12:35:28.000000 linearmodels-4.8/linearmodels.egg-info/not-zip-safe
--rw-r--r--   0 kevin     (1000) kevin     (1000)       13 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/top_level.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2018-05-18 12:37:07.000000 linearmodels-4.8/linearmodels.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      276 2018-05-18 12:37:07.000000 linearmodels-4.8/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)      171 2018-05-18 12:29:16.000000 linearmodels-4.8/requirements-dev.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)    68611 2018-05-18 12:29:16.000000 linearmodels-4.8/versioneer.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/_templates/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      213 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/_templates/layout.html
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/iv/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8666 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/introduction.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      252 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/mathematical-formula.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/iv/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    22354 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/iv/examples/basic-examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6589 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/iv/examples/using-formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    18211 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/iv/examples/advanced-examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      390 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/methods.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      291 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/convert-lyx.cmd
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      533 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/gmm.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      742 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/covariance.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    34612 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/estimators.lyx
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      473 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/results.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1190 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/index.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      157 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/reference.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    21743 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/iv/estimators.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2197 2018-08-29 15:06:48.000000 linearmodels-4.9/doc/source/plan.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      744 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/contributing.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1957 2018-08-29 15:06:48.000000 linearmodels-4.9/doc/source/changes.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/asset-pricing/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3610 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/introduction.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      173 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/mathematical-formula.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      655 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/models.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8882 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/mathematical-detail.txt
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/asset-pricing/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5084 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/asset-pricing/examples/formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12516 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/asset-pricing/examples/examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      422 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/convert-lyx.cmd
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    22515 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/mathematical-detail.lyx
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      585 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/covariance.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      255 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/results.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2689 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/index.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      161 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/asset-pricing/reference.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/_static/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/_static/css/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1323 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/_static/css/overrides.css
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1024 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/spelling_wordlist.txt
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/panel/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5721 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/introduction.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       71 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/mathematical-formula.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      749 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/models.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7696 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/pandas.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1418 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/faq.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9282 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/mathematical-detail.txt
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/panel/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5945 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/panel/examples/using-formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    15374 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/panel/examples/examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8240 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/panel/examples/data-formats.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      394 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/convert-lyx.cmd
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    15701 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/mathematical-detail.lyx
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1209 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/covariance.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      651 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/results.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1578 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/index.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      162 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/reference.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      233 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/panel/data.rst
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/system/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      161 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/mathematical-formula.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      629 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/models.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13225 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/mathematical-detail.txt
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/doc/source/system/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5896 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    35002 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-1.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    24895 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    31657 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-3.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17212 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-2.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8799 2018-08-29 15:12:29.000000 linearmodels-4.9/doc/source/system/examples/three-stage-ls.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      422 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/convert-lyx.cmd
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    21447 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/mathematical-detail.lyx
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1452 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/covariance.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      414 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/results.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3828 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/index.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      371 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/gmm-weights.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      176 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/system/reference.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7518 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/conf.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2253 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/index.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      240 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/utility.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      262 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/names_wordlist.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2063 2018-08-29 14:53:32.000000 linearmodels-4.9/doc/source/references.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       61 2018-08-29 14:53:32.000000 linearmodels-4.9/requirements.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      276 2018-08-29 15:12:30.000000 linearmodels-4.9/setup.cfg
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels.egg-info/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       60 2018-08-29 15:12:29.000000 linearmodels-4.9/linearmodels.egg-info/requires.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2018-08-29 15:12:29.000000 linearmodels-4.9/linearmodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2018-08-29 15:12:29.000000 linearmodels-4.9/linearmodels.egg-info/not-zip-safe
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7459 2018-08-29 15:12:29.000000 linearmodels-4.9/linearmodels.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       13 2018-08-29 15:12:29.000000 linearmodels-4.9/linearmodels.egg-info/top_level.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12930 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels.egg-info/SOURCES.txt
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/examples/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5896 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8799 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_three-stage-ls.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5945 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/panel_using-formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    35002 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_correct-greene-table-10-1.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6589 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/iv_using-formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    22354 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/iv_basic-examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    24895 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    15374 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/panel_examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    31657 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_correct-greene-table-10-3.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8240 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/panel_data-formats.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    18211 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/iv_advanced-examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17212 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/system_correct-greene-table-10-2.png
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5084 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/asset-pricing_formulas.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12516 2018-08-29 14:53:32.000000 linearmodels-4.9/examples/asset-pricing_examples.ipynb
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5215 2018-08-29 15:06:48.000000 linearmodels-4.9/README.rst
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      171 2018-08-29 14:53:32.000000 linearmodels-4.9/requirements-dev.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7459 2018-08-29 15:12:30.000000 linearmodels-4.9/PKG-INFO
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4680 2018-08-29 15:06:48.000000 linearmodels-4.9/README.md
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4098 2018-08-29 14:53:32.000000 linearmodels-4.9/setup.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      399 2018-08-29 14:53:32.000000 linearmodels-4.9/MANIFEST.in
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/iv/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    42331 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    48559 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5100 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    18877 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6091 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/iv/data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      112 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13537 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/iv/gmm.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      621 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/conftest.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      928 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/formula.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/typing/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      349 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/typing/iv.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       96 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/typing/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/asset_pricing/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    34466 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/asset_pricing/model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9437 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/asset_pricing/results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9222 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/asset_pricing/covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      188 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/asset_pricing/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/iv/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2783 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_missing_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7661 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_against_stata.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12050 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4505 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_postestimation.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1349 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2937 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/iv/test_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8398 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/iv/test_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11439 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10592 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/test_gmm.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8594 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/iv/test_formulas.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/iv/results/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5777 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/housing.csv
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2170 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/simulated-test-data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2533 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/execute-stata.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3331 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/read_stata_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13232 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/stata-iv-housing-results.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)   547258 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/stata-iv-simulated-results.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4111 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/execute-stata-simulated-data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    97696 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/iv/results/simulated-data.dta
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3240 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2023 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/test_covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1557 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7205 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/test_model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3144 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/test_formulas.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11627 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/test_linear_factor_model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/asset_pricing/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/datasets/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      598 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/datasets/test_datasets.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/datasets/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1441 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/test_examples.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6487 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/test_utility.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/panel/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3375 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_fama_macbeth.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2608 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_random_effects.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    11724 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_between_ols.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7137 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/panel/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5606 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/panel/test_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7492 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_pooled_ols.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    27792 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/panel/test_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6602 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7928 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/panel/test_formula.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    40754 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_panel_ols.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4863 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_cluster_input_formats.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4934 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_simulated_against_stata.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/panel/results/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1723 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/panel/results/generate-panel-data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    65624 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/results/stata-panel-simulated-results.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1957 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/results/parse_stata_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)   578091 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/results/simulated-panel.dta
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/results/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3504 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/results/execute-stata-simulated-data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     6852 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_firstdifference_ols.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5929 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/panel/test_panel_covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/system/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    22669 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/test_sur.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9841 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/test_covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4888 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/test_sur_against_stata.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    12313 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1618 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/test_equivalence.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2494 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/test_3sls_against_stata.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    13632 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/test_gmm.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5397 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/test_formulas.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5698 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/test_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9252 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/test_3sls.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/tests/system/results/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2641 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/results/execute-stata-3sls.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2636 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/parse_stata_3sls_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3607 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/execute-stata.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    55085 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/simulated-sur.dta
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3350 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/parse_stata_results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    32162 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/stata-sur-results.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    85208 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/stata-3sls-results.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1601 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/system/results/generate_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    50504 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/tests/system/results/simulated-3sls.dta
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      972 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/tests/test_compat.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/fringe/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2042 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/fringe/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/jobtraining/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1635 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/jobtraining/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/birthweight/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      962 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/birthweight/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/fertility/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1025 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/fertility/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/mroz/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1032 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/mroz/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/card/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1991 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/card/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/munnell/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      517 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/munnell/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/meps/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1042 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/meps/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/wage/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1022 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/wage/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      221 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/french/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1353 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/french/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/datasets/wage_panel/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      789 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/datasets/wage_panel/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    17354 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/utility.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/panel/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    76759 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/panel/model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    27383 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/panel/results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    20637 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/panel/covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    21108 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/panel/data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      297 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/panel/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      495 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/_version.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     2150 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/__init__.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/system/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    62913 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/system/model.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    19995 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/system/results.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     8459 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/system/_utility.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    16699 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/system/covariance.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      107 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/system/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     9612 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/system/gmm.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2018-08-29 15:12:30.000000 linearmodels-4.9/linearmodels/compat/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1496 2018-08-29 15:06:48.000000 linearmodels-4.9/linearmodels/compat/pandas.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      469 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/compat/statsmodels.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/compat/__init__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      375 2018-08-29 14:53:32.000000 linearmodels-4.9/linearmodels/compat/numpy.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    68611 2018-08-29 14:53:32.000000 linearmodels-4.9/versioneer.py
```

### Comparing `linearmodels-4.8/examples/system_formulas.ipynb` & `linearmodels-4.9/doc/source/system/examples/formulas.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979967948717949%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(2, 'When using the curly brace formula specification, the "*

 * *            'equation names are determined by the dependent variable names.  When names are '*

 * *            'repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) '*

 * *            'then the equation labels will be modified until they are unique.  This can produce '*

 * *            'meaningless equation labels, and so it is possible to pass an equation label using '*

 * *            "the syntax\\ […]*

```diff
@@ -89,15 +89,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Labeled Formulas\n",
                 "\n",
-                "When using the curly brace formula specification, the equation names are determined by the dependent variable names.  When names are repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) then the equation labels will be \"uglified\" until they are unique.  This can produce meaningless equation labels, and so it is possible to pass an equation label using the syntax\n",
+                "When using the curly brace formula specification, the equation names are determined by the dependent variable names.  When names are repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) then the equation labels will be modified until they are unique.  This can produce meaningless equation labels, and so it is possible to pass an equation label using the syntax\n",
                 "\n",
                 "```\n",
                 "{label : dep ~ exog}\n",
                 "```\n"
             ]
         },
         {
@@ -153,16 +153,16 @@
                 "print(weighted_mod.fit())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pre-specified Residual Covariance\n",
-                "Like a standard SUR, it is possible to pass a pre-specified residual covariance for use in the GLS step.  This is done using the keyword argument `sigma` in the `from_formula` method, and is otherwise identical to passing one to the standard SUR."
+                "### Prespecified Residual Covariance\n",
+                "Like a standard SUR, it is possible to pass a prespecified residual covariance for use in the GLS step.  This is done using the keyword argument `sigma` in the `from_formula` method, and is otherwise identical to passing one to the standard SUR."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `linearmodels-4.8/examples/iv_using-formulas.ipynb` & `linearmodels-4.9/doc/source/iv/examples/using-formulas.ipynb`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/examples/iv_advanced-examples.ipynb` & `linearmodels-4.9/doc/source/iv/examples/advanced-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'cells'": '{9: {\'source\': ["And finally the simple correlation between the endogenous variable '*

 * *            'and the instruments.  Instruments must be correlated to be relevant (but also must be '*

 * *            "exogenous, which can't be examined using simple correlation).  The correlation of "*

 * *            '`firmsz` is especially low, which might lead to the weak instruments problem if used '*

 * *            'exclusively.  "]}, 21: {\'source\': {insert: [(4, \'The default weighting matrix is '*

 * *            "r […]*

```diff
@@ -87,15 +87,15 @@
                 "print(data[instruments].describe(percentiles=[]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "And finally the simple correlation between the endogenous variable and the instruments.  Instruments must be correlated to be relevant (but also must be exogenous, which can't be examined using simple correlation).  THe correlation of `firmsz` is especially low, which might lead to the weak instruments problem if used exclusively.  "
+                "And finally the simple correlation between the endogenous variable and the instruments.  Instruments must be correlated to be relevant (but also must be exogenous, which can't be examined using simple correlation).  The correlation of `firmsz` is especially low, which might lead to the weak instruments problem if used exclusively.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -220,15 +220,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## GMM Estimation\n",
                 "\n",
                 "GMM estimation can be more efficient than 2SLS when there are more than one instrument.  By default, 2-step efficient GMM is used (assuming the weighting matrix is correctly specified).  It is possible to iterate until convergence using the optional keyword input ``iter_limit``, which is naturally 2 by default.  Generally, GMM-CUE would be preferred to using multiple iterations of standard GMM.\n",
                 "\n",
-                "The default weighting matrix is robust to heteroskecasticity (but not clustering)."
+                "The default weighting matrix is robust to heteroskedasticity (but not clustering)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": true
@@ -430,15 +430,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Single Instrument Regressions\n",
-                "It can be useful to run the just identified regressions to see how the IV estimate varies by instrument. The OLS model is included for comparrison. The coefficient when using ``lowincome`` is very similar to the OLS as is the $R^2$ which indicates this variable may be endogenous. The coefficient using ``firmsz`` is also very different, but this is probably due to the low correlation between ``firmsz`` and the endogenous regressor so that this is a weak instrument. "
+                "It can be useful to run the just identified regressions to see how the IV estimate varies by instrument. The OLS model is included for comparison. The coefficient when using ``lowincome`` is very similar to the OLS as is the $R^2$ which indicates this variable may be endogenous. The coefficient using ``firmsz`` is also very different, but this is probably due to the low correlation between ``firmsz`` and the endogenous regressor so that this is a weak instrument. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/examples/iv_basic-examples.ipynb` & `linearmodels-4.9/doc/source/iv/examples/basic-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'cells'": '{22: {\'source\': ["The variance of the squared residuals is not particularly well '*

 * *            "explained by the data, and so the GLS-type estimates and the usual IV estimates don't "*

 * *            'differ by much."]}, 50: {\'source\': ["Wooldridge\'s regression test of exogeneity '*

 * *            'uses regression residual where the endogenous variables are regressed on the '*

 * *            'exogenous and the instrument to test for endogeneity. IF the endogenous variable is '*

 * *            'actually ex […]*

```diff
@@ -216,15 +216,15 @@
                 "print(fgls_res)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The variance of the squared residuals isn't particularly well explained by the data, and so the GLS-type estimates and the usual IV estimates don't differ by much."
+                "The variance of the squared residuals is not particularly well explained by the data, and so the GLS-type estimates and the usual IV estimates don't differ by much."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -499,15 +499,15 @@
                 "print(res)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Wooldridge's regression test of exogeneity uses regression residual where the endogenous variables are regressed on the exogenous and the instrument to test for endogenity. IF the endogenous variable is actually exogenous these residuals should not be correlated with the variable of interest. "
+                "Wooldridge's regression test of exogeneity uses regression residual where the endogenous variables are regressed on the exogenous and the instrument to test for endogeneity. IF the endogenous variable is actually exogenous these residuals should not be correlated with the variable of interest. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -536,15 +536,15 @@
                 "print(res_direct)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Since this regression has two instrument it is possible to test for overidentification.  Wooldridge's overidentification test uses a regression to test whether the 2SLS residuals are uncorrelated with the instruments, which should be the case if the model is correct and the instruments aren't needed in the original model."
+                "Since this regression has two instrument it is possible to test for overidentification.  Wooldridge's overidentification test uses a regression to test whether the 2SLS residuals are uncorrelated with the instruments, which should be the case if the model is correct and the instruments are not needed in the original model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/examples/system_three-stage-ls.ipynb` & `linearmodels-4.9/doc/source/system/examples/three-stage-ls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998196248196248%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(9, 'The estimates are the same.  This interface is more "*

 * *            "useful for programmatically generating and estimating models.')], delete: [9]}}}"}*

```diff
@@ -166,15 +166,15 @@
                 "The model can be directly specified using a dictionary of dictionaries where the inner dictionaries contain the 4 components of the model:\n",
                 "\n",
                 "* dependent - The dependent variable\n",
                 "* exog - Exogenous regressors\n",
                 "* endog - Endogenous regressors\n",
                 "* instruments - Instrumental variables\n",
                 "\n",
-                "The estimates are the same.  This interface is more useful for programatically generating and estimating models."
+                "The estimates are the same.  This interface is more useful for programmatically generating and estimating models."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/examples/system_correct-greene-table-10-1.png` & `linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-1.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/examples/system_correct-greene-table-10-2.png` & `linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-2.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/examples/panel_using-formulas.ipynb` & `linearmodels-4.9/doc/source/panel/examples/using-formulas.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, 'The constant can be explicitly included using the `1 + "*

 * *            '` notation.  When a constant is included in the model, and additional constraint is '*

 * *            'imposed that the number of the effects is 0.  This allows the constant to be '*

 * *            "identified using the grand mean of the dependent and the regressors.')], delete: "*

 * *            '[2]}}}'}*

```diff
@@ -63,15 +63,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## PanelOLS with Entity Effects and a constant\n",
                 "\n",
-                "The constant can be explicitly included using the `1 + ` notation.  When a constant is included in the model, and additional constraint is imposed that the number of the effects is 0.  This allows the constant to be identified using teh grand mean of the dependent and the regressors."
+                "The constant can be explicitly included using the `1 + ` notation.  When a constant is included in the model, and additional constraint is imposed that the number of the effects is 0.  This allows the constant to be identified using the grand mean of the dependent and the regressors."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/examples/panel_examples.ipynb` & `linearmodels-4.9/doc/source/panel/examples/examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990354938271605%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(1, 'The random effects model is virtually identical to the "*

 * *            'pooled OLS model except that is accounts for the structure of the model and so is '*

 * *            'more efficient. Random effects uses a quasi-demeaning strategy which subtracts the '*

 * *            "time average of the within entity values to account for the common shock.')], delete: "*

 * *            "[1]}}, 18: {'source': {insert: [(4, 'For variable which can be consistently "*

 * *            'estimated, s […]*

```diff
@@ -74,15 +74,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Random effects\n",
-                "The random effects model is virtually identical to the pooled OLS model except that is accounts for the structure of the model and so is more efficient. Random effects uses a quasi-demeaning strategy which subtracts the time average fo the within entity values to account for the common shock."
+                "The random effects model is virtually identical to the pooled OLS model except that is accounts for the structure of the model and so is more efficient. Random effects uses a quasi-demeaning strategy which subtracts the time average of the within entity values to account for the common shock."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -195,15 +195,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Time Effects\n",
                 "Time effect can be added using ``time_effects=True``.  Here the time dummies are removed. Note that the core coefficients are identical. The only change is in the test statistic for poolability since not the \"effects\" include both entity and time, whereas before only entity were included.\n",
                 "\n",
                 "#### Effects vs Dummies\n",
-                "For variable which can be consistently estimated, such as time effects in the usual large N, fixed T panel, it isn't necessary to include these as effects.  They can instead be implemented as dummy variables.  "
+                "For variable which can be consistently estimated, such as time effects in the usual large N, fixed T panel, it is not necessary to include these as effects.  They can instead be implemented as dummy variables.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -217,15 +217,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Other Options\n",
-                "Some additional options are available when using ``PanelOLS`` and effects.  The ``use_lsdv`` can be used to force the model to be estimated using dummy variables.  This isn't necessary and will be slower in most circumstances.  This options is primarily included for testing.  ``auto_df`` instructs ``PanelOLS`` to determine the degree of freedom adjustment to make.  Unlike most other estimators, the treatment of effects depends on the covariance estimator.  For example, when using a classic covariance estimator, effects count as lost degrees of freedom.  When using entity effects and clustering by entity, they do not.  Setting ``auto_df=False`` will allow the entities to be counted or not, depending on the value of ``count_effects``."
+                "Some additional options are available when using ``PanelOLS`` and effects.  The ``use_lsdv`` can be used to force the model to be estimated using dummy variables.  This is not necessary and will be slower in most circumstances.  This options is primarily included for testing.  ``auto_df`` instructs ``PanelOLS`` to determine the degree of freedom adjustment to make.  Unlike most other estimators, the treatment of effects depends on the covariance estimator.  For example, when using a classic covariance estimator, effects count as lost degrees of freedom.  When using entity effects and clustering by entity, they do not.  Setting ``auto_df=False`` will allow the entities to be counted or not, depending on the value of ``count_effects``."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Using first differences\n",
```

### Comparing `linearmodels-4.8/examples/asset-pricing_examples.ipynb` & `linearmodels-4.9/doc/source/asset-pricing/examples/examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990146396396397%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(4, 'Note that when using this type of model, it is "*

 * *            'essential that the test portfolios are excess returns. This is not a requirement of '*

 * *            "the other factor model estimators. \\n')], delete: [4]}}, 22: {'source': ['The size "*

 * *            'factor was insignificant and so is dropped. This does not have much of an effect on '*

 * *            "the estimates.']}, 24: {'source': {insert: [(0, 'The risk-free rate can be optionally "*

 * *            'estimated […]*

```diff
@@ -62,15 +62,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 1-Step Estimation using Seemingly Unrelated Regression (SUR)\n",
                 "\n",
                 "When the factors are traded assets, they must price themselves, and so the observed factor returns can be used to consistently estimate the expected factor returns.  This also allows a set of seemingly unrelated regressions where each test portfolio is regressed on the factors and a constant to estimate factor loadings and $\\alpha$s. \n",
                 "\n",
-                "Note that when using this type of model, it is essential that the test portfolios are excess returns. This isn't a requirement of the other factor model estimators. \n",
+                "Note that when using this type of model, it is essential that the test portfolios are excess returns. This is not a requirement of the other factor model estimators. \n",
                 "\n",
                 "This specification is a CAP-M since only the market is included.  The J-statistic tests whether all model $\\alpha$s are 0.  The CAP-M is unsurprisingly unable to price the test portfolios."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -220,15 +220,15 @@
                 "print(res.betas.corr())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The size factor was insignificant and so is dropped. This doesn't have much of an effect on the estimates."
+                "The size factor was insignificant and so is dropped. This does not have much of an effect on the estimates."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -240,15 +240,15 @@
                 "print(mod.fit())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The risk-free rate can be optionally estimated.  This is useful in case excess returns are not available of if the risk-free rate used to construct the excess returns might be mis-specified.\n",
+                "The risk-free rate can be optionally estimated.  This is useful in case excess returns are not available of if the risk-free rate used to construct the excess returns might be misspecified.\n",
                 "\n",
                 "Here the estimated risk-free rate is small and insignificant and has little impact on the model J-statistic."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `linearmodels-4.8/examples/system_examples.ipynb` & `linearmodels-4.9/doc/source/system/examples/examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998836267961951%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(15, 'where $Y$ is a column vector that stacks the vectors "*

 * *            '$Y_i$ for $i=1,2,\\\\ldots,K$, $X$ is a block-diagonal matrix where diagonal block i '*

 * *            'is $X_i$, $\\\\beta$ is a stacked vector of the $K$ $\\\\beta_i$s and $\\\\epsilon$ '*

 * *            "is similarly comprised of the stacked columns of $\\\\epsilon_i$.\\n')], delete: "*

 * *            "[15]}}, 6: {'source': {insert: [(2, 'Seemingly Unrelated Models are fairly complex "*

 * *            'and eac […]*

```diff
@@ -15,15 +15,15 @@
                 "\n",
                 "$$ Y_i = X_i\\beta_i + \\epsilon_i$$\n",
                 "\n",
                 "so that the set of models can be expressed as \n",
                 "\n",
                 "$$ Y = X\\beta + \\epsilon$$\n",
                 "\n",
-                "where $Y$ is a column vector that stacks the vectors $Y_i$ for $i=1,2,\\ldots,K$, $X$ is a block-diagonal matrix where the i-th block is $X_i$, $\\beta$ is a stacked vector of the $K$ $\\beta_i$s and $\\epsilon$ is similarly comprised of the stacked columns of $\\epsilon_i$.\n",
+                "where $Y$ is a column vector that stacks the vectors $Y_i$ for $i=1,2,\\ldots,K$, $X$ is a block-diagonal matrix where diagonal block i is $X_i$, $\\beta$ is a stacked vector of the $K$ $\\beta_i$s and $\\epsilon$ is similarly comprised of the stacked columns of $\\epsilon_i$.\n",
                 "\n",
                 "The model can be estimated using OLS with the usual estimator\n",
                 "\n",
                 "$$\\hat{\\beta}_{OLS} = \\left(X^\\prime X\\right)^{-1}X^\\prime Y.$$\n",
                 "\n",
                 "Since there are multiple series, a GLS estimator that accounts for the cross-sectional heteroskedasticity as well as the correlation of residuals can be estimated \n",
                 "\n",
@@ -115,15 +115,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Basic Usage\n",
                 "\n",
-                "Seemingly Unrelated Models are fairly complex and each equation could have a different number of regressors.  As a result, it isn't possibly to use standard `pandas` or `numpy` data structures, and so dictionaries (or technically dictionary-like objects) are used.  In practice, it is strongly recommended to use a `OrderedDictionary` from the `collections` module.  This ensures that equation order will be preserved. In addition, the dictionary must have the following structure:\n",
+                "Seemingly Unrelated Models are fairly complex and each equation could have a different number of regressors.  As a result, it is not possibly to use standard `pandas` or `numpy` data structures, and so dictionaries (or technically dictionary-like objects) are used.  In practice, it is strongly recommended to use a `OrderedDictionary` from the `collections` module.  This ensures that equation order will be preserved. In addition, the dictionary must have the following structure:\n",
                 "\n",
                 "* `keys` **must be strings** and will be used as equation labels\n",
                 "* The value associated with each key must be either a dictionary or a tuple.\n",
                 "\n",
                 "  * When a dictionary is used, it must have two keys, `dependent` and `exog`.  It can optionally have a third key `weights` which provides weights to use in the regression.\n",
                 "  * When a tuple is used, it must have two elements and takes the form `(dependent, exog)`.  It can optionally contains weights in which case it takes the form `(dependent, exog, weights)`.\n",
                 "\n",
@@ -245,15 +245,15 @@
                 "print(res.equations['WC'])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The current version of the model doesn't facilitate cross equation comparisons and so this is manually implemented here. "
+                "The current version of the model does not facilitate cross equation comparisons and so this is manually implemented here. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -491,22 +491,22 @@
                 "print(fres_het.summary)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Pre-specified Residual Covariance Estimators"
+                "## Prespecified Residual Covariance Estimators"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The GLS estimator can be used with a user specified covariance.  This example uses and equi-correlation covariance in the state GDP model.  The estimator must be used when constructing the model through the `sigma` keyword argument."
+                "The GLS estimator can be used with a user specified covariance.  This example uses a covariance where all correlations are identical (equicorrelation) in the state GDP model.  The estimator must be used when constructing the model through the `sigma` keyword argument."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -605,15 +605,15 @@
                 "\n",
                 "More complicated constraints can be used to produce interesting models.  Using the same idea as the previous set of constraints, a pooled SUR (excluding the constant) is constructed by restricting all coefficients to have the same value.  Here the form of the restriction is \n",
                 "\n",
                 "$$ \\beta_{var,0} - \\beta_{var,j} = 0$$\n",
                 "\n",
                 "so that the restriction is identical to the previous, only applied to all variables excluding the constant.\n",
                 "\n",
-                "Here the estimated from the first two equations are shown. ALl coefficients except the intercept are identical across equations.\n",
+                "Here the estimated from the first two equations are shown. All coefficients except the intercept are identical across equations.\n",
                 "\n",
                 "**Note**: When linear constraints are imposed, the parameter covariance matrix will be singular.  Caution is needed to ensure test statistics are meaningful."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `linearmodels-4.8/examples/asset-pricing_formulas.ipynb` & `linearmodels-4.9/doc/source/asset-pricing/examples/formulas.ipynb`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/examples/panel_data-formats.ipynb` & `linearmodels-4.9/doc/source/panel/examples/data-formats.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'This example uses the job training data to construct a "*

 * *            'MultiIndex `DataFrame` using the `set_index` command. The entity index is `fcode` and '*

 * *            "the time index is `year`.')], delete: [3]}}}"}*

```diff
@@ -17,15 +17,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Multi Index DataFrames\n",
                 "The most precise data format to use is a MultiIndex `DataFrame`.  This is the most precise since only single columns can preserve all types within a panel.  For example, it is not possible to span a single Categorical variable across multiple columns when using a pandas `Panel`. \n",
                 "\n",
-                "This example uses the jobtraining example to format a MultiIndex `DataFrame` using the `set_index` command. The entity index is known as fcode and the time index is year."
+                "This example uses the job training data to construct a MultiIndex `DataFrame` using the `set_index` command. The entity index is `fcode` and the time index is `year`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/examples/system_correct-greene-table-10-3.png` & `linearmodels-4.9/doc/source/system/examples/system_correct-greene-table-10-3.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/README.rst` & `linearmodels-4.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Linear Models
 =============
 
-|Build Status| |codecov|
+|Build Status| |codecov| |Codacy Badge| |codebeat badge|
 
 Linear (regression) models for Python. Extends
 `statsmodels <http://www.statsmodels.org>`__ with Panel regression,
 instrumental variable estimators, system estimators and models for
 estimating asset prices:
 
 -  **Panel models**:
@@ -43,68 +43,68 @@
 Like `statsmodels <http://www.statsmodels.org>`__ to include, supports
 `patsy <https://patsy.readthedocs.io/en/latest/>`__ formulas for
 specifying models. For example, the classic Grunfeld regression can be
 specified
 
 .. code:: python
 
-    import numpy as np
-    from statsmodels.datasets import grunfeld
-    data = grunfeld.load_pandas().data
-    data.year = data.year.astype(np.int64)
-    # MultiIndex, entity - time
-    data = data.set_index(['firm','year'])
-    from linearmodels import PanelOLS
-    mod = PanelOLS(data.invest, data[['value','capital']], entity_effect=True)
-    res = mod.fit(cov_type='clustered', cluster_entity=True)
+   import numpy as np
+   from statsmodels.datasets import grunfeld
+   data = grunfeld.load_pandas().data
+   data.year = data.year.astype(np.int64)
+   # MultiIndex, entity - time
+   data = data.set_index(['firm','year'])
+   from linearmodels import PanelOLS
+   mod = PanelOLS(data.invest, data[['value','capital']], entity_effects=True)
+   res = mod.fit(cov_type='clustered', cluster_entity=True)
 
 Models can also be specified using the formula interface.
 
 .. code:: python
 
-    from linearmodels import PanelOLS
-    mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffect', data)
-    res = mod.fit(cov_type='clustered', cluster_entity=True)
+   from linearmodels import PanelOLS
+   mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffects', data)
+   res = mod.fit(cov_type='clustered', cluster_entity=True)
 
 The formula interface for ``PanelOLS`` supports the special values
 ``EntityEffects`` and ``TimeEffects`` which add entity (fixed) and time
 effects, respectively.
 
 Instrumental Variable Models
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 IV regression models can be similarly specified.
 
 .. code:: python
 
-    import numpy as np
-    from linearmodels.iv import IV2SLS
-    from linearmodels.datasets import mroz
-    data = mroz.load()
-    mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
+   import numpy as np
+   from linearmodels.iv import IV2SLS
+   from linearmodels.datasets import mroz
+   data = mroz.load()
+   mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
 
 The expressions in the ``[ ]`` indicate endogenous regressors (before
 ``~``) and the instruments.
 
 Installing
 ----------
 
 The latest release can be installed using pip
 
 .. code:: bash
 
-    pip install linearmodels
+   pip install linearmodels
 
 The master branch can be installed by cloning the repo and running setup
 
 .. code:: bash
 
-    git clone https://github.com/bashtage/linearmodels
-    cd linearmodels
-    python setup.py install
+   git clone https://github.com/bashtage/linearmodels
+   cd linearmodels
+   python setup.py install
 
 Documentation
 -------------
 
 `Stable Documentation <https://bashtage.github.io/linearmodels/>`__ is
 built on every tagged version using
 `doctr <https://github.com/drdoctr/doctr>`__. `Development
@@ -144,22 +144,28 @@
 -  xarray (0.9+, optional)
 
 Testing
 ~~~~~~~
 
 -  py.test
 
+.. _documentation-1:
+
 Documentation
 ~~~~~~~~~~~~~
 
 -  sphinx
--  guzzle\_sphinx\_theme
+-  guzzle_sphinx_theme
 -  nbsphinx
 -  nbconvert
 -  nbformat
 -  ipython
 -  jupyter
 
 .. |Build Status| image:: https://travis-ci.org/bashtage/linearmodels.svg?branch=master
    :target: https://travis-ci.org/bashtage/linearmodels
 .. |codecov| image:: https://codecov.io/gh/bashtage/linearmodels/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/bashtage/linearmodels
+.. |Codacy Badge| image:: https://api.codacy.com/project/badge/Grade/c771bce50a164b6fa71c344b374f140d
+   :target: https://www.codacy.com/app/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade
+.. |codebeat badge| image:: https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243
+   :target: https://codebeat.co/projects/github-com-bashtage-linearmodels-master
```

### Comparing `linearmodels-4.8/README.md` & `linearmodels-4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Linear Models
 
 [![Build Status](https://travis-ci.org/bashtage/linearmodels.svg?branch=master)](https://travis-ci.org/bashtage/linearmodels)
 [![codecov](https://codecov.io/gh/bashtage/linearmodels/branch/master/graph/badge.svg)](https://codecov.io/gh/bashtage/linearmodels)
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/c771bce50a164b6fa71c344b374f140d)](https://www.codacy.com/app/bashtage/linearmodels?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bashtage/linearmodels&amp;utm_campaign=Badge_Grade)
+[![codebeat badge](https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243)](https://codebeat.co/projects/github-com-bashtage-linearmodels-master)
 
 Linear (regression) models for Python.  Extends
 [statsmodels](http://www.statsmodels.org) with Panel regression,
 instrumental variable estimators, system estimators and models for
 estimating asset prices:
  
 - **Panel models**:
@@ -44,23 +46,23 @@
 import numpy as np
 from statsmodels.datasets import grunfeld
 data = grunfeld.load_pandas().data
 data.year = data.year.astype(np.int64)
 # MultiIndex, entity - time
 data = data.set_index(['firm','year'])
 from linearmodels import PanelOLS
-mod = PanelOLS(data.invest, data[['value','capital']], entity_effect=True)
+mod = PanelOLS(data.invest, data[['value','capital']], entity_effects=True)
 res = mod.fit(cov_type='clustered', cluster_entity=True)
 ```
 
 Models can also be specified using the formula interface.
  
 ```python
 from linearmodels import PanelOLS
-mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffect', data)
+mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffects', data)
 res = mod.fit(cov_type='clustered', cluster_entity=True)
 ```
 
 The formula interface for ``PanelOLS`` supports the special values
 ``EntityEffects`` and ``TimeEffects`` which add entity (fixed) and time
 effects, respectively.
 
@@ -142,8 +144,8 @@
 
 * sphinx
 * guzzle_sphinx_theme
 * nbsphinx
 * nbconvert
 * nbformat
 * ipython
-* jupyter
+* jupyter
```

### Comparing `linearmodels-4.8/linearmodels/formula.py` & `linearmodels-4.9/linearmodels/formula.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/compat/pandas.py` & `linearmodels-4.9/linearmodels/compat/pandas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,30 @@
-from pandas.util.testing import assert_panel_equal
+from distutils.version import LooseVersion
+
+import pandas as pd
+
+PD_LT_023 = LooseVersion(pd.__version__) < LooseVersion('0.23')
+
+
+def concat(*args, **kwargs):
+    """
+    Shim around pandas concat that passes sort if allowed
+
+    See pandas.compat
+    """
+    if PD_LT_023 and 'sort' in kwargs:
+        kwargs = kwargs.copy()
+        del kwargs['sort']
+    elif not PD_LT_023:
+        if 'sort' not in kwargs:
+            kwargs = kwargs.copy()
+            kwargs['sort'] = False
+
+    return pd.concat(*args, **kwargs)
+
 
 try:
     from pandas.api.types import (is_numeric_dtype, is_categorical,
                                   is_string_dtype, is_categorical_dtype,
                                   is_datetime64_any_dtype)
 
     # From pandas 0.20.1
@@ -22,15 +44,10 @@
         return isinstance(obj, str)
 
 except ImportError:  # pragma: no cover
     from pandas.core.common import (is_string_dtype, is_numeric_dtype,
                                     is_categorical, is_categorical_dtype,
                                     is_datetime64_any_dtype, is_string_like)
 
-try:
-    from pandas.testing import assert_frame_equal, assert_series_equal
-except ImportError:
-    from pandas.util.testing import assert_frame_equal, assert_series_equal
-
 __all__ = ['is_string_dtype', 'is_numeric_dtype', 'is_categorical',
            'is_string_like', 'is_categorical_dtype', 'is_datetime64_any_dtype',
-           'assert_frame_equal', 'assert_series_equal', 'assert_panel_equal']
+           'concat']
```

### Comparing `linearmodels-4.8/linearmodels/panel/data.py` & `linearmodels-4.9/linearmodels/panel/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from itertools import product
 
 import numpy as np
 import pandas as pd
-from numpy import ndarray
 from pandas import DataFrame, Panel, Series
 
 from linearmodels.compat.numpy import lstsq
 from linearmodels.compat.pandas import (is_categorical,
                                         is_datetime64_any_dtype,
                                         is_numeric_dtype, is_string_dtype,
-                                        is_string_like)
-from linearmodels.utility import ensure_unique_column
+                                        is_string_like, concat)
+from linearmodels.utility import ensure_unique_column, panel_to_frame
 
 __all__ = ['PanelData']
 
 
 class _Panel(object):
     """
     Convert a MI DataFrame to a 3-d structure where columns are items
@@ -75,26 +74,26 @@
         return self._values
 
     def to_frame(self):
         return self._frame
 
 
 def convert_columns(s, drop_first):
-    if is_string_dtype(s.dtype) and s.map(lambda v: is_string_like(v)).all():
+    if is_string_dtype(s.dtype) and s.map(is_string_like).all():
         s = s.astype('category')
 
     if is_categorical(s):
         out = pd.get_dummies(s, drop_first=drop_first)
         out.columns = [str(s.name) + '.' + str(c) for c in out]
         return out
     return s
 
 
 def expand_categoricals(x, drop_first):
-    return pd.concat([convert_columns(x[c], drop_first) for c in x.columns], axis=1)
+    return concat([convert_columns(x[c], drop_first) for c in x.columns], axis=1)
 
 
 class PanelData(object):
     """
     Abstraction to handle alternative formats for panel data
 
     Parameters
@@ -105,14 +104,17 @@
         Variable name to use when naming variables in NumPy arrays or
         xarray DataArrays
     convert_dummies : bool, optional
         Flat indicating whether pandas categoricals or string input data
         should be converted to dummy variables
     drop_first : bool, optional
         Flag indicating to drop first dummy category when converting
+    copy: bool, optional
+        Flag indicating whether to copy the input. Only has an effect when
+        x is a DataFrame
 
     Notes
     -----
     Data can be either 2- or 3-dimensional. The three key dimensions are
 
     * nvar - number of variables
     * nobs - number of time periods
@@ -135,51 +137,64 @@
     TypeError
         If the input type is not supported
     ValueError
         If the input has the wrong number of dimensions or a MultiIndex
         DataFrame does not have 2 levels
     """
 
-    def __init__(self, x, var_name='x', convert_dummies=True, drop_first=True):
+    def __init__(self, x, var_name='x', convert_dummies=True, drop_first=True, copy=True):
         self._var_name = var_name
         self._convert_dummies = convert_dummies
         self._drop_first = drop_first
         self._panel = None
         self._shape = None
+        index_names = ['entity', 'time']
         if isinstance(x, PanelData):
             x = x.dataframe
         self._original = x
 
-        if not isinstance(x, (Series, DataFrame, Panel, ndarray)):
+        if not isinstance(x, (Series, DataFrame, Panel, np.ndarray)):
             try:
                 from xarray import DataArray
                 if isinstance(x, DataArray):
                     if x.ndim not in (2, 3):
                         raise ValueError('Only 2-d or 3-d DataArrays are supported')
-                    x = x.to_pandas()
+                    if x.ndim == 2:
+                        x = x.to_pandas()
+                    else:
+                        items = x.coords[x.dims[0]].values.tolist()
+                        major = x.coords[x.dims[1]].values.tolist()
+                        minor = x.coords[x.dims[2]].values.tolist()
+                        values = x.values
+                        x = panel_to_frame(values, items, major, minor, True)
             except ImportError:
                 pass
 
         if isinstance(x, Series) and isinstance(x.index, pd.MultiIndex):
             x = DataFrame(x)
         elif isinstance(x, Series):
             raise ValueError('Series can only be used with a 2-level MultiIndex')
 
         if isinstance(x, (Panel, DataFrame)):
             if isinstance(x, DataFrame):
                 if isinstance(x.index, pd.MultiIndex):
                     if len(x.index.levels) != 2:
                         raise ValueError('DataFrame input must have a '
                                          'MultiIndex with 2 levels')
-                    self._frame = x.copy()
+                    if isinstance(self._original, (pd.DataFrame, PanelData, pd.Series)):
+                        for i in range(2):
+                            index_names[i] = x.index.levels[i].name or index_names[i]
+                    self._frame = x
+                    if copy:
+                        self._frame = self._frame.copy()
                 else:
                     self._frame = DataFrame({var_name: x.T.stack(dropna=False)})
             else:
                 self._frame = x.swapaxes(1, 2).to_frame(filter_observations=False)
-        elif isinstance(x, ndarray):
+        elif isinstance(x, np.ndarray):
             if x.ndim not in (2, 3):
                 raise ValueError('2 or 3-d array required for numpy input')
             if x.ndim == 2:
                 x = x[None, :, :]
 
             k, t, n = x.shape
             var_str = var_name + '.{0:0>' + str(int(np.log10(k) + .01)) + '}'
@@ -202,16 +217,17 @@
         time_index = Series(self._frame.index.levels[1])
         if not (is_numeric_dtype(time_index.dtype) or
                 is_datetime64_any_dtype(time_index.dtype)):
             raise ValueError('The index on the time dimension must be either '
                              'numeric or date-like')
         # self._k, self._t, self._n = self.panel.shape
         self._k, self._t, self._n = self.shape
-        self._frame.index.levels[0].name = 'entity'
-        self._frame.index.levels[1].name = 'time'
+        levels = self._frame.index.levels
+        for i in range(2):
+            levels[i].name = index_names[i]
 
     @property
     def panel(self):
         """pandas Panel view of data"""
         if self._panel is None:
             self._panel = _Panel(self._frame)
         return self._panel
@@ -448,15 +464,16 @@
         -------
         demeaned : PanelData
             Demeaned data according to type
 
         Notes
         -----
         If weights are provided, the values returned will be scaled by
-        sqrt(weights) so that they can be used in WLS estimation.
+        the square root of the weights so that they can be used in WLS
+        estimation.
         """
         if group not in ('entity', 'time', 'both'):
             raise ValueError
         if group == 'both':
             return self._demean_both(weights)
 
         level = 0 if group == 'entity' else 1
@@ -558,18 +575,16 @@
         Returns
         -------
         diffs : PanelData
             Differenced values
         """
         diffs = self.panel.values
         diffs = diffs[:, 1:] - diffs[:, :-1]
-        diffs = Panel(diffs, items=self.panel.items,
-                      major_axis=self.panel.major_axis[1:],
-                      minor_axis=self.panel.minor_axis)
-        diffs = diffs.swapaxes(1, 2).to_frame(filter_observations=False)
+        diffs = panel_to_frame(diffs, self.panel.items, self.panel.major_axis[1:],
+                               self.panel.minor_axis, True)
         diffs = diffs.reindex(self._frame.index).dropna(how='any')
         return PanelData(diffs)
 
     @staticmethod
     def _minimize_multiindex(df):
         index_cols = list(df.index.names)
         orig_names = index_cols[:]
```

### Comparing `linearmodels-4.8/linearmodels/panel/results.py` & `linearmodels-4.9/linearmodels/panel/results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime as dt
 
 import numpy as np
-from numpy import diag, sqrt
 from pandas import DataFrame, Series, concat
 from scipy import stats
 from statsmodels.iolib.summary import SimpleTable, fmt_2cols, fmt_params
 
 from linearmodels.compat.statsmodels import Summary
 from linearmodels.iv.results import default_txt_fmt, stub_concat, table_concat
 from linearmodels.utility import (_ModelComparison, _SummaryStr, _str, cached_property,
@@ -63,15 +62,15 @@
         return DataFrame(self._deferred_cov(),
                          columns=self._var_names,
                          index=self._var_names)
 
     @property
     def std_errors(self):
         """Estimated parameter standard errors"""
-        return Series(sqrt(diag(self.cov)), self._var_names, name='std_error')
+        return Series(np.sqrt(np.diag(self.cov)), self._var_names, name='std_error')
 
     @property
     def tstats(self):
         """Parameter t-statistics"""
         return Series(self._params / self.std_errors, name='tstat')
 
     @cached_property
@@ -227,15 +226,19 @@
             q = stats.norm.ppf(ci_quantiles)
         q = q[None, :]
         ci = self.params[:, None] + self.std_errors[:, None] * q
         return DataFrame(ci, index=self._var_names, columns=['lower', 'upper'])
 
     @property
     def summary(self):
-        """Summary table of model estimation results"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
 
         title = self.name + ' Estimation Summary'
         mod = self.model
 
         top_left = [('Dep. Variable:', mod.dependent.vars[0]),
                     ('Estimator:', self.name),
                     ('No. Observations:', self.nobs),
@@ -358,15 +361,15 @@
         In- and out-of-sample predictions
 
         Parameters
         ----------
         exog : array-like
             Exogenous values to use in out-of-sample prediction (nobs by nexog)
         data : DataFrame, optional
-            Dataframe to use for out-of-sample predictions when model was
+            DataFrame to use for out-of-sample predictions when model was
             constructed using a formula.
         fitted : bool, optional
             Flag indicating whether to include the fitted values
         effects : bool, optional
             Flag indicating whether to include estimated effects
         idiosyncratic : bool, optional
             Flag indicating whether to include the estimated idiosyncratic shock
@@ -462,15 +465,15 @@
         provides.
 
         .. math::
 
            W = \hat{\beta}_{-}' \hat{\Sigma}_{-}^{-1} \hat{\beta}_{-}
 
         where :math:`\hat{\beta}_{-}` does not include the model constant and
-        :math:`\hat{\Sigma}_{-}` is tht estimated covariance of the
+        :math:`\hat{\Sigma}_{-}` is the estimated covariance of the
         parameters, also excluding the constant.  The test statistic is
         distributed as :math:`\chi^2_{k}` where k is the number of non-
         constant parameters.
 
         If ``debiased`` is True, then the Wald statistic is divided by the
         number of restrictions and inference is made using an :math:`F_{k,df}`
         distribution where df is the residual degree of freedom from the model.
@@ -588,15 +591,20 @@
     @property
     def rsquared_inclusive(self):
         """Model Coefficient of determination including fit of included effects"""
         return self._r2_ex_effects
 
     @property
     def summary(self):
-        """Summary table of model estimation results"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
+
         smry = super(PanelEffectsResults, self).summary
 
         is_invalid = np.isfinite(self.f_pooled.stat)
         f_pool = _str(self.f_pooled.stat) if is_invalid else '--'
         f_pool_pval = pval_format(self.f_pooled.pval) if is_invalid else '--'
         f_pool_name = self.f_pooled.dist_name if is_invalid else '--'
 
@@ -714,15 +722,20 @@
     @property
     def cov_estimator(self):
         """Covariance estimator descriptions"""
         return self._get_property('_cov_type')
 
     @property
     def summary(self):
-        """Summary table of model comparison"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
+
         smry = Summary()
         models = list(self._results.keys())
         title = 'Model Comparison'
         stubs = ['Dep. Variable', 'Estimator', 'No. Observations', 'Cov. Est.', 'R-squared',
                  'R-Squared (Within)', 'R-Squared (Between)', 'R-Squared (Overall)',
                  'F-statistic', 'P-value (F-stat)']
         dep_name = {}
@@ -761,15 +774,15 @@
 
         all_effects = []
         for key in self._results:
             res = self._results[key]
             effects = getattr(res, 'included_effects', [])
             all_effects.append(effects)
 
-        neffect = max(map(lambda l: len(l), all_effects))
+        neffect = max(map(len, all_effects))
         effects = []
         effects_stub = ['Effects']
         for i in range(neffect):
             if i > 0:
                 effects_stub.append('')
             row = []
             for j in range(len(self._results)):
```

### Comparing `linearmodels-4.8/linearmodels/panel/covariance.py` & `linearmodels-4.9/linearmodels/panel/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/panel/model.py` & `linearmodels-4.9/linearmodels/panel/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                                            HomoskedasticCovariance)
 from linearmodels.panel.data import PanelData
 from linearmodels.panel.results import (PanelEffectsResults, PanelResults,
                                         RandomEffectsResults)
 from linearmodels.utility import (AttrDict, InapplicableTestStatistic,
                                   InvalidTestStatistic, WaldTestStatistic,
                                   ensure_unique_column, has_constant,
-                                  missing_warning)
+                                  missing_warning, panel_to_frame)
 
 
 class PanelFormulaParser(object):
     """
     Parse formulas for OLS and IV models
 
     Parameters
@@ -36,15 +36,15 @@
     Notes
     -----
     The general structure of a formula is `dep ~ exog`
     """
 
     def __init__(self, formula, data, eval_env=2):
         self._formula = formula
-        self._data = PanelData(data)
+        self._data = PanelData(data, convert_dummies=False, copy=False)
         self._na_action = NAAction(on_NA='raise', NA_types=[])
         self._eval_env = eval_env
         self._dependent = self._exog = None
         self._parse()
 
     def _parse(self):
         parts = self._formula.split('~')
@@ -1350,15 +1350,15 @@
             be coerced to integer values by treating as categorical variables
 
         When using a clustered covariance estimator, all cluster ids must be
         identical within an entity.
         """
         y, x, w = self._prepare_between()
         if np.all(self.weights.values2d == 1.0) and not reweight:
-            w = root_w = np.ones_like(w)
+            w = root_w = np.ones_like(y)
         else:
             root_w = np.sqrt(w)
 
         wx = root_w * x
         wy = root_w * y
         params = lstsq(wx, wy)[0]
 
@@ -1496,17 +1496,16 @@
                                   name=name)
             if clusters is not None:
                 clusters[name] = group_ids
             else:
                 clusters = pd.DataFrame(group_ids)
         clusters = PanelData(clusters)
         values = clusters.values3d[:, 1:]
-        clusters = pd.Panel(values, items=clusters.panel.items,
-                            major_axis=clusters.panel.major_axis[1:],
-                            minor_axis=clusters.panel.minor_axis)
+        clusters = panel_to_frame(values, clusters.panel.items, clusters.panel.major_axis[1:],
+                                  clusters.panel.minor_axis, True)
         clusters = PanelData(clusters).dataframe
         clusters = clusters.loc[self.dependent.first_difference().index]
         clusters = clusters.astype(np.int64)
 
         cov_config_upd['clusters'] = clusters.values if clusters is not None else clusters
 
         return cov_est, cov_config_upd
@@ -1573,18 +1572,16 @@
 
         if np.all(self.weights.values2d == 1.0):
             w = root_w = np.ones_like(y)
         else:
             w = 1.0 / self.weights.values3d
             w = w[:, :-1] + w[:, 1:]
             w = 1.0 / w
-            w = pd.Panel(w, items=self.weights.panel.items,
-                         major_axis=self.weights.panel.major_axis[1:],
-                         minor_axis=self.weights.panel.minor_axis)
-            w = w.swapaxes(1, 2).to_frame(filter_observations=False)
+            w = panel_to_frame(w, self.weights.panel.items, self.weights.panel.major_axis[1:],
+                               self.weights.panel.minor_axis, True)
             w = w.reindex(self.weights.index).dropna(how='any')
             index = w.index
             w = w.values
 
             w /= w.mean()
             root_w = np.sqrt(w)
```

### Comparing `linearmodels-4.8/linearmodels/datasets/birthweight/__init__.py` & `linearmodels-4.9/linearmodels/datasets/birthweight/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/jobtraining/__init__.py` & `linearmodels-4.9/linearmodels/datasets/jobtraining/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/french/__init__.py` & `linearmodels-4.9/linearmodels/datasets/french/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/meps/__init__.py` & `linearmodels-4.9/linearmodels/datasets/meps/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/mroz/__init__.py` & `linearmodels-4.9/linearmodels/datasets/mroz/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/munnell/__init__.py` & `linearmodels-4.9/linearmodels/datasets/munnell/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/wage_panel/__init__.py` & `linearmodels-4.9/linearmodels/datasets/wage_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/fertility/__init__.py` & `linearmodels-4.9/linearmodels/datasets/fertility/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/fringe/__init__.py` & `linearmodels-4.9/linearmodels/datasets/fringe/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/wage/__init__.py` & `linearmodels-4.9/linearmodels/datasets/wage/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/datasets/card/__init__.py` & `linearmodels-4.9/linearmodels/datasets/card/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/iv/gmm.py` & `linearmodels-4.9/linearmodels/iv/gmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,23 +342,23 @@
     Notes
     -----
     Optional keyword argument for specific covariance estimators:
 
     **kernel**
 
     * ``kernel``: Name of kernel to use.  See
-      linearmodels.covariance.KernelCovariance for details on available
-      kernels
+      :class:`~linearmodels.covariance.KernelCovariance` for details on
+      available kernels
     * ``bandwidth``: Bandwidth to use when computing the weight.  If not
       provided, nobs - 2 is used.
 
     **cluster**
 
     * ``clusters``: Array containing the cluster indices.  See
-      linearmodels.covariance.OneWayClusteredCovariance
+      :class:`~linearmodels.covariance.OneWayClusteredCovariance`
 
     See also
     --------
     linearmodels.iv.covariance.HomoskedasticCovariance,
     linearmodels.iv.covariance.HeteroskedasticCovariance,
     linearmodels.iv.covariance.KernelCovariance,
     linearmodels.iv.covariance.OneWayClusteredCovariance
@@ -406,15 +406,15 @@
             if self._cov_config.get('bandwidth', False):
                 out += '\nBandwidth: {0}'.format(self._cov_config['bandwidth'])
         return out
 
     @property
     def cov(self):
         x, z, eps, w = self.x, self.z, self.eps, self.w
-        nobs, nvar = x.shape
+        nobs = x.shape[0]
         xpz = x.T @ z / nobs
         xpzw = xpz @ w
         xpzwzpx_inv = inv(xpzw @ xpz.T)
 
         score_cov = self._score_cov_estimator(debiased=self.debiased,
                                               **self._cov_config)
         s = score_cov.weight_matrix(x, z, eps)
```

### Comparing `linearmodels-4.8/linearmodels/iv/data.py` & `linearmodels-4.9/linearmodels/iv/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 
 import numpy as np
 import pandas as pd
 
 from linearmodels.compat.pandas import (is_categorical, is_categorical_dtype,
                                         is_numeric_dtype, is_string_dtype,
-                                        is_string_like)
+                                        is_string_like, concat)
 
 dim_err = '{0} has too many dims.  Maximum is 2, actual is {1}'
 type_err = 'Only ndarrays, DataArrays and Series and DataFrames are supported'
 
 
 def convert_columns(s, drop_first):
     if is_categorical(s):
@@ -21,15 +21,15 @@
         return out
     return s
 
 
 def expand_categoricals(x, drop_first):
     if x.shape[1] == 0:
         return x
-    return pd.concat([convert_columns(x[c], drop_first) for c in x.columns], axis=1)
+    return concat([convert_columns(x[c], drop_first) for c in x.columns], axis=1)
 
 
 class IVData(object):
     """Simple class to abstract different input data formats
 
     Parameters
     ----------
@@ -74,34 +74,40 @@
             self._labels = {0: index, 1: cols}
 
         elif isinstance(x, (pd.Series, pd.DataFrame)):
             if isinstance(x, pd.Series):
                 name = var_name if not x.name else x.name
                 x = pd.DataFrame({name: x})
             copied = False
+            columns = list(x.columns)
+            if len(set(columns)) != len(columns):
+                raise ValueError('DataFrame contains duplicate column names. '
+                                 'All column names must be distinct')
+            all_numeric = True
             for col in x:
                 c = x[col]
-                if is_string_dtype(c.dtype) and \
-                        c.map(lambda v: is_string_like(v)).all():
-
+                if is_string_dtype(c.dtype) and c.map(is_string_like).all():
                     c = c.astype('category')
                     if not copied:
                         x = x.copy()
                         copied = True
                     x[col] = c
                 dt = c.dtype
+                all_numeric = all_numeric and is_numeric_dtype(dt)
                 if not (is_numeric_dtype(dt) or is_categorical_dtype(dt)):
                     raise ValueError('Only numeric, string  or categorical '
                                      'data permitted')
 
             if convert_dummies:
                 x = expand_categoricals(x, drop_first)
 
             self._pandas = x
-            self._ndarray = self._pandas.values.astype(np.float64)
+            self._ndarray = self._pandas.values
+            if all_numeric or convert_dummies:
+                self._ndarray = self._ndarray.astype(np.float64)
             self._labels = {i: list(label) for i, label in zip(range(x.ndim), x.axes)}
 
         else:
             try:
                 import xarray as xr
             except ImportError:
                 raise TypeError(type_err)
@@ -163,10 +169,11 @@
         return self._labels
 
     @property
     def isnull(self):
         return np.any(self._pandas.isnull(), axis=1)
 
     def drop(self, locs):
+        locs = np.asarray(locs)
         self._pandas = self.pandas.loc[~locs]
         self._ndarray = self._ndarray[~locs]
         self._labels[0] = list(pd.Series(self._labels[0]).loc[~locs])
```

### Comparing `linearmodels-4.8/linearmodels/iv/results.py` & `linearmodels-4.9/linearmodels/iv/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from linearmodels.compat.statsmodels import Summary
 from linearmodels.iv._utility import annihilate, proj
 from linearmodels.utility import (InvalidTestStatistic, WaldTestStatistic, _ModelComparison,
                                   _SummaryStr, _str, cached_property, pval_format)
 
 
 def stub_concat(lists, sep='='):
-    col_size = max([max(map(lambda s: len(s), l)) for l in lists])
+    col_size = max([max(map(len, l)) for l in lists])
     out = []
     for l in lists:
         out.extend(l)
         out.append(sep * (col_size + 2))
     return out[:-1]
 
 
 def table_concat(lists, sep='='):
     col_sizes = []
     for l in lists:
-        size = list(map(lambda r: list(map(lambda v: len(v), r)), l))
+        size = list(map(lambda r: list(map(len, r)), l))
         col_sizes.append(list(array(size).max(0)))
     col_size = array(col_sizes).max(axis=0)
     sep_cols = [sep * (cs + 2) for cs in col_size]
     out = []
     for l in lists:
         out.extend(l)
         out.append(sep_cols)
@@ -126,15 +126,15 @@
         Parameters
         ----------
         exog : array-like
             Exogenous values to use in out-of-sample prediction (nobs by nexog)
         endog : array-like
             Endogenous values to use in out-of-sample prediction (nobs by nendog)
         data : DataFrame, optional
-            Dataframe to use for out-of-sample predictions when model was
+            DataFrame to use for out-of-sample predictions when model was
             constructed using a formula.
         fitted : bool, optional
             Flag indicating whether to include the fitted values
         idiosyncratic : bool, optional
             Flag indicating whether to include the estimated idiosyncratic shock
         missing : bool, optional
             Flag indicating to adjust for dropped observations.  If True, the
@@ -216,21 +216,21 @@
         return 1 - ((n - c) / (n - k)) * (1 - self._r2)
 
     @property
     def cov_type(self):
         """Covariance estimator used"""
         return self._cov_type
 
-    @property
+    @cached_property
     def std_errors(self):
         """Estimated parameter standard errors"""
         std_errors = sqrt(diag(self.cov))
         return Series(std_errors, index=self._vars, name='stderr')
 
-    @property
+    @cached_property
     def tstats(self):
         """Parameter t-statistics"""
         return Series(self._params / self.std_errors, name='tstat')
 
     @cached_property
     def pvalues(self):
         """
@@ -321,15 +321,19 @@
             q = stats.norm.ppf(ci_quantiles)
         q = q[None, :]
         ci = self.params[:, None] + self.std_errors[:, None] * q
         return DataFrame(ci, index=self._vars, columns=['lower', 'upper'])
 
     @property
     def summary(self):
-        """Summary table of model estimation results"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
 
         title = self._method + ' Estimation Summary'
         mod = self.model
         top_left = [('Dep. Variable:', mod.dependent.cols[0]),
                     ('Estimator:', self._method),
                     ('No. Observations:', self.nobs),
                     ('Date:', self._datetime.strftime('%a, %b %d %Y')),
@@ -608,15 +612,15 @@
         t : WaldTestStatistic
             Object containing test statistic, p-value, distribution and null
 
         Notes
         -----
         Test statistic is difference between sum of squared OLS and sum of
         squared IV residuals where each set of residuals has been projected
-        onto the set of instruments in teh IV model.
+        onto the set of instruments in the IV model.
 
         Start by defining
 
         .. math ::
 
           \delta & = \hat{\epsilon}'_e P_{[z,w]} \hat{\epsilon}_e -
                      \hat{\epsilon}'_c P_{z} \hat{\epsilon}_c
@@ -636,15 +640,15 @@
 
         where :math:`q` is the number of variables tested.
         """
         null = 'All endogenous variables are exogenous'
         if variables is not None:
             null = 'Variables {0} are exogenous'.format(', '.join(variables))
 
-        e0, e1, e2, nobs, nexog, nendog, ntested = self._endogeneity_setup(variables)
+        e0, e1, e2, nobs, _, _, ntested = self._endogeneity_setup(variables)
         stat = e1.T @ e1 - e2.T @ e2
         stat /= (e0.T @ e0) / nobs
 
         name = 'Durbin test of exogeneity'
         df = ntested
         return WaldTestStatistic(float(stat), null, df, name=name)
 
@@ -663,15 +667,15 @@
         t : WaldTestStatistic
             Object containing test statistic, p-value, distribution and null
 
         Notes
         -----
         Test statistic is difference between sum of squared OLS and sum of
         squared IV residuals where each set of residuals has been projected
-        onto the set of instruments in teh IV model.
+        onto the set of instruments in the IV model.
 
         Start by defining
 
         .. math ::
 
           \delta & = \hat{\epsilon}'_e P_{[z,w]} \hat{\epsilon}_e -
                      \hat{\epsilon}'_c P_{z} \hat{\epsilon}_c
@@ -826,31 +830,28 @@
         The order of the instruments does not affect this test.
         """
         from linearmodels.iv.model import _OLS
         exog, endog = self.model.exog, self.model.endog
         instruments = self.model.instruments
         nobs, nendog = endog.shape
         ninstr = instruments.shape[1]
+        name = 'Wooldridge\'s score test of overidentification'
         if ninstr - nendog == 0:
-            import warnings
-            warnings.warn('Test requires more instruments than '
-                          'endogenous variables',
-                          UserWarning)
-            return WaldTestStatistic(0, 'Test is not feasible.', 1, name='Infeasible test.')
+            return InvalidTestStatistic('Test requires more instruments than '
+                                        'endogenous variables.', name=name)
 
         endog_hat = proj(endog.ndarray, c_[exog.ndarray, instruments.ndarray])
         q = instruments.ndarray[:, :(ninstr - nendog)]
         q_res = annihilate(q, c_[self.model.exog.ndarray, endog_hat])
         test_functions = q_res * self.resids.values[:, None]
         res = _OLS(ones((nobs, 1)), test_functions).fit(cov_type='unadjusted')
 
         stat = res.nobs * res.rsquared
         df = ninstr - nendog
         null = 'Model is not overidentified.'
-        name = 'Wooldridge\'s score test of overidentification'
         return WaldTestStatistic(stat, null, df, name=name)
 
     @cached_property
     def anderson_rubin(self):
         """
         Anderson-Rubin test of overidentifying restrictions
 
@@ -1168,15 +1169,19 @@
             mod = _OLS(dep, exog_instr)
             res[col] = mod.fit(cov_type=self._cov_type, **self._cov_config)
 
         return res
 
     @property
     def summary(self):
-        """Summary table of first-stage estimation results"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
         stubs_lookup = {'rsquared': 'R-squared',
                         'partial.rsquared': 'Partial R-squared',
                         'shea.rsquared': 'Shea\'s R-squared',
                         'f.stat': 'Partial F-statistic',
                         'f.pval': 'P-value (Partial F-stat)',
                         'f.dist': 'Partial F-stat Distn'}
         smry = Summary()
@@ -1266,15 +1271,19 @@
     @property
     def cov_estimator(self):
         """Covariance estimator descriptions"""
         return self._get_property('cov_estimator')
 
     @property
     def summary(self):
-        """Summary table of model comparison"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
         smry = Summary()
         models = list(self._results.keys())
         title = 'Model Comparison'
         stubs = ['Dep. Variable', 'Estimator', 'No. Observations', 'Cov. Est.', 'R-squared',
                  'Adj. R-squared', 'F-statistic', 'P-value (F-stat)']
         dep_name = OrderedDict()
         for key in self._results:
@@ -1306,15 +1315,15 @@
         vals = table_concat((vals, params_fmt))
         stubs = stub_concat((stubs, params_stub))
 
         all_instr = []
         for key in self._results:
             res = self._results[key]
             all_instr.append(res.model.instruments.cols)
-        ninstr = max(map(lambda l: len(l), all_instr))
+        ninstr = max(map(len, all_instr))
         instruments = []
         instrument_stub = ['Instruments']
         for i in range(ninstr):
             if i > 0:
                 instrument_stub.append('')
             row = []
             for j in range(len(self._results)):
```

### Comparing `linearmodels-4.8/linearmodels/iv/_utility.py` & `linearmodels-4.9/linearmodels/iv/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/iv/covariance.py` & `linearmodels-4.9/linearmodels/iv/covariance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Covariance estimation for 2SLS and LIML IV estimators
 """
 from numpy import (arange, argsort, asarray, ceil, cos, empty, int64, ones, pi,
-                   r_, sin, sum, unique, where, zeros)
+                   r_, sin, sum as npsum, unique, where, zeros)
 from numpy.linalg import inv, pinv
 
 CLUSTER_ERR = """
 clusters has the wrong nobs. Expected {0}, got {1}.  Any missing observation
 in the regression variables have have been dropped.  When using a clustered
 covariance estimator, drop missing data before estimating the model. The model
 property `notnull` contains the locations of the observations that have no
@@ -217,15 +217,15 @@
     else:
         raise ValueError('Unknown kernel: {0}'.format(kernel))
     sigma = empty(m_star + 1)
     sigma[0] = x.T @ x / t
     for i in range(1, m_star + 1):
         sigma[i] = x[i:].T @ x[:-i] / t
     s0 = sigma[0] + 2 * sigma[1:].sum()
-    sq = 2 * sum(sigma[1:] * arange(1, m_star + 1) ** q)
+    sq = 2 * npsum(sigma[1:] * arange(1, m_star + 1) ** q)
     rate = 1 / (2 * q + 1)
     gamma = c * ((sq / s0) ** 2) ** rate
     m = gamma * t ** rate
     return min(int(ceil(m)), t - 1)
 
 
 KERNEL_LOOKUP = {'bartlett': kernel_weight_bartlett,
@@ -310,15 +310,15 @@
                self.__class__.__name__ + \
                ', id: {0}'.format(hex(id(self)))
 
     @property
     def s(self):
         """Score covariance estimate"""
         x, z, eps = self.x, self.z, self.eps
-        nobs, nvar = x.shape
+        nobs = x.shape[0]
         s2 = eps.T @ eps / nobs
         pinvz = self._pinvz
         v = (x.T @ z) @ (pinvz @ x) / nobs
         if self._kappa != 1:
             kappa = self._kappa
             xpx = x.T @ x / nobs
             v = (1 - kappa) * xpx + kappa * v
@@ -344,15 +344,15 @@
         return (c + c.T) / 2
 
     @property
     def s2(self):
         """
         Estimated variance of residuals. Small-sample adjusted if debiased.
         """
-        nobs, nvar = self.x.shape
+        nobs = self.x.shape[0]
         eps = self.eps
 
         return self._scale * eps.T @ eps / nobs
 
     @property
     def debiased(self):
         """Flag indicating if covariance is debiased"""
```

### Comparing `linearmodels-4.8/linearmodels/iv/model.py` & `linearmodels-4.9/linearmodels/iv/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
                                         KernelCovariance)
 from linearmodels.iv.data import IVData
 from linearmodels.iv.gmm import (HeteroskedasticWeightMatrix,
                                  HomoskedasticWeightMatrix, IVGMMCovariance,
                                  KernelWeightMatrix,
                                  OneWayClusteredWeightMatrix)
 from linearmodels.iv.results import IVGMMResults, IVResults, OLSResults
+from linearmodels.typing import Numeric, OptionalNumeric
+from linearmodels.typing.iv import ArrayLike, OptionalArrayLike
 from linearmodels.utility import (WaldTestStatistic, has_constant, inv_sqrth,
                                   missing_warning)
 
 __all__ = ['COVARIANCE_ESTIMATORS', 'WEIGHT_MATRICES', 'IVGMM', 'IVLIML', 'IV2SLS',
            'IVGMMCUE', '_OLS']
 
 COVARIANCE_ESTIMATORS = {'homoskedastic': HomoskedasticCovariance,
@@ -101,19 +103,21 @@
       * VCV: bootstrap
 
     See Also
     --------
     IV2SLS, IVGMM, IVGMMCUE
     """
 
-    def __init__(self, dependent, exog, endog, instruments, *, weights=None,
-                 fuller=0, kappa=None):
+    def __init__(self, dependent: ArrayLike, exog: OptionalArrayLike,
+                 endog: OptionalArrayLike, instruments: OptionalArrayLike, *,
+                 weights: OptionalArrayLike = None, fuller: Numeric = 0,
+                 kappa: OptionalNumeric = None):
 
         self.dependent = IVData(dependent, var_name='dependent')
-        nobs = self.dependent.shape[0]
+        nobs = self.dependent.shape[0]  # type: int
         self.exog = IVData(exog, var_name='exog', nobs=nobs)
         self.endog = IVData(endog, var_name='endog', nobs=nobs)
         self.instruments = IVData(instruments, var_name='instruments', nobs=nobs)
         self._original_index = self.dependent.pandas.index
         if weights is None:
             weights = ones(self.dependent.shape)
         weights = IVData(weights).ndarray
@@ -488,15 +492,15 @@
                                      name=name)
         else:
             wald = WaldTestStatistic(test_stat, null, df, name=name)
 
         return wald
 
     def _post_estimation(self, params, cov_estimator, cov_type):
-        vars = self._columns
+        columns = self._columns
         index = self._index
         eps = self.resids(params)
         y = self.dependent.pandas
         fitted = DataFrame(y.values - eps, y.index, ['fitted_values'])
         weps = self.wresids(params)
         cov = cov_estimator.cov
         debiased = cov_estimator.debiased
@@ -508,25 +512,25 @@
         if self.has_constant:
             e = e - sqrt(self.weights.ndarray) * average(self._y, weights=w)
 
         total_ss = float(e.T @ e)
         r2 = 1 - residual_ss / total_ss
 
         fstat = self._f_statistic(params, cov, debiased)
-        out = {'params': Series(params.squeeze(), vars, name='parameter'),
+        out = {'params': Series(params.squeeze(), columns, name='parameter'),
                'eps': Series(eps.squeeze(), index=index, name='residual'),
                'weps': Series(weps.squeeze(), index=index, name='weighted residual'),
-               'cov': DataFrame(cov, columns=vars, index=vars),
+               'cov': DataFrame(cov, columns=columns, index=columns),
                's2': float(cov_estimator.s2),
                'debiased': debiased,
                'residual_ss': float(residual_ss),
                'total_ss': float(total_ss),
                'r2': float(r2),
                'fstat': fstat,
-               'vars': vars,
+               'vars': columns,
                'instruments': self._instr_columns,
                'cov_config': cov_estimator.config,
                'cov_type': cov_type,
                'method': self._method,
                'cov_estimator': cov_estimator,
                'fitted': fitted,
                'original_index': self._original_index}
@@ -569,15 +573,17 @@
       * VCV: bootstrap
 
     See Also
     --------
     IVLIML, IVGMM, IVGMMCUE
     """
 
-    def __init__(self, dependent, exog, endog, instruments, *, weights=None):
+    def __init__(self, dependent: ArrayLike, exog: OptionalArrayLike,
+                 endog: OptionalArrayLike, instruments: OptionalArrayLike, *,
+                 weights: OptionalArrayLike = None):
         self._method = 'IV-2SLS'
         super(IV2SLS, self).__init__(dependent, exog, endog, instruments,
                                      weights=weights, fuller=0, kappa=1)
 
     @staticmethod
     def from_formula(formula, data, *, weights=None):
         """
@@ -671,16 +677,18 @@
       * VCV: bootstrap
 
     See Also
     --------
     IV2SLS, IVLIML, IVGMMCUE
     """
 
-    def __init__(self, dependent, exog, endog, instruments, *, weights=None,
-                 weight_type='robust', **weight_config):
+    def __init__(self, dependent: ArrayLike, exog: OptionalArrayLike,
+                 endog: OptionalArrayLike, instruments: OptionalArrayLike, *,
+                 weights: OptionalArrayLike = None,
+                 weight_type: str = 'robust', **weight_config):
         self._method = 'IV-GMM'
         self._result_container = IVGMMResults
         super(IVGMM, self).__init__(dependent, exog, endog, instruments, weights=weights)
         weight_matrix_estimator = WEIGHT_MATRICES[weight_type]
         self._weight = weight_matrix_estimator(**weight_config)
         self._weight_type = weight_type
         self._weight_config = self._weight.config
@@ -910,16 +918,18 @@
     through :math:`\epsilon_i = y_i - x_i\beta`.
 
     See Also
     --------
     IV2SLS, IVLIML, IVGMM
     """
 
-    def __init__(self, dependent, exog, endog, instruments, *, weights=None,
-                 weight_type='robust', **weight_config):
+    def __init__(self, dependent: ArrayLike, exog: OptionalArrayLike,
+                 endog: OptionalArrayLike, instruments: OptionalArrayLike, *,
+                 weights: OptionalArrayLike = None,
+                 weight_type: str = 'robust', **weight_config):
         self._method = 'IV-GMM-CUE'
         super(IVGMMCUE, self).__init__(dependent, exog, endog, instruments, weights=weights,
                                        weight_type=weight_type, **weight_config)
         if 'center' not in weight_config:
             weight_config['center'] = True
 
     @staticmethod
@@ -1013,28 +1023,31 @@
         nobs = y.shape[0]
         weight_matrix = self._weight.weight_matrix
         eps = y - x @ params[:, None]
         w = inv(weight_matrix(x, z, eps))
         g_bar = (z * eps).mean(0)
         return nobs * g_bar.T @ w @ g_bar.T
 
-    def estimate_parameters(self, starting, x, y, z, display=False):
+    def estimate_parameters(self, starting, x, y, z, display=False, opt_options=None):
         r"""
         Parameters
         ----------
         starting : ndarray
             Starting values for the optimization
         x : ndarray
             Regressor matrix (nobs by nvar)
         y : ndarray
             Regressand matrix (nobs by 1)
         z : ndarray
             Instrument matrix (nobs by ninstr)
         display : bool
             Flag indicating whether to display iterative optimizer output
+        opt_options : dict, optional
+            Dictionary containing additional keyword arguments to pass to
+            scipy.optimize.minimize.
 
         Returns
         -------
         params : ndarray
             Estimated parameters (nvar by 1)
 
         Notes
@@ -1043,31 +1056,42 @@
         samples.  Performs no error checking.
 
         See Also
         --------
         scipy.optimize.minimize
         """
         args = (x, y, z)
-        res = minimize(self.j, starting, args=args, options={'disp': display})
+        opt_options = {} if opt_options is None else opt_options
+        options = {'disp': display}
+        if 'options' in opt_options:
+            opt_options = opt_options.copy()
+            options.update(opt_options.pop('options'))
+
+        res = minimize(self.j, starting, args=args, options=options, **opt_options)
 
         return res.x[:, None], res.nit
 
-    def fit(self, *, starting=None, display=False, cov_type='robust', **cov_config):
+    def fit(self, *, starting=None, display=False, cov_type='robust', opt_options=None,
+            **cov_config):
         r"""
         Estimate model parameters
 
         Parameters
         ----------
         starting : ndarray, optional
             Starting values to use in optimization.  If not provided, 2SLS
             estimates are used.
         display : bool, optional
             Flag indicating whether to display optimization output
         cov_type : str, optional
             Name of covariance estimator to use
+        opt_options : dict, optional
+            Additional options to pass to scipy.optimize.minimize when
+            optimizing the objective function. If not provided, defers to
+            scipy to choose an appropriate optimizer.
         **cov_config
             Additional parameters to pass to covariance estimator
 
         Returns
         -------
         results : IVGMMResults
             Results container
@@ -1076,18 +1100,14 @@
         -----
         Additional covariance parameters depend on specific covariance used.
         The see the docstring of specific covariance estimator for a list of
         supported options. Defaults are used if no covariance configuration
         is provided.
 
         Starting values are computed by IVGMM.
-
-        .. todo::
-
-          * Expose method to pass optimization options
         """
 
         wy, wx, wz = self._wy, self._wx, self._wz
         weight_matrix = self._weight.weight_matrix
         if starting is None:
             exog = None if self.exog.shape[1] == 0 else self.exog
             endog = None if self.endog.shape[1] == 0 else self.endog
@@ -1099,15 +1119,16 @@
                         **self._weight_config).fit()
             starting = res.params.values
         else:
             starting = asarray(starting)
             if len(starting) != self.exog.shape[1] + self.endog.shape[1]:
                 raise ValueError('starting does not have the correct number '
                                  'of values')
-        params, iters = self.estimate_parameters(starting, wx, wy, wz, display)
+        params, iters = self.estimate_parameters(starting, wx, wy, wz, display,
+                                                 opt_options=opt_options)
         eps = wy - wx @ params
         wmat = inv(weight_matrix(wx, wz, eps))
 
         cov_estimator = IVGMMCovariance(wx, wy, wz, params, wmat, cov_type,
                                         **cov_config)
         results = self._post_estimation(params, cov_estimator, cov_type)
         gmm_pe = self._gmm_post_estimation(params, wmat, iters)
@@ -1136,10 +1157,11 @@
 
     See Also
     --------
     statsmodels.regression.linear_model.OLS,
     statsmodels.regression.linear_model.GLS
     """
 
-    def __init__(self, dependent, exog, *, weights=None):
+    def __init__(self, dependent: ArrayLike, exog: OptionalArrayLike, *,
+                 weights: OptionalArrayLike = None):
         super(_OLS, self).__init__(dependent, exog, None, None, weights=weights, kappa=0.0)
         self._result_container = OLSResults
```

### Comparing `linearmodels-4.8/linearmodels/__init__.py` & `linearmodels-4.9/linearmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/conftest.py` & `linearmodels-4.9/linearmodels/conftest.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/system/gmm.py` & `linearmodels-4.9/linearmodels/system/gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/system/results.py` & `linearmodels-4.9/linearmodels/system/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime as dt
 
 import numpy as np
-from numpy import diag, sqrt
 from pandas import DataFrame, Series, concat
 from scipy import stats
 from statsmodels.iolib.summary import SimpleTable, fmt_2cols
 
 from linearmodels.compat.statsmodels import Summary
 from linearmodels.utility import (AttrDict, _SummaryStr, _str, cached_property, format_wide,
                                   param_table, pval_format)
@@ -72,15 +71,15 @@
     def params(self):
         """Estimated parameters"""
         return Series(self._params.squeeze(), index=self._param_names, name='params')
 
     @property
     def std_errors(self):
         """Estimated parameter standard errors"""
-        std_errors = sqrt(diag(self.cov))
+        std_errors = np.sqrt(np.diag(self.cov))
         return Series(std_errors, index=self._param_names, name='stderr')
 
     @property
     def tstats(self):
         """Parameter t-statistics"""
         return Series(self.params / self.std_errors, name='tstat')
 
@@ -233,15 +232,15 @@
             Dictionary-like structure containing exogenous and endogenous
             variables.  Each key is an equations label and must
             match the labels used to fir the model. Each value must be either a tuple
             of the form (exog, endog) or a dictionary with keys 'exog' and 'endog'.
             If predictions are not required for one of more of the model equations,
             these keys can be omitted.
         data : DataFrame
-            Dataframe to use for out-of-sample predictions when model was
+            DataFrame to use for out-of-sample predictions when model was
             constructed using a formula.
         fitted : bool, optional
             Flag indicating whether to include the fitted values
         idiosyncratic : bool, optional
             Flag indicating whether to include the estimated idiosyncratic shock
         missing : bool, optional
             Flag indicating to adjust for dropped observations.  if True, the
@@ -311,15 +310,20 @@
     @property
     def sigma(self):
         """Estimated residual covariance"""
         return self._sigma
 
     @property
     def summary(self):
-        """Model summary"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
+
         title = 'System ' + self._method + ' Estimation Summary'
 
         top_left = [('Estimator:', self._method),
                     ('No. Equations.:', str(len(self.equation_labels))),
                     ('No. Observations:', str(self.resids.shape[0])),
                     ('Date:', self._datetime.strftime('%a, %b %d %Y')),
                     ('Time:', self._datetime.strftime('%H:%M:%S')),
@@ -414,15 +418,20 @@
     @property
     def instruments(self):
         """Instruments used in estimation.  None if all variables assumed exogenous."""
         return self._instruments
 
     @property
     def summary(self):
-        """Equation summary"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
+
         title = self._method + ' Estimation Summary'
 
         top_left = [('Eq. Label:', self.equation_label),
                     ('Dep. Variable:', self.dependent),
                     ('Estimator:', self._method),
                     ('No. Observations:', self.nobs),
                     ('Date:', self._datetime.strftime('%a, %b %d %Y')),
```

### Comparing `linearmodels-4.8/linearmodels/system/_utility.py` & `linearmodels-4.9/linearmodels/system/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/system/covariance.py` & `linearmodels-4.9/linearmodels/system/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,19 +223,19 @@
 
     def _gls_cov(self):
         return self._cov(True)
 
     def _adjustment(self):
         if not self._debiased:
             return 1.0
-        k = list(map(lambda s: s.shape[1], self._x))
+        ks = list(map(lambda s: s.shape[1], self._x))
         nobs = self._x[0].shape[0]
         adj = []
-        for i in range(len(k)):
-            adj.append(nobs / (nobs - k[i]) * ones((k[i], 1)))
+        for k in ks:
+            adj.append(nobs / (nobs - k) * ones((k, 1)))
         adj = vstack(adj)
         adj = sqrt(adj)
         return adj @ adj.T
 
 
 class KernelCovariance(HeteroskedasticCovariance, _HACMixin):
     r"""
```

### Comparing `linearmodels-4.8/linearmodels/system/model.py` & `linearmodels-4.9/linearmodels/system/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                         weight_dict[key] = weights[key]
                     else:
                         weight_dict[key] = None
                 cln_fromula[key] = f
         else:
             formula = formula.replace('\n', ' ').strip()
             parts = formula.split('}')
-            for i, part in enumerate(parts):
+            for part in parts:
                 base_key = None
                 part = part.strip()
                 if part == '':
                     continue
                 part = part.replace('{', '')
                 if ':' in part.split('~')[0]:
                     base_key, part = part.split(':')
@@ -277,15 +277,15 @@
         'exog', 'endog', 'instruments', and 'weights'. 'exog' can be omitted
         if all variables in an equation are endogenous. Alternatively, 'exog'
         can contain either an empty array or `None` to indicate that an
         equation contains no exogenous regressors. Similarly 'endog' and
         'instruments' can either be omitted or may contain an empty array (or
         `None`) if all variables in an equation are exogenous.
     sigma : array-like
-        Pre-specified residual covariance to use in GLS estimation. If not
+        Prespecified residual covariance to use in GLS estimation. If not
         provided, FGLS is implemented based on an estimate of sigma.
 
     Notes
     -----
     Estimates a set of regressions which are seemingly unrelated in the sense
     that separate estimation would lead to consistent parameter estimates.
     Each equation is of the form
@@ -502,15 +502,15 @@
             if z.shape[1] > z.shape[0]:
                 raise ValueError('Fewer observations than instruments in '
                                  'equation {eq}'.format(eq=label))
             if matrix_rank(z) < z.shape[1]:
                 raise ValueError('Equation {eq} instrument array is full '
                                  'rank'.format(eq=label))
 
-        for lhs, rhs, label in zip(self._y, self._x, self._eq_labels):
+        for rhs in self._x:
             const, const_loc = has_constant(rhs)
             constant.append(const)
             constant_loc.append(const_loc)
         self._has_constant = Series(constant,
                                     index=[d.cols[0] for d in self._dependent])
         self._constant_loc = constant_loc
 
@@ -829,15 +829,15 @@
         Parameters
         ----------
         dependent : array-like
             nobs by ndep array of dependent variables
         exog : array-like, optional
             nobs by nexog array of exogenous regressors common to all models
         endog : array-like, optional
-            nobs by nengod array of endogenous regressors common to all models
+            nobs by nendog array of endogenous regressors common to all models
         instruments : array-like, optional
             nobs by ninstr array of instruments to use in all equations
 
         Returns
         -------
         model : IV3SLS
             Model instance
@@ -872,15 +872,15 @@
         formula : {str, dict-like}
             Either a string or a dictionary of strings where each value in
             the dictionary represents a single equation. See Notes for a
             description of the accepted syntax
         data : DataFrame
             Frame containing named variables
         sigma : array-like
-            Pre-specified residual covariance to use in GLS estimation. If
+            Prespecified residual covariance to use in GLS estimation. If
             not provided, FGLS is implemented based on an estimate of sigma.
         weights : dict-like
             Dictionary like object (e.g. a DataFrame) containing variable
             weights.  Each entry must have the same number of observations as
             data.  If an equation label is not a key weights, the weights will
             be set to unity
 
@@ -1173,15 +1173,15 @@
     equations : dict
         Dictionary-like structure containing dependent and exogenous variable
         values.  Each key is an equations label and must be a string. Each
         value must be either a tuple of the form (dependent,
         exog, [weights]) or a dictionary with keys 'dependent' and 'exog' and
         the optional key 'weights'.
     sigma : array-like
-        Pre-specified residual covariance to use in GLS estimation. If not
+        Prespecified residual covariance to use in GLS estimation. If not
         provided, FGLS is implemented based on an estimate of sigma.
 
     Notes
     -----
     Estimates a set of regressions which are seemingly unrelated in the sense
     that separate estimation would lead to consistent parameter estimates.
     Each equation is of the form
@@ -1313,15 +1313,15 @@
         formula : {str, dict-like}
             Either a string or a dictionary of strings where each value in
             the dictionary represents a single equation. See Notes for a
             description of the accepted syntax
         data : DataFrame
             Frame containing named variables
         sigma : array-like
-            Pre-specified residual covariance to use in GLS estimation. If
+            Prespecified residual covariance to use in GLS estimation. If
             not provided, FGLS is implemented based on an estimate of sigma.
         weights : dict-like
             Dictionary like object (e.g. a DataFrame) containing variable
             weights.  Each entry must have the same number of observations as
             data.  If an equation label is not a key weights, the weights will
             be set to unity
 
@@ -1376,15 +1376,15 @@
         and instrumental variables.  Each key is an equations label and must
         be a string. Each value must be either a tuple of the form (dependent,
         exog, endog, instrument[, weights]) or a dictionary with keys 'dependent',
         'exog'.  The dictionary may contain optional keys for 'endog',
         'instruments', and 'weights'. Endogenous and/or Instrument can be empty
         if all variables in an equation are exogenous.
     sigma : array-like
-        Pre-specified residual covariance to use in GLS estimation. If not
+        Prespecified residual covariance to use in GLS estimation. If not
         provided, FGLS is implemented based on an estimate of sigma. Only used
         if weight_type is 'unadjusted'
     weight_type : str
         Name of moment condition weight function to use in the GMM estimation
     **weight_config
         Additional keyword arguments to pass to the moment condition weight
         function
```

### Comparing `linearmodels-4.8/linearmodels/tests/test_utility.py` & `linearmodels-4.9/linearmodels/tests/test_utility.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import random
+import string
 import warnings
 
 import numpy as np
 import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
 from scipy import stats
 
 import linearmodels
 from linearmodels.utility import (AttrDict, InapplicableTestStatistic, InvalidTestStatistic,
                                   WaldTestStatistic, cached_property, ensure_unique_column,
-                                  format_wide, has_constant, inv_sqrth, missing_warning)
+                                  format_wide, has_constant, inv_sqrth, missing_warning,
+                                  panel_to_frame)
+
+MISSING_PANEL = 'Panel' not in dir(pd)
 
 
 def test_missing_warning():
     missing = np.zeros(500, dtype=np.bool)
     with warnings.catch_warnings(record=True) as w:
         missing_warning(missing)
         assert len(w) == 0
@@ -198,7 +203,28 @@
 
 
 def test_format_wide():
     k = 26
     inputs = [chr(65 + i) * (20 + i) for i in range(k)]
     out = format_wide(inputs, 80)
     assert max(map(lambda v: len(v), out)) <= 80
+
+
+@pytest.mark.skipif(MISSING_PANEL, reason='pd.Panel is not installed')
+@pytest.mark.filterwarnings('ignore::FutureWarning')
+def test_panel_to_midf():
+    x = np.random.standard_normal((3, 7, 100))
+    expected = pd.Panel(x).to_frame()
+    df = panel_to_frame(x, list(range(3)), list(range(7)), list(range(100)))
+    pd.testing.assert_frame_equal(df, expected)
+
+    expected = pd.Panel(x).swapaxes(1, 2).to_frame(filter_observations=False)
+    df = panel_to_frame(x, list(range(3)), list(range(7)), list(range(100)), True)
+    pd.testing.assert_frame_equal(df, expected)
+    entities = list(map(''.join, [[random.choice(string.ascii_lowercase) for __ in range(10)]
+                                  for _ in range(100)]))
+    times = pd.date_range('1999-12-31', freq='A-DEC', periods=7)
+    var_names = ['x.{0}'.format(i) for i in range(1, 4)]
+    expected = pd.Panel(x, items=var_names, major_axis=times, minor_axis=entities)
+    expected = expected.swapaxes(1, 2).to_frame(filter_observations=False)
+    df = panel_to_frame(x, var_names, times, entities, True)
+    pd.testing.assert_frame_equal(df, expected)
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_simulated_against_stata.py` & `linearmodels-4.9/linearmodels/tests/panel/test_simulated_against_stata.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from linearmodels.panel.data import PanelData
 from linearmodels.panel.model import (BetweenOLS, PanelOLS, PooledOLS,
                                       RandomEffects)
 from linearmodels.tests.panel.results import parse_stata_results
 from linearmodels.utility import AttrDict
 
-pytestmark = pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
+pytestmark = pytest.mark.filterwarnings(
+    'ignore::linearmodels.utility.MissingValueWarning')
 
 STATA_RESULTS = parse_stata_results.data()
 MODELS = {'between': BetweenOLS, 'fixed_effect': PanelOLS, 'pooled': PooledOLS,
           'random_effect': RandomEffects}
 cwd = os.path.split(os.path.abspath(__file__))[0]
 sim_data = pd.read_stata(os.path.join(cwd, 'results', 'simulated-panel.dta'))
 sim_data = sim_data.set_index(['firm', 'time'])
@@ -51,34 +52,52 @@
         y_data = PanelData(y)
         eid = y_data.entity_ids
         entities = pd.DataFrame(eid, index=y_data.index, columns=['firm_ids'])
         fit_options.update({'cov_type': 'clustered', 'clusters': entities})
     else:
         fit_options.update({'cov_type': 'unadjusted'})
 
-    if vcv == 'cluster' or (model in ('fixed_effect', 'random_effect') and vcv == 'robust'):
+    if vcv == 'cluster' or (
+            model in ('fixed_effect', 'random_effect') and vcv == 'robust'):
         fit_options.update({'group_debias': True})
     spec_mod = mod(y, x, **mod_options)
     fit = spec_mod.fit(**fit_options)
-    return AttrDict(fit=fit, model=spec_mod, model_options=mod_options, y=y, x=x,
-                    stata=STATA_RESULTS[request.param], fit_options=fit_options,
-                    model_name=model, vcv=vcv, weights=weights, missing=missing)
+    return AttrDict(fit=fit, model=spec_mod, model_options=mod_options, y=y,
+                    x=x,
+                    stata=STATA_RESULTS[request.param],
+                    fit_options=fit_options,
+                    model_name=model, vcv=vcv, weights=weights,
+                    missing=missing)
 
 
 # TODO: pvals, r2o, r2
+def correct_order(stata, lm):
+    repl = []
+    for c in stata.index:
+        if c == '_cons':
+            repl.append('intercept')
+        else:
+            repl.append(c)
+    stata = stata.copy()
+    stata.index = repl
+    index = lm.index
+
+    return stata.reindex(index)
 
 
 def test_params(data):
-    model_params = data.fit
-    stata_params = data.stata.params.param
-    assert_allclose(stata_params.values, model_params.params.squeeze())
+    model_params = data.fit.params
+    stata = data.stata.params
+    stata = correct_order(stata, model_params)
+    assert_allclose(stata.param, model_params)
 
 
 def test_rsquared_between(data):
-    if data.weights in ('weighted', 'wls') or data.missing in ('_heavy', '_light'):
+    if (data.weights in ('weighted', 'wls') or
+            data.missing in ('_heavy', '_light')):
         pytest.xfail(reason='Respect weights in calculation')
     r2_between = data.fit.rsquared_between
     if np.isnan(data.stata.r2_b):
         return
     assert_allclose(r2_between, data.stata.r2_b, rtol=1e-3)
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_panel_covariance.py` & `linearmodels-4.9/linearmodels/tests/panel/test_panel_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/_utility.py` & `linearmodels-4.9/linearmodels/tests/panel/_utility.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import numpy as np
-import pandas as pd
 from numpy.random import standard_normal
 from numpy.testing import assert_allclose
+from pandas import DataFrame, Categorical, get_dummies, date_range
+from pandas.testing import assert_frame_equal, assert_series_equal
 
 from linearmodels.compat.numpy import lstsq
+from linearmodels.panel.data import PanelData
+from linearmodels.utility import panel_to_frame
 
 try:
     import xarray  # flake8: noqa
 
     MISSING_XARRAY = False
 except ImportError:
     MISSING_XARRAY = True
-from linearmodels.compat.pandas import assert_frame_equal, assert_series_equal
 from linearmodels.utility import AttrDict
 
 datatypes = ['numpy', 'pandas']
 if not MISSING_XARRAY:
     datatypes += ['xarray']
 
 
-def lsdv(y: pd.DataFrame, x: pd.DataFrame, has_const=False, entity=False, time=False,
+def lsdv(y: DataFrame, x: DataFrame, has_const=False, entity=False, time=False,
          general=None):
     nvar = x.shape[1]
     temp = x.reset_index()
     cat_index = temp.index
     if entity:
-        cat = pd.Categorical(temp.iloc[:, 0])
+        cat = Categorical(temp.iloc[:, 0])
         cat.index = cat_index
-        dummies = pd.get_dummies(cat, drop_first=has_const)
-        x = pd.DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
+        dummies = get_dummies(cat, drop_first=has_const)
+        x = DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
                          index=x.index,
                          columns=list(x.columns) + list(dummies.columns))
     if time:
-        cat = pd.Categorical(temp.iloc[:, 1])
+        cat = Categorical(temp.iloc[:, 1])
         cat.index = cat_index
-        dummies = pd.get_dummies(cat, drop_first=(has_const or entity))
-        x = pd.DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
+        dummies = get_dummies(cat, drop_first=(has_const or entity))
+        x = DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
                          index=x.index,
                          columns=list(x.columns) + list(dummies.columns))
     if general is not None:
-        cat = pd.Categorical(general)
+        cat = Categorical(general)
         cat.index = cat_index
-        dummies = pd.get_dummies(cat, drop_first=(has_const or entity or time))
-        x = pd.DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
+        dummies = get_dummies(cat, drop_first=(has_const or entity or time))
+        x = DataFrame(np.c_[x.values, dummies.values.astype(np.float64)],
                          index=x.index,
                          columns=list(x.columns) + list(dummies.columns))
     w = np.ones_like(y)
 
     wy = w * y.values
     wx = w * x.values
     params = lstsq(wx, wy)[0]
@@ -86,31 +88,57 @@
         locs = np.random.choice(n * t, int(n * t * missing))
         y.flat[locs] = np.nan
         locs = np.random.choice(n * t * k, int(n * t * k * missing))
         x.flat[locs] = np.nan
 
     if datatype in ('pandas', 'xarray'):
         entities = ['firm' + str(i) for i in range(n)]
-        time = pd.date_range('1-1-1900', periods=t, freq='A-DEC')
+        time = date_range('1-1-1900', periods=t, freq='A-DEC')
         var_names = ['x' + str(i) for i in range(k)]
-        y = pd.DataFrame(y, index=time, columns=entities)
-        w = pd.DataFrame(w, index=time, columns=entities)
-        x = pd.Panel(x, items=var_names, major_axis=time, minor_axis=entities)
-        c = pd.Panel(c, items=cats, major_axis=time, minor_axis=entities)
-        vc1 = pd.Panel(vc1, items=vcats[:1], major_axis=time, minor_axis=entities)
-        vc2 = pd.Panel(vc2, items=vcats, major_axis=time, minor_axis=entities)
+        # y = DataFrame(y, index=time, columns=entities)
+        y = panel_to_frame(y[None], items=['y'], major_axis=time, minor_axis=entities, swap=True)
+        w = panel_to_frame(w[None], items=['w'], major_axis=time, minor_axis=entities, swap=True)
+        w = w.reindex(y.index)
+        x = panel_to_frame(x, items=var_names, major_axis=time, minor_axis=entities, swap=True)
+        x = x.reindex(y.index)
+        c = panel_to_frame(c, items=cats, major_axis=time, minor_axis=entities, swap=True)
+        c = c.reindex(y.index)
+        vc1 = panel_to_frame(vc1, items=vcats[:1], major_axis=time, minor_axis=entities, swap=True)
+        vc1 = vc1.reindex(y.index)
+        vc2 = panel_to_frame(vc2, items=vcats, major_axis=time, minor_axis=entities, swap=True)
+        vc2 = vc2.reindex(y.index)
 
     if datatype == 'xarray':
+        # TODO: This is broken now, need to transfor multiindex to xarray 3d
         import xarray as xr
-        x = xr.DataArray(x)
-        y = xr.DataArray(y)
-        w = xr.DataArray(w)
-        c = xr.DataArray(c)
-        vc1 = xr.DataArray(vc1)
-        vc2 = xr.DataArray(vc2)
+        x = xr.DataArray(PanelData(x).values3d,
+                         coords={'entities': entities, 'time': time,
+                                 'vars': var_names},
+                         dims=['vars', 'time', 'entities'])
+        y = xr.DataArray(PanelData(y).values3d,
+                         coords={'entities': entities, 'time': time,
+                                 'vars': ['y']},
+                         dims=['vars', 'time', 'entities'])
+        w = xr.DataArray(PanelData(w).values3d,
+                         coords={'entities': entities, 'time': time,
+                                 'vars': ['w']},
+                         dims=['vars', 'time', 'entities'])
+        if c.shape[1] > 0:
+            c = xr.DataArray(PanelData(c).values3d,
+                             coords={'entities': entities, 'time': time,
+                                     'vars': c.columns},
+                             dims=['vars', 'time', 'entities'])
+        vc1 = xr.DataArray(PanelData(vc1).values3d,
+                           coords={'entities': entities, 'time': time,
+                                   'vars': vc1.columns},
+                           dims=['vars', 'time', 'entities'])
+        vc2 = xr.DataArray(PanelData(vc2).values3d,
+                           coords={'entities': entities, 'time': time,
+                                   'vars': vc2.columns},
+                           dims=['vars', 'time', 'entities'])
 
     if rng is not None:
         rng.set_state(np.random.get_state())
 
     return AttrDict(y=y, x=x, w=w, c=c, vc1=vc1, vc2=vc2)
 
 
@@ -120,19 +148,21 @@
     assert_series_equal(res1.params.iloc[:n], res2.params.iloc[:n])
     assert_series_equal(res1.pvalues.iloc[:n], res2.pvalues.iloc[:n])
     assert_series_equal(res1.tstats.iloc[:n], res2.tstats.iloc[:n])
     assert_frame_equal(res1.cov.iloc[:n, :n], res2.cov.iloc[:n, :n])
     assert_frame_equal(res1.conf_int().iloc[:n], res2.conf_int().iloc[:n])
     assert_allclose(res1.s2, res2.s2)
 
-    delta = 1 + (res1.resids.values - res2.resids.values) / max(res1.resids.std(),
-                                                                res2.resids.std())
+    delta = 1 + (res1.resids.values - res2.resids.values) / max(
+        res1.resids.std(),
+        res2.resids.std())
     assert_allclose(delta, np.ones_like(delta))
-    delta = 1 + (res1.wresids.values - res2.wresids.values) / max(res1.wresids.std(),
-                                                                  res2.wresids.std())
+    delta = 1 + (res1.wresids.values - res2.wresids.values) / max(
+        res1.wresids.std(),
+        res2.wresids.std())
     assert_allclose(delta, np.ones_like(delta))
 
     if test_df:
         assert_allclose(res1.df_model, res2.df_model)
         assert_allclose(res1.df_resid, res2.df_resid)
 
     if test_fit:
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_data.py` & `linearmodels-4.9/linearmodels/tests/panel/test_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from linearmodels.compat.pandas import (assert_frame_equal, assert_panel_equal,
-                                        is_string_dtype)
-
 from itertools import product
 
 import numpy as np
-import pandas as pd
 import pytest
 from numpy.linalg import pinv
 from numpy.testing import assert_allclose, assert_equal
+from pandas import DataFrame, date_range, Categorical, get_dummies, Series, datetime
+from pandas.testing import assert_frame_equal
+
+from linearmodels.compat.pandas import is_string_dtype
 
 try:
     import xarray as xr
 except ImportError:
     pass
 
 from linearmodels.compat.numpy import lstsq
 from linearmodels.panel.data import PanelData
 from linearmodels.panel.model import PanelOLS
 from linearmodels.tests.panel._utility import generate_data, datatypes, \
     MISSING_XARRAY
+from linearmodels.utility import panel_to_frame
 
 pytestmark = pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
 
 PERC_MISSING = [0, 0.02, 0.10, 0.33]
 TYPES = datatypes
 
 
@@ -31,39 +32,38 @@
                              product(PERC_MISSING, TYPES))))
 def data(request):
     missing, datatype = request.param
     return generate_data(missing, datatype, ntk=(231, 7, 5))
 
 
 @pytest.fixture
-def panel():
+def mi_df():
     np.random.seed(12345)
     n, t, k = 11, 7, 3
     x = np.random.standard_normal((k, t, n))
-    major = pd.date_range('12-31-1999', periods=7)
+    major = date_range('12-31-1999', periods=7)
     items = ['var.{0}'.format(i) for i in range(1, k + 1)]
     minor = ['entities.{0}'.format(i) for i in range(1, n + 1)]
-    return pd.Panel(x, items=items, major_axis=major, minor_axis=minor)
+    return panel_to_frame(x, items, major, minor, swap=True)
 
 
 def test_numpy_3d():
     n, t, k = 11, 7, 3
     x = np.random.random((k, t, n))
     dh = PanelData(x)
     assert_equal(x, dh.values3d)
     assert dh.nentity == n
     assert dh.nobs == t
     assert dh.nvar == k
     assert_equal(np.reshape(x.T, (n * t, k)), dh.values2d)
     items = ['entity.{0}'.format(i) for i in range(n)]
     obs = [i for i in range(t)]
     var_names = ['x.{0}'.format(i) for i in range(k)]
-    expected = pd.Panel(np.reshape(x, (k, t, n)), items=var_names,
-                        major_axis=obs, minor_axis=items)
-    expected_frame = expected.swapaxes(1, 2).to_frame()
+    expected_frame = panel_to_frame(np.reshape(x, (k, t, n)), items=var_names,
+                                    major_axis=obs, minor_axis=items, swap=True)
     expected_frame.index.levels[0].name = 'entity'
     expected_frame.index.levels[1].name = 'time'
     assert_frame_equal(dh.dataframe, expected_frame)
 
 
 def test_numpy_1d():
     n = 11
@@ -79,61 +79,40 @@
     assert dh.nentity == n
     assert dh.nobs == t
     assert dh.nvar == k
     assert_equal(np.reshape(x.T, (n * t, k)), dh.values2d)
     assert_equal(np.reshape(x, (k, t, n)), dh.values3d)
 
 
-def test_pandas_panel():
-    n, t, k = 11, 7, 3
-    x = np.random.random((k, t, n))
-    major = pd.date_range('12-31-1999', periods=7)
-    items = ['var.{0}'.format(i) for i in range(1, k + 1)]
-    minor = ['entities.{0}'.format(i) for i in range(1, n + 1)]
-    x = pd.Panel(x, items=items, major_axis=major, minor_axis=minor)
-    dh = PanelData(x)
-    assert dh.nentity == n
-    assert dh.nobs == t
-    assert dh.nvar == k
-    assert_equal(dh.values3d, x.values)
-    expected = np.reshape(x.swapaxes(0, 2).values, (n * t, k))
-    assert_equal(dh.values2d, expected)
-    expected_frame = x.swapaxes(1, 2).to_frame()
-    expected_frame.index.levels[0].name = 'entity'
-    expected_frame.index.levels[1].name = 'time'
-    assert_frame_equal(dh.dataframe, expected_frame)
-
-
 def test_pandas_multiindex_dataframe():
     n, t, k = 11, 7, 3
     x = np.random.random((n, t, k))
-    major = pd.date_range('12-31-1999', periods=7)
+    major = date_range('12-31-1999', periods=7)
     minor = ['var.{0}'.format(i) for i in range(1, k + 1)]
     items = ['item.{0}'.format(i) for i in range(1, n + 1)]
-    x = pd.Panel(x, items=items, major_axis=major, minor_axis=minor)
-    x = x.swapaxes(1, 2).swapaxes(0, 1).to_frame()
+    x = panel_to_frame(x, items=items, major_axis=major, minor_axis=minor, swap=True)
     PanelData(x)
 
 
 def test_pandas_dataframe():
     t, n = 11, 7
     x = np.random.random((t, n))
-    index = pd.date_range('12-31-1999', periods=t)
+    index = date_range('12-31-1999', periods=t)
     cols = ['entity.{0}'.format(i) for i in range(1, n + 1)]
-    x = pd.DataFrame(x, columns=cols, index=index)
+    x = DataFrame(x, columns=cols, index=index)
     PanelData(x)
 
 
 def test_existing_panel_data():
     n, t, k = 11, 7, 3
     x = np.random.random((k, t, n))
-    major = pd.date_range('12-31-1999', periods=7)
+    major = date_range('12-31-1999', periods=7)
     items = ['var.{0}'.format(i) for i in range(1, k + 1)]
     minor = ['entities.{0}'.format(i) for i in range(1, n + 1)]
-    x = pd.Panel(x, items=items, major_axis=major, minor_axis=minor)
+    x = panel_to_frame(x, items=items, major_axis=major, minor_axis=minor, swap=True)
     dh = PanelData(x)
     dh2 = PanelData(dh)
     assert_frame_equal(dh.dataframe, dh2.dataframe)
 
 
 @pytest.mark.skipif(MISSING_XARRAY, reason='xarray is not installed')
 def test_xarray_2d():
@@ -154,49 +133,52 @@
                      coords={
                          'entity': list('firm.' + str(i) for i in range(n)),
                          'var': list('x.' + str(i) for i in range(k))})
     dh = PanelData(x)
     assert_equal(np.reshape(x.values.T, (n * t, k)), dh.values2d)
 
 
-def test_dimensions(panel):
-    dh = PanelData(panel)
-    assert dh.nentity == panel.shape[2]
-    assert dh.nvar == panel.shape[0]
-    assert dh.nobs == panel.shape[1]
+def test_dimensions(mi_df):
+    dh = PanelData(mi_df)
+    assert dh.nentity == len(mi_df.index.levels[0])
+    assert dh.nvar == mi_df.shape[1]
+    assert dh.nobs == len(mi_df.index.levels[1])
 
 
-def test_drop(panel):
-    dh = PanelData(panel)
+def test_drop(mi_df):
+    dh = PanelData(mi_df)
     orig = dh.dataframe.copy()
     sel = np.zeros(orig.shape[0], dtype=np.bool)
     sel[::3] = True
     dh.drop(sel)
     assert dh.dataframe.shape[0] == len(sel) - sel.sum()
 
 
-def test_labels(panel):
-    dh = PanelData(panel)
-    assert dh.vars == list(panel.items)
-    assert dh.time == list(panel.major_axis)
-    assert dh.entities == list(panel.minor_axis)
+def test_labels(mi_df):
+    dh = PanelData(mi_df)
+    assert dh.vars == list(mi_df.columns)
+    assert dh.time == list(mi_df.index.levels[1])
+    assert dh.entities == list(mi_df.index.get_level_values(0).unique())
 
 
-def test_missing(panel):
-    panel.iloc[0, :, ::3] = np.nan
-    dh = PanelData(panel)
+def test_missing(mi_df):
+    mi_df = mi_df.copy()
+    entities = mi_df.index.levels[0]
+    for entity in entities[::3]:
+        mi_df.loc[entity] = np.nan
+    dh = PanelData(mi_df)
     assert_equal(dh.isnull, np.any(np.isnan(dh.values2d), 1))
 
 
 def test_incorrect_dataframe():
     grouped = np.array(list([i] * 10 for i in range(10))).ravel()
-    df = pd.DataFrame({'a': np.arange(100),
-                       'b': grouped,
-                       'c': np.random.permutation(grouped),
-                       'data': np.random.randn(100)})
+    df = DataFrame({'a': np.arange(100),
+                    'b': grouped,
+                    'c': np.random.permutation(grouped),
+                    'data': np.random.randn(100)})
     df = df.set_index(['a', 'b', 'c'])
     with pytest.raises(ValueError):
         PanelData(df)
 
 
 def test_incorrect_types():
     with pytest.raises(TypeError):
@@ -205,46 +187,46 @@
 
 @pytest.mark.skipif(MISSING_XARRAY, reason='xarray is not installed')
 def test_incorrect_types_xarray():
     with pytest.raises(ValueError):
         PanelData(xr.DataArray(np.random.randn(10)))
 
 
-def test_ids(panel):
-    data = PanelData(panel)
+def test_ids(mi_df):
+    data = PanelData(mi_df)
     eids = data.entity_ids
     assert eids.shape == (77, 1)
     assert len(np.unique(eids)) == 11
     for i in range(0, len(eids), 7):
         assert np.ptp(eids[i:i + 7]) == 0
         assert np.all((eids[i + 8:] - eids[i]) != 0)
 
     tids = data.time_ids
     assert tids.shape == (77, 1)
     assert len(np.unique(tids)) == 7
     for i in range(0, 11):
         assert np.ptp(tids[i::7]) == 0
 
 
-def test_str_repr(panel):
-    data = PanelData(panel)
+def test_str_repr(mi_df):
+    data = PanelData(mi_df)
     assert 'PanelData' in str(data)
     assert str(hex(id(data))) in data.__repr__()
 
 
-def test_demean(panel):
-    data = PanelData(panel)
+def test_demean(mi_df):
+    data = PanelData(mi_df)
     fe = data.demean('entity')
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         expected[i] -= expected[i].mean(0)
     assert_allclose(fe.values3d, expected)
 
     te = data.demean('time')
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         expected[i] -= expected[i].mean(1)[:, None]
     assert_allclose(te.values3d, expected)
 
 
 def test_demean_against_groupby(data):
     dh = PanelData(data.x)
@@ -265,125 +247,142 @@
 def test_demean_against_dummy_regression(data):
     dh = PanelData(data.x)
     dh.drop(dh.isnull)
 
     df = dh.dataframe
     no_index = df.reset_index()
 
-    cat = pd.Categorical(no_index[df.index.levels[0].name])
-    d = pd.get_dummies(cat, drop_first=False).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[0].name])
+    d = get_dummies(cat, drop_first=False).astype(np.float64)
     dummy_demeaned = df.values - d @ lstsq(d, df.values)[0]
     entity_demean = dh.demean('entity')
     assert_allclose(1 + np.abs(entity_demean.values2d),
                     1 + np.abs(dummy_demeaned))
 
-    cat = pd.Categorical(no_index[df.index.levels[1].name])
-    d = pd.get_dummies(cat, drop_first=False).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[1].name])
+    d = get_dummies(cat, drop_first=False).astype(np.float64)
     dummy_demeaned = df.values - d @ lstsq(d, df.values)[0]
     time_demean = dh.demean('time')
     assert_allclose(1 + np.abs(time_demean.values2d),
                     1 + np.abs(dummy_demeaned))
 
-    cat = pd.Categorical(no_index[df.index.levels[0].name])
-    d1 = pd.get_dummies(cat, drop_first=False).astype(np.float64)
-    cat = pd.Categorical(no_index[df.index.levels[1].name])
-    d2 = pd.get_dummies(cat, drop_first=True).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[0].name])
+    d1 = get_dummies(cat, drop_first=False).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[1].name])
+    d2 = get_dummies(cat, drop_first=True).astype(np.float64)
     d = np.c_[d1.values, d2.values]
     dummy_demeaned = df.values - d @ lstsq(d, df.values)[0]
     both_demean = dh.demean('both')
     assert_allclose(1 + np.abs(both_demean.values2d),
                     1 + np.abs(dummy_demeaned))
 
 
-def test_demean_missing(panel):
-    panel.values.flat[::13] = np.nan
-    data = PanelData(panel)
+def test_demean_missing(mi_df):
+    mi_df.values.flat[::13] = np.nan
+    data = PanelData(mi_df)
     fe = data.demean('entity')
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         expected[i] -= np.nanmean(expected[i], 0)
     assert_allclose(fe.values3d, expected)
 
     te = data.demean('time')
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         expected[i] -= np.nanmean(expected[i], 1)[:, None]
     assert_allclose(te.values3d, expected)
 
 
-def test_demean_many_missing(panel):
-    panel.iloc[0, ::3] = np.nan
-    panel.iloc[0, :, ::3] = np.nan
-    panel.iloc[1, ::5] = np.nan
-    panel.iloc[1, :, ::5] = np.nan
-    panel.iloc[2, ::2] = np.nan
-    panel.iloc[2, :, ::2] = np.nan
-    data = PanelData(panel)
+def test_demean_many_missing(mi_df):
+    entities = mi_df.index.levels[0]
+    times = mi_df.index.levels[1]
+    skips = (3, 5, 2)
+    for column, skip in zip(mi_df, skips):
+        for entity in entities[::skip]:
+            mi_df.loc[entity, column] = np.nan
+        mi_df.index = mi_df.index.swaplevel()
+        for time in times[::skip]:
+            mi_df.loc[time, column] = np.nan
+        mi_df.index = mi_df.index.swaplevel()
+    data = PanelData(mi_df)
     fe = data.demean('entity')
-    orig_nan = np.isnan(panel.values.ravel())
+    orig_nan = np.isnan(data.values3d.ravel())
     fe_nan = np.isnan(fe.values3d.ravel())
     assert np.all(fe_nan[orig_nan])
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         mu = np.ones(expected[i].shape[1]) * np.nan
         for j in range(expected[i].shape[1]):
             if np.any(np.isfinite(expected[i][:, j])):
                 mu[j] = np.nanmean(expected[i][:, j])
         expected[i] -= mu
     assert_allclose(fe.values3d, expected)
 
     te = data.demean('time')
-    expected = panel.values.copy()
+    expected = data.values3d.copy()
     for i in range(3):
         mu = np.ones((expected[i].shape[0], 1)) * np.nan
         for j in range(expected[i].shape[0]):
             if np.any(np.isfinite(expected[i][j])):
                 mu[j, 0] = np.nanmean(expected[i][j])
         expected[i] -= mu
     assert_allclose(te.values3d, expected)
 
 
-def test_demean_many_missing_dropped(panel):
-    panel.iloc[0, ::3, ::3] = np.nan
-    data = PanelData(panel)
+def test_demean_many_missing_dropped(mi_df):
+    entities = mi_df.index.levels[0]
+    times = mi_df.index.levels[1]
+    column = mi_df.columns[0]
+    for entity in entities[::3]:
+        mi_df.loc[entity, column] = np.nan
+    mi_df.index = mi_df.index.swaplevel()
+    for time in times[::3]:
+        mi_df.loc[time, column] = np.nan
+    mi_df.index = mi_df.index.swaplevel()
+
+    data = PanelData(mi_df)
     data.drop(data.isnull)
     fe = data.demean('entity')
 
     expected = data.values2d.copy()
     eid = data.entity_ids.ravel()
     for i in np.unique(eid):
         expected[eid == i] -= np.nanmean(expected[eid == i], 0)
 
     assert_allclose(fe.values2d, expected)
 
 
 def test_demean_both_large_t():
-    data = PanelData(pd.Panel(np.random.standard_normal((1, 100, 10))))
+    x = np.random.standard_normal((1, 100, 10))
+    time = date_range('1-1-2000', periods=100)
+    entities = ['entity.{0}'.format(i) for i in range(10)]
+    data = panel_to_frame(x, ['x'], time, entities, swap=True)
+    data = PanelData(data)
     demeaned = data.demean('both')
 
     df = data.dataframe
     no_index = df.reset_index()
-    cat = pd.Categorical(no_index[df.index.levels[0].name])
-    d1 = pd.get_dummies(cat, drop_first=False).astype(np.float64)
-    cat = pd.Categorical(no_index[df.index.levels[1].name])
-    d2 = pd.get_dummies(cat, drop_first=True).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[0].name])
+    d1 = get_dummies(cat, drop_first=False).astype(np.float64)
+    cat = Categorical(no_index[df.index.levels[1].name])
+    d2 = get_dummies(cat, drop_first=True).astype(np.float64)
     d = np.c_[d1.values, d2.values]
     dummy_demeaned = df.values - d @ pinv(d) @ df.values
     assert_allclose(1 + np.abs(demeaned.values2d),
                     1 + np.abs(dummy_demeaned))
 
 
-def test_demean_invalid(panel):
-    data = PanelData(panel)
+def test_demean_invalid(mi_df):
+    data = PanelData(mi_df)
     with pytest.raises(ValueError):
         data.demean('unknown')
 
 
-def test_dummies(panel):
-    data = PanelData(panel)
+def test_dummies(mi_df):
+    data = PanelData(mi_df)
     edummy = data.dummies()
     assert edummy.shape == (77, 11)
     assert np.all(edummy.sum(0) == 7)
     tdummy = data.dummies(group='time')
     assert tdummy.shape == (77, 7)
     assert np.all(tdummy.sum(0) == 11)
     tdummy_drop = data.dummies(group='time', drop_first=True)
@@ -393,40 +392,47 @@
         data.dummies('unknown')
 
 
 def test_roundtrip_3d(data):
     x = data.x
     xpd = PanelData(x)
     xv = x if isinstance(x, np.ndarray) else x.values
-    assert_equal(xpd.values3d, xv)
+    if isinstance(x, DataFrame):
+        assert_equal(xpd.values2d, xv)
+    else:
+        assert_equal(xpd.values3d, xv)
 
 
-def test_series_multiindex(panel):
-    mi = panel.swapaxes(1, 2).to_frame(filter_observations=False)
-    from_df = PanelData(mi.iloc[:, [0]])
-    from_series = PanelData(mi.iloc[:, 0])
+def test_series_multiindex(mi_df):
+    from_df = PanelData(mi_df.iloc[:, [0]])
+    from_series = PanelData(mi_df.iloc[:, 0])
     assert_frame_equal(from_df.dataframe, from_series.dataframe)
 
 
-def test_invalid_seires(panel):
-    si = panel.to_frame().reset_index()
+def test_invalid_seires(mi_df):
+    si = mi_df.reset_index()
     with pytest.raises(ValueError):
         PanelData(si.iloc[:, 0])
 
 
 def test_demean_missing_alt_types(data):
+    check = isinstance(data.x, (DataFrame, np.ndarray))
     xpd = PanelData(data.x)
     xpd.drop(xpd.isnull)
     entity_demean = xpd.demean('entity')
     expected = xpd.dataframe.groupby(level=0).transform(lambda s: s - s.mean())
-    assert_frame_equal(entity_demean.dataframe, expected)
+    assert_frame_equal(entity_demean.dataframe, expected,
+                       check_index_type=check,
+                       check_column_type=check)
 
     time_demean = xpd.demean('time')
     expected = xpd.dataframe.groupby(level=1).transform(lambda s: s - s.mean())
-    assert_frame_equal(time_demean.dataframe, expected)
+    assert_frame_equal(time_demean.dataframe, expected,
+                       check_index_type=check,
+                       check_column_type=check)
 
 
 def test_mean_missing(data):
     xpd = PanelData(data.x)
     xpd.drop(xpd.isnull)
     entity_mean = xpd.mean('entity')
     expected = xpd.dataframe.groupby(level=0).mean()
@@ -486,26 +492,26 @@
     x = PanelData(data.x)
     w = PanelData(data.w)
     missing = x.isnull | w.isnull
     x.drop(missing)
     w.drop(missing)
 
     entity_demean = x.demean('entity', weights=w)
-    d = pd.get_dummies(pd.Categorical(x.index.labels[0]))
+    d = get_dummies(Categorical(x.index.labels[0]))
     d = d.values
     root_w = np.sqrt(w.values2d)
     wx = root_w * x.values2d
     wd = d * root_w
     mu = wd @ lstsq(wd, wx)[0]
     e = wx - mu
     assert_allclose(1 + np.abs(entity_demean.values2d),
                     1 + np.abs(e))
 
     time_demean = x.demean('time', weights=w)
-    d = pd.get_dummies(pd.Categorical(x.index.labels[1]))
+    d = get_dummies(Categorical(x.index.labels[1]))
     d = d.values
     root_w = np.sqrt(w.values2d)
     wx = root_w * x.values2d
     wd = d * root_w
     mu = wd @ lstsq(wd, wx)[0]
     e = wx - mu
     assert_allclose(1 + np.abs(time_demean.values2d),
@@ -516,44 +522,49 @@
     x = PanelData(data.x)
     w = PanelData(data.w)
     missing = x.isnull | w.isnull
     x.drop(missing)
     w.drop(missing)
     entity_mean = x.mean('entity', weights=w)
     c = x.index.levels[0][x.index.labels[0]]
-    d = pd.get_dummies(pd.Categorical(c, ordered=True))
+    d = get_dummies(Categorical(c, ordered=True))
     d = d[entity_mean.index]
     d = d.values
     root_w = np.sqrt(w.values2d)
     wx = root_w * x.values2d
     wd = d * root_w
     mu = lstsq(wd, wx)[0]
     assert_allclose(entity_mean, mu)
 
     time_mean = x.mean('time', weights=w)
     c = x.index.levels[1][x.index.labels[1]]
-    d = pd.get_dummies(pd.Categorical(c, ordered=True))
+    d = get_dummies(Categorical(c, ordered=True))
     d = d[time_mean.index]
     d = d.values
     root_w = np.sqrt(w.values2d)
     wx = root_w * x.values2d
     wd = d * root_w
     mu = pinv(wd) @ wx
     assert_allclose(time_mean, mu)
 
 
 def test_categorical_conversion():
     t, n = 3, 1000
     string = np.random.choice(['a', 'b', 'c'], (t, n))
     num = np.random.randn(t, n)
-    p = pd.Panel({'a': string, 'b': num})
+    time = date_range('1-1-2000', periods=t)
+    entities = ['entity.{0}'.format(i) for i in range(n)]
+    p = panel_to_frame(None, items=['a', 'b'], major_axis=time,
+                       minor_axis=entities, swap=True)
+    p['a'] = string.T.ravel()
+    p['b'] = num.T.ravel()
     p = p[['a', 'b']]
     panel = PanelData(p, convert_dummies=False)
     df = panel.dataframe.copy()
-    df['a'] = pd.Categorical(df['a'])
+    df['a'] = Categorical(df['a'])
     panel = PanelData(df, convert_dummies=True)
 
     df = panel.dataframe
     assert df.shape == (3000, 3)
     s = string.T.ravel()
     a_locs = np.where(s == 'a')
     b_locs = np.where(s == 'b')
@@ -567,15 +578,20 @@
     assert np.all(df.loc[:, 'a.c'].values[c_locs] == 1.0)
 
 
 def test_string_conversion():
     t, n = 3, 1000
     string = np.random.choice(['a', 'b', 'c'], (t, n))
     num = np.random.randn(t, n)
-    p = pd.Panel({'a': string, 'b': num})
+    time = date_range('1-1-2000', periods=t)
+    entities = ['entity.{0}'.format(i) for i in range(n)]
+    p = panel_to_frame(None, items=['a', 'b'], major_axis=time, minor_axis=entities,
+                       swap=True)
+    p['a'] = string.T.ravel()
+    p['b'] = num.T.ravel()
     p = p[['a', 'b']]
     panel = PanelData(p, var_name='OtherEffect')
     df = panel.dataframe
     assert df.shape == (3000, 3)
     s = string.T.ravel()
     a_locs = np.where(s == 'a')
     b_locs = np.where(s == 'b')
@@ -589,161 +605,162 @@
     assert np.all(df.loc[:, 'a.c'].values[c_locs] == 1.0)
 
 
 def test_string_nonconversion():
     t, n = 3, 1000
     string = np.random.choice(['a', 'b', 'c'], (t, n))
     num = np.random.randn(t, n)
-    p = pd.Panel({'a': string, 'b': num})
+    time = date_range('1-1-2000', periods=t)
+    entities = ['entity.{0}'.format(i) for i in range(n)]
+    p = panel_to_frame(None, items=['a', 'b'], major_axis=time, minor_axis=entities,
+                       swap=True)
+    p['a'] = string.T.ravel()
+    p['b'] = num.T.ravel()
     panel = PanelData(p, var_name='OtherEffect', convert_dummies=False)
     assert is_string_dtype(panel.dataframe['a'].dtype)
     assert np.all(panel.dataframe['a'] == string.T.ravel())
 
 
-def test_repr_html(panel):
-    data = PanelData(panel)
+def test_repr_html(mi_df):
+    data = PanelData(mi_df)
     html = data._repr_html_()
     assert '<br/>' in html
 
 
-def test_general_demean_oneway(panel):
-    y = PanelData(panel)
+def test_general_demean_oneway(mi_df):
+    y = PanelData(mi_df)
     dm1 = y.demean('entity')
-    g = pd.DataFrame(y.entity_ids, index=y.index)
+    g = DataFrame(y.entity_ids, index=y.index)
     dm2 = y.general_demean(g)
     assert_allclose(dm1.values2d, dm2.values2d)
 
     dm1 = y.demean('time')
-    g = pd.DataFrame(y.time_ids, index=y.index)
+    g = DataFrame(y.time_ids, index=y.index)
     dm2 = y.general_demean(g)
     assert_allclose(dm1.values2d, dm2.values2d)
 
-    g = pd.DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
+    g = DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
     dm2 = y.general_demean(g)
-    g = pd.Categorical(g.iloc[:, 0])
-    d = pd.get_dummies(g)
+    g = Categorical(g.iloc[:, 0])
+    d = get_dummies(g)
     dm1 = y.values2d - d @ lstsq(d, y.values2d)[0]
     assert_allclose(dm1, dm2.values2d)
 
 
-def test_general_demean_twoway(panel):
-    y = PanelData(panel)
+def test_general_demean_twoway(mi_df):
+    y = PanelData(mi_df)
     dm1 = y.demean('both')
-    g = pd.DataFrame(y.entity_ids, index=y.index)
-    g['column2'] = pd.Series(y.time_ids.squeeze(), index=y.index)
+    g = DataFrame(y.entity_ids, index=y.index)
+    g['column2'] = Series(y.time_ids.squeeze(), index=y.index)
     dm2 = y.general_demean(g)
     assert_allclose(dm1.values2d, dm2.values2d)
 
-    g = pd.DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
+    g = DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
     dm2 = y.general_demean(g)
-    g1 = pd.Categorical(g.iloc[:, 0])
-    d1 = pd.get_dummies(g1)
-    g2 = pd.Categorical(g.iloc[:, 1])
-    d2 = pd.get_dummies(g2, drop_first=True)
+    g1 = Categorical(g.iloc[:, 0])
+    d1 = get_dummies(g1)
+    g2 = Categorical(g.iloc[:, 1])
+    d2 = get_dummies(g2, drop_first=True)
     d = np.c_[d1, d2]
     dm1 = y.values2d - d @ lstsq(d, y.values2d)[0]
     assert_allclose(dm1 - dm2.values2d, np.zeros_like(dm2.values2d), atol=1e-7)
 
 
-def test_general_unit_weighted_demean_oneway(panel):
-    y = PanelData(panel)
+def test_general_unit_weighted_demean_oneway(mi_df):
+    y = PanelData(mi_df)
     dm1 = y.demean('entity')
-    g = PanelData(pd.DataFrame(y.entity_ids, index=y.index))
+    g = PanelData(DataFrame(y.entity_ids, index=y.index))
     weights = PanelData(g).copy()
     weights.dataframe.iloc[:, :] = 1
     dm2 = y.general_demean(g, weights)
     assert_allclose(dm1.values2d, dm2.values2d)
     dm3 = y.general_demean(g)
     assert_allclose(dm3.values2d, dm2.values2d)
 
     dm1 = y.demean('time')
-    g = PanelData(pd.DataFrame(y.time_ids, index=y.index))
+    g = PanelData(DataFrame(y.time_ids, index=y.index))
     dm2 = y.general_demean(g, weights)
     assert_allclose(dm1.values2d, dm2.values2d)
     dm3 = y.general_demean(g)
     assert_allclose(dm3.values2d, dm2.values2d)
 
-    g = PanelData(pd.DataFrame(np.random.randint(0, 10, g.dataframe.shape),
-                               index=y.index))
+    g = PanelData(DataFrame(np.random.randint(0, 10, g.dataframe.shape),
+                            index=y.index))
     dm2 = y.general_demean(g, weights)
     dm3 = y.general_demean(g)
-    g = pd.Categorical(g.dataframe.iloc[:, 0])
-    d = pd.get_dummies(g)
+    g = Categorical(g.dataframe.iloc[:, 0])
+    d = get_dummies(g)
     dm1 = y.values2d - d @ lstsq(d, y.values2d)[0]
     assert_allclose(dm1, dm2.values2d)
     assert_allclose(dm3.values2d, dm2.values2d)
 
 
-def test_general_weighted_demean_oneway(panel):
-    y = PanelData(panel)
-    weights = pd.DataFrame(
+def test_general_weighted_demean_oneway(mi_df):
+    y = PanelData(mi_df)
+    weights = DataFrame(
         np.random.chisquare(10, (y.dataframe.shape[0], 1)) / 10, index=y.index)
     w = PanelData(weights)
 
     dm1 = y.demean('entity', weights=w)
-    g = PanelData(pd.DataFrame(y.entity_ids, index=y.index))
+    g = PanelData(DataFrame(y.entity_ids, index=y.index))
     dm2 = y.general_demean(g, w)
     assert_allclose(dm1.values2d, dm2.values2d)
 
     dm1 = y.demean('time', weights=w)
-    g = PanelData(pd.DataFrame(y.time_ids, index=y.index))
+    g = PanelData(DataFrame(y.time_ids, index=y.index))
     dm2 = y.general_demean(g, w)
     assert_allclose(dm1.values2d, dm2.values2d)
 
-    g = PanelData(pd.DataFrame(np.random.randint(0, 10, g.dataframe.shape),
-                               index=y.index))
+    g = PanelData(DataFrame(np.random.randint(0, 10, g.dataframe.shape),
+                            index=y.index))
     dm2 = y.general_demean(g, w)
-    g = pd.Categorical(g.dataframe.iloc[:, 0])
-    d = pd.get_dummies(g)
+    g = Categorical(g.dataframe.iloc[:, 0])
+    d = get_dummies(g)
     wd = np.sqrt(w.values2d) * d
     wy = np.sqrt(w.values2d) * y.values2d
     dm1 = wy - wd @ lstsq(wd, wy)[0]
     assert_allclose(dm1, dm2.values2d, atol=1e-14)
 
 
-def test_general_unit_weighted_demean_twoway(panel):
+def test_general_unit_weighted_demean_twoway(mi_df):
     np.random.seed(12345)
-    y = PanelData(panel)
-    weights = pd.DataFrame(
+    y = PanelData(mi_df)
+    weights = DataFrame(
         np.random.chisquare(10, (y.dataframe.shape[0], 1)) / 10, index=y.index)
     w = PanelData(weights)
 
     dm1 = y.demean('both', weights=w)
-    g = pd.DataFrame(y.entity_ids, index=y.index)
-    g['column2'] = pd.Series(y.time_ids.squeeze(), index=y.index)
+    g = DataFrame(y.entity_ids, index=y.index)
+    g['column2'] = Series(y.time_ids.squeeze(), index=y.index)
     dm2 = y.general_demean(g, weights=w)
     assert_allclose(dm1.values2d - dm2.values2d, np.zeros_like(dm2.values2d),
                     atol=1e-7)
 
-    g = pd.DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
+    g = DataFrame(np.random.randint(0, 10, g.shape), index=y.index)
     dm2 = y.general_demean(g, weights=w)
-    g1 = pd.Categorical(g.iloc[:, 0])
-    d1 = pd.get_dummies(g1)
-    g2 = pd.Categorical(g.iloc[:, 1])
-    d2 = pd.get_dummies(g2, drop_first=True)
+    g1 = Categorical(g.iloc[:, 0])
+    d1 = get_dummies(g1)
+    g2 = Categorical(g.iloc[:, 1])
+    d2 = get_dummies(g2, drop_first=True)
     d = np.c_[d1, d2]
     wd = np.sqrt(w.values2d) * d
     wy = np.sqrt(w.values2d) * y.values2d
     dm1 = wy - wd @ lstsq(wd, wy)[0]
     assert_allclose(dm1 - dm2.values2d, np.zeros_like(dm2.values2d), atol=1e-7)
 
 
 def test_original_unmodified(data):
     pre_y = data.y.copy()
     pre_x = data.x.copy()
     pre_w = data.w.copy()
     mod = PanelOLS(data.y, data.x, weights=data.w)
     mod.fit(debiased=True)
-    if isinstance(data.y, (pd.DataFrame, pd.Panel)):
-        for after, before in (
-                (data.y, pre_y), (data.x, pre_x), (data.w, pre_w)):
-            if isinstance(before, pd.DataFrame):
-                assert_frame_equal(before, after)
-            else:
-                assert_panel_equal(before, after)
+    if isinstance(data.y, (DataFrame)):
+        for after, before in ((data.y, pre_y), (data.x, pre_x), (data.w, pre_w)):
+            assert_frame_equal(before, after)
 
         mi_df_y = PanelData(data.y).dataframe
         mi_df_x = PanelData(data.x).dataframe
         mi_df_y.index.names = ['firm', 'period']
         mi_df_x.index.names = ['firm', 'period']
         mi_df_w = PanelData(data.w).dataframe
         pre_y = mi_df_y.copy()
@@ -765,29 +782,26 @@
 
 
 def test_incorrect_time_axis():
     x = np.random.randn(3, 3, 1000)
     entities = ['entity.{0}'.format(i) for i in range(1000)]
     time = ['time.{0}'.format(i) for i in range(3)]
     var_names = ['var.{0}'.format(i) for i in range(3)]
-    p = pd.Panel(x, items=var_names, major_axis=time, minor_axis=entities)
+    p = panel_to_frame(x, items=var_names, major_axis=time, minor_axis=entities,
+                       swap=True)
     with pytest.raises(ValueError):
         PanelData(p)
-    df = p.swapaxes(1, 2).swapaxes(0, 1).to_frame()
-    with pytest.raises(ValueError):
-        PanelData(df)
 
-    time = [1, pd.datetime(1960, 1, 1), 'a']
+    time = [1, 2, 3]
     var_names = ['var.{0}'.format(i) for i in range(3)]
-    p = pd.Panel(x, items=var_names, major_axis=time, minor_axis=entities)
+    p = panel_to_frame(x, items=var_names, major_axis=time, minor_axis=entities,
+                       swap=True)
+    p.index = p.index.set_levels([1, datetime(1960, 1, 1), 'a'], 1)
     with pytest.raises(ValueError):
         PanelData(p)
-    df = p.swapaxes(1, 2).swapaxes(0, 1).to_frame()
-    with pytest.raises(ValueError):
-        PanelData(df)
 
 
 @pytest.mark.skipif(MISSING_XARRAY, reason='xarray is not installed')
 def test_incorrect_time_axis_xarray():
     x = np.random.randn(3, 3, 1000)
     entities = ['entity.{0}'.format(i) for i in range(1000)]
     time = ['time.{0}'.format(i) for i in range(3)]
@@ -799,7 +813,21 @@
         PanelData(da)
 
     da = xr.DataArray(x, coords={'entities': entities, 'time': time,
                                  'vars': vars},
                       dims=['vars', 'time', 'entities'])
     with pytest.raises(ValueError):
         PanelData(da)
+
+
+def test_named_index(data):
+    pdata = PanelData(data.x)
+    if isinstance(data.x, DataFrame):
+        assert pdata.dataframe.index.levels[0].name == data.x.index.levels[0].name
+        assert pdata.dataframe.index.levels[1].name == data.x.index.levels[1].name
+
+        data.x.index.levels[0].name = None
+        data.x.index.levels[1].name = None
+        pdata = PanelData(data.x)
+
+    assert pdata.dataframe.index.levels[0].name == 'entity'
+    assert pdata.dataframe.index.levels[1].name == 'time'
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_formula.py` & `linearmodels-4.9/linearmodels/tests/panel/test_formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import product
 
 import numpy as np
-import pandas as pd
 import pytest
+from pandas import DataFrame
+from pandas.testing import assert_frame_equal
 
-from linearmodels.compat.pandas import assert_frame_equal
 from linearmodels.formula import (between_ols, first_difference_ols, panel_ols,
                                   pooled_ols, random_effects, fama_macbeth)
 from linearmodels.panel.model import (BetweenOLS, FirstDifferenceOLS, PanelOLS,
                                       PooledOLS, RandomEffects, FamaMacBeth,
                                       PanelFormulaParser)
 from linearmodels.tests.panel._utility import generate_data, datatypes
 
@@ -48,15 +48,15 @@
 
 
 def sigmoid(v):
     return np.exp(v) / (1 + np.exp(v))
 
 
 def test_basic_formulas(data, models, formula):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     model, formula_func = models
     mod = model.from_formula(formula, joined)
     res = mod.fit()
     wmod = model.from_formula(formula, joined, weights=data.w)
@@ -95,39 +95,39 @@
     mod2 = model(data.y, x[vars])
     res2 = mod2.fit()
     np.testing.assert_allclose(res.params, res2.params)
     assert mod.formula == formula
 
 
 def test_basic_formulas_math_op(data, models, formula):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     formula = formula.replace('x0', 'np.exp(x0)')
     formula = formula.replace('x1', 'sigmoid(x1)')
     model, formula_func = models
     res = model.from_formula(formula, joined).fit()
     pred = res.predict(data=joined)
     pred = pred.reindex(res.fitted_values.index)
     np.testing.assert_allclose(pred.values, res.fitted_values.values)
 
 
 def test_panel_ols_formulas_math_op(data):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     formula = 'y ~ x1 + np.exp(x2)'
     mod = PanelOLS.from_formula(formula, joined)
     mod.fit()
 
 
 def test_panel_ols_formula(data):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     formula = 'y ~ x1 + x2'
     mod = PanelOLS.from_formula(formula, joined)
     assert mod.formula == formula
 
@@ -155,15 +155,15 @@
 
     formula = 'y ~ x1 + EntityEffects + FixedEffects + x2 '
     with pytest.raises(ValueError):
         PanelOLS.from_formula(formula, joined)
 
 
 def test_basic_formulas_predict(data, models, formula):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     model, formula_func = models
     mod = model.from_formula(formula, joined)
     res = mod.fit()
     pred = res.predict(data=joined)
@@ -200,15 +200,15 @@
     pred2 = res.predict(x[vars])
     pred3 = res2.predict(x[vars])
     np.testing.assert_allclose(pred, pred2, atol=1e-8)
     np.testing.assert_allclose(pred, pred3, atol=1e-8)
 
 
 def test_formulas_predict_error(data, models, formula):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     joined = data.x
     joined['y'] = data.y
     model, formula_func = models
     mod = model.from_formula(formula, joined)
     res = mod.fit()
     with pytest.raises(ValueError):
@@ -222,15 +222,15 @@
     x = data.x
     res = model(data.y, x[vars]).fit()
     with pytest.raises(ValueError):
         res.predict(data=joined)
 
 
 def test_parser(data, formula, effects):
-    if not isinstance(data.y, pd.DataFrame):
+    if not isinstance(data.y, DataFrame):
         return
     if effects:
         formula += ' + EntityEffects + TimeEffects'
     joined = data.x
     joined['y'] = data.y
     parser = PanelFormulaParser(formula, joined)
     dep, exog = parser.data
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_between_ols.py` & `linearmodels-4.9/linearmodels/tests/panel/test_between_ols.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,20 +31,25 @@
     else:
         return missing_data(request)
 
 
 def test_single_entity(data):
     x = data.x
     y = data.y
-    if isinstance(x, pd.Panel):
-        x = x.iloc[:, [0], :]
-        y = y.iloc[[0], :]
-    else:
+    if isinstance(x, pd.DataFrame):
+        time = y.index.levels[1][0]
+        y = y.xs(time, level=1, drop_level=False)
+        x = x.xs(time, level=1, drop_level=False)
+    elif isinstance(x, np.ndarray):
         x = x[:, [0]]
         y = y[[0]]
+    else:
+        # xarray DataArray
+        x = x[:, [0]]
+        y = y[:, [0]]
     mod = BetweenOLS(y, x)
     res = mod.fit(reweight=True, debiased=False)
 
     dep = mod.dependent.dataframe
     exog = mod.exog.dataframe
     ols = IV2SLS(dep, exog, None, None)
     ols_res = ols.fit(cov_type='unadjusted')
@@ -61,22 +66,28 @@
     assert_results_equal(res, ols_res)
 
 
 def test_single_entity_weights(data):
     x = data.x
     y = data.y
     w = data.w
-    if isinstance(x, pd.Panel):
-        x = x.iloc[:, [0], :]
-        y = y.iloc[[0], :]
-        w = w.iloc[[0], :]
-    else:
+    if isinstance(x, pd.DataFrame):
+        time = y.index.levels[1][0]
+        y = y.xs(time, level=1, drop_level=False)
+        x = x.xs(time, level=1, drop_level=False)
+        w = w.xs(time, level=1, drop_level=False)
+    elif isinstance(x, np.ndarray):
         x = x[:, [0]]
         y = y[[0]]
         w = w[[0]]
+    else:
+        # xarray DataArray
+        x = x[:, [0]]
+        y = y[:, [0]]
+        w = w[:, [0]]
 
     mod = BetweenOLS(y, x, weights=w)
     res = mod.fit(reweight=True, debiased=False)
 
     dep = mod.dependent.dataframe
     exog = mod.exog.dataframe
     ols = IV2SLS(dep, exog, None, None, weights=mod.weights.values2d)
@@ -174,15 +185,16 @@
     ols_res = ols.fit(cov_type='robust')
     assert_results_equal(res, ols_res)
 
     vc1 = PanelData(missing_data.vc1)
     ols_clusters = vc1.dataframe.groupby(level=0).mean().astype(np.int32)
     ols_clusters = ols_clusters.reindex(mod.dependent.entities)
 
-    res = mod.fit(reweight=True, cov_type='clustered', clusters=missing_data.vc1, debiased=False)
+    res = mod.fit(reweight=True, cov_type='clustered',
+                  clusters=missing_data.vc1, debiased=False)
     ols_res = ols.fit(cov_type='clustered', clusters=ols_clusters)
     assert_results_equal(res, ols_res)
 
 
 def test_missing_weighted(missing_data):
     mod = BetweenOLS(missing_data.y, missing_data.x, weights=missing_data.w)
     res = mod.fit(reweight=True, debiased=False)
@@ -285,34 +297,38 @@
     with pytest.raises(ValueError):
         mod.fit(cov_type='clustered', clusters=clusters, debiased=False)
 
 
 def test_default_clusters(data):
     x = data.x
     y = data.y
-    if isinstance(x, pd.Panel):
-        x = x.iloc[:, [0], :]
-        y = y.iloc[[0], :]
-    else:
+    if isinstance(x, pd.DataFrame):
+        time = y.index.levels[1][0]
+        y = y.xs(time, level=1, drop_level=False)
+        x = x.xs(time, level=1, drop_level=False)
+    elif isinstance(x, np.ndarray):
         x = x[:, [0]]
         y = y[[0]]
+    else:
+        # xarray DataArray
+        x = x[:, [0]]
+        y = y[:, [0]]
     mod = BetweenOLS(y, x)
     res = mod.fit(reweight=True, cov_type='clustered', debiased=False)
 
     dep = mod.dependent.dataframe
     exog = mod.exog.dataframe
     ols = IV2SLS(dep, exog, None, None)
     ols_res = ols.fit(cov_type='clustered')
     assert_results_equal(res, ols_res)
 
 
 def test_fitted_effects_residuals(both_data_types):
     mod = BetweenOLS(both_data_types.y, both_data_types.x)
     res = mod.fit(reweight=True, debiased=False)
-    res.idiosyncratic
     expected = pd.DataFrame(mod.exog.values2d @ res.params.values, mod.dependent.index,
                             columns=['fitted_values'])
     assert_allclose(expected, res.fitted_values)
     assert_frame_similar(res.fitted_values, expected)
 
     index = mod.dependent.dataframe.index
     reindex = index.levels[0][index.labels[0]]
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_random_effects.py` & `linearmodels-4.9/linearmodels/tests/panel/test_random_effects.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_model.py` & `linearmodels-4.9/linearmodels/tests/panel/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,32 +40,49 @@
     w = mod.weights.values2d
     missing = PanelData(data.y).isnull | PanelData(data.x).isnull
     expected = weights[~missing.squeeze()][:, None]
     expected = expected / expected.mean()
     assert_equal(w, expected)
 
     # Per time
-    n = data.y.shape[0]
+    if isinstance(data.x, pd.DataFrame):
+        n = len(data.y.index.levels[1])
+        k = len(data.y.index.levels[0])
+    elif isinstance(data.x, np.ndarray):
+        n = data.y.shape[0]
+        k = data.y.shape[1]
+    else:
+        n = data.y.shape[1]
+        k = data.y.shape[2]
+
     weights = 1 + np.random.random_sample(n)
     mod = PanelOLS(data.y, data.x, weights=weights)
     mod.fit()
     w = mod.weights.values2d
-    expected = weights[:, None] @ np.ones((1, data.y.shape[1]))
+    expected = weights[:, None] @ np.ones((1, k))
     expected = expected.T.ravel()
     expected = expected[~missing.squeeze()][:, None]
     expected = expected / expected.mean()
     assert_equal(w, expected)
 
     # Per entity
-    n = data.y.shape[1]
+    if isinstance(data.x, pd.DataFrame):
+        n = len(data.y.index.levels[0])
+        k = len(data.y.index.levels[1])
+    elif isinstance(data.x, np.ndarray):
+        n = data.y.shape[1]
+        k = data.y.shape[0]
+    else:
+        n = data.y.shape[2]
+        k = data.y.shape[1]
     weights = 1 + np.random.random_sample(n)
     mod = PanelOLS(data.y, data.x, weights=weights)
     mod.fit()
     w = mod.weights.values2d
-    expected = np.ones((data.y.shape[0], 1)) @ weights[None, :]
+    expected = np.ones((k, 1)) @ weights[None, :]
     expected = expected.T.ravel()
     expected = expected[~missing.squeeze()][:, None]
     expected = expected / expected.mean()
     assert_equal(w, expected)
 
     weights = 1 + np.random.random_sample(data.y.shape)
     mod = PanelOLS(data.y, data.x, weights=weights)
@@ -133,46 +150,50 @@
     expected = lsdv(y, x, has_const=False, general=other.iloc[:, 0].values)
     assert_allclose(res.params.squeeze(), expected, rtol=1e-4)
 
 
 def test_incorrect_weight_shape(data):
     w = data.w
     if isinstance(w, pd.DataFrame):
-        w = w.iloc[:3]
-        w = pd.Panel({'weights': w})
+        entities = w.index.levels[0][:4]
+        w = w.loc[pd.IndexSlice[entities[0]:entities[-1]], :]
     elif isinstance(w, np.ndarray):
         w = w[:3]
         w = w[None, :, :]
     else:  # xarray
         return
 
     with pytest.raises(ValueError):
         PanelOLS(data.y, data.x, weights=w)
 
 
 def test_weight_ambiguity(data):
-    t = data.y.shape[0]
-    if isinstance(data.x, pd.Panel):
-        x = data.x.iloc[:, :, :t]
+    if isinstance(data.x, pd.DataFrame):
+        t = len(data.y.index.levels[1])
+        entities = data.x.index.levels[0]
+        slice = pd.IndexSlice[entities[0]:entities[t - 1]]
+        x = data.x.loc[slice, :]
     else:
+        t = data.x.shape[1]
         x = data.x[:, :, :t]
     y = data.y
     weights = 1 + np.random.random_sample(t)
     with pytest.raises(AmbiguityError):
         PanelOLS(y, x, weights=weights)
 
 
 def test_absorbing_effect(data):
-    if not isinstance(data.x, pd.Panel):
+    if not isinstance(data.x, pd.DataFrame):
         return
     x = data.x.copy()
-    temp = data.x.iloc[0].copy()
-    temp.values[:, :] = 1.0
-    n = temp.shape[1]
-    temp.values[:, n // 2:] = 0
+    nentity = len(x.index.levels[0])
+    ntime = len(x.index.levels[1])
+    temp = data.x.iloc[:, 0].copy()
+    temp.values[:] = 1.0
+    temp.values[:(ntime * (nentity // 2))] = 0
     x['Intercept'] = 1.0
     x['absorbed'] = temp
     with pytest.raises(AbsorbingEffectError):
         PanelOLS(data.y, x, entity_effects=True).fit()
 
 
 @pytest.mark.filterwarnings('ignore::DeprecationWarning')
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_fama_macbeth.py` & `linearmodels-4.9/linearmodels/tests/panel/test_fama_macbeth.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_pooled_ols.py` & `linearmodels-4.9/linearmodels/tests/panel/test_pooled_ols.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,32 +52,33 @@
     w.index = x.index = y.index
 
     res2 = IV2SLS(y, x, None, None, weights=w).fit(cov_type='unadjusted')
     assert_results_equal(res, res2)
 
 
 def test_diff_data_size(data):
-    if isinstance(data.x, pd.Panel):
-        x = data.x.iloc[:, :, :-1]
+    if isinstance(data.x, pd.DataFrame):
+        entities = data.x.index.levels[0]
+        x = data.x.loc[pd.IndexSlice[entities[0]:entities[-2]]]
         y = data.y
     elif isinstance(data.x, np.ndarray):
         x = data.x
         y = data.y[:-1]
     else:  # xr.DataArray:
-        x = data.x[:, :-1]
-        y = data.y[:, :-1]
+        x = data.x[:, :, :-1]
+        y = data.y
 
     with pytest.raises(ValueError):
         PooledOLS(y, x)
 
 
 def test_rank_deficient_array(data):
-    x = data.x
-    if isinstance(data.x, pd.Panel):
-        x.iloc[1] = x.iloc[0]
+    x = data.x.copy()
+    if isinstance(data.x, pd.DataFrame):
+        x.iloc[:, 1] = x.iloc[:, 0]
     else:
         x[1] = x[0]
     with pytest.raises(ValueError):
         PooledOLS(data.y, x)
 
 
 def test_results_access(data):
@@ -95,15 +96,15 @@
     d = dir(res)
     for key in d:
         if not key.startswith('_'):
             val = getattr(res, key)
             if callable(val):
                 val()
 
-    if not isinstance(data.x, pd.Panel):
+    if not isinstance(data.x, pd.DataFrame):
         return
     x = data.y.copy()
     x.iloc[:, :] = 1
     mod = PooledOLS(data.y, x)
     res = mod.fit(debiased=False)
     d = dir(res)
     for key in d:
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_firstdifference_ols.py` & `linearmodels-4.9/linearmodels/tests/panel/test_firstdifference_ols.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,24 +134,25 @@
 
     res = mod.fit(cov_type='clustered', clusters=clusters, debiased=False)
     ols_res = ols_mod.fit(cov_type='clustered', clusters=ols_clusters)
     assert_results_equal(res, ols_res)
 
 
 def test_first_difference_errors(data):
-    if isinstance(data.x, pd.Panel):
-        x = data.x.iloc[:, [0], :]
-        y = data.y.iloc[[0], :]
+    if isinstance(data.x, pd.DataFrame):
+        time = data.y.index.levels[1][0]
+        y = data.y.xs(time, level=1, drop_level=False)
+        x = data.x.xs(time, level=1, drop_level=False)
     else:
         x = data.x[:, [0], :]
         y = data.y[[0], :]
     with pytest.raises(ValueError):
         FirstDifferenceOLS(y, x)
 
-    if not isinstance(data.x, pd.Panel):
+    if not isinstance(data.x, pd.DataFrame):
         return
     x = data.x.copy()
     x['Intercept'] = 1.0
     with pytest.raises(ValueError):
         FirstDifferenceOLS(data.y, x)
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_cluster_input_formats.py` & `linearmodels-4.9/linearmodels/tests/panel/test_cluster_input_formats.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_panel_ols.py` & `linearmodels-4.9/linearmodels/tests/panel/test_panel_ols.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 perms = list(product(missing, datatypes, has_const))
 ids = list(map(lambda s: '-'.join(map(str, s)), perms))
 
 
 @pytest.fixture(params=perms, ids=ids)
 def data(request):
     missing, datatype, const = request.param
-    return generate_data(missing, datatype, const=const, ntk=(91, 7, 5), other_effects=2)
+    return generate_data(missing, datatype, const=const, ntk=(91, 15, 5), other_effects=2)
+
+
+@pytest.fixture(params=perms, ids=ids)
+def large_data(request):
+    missing, datatype, const = request.param
+    return generate_data(missing, datatype, const=const, ntk=(51, 71, 5), other_effects=2)
 
 
 perms = list(product(missing, datatypes))
 ids = list(map(lambda s: '-'.join(map(str, s)), perms))
 
 
 @pytest.fixture(params=perms, ids=ids)
@@ -152,15 +158,17 @@
 def test_const_data_both(const_data):
     y, x = const_data.y, const_data.x
     mod = PanelOLS(y, x, entity_effects=True, time_effects=True)
     res = mod.fit(debiased=False)
 
     x = mod.exog.dataframe
     d1 = mod.dependent.dummies('entity', drop_first=True)
+    d1.columns = ['d.entity.{0}'.format(i) for i in d1]
     d2 = mod.dependent.dummies('time', drop_first=True)
+    d2.columns = ['d.time.{0}'.format(i) for i in d2]
     d = np.c_[d1.values, d2.values]
     d = pd.DataFrame(d, index=x.index, columns=list(d1.columns) + list(d2.columns))
     d.iloc[:, :] = d.values - x.values @ lstsq(x.values, d.values)[0]
 
     xd = np.c_[x.values, d.values]
     xd = pd.DataFrame(xd, index=x.index, columns=list(x.columns) + list(d.columns))
 
@@ -173,15 +181,17 @@
     mod = PanelOLS(y, x, entity_effects=True, time_effects=True, weights=const_data.w)
     res = mod.fit(debiased=False)
 
     w = mod.weights.dataframe
     x = mod.exog.dataframe
 
     d1 = mod.dependent.dummies('entity', drop_first=True)
+    d1.columns = ['d.entity.{0}'.format(i) for i in d1]
     d2 = mod.dependent.dummies('time', drop_first=True)
+    d2.columns = ['d.time.{0}'.format(i) for i in d2]
     d = np.c_[d1.values, d2.values]
     root_w = np.sqrt(w.values)
     z = np.ones_like(x)
     wd = root_w * d
     wz = root_w
     d = d - z @ lstsq(wz, wd)[0]
     d = pd.DataFrame(d, index=x.index, columns=list(d1.columns) + list(d2.columns))
@@ -284,16 +294,16 @@
     assert_results_equal(res, res2, test_df=False)
 
     res = mod.fit(cov_type='robust', auto_df=False, count_effects=False, debiased=False)
     res2 = ols_mod.fit(cov_type='robust')
     assert_results_equal(res, res2, test_df=False)
 
 
-def test_panel_time_lsdv(data):
-    mod = PanelOLS(data.y, data.x, time_effects=True)
+def test_panel_time_lsdv(large_data):
+    mod = PanelOLS(large_data.y, large_data.x, time_effects=True)
     res = mod.fit(auto_df=False, count_effects=False, debiased=False)
 
     y = mod.dependent.dataframe
     x = mod.exog.dataframe
     d = mod.dependent.dummies('time', drop_first=mod.has_constant)
     d_cols = list(d.columns)
     d = d.values
@@ -309,22 +319,22 @@
     assert_results_equal(res, res2, test_fit=False)
     assert_allclose(res.rsquared_inclusive, res2.rsquared)
 
     res = mod.fit(cov_type='robust', auto_df=False, count_effects=False, debiased=False)
     res2 = ols_mod.fit(cov_type='robust')
     assert_results_equal(res, res2, test_fit=False)
 
-    clusters = data.vc1
+    clusters = large_data.vc1
     ols_clusters = mod.reformat_clusters(clusters)
     res = mod.fit(cov_type='clustered', clusters=clusters, auto_df=False, count_effects=False,
                   debiased=False)
     res2 = ols_mod.fit(cov_type='clustered', clusters=ols_clusters.dataframe)
     assert_results_equal(res, res2, test_fit=False)
 
-    clusters = data.vc2
+    clusters = large_data.vc2
     ols_clusters = mod.reformat_clusters(clusters)
     res = mod.fit(cov_type='clustered', clusters=clusters, auto_df=False, count_effects=False,
                   debiased=False)
     res2 = ols_mod.fit(cov_type='clustered', clusters=ols_clusters.dataframe)
     assert_results_equal(res, res2, test_fit=False)
 
     res = mod.fit(cov_type='clustered', cluster_time=True, auto_df=False, count_effects=False,
@@ -509,16 +519,16 @@
     clusters = pd.DataFrame(mod.dependent.entity_ids,
                             index=mod.dependent.index,
                             columns=['var.clust'])
     res2 = ols_mod.fit(cov_type='clustered', clusters=clusters)
     assert_results_equal(res, res2, test_fit=False)
 
 
-def test_panel_time_lsdv_weighted(data):
-    mod = PanelOLS(data.y, data.x, time_effects=True, weights=data.w)
+def test_panel_time_lsdv_weighted(large_data):
+    mod = PanelOLS(large_data.y, large_data.x, time_effects=True, weights=large_data.w)
     res = mod.fit(auto_df=False, count_effects=False, debiased=False)
 
     y = mod.dependent.dataframe
     x = mod.exog.dataframe
     w = mod.weights.dataframe
     d = mod.dependent.dummies('time', drop_first=mod.has_constant)
     d_cols = d.columns
@@ -537,22 +547,22 @@
     res2 = ols_mod.fit(cov_type='unadjusted')
     assert_results_equal(res, res2, test_fit=False)
 
     res = mod.fit(cov_type='robust', auto_df=False, count_effects=False, debiased=False)
     res2 = ols_mod.fit(cov_type='robust')
     assert_results_equal(res, res2, test_fit=False)
 
-    clusters = data.vc1
+    clusters = large_data.vc1
     ols_clusters = mod.reformat_clusters(clusters)
     res = mod.fit(cov_type='clustered', clusters=clusters, auto_df=False, count_effects=False,
                   debiased=False)
     res2 = ols_mod.fit(cov_type='clustered', clusters=ols_clusters.dataframe)
     assert_results_equal(res, res2, test_fit=False)
 
-    clusters = data.vc2
+    clusters = large_data.vc2
     ols_clusters = mod.reformat_clusters(clusters)
     res = mod.fit(cov_type='clustered', clusters=clusters, auto_df=False, count_effects=False,
                   debiased=False)
     res2 = ols_mod.fit(cov_type='clustered', clusters=ols_clusters.dataframe)
     assert_results_equal(res, res2, test_fit=False)
 
     res = mod.fit(cov_type='clustered', cluster_time=True, auto_df=False, count_effects=False,
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/results/parse_stata_results.py` & `linearmodels-4.9/linearmodels/tests/panel/results/parse_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/results/generate-panel-data.py` & `linearmodels-4.9/linearmodels/tests/panel/results/generate-panel-data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import pandas as pd
 
+from linearmodels.compat.pandas import concat
 from linearmodels.panel.data import PanelData
+from linearmodels.utility import panel_to_frame
 
 np.random.seed(12345)
 n, t, k = 1000, 3, 6
 x = np.random.randn(k + 1, t, n)
 x[0, :, :] = 1
 beta = np.arange(1, k + 2) / (k + 1)
 eps = np.random.randn(t, n)
@@ -17,28 +19,29 @@
 w = w / w.mean()
 
 items = ['x' + str(i) for i in range(1, k + 1)]
 items = ['intercept'] + items
 major = pd.date_range('12-31-1999', periods=t, freq='A-DEC')
 minor = ['firm.' + str(i) for i in range(1, n + 1)]
 
-x = pd.Panel(x, items=items, major_axis=major, minor_axis=minor)
-
-y = pd.DataFrame(y, index=major, columns=minor)
-y = pd.Panel({'y': y})
-
-w = pd.DataFrame(w, index=major, columns=minor)
-w = pd.Panel({'w': w})
+x = panel_to_frame(x, items, major, minor, swap=True)
+y = panel_to_frame(y[None, :], ['y'], major, minor, swap=True)
+w = panel_to_frame(w[None, :], ['w'], major, minor, swap=True)
 
 x = PanelData(x)
 y = PanelData(y)
 w = PanelData(w)
 
-z = pd.concat([x.dataframe, y.dataframe, w.dataframe], 1)
+z = concat([x.dataframe, y.dataframe, w.dataframe], 1)
+final_index = pd.MultiIndex.from_product([minor, major])
+final_index.levels[0].name = 'firm'
+z = z.reindex(final_index)
 z.index.levels[0].name = 'firm'
+z.index.levels[1].name = 'time'
+
 z = z.reset_index()
 z['firm_id'] = z.firm.astype('category')
 z['firm_id'] = z.firm_id.cat.codes
 
 vars = ['y', 'x1', 'x2', 'x3', 'x4', 'x5']
 missing = 0.05
 for v in vars:
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/results/stata-panel-simulated-results.txt` & `linearmodels-4.9/linearmodels/tests/panel/results/stata-panel-simulated-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/results/simulated-panel.dta` & `linearmodels-4.9/linearmodels/tests/panel/results/simulated-panel.dta`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 7202 0100 1900 b80b 0000 0000 0000 0000  r...............
 00000010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0031 3020 4170  ...........10 Ap
-00000060: 7220 3230 3137 2031 303a 3433 00fd 09ff  r 2017 10:43....
+00000050: 0000 0000 0000 0000 0000 0032 3720 4d61  ...........27 Ma
+00000060: 7920 3230 3138 2031 363a 3333 00fd 09ff  y 2018 16:33....
 00000070: ffff ffff ffff ffff fffc ffff ffff ffff  ................
 00000080: ffff ffff ffff 696e 6465 7800 0000 0000  ......index.....
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0066 6972 6d00 0000 0000  .......firm.....
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 7469 6d65 0000 0000  ........time....
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -554,23 +554,23 @@
 00002290: 2157 c006 25c4 3ff1 607f f63e d9f3 3f00  !W..%.?.`..>..?.
 000022a0: 0000 0000 00e0 7f00 0000 0000 00e0 7fae  ................
 000022b0: 0ddb 5b42 4dee 3ff9 428d 8851 03b9 bfec  ..[BM.?.B..Q....
 000022c0: 2157 c006 25c4 3f00 0000 0000 00e0 7f14  !W..%.?.........
 000022d0: 0000 0066 6972 6d2e 3700 0000 0000 000d  ...firm.7.......
 000022e0: 6949 7342 0000 0000 0000 f03f c095 dc79  iIsB.......?...y
 000022f0: 9f6b df3f 5b1f 7964 8c6c e7bf 153a 6e8a  .k.?[.yd.l...:n.
-00002300: 39bd dabf 96b4 9c2d ccc0 fa3f 340f f171  9......-...?4..q
+00002300: 39bd dabf 96b4 9c2d ccc0 fa3f 330f f171  9......-...?3..q
 00002310: 3add ac3f 29b3 ca56 ad13 f33f fed4 b37f  :..?)..V...?....
 00002320: e155 d73f 7e24 839a 4f7b f03f 9b02 0000  .U.?~$..O{.?....
 00002330: 0000 0000 e07f c095 dc79 9f6b df3f 5b1f  .........y.k.?[.
 00002340: 7964 8c6c e7bf 0000 0000 0000 e07f 96b4  yd.l............
-00002350: 9c2d ccc0 fa3f 340f f171 3add ac3f fed4  .-...?4..q:..?..
+00002350: 9c2d ccc0 fa3f 330f f171 3add ac3f fed4  .-...?3..q:..?..
 00002360: b37f e155 d73f c095 dc79 9f6b df3f 0000  ...U.?...y.k.?..
 00002370: 0000 0000 e07f 153a 6e8a 39bd dabf 96b4  .......:n.9.....
-00002380: 9c2d ccc0 fa3f 340f f171 3add ac3f 1500  .-...?4..q:..?..
+00002380: 9c2d ccc0 fa3f 330f f171 3add ac3f 1500  .-...?3..q:..?..
 00002390: 0000 6669 726d 2e38 0000 0000 00c0 8120  ..firm.8....... 
 000023a0: 5e72 4200 0000 0000 00f0 3ffe 8650 b2d9  ^rB.......?..P..
 000023b0: 6da4 3f3e 3778 3ed4 d296 bfd8 54b9 d31b  m.?>7x>.....T...
 000023c0: 09d6 bf59 f390 f5a2 57be 3fad 7983 c618  ...Y....W.?.y...
 000023d0: a1f5 3f5f b912 3dd8 c0cb bf82 1860 15ab  ..?_..=......`..
 000023e0: 75e3 bfd2 ec3f 4df3 b1e7 3f0a 0382 1860  u....?M...?....`
 000023f0: 15ab 75e3 bffe 8650 b2d9 6da4 3f3e 3778  ..u....P..m.?>7x
@@ -590,23 +590,23 @@
 000024d0: 2899 febf bc63 1a76 00a5 02c0 a4db ee3a  (....c.v.......:
 000024e0: 6c4b 14c0 ea25 60da a8e3 c3bf c3b6 8af2  lK...%`.........
 000024f0: 0733 e2bf 0000 0000 0000 e07f dc5a f3d7  .3...........Z..
 00002500: 2899 febf bc63 1a76 00a5 02c0 1700 0000  (....c.v........
 00002510: 6669 726d 2e38 0000 0000 0000 0d69 4973  firm.8.......iIs
 00002520: 4200 0000 0000 00f0 3f6a b9dd 47e8 65e6  B.......?j..G.e.
 00002530: bf6a 2784 f022 cdeb 3fe0 a5c9 a3a0 9fe1  .j'.."..?.......
-00002540: bf6a c6bd c671 06e7 3f69 35a9 ddb8 13cd  .j...q..?i5.....
+00002540: bf6a c6bd c671 06e7 3f68 35a9 ddb8 13cd  .j...q..?h5.....
 00002550: bfab ff4e 9fb5 35d8 bfd5 5915 39bc 45f6  ...N..5...Y.9.E.
 00002560: bfd2 ec3f 4df3 b1e7 3f0a 03d5 5915 39bc  ...?M...?...Y.9.
 00002570: 45f6 bf6a b9dd 47e8 65e6 bf6a 2784 f022  E..j..G.e..j'.."
 00002580: cdeb 3fe0 a5c9 a3a0 9fe1 bf6a c6bd c671  ..?........j...q
-00002590: 06e7 3f69 35a9 ddb8 13cd bfd5 5915 39bc  ..?i5.......Y.9.
+00002590: 06e7 3f68 35a9 ddb8 13cd bfd5 5915 39bc  ..?h5.......Y.9.
 000025a0: 45f6 bf00 0000 0000 00e0 7f6a 2784 f022  E..........j'.."
 000025b0: cdeb 3fe0 a5c9 a3a0 9fe1 bf6a c6bd c671  ..?........j...q
-000025c0: 06e7 3f69 35a9 ddb8 13cd bf18 0000 0066  ..?i5..........f
+000025c0: 06e7 3f68 35a9 ddb8 13cd bf18 0000 0066  ..?h5..........f
 000025d0: 6972 6d2e 3900 0000 0000 c081 205e 7242  irm.9....... ^rB
 000025e0: 0000 0000 0000 f03f bb5c 38c7 dd3c e8bf  .......?.\8..<..
 000025f0: df02 16c2 6bce cdbf 47bc 65c0 ae8c a3bf  ....k...G.e.....
 00002600: 206c ba8e 5275 e53f e12f c056 8ece e93f   l..Ru.?./.V...?
 00002610: e0ca 21cf a3c5 f5bf 9c40 5560 f496 03c0  ..!......@U`....
 00002620: 9c6b ddd0 df26 f13f 7903 9c40 5560 f496  .k...&.?y..@U`..
 00002630: 03c0 bb5c 38c7 dd3c e8bf df02 16c2 6bce  ...\8..<......k.
@@ -4480,22 +4480,22 @@
 000117f0: 99c6 7486 c4bf 8865 95d2 d925 dabf cab1  ..t....e...%....
 00011800: fe76 e721 f5bf c3a6 4f5c bc0a f0bf 9b12  .v.!....O\......
 00011810: 79b6 d1ca dfbf cecb e57f 7247 12c0 a623  y.........rG...#
 00011820: 99c6 7486 c4bf 8865 95d2 d925 dabf cab1  ..t....e...%....
 00011830: fe76 e721 f5bf c3a6 4f5c bc0a f0bf 9b12  .v.!....O\......
 00011840: 79b6 d1ca dfbf 5d01 0000 6669 726d 2e31  y.....]...firm.1
 00011850: 3137 0000 0040 faed d372 4200 0000 0000  17...@...rB.....
-00011860: 00f0 3f0d d775 01ca 94d9 bf03 44d6 5c51  ..?..u......D.\Q
+00011860: 00f0 3f0c d775 01ca 94d9 bf03 44d6 5c51  ..?..u......D.\Q
 00011870: 63d4 bf76 b8ff 6e42 c4a7 bf8b 9f90 224a  c..v..nB......"J
 00011880: 34d4 bff4 84e9 76bb 50c1 bf1d 8556 da10  4.....v.P....V..
 00011890: 0ae6 3f66 e6eb 73a8 e4f0 bf9d 5a0e 353c  ..?f..s.....Z.5<
-000118a0: bdf0 3f15 0066 e6eb 73a8 e4f0 bf0d d775  ..?..f..s......u
+000118a0: bdf0 3f15 0066 e6eb 73a8 e4f0 bf0c d775  ..?..f..s......u
 000118b0: 01ca 94d9 bf03 44d6 5c51 63d4 bf76 b8ff  ......D.\Qc..v..
 000118c0: 6e42 c4a7 bf8b 9f90 224a 34d4 bff4 84e9  nB......"J4.....
-000118d0: 76bb 50c1 bf66 e6eb 73a8 e4f0 bf0d d775  v.P..f..s......u
+000118d0: 76bb 50c1 bf66 e6eb 73a8 e4f0 bf0c d775  v.P..f..s......u
 000118e0: 01ca 94d9 bf03 44d6 5c51 63d4 bf76 b8ff  ......D.\Qc..v..
 000118f0: 6e42 c4a7 bf8b 9f90 224a 34d4 bff4 84e9  nB......"J4.....
 00011900: 76bb 50c1 bf5e 0100 0066 6972 6d2e 3131  v.P..^...firm.11
 00011910: 3700 0000 000d 6949 7342 0000 0000 0000  7.....iIsB......
 00011920: f03f ad05 bf97 e81e d0bf de96 264e 6c2b  .?..........&Nl+
 00011930: eb3f d1db a447 aba6 d9bf 6a3f 9a63 9a8d  .?...G....j?.c..
 00011940: dc3f c19d 05ad dfa0 ef3f c997 43da df4c  .?.......?..C..L
@@ -11345,22 +11345,22 @@
 0002c500: ada0 ebba 9bee 3f47 c677 8e1f 71d0 3fa6  ......?G.w..q.?.
 0002c510: 4618 459e 72e1 3faa f7f6 8ced 9c04 409e  F.E.r.?.......@.
 0002c520: 0737 7ec3 b1d1 3f00 0000 0000 00e0 7fa4  .7~...?.........
 0002c530: ada0 ebba 9bee 3f00 0000 0000 00e0 7f00  ......?.........
 0002c540: 0000 0000 00e0 7f9c 0300 0066 6972 6d2e  ...........firm.
 0002c550: 3330 3900 0000 c081 205e 7242 0000 0000  309..... ^rB....
 0002c560: 0000 f03f 25b3 d164 584c eebf 2f0f b083  ...?%..dXL../...
-0002c570: d28c f0bf 3b25 4a81 eafa 9dbf f55b 5193  ....;%J......[Q.
+0002c570: d28c f0bf 3c25 4a81 eafa 9dbf f55b 5193  ....<%J......[Q.
 0002c580: 0d9e bebf 45b8 ed12 7fec f1bf 1dd7 69e6  ....E.........i.
 0002c590: 2dc2 be3f 1055 2e05 4e13 bb3f 74c0 6981  -..?.U..N..?t.i.
 0002c5a0: 966f eb3f ea00 1055 2e05 4e13 bb3f 25b3  .o.?...U..N..?%.
-0002c5b0: d164 584c eebf 2f0f b083 d28c f0bf 3b25  .dXL../.......;%
+0002c5b0: d164 584c eebf 2f0f b083 d28c f0bf 3c25  .dXL../.......<%
 0002c5c0: 4a81 eafa 9dbf f55b 5193 0d9e bebf 45b8  J......[Q.....E.
 0002c5d0: ed12 7fec f1bf 1055 2e05 4e13 bb3f 25b3  .......U..N..?%.
-0002c5e0: d164 584c eebf 2f0f b083 d28c f0bf 3b25  .dXL../.......;%
+0002c5e0: d164 584c eebf 2f0f b083 d28c f0bf 3c25  .dXL../.......<%
 0002c5f0: 4a81 eafa 9dbf 0000 0000 0000 e07f 45b8  J.............E.
 0002c600: ed12 7fec f1bf 9d03 0000 6669 726d 2e33  ..........firm.3
 0002c610: 3039 0000 0040 faed d372 4200 0000 0000  09...@...rB.....
 0002c620: 00f0 3fec 48c3 5d5f 62d2 3fff 7cd9 7d89  ..?.H.]_b.?.|.}.
 0002c630: 31e9 bfe4 d0d0 b7cb 3aa5 bfe9 e738 3f2e  1.......:....8?.
 0002c640: 3af1 bf88 166b 12b6 07c4 3f57 ae60 3b4a  :....k....?W.`;J
 0002c650: d4f0 bff5 df77 dce6 cfef 3f74 c069 8196  .....w....?t.i..
@@ -11381,22 +11381,22 @@
 0002c740: a15b de3f e2f0 09b6 281a e13f 8b92 964a  .[.?....(..?...J
 0002c750: 149a ee3f 3462 9f6e 7ee6 0940 c8e6 b7a1  ...?4b.n~..@....
 0002c760: a7ea f1bf f091 1cbd 26b1 f13f 84a5 921a  ........&..?....
 0002c770: a15b de3f e2f0 09b6 281a e13f 0000 0000  .[.?....(..?....
 0002c780: 0000 e07f 9f03 0000 6669 726d 2e33 3130  ........firm.310
 0002c790: 0000 00c0 8120 5e72 4200 0000 0000 00f0  ..... ^rB.......
 0002c7a0: 3f87 c092 7fd9 679c 3f03 2876 1f01 3bf6  ?.....g.?.(v..;.
-0002c7b0: 3f5e a4e8 5789 53cc 3fb1 e8ec 677a dac0  ?^..W.S.?...gz..
+0002c7b0: 3f5f a4e8 5789 53cc 3fb1 e8ec 677a dac0  ?_..W.S.?...gz..
 0002c7c0: 3fa7 cfdd a762 7cae 3f76 889d d7f3 27ec  ?....b|.?v....'.
 0002c7d0: 3f52 ed6d 6ea4 6c03 40b6 d19e 1f38 1eeb  ?R.mn.l.@....8..
 0002c7e0: 3fec 0052 ed6d 6ea4 6c03 4087 c092 7fd9  ?..R.mn.l.@.....
-0002c7f0: 679c 3f03 2876 1f01 3bf6 3f5e a4e8 5789  g.?.(v..;.?^..W.
+0002c7f0: 679c 3f03 2876 1f01 3bf6 3f5f a4e8 5789  g.?.(v..;.?_..W.
 0002c800: 53cc 3fb1 e8ec 677a dac0 3fa7 cfdd a762  S.?...gz..?....b
 0002c810: 7cae 3f52 ed6d 6ea4 6c03 4087 c092 7fd9  |.?R.mn.l.@.....
-0002c820: 679c 3f03 2876 1f01 3bf6 3f5e a4e8 5789  g.?.(v..;.?^..W.
+0002c820: 679c 3f03 2876 1f01 3bf6 3f5f a4e8 5789  g.?.(v..;.?_..W.
 0002c830: 53cc 3fb1 e8ec 677a dac0 3fa7 cfdd a762  S.?...gz..?....b
 0002c840: 7cae 3fa0 0300 0066 6972 6d2e 3331 3000  |.?....firm.310.
 0002c850: 0000 40fa edd3 7242 0000 0000 0000 f03f  ..@...rB.......?
 0002c860: 7b86 3fc1 b3c4 eebf 7908 54e5 c0a4 9f3f  {.?.....y.T....?
 0002c870: dc86 bf89 a5dc d1bf 2a49 249a 4b47 e5bf  ........*I$.KG..
 0002c880: be93 655c 5648 f9bf 2cd8 b153 f95c 01c0  ..e\VH..,..S.\..
 0002c890: ba45 1eed d6db 00c0 b6d1 9e1f 381e eb3f  .E..........8..?
@@ -12717,22 +12717,22 @@
 00031ac0: b4a2 00c0 bc96 a735 3747 f4bf b440 0dd6  .......57G...@..
 00031ad0: b1e6 fe3f 9dec 012e 0bcb e73f 091e acf5  ...?.......?....
 00031ae0: bcc2 e9bf ee6f a435 61b8 d8bf 4254 059b  .....o.5a...BT..
 00031af0: b4a2 00c0 bc96 a735 3747 f4bf b440 0dd6  .......57G...@..
 00031b00: b1e6 fe3f 9dec 012e 0bcb e73f 091e acf5  ...?.......?....
 00031b10: bcc2 e9bf 0f04 0000 6669 726d 2e33 3437  ........firm.347
 00031b20: 0000 0040 faed d372 4200 0000 0000 00f0  ...@...rB.......
-00031b30: 3f14 76e9 6ef5 44e1 3f93 ddf5 8b9d a903  ?.v.n.D.?.......
+00031b30: 3f13 76e9 6ef5 44e1 3f93 ddf5 8b9d a903  ?.v.n.D.?.......
 00031b40: c0ea 7a95 9a83 ebf0 3f48 5473 4b83 58bc  ..z.....?HTsK.X.
 00031b50: bfac 1ae0 4367 4df1 bf5c 514a 87c2 bff7  ....CgM..\QJ....
 00031b60: 3f90 00dd a013 11df 3fe5 494e 9046 21d7  ?.......?.IN.F!.
-00031b70: 3f14 0190 00dd a013 11df 3f14 76e9 6ef5  ?.........?.v.n.
+00031b70: 3f14 0190 00dd a013 11df 3f13 76e9 6ef5  ?.........?.v.n.
 00031b80: 44e1 3f93 ddf5 8b9d a903 c0ea 7a95 9a83  D.?.........z...
 00031b90: ebf0 3f48 5473 4b83 58bc bfac 1ae0 4367  ..?HTsK.X.....Cg
-00031ba0: 4df1 bf90 00dd a013 11df 3f14 76e9 6ef5  M.........?.v.n.
+00031ba0: 4df1 bf90 00dd a013 11df 3f13 76e9 6ef5  M.........?.v.n.
 00031bb0: 44e1 3f93 ddf5 8b9d a903 c0ea 7a95 9a83  D.?.........z...
 00031bc0: ebf0 3f48 5473 4b83 58bc bfac 1ae0 4367  ..?HTsK.X.....Cg
 00031bd0: 4df1 bf10 0400 0066 6972 6d2e 3334 3700  M......firm.347.
 00031be0: 0000 000d 6949 7342 0000 0000 0000 f03f  ....iIsB.......?
 00031bf0: be2b de77 2b62 f93f aee1 2b41 2734 f0bf  .+.w+b.?..+A'4..
 00031c00: ab4e 4963 ea63 e13f 9088 3e3e fb3d f5bf  .NIc.c.?..>>.=..
 00031c10: 5f2a 9bfc b62b f3bf 2f83 9890 8779 e5bf  _*...+../....y..
@@ -12752,23 +12752,23 @@
 00031cf0: 0104 d599 4295 14fe 3f03 2c78 c2e0 60f6  ....B...?.,x..`.
 00031d00: bf6f f89e c63a 73db 3f18 8d1e c2da fcdb  .o...:s.?.......
 00031d10: 3f94 e0a3 d97c 96c9 3f1a 0e95 476f c3f3  ?....|..?...Go..
 00031d20: 3f04 d599 4295 14fe 3f03 2c78 c2e0 60f6  ?...B...?.,x..`.
 00031d30: bf6f f89e c63a 73db 3f00 0000 0000 00e0  .o...:s.?.......
 00031d40: 7f94 e0a3 d97c 96c9 3f00 0000 0000 00e0  .....|..?.......
 00031d50: 7f12 0400 0066 6972 6d2e 3334 3800 0000  .....firm.348...
-00031d60: 40fa edd3 7242 0000 0000 0000 f03f d851  @...rB.......?.Q
+00031d60: 40fa edd3 7242 0000 0000 0000 f03f d651  @...rB.......?.Q
 00031d70: b9c9 a448 e6bf df16 4932 1f34 c8bf 7599  ...H....I2.4..u.
 00031d80: f2ed 9cd3 d4bf fa8f 939f 4003 cf3f ea28  ..........@..?.(
-00031d90: 94f7 2a11 dbbf 3caf 6488 8e8b e73f 12ef  ..*...<.d....?..
+00031d90: 94f7 2a11 dbbf 3caf 6488 8e8b e73f 13ef  ..*...<.d....?..
 00031da0: bee1 d842 0940 b6c8 351d a57e f43f 1501  ...B.@..5..~.?..
-00031db0: 12ef bee1 d842 0940 d851 b9c9 a448 e6bf  .....B.@.Q...H..
+00031db0: 13ef bee1 d842 0940 d651 b9c9 a448 e6bf  .....B.@.Q...H..
 00031dc0: df16 4932 1f34 c8bf 7599 f2ed 9cd3 d4bf  ..I2.4..u.......
 00031dd0: fa8f 939f 4003 cf3f ea28 94f7 2a11 dbbf  ....@..?.(..*...
-00031de0: 12ef bee1 d842 0940 0000 0000 0000 e07f  .....B.@........
+00031de0: 13ef bee1 d842 0940 0000 0000 0000 e07f  .....B.@........
 00031df0: df16 4932 1f34 c8bf 7599 f2ed 9cd3 d4bf  ..I2.4..u.......
 00031e00: fa8f 939f 4003 cf3f ea28 94f7 2a11 dbbf  ....@..?.(..*...
 00031e10: 1304 0000 6669 726d 2e33 3438 0000 0000  ....firm.348....
 00031e20: 0d69 4973 4200 0000 0000 00f0 3fa4 11a8  .iIsB.......?...
 00031e30: 923f 0ee3 bfdb 08a6 f543 50b0 3fdc 13c1  .?.......CP.?...
 00031e40: 8ff0 63c3 3fa1 62ab 3a1d 0ed6 bf6c 3d2c  ..c.?.b.:....l=,
 00031e50: e286 33e0 bf8b 5b4d aa11 abf7 3f08 ee8d  ..3...[M....?...
@@ -17292,19 +17292,19 @@
 000438b0: cd4c 1fe4 3fa9 21be 2e19 0bd5 3f8e 236f  .L..?.!.....?.#o
 000438c0: 4e81 21d4 3fb0 021a 3dc5 b5f0 3f00 0000  N.!.?...=...?...
 000438d0: 0000 00e0 7f8e 0500 0066 6972 6d2e 3437  .........firm.47
 000438e0: 3500 0000 c081 205e 7242 0000 0000 0000  5..... ^rB......
 000438f0: f03f 5a80 91f3 3367 ecbf cdbc 2bff 9b30  .?Z...3g....+..0
 00043900: f33f 72b2 372b 92e9 e6bf db7e d297 3d2e  .?r.7+.....~..=.
 00043910: c5bf e922 d06c 5626 d23f 532b 29e9 81e6  ...".lV&.?S+)...
-00043920: ebbf f4bc 73ed 872b da3f a06f c434 b4e3  ....s..+.?.o.4..
-00043930: ec3f a201 f4bc 73ed 872b da3f 5a80 91f3  .?....s..+.?Z...
+00043920: ebbf f8bc 73ed 872b da3f a06f c434 b4e3  ....s..+.?.o.4..
+00043930: ec3f a201 f8bc 73ed 872b da3f 5a80 91f3  .?....s..+.?Z...
 00043940: 3367 ecbf cdbc 2bff 9b30 f33f 72b2 372b  3g....+..0.?r.7+
 00043950: 92e9 e6bf db7e d297 3d2e c5bf e922 d06c  .....~..=....".l
-00043960: 5626 d23f f4bc 73ed 872b da3f 5a80 91f3  V&.?..s..+.?Z...
+00043960: 5626 d23f f8bc 73ed 872b da3f 5a80 91f3  V&.?..s..+.?Z...
 00043970: 3367 ecbf cdbc 2bff 9b30 f33f 0000 0000  3g....+..0.?....
 00043980: 0000 e07f db7e d297 3d2e c5bf 0000 0000  .....~..=.......
 00043990: 0000 e07f 8f05 0000 6669 726d 2e34 3735  ........firm.475
 000439a0: 0000 0040 faed d372 4200 0000 0000 00f0  ...@...rB.......
 000439b0: 3fd1 e699 057d 91e0 bf7c 524d d942 70f4  ?....}...|RM.Bp.
 000439c0: 3ff4 c1c2 6701 96d0 bf89 fb0d f21d dac7  ?...g...........
 000439d0: bfde 1cc4 2254 82e3 3f53 199a 6e19 14f1  ...."T..?S..n...
@@ -27200,19 +27200,19 @@
 0006a3f0: b9f8 4142 14eb 3fb0 393e ea0a 28e6 bffd  ..AB..?.9>..(...
 0006a400: 30f4 57f7 a0ed bfde 7a1f b9a9 16ac bfb8  0.W.....z.......
 0006a410: 1e6d 0f9c 28f0 bfcc 0800 0066 6972 6d2e  .m..(......firm.
 0006a420: 3735 3100 0000 000d 6949 7342 0000 0000  751.....iIsB....
 0006a430: 0000 f03f 063c 6de1 96a4 d33f 03aa edf9  ...?.<m....?....
 0006a440: e6e9 a23f f11b d96d 423a febf 8fc9 7626  ...?...mB:....v&
 0006a450: 1f3b c0bf 0070 3f97 7369 aebf 154e a5c0  .;...p?.si...N..
-0006a460: 8c9d e7bf 36f9 70a3 3d2c e5bf faaa e81e  ....6.p.=,......
-0006a470: a031 e23f d502 36f9 70a3 3d2c e5bf 063c  .1.?..6.p.=,...<
+0006a460: 8c9d e7bf 37f9 70a3 3d2c e5bf faaa e81e  ....7.p.=,......
+0006a470: a031 e23f d502 37f9 70a3 3d2c e5bf 063c  .1.?..7.p.=,...<
 0006a480: 6de1 96a4 d33f 03aa edf9 e6e9 a23f f11b  m....?.......?..
 0006a490: d96d 423a febf 8fc9 7626 1f3b c0bf 0070  .mB:....v&.;...p
-0006a4a0: 3f97 7369 aebf 36f9 70a3 3d2c e5bf 063c  ?.si..6.p.=,...<
+0006a4a0: 3f97 7369 aebf 37f9 70a3 3d2c e5bf 063c  ?.si..7.p.=,...<
 0006a4b0: 6de1 96a4 d33f 03aa edf9 e6e9 a23f f11b  m....?.......?..
 0006a4c0: d96d 423a febf 8fc9 7626 1f3b c0bf 0070  .mB:....v&.;...p
 0006a4d0: 3f97 7369 aebf cd08 0000 6669 726d 2e37  ?.si......firm.7
 0006a4e0: 3532 0000 00c0 8120 5e72 4200 0000 0000  52..... ^rB.....
 0006a4f0: 00f0 3fce 928e 342b 59e9 bf44 69cb e534  ..?...4+Y..Di..4
 0006a500: cde4 bf5c 6d83 bea7 adf0 bf57 5818 b497  ...\m......WX...
 0006a510: 34db bf7a f009 ee38 e5a5 3f3f afa6 1b85  4..z...8..??....
@@ -28393,22 +28393,22 @@
 0006ee80: 6df5 bf00 0000 0000 00e0 7fbc eb44 28fd  m............D(.
 0006ee90: 83f5 3f6c 4147 0e0f ace5 bf00 0000 0000  ..?lAG..........
 0006eea0: 00e0 7f5f 11e2 2234 8bed bf1b 995a 536e  ..._.."4.....ZSn
 0006eeb0: 6df5 bf30 0900 0066 6972 6d2e 3738 3500  m..0...firm.785.
 0006eec0: 0000 c081 205e 7242 0000 0000 0000 f03f  .... ^rB.......?
 0006eed0: 8205 9952 249d ee3f 3317 b24d 5c59 c53f  ...R$..?3..M\Y.?
 0006eee0: b0ac 4808 6a8e d83f 4edc acd5 7a91 d03f  ..H.j..?N...z..?
-0006eef0: 1d45 8aa8 929e ecbf 1e99 8f76 1592 f13f  .E.........v...?
+0006eef0: 1c45 8aa8 929e ecbf 1e99 8f76 1592 f13f  .E.........v...?
 0006ef00: 0926 0af6 83bc 1140 8d09 8730 78d2 ee3f  .&.....@...0x..?
 0006ef10: fa02 0000 0000 0000 e07f 8205 9952 249d  .............R$.
 0006ef20: ee3f 3317 b24d 5c59 c53f b0ac 4808 6a8e  .?3..M\Y.?..H.j.
-0006ef30: d83f 4edc acd5 7a91 d03f 1d45 8aa8 929e  .?N...z..?.E....
+0006ef30: d83f 4edc acd5 7a91 d03f 1c45 8aa8 929e  .?N...z..?.E....
 0006ef40: ecbf 0926 0af6 83bc 1140 8205 9952 249d  ...&.....@...R$.
 0006ef50: ee3f 3317 b24d 5c59 c53f 0000 0000 0000  .?3..M\Y.?......
-0006ef60: e07f 4edc acd5 7a91 d03f 1d45 8aa8 929e  ..N...z..?.E....
+0006ef60: e07f 4edc acd5 7a91 d03f 1c45 8aa8 929e  ..N...z..?.E....
 0006ef70: ecbf 3109 0000 6669 726d 2e37 3835 0000  ..1...firm.785..
 0006ef80: 0040 faed d372 4200 0000 0000 00f0 3fb8  .@...rB.......?.
 0006ef90: cd03 806c 2ce8 3fe9 c4a3 3279 e3f2 3f2a  ...l,.?...2y..?*
 0006efa0: c005 839a b7cc 3f4a 2b67 b8da b0b2 3fa4  ......?J+g....?.
 0006efb0: 5ab8 7062 73f1 3f26 1c5a 4f8c 71e8 bf2d  Z.pbs.?&.ZO.q..-
 0006efc0: be03 120a be0e 408d 0987 3078 d2ee 3ffa  ......@...0x..?.
 0006efd0: 022d be03 120a be0e 40b8 cd03 806c 2ce8  .-......@....l,.
@@ -28428,23 +28428,23 @@
 0006f0b0: a229 0d5d e127 65bf be0f 108b 7828 f1bf  .).].'e.....x(..
 0006f0c0: f674 01b7 56b4 0b40 89d2 508c a93c e73f  .t..V..@..P..<.?
 0006f0d0: 0c1f d039 7e3d dbbf 3828 b4f1 04e7 eb3f  ...9~=..8(.....?
 0006f0e0: 0000 0000 0000 e07f be0f 108b 7828 f1bf  ............x(..
 0006f0f0: 3309 0000 6669 726d 2e37 3836 0000 00c0  3...firm.786....
 0006f100: 8120 5e72 4200 0000 0000 00f0 3f16 3653  . ^rB.......?.6S
 0006f110: 19ba 04ef bf4a 2e47 df6f e0d3 3f3b 6e0a  .....J.G.o..?;n.
-0006f120: 653d d5b5 3f40 f083 c363 9bef bfef 5d85  e=..?@...c....].
+0006f120: 653d d5b5 3f40 f083 c363 9bef bfee 5d85  e=..?@...c....].
 0006f130: 73ef d5df 3f72 1f66 4043 e2da bfc8 c37d  s...?r.f@C.....}
 0006f140: 7267 9bfd bf61 d271 6d53 53f7 3ffb 02c8  rg...a.qmSS.?...
 0006f150: c37d 7267 9bfd bf16 3653 19ba 04ef bf4a  .}rg....6S.....J
 0006f160: 2e47 df6f e0d3 3f3b 6e0a 653d d5b5 3f40  .G.o..?;n.e=..?@
-0006f170: f083 c363 9bef bfef 5d85 73ef d5df 3fc8  ...c....].s...?.
+0006f170: f083 c363 9bef bfee 5d85 73ef d5df 3fc8  ...c....].s...?.
 0006f180: c37d 7267 9bfd bf16 3653 19ba 04ef bf4a  .}rg....6S.....J
 0006f190: 2e47 df6f e0d3 3f3b 6e0a 653d d5b5 3f00  .G.o..?;n.e=..?.
-0006f1a0: 0000 0000 00e0 7fef 5d85 73ef d5df 3f34  ........].s...?4
+0006f1a0: 0000 0000 00e0 7fee 5d85 73ef d5df 3f34  ........].s...?4
 0006f1b0: 0900 0066 6972 6d2e 3738 3600 0000 40fa  ...firm.786...@.
 0006f1c0: edd3 7242 0000 0000 0000 f03f faf7 e570  ..rB.......?...p
 0006f1d0: 3bdf b93f 8f17 0f63 310b f83f afb9 4e76  ;..?...c1..?..Nv
 0006f1e0: 887d d83f a1f0 5d3d afab f2bf a013 f95f  .}.?..]=......._
 0006f1f0: ac9d f73f a90e 73e7 ac6f b9bf 60be ae69  ...?..s..o..`..i
 0006f200: 2c65 9f3f 61d2 716d 5353 f73f fb02 60be  ,e.?a.qmSS.?..`.
 0006f210: ae69 2c65 9f3f faf7 e570 3bdf b93f 8f17  .i,e.?...p;..?..
@@ -34145,23 +34145,23 @@
 00085600: c09d 5408 ad5d 5df8 bfe8 c022 ab3d 5ae2  ..T..]]....".=Z.
 00085610: bf7f 3bf8 b76d 39bf bf85 de46 3050 93e5  ..;..m9....F0P..
 00085620: 3f74 3f83 5f1d 05fa 3ffb 4599 31dc b706  ?t?._...?.E.1...
 00085630: c09d 5408 ad5d 5df8 bf00 0000 0000 00e0  ..T..]].........
 00085640: 7f00 0000 0000 00e0 7f00 0000 0000 00e0  ................
 00085650: 7f12 0b00 0066 6972 6d2e 3934 3500 0000  .....firm.945...
 00085660: 000d 6949 7342 0000 0000 0000 f03f 8970  ..iIsB.......?.p
-00085670: ca88 6448 e4bf c948 4867 fdc4 fa3f c15d  ..dH...HHg...?.]
+00085670: ca88 6448 e4bf c948 4867 fdc4 fa3f c05d  ..dH...HHg...?.]
 00085680: 67b9 775e 963f a971 4ace 038f e93f b407  g.w^.?.qJ....?..
 00085690: 598b f75a efbf 8f5b c77b 96f2 e33f b2e5  Y..Z...[.{...?..
 000856a0: a6e3 6725 0440 aa2c d3db 8f33 eb3f ac03  ..g%.@.,...3.?..
 000856b0: b2e5 a6e3 6725 0440 8970 ca88 6448 e4bf  ....g%.@.p..dH..
-000856c0: c948 4867 fdc4 fa3f c15d 67b9 775e 963f  .HHg...?.]g.w^.?
+000856c0: c948 4867 fdc4 fa3f c05d 67b9 775e 963f  .HHg...?.]g.w^.?
 000856d0: a971 4ace 038f e93f b407 598b f75a efbf  .qJ....?..Y..Z..
 000856e0: b2e5 a6e3 6725 0440 8970 ca88 6448 e4bf  ....g%.@.p..dH..
-000856f0: c948 4867 fdc4 fa3f c15d 67b9 775e 963f  .HHg...?.]g.w^.?
+000856f0: c948 4867 fdc4 fa3f c05d 67b9 775e 963f  .HHg...?.]g.w^.?
 00085700: 0000 0000 0000 e07f b407 598b f75a efbf  ..........Y..Z..
 00085710: 130b 0000 6669 726d 2e39 3436 0000 00c0  ....firm.946....
 00085720: 8120 5e72 4200 0000 0000 00f0 3fb1 2460  . ^rB.......?.$`
 00085730: 0703 795e bf0f d3a2 39de 11e7 bf5b 722d  ..y^....9....[r-
 00085740: feaa a7ba 3faa 562f 0bcd 7f04 c010 8844  ....?.V/.......D
 00085750: 84df fed3 3fb6 02ff bedb 5ef3 3f89 4079  ....?.....^.?.@y
 00085760: 4f39 2405 c0cc 2ad6 6648 f9e7 3fad 0389  O9$...*.fH..?...
@@ -34181,23 +34181,23 @@
 00085840: facd 8ae6 9bbf f08f 56ea 505e eabf 0000  ........V.P^....
 00085850: 0000 0000 e07f 1b28 cd27 68b9 da3f 30e9  .......(.'h..?0.
 00085860: 64fc a0d1 b4bf ced0 5e74 7ba2 dcbf 564b  d.......^t{...VK
 00085870: facd 8ae6 9bbf f08f 56ea 505e eabf f959  ........V.P^...Y
 00085880: 3958 a106 f23f 1b28 cd27 68b9 da3f 150b  9X...?.(.'h..?..
 00085890: 0000 6669 726d 2e39 3436 0000 0000 0d69  ..firm.946.....i
 000858a0: 4973 4200 0000 0000 00f0 3f95 1aaf 0cfe  IsB.......?.....
-000858b0: 66ce 3f22 1fc9 5c8d ebc9 bf3c 58e2 a69a  f.?"..\....<X...
+000858b0: 66ce 3f22 1fc9 5c8d ebc9 bf3a 58e2 a69a  f.?"..\....:X...
 000858c0: ceef 3f88 e29e 206c 39fa bf2b b4e4 99fc  ..?... l9..+....
-000858d0: 59a8 3f44 e4e0 a8e3 77d6 3fa4 3462 23eb  Y.?D....w.?.4b#.
-000858e0: 8dfc bfcc 2ad6 6648 f9e7 3fad 03a4 3462  ....*.fH..?...4b
+000858d0: 59a8 3f44 e4e0 a8e3 77d6 3fa6 3462 23eb  Y.?D....w.?.4b#.
+000858e0: 8dfc bfcc 2ad6 6648 f9e7 3fad 03a6 3462  ....*.fH..?...4b
 000858f0: 23eb 8dfc bf95 1aaf 0cfe 66ce 3f22 1fc9  #.........f.?"..
-00085900: 5c8d ebc9 bf3c 58e2 a69a ceef 3f88 e29e  \....<X.....?...
-00085910: 206c 39fa bf2b b4e4 99fc 59a8 3fa4 3462   l9..+....Y.?.4b
+00085900: 5c8d ebc9 bf3a 58e2 a69a ceef 3f88 e29e  \....:X.....?...
+00085910: 206c 39fa bf2b b4e4 99fc 59a8 3fa6 3462   l9..+....Y.?.4b
 00085920: 23eb 8dfc bf95 1aaf 0cfe 66ce 3f22 1fc9  #.........f.?"..
-00085930: 5c8d ebc9 bf3c 58e2 a69a ceef 3f88 e29e  \....<X.....?...
+00085930: 5c8d ebc9 bf3a 58e2 a69a ceef 3f88 e29e  \....:X.....?...
 00085940: 206c 39fa bf2b b4e4 99fc 59a8 3f16 0b00   l9..+....Y.?...
 00085950: 0066 6972 6d2e 3934 3700 0000 c081 205e  .firm.947..... ^
 00085960: 7242 0000 0000 0000 f03f 856a 7662 7a46  rB.......?.jvbzF
 00085970: d43f 77c7 c804 99d8 c33f df55 2fa4 70bf  .?w......?.U/.p.
 00085980: f0bf ebe5 dc3e d0ef ddbf 30f6 6ab8 5190  .....>....0.j.Q.
 00085990: ec3f 4bda 1dd2 784d d0bf fcb2 ec23 c75f  .?K...xM.....#._
 000859a0: 03c0 fdf0 556f 257e 0140 ae03 fcb2 ec23  ....Uo%~.@.....#
@@ -35196,20 +35196,20 @@
 000897b0: bfc4 b52e 40f2 53db bf6a 01fb 6b5a 23f3  ....@.S..j..kZ#.
 000897c0: 3f8d c8b7 372f 82f0 bfc4 4e4a c0a0 f708  ?...7/....NJ....
 000897d0: 402d 0aff 31bd cef9 bf1d 3950 77e1 c1fa  @-..1.....9Pw...
 000897e0: bfc4 b52e 40f2 53db bf6a 01fb 6b5a 23f3  ....@.S..j..kZ#.
 000897f0: 3f00 0000 0000 00e0 7f6a 0b00 0066 6972  ?........j...fir
 00089800: 6d2e 3937 3500 0000 c081 205e 7242 0000  m.975..... ^rB..
 00089810: 0000 0000 f03f cef5 7e49 0587 d8bf c04d  .....?..~I.....M
-00089820: 5fdf ca6b e8bf b753 c792 0433 e53f 96a2  _..k...S...3.?..
+00089820: 5fdf ca6b e8bf b653 c792 0433 e53f 96a2  _..k...S...3.?..
 00089830: 4f91 a447 e83f 47a3 77ab 2b9b e9bf 2ae3  O..G.?G.w.+...*.
 00089840: 27c8 814c f13f 6e19 45a8 ea28 f63f af2f  '..L.?n.E..(.?./
 00089850: d244 decc f73f cd03 6e19 45a8 ea28 f63f  .D...?..n.E..(.?
 00089860: cef5 7e49 0587 d8bf c04d 5fdf ca6b e8bf  ..~I.....M_..k..
-00089870: b753 c792 0433 e53f 96a2 4f91 a447 e83f  .S...3.?..O..G.?
+00089870: b653 c792 0433 e53f 96a2 4f91 a447 e83f  .S...3.?..O..G.?
 00089880: 47a3 77ab 2b9b e9bf 6e19 45a8 ea28 f63f  G.w.+...n.E..(.?
 00089890: 0000 0000 0000 e07f c04d 5fdf ca6b e8bf  .........M_..k..
 000898a0: 0000 0000 0000 e07f 0000 0000 0000 e07f  ................
 000898b0: 0000 0000 0000 e07f 6b0b 0000 6669 726d  ........k...firm
 000898c0: 2e39 3735 0000 0040 faed d372 4200 0000  .975...@...rB...
 000898d0: 0000 00f0 3fc5 a845 d6b3 c400 c0d8 7a15  ....?..E......z.
 000898e0: 3e33 64da 3fdf c1ba 815e 4dc2 3f99 1190  >3d.?....^M.?...
@@ -35232,22 +35232,22 @@
 000899f0: 7d9e 741f a73f 08cb 7b77 9ee0 e23f 30e2  }.t..?..{w...?0.
 00089a00: 4d63 0b03 f9bf ddd1 ab1e 8c95 f5bf bea3  Mc..............
 00089a10: e225 659c f73f 0447 4d8b ee54 ec3f f76f  .%e..?.GM..T.?.o
 00089a20: 7d9e 741f a73f 08cb 7b77 9ee0 e23f 0000  }.t..?..{w...?..
 00089a30: 0000 0000 e07f 6d0b 0000 6669 726d 2e39  ......m...firm.9
 00089a40: 3736 0000 00c0 8120 5e72 4200 0000 0000  76..... ^rB.....
 00089a50: 00f0 3f42 c74d 6aad a1f1 3f55 1b1a ac79  ..?B.Mj...?U...y
-00089a60: c3f0 3fbd d04b e2d8 b0bc bf58 f88f 22dc  ..?..K.....X..".
+00089a60: c3f0 3fbb d04b e2d8 b0bc bf58 f88f 22dc  ..?..K.....X..".
 00089a70: 7bf3 3fde 1aae 1243 92f2 bfc6 e778 3f04  {.?....C.....x?.
-00089a80: bef0 bfe9 cf3d d05f 1cf3 bf81 94b5 ca84  .....=._........
-00089a90: 40f0 3fce 03e9 cf3d d05f 1cf3 bf42 c74d  @.?....=._...B.M
-00089aa0: 6aad a1f1 3f00 0000 0000 00e0 7fbd d04b  j...?..........K
+00089a80: bef0 bfe8 cf3d d05f 1cf3 bf81 94b5 ca84  .....=._........
+00089a90: 40f0 3fce 03e8 cf3d d05f 1cf3 bf42 c74d  @.?....=._...B.M
+00089aa0: 6aad a1f1 3f00 0000 0000 00e0 7fbb d04b  j...?..........K
 00089ab0: e2d8 b0bc bf58 f88f 22dc 7bf3 3fde 1aae  .....X..".{.?...
-00089ac0: 1243 92f2 bfe9 cf3d d05f 1cf3 bf42 c74d  .C.....=._...B.M
-00089ad0: 6aad a1f1 3f55 1b1a ac79 c3f0 3fbd d04b  j...?U...y..?..K
+00089ac0: 1243 92f2 bfe8 cf3d d05f 1cf3 bf42 c74d  .C.....=._...B.M
+00089ad0: 6aad a1f1 3f55 1b1a ac79 c3f0 3fbb d04b  j...?U...y..?..K
 00089ae0: e2d8 b0bc bf58 f88f 22dc 7bf3 3fde 1aae  .....X..".{.?...
 00089af0: 1243 92f2 bf6e 0b00 0066 6972 6d2e 3937  .C...n...firm.97
 00089b00: 3600 0000 40fa edd3 7242 0000 0000 0000  6...@...rB......
 00089b10: f03f a691 a349 fb73 e6bf 87f4 b864 5ec3  .?...I.s.....d^.
 00089b20: e33f c93f 1f60 33f7 ecbf 0a49 2412 6551  .?.?.`3....I$.eQ
 00089b30: fbbf fc9e 0547 aee4 e9bf b867 ac63 9e9a  .....G.....g.c..
 00089b40: c73f 5844 043c 757e 0bc0 8194 b5ca 8440  .?XD.<u~.......@
```

### Comparing `linearmodels-4.8/linearmodels/tests/panel/results/execute-stata-simulated-data.py` & `linearmodels-4.9/linearmodels/tests/panel/results/execute-stata-simulated-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/panel/test_results.py` & `linearmodels-4.9/linearmodels/tests/panel/test_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import OrderedDict
 from itertools import product
 
 import pytest
 import statsmodels.api as sm
+from pandas.testing import assert_series_equal
 
-from linearmodels.compat.pandas import assert_series_equal
 from linearmodels.datasets import wage_panel
 from linearmodels.iv.model import IV2SLS
 from linearmodels.panel.data import PanelData
 from linearmodels.panel.model import PanelOLS, PooledOLS, RandomEffects
 from linearmodels.panel.results import compare
 from linearmodels.tests.panel._utility import generate_data, datatypes
 
@@ -87,14 +87,15 @@
     res = mod.fit()
     mod2 = IV2SLS(mod.dependent.dataframe, mod.exog.dataframe, None, None)
     res2 = mod2.fit()
     with pytest.raises(TypeError):
         compare(dict(model1=res, model2=res2))
 
 
+@pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
 def test_predict(generated_data):
     mod = PanelOLS(generated_data.y, generated_data.x, entity_effects=True)
     res = mod.fit()
     pred = res.predict()
     nobs = mod.dependent.dataframe.shape[0]
     assert list(pred.columns) == ['fitted_values']
     assert pred.shape == (nobs, 1)
@@ -120,14 +121,15 @@
     assert_series_equal(pred.estimated_effects, res.estimated_effects.iloc[:, 0])
     assert_series_equal(pred.idiosyncratic, res.idiosyncratic.iloc[:, 0])
     pred = res.predict(effects=True, idiosyncratic=True, missing=True)
     assert list(pred.columns) == ['fitted_values', 'estimated_effects', 'idiosyncratic']
     assert pred.shape == (PanelData(generated_data.y).dataframe.shape[0], 3)
 
 
+@pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
 def test_predict_no_selection(generated_data):
     mod = PanelOLS(generated_data.y, generated_data.x, entity_effects=True)
     res = mod.fit()
     with pytest.raises(ValueError):
         res.predict(fitted=False)
     with pytest.raises(ValueError):
         res.predict(fitted=False, effects=False, idiosyncratic=False, missing=True)
```

### Comparing `linearmodels-4.8/linearmodels/tests/datasets/test_datasets.py` & `linearmodels-4.9/linearmodels/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/test_examples.py` & `linearmodels-4.9/linearmodels/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_gmm.py` & `linearmodels-4.9/linearmodels/tests/iv/test_gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_against_stata.py` & `linearmodels-4.9/linearmodels/tests/iv/test_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_covariance.py` & `linearmodels-4.9/linearmodels/tests/iv/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/_utility.py` & `linearmodels-4.9/linearmodels/tests/iv/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_data.py` & `linearmodels-4.9/linearmodels/tests/iv/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     import xarray as xr
 
     MISSING_XARRAY = False
 except ImportError:
     MISSING_XARRAY = True
 
-from linearmodels.compat.pandas import assert_frame_equal, assert_series_equal
+from pandas.testing import assert_frame_equal, assert_series_equal
 from linearmodels.iv.data import IVData
 
 
 class TestDataHandler(object):
     def test_numpy_2d(self):
         x = np.empty((10, 2))
         xdh = IVData(x)
@@ -172,15 +172,15 @@
         assert dh.rows == list(index)
         assert_equal(dh.pandas['cat.b'].values, (cat == 'b').astype(np.float))
         assert_equal(dh.pandas['cat.c'].values, (cat == 'c').astype(np.float))
 
     def test_categorical_no_conversion(self):
         index = pd.date_range('2017-01-01', periods=10)
         cat = pd.Categorical(['a', 'b', 'a', 'b', 'a', 'a', 'b', 'c', 'c', 'a'])
-        s = pd.Series({'cat': cat}, index=index, name='cat')
+        s = pd.Series(cat, index=index, name='cat')
         dh = IVData(s, convert_dummies=False)
         assert dh.ndim == 2
         assert dh.shape == (10, 1)
         assert dh.cols == ['cat']
         assert dh.rows == list(index)
         df = pd.DataFrame(s)
         assert_frame_equal(dh.pandas, df)
```

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_missing_data.py` & `linearmodels-4.9/linearmodels/tests/iv/test_missing_data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_model.py` & `linearmodels-4.9/linearmodels/tests/iv/test_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -338,7 +338,25 @@
 
 def test_gmm_str(data):
     mod = IVGMM(data.dep, data.exog, data.endog, data.instr)
     str(mod.fit(cov_type='unadjusted'))
     str(mod.fit(cov_type='robust'))
     str(mod.fit(cov_type='clustered', clusters=data.clusters))
     str(mod.fit(cov_type='kernel'))
+
+
+def test_gmm_cue_optimization_options(data):
+    mod = IVGMMCUE(data.dep, data.exog, data.endog, data.instr)
+    res_none = mod.fit(display=False)
+    opt_options = dict(method='BFGS', options={'disp': False})
+    res_bfgs = mod.fit(display=False, opt_options=opt_options)
+    opt_options = dict(method='L-BFGS-B', options={'disp': False})
+    res_lbfgsb = mod.fit(display=False, opt_options=opt_options)
+    assert res_none.iterations > 2
+    assert res_bfgs.iterations > 2
+    assert res_lbfgsb.iterations > 2
+
+    mod2 = IVGMM(data.dep, data.exog, data.endog, data.instr)
+    res2 = mod2.fit()
+    assert res_none.j_stat.stat <= res2.j_stat.stat
+    assert res_bfgs.j_stat.stat <= res2.j_stat.stat
+    assert res_lbfgsb.j_stat.stat <= res2.j_stat.stat
```

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_formulas.py` & `linearmodels-4.9/linearmodels/tests/iv/test_formulas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
-import pandas as pd
 import pytest
 from numpy.testing import assert_allclose, assert_equal
+from pandas import DataFrame, Categorical
+from pandas.testing import assert_frame_equal
 
-from linearmodels.compat.pandas import assert_frame_equal
+from linearmodels.compat.pandas import concat
 from linearmodels.formula import iv_2sls, iv_gmm, iv_gmm_cue, iv_liml
 from linearmodels.iv import IV2SLS, IVGMM, IVGMMCUE, IVLIML
 
 
 @pytest.fixture(scope='module',
                 params=list(zip([IV2SLS, IVLIML, IVGMMCUE, IVGMM],
                                 [iv_2sls, iv_liml, iv_gmm_cue, iv_gmm])))
@@ -45,15 +46,15 @@
     z = v[:, k:k + p]
     e = v[:, [-1]]
     params = np.arange(1, k + 1) / k
     params = params[:, None]
     y = x @ params + e
     cols = ['y'] + ['x' + str(i) for i in range(1, 6)]
     cols += ['z' + str(i) for i in range(1, 4)]
-    data = pd.DataFrame(np.c_[y, x, z], columns=cols)
+    data = DataFrame(np.c_[y, x, z], columns=cols)
     data['Intercept'] = 1.0
     data['weights'] = np.random.chisquare(10, size=data.shape[0]) / 10
     return data
 
 
 def test_formula(data, model_and_func, formula):
     model, func = model_and_func
@@ -160,16 +161,16 @@
 
 
 def test_categorical(model_and_func):
     formula = 'y ~ 1 + d + x1'
     y = np.random.randn(1000)
     x1 = np.random.randn(1000)
     d = np.random.randint(0, 4, 1000)
-    d = pd.Categorical(d)
-    data = pd.DataFrame({'y': y, 'x1': x1, 'd': d})
+    d = Categorical(d)
+    data = DataFrame({'y': y, 'x1': x1, 'd': d})
     data['Intercept'] = 1.0
     model, func = model_and_func
     mod = model.from_formula(formula, data)
     res3 = mod.fit()
     res2 = func(formula, data).fit()
     res = model(data.y, data[['Intercept', 'x1', 'd']], None, None).fit()
 
@@ -195,15 +196,15 @@
     fmla = 'y ~ 1 + sigmoid(x3) + x4 + [x1 + x2 ~ z1 + z2 + z3] + np.exp(x5)'
     mod = model.from_formula(fmla, data)
     res = mod.fit()
 
     dep = data.y
     exog = [data[['Intercept']], sigmoid(data[['x3']]), data[['x4']],
             np.exp(data[['x5']])]
-    exog = pd.concat(exog, 1)
+    exog = concat(exog, 1)
     endog = data[['x1', 'x2']]
     instr = data[['z1', 'z2', 'z3']]
     mod = model(dep, exog, endog, instr)
     res2 = mod.fit()
     assert_equal(res.params.values, res2.params.values)
     res3 = func(fmla, data).fit()
     assert_equal(res.params.values, res3.params.values)
@@ -216,15 +217,15 @@
     model, func = model_and_func
     fmla = 'y ~ 1 + sigmoid(x3) + x4 + [x1 + x2 ~ z1 + z2 + z3] + np.exp(x5)'
     mod = model.from_formula(fmla, data)
     res = mod.fit()
 
     exog = [data[['Intercept']], sigmoid(data[['x3']]), data[['x4']],
             np.exp(data[['x5']])]
-    exog = pd.concat(exog, 1)
+    exog = concat(exog, 1)
     endog = data[['x1', 'x2']]
     pred = res.predict(exog, endog)
     pred2 = res.predict(data=data)
     assert_frame_equal(pred, pred2)
     assert_allclose(res.fitted_values, pred)
 
     res2 = func(fmla, data).fit()
```

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_postestimation.py` & `linearmodels-4.9/linearmodels/tests/iv/test_postestimation.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/stata-iv-housing-results.txt` & `linearmodels-4.9/linearmodels/tests/iv/results/stata-iv-housing-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/execute-stata.py` & `linearmodels-4.9/linearmodels/tests/iv/results/execute-stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/simulated-data.dta` & `linearmodels-4.9/linearmodels/tests/iv/results/simulated-data.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/stata-iv-simulated-results.txt` & `linearmodels-4.9/linearmodels/tests/iv/results/stata-iv-simulated-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/read_stata_results.py` & `linearmodels-4.9/linearmodels/tests/iv/results/read_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/simulated-test-data.py` & `linearmodels-4.9/linearmodels/tests/iv/results/simulated-test-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/execute-stata-simulated-data.py` & `linearmodels-4.9/linearmodels/tests/iv/results/execute-stata-simulated-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/results/housing.csv` & `linearmodels-4.9/linearmodels/tests/iv/results/housing.csv`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/iv/test_results.py` & `linearmodels-4.9/linearmodels/tests/iv/test_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
+from pandas import DataFrame
+from pandas.testing import assert_series_equal
 
-from linearmodels.compat.pandas import assert_series_equal
 from linearmodels.iv.data import IVData
 from linearmodels.iv.model import IV2SLS, IVGMM, IVGMMCUE, IVLIML
 from linearmodels.tests.iv._utility import generate_data
 from linearmodels.tests.panel._utility import assert_frame_similar
 
 
 @pytest.fixture(scope='module')
@@ -61,20 +61,20 @@
 
 def test_fitted_predict(data, model):
     mod = model(data.dep, None, data.endog, data.instr)
     res = mod.fit()
     assert_series_equal(res.idiosyncratic, res.resids)
     y = mod.dependent.pandas
     expected = y.values - res.resids.values[:, None]
-    expected = pd.DataFrame(expected, y.index, ['fitted_values'])
+    expected = DataFrame(expected, y.index, ['fitted_values'])
     assert_frame_similar(expected, res.fitted_values)
     assert_allclose(expected, res.fitted_values)
     pred = res.predict()
     nobs = res.resids.shape[0]
-    assert isinstance(pred, pd.DataFrame)
+    assert isinstance(pred, DataFrame)
     assert pred.shape == (nobs, 1)
     pred = res.predict(idiosyncratic=True, missing=True)
     nobs = IVData(data.dep).pandas.shape[0]
     assert pred.shape == (nobs, 2)
     assert list(pred.columns) == ['fitted_values', 'residual']
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_utility.py` & `linearmodels-4.9/linearmodels/tests/system/test_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     lc = LinearConstraint(r, require_pandas=False)
     assert hex(id(lc)) in lc.__repr__()
     assert '10 constraints' in lc.__repr__()
     assert isinstance(lc.q, pd.Series)
     assert np.all(lc.q == 0)
     assert lc.q.shape == (10,)
     assert isinstance(lc.r, pd.DataFrame)
-    assert np.all(lc.r == np.eye(10))
+    assert np.all(lc.r.values == np.eye(10))
 
 
 def test_blocked_full_inner_product():
     k = 3
     t = 100
     kt = k * t
     x = np.random.randn(kt, kt)
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_gmm.py` & `linearmodels-4.9/linearmodels/tests/system/test_gmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections import OrderedDict
 from itertools import product
 
 import numpy as np
-import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
+from pandas import DataFrame, Series
+from pandas.testing import assert_frame_equal, assert_series_equal
 
-from linearmodels.compat.pandas import assert_frame_equal, assert_series_equal
+from linearmodels.compat.pandas import concat
 from linearmodels.iv.covariance import kernel_weight_parzen
 from linearmodels.system import IV3SLS, IVSystemGMM
 from linearmodels.system.gmm import HeteroskedasticWeightMatrix, HomoskedasticWeightMatrix, \
     KernelWeightMatrix
 from linearmodels.tests.system._utility import generate_3sls_data_v2, simple_gmm
 from linearmodels.utility import AttrDict
 
@@ -96,36 +97,36 @@
     df = []
     for i, key in enumerate(data.eqns):
         eqn = data.eqns[key]
         dep = eqn.dependent
         ex = eqn.exog
         en = eqn.endog
         instr = eqn.instruments
-        dep = pd.DataFrame(dep, columns=['dep_{0}'.format(i)])
+        dep = DataFrame(dep, columns=['dep_{0}'.format(i)])
         has_const = False
         if np.any(np.all(ex == 1, 0)):
             ex = ex[:, 1:]
             has_const = True
-        ex = pd.DataFrame(ex, columns=['ex_{0}_{1}'.format(i, j) for j in range(ex.shape[1])])
-        en = pd.DataFrame(en, columns=['en_{0}_{1}'.format(i, j) for j in range(en.shape[1])])
-        instr = pd.DataFrame(instr, columns=['instr_{0}_{1}'.format(i, j)
-                                             for j in range(ex.shape[1])])
+        ex = DataFrame(ex, columns=['ex_{0}_{1}'.format(i, j) for j in range(ex.shape[1])])
+        en = DataFrame(en, columns=['en_{0}_{1}'.format(i, j) for j in range(en.shape[1])])
+        instr = DataFrame(instr, columns=['instr_{0}_{1}'.format(i, j)
+                                          for j in range(ex.shape[1])])
         fmla = ''.join(dep.columns) + ' ~  '
         if has_const:
             fmla += ' 1 + '
         fmla += ' + '.join(ex.columns) + ' + ['
         fmla += ' + '.join(en.columns) + ' ~ '
         fmla += ' + '.join(instr.columns) + ' ] '
         formula.append(fmla)
         df.extend([dep, ex, en, instr])
     from collections import OrderedDict
     formulas = OrderedDict()
     for i, f in enumerate(formula):
         formulas['eq{0}'.format(i)] = f
-    df = pd.concat(df, 1)
+    df = concat(df, 1)
     formula_mod = IVSystemGMM.from_formula(formulas, df, weight_type='unadjusted')
     res = mod.fit(cov_type='unadjusted')
     formula_res = formula_mod.fit(cov_type='unadjusted')
     assert_allclose(res.params, formula_res.params)
 
 
 def test_formula_equivalence_weights(data):
@@ -144,32 +145,32 @@
     formulas = OrderedDict()
     for i, key in enumerate(data.eqns):
         eqn = data.eqns[key]
         dep = eqn.dependent
         ex = eqn.exog
         en = eqn.endog
         instr = eqn.instruments
-        dep = pd.DataFrame(dep, columns=['dep_{0}'.format(i)])
+        dep = DataFrame(dep, columns=['dep_{0}'.format(i)])
         has_const = False
         if np.any(np.all(ex == 1, 0)):
             ex = ex[:, 1:]
             has_const = True
-        ex = pd.DataFrame(ex, columns=['ex_{0}_{1}'.format(i, j) for j in range(ex.shape[1])])
-        en = pd.DataFrame(en, columns=['en_{0}_{1}'.format(i, j) for j in range(en.shape[1])])
-        instr = pd.DataFrame(instr, columns=['instr_{0}_{1}'.format(i, j)
-                                             for j in range(ex.shape[1])])
+        ex = DataFrame(ex, columns=['ex_{0}_{1}'.format(i, j) for j in range(ex.shape[1])])
+        en = DataFrame(en, columns=['en_{0}_{1}'.format(i, j) for j in range(en.shape[1])])
+        instr = DataFrame(instr, columns=['instr_{0}_{1}'.format(i, j)
+                                          for j in range(ex.shape[1])])
         fmla = ''.join(dep.columns) + ' ~  '
         if has_const:
             fmla += ' 1 + '
         fmla += ' + '.join(ex.columns) + ' + ['
         fmla += ' + '.join(en.columns) + ' ~ '
         fmla += ' + '.join(instr.columns) + ' ] '
         formulas[key] = fmla
         df.extend([dep, ex, en, instr])
-    df = pd.concat(df, 1)
+    df = concat(df, 1)
     formula_mod = IVSystemGMM.from_formula(formulas, df, weights=weights, weight_type='unadjusted')
     res = mod.fit(cov_type='unadjusted')
     formula_res = formula_mod.fit(cov_type='unadjusted')
     assert_allclose(res.params, formula_res.params)
 
 
 def test_weight_options(data):
@@ -272,17 +273,17 @@
     simple = simple_gmm(data.y, data.x, data.z, data.robust, steps=data.steps)
     assert_allclose(res.j_stat.stat, simple.j_stat, rtol=1e-4)
 
 
 def test_linear_constraint(data):
     mod = IVSystemGMM(data.eqns, weight_type=data.weight_type)
     p = mod.param_names
-    r = pd.DataFrame(np.zeros((1, len(p))), index=[0], columns=p)
+    r = DataFrame(np.zeros((1, len(p))), index=[0], columns=p)
     r.iloc[0, 1::6] = 1
-    q = pd.Series([6])
+    q = Series([6])
     mod.add_constraints(r, q)
 
     res = mod.fit()
     assert_allclose(res.params.iloc[1::6].sum(), 6)
 
 
 def test_kernel_equiv(data):
@@ -379,10 +380,10 @@
         fv.name = 'fitted_values'
         assert_series_equal(eq.fitted_values, fv)
         b = eq.params.values
         direct = mod._x[i] @ b
         expected.append(direct[:, None])
         assert_allclose(eq.fitted_values, direct, atol=1e-8)
     expected = np.concatenate(expected, 1)
-    expected = pd.DataFrame(expected, index=mod._dependent[i].pandas.index,
-                            columns=[key for key in res.equations])
+    expected = DataFrame(expected, index=mod._dependent[i].pandas.index,
+                         columns=[key for key in res.equations])
     assert_frame_equal(expected, res.fitted_values)
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_3sls_against_stata.py` & `linearmodels-4.9/linearmodels/tests/system/test_3sls_against_stata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
 
+from linearmodels.compat.pandas import concat
 from linearmodels.system import IV3SLS, SUR
 from linearmodels.tests.system._utility import generate_simultaneous_data
 from linearmodels.tests.system.results.parse_stata_3sls_results import results
 
 
 @pytest.fixture(scope='module', params=list(results.keys()))
 def fit(request):
     method = request.param
     data = generate_simultaneous_data()
     if 'ols' in method or 'sur' in method:
         mod = SUR
         for key in data:
             temp = data[key]
-            temp['exog'] = pd.concat([temp['exog'], temp['endog']], 1)
+            temp['exog'] = concat([temp['exog'], temp['endog']], 1)
             del temp['endog']
             del temp['instruments']
     else:
         mod = IV3SLS
     if 'ols' in method or '2sls' in method:
         fit_method = 'ols'
     else:
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_sur_against_stata.py` & `linearmodels-4.9/linearmodels/tests/system/test_sur_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_3sls.py` & `linearmodels-4.9/linearmodels/tests/system/test_3sls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from itertools import product
 
 import numpy as np
-import pandas as pd
 import pytest
 from numpy.testing import assert_allclose
+from pandas import DataFrame
+from pandas.testing import assert_frame_equal, assert_series_equal
 
-from linearmodels.compat.pandas import assert_frame_equal, assert_series_equal
 from linearmodels.system.model import IV3SLS
 from linearmodels.tests.system._utility import generate_3sls_data, simple_3sls, \
     generate_3sls_data_v2
 
 nexog = [3, [1, 2, 3, 4, 5]]
 nendog = [2, [1, 2, 1, 2, 1]]
 ninstr = [3, 2, [2, 3, 2, 3, 2]]
@@ -179,19 +179,19 @@
         IV3SLS(eqns)
 
 
 def test_multivariate_iv():
     n = 250
     dep = np.random.standard_normal((n, 2))
     exog = np.random.standard_normal((n, 3))
-    exog = pd.DataFrame(exog, columns=['exog.{0}'.format(i) for i in range(3)])
+    exog = DataFrame(exog, columns=['exog.{0}'.format(i) for i in range(3)])
     endog = np.random.standard_normal((n, 2))
-    endog = pd.DataFrame(endog, columns=['endog.{0}'.format(i) for i in range(2)])
+    endog = DataFrame(endog, columns=['endog.{0}'.format(i) for i in range(2)])
     instr = np.random.standard_normal((n, 3))
-    instr = pd.DataFrame(instr, columns=['instr.{0}'.format(i) for i in range(3)])
+    instr = DataFrame(instr, columns=['instr.{0}'.format(i) for i in range(3)])
     eqns = {}
     for i in range(2):
         eqns['dependent.{0}'.format(i)] = (dep[:, i], exog, endog, instr)
     mod = IV3SLS(eqns)
     res = mod.fit()
 
     common_mod = IV3SLS.multivariate_ls(dep, exog, endog, instr)
@@ -200,15 +200,15 @@
     assert_series_equal(res.params, common_res.params)
 
 
 def test_multivariate_iv_bad_data():
     n = 250
     dep = np.random.standard_normal((n, 2))
     instr = np.random.standard_normal((n, 3))
-    instr = pd.DataFrame(instr, columns=['instr.{0}'.format(i) for i in range(3)])
+    instr = DataFrame(instr, columns=['instr.{0}'.format(i) for i in range(3)])
 
     with pytest.raises(ValueError):
         IV3SLS.multivariate_ls(dep, None, None, instr)
 
 
 def test_fitted(data):
     mod = IV3SLS(data)
@@ -220,16 +220,16 @@
         fv.name = 'fitted_values'
         assert_series_equal(eq.fitted_values, fv)
         b = eq.params.values
         direct = mod._x[i] @ b
         expected.append(direct[:, None])
         assert_allclose(eq.fitted_values, direct, atol=1e-8)
     expected = np.concatenate(expected, 1)
-    expected = pd.DataFrame(expected, index=mod._dependent[i].pandas.index,
-                            columns=[key for key in res.equations])
+    expected = DataFrame(expected, index=mod._dependent[i].pandas.index,
+                         columns=[key for key in res.equations])
     assert_frame_equal(expected, res.fitted_values)
 
 
 def test_no_exog():
     data = generate_3sls_data_v2(nexog=0, const=False)
     mod = IV3SLS(data)
     res = mod.fit()
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_covariance.py` & `linearmodels-4.9/linearmodels/tests/system/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/_utility.py` & `linearmodels-4.9/linearmodels/tests/system/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_formulas.py` & `linearmodels-4.9/linearmodels/tests/system/test_formulas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import OrderedDict
 from itertools import product
 
 import numpy as np
 import pytest
 from pandas import Series, concat
+from pandas.testing import assert_series_equal, assert_frame_equal
 
 from linearmodels import SUR, IVSystemGMM, IV3SLS
-from linearmodels.compat.pandas import assert_series_equal, assert_frame_equal
 from linearmodels.formula import sur, iv_system_gmm, iv_3sls
 from linearmodels.system.model import SystemFormulaParser
 from linearmodels.tests.system._utility import generate_3sls_data_v2
 from linearmodels.utility import AttrDict
 
 data = generate_3sls_data_v2(k=2, const=False)
 joined = []
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_equivalence.py` & `linearmodels-4.9/linearmodels/tests/system/test_equivalence.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/test_sur.py` & `linearmodels-4.9/linearmodels/tests/system/test_sur.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from collections.abc import Mapping
 from itertools import product
 
 import numpy as np
 import pytest
 from numpy.testing import assert_allclose
 from pandas import DataFrame, Series, concat
+from pandas.testing import assert_frame_equal, assert_series_equal
 
-from linearmodels.compat.pandas import assert_frame_equal, assert_series_equal
 from linearmodels.iv.model import _OLS as OLS
 from linearmodels.system._utility import blocked_column_product, blocked_diag_product, \
     inv_matrix_sqrt
 from linearmodels.system.model import SUR
 from linearmodels.tests.system._utility import generate_data, simple_sur
 from linearmodels.utility import AttrDict, InvalidTestStatistic
 
@@ -633,14 +633,15 @@
         assert_allclose(eq.fitted_values, direct, atol=1e-8)
     expected = np.concatenate(expected, 1)
     expected = DataFrame(expected, index=mod._dependent[i].pandas.index,
                          columns=[key for key in res.equations])
     assert_frame_equal(expected, res.fitted_values)
 
 
+@pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
 def test_predict(missing_data):
     mod = SUR(missing_data)
     res = mod.fit()
     pred = res.predict()
     for key in pred:
         assert_series_equal(pred[key].iloc[:, 0], res.equations[key].fitted_values,
                             check_names=False)
@@ -670,12 +671,13 @@
     assert pred.shape[0] == nobs
 
     pred = res.predict(fitted=True, idiosyncratic=True, missing=True)
     for key in pred:
         assert pred[key].shape[0] == nobs
 
 
+@pytest.mark.filterwarnings('ignore::linearmodels.utility.MissingValueWarning')
 def test_predict_error(missing_data):
     mod = SUR(missing_data)
     res = mod.fit()
     with pytest.raises(ValueError):
         res.predict(fitted=False, idiosyncratic=False)
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/parse_stata_3sls_results.py` & `linearmodels-4.9/linearmodels/tests/system/results/parse_stata_3sls_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/execute-stata.py` & `linearmodels-4.9/linearmodels/tests/system/results/execute-stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/parse_stata_results.py` & `linearmodels-4.9/linearmodels/tests/system/results/parse_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/simulated-sur.dta` & `linearmodels-4.9/linearmodels/tests/system/results/simulated-sur.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/execute-stata-3sls.py` & `linearmodels-4.9/linearmodels/tests/system/results/execute-stata-3sls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Important cases
 
 """
 import os
 import subprocess
 
-import pandas as pd
+from linearmodels.compat.pandas import concat
 from linearmodels.tests.system._utility import generate_simultaneous_data
 
 data = generate_simultaneous_data()
 all_cols = []
 out = []
 for key in data:
     eqn = data[key]
@@ -17,15 +17,15 @@
         vals = eqn[key]
         for col in vals:
             if col in all_cols:
                 continue
             else:
                 out.append(vals[col])
                 all_cols.append(col)
-out = pd.concat(out, 1)
+out = concat(out, 1)
 if 'const' in out:
     out.pop('const')
 out.to_stata('simulated-3sls.dta', write_index=False)
 SEP = """
 
 file open myfile using {outfile}, write append
 file write myfile  "!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! {method} !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!" _n
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/generate_data.py` & `linearmodels-4.9/linearmodels/tests/system/results/generate_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 2. Small sample adjustment
 3. Constraints across equations
 """
 
 import numpy as np
 import pandas as pd
 
+from linearmodels.compat.pandas import concat
 from linearmodels.tests.system._utility import generate_data
 
 basic_data = generate_data(n=200, k=3, p=[2, 3, 4], const=True, seed=0)
 common_data = generate_data(n=200, k=3, p=3, common_exog=True, seed=1)
 missing_data = generate_data(n=200, k=3, p=[2, 3, 4], const=True, seed=2)
 
 np.random.seed(1234)
@@ -41,9 +42,9 @@
         dataset[key]['exog'] = exog
         if i != 1 or j == 0:
             out.extend([dep, exog])
         else:
             out.extend([dep])
 
 if __name__ == '__main__':
-    df = pd.concat(out, 1)
+    df = concat(out, 1)
     df.to_stata('simulated-sur.dta')
```

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/stata-sur-results.txt` & `linearmodels-4.9/linearmodels/tests/system/results/stata-sur-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/simulated-3sls.dta` & `linearmodels-4.9/linearmodels/tests/system/results/simulated-3sls.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/system/results/stata-3sls-results.txt` & `linearmodels-4.9/linearmodels/tests/system/results/stata-3sls-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/test_covariance.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/_utility.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/test_model.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/test_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/test_formulas.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/test_formulas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
-import pandas as pd
 import pytest
+from pandas.testing import assert_frame_equal
 
 from linearmodels.asset_pricing.model import (LinearFactorModel,
                                               LinearFactorModelGMM,
                                               TradedFactorModel)
-from linearmodels.compat.pandas import assert_frame_equal
+from linearmodels.compat.pandas import concat
 from linearmodels.tests.asset_pricing._utility import generate_data
 
 FORMULA_FACTORS = 'factor_1 + factor_2 + factor_3'
 FORMULA_PORT = 'port_1 + port_2 + port_3 + port_4 + port_5 + port_6 + port_7 + ' \
                'port_8 + port_9 + port_10'
 FORMULA = ' ~ '.join((FORMULA_PORT, FORMULA_FACTORS))
 
@@ -25,15 +25,15 @@
     return request.param
 
 
 @pytest.fixture(scope='module')
 def data(request):
     premia = np.array([.1, .1, .1])
     out = generate_data(nportfolio=10, output='pandas', alpha=True, premia=premia)
-    out['joined'] = pd.concat([out.factors, out.portfolios], 1)
+    out['joined'] = concat([out.factors, out.portfolios], 1)
     return out
 
 
 def test_traded_model_formula(data, model):
     mod1 = model.from_formula(FORMULA, data.joined)
     mod2 = model(data.portfolios, data.factors)
     res1 = mod1.fit()
```

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/tests/asset_pricing/test_linear_factor_model.py` & `linearmodels-4.9/linearmodels/tests/asset_pricing/test_linear_factor_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/asset_pricing/results.py` & `linearmodels-4.9/linearmodels/asset_pricing/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,19 @@
         self._cols = ['alpha'] + ['{0}'.format(f) for f in self._factor_names]
         self._rp_names = res.rp_names
         self._alpha_vcv = res.alpha_vcv
         self._cov_est = res.cov_est
 
     @property
     def summary(self):
-        """Summary table of model estimation results"""
+        """:obj:`statsmodels.iolib.summary.Summary` : Summary table of model estimation results
+
+        Supports export to csv, html and latex  using the methods ``summary.as_csv()``,
+        ``summary.as_html()`` and ``summary.as_latex()``.
+        """
 
         title = self.name + ' Estimation Summary'
 
         top_left = [('No. Test Portfolios:', len(self._portfolio_names)),
                     ('No. Factors:', len(self._factor_names)),
                     ('No. Observations:', self.nobs),
                     ('Date:', self._datetime.strftime('%a, %b %d %Y')),
```

### Comparing `linearmodels-4.8/linearmodels/asset_pricing/covariance.py` & `linearmodels-4.9/linearmodels/asset_pricing/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels/asset_pricing/model.py` & `linearmodels-4.9/linearmodels/asset_pricing/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,15 +549,15 @@
 
         return jac
 
     def _moments(self, eps, betas, lam, alphas, pricing_errors):
         sigma_inv = self._sigma_inv
 
         f = self.factors.ndarray
-        nobs, nf, nport, nrf, s1, s2, s3 = self._boundaries()
+        nobs, nf, nport, _, s1, s2, s3 = self._boundaries()
         fc = np.c_[np.ones((nobs, 1)), f]
         f_rep = np.tile(fc, (1, nport))
         eps_rep = np.tile(eps, (nf + 1, 1))
         eps_rep = np.reshape(eps_rep.T, (nport * (nf + 1), nobs)).T
 
         # Moments
         g1 = f_rep * eps_rep
@@ -671,15 +671,15 @@
         center : bool, optional
             Flag indicating to center the moment conditions before computing
             the weighting matrix.
         use_cue : bool, optional
             Flag indicating to use continuously updating estimator
         steps : int, optional
             Number of steps to use when estimating parameters.  2 corresponds
-            to the standard efficient gmm estimator. Higher values will
+            to the standard efficient GMM estimator. Higher values will
             iterate until convergence or up to the number of steps given
         disp : int, optional
             Number of iterations between printed update. 0 or negative values
             suppresses output
         max_iter : int, positive, optional
             Maximum number of iterations when minimizing objective
         cov_type : str, optional
```

### Comparing `linearmodels-4.8/linearmodels/utility.py` & `linearmodels-4.9/linearmodels/utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from collections import OrderedDict
 from collections.abc import MutableMapping
 
 import numpy as np
 from numpy import NaN, ceil, diag, isnan, log10, sqrt
 from numpy.linalg import eigh, matrix_rank
-from pandas import DataFrame, Series, concat
+from pandas import DataFrame, Series, concat, MultiIndex
 from scipy.stats import chi2, f
 from statsmodels.iolib.summary import SimpleTable, fmt_params
 
 from linearmodels.compat.numpy import lstsq
 
 
 class MissingValueWarning(Warning):
@@ -23,15 +23,15 @@
 class AttrDict(MutableMapping):
     """
     Ordered dictionary-like object that exposes keys as attributes
     """
 
     def update(self, *args, **kwargs):
         """
-        Update AD from dict/iterable E and F.
+        Update AD from dictionary or iterable E and F.
         If E is present and has a .keys() method, then does:  for k in E: AD[k] = E[k]
         If E is present and lacks a .keys() method, then does:  for k, v in E: AD[k] = v
         In either case, this is followed by: for k in F:  AD[k] = F[k]
         """
         self.__ordered_dict__.update(*args, **kwargs)
 
     def clear(self):
@@ -553,7 +553,49 @@
                 line = val
                 if i + 1 != len(s):
                     line += ', '
             else:
                 line = temp
     lines.append([line])
     return lines
+
+
+def panel_to_frame(x, items, major_axis, minor_axis, swap=False):
+    """
+    Construct a multiindex DataFrame using Panel-like arguments
+
+    Parameters
+    ----------
+    x : ndarray
+        3-d array with size nite, nmajor, nminor
+    items : list-like
+        List like object with item labels
+    major_axis : list-like
+        List like object with major_axis labels
+    minor_axis : list-like
+        List like object with minor_axis labels
+
+    Notes
+    -----
+    This function is equivalent to
+
+    Panel(x, items, major_axis, minor_axis).to_frame()
+
+    if `swap` is True, it is equivalent to
+
+    Panel(x, items, major_axis, minor_axis).swapaxes(1,2).to_frame()
+    """
+    nmajor = np.arange(len(major_axis))
+    nminor = np.arange(len(minor_axis))
+    final_levels = [major_axis, minor_axis]
+    mi = MultiIndex.from_product([nmajor, nminor])
+    if x is not None:
+        shape = x.shape
+        x = x.reshape((shape[0], shape[1] * shape[2])).T
+    df = DataFrame(x, columns=items, index=mi)
+    if swap:
+        df.index = df.index.swaplevel()
+        df.sort_index(inplace=True)
+        final_levels = [minor_axis, major_axis]
+    df.index.set_levels(final_levels, [0, 1], inplace=True)
+    df.index.names = ['major', 'minor']
+    return df
```

### Comparing `linearmodels-4.8/setup.py` & `linearmodels-4.9/setup.py`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/PKG-INFO` & `linearmodels-4.9/linearmodels.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: linearmodels
-Version: 4.8
+Version: 4.9
 Summary: Instrumental Variable and Linear Panel models for Python
 Home-page: http://github.com/bashtage/linearmodels
 Author: Kevin Sheppard
 Author-email: kevin.k.sheppard@gmail.com
 License: NCSA
 Description: Linear Models
         =============
         
-        |Build Status| |codecov|
+        |Build Status| |codecov| |Codacy Badge| |codebeat badge|
         
         Linear (regression) models for Python. Extends
         `statsmodels <http://www.statsmodels.org>`__ with Panel regression,
         instrumental variable estimators, system estimators and models for
         estimating asset prices:
         
         -  **Panel models**:
@@ -51,68 +51,68 @@
         Like `statsmodels <http://www.statsmodels.org>`__ to include, supports
         `patsy <https://patsy.readthedocs.io/en/latest/>`__ formulas for
         specifying models. For example, the classic Grunfeld regression can be
         specified
         
         .. code:: python
         
-            import numpy as np
-            from statsmodels.datasets import grunfeld
-            data = grunfeld.load_pandas().data
-            data.year = data.year.astype(np.int64)
-            # MultiIndex, entity - time
-            data = data.set_index(['firm','year'])
-            from linearmodels import PanelOLS
-            mod = PanelOLS(data.invest, data[['value','capital']], entity_effect=True)
-            res = mod.fit(cov_type='clustered', cluster_entity=True)
+           import numpy as np
+           from statsmodels.datasets import grunfeld
+           data = grunfeld.load_pandas().data
+           data.year = data.year.astype(np.int64)
+           # MultiIndex, entity - time
+           data = data.set_index(['firm','year'])
+           from linearmodels import PanelOLS
+           mod = PanelOLS(data.invest, data[['value','capital']], entity_effects=True)
+           res = mod.fit(cov_type='clustered', cluster_entity=True)
         
         Models can also be specified using the formula interface.
         
         .. code:: python
         
-            from linearmodels import PanelOLS
-            mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffect', data)
-            res = mod.fit(cov_type='clustered', cluster_entity=True)
+           from linearmodels import PanelOLS
+           mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffects', data)
+           res = mod.fit(cov_type='clustered', cluster_entity=True)
         
         The formula interface for ``PanelOLS`` supports the special values
         ``EntityEffects`` and ``TimeEffects`` which add entity (fixed) and time
         effects, respectively.
         
         Instrumental Variable Models
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         IV regression models can be similarly specified.
         
         .. code:: python
         
-            import numpy as np
-            from linearmodels.iv import IV2SLS
-            from linearmodels.datasets import mroz
-            data = mroz.load()
-            mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
+           import numpy as np
+           from linearmodels.iv import IV2SLS
+           from linearmodels.datasets import mroz
+           data = mroz.load()
+           mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
         
         The expressions in the ``[ ]`` indicate endogenous regressors (before
         ``~``) and the instruments.
         
         Installing
         ----------
         
         The latest release can be installed using pip
         
         .. code:: bash
         
-            pip install linearmodels
+           pip install linearmodels
         
         The master branch can be installed by cloning the repo and running setup
         
         .. code:: bash
         
-            git clone https://github.com/bashtage/linearmodels
-            cd linearmodels
-            python setup.py install
+           git clone https://github.com/bashtage/linearmodels
+           cd linearmodels
+           python setup.py install
         
         Documentation
         -------------
         
         `Stable Documentation <https://bashtage.github.io/linearmodels/>`__ is
         built on every tagged version using
         `doctr <https://github.com/drdoctr/doctr>`__. `Development
@@ -152,29 +152,35 @@
         -  xarray (0.9+, optional)
         
         Testing
         ~~~~~~~
         
         -  py.test
         
+        .. _documentation-1:
+        
         Documentation
         ~~~~~~~~~~~~~
         
         -  sphinx
-        -  guzzle\_sphinx\_theme
+        -  guzzle_sphinx_theme
         -  nbsphinx
         -  nbconvert
         -  nbformat
         -  ipython
         -  jupyter
         
         .. |Build Status| image:: https://travis-ci.org/bashtage/linearmodels.svg?branch=master
            :target: https://travis-ci.org/bashtage/linearmodels
         .. |codecov| image:: https://codecov.io/gh/bashtage/linearmodels/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/bashtage/linearmodels
+        .. |Codacy Badge| image:: https://api.codacy.com/project/badge/Grade/c771bce50a164b6fa71c344b374f140d
+           :target: https://www.codacy.com/app/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade
+        .. |codebeat badge| image:: https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243
+           :target: https://codebeat.co/projects/github-com-bashtage-linearmodels-master
         
 Keywords: linear models,regression,instrumental variables,IV,panel,fixed effects,clustered,heteroskedasticity,endogeneity,instruments,statistics,statistical inference,econometrics
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `linearmodels-4.8/doc/source/panel/mathematical-detail.txt` & `linearmodels-4.9/doc/source/panel/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/examples/data-formats.ipynb` & `linearmodels-4.9/examples/panel_data-formats.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'This example uses the job training data to construct a "*

 * *            'MultiIndex `DataFrame` using the `set_index` command. The entity index is `fcode` and '*

 * *            "the time index is `year`.')], delete: [3]}}}"}*

```diff
@@ -17,15 +17,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Multi Index DataFrames\n",
                 "The most precise data format to use is a MultiIndex `DataFrame`.  This is the most precise since only single columns can preserve all types within a panel.  For example, it is not possible to span a single Categorical variable across multiple columns when using a pandas `Panel`. \n",
                 "\n",
-                "This example uses the jobtraining example to format a MultiIndex `DataFrame` using the `set_index` command. The entity index is known as fcode and the time index is year."
+                "This example uses the job training data to construct a MultiIndex `DataFrame` using the `set_index` command. The entity index is `fcode` and the time index is `year`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/doc/source/panel/examples/using-formulas.ipynb` & `linearmodels-4.9/examples/panel_using-formulas.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, 'The constant can be explicitly included using the `1 + "*

 * *            '` notation.  When a constant is included in the model, and additional constraint is '*

 * *            'imposed that the number of the effects is 0.  This allows the constant to be '*

 * *            "identified using the grand mean of the dependent and the regressors.')], delete: "*

 * *            '[2]}}}'}*

```diff
@@ -63,15 +63,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## PanelOLS with Entity Effects and a constant\n",
                 "\n",
-                "The constant can be explicitly included using the `1 + ` notation.  When a constant is included in the model, and additional constraint is imposed that the number of the effects is 0.  This allows the constant to be identified using teh grand mean of the dependent and the regressors."
+                "The constant can be explicitly included using the `1 + ` notation.  When a constant is included in the model, and additional constraint is imposed that the number of the effects is 0.  This allows the constant to be identified using the grand mean of the dependent and the regressors."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/doc/source/panel/examples/examples.ipynb` & `linearmodels-4.9/examples/panel_examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990354938271605%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(1, 'The random effects model is virtually identical to the "*

 * *            'pooled OLS model except that is accounts for the structure of the model and so is '*

 * *            'more efficient. Random effects uses a quasi-demeaning strategy which subtracts the '*

 * *            "time average of the within entity values to account for the common shock.')], delete: "*

 * *            "[1]}}, 18: {'source': {insert: [(4, 'For variable which can be consistently "*

 * *            'estimated, s […]*

```diff
@@ -74,15 +74,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Random effects\n",
-                "The random effects model is virtually identical to the pooled OLS model except that is accounts for the structure of the model and so is more efficient. Random effects uses a quasi-demeaning strategy which subtracts the time average fo the within entity values to account for the common shock."
+                "The random effects model is virtually identical to the pooled OLS model except that is accounts for the structure of the model and so is more efficient. Random effects uses a quasi-demeaning strategy which subtracts the time average of the within entity values to account for the common shock."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -195,15 +195,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Time Effects\n",
                 "Time effect can be added using ``time_effects=True``.  Here the time dummies are removed. Note that the core coefficients are identical. The only change is in the test statistic for poolability since not the \"effects\" include both entity and time, whereas before only entity were included.\n",
                 "\n",
                 "#### Effects vs Dummies\n",
-                "For variable which can be consistently estimated, such as time effects in the usual large N, fixed T panel, it isn't necessary to include these as effects.  They can instead be implemented as dummy variables.  "
+                "For variable which can be consistently estimated, such as time effects in the usual large N, fixed T panel, it is not necessary to include these as effects.  They can instead be implemented as dummy variables.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -217,15 +217,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Other Options\n",
-                "Some additional options are available when using ``PanelOLS`` and effects.  The ``use_lsdv`` can be used to force the model to be estimated using dummy variables.  This isn't necessary and will be slower in most circumstances.  This options is primarily included for testing.  ``auto_df`` instructs ``PanelOLS`` to determine the degree of freedom adjustment to make.  Unlike most other estimators, the treatment of effects depends on the covariance estimator.  For example, when using a classic covariance estimator, effects count as lost degrees of freedom.  When using entity effects and clustering by entity, they do not.  Setting ``auto_df=False`` will allow the entities to be counted or not, depending on the value of ``count_effects``."
+                "Some additional options are available when using ``PanelOLS`` and effects.  The ``use_lsdv`` can be used to force the model to be estimated using dummy variables.  This is not necessary and will be slower in most circumstances.  This options is primarily included for testing.  ``auto_df`` instructs ``PanelOLS`` to determine the degree of freedom adjustment to make.  Unlike most other estimators, the treatment of effects depends on the covariance estimator.  For example, when using a classic covariance estimator, effects count as lost degrees of freedom.  When using entity effects and clustering by entity, they do not.  Setting ``auto_df=False`` will allow the entities to be counted or not, depending on the value of ``count_effects``."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Using first differences\n",
```

### Comparing `linearmodels-4.8/doc/source/panel/covariance.rst` & `linearmodels-4.9/doc/source/panel/covariance.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/mathematical-detail.lyx` & `linearmodels-4.9/doc/source/panel/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/pandas.rst` & `linearmodels-4.9/doc/source/panel/pandas.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/results.rst` & `linearmodels-4.9/doc/source/panel/results.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/faq.rst` & `linearmodels-4.9/doc/source/panel/faq.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ----------------------
 
 While the implementation of the panel estimators is similar to Stata, there
 are some differenced worth noting.
 
 Clustered Covariance with Fixed Effects
 =======================================
-When suing clustered standard errors and entity effects, it isn't necessary
+When suing clustered standard errors and entity effects, it is not necessary
 to adjust for estimated effects. ``PanelOLS`` attempts to detect when this is
 the case and automatically adjust the degree of freedom. This can be
 overridden using by setting the fit option ``auto_df=False`` and then
 changing the value of ``count_effects``.
 
 R2 definitions
 ==============
```

### Comparing `linearmodels-4.8/doc/source/panel/index.rst` & `linearmodels-4.9/doc/source/panel/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/panel/introduction.rst` & `linearmodels-4.9/doc/source/panel/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 :class:`~linearmodels.panel.model.PanelOLS` is somewhat more general than the
 other estimators and can be used to model 2 effects (e.g., entity and time
 effects).
 
 Model specification is similar to `statsmodels <http://www.statsmodels.org/>`_.
 This example estimates a fixed effect regression on a panel of the wages of working
-men modeling teh log wage as a function of squared experience, a dummy if the
+men modeling the log wage as a function of squared experience, a dummy if the
 man is married and a dummy indicating if the man is a union member.
 
 .. code-block:: python
 
    from linearmodels.panel import PanelOLS
    from linearmodels.datasets import wage_panel
    import statsmodels.api as sm
```

### Comparing `linearmodels-4.8/doc/source/panel/models.rst` & `linearmodels-4.9/doc/source/panel/models.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/iv/examples/using-formulas.ipynb` & `linearmodels-4.9/examples/iv_using-formulas.ipynb`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/iv/examples/basic-examples.ipynb` & `linearmodels-4.9/examples/iv_basic-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'cells'": '{22: {\'source\': ["The variance of the squared residuals is not particularly well '*

 * *            "explained by the data, and so the GLS-type estimates and the usual IV estimates don't "*

 * *            'differ by much."]}, 50: {\'source\': ["Wooldridge\'s regression test of exogeneity '*

 * *            'uses regression residual where the endogenous variables are regressed on the '*

 * *            'exogenous and the instrument to test for endogeneity. IF the endogenous variable is '*

 * *            'actually ex […]*

```diff
@@ -216,15 +216,15 @@
                 "print(fgls_res)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The variance of the squared residuals isn't particularly well explained by the data, and so the GLS-type estimates and the usual IV estimates don't differ by much."
+                "The variance of the squared residuals is not particularly well explained by the data, and so the GLS-type estimates and the usual IV estimates don't differ by much."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -499,15 +499,15 @@
                 "print(res)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Wooldridge's regression test of exogeneity uses regression residual where the endogenous variables are regressed on the exogenous and the instrument to test for endogenity. IF the endogenous variable is actually exogenous these residuals should not be correlated with the variable of interest. "
+                "Wooldridge's regression test of exogeneity uses regression residual where the endogenous variables are regressed on the exogenous and the instrument to test for endogeneity. IF the endogenous variable is actually exogenous these residuals should not be correlated with the variable of interest. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -536,15 +536,15 @@
                 "print(res_direct)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Since this regression has two instrument it is possible to test for overidentification.  Wooldridge's overidentification test uses a regression to test whether the 2SLS residuals are uncorrelated with the instruments, which should be the case if the model is correct and the instruments aren't needed in the original model."
+                "Since this regression has two instrument it is possible to test for overidentification.  Wooldridge's overidentification test uses a regression to test whether the 2SLS residuals are uncorrelated with the instruments, which should be the case if the model is correct and the instruments are not needed in the original model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/doc/source/iv/examples/advanced-examples.ipynb` & `linearmodels-4.9/examples/iv_advanced-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'cells'": '{9: {\'source\': ["And finally the simple correlation between the endogenous variable '*

 * *            'and the instruments.  Instruments must be correlated to be relevant (but also must be '*

 * *            "exogenous, which can't be examined using simple correlation).  The correlation of "*

 * *            '`firmsz` is especially low, which might lead to the weak instruments problem if used '*

 * *            'exclusively.  "]}, 21: {\'source\': {insert: [(4, \'The default weighting matrix is '*

 * *            "r […]*

```diff
@@ -87,15 +87,15 @@
                 "print(data[instruments].describe(percentiles=[]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "And finally the simple correlation between the endogenous variable and the instruments.  Instruments must be correlated to be relevant (but also must be exogenous, which can't be examined using simple correlation).  THe correlation of `firmsz` is especially low, which might lead to the weak instruments problem if used exclusively.  "
+                "And finally the simple correlation between the endogenous variable and the instruments.  Instruments must be correlated to be relevant (but also must be exogenous, which can't be examined using simple correlation).  The correlation of `firmsz` is especially low, which might lead to the weak instruments problem if used exclusively.  "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -220,15 +220,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## GMM Estimation\n",
                 "\n",
                 "GMM estimation can be more efficient than 2SLS when there are more than one instrument.  By default, 2-step efficient GMM is used (assuming the weighting matrix is correctly specified).  It is possible to iterate until convergence using the optional keyword input ``iter_limit``, which is naturally 2 by default.  Generally, GMM-CUE would be preferred to using multiple iterations of standard GMM.\n",
                 "\n",
-                "The default weighting matrix is robust to heteroskecasticity (but not clustering)."
+                "The default weighting matrix is robust to heteroskedasticity (but not clustering)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": true
@@ -430,15 +430,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Single Instrument Regressions\n",
-                "It can be useful to run the just identified regressions to see how the IV estimate varies by instrument. The OLS model is included for comparrison. The coefficient when using ``lowincome`` is very similar to the OLS as is the $R^2$ which indicates this variable may be endogenous. The coefficient using ``firmsz`` is also very different, but this is probably due to the low correlation between ``firmsz`` and the endogenous regressor so that this is a weak instrument. "
+                "It can be useful to run the just identified regressions to see how the IV estimate varies by instrument. The OLS model is included for comparison. The coefficient when using ``lowincome`` is very similar to the OLS as is the $R^2$ which indicates this variable may be endogenous. The coefficient using ``firmsz`` is also very different, but this is probably due to the low correlation between ``firmsz`` and the endogenous regressor so that this is a weak instrument. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/doc/source/iv/covariance.rst` & `linearmodels-4.9/doc/source/iv/covariance.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/iv/estimators.lyx` & `linearmodels-4.9/doc/source/iv/estimators.lyx`

 * *Files 0% similar despite different names*

```diff
@@ -1510,15 +1510,15 @@
 
 \series bold
 Durbin and Wu-Haussman
 \end_layout
 
 \begin_layout Standard
 \noindent
-Durbin's and the Wu-Hausmann tests of exogeneity test of exogeneity is depends
+Durbin's and the Wu-Hausman tests of exogeneity test of exogeneity is depends
  on the variance of the residuals when come endogenous variables are treated
  as exogenous against the case where they are treated as endogenous.
  Durbin's test statistic is
 \begin_inset Formula 
 \begin{align*}
 \delta= & \hat{\epsilon}'_{e}P_{[z,w]}\hat{\epsilon}_{e}-\hat{\epsilon}'_{c}P_{z}\hat{\epsilon}_{c}\\
 D= & \delta/(\hat{\epsilon}'_{e}\hat{\epsilon}_{e})/n\sim\chi_{q}^{2}
@@ -1527,15 +1527,15 @@
 \end_inset
 
 
 \end_layout
 
 \begin_layout Standard
 \noindent
-and the Wu-Hausmann test statistic is
+and the Wu-Hausman test statistic is
 \end_layout
 
 \begin_layout Standard
 \noindent
 \begin_inset Formula 
 \begin{align*}
 WH= & \frac{\delta/q}{(\hat{\epsilon}'_{e}\hat{\epsilon}_{e}-\delta)/v}\sim F_{q,\nu}
```

### Comparing `linearmodels-4.8/doc/source/iv/index.rst` & `linearmodels-4.9/doc/source/iv/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 :ref:`Basic Examples <iv/examples/basic-examples.ipynb>` shows basic usage
 through examples from Wooldridge's introductory text book and
 :ref:`Advanced Examples <iv/examples/advanced-examples.ipynb>` shows more
 advanced examples following the examples in Cameron and Trivedi's Stata
 introduction.
 
-:ref:`iv-mathematical-notation` contains a concise explanation of teh formulas
+:ref:`iv-mathematical-notation` contains a concise explanation of the formulas
 used in estimating parameters, estimating covariances and conducting hypothesis
 tests.
 
 .. toctree::
    :maxdepth: 1
    :glob:
```

### Comparing `linearmodels-4.8/doc/source/iv/introduction.rst` & `linearmodels-4.9/doc/source/iv/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -123,37 +123,37 @@
   if weighting matrices available:
 
   * 'unadjusted' - Assumes the GMM moment conditions are homoskedastic. See
     :class:`~linearmodels.iv.gmm.HomoskedasticWeightMatrix`.
   * 'robust' - Allows the GMM moment conditions to be heteroskedastic while
     assuming they are not correlated across observations. See
     :class:`~linearmodels.iv.gmm.HeteroskedasticWeightMatrix`.
-  * 'kernel' - Allows for both heteroskedasticity and autocorrrelation in the
+  * 'kernel' - Allows for both heteroskedasticity and autocorrelation in the
     moment conditions. See :class:`~linearmodels.iv.gmm.KernelWeightMatrix`.
   * 'cluster' - Allows for a one- and two-way cluster structure where moment
     conditions within a cluster are correlated.
     See :class:`~linearmodels.iv.gmm.ClusteredWeightMatrix`.
 
   Each weight type accepts a set of additional parameters which are similar to
   those for the corresponding covariance estimator.
 
 Model Estimation and Covariance Specification
 =============================================
-All models are estimated using teh ``fit`` method which provides an
+All models are estimated using the ``fit`` method which provides an
 opportunity to customize the parameter covariance estimator used to
 perform inference. Four classes of covariance estimators are available:
 
 * 'unadjusted' - Assumes the model scores are homoskedastic. See
   :class:`~linearmodels.iv.covariance.HomoskedasticCovariance`.
 
 * 'robust', 'heteroskedastic' - Allows the model scores to be heteroskedastic
   while assuming they are not correlated across observations. See
   :class:`~linearmodels.iv.covariance.HeteroskedasticCovariance`.
 
-* 'kernel' - Allows for both heteroskedasticity and autocorrrelation in the
+* 'kernel' - Allows for both heteroskedasticity and autocorrelation in the
   model scores. The estimator allows the ``kernel`` to be selected from
 
   * 'bartlett', 'newey-west` - Triangular kernel utilized in the common
     Newey-West estimator.
   * 'parzen' - Parzen's kernel.
   * 'qs', 'quadratic-spectral' - The quadratic spectral kernel studied by
     Andrews.
@@ -181,15 +181,15 @@
 particular, the default is to use two-step GMM.  One-step (inefficient)
 GMM can be forced by setting ``iter_limit`` to 1.  If ``iter_limit`` is
 raised above 2, then an iterative method is used where multiple steps
 are used to estimate the model parameters.  If normalized model parameters
 change by less than ``tol`` across successive iterations, then the estimation
 is assumed to converge and the iterations are stopped.
 
-By default, the first-step uses teh average outer-product of the instruments
+By default, the first-step uses the average outer-product of the instruments
 as the weighting matrix.  ``initial_weight`` allows a user-specified choice of
 weighting matrix to be used instead.
 
 GMM-CUE Estimation
 ******************
 GMM CUE uses a non-linear optimizer to optimize the GMM objective directly
 where both the moment condition and the moment score estimator change with
```

### Comparing `linearmodels-4.8/doc/source/iv/gmm.rst` & `linearmodels-4.9/doc/source/iv/gmm.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/iv/estimators.txt` & `linearmodels-4.9/doc/source/iv/estimators.txt`

 * *Files 0% similar despite different names*

```diff
@@ -434,26 +434,26 @@
 
 .. math:: \hat{\kappa}(n-p)/q\sim F_{q,n-n_{instr}}
 
 where :math:`q=p-k_{2}`.
 
 **Durbin and Wu-Haussman**
 
-Durbin’s and the Wu-Hausmann tests of exogeneity test of exogeneity is
+Durbin’s and the Wu-Hausman tests of exogeneity test of exogeneity is
 depends on the variance of the residuals when come endogenous variables
 are treated as exogenous against the case where they are treated as
 endogenous. Durbin’s test statistic is
 
 .. math::
 
    \begin{aligned}
    \delta= & \hat{\epsilon}'_{e}P_{[z,w]}\hat{\epsilon}_{e}-\hat{\epsilon}'_{c}P_{z}\hat{\epsilon}_{c}\\
    D= & \delta/(\hat{\epsilon}'_{e}\hat{\epsilon}_{e})/n\sim\chi_{q}^{2}\end{aligned}
 
-and the Wu-Hausmann test statistic is
+and the Wu-Hausman test statistic is
 
 .. math::
 
    \begin{aligned}
    WH= & \frac{\delta/q}{(\hat{\epsilon}'_{e}\hat{\epsilon}_{e}-\delta)/v}\sim F_{q,\nu}\end{aligned}
 
 where :math:`\hat{\epsilon}_{e}` treats the selected set of endogenous
```

### Comparing `linearmodels-4.8/doc/source/contributing.rst` & `linearmodels-4.9/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/mathematical-detail.txt` & `linearmodels-4.9/doc/source/system/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/examples/formulas.ipynb` & `linearmodels-4.9/examples/system_formulas.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979967948717949%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(2, 'When using the curly brace formula specification, the "*

 * *            'equation names are determined by the dependent variable names.  When names are '*

 * *            'repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) '*

 * *            'then the equation labels will be modified until they are unique.  This can produce '*

 * *            'meaningless equation labels, and so it is possible to pass an equation label using '*

 * *            "the syntax\\ […]*

```diff
@@ -89,15 +89,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Labeled Formulas\n",
                 "\n",
-                "When using the curly brace formula specification, the equation names are determined by the dependent variable names.  When names are repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) then the equation labels will be \"uglified\" until they are unique.  This can produce meaningless equation labels, and so it is possible to pass an equation label using the syntax\n",
+                "When using the curly brace formula specification, the equation names are determined by the dependent variable names.  When names are repeated as is the case in some datasets (e.g. a SUR on GDP of multiple countries) then the equation labels will be modified until they are unique.  This can produce meaningless equation labels, and so it is possible to pass an equation label using the syntax\n",
                 "\n",
                 "```\n",
                 "{label : dep ~ exog}\n",
                 "```\n"
             ]
         },
         {
@@ -153,16 +153,16 @@
                 "print(weighted_mod.fit())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Pre-specified Residual Covariance\n",
-                "Like a standard SUR, it is possible to pass a pre-specified residual covariance for use in the GLS step.  This is done using the keyword argument `sigma` in the `from_formula` method, and is otherwise identical to passing one to the standard SUR."
+                "### Prespecified Residual Covariance\n",
+                "Like a standard SUR, it is possible to pass a prespecified residual covariance for use in the GLS step.  This is done using the keyword argument `sigma` in the `from_formula` method, and is otherwise identical to passing one to the standard SUR."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `linearmodels-4.8/doc/source/system/examples/examples.ipynb` & `linearmodels-4.9/examples/system_examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998836267961951%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(15, 'where $Y$ is a column vector that stacks the vectors "*

 * *            '$Y_i$ for $i=1,2,\\\\ldots,K$, $X$ is a block-diagonal matrix where diagonal block i '*

 * *            'is $X_i$, $\\\\beta$ is a stacked vector of the $K$ $\\\\beta_i$s and $\\\\epsilon$ '*

 * *            "is similarly comprised of the stacked columns of $\\\\epsilon_i$.\\n')], delete: "*

 * *            "[15]}}, 6: {'source': {insert: [(2, 'Seemingly Unrelated Models are fairly complex "*

 * *            'and eac […]*

```diff
@@ -15,15 +15,15 @@
                 "\n",
                 "$$ Y_i = X_i\\beta_i + \\epsilon_i$$\n",
                 "\n",
                 "so that the set of models can be expressed as \n",
                 "\n",
                 "$$ Y = X\\beta + \\epsilon$$\n",
                 "\n",
-                "where $Y$ is a column vector that stacks the vectors $Y_i$ for $i=1,2,\\ldots,K$, $X$ is a block-diagonal matrix where the i-th block is $X_i$, $\\beta$ is a stacked vector of the $K$ $\\beta_i$s and $\\epsilon$ is similarly comprised of the stacked columns of $\\epsilon_i$.\n",
+                "where $Y$ is a column vector that stacks the vectors $Y_i$ for $i=1,2,\\ldots,K$, $X$ is a block-diagonal matrix where diagonal block i is $X_i$, $\\beta$ is a stacked vector of the $K$ $\\beta_i$s and $\\epsilon$ is similarly comprised of the stacked columns of $\\epsilon_i$.\n",
                 "\n",
                 "The model can be estimated using OLS with the usual estimator\n",
                 "\n",
                 "$$\\hat{\\beta}_{OLS} = \\left(X^\\prime X\\right)^{-1}X^\\prime Y.$$\n",
                 "\n",
                 "Since there are multiple series, a GLS estimator that accounts for the cross-sectional heteroskedasticity as well as the correlation of residuals can be estimated \n",
                 "\n",
@@ -115,15 +115,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Basic Usage\n",
                 "\n",
-                "Seemingly Unrelated Models are fairly complex and each equation could have a different number of regressors.  As a result, it isn't possibly to use standard `pandas` or `numpy` data structures, and so dictionaries (or technically dictionary-like objects) are used.  In practice, it is strongly recommended to use a `OrderedDictionary` from the `collections` module.  This ensures that equation order will be preserved. In addition, the dictionary must have the following structure:\n",
+                "Seemingly Unrelated Models are fairly complex and each equation could have a different number of regressors.  As a result, it is not possibly to use standard `pandas` or `numpy` data structures, and so dictionaries (or technically dictionary-like objects) are used.  In practice, it is strongly recommended to use a `OrderedDictionary` from the `collections` module.  This ensures that equation order will be preserved. In addition, the dictionary must have the following structure:\n",
                 "\n",
                 "* `keys` **must be strings** and will be used as equation labels\n",
                 "* The value associated with each key must be either a dictionary or a tuple.\n",
                 "\n",
                 "  * When a dictionary is used, it must have two keys, `dependent` and `exog`.  It can optionally have a third key `weights` which provides weights to use in the regression.\n",
                 "  * When a tuple is used, it must have two elements and takes the form `(dependent, exog)`.  It can optionally contains weights in which case it takes the form `(dependent, exog, weights)`.\n",
                 "\n",
@@ -245,15 +245,15 @@
                 "print(res.equations['WC'])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The current version of the model doesn't facilitate cross equation comparisons and so this is manually implemented here. "
+                "The current version of the model does not facilitate cross equation comparisons and so this is manually implemented here. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -491,22 +491,22 @@
                 "print(fres_het.summary)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Pre-specified Residual Covariance Estimators"
+                "## Prespecified Residual Covariance Estimators"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The GLS estimator can be used with a user specified covariance.  This example uses and equi-correlation covariance in the state GDP model.  The estimator must be used when constructing the model through the `sigma` keyword argument."
+                "The GLS estimator can be used with a user specified covariance.  This example uses a covariance where all correlations are identical (equicorrelation) in the state GDP model.  The estimator must be used when constructing the model through the `sigma` keyword argument."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -605,15 +605,15 @@
                 "\n",
                 "More complicated constraints can be used to produce interesting models.  Using the same idea as the previous set of constraints, a pooled SUR (excluding the constant) is constructed by restricting all coefficients to have the same value.  Here the form of the restriction is \n",
                 "\n",
                 "$$ \\beta_{var,0} - \\beta_{var,j} = 0$$\n",
                 "\n",
                 "so that the restriction is identical to the previous, only applied to all variables excluding the constant.\n",
                 "\n",
-                "Here the estimated from the first two equations are shown. ALl coefficients except the intercept are identical across equations.\n",
+                "Here the estimated from the first two equations are shown. All coefficients except the intercept are identical across equations.\n",
                 "\n",
                 "**Note**: When linear constraints are imposed, the parameter covariance matrix will be singular.  Caution is needed to ensure test statistics are meaningful."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-1.png` & `linearmodels-4.9/examples/system_correct-greene-table-10-1.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-2.png` & `linearmodels-4.9/examples/system_correct-greene-table-10-2.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/examples/three-stage-ls.ipynb` & `linearmodels-4.9/examples/system_three-stage-ls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998196248196248%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(9, 'The estimates are the same.  This interface is more "*

 * *            "useful for programmatically generating and estimating models.')], delete: [9]}}}"}*

```diff
@@ -166,15 +166,15 @@
                 "The model can be directly specified using a dictionary of dictionaries where the inner dictionaries contain the 4 components of the model:\n",
                 "\n",
                 "* dependent - The dependent variable\n",
                 "* exog - Exogenous regressors\n",
                 "* endog - Endogenous regressors\n",
                 "* instruments - Instrumental variables\n",
                 "\n",
-                "The estimates are the same.  This interface is more useful for programatically generating and estimating models."
+                "The estimates are the same.  This interface is more useful for programmatically generating and estimating models."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `linearmodels-4.8/doc/source/system/examples/system_correct-greene-table-10-3.png` & `linearmodels-4.9/examples/system_correct-greene-table-10-3.png`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/covariance.rst` & `linearmodels-4.9/doc/source/system/covariance.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 Heteroskedasticity-Autocorrelation (HAC) Robust Covariance Estimation
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. autoclass:: KernelCovariance
    :members:
    :inherited-members:
 
-Genralized Method of Moments (GMM)
-==================================
+Generalized Method of Moments (GMM)
+===================================
 
 GMM Homoskedastic Covariance Estimation
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. autoclass:: GMMHomoskedasticCovariance
    :members:
    :inherited-members:
```

### Comparing `linearmodels-4.8/doc/source/system/mathematical-detail.lyx` & `linearmodels-4.9/doc/source/system/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/index.rst` & `linearmodels-4.9/doc/source/system/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/system/models.rst` & `linearmodels-4.9/doc/source/system/models.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/conf.py` & `linearmodels-4.9/doc/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,24 @@
               'sphinx.ext.extlinks',
               'sphinx.ext.doctest',
               'IPython.sphinxext.ipython_console_highlighting',
               'IPython.sphinxext.ipython_directive',
               'nbsphinx'
               ]
 
+try:
+    import sphinxcontrib.spelling
+except ImportError as err:
+    pass
+else:
+    extensions.append('sphinxcontrib.spelling')
+
+spelling_word_list_filename = ['spelling_wordlist.txt', 'names_wordlist.txt']
+spelling_ignore_pypi_package_names = True
+
 add_module_names = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
```

### Comparing `linearmodels-4.8/doc/source/plan.rst` & `linearmodels-4.9/doc/source/plan.rst`

 * *Files 16% similar despite different names*

```diff
@@ -43,11 +43,15 @@
 **************************************
 Planned but not implemented
 
 System Estimation
 =================
 * Seemingly Unrelated Regression (SUR) Estimator - :class:`linearmodels.system.model.SUR`
 
+  - Multivariate OLS is supported as a special case of SUR.  This method does
+    not perform well on large datasets and should be improved by a special
+    purpose implementation.
+
 Instrumental Variable Estimators
 ********************************
 * Three-stage Least Squares (3SLS) Estimator - :class:`linearmodels.system.model.IV3SLS`
 * Generalized Method of Moments (GMM) System Estimation - :class:`linearmodels.system.model.IVSystemGMM`
```

### Comparing `linearmodels-4.8/doc/source/index.rst` & `linearmodels-4.9/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/_static/css/overrides.css` & `linearmodels-4.9/doc/source/_static/css/overrides.css`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/mathematical-detail.txt` & `linearmodels-4.9/doc/source/asset-pricing/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/examples/formulas.ipynb` & `linearmodels-4.9/examples/asset-pricing_formulas.ipynb`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/examples/examples.ipynb` & `linearmodels-4.9/examples/asset-pricing_examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990146396396397%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(4, 'Note that when using this type of model, it is "*

 * *            'essential that the test portfolios are excess returns. This is not a requirement of '*

 * *            "the other factor model estimators. \\n')], delete: [4]}}, 22: {'source': ['The size "*

 * *            'factor was insignificant and so is dropped. This does not have much of an effect on '*

 * *            "the estimates.']}, 24: {'source': {insert: [(0, 'The risk-free rate can be optionally "*

 * *            'estimated […]*

```diff
@@ -62,15 +62,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 1-Step Estimation using Seemingly Unrelated Regression (SUR)\n",
                 "\n",
                 "When the factors are traded assets, they must price themselves, and so the observed factor returns can be used to consistently estimate the expected factor returns.  This also allows a set of seemingly unrelated regressions where each test portfolio is regressed on the factors and a constant to estimate factor loadings and $\\alpha$s. \n",
                 "\n",
-                "Note that when using this type of model, it is essential that the test portfolios are excess returns. This isn't a requirement of the other factor model estimators. \n",
+                "Note that when using this type of model, it is essential that the test portfolios are excess returns. This is not a requirement of the other factor model estimators. \n",
                 "\n",
                 "This specification is a CAP-M since only the market is included.  The J-statistic tests whether all model $\\alpha$s are 0.  The CAP-M is unsurprisingly unable to price the test portfolios."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -220,15 +220,15 @@
                 "print(res.betas.corr())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The size factor was insignificant and so is dropped. This doesn't have much of an effect on the estimates."
+                "The size factor was insignificant and so is dropped. This does not have much of an effect on the estimates."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -240,15 +240,15 @@
                 "print(mod.fit())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The risk-free rate can be optionally estimated.  This is useful in case excess returns are not available of if the risk-free rate used to construct the excess returns might be mis-specified.\n",
+                "The risk-free rate can be optionally estimated.  This is useful in case excess returns are not available of if the risk-free rate used to construct the excess returns might be misspecified.\n",
                 "\n",
                 "Here the estimated risk-free rate is small and insignificant and has little impact on the model J-statistic."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `linearmodels-4.8/doc/source/asset-pricing/covariance.rst` & `linearmodels-4.9/doc/source/asset-pricing/covariance.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/mathematical-detail.lyx` & `linearmodels-4.9/doc/source/asset-pricing/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/index.rst` & `linearmodels-4.9/doc/source/asset-pricing/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/introduction.rst` & `linearmodels-4.9/doc/source/asset-pricing/introduction.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/asset-pricing/models.rst` & `linearmodels-4.9/doc/source/asset-pricing/models.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/doc/source/references.rst` & `linearmodels-4.9/doc/source/references.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-4.8/linearmodels.egg-info/PKG-INFO` & `linearmodels-4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: linearmodels
-Version: 4.8
+Version: 4.9
 Summary: Instrumental Variable and Linear Panel models for Python
 Home-page: http://github.com/bashtage/linearmodels
 Author: Kevin Sheppard
 Author-email: kevin.k.sheppard@gmail.com
 License: NCSA
 Description: Linear Models
         =============
         
-        |Build Status| |codecov|
+        |Build Status| |codecov| |Codacy Badge| |codebeat badge|
         
         Linear (regression) models for Python. Extends
         `statsmodels <http://www.statsmodels.org>`__ with Panel regression,
         instrumental variable estimators, system estimators and models for
         estimating asset prices:
         
         -  **Panel models**:
@@ -51,68 +51,68 @@
         Like `statsmodels <http://www.statsmodels.org>`__ to include, supports
         `patsy <https://patsy.readthedocs.io/en/latest/>`__ formulas for
         specifying models. For example, the classic Grunfeld regression can be
         specified
         
         .. code:: python
         
-            import numpy as np
-            from statsmodels.datasets import grunfeld
-            data = grunfeld.load_pandas().data
-            data.year = data.year.astype(np.int64)
-            # MultiIndex, entity - time
-            data = data.set_index(['firm','year'])
-            from linearmodels import PanelOLS
-            mod = PanelOLS(data.invest, data[['value','capital']], entity_effect=True)
-            res = mod.fit(cov_type='clustered', cluster_entity=True)
+           import numpy as np
+           from statsmodels.datasets import grunfeld
+           data = grunfeld.load_pandas().data
+           data.year = data.year.astype(np.int64)
+           # MultiIndex, entity - time
+           data = data.set_index(['firm','year'])
+           from linearmodels import PanelOLS
+           mod = PanelOLS(data.invest, data[['value','capital']], entity_effects=True)
+           res = mod.fit(cov_type='clustered', cluster_entity=True)
         
         Models can also be specified using the formula interface.
         
         .. code:: python
         
-            from linearmodels import PanelOLS
-            mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffect', data)
-            res = mod.fit(cov_type='clustered', cluster_entity=True)
+           from linearmodels import PanelOLS
+           mod = PanelOLS.from_formula('invest ~ value + capital + EntityEffects', data)
+           res = mod.fit(cov_type='clustered', cluster_entity=True)
         
         The formula interface for ``PanelOLS`` supports the special values
         ``EntityEffects`` and ``TimeEffects`` which add entity (fixed) and time
         effects, respectively.
         
         Instrumental Variable Models
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         IV regression models can be similarly specified.
         
         .. code:: python
         
-            import numpy as np
-            from linearmodels.iv import IV2SLS
-            from linearmodels.datasets import mroz
-            data = mroz.load()
-            mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
+           import numpy as np
+           from linearmodels.iv import IV2SLS
+           from linearmodels.datasets import mroz
+           data = mroz.load()
+           mod = IV2SLS.from_formula('np.log(wage) ~ 1 + exper + exper ** 2 + [educ ~ motheduc + fatheduc]', data)
         
         The expressions in the ``[ ]`` indicate endogenous regressors (before
         ``~``) and the instruments.
         
         Installing
         ----------
         
         The latest release can be installed using pip
         
         .. code:: bash
         
-            pip install linearmodels
+           pip install linearmodels
         
         The master branch can be installed by cloning the repo and running setup
         
         .. code:: bash
         
-            git clone https://github.com/bashtage/linearmodels
-            cd linearmodels
-            python setup.py install
+           git clone https://github.com/bashtage/linearmodels
+           cd linearmodels
+           python setup.py install
         
         Documentation
         -------------
         
         `Stable Documentation <https://bashtage.github.io/linearmodels/>`__ is
         built on every tagged version using
         `doctr <https://github.com/drdoctr/doctr>`__. `Development
@@ -152,29 +152,35 @@
         -  xarray (0.9+, optional)
         
         Testing
         ~~~~~~~
         
         -  py.test
         
+        .. _documentation-1:
+        
         Documentation
         ~~~~~~~~~~~~~
         
         -  sphinx
-        -  guzzle\_sphinx\_theme
+        -  guzzle_sphinx_theme
         -  nbsphinx
         -  nbconvert
         -  nbformat
         -  ipython
         -  jupyter
         
         .. |Build Status| image:: https://travis-ci.org/bashtage/linearmodels.svg?branch=master
            :target: https://travis-ci.org/bashtage/linearmodels
         .. |codecov| image:: https://codecov.io/gh/bashtage/linearmodels/branch/master/graph/badge.svg
            :target: https://codecov.io/gh/bashtage/linearmodels
+        .. |Codacy Badge| image:: https://api.codacy.com/project/badge/Grade/c771bce50a164b6fa71c344b374f140d
+           :target: https://www.codacy.com/app/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade
+        .. |codebeat badge| image:: https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243
+           :target: https://codebeat.co/projects/github-com-bashtage-linearmodels-master
         
 Keywords: linear models,regression,instrumental variables,IV,panel,fixed effects,clustered,heteroskedasticity,endogeneity,instruments,statistics,statistical inference,econometrics
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `linearmodels-4.8/linearmodels.egg-info/SOURCES.txt` & `linearmodels-4.9/linearmodels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 ./linearmodels/system/__init__.py
 ./linearmodels/system/_utility.py
 ./linearmodels/system/covariance.py
 ./linearmodels/system/gmm.py
 ./linearmodels/system/model.py
 ./linearmodels/system/results.py
 ./linearmodels/tests/__init__.py
+./linearmodels/tests/test_compat.py
 ./linearmodels/tests/test_examples.py
 ./linearmodels/tests/test_utility.py
 ./linearmodels/tests/asset_pricing/__init__.py
 ./linearmodels/tests/asset_pricing/_utility.py
 ./linearmodels/tests/asset_pricing/test_covariance.py
 ./linearmodels/tests/asset_pricing/test_formulas.py
 ./linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
@@ -109,20 +110,24 @@
 ./linearmodels/tests/system/test_utility.py
 ./linearmodels/tests/system/results/__init__.py
 ./linearmodels/tests/system/results/execute-stata-3sls.py
 ./linearmodels/tests/system/results/execute-stata.py
 ./linearmodels/tests/system/results/generate_data.py
 ./linearmodels/tests/system/results/parse_stata_3sls_results.py
 ./linearmodels/tests/system/results/parse_stata_results.py
+./linearmodels/typing/__init__.py
+./linearmodels/typing/iv.py
 doc/source/changes.rst
 doc/source/conf.py
 doc/source/contributing.rst
 doc/source/index.rst
+doc/source/names_wordlist.txt
 doc/source/plan.rst
 doc/source/references.rst
+doc/source/spelling_wordlist.txt
 doc/source/utility.rst
 doc/source/_static/css/overrides.css
 doc/source/_templates/layout.html
 doc/source/asset-pricing/convert-lyx.cmd
 doc/source/asset-pricing/covariance.rst
 doc/source/asset-pricing/index.rst
 doc/source/asset-pricing/introduction.rst
@@ -240,14 +245,15 @@
 linearmodels/system/__init__.py
 linearmodels/system/_utility.py
 linearmodels/system/covariance.py
 linearmodels/system/gmm.py
 linearmodels/system/model.py
 linearmodels/system/results.py
 linearmodels/tests/__init__.py
+linearmodels/tests/test_compat.py
 linearmodels/tests/test_examples.py
 linearmodels/tests/test_utility.py
 linearmodels/tests/asset_pricing/__init__.py
 linearmodels/tests/asset_pricing/_utility.py
 linearmodels/tests/asset_pricing/test_covariance.py
 linearmodels/tests/asset_pricing/test_formulas.py
 linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
@@ -312,8 +318,10 @@
 linearmodels/tests/system/results/execute-stata.py
 linearmodels/tests/system/results/generate_data.py
 linearmodels/tests/system/results/parse_stata_3sls_results.py
 linearmodels/tests/system/results/parse_stata_results.py
 linearmodels/tests/system/results/simulated-3sls.dta
 linearmodels/tests/system/results/simulated-sur.dta
 linearmodels/tests/system/results/stata-3sls-results.txt
-linearmodels/tests/system/results/stata-sur-results.txt
+linearmodels/tests/system/results/stata-sur-results.txt
+linearmodels/typing/__init__.py
+linearmodels/typing/iv.py
```

### Comparing `linearmodels-4.8/versioneer.py` & `linearmodels-4.9/versioneer.py`

 * *Files identical despite different names*

