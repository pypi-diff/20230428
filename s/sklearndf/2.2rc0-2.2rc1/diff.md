# Comparing `tmp/sklearndf-2.2rc0.tar.gz` & `tmp/sklearndf-2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearndf-2.2rc0.tar", last modified: Mon Jan 23 15:14:29 2023, max compression
+gzip compressed data, was "sklearndf-2.2rc1.tar", last modified: Fri Apr 28 06:48:27 2023, max compression
```

## Comparing `sklearndf-2.2rc0.tar` & `sklearndf-2.2rc1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0      834 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4921 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/.gitignore
--rw-r--r--   0        0        0     1098 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/LICENSE
--rw-r--r--   0        0        0    11419 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/README.rst
--rw-r--r--   0        0        0     8197 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    25405 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/azure-pipelines.yml
--rw-r--r--   0        0        0     2345 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/config/spelling.dic
--rw-r--r--   0        0        0      124 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/config/test_config.yml
--rwxr-xr-x   0        0        0       97 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/dev-setup.sh
--rw-r--r--   0        0        0      919 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/environment.yml
--rwxr-xr-x   0        0        0      380 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/make.py
--rw-r--r--   0        0        0      660 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/mypy.ini
--rw-r--r--   0        0        0     2070 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/pypi_description.rst
--rw-r--r--   0        0        0     3387 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-01-23 15:12:31.671745 sklearndf-2.2rc0/sphinx/.gitignore
--rw-r--r--   0        0        0    14394 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/auxiliary/Titanic_getting_started_example.ipynb
--rwxr-xr-x   0        0        0      664 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/make.py
--rw-r--r--   0        0        0    19025 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/_images/gamma_sklearndf_logo.png
--rw-r--r--   0        0        0    10916 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/_images/sklearndf-class-hierarchy.graffle/data.plist
--rw-r--r--   0        0        0    13433 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/_images/sklearndf-class-hierarchy.svg
--rw-r--r--   0        0        0     9791 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/_images/sklearndf_logo.png
--rw-r--r--   0        0        0     3448 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      769 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/conf.py
--rw-r--r--   0        0        0    17214 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     1142 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      281 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/index.rst
--rw-r--r--   0        0        0    66006 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/tutorial/sklearndf_tutorial.ipynb
--rw-r--r--   0        0        0      369 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/sphinx/source/tutorials.rst
--rw-r--r--   0        0        0      291 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/__init__.py
--rw-r--r--   0        0        0      703 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/_sklearn_version.py
--rw-r--r--   0        0        0    21217 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/_sklearndf.py
--rw-r--r--   0        0        0     2251 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/_util.py
--rw-r--r--   0        0        0      474 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/__init__.py
--rw-r--r--   0        0        0    10036 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/_classification.py
--rw-r--r--   0        0        0     1461 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/_classification_v0_22.py
--rw-r--r--   0        0        0      937 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/_classification_v0_23.py
--rw-r--r--   0        0        0     1211 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/_classification_v1_0.py
--rw-r--r--   0        0        0      347 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/extra/__init__.py
--rw-r--r--   0        0        0     1336 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/extra/_extra.py
--rw-r--r--   0        0        0      125 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/wrapper/__init__.py
--rw-r--r--   0        0        0     6735 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/classification/wrapper/_wrapper.py
--rw-r--r--   0        0        0      264 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/clustering/__init__.py
--rw-r--r--   0        0        0     2464 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/clustering/_clustering.py
--rw-r--r--   0        0        0      680 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/clustering/_clustering_v1_1.py
--rw-r--r--   0        0        0      124 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/clustering/wrapper/__init__.py
--rw-r--r--   0        0        0     2036 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/clustering/wrapper/_wrapper.py
--rw-r--r--   0        0        0      155 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/pipeline/__init__.py
--rw-r--r--   0        0        0    12410 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/pipeline/_learner_pipeline.py
--rw-r--r--   0        0        0      736 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/pipeline/_pipeline.py
--rw-r--r--   0        0        0      145 2023-01-23 15:12:31.675745 sklearndf-2.2rc0/src/sklearndf/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0    10865 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/pipeline/wrapper/_wrapper.py
--rw-r--r--   0        0        0        0 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/py.typed
--rw-r--r--   0        0        0      457 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/__init__.py
--rw-r--r--   0        0        0    11191 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/_regression.py
--rw-r--r--   0        0        0     1152 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/_regression_v0_22.py
--rw-r--r--   0        0        0     1525 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/_regression_v0_23.py
--rw-r--r--   0        0        0     1455 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/_regression_v1_0.py
--rw-r--r--   0        0        0      346 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/extra/__init__.py
--rw-r--r--   0        0        0     1309 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/extra/_extra.py
--rw-r--r--   0        0        0      124 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/wrapper/__init__.py
--rw-r--r--   0        0        0     4698 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/regression/wrapper/_wrapper.py
--rw-r--r--   0        0        0      602 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/__init__.py
--rw-r--r--   0        0        0    15437 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/_transformation.py
--rw-r--r--   0        0        0     1071 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v0_22.py
--rw-r--r--   0        0        0     1614 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v0_24.py
--rw-r--r--   0        0        0      973 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v1_0.py
--rw-r--r--   0        0        0     1246 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v1_1.py
--rw-r--r--   0        0        0      348 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/extra/__init__.py
--rw-r--r--   0        0        0      916 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/extra/_extra.py
--rw-r--r--   0        0        0      135 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/extra/wrapper/__init__.py
--rw-r--r--   0        0        0     1205 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/extra/wrapper/_wrapper.py
--rw-r--r--   0        0        0      126 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/wrapper/__init__.py
--rw-r--r--   0        0        0    27804 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/transformation/wrapper/_wrapper.py
--rw-r--r--   0        0        0     2392 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/__init__.py
--rw-r--r--   0        0        0     1137 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/_missing.py
--rw-r--r--   0        0        0    47761 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/_wrapper.py
--rw-r--r--   0        0        0      269 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/numpy/__init__.py
--rw-r--r--   0        0        0    11212 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/numpy/_numpy.py
--rw-r--r--   0        0        0       78 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/stacking/__init__.py
--rw-r--r--   0        0        0    12154 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/src/sklearndf/wrapper/stacking/_stacking.py
--rw-r--r--   0        0        0       38 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/__init__.py
--rw-r--r--   0        0        0     3222 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/conftest.py
--rw-r--r--   0        0        0      195 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/paths.py
--rw-r--r--   0        0        0     5272 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/sklearndf/__init__.py
--rw-r--r--   0        0        0     1015 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/sklearndf/pipeline/__init__.py
--rw-r--r--   0        0        0     1496 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_classification_pipeline_df.py
--rw-r--r--   0        0        0     1040 2023-01-23 15:12:31.679745 sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_clustering_pipeline.py
--rw-r--r--   0        0        0    13550 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_pipeline_df.py
--rw-r--r--   0        0        0     1453 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_regression_pipeline_df.py
--rw-r--r--   0        0        0     8288 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_base.py
--rw-r--r--   0        0        0     7171 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_classification.py
--rw-r--r--   0        0        0     1857 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_clustering.py
--rw-r--r--   0        0        0     6545 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_meta_estimators.py
--rw-r--r--   0        0        0      448 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_missing.py
--rw-r--r--   0        0        0     4585 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_regression.py
--rw-r--r--   0        0        0     7259 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/test_sklearn_coverage.py
--rw-r--r--   0        0        0        0 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/transformation/__init__.py
--rw-r--r--   0        0        0     2163 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/transformation/test_extra.py
--rw-r--r--   0        0        0     2682 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/transformation/test_imputers.py
--rw-r--r--   0        0        0     3458 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/transformation/test_sparse.py
--rw-r--r--   0        0        0    19562 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/sklearndf/transformation/test_transformation.py
--rw-r--r--   0        0        0     1205 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/test/test/test_docs.py
--rw-r--r--   0        0        0     2511 2023-01-23 15:12:31.683745 sklearndf-2.2rc0/tox.ini
--rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 sklearndf-2.2rc0/PKG-INFO
+-rw-r--r--   0        0        0      834 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     4921 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/.gitignore
+-rw-r--r--   0        0        0     1098 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/LICENSE
+-rw-r--r--   0        0        0    11419 2023-04-28 06:46:56.942777 sklearndf-2.2rc1/README.rst
+-rw-r--r--   0        0        0     8368 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0    26130 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/azure-pipelines.yml
+-rw-r--r--   0        0        0     2764 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/condabuild/meta.yaml
+-rw-r--r--   0        0        0        0 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/config/spelling.dic
+-rw-r--r--   0        0        0      124 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/config/test_config.yml
+-rwxr-xr-x   0        0        0       97 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/dev-setup.sh
+-rw-r--r--   0        0        0      960 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/environment.yml
+-rwxr-xr-x   0        0        0      380 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/make.py
+-rw-r--r--   0        0        0      745 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/mypy.ini
+-rw-r--r--   0        0        0     2070 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/pypi_description.rst
+-rw-r--r--   0        0        0     3439 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-28 06:46:56.946777 sklearndf-2.2rc1/sphinx/.gitignore
+-rw-r--r--   0        0        0    14394 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/auxiliary/Titanic_getting_started_example.ipynb
+-rwxr-xr-x   0        0        0      664 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/make.py
+-rw-r--r--   0        0        0    19025 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/_images/gamma_sklearndf_logo.png
+-rw-r--r--   0        0        0    10916 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/_images/sklearndf-class-hierarchy.graffle/data.plist
+-rw-r--r--   0        0        0    13433 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/_images/sklearndf-class-hierarchy.svg
+-rw-r--r--   0        0        0     9791 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/_images/sklearndf_logo.png
+-rw-r--r--   0        0        0     3448 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/api_landing.rst
+-rw-r--r--   0        0        0      769 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/conf.py
+-rw-r--r--   0        0        0    17214 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/contribution_guide.rst
+-rw-r--r--   0        0        0     1142 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/faqs.rst
+-rw-r--r--   0        0        0      281 2023-04-28 06:46:56.950778 sklearndf-2.2rc1/sphinx/source/index.rst
+-rw-r--r--   0        0        0    66006 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/sphinx/source/tutorial/sklearndf_tutorial.ipynb
+-rw-r--r--   0        0        0      369 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/sphinx/source/tutorials.rst
+-rw-r--r--   0        0        0      291 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/__init__.py
+-rw-r--r--   0        0        0      585 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/_sklearn_version.py
+-rw-r--r--   0        0        0    21217 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/_sklearndf.py
+-rw-r--r--   0        0        0     2251 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/_util.py
+-rw-r--r--   0        0        0      340 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/__init__.py
+-rw-r--r--   0        0        0    10036 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/_classification.py
+-rw-r--r--   0        0        0     1461 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/_classification_v0_22.py
+-rw-r--r--   0        0        0      937 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/_classification_v0_23.py
+-rw-r--r--   0        0        0     1211 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/_classification_v1_0.py
+-rw-r--r--   0        0        0      347 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/extra/__init__.py
+-rw-r--r--   0        0        0     1336 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/extra/_extra.py
+-rw-r--r--   0        0        0      125 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/wrapper/__init__.py
+-rw-r--r--   0        0        0     6735 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/classification/wrapper/_wrapper.py
+-rw-r--r--   0        0        0      264 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/clustering/__init__.py
+-rw-r--r--   0        0        0     2464 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/clustering/_clustering.py
+-rw-r--r--   0        0        0      680 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/clustering/_clustering_v1_1.py
+-rw-r--r--   0        0        0      124 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/clustering/wrapper/__init__.py
+-rw-r--r--   0        0        0     2036 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/clustering/wrapper/_wrapper.py
+-rw-r--r--   0        0        0      155 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/pipeline/__init__.py
+-rw-r--r--   0        0        0    12410 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/pipeline/_learner_pipeline.py
+-rw-r--r--   0        0        0      736 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/pipeline/_pipeline.py
+-rw-r--r--   0        0        0      145 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0    10865 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/pipeline/wrapper/_wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/py.typed
+-rw-r--r--   0        0        0      323 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/__init__.py
+-rw-r--r--   0        0        0    11191 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/_regression.py
+-rw-r--r--   0        0        0     1152 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/_regression_v0_22.py
+-rw-r--r--   0        0        0     1525 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/_regression_v0_23.py
+-rw-r--r--   0        0        0     1455 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/_regression_v1_0.py
+-rw-r--r--   0        0        0      346 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/extra/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/extra/_extra.py
+-rw-r--r--   0        0        0      124 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/wrapper/__init__.py
+-rw-r--r--   0        0        0     4698 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/regression/wrapper/_wrapper.py
+-rw-r--r--   0        0        0      510 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/__init__.py
+-rw-r--r--   0        0        0    15437 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/_transformation.py
+-rw-r--r--   0        0        0     1071 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v0_22.py
+-rw-r--r--   0        0        0     1614 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v0_24.py
+-rw-r--r--   0        0        0      973 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v1_0.py
+-rw-r--r--   0        0        0     1246 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v1_1.py
+-rw-r--r--   0        0        0      348 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/extra/__init__.py
+-rw-r--r--   0        0        0     3088 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/extra/_extra.py
+-rw-r--r--   0        0        0      135 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/extra/wrapper/__init__.py
+-rw-r--r--   0        0        0     1736 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/extra/wrapper/_wrapper.py
+-rw-r--r--   0        0        0      126 2023-04-28 06:46:56.954778 sklearndf-2.2rc1/src/sklearndf/transformation/wrapper/__init__.py
+-rw-r--r--   0        0        0    27804 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/transformation/wrapper/_wrapper.py
+-rw-r--r--   0        0        0     2392 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/__init__.py
+-rw-r--r--   0        0        0     1137 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/_missing.py
+-rw-r--r--   0        0        0    49579 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/_wrapper.py
+-rw-r--r--   0        0        0      269 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/numpy/__init__.py
+-rw-r--r--   0        0        0    11212 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/numpy/_numpy.py
+-rw-r--r--   0        0        0       78 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/stacking/__init__.py
+-rw-r--r--   0        0        0    12154 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/src/sklearndf/wrapper/stacking/_stacking.py
+-rw-r--r--   0        0        0       38 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/__init__.py
+-rw-r--r--   0        0        0     3503 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/conftest.py
+-rw-r--r--   0        0        0      195 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/paths.py
+-rw-r--r--   0        0        0     5146 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/pipeline/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_classification_pipeline_df.py
+-rw-r--r--   0        0        0     1040 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_clustering_pipeline.py
+-rw-r--r--   0        0        0    13550 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_pipeline_df.py
+-rw-r--r--   0        0        0     1453 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_regression_pipeline_df.py
+-rw-r--r--   0        0        0     8288 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_base.py
+-rw-r--r--   0        0        0     7002 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_classification.py
+-rw-r--r--   0        0        0     1857 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_clustering.py
+-rw-r--r--   0        0        0     6893 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_meta_estimators.py
+-rw-r--r--   0        0        0      448 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_missing.py
+-rw-r--r--   0        0        0     4376 2023-04-28 06:46:56.962778 sklearndf-2.2rc1/test/test/sklearndf/test_regression.py
+-rw-r--r--   0        0        0     7091 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/test_sklearn_coverage.py
+-rw-r--r--   0        0        0        0 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/transformation/__init__.py
+-rw-r--r--   0        0        0     4058 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/transformation/test_extra.py
+-rw-r--r--   0        0        0     2682 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/transformation/test_imputers.py
+-rw-r--r--   0        0        0     3458 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/transformation/test_sparse.py
+-rw-r--r--   0        0        0    19369 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/sklearndf/transformation/test_transformation.py
+-rw-r--r--   0        0        0     1422 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/test/test/test_docs.py
+-rw-r--r--   0        0        0     2618 2023-04-28 06:46:56.966778 sklearndf-2.2rc1/tox.ini
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 sklearndf-2.2rc1/PKG-INFO
```

### Comparing `sklearndf-2.2rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `sklearndf-2.2rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/.github/ISSUE_TEMPLATE/feature_request.md` & `sklearndf-2.2rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/.gitignore` & `sklearndf-2.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/.pre-commit-config.yaml` & `sklearndf-2.2rc1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 repos:
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
     rev: 22.8.0
     hooks:
       - id: black
         language: python_venv
         language_version: python39
 
-  - repo: https://gitlab.com/pycqa/flake8
+  - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         name: flake8
         entry: flake8 --config tox.ini
         language: python_venv
         language_version: python39
@@ -30,15 +30,15 @@
       - id: check-json
       - id: check-xml
       - id: check-yaml
         language: python_venv
         exclude: condabuild/meta.yaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.981
+    rev: v1.2.0
     hooks:
       - id: mypy
         files: src|sphinx|test
         language: python_venv
         language_version: python39
         additional_dependencies:
           - numpy~=1.22
```

### Comparing `sklearndf-2.2rc0/LICENSE` & `sklearndf-2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/README.rst` & `sklearndf-2.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/RELEASE_NOTES.rst` & `sklearndf-2.2rc1/RELEASE_NOTES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 API.
 
 2.2.0
 ~~~~~
 
 *sklearndf* 2.2 adds support for
 `scikit-learn |nbsp| 1.2 <https://scikit-learn.org/1.2>`_.
+It drops support for *scikit-learn* |nbsp| 0.23 and earlier due to incomplete
+support of sparse output (see below).
 
 - API: DF estimators now support native estimators using sparse matrices as input or
   output, and automatically convert them to or from sparse :class:`~pandas.DataFrame`
   objects
 - API: new property :attr:`.EstimatorDF.output_names_` to get the names of the output
   columns the estimator was fitted with
 - API: new method :attr:`.LearnerPipelineDF.preprocess` to apply the preprocessing step
@@ -73,23 +75,26 @@
 ---------------
 
 *sklearndf* 2.0 adds support for
 `scikit-learn |nbsp| 1.0 <https://scikit-learn.org/1.0>`_,
 adds data frame support for clusterers along with additional API enhancements and
 improvements, and is now subject to static type checking with |mypy|.
 
+
 2.0.2
 ~~~~~
 
+- BUILD: add support for :mod:`pandas` 2.0 and above
 - FIX: property :attr:`.PCADF.n_components_` now returns the value of
   :attr:`~sklearndf.decomposition.PCA.n_components_`, not
   :attr:`~sklearndf.decomposition.PCA.n_components`
 - FIX: detect missing and extra columns when validating data frames resulting from
   transforms, even when the total column count is correct
 
+
 2.0.1
 ~~~~~
 
 - API: upon declaration of new wrapper classes, automatically validate that their
   associated native estimators are compatible with the wrapper class
 - API: new public constants ``DROP`` and ``PASSTHROUGH`` in
   :class:`.ColumnTransformerDF`
```

### Comparing `sklearndf-2.2rc0/azure-pipelines.yml` & `sklearndf-2.2rc1/azure-pipelines.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 resources:
   repositories:
     - repository: pytools
       type: github
       endpoint: BCG-Gamma
       name: BCG-Gamma/pytools
-      ref: 2.0.x
+      ref: 2.1.x
 
 variables:
   ${{ if not(startsWith(variables['Build.SourceBranch'], 'refs/pull/')) }}:
     branchName: $[ replace(variables['Build.SourceBranch'], 'refs/heads/', '') ]
   ${{ if startsWith(variables['Build.SourceBranch'], 'refs/pull/') }}:
     branchName: $[ replace(variables['System.PullRequest.SourceBranch'], 'refs/heads/', '') ]
   source_is_release_branch: $[ startsWith(variables['branchName'], 'release/') ]
@@ -50,15 +50,15 @@
         displayName: 'isort'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install isort~=5.10
+              python -m pip install isort~=5.12
               python -m isort --check --diff .
             displayName: 'Run isort'
       - job:
         displayName: 'black'
         steps:
           - task: UsePythonVersion@0
             inputs:
@@ -83,39 +83,42 @@
         displayName: 'mypy'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install mypy~=0.981 numpy~=1.22 gamma-pytools~=2.1rc
+              python -m pip install mypy~=1.2.0 numpy~=1.24 gamma-pytools~=2.1rc
               python -m mypy src
             displayName: 'Run mypy'
 
   # detect whether the build config (pyproject.toml) was changed -> then we must run a build test
   - stage: detect_build_config_changes
     displayName: 'Pyproject.toml build config'
 
     jobs:
 
       - job: checkout_and_diff
         displayName: 'detect changes'
         steps:
           - checkout: self
+            fetchDepth: 2
 
           - task: Bash@3
             name: diff
             inputs:
               targetType: 'inline'
               script: |
+                set -eux
+
                 echo Repo: $(Build.DefinitionName)
                 cd $(System.DefaultWorkingDirectory)
-                files_changed=$(git diff $(Build.SourceVersion)^! --name-only)
+                files_changed=$(git diff $(Build.SourceVersion)^ --name-only)
                 echo "Files changed since last commit: ${files_changed}"
-                n_files_changed=$(git diff $(Build.SourceVersion)^! --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
+                n_files_changed=$(git diff $(Build.SourceVersion)^ --name-only | grep -i -E 'meta\.yaml|pyproject\.toml|azure-pipelines\.yml|tox\.ini|make\.py'  | wc -l | xargs)
                 if [ ${n_files_changed} -gt 0 ]
                 then
                 build_changed=1
                 echo "build config has been changed"
                 else
                 build_changed=0
                 echo "build config is unchanged";
@@ -137,30 +140,35 @@
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
 
-                conda env create
-                conda activate $(project_name)-develop
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
 
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 pytest \
                    --cov $(project_name) \
                    --cov-config "tox.ini" \
@@ -405,16 +413,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             env:
               BRANCH_NAME: $(branchName)
@@ -470,16 +478,16 @@
           eq(variables.source_is_release_branch, 'True'),
           eq(variables.source_is_develop_branch, 'True')
           )
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - checkout: pytools
           - checkout: self
 
           - task: Bash@3
             inputs:
               targetType: inline
@@ -597,16 +605,16 @@
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
           - task: UsePythonVersion@0
             inputs:
-              versionSpec: '3.8'
-            displayName: 'use Python 3.8'
+              versionSpec: '3.9'
+            displayName: 'use Python 3.9'
 
           - task: InstallSSHKey@0
             inputs:
               knownHostsEntry: $(knownHostsEntry)
               sshPublicKey: $(sshPublicKey)
               sshKeySecureFile: 'deploy_docs_$(project_name)'
             displayName: 'Install the deploy SSH key'
@@ -637,49 +645,54 @@
             displayName: 'Retrieve current documentation versions from github-pages'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
 
                 cd $(System.DefaultWorkingDirectory)
                 echo "Checking out $(branchName)"
                 git checkout $(branchName)
 
-                conda env create
-                conda activate $(project_name)-develop
+                # install micromamba
+                curl -Ls https://micro.mamba.pm/api/micromamba/linux-64/latest | tar -xvj bin/micromamba
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
+                # install the develop environment
+                micromamba env create --yes --file environment.yml
+                micromamba activate $(project_name)-develop
 
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
 
                 python sphinx/make.py html
 
             displayName: 'Build latest documentation'
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                eval "$(conda shell.bash hook)"
+                export MAMBA_ROOT_PREFIX=~/micromamba
+                eval "$(./bin/micromamba shell hook -s posix)"
 
                 # install the tree utility
                 sudo apt-get install tree
 
                 cd $(System.DefaultWorkingDirectory)
 
                 echo "Restoring previous documentation to the docs directory"
                 mkdir -p docs
                 mv $(Build.ArtifactStagingDirectory)/docs-version.bak docs/docs-version
                 ls docs/docs-version
 
                 mkdir -p $(System.DefaultWorkingDirectory)/sphinx/build/
 
-                conda activate $(project_name)-develop
+                micromamba activate $(project_name)-develop
                 python sphinx/make.py prepare_docs_deployment
 
                 echo "Current docs contents:"
                 tree docs
                 mv docs $(Build.ArtifactStagingDirectory)/docs
             displayName: 'Merge previous and latest docs'
```

### Comparing `sklearndf-2.2rc0/condabuild/meta.yaml` & `sklearndf-2.2rc1/condabuild/meta.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
   host:
     - pip>=20.*
     - python        {{ environ.get('FACET_V_PYTHON', '=3.8.*') }}
     - numpy         {{ environ.get('FACET_V_NUMPY', '>=1.11.*') }}
     - flit>=3.0.*
     - packaging>=20
   run:
-    - boruta_py     {{ environ.get('FACET_V_BORUTA') }}
     - gamma-pytools {{ environ.get('FACET_V_GAMMA_PYTOOLS') }}
     - numpy         {{ environ.get('FACET_V_NUMPY') }}
     - packaging     {{ environ.get('FACET_V_PACKAGING') }}
     - pandas        {{ environ.get('FACET_V_PANDAS') }}
     - python        {{ environ.get('FACET_V_PYTHON') }}
     - scikit-learn  {{ environ.get('FACET_V_SCIKIT_LEARN') }}
     - scipy         {{ environ.get('FACET_V_SCIPY') }}
@@ -33,26 +32,35 @@
     - sklearndf.pipeline
     - sklearndf.regression
     - sklearndf.regression.extra
     - sklearndf.transformation
     - sklearndf.transformation.extra
   requires:
     - pytest ~= 7.1
+    # we need pip to install arfs
+    - pip # {{ '[False]' if not environ.get('FACET_V_ARFS') }}
     # optional libraries of sklearndf, needed for testing
-    - lightgbm {{ environ.get('FACET_V_LIGHTGBM') }}
-    - xgboost  {{ environ.get('FACET_V_XGBOOST') }}
+    - boruta_py  {{ environ.get('FACET_V_BORUTA', '[False]') }}
+    - xgboost    {{ environ.get('FACET_V_XGBOOST', '[False]') }}
+    # we always need lightgbm for testing; version spec is optional
+    - lightgbm   {{ environ.get('FACET_V_LIGHTGBM', '') }}
     # additional requirements of gamma-pytools
-    - joblib          {{ environ.get('FACET_V_JOBLIB') }}
-    - matplotlib-base {{ environ.get('FACET_V_MATPLOTLIB') }}
-    - typing_inspect  {{ environ.get('FACET_V_TYPING_INSPECT') }}
+    - joblib          {{ environ.get('FACET_V_JOBLIB', '[False]') }}
+    - matplotlib-base {{ environ.get('FACET_V_MATPLOTLIB', '[False]') }}
+    - typing_inspect  {{ environ.get('FACET_V_TYPING_INSPECT', '[False]') }}
   commands:
     - conda list
     - python -c 'import sklearndf;
                  import os;
                  assert sklearndf.__version__ == os.environ["PKG_VERSION"]'
+    # optional PyPi package ARFS needed for testing
+    {% if environ.get('FACET_V_ARFS') -%}
+    - pip install 'arfs{{ environ.get("FACET_V_ARFS") }}'
+    {%- endif %}
+    # run the test suite
     - cd "${FACET_PATH}/sklearndf"
     - pytest -vs test
 
 about:
   home: https://github.com/BCG-Gamma/sklearndf
   license: Apache Software License v2.0
   license_file: LICENSE
```

### Comparing `sklearndf-2.2rc0/environment.yml` & `sklearndf-2.2rc1/environment.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 name: sklearndf-develop
 channels:
   - conda-forge
   - bcg_gamma
 dependencies:
   # run
-  - boruta_py ~= 0.3
-  - gamma-pytools ~= 2.1rc, <3a
+  - gamma-pytools ~= 2.1rc1, <3a
   - joblib ~= 1.2
-  - lightgbm ~= 3.3.4
-  - matplotlib ~= 3.6.3
-  - numpy ~= 1.23.5
-  - pandas ~= 1.5.3
-  - python ~= 3.9.15
-  - scikit-learn ~= 1.2.0
+  - lightgbm ~= 3.3
+  - matplotlib ~= 3.6
+  - numpy ~= 1.24
+  - pandas ~=1.5|~=2.0
+  - python ~= 3.9
+  - scikit-learn ~= 1.2.2
   - scipy ~= 1.10.0
-  - xgboost ~= 1.7.1
+  - xgboost ~= 1.7
+  - pip ~= 23.0.1
+  - pip:
+    - arfs ~= 1.0.5
+    - shap ~= 0.41.0
   # build/test
   - conda-build ~= 3.23.3
   - conda-verify ~= 3.1.1
   - docutils ~= 0.17.1
   - flit ~= 3.8.0
   - jinja2 ~= 2.11.3
   - markupsafe ~= 2.0.1  # markupsafe 2.1 breaks support for jinja2
   - m2r ~= 0.3.1
   - pluggy ~= 0.13.1
   - pre-commit ~= 2.21.0
-  - pytest ~= 7.2.1
+  - pytest ~= 7.2.2
   - pytest-cov ~= 2.12.1
   - pyyaml ~= 5.4.1
   - toml ~= 0.10.2
   - tox ~= 3.27.1
   - yaml ~= 0.2.5
   # sphinx
-  - nbsphinx ~= 0.8.9
+  - nbsphinx ~= 0.8.12
   - sphinx ~= 4.5.0
   - sphinx-autodoc-typehints ~= 1.19.2
   - pydata-sphinx-theme ~= 0.8.1
   # notebooks
-  - jupyterlab ~= 3.5.2
+  - jupyterlab ~= 3.5.3
   - openpyxl ~= 3.0.10
   - seaborn ~= 0.12.2
```

### Comparing `sklearndf-2.2rc0/mypy.ini` & `sklearndf-2.2rc1/mypy.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 [mypy]
 strict = True
 show_error_codes = True
 
+[mypy-arfs.*]
+; TODO remove once PEP 561 is supported
+ignore_missing_imports = True
+
 [mypy-boruta.*]
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
 
 [mypy-lightgbm.*]
 ; TODO remove once PEP 561 is supported
 ignore_missing_imports = True
```

### Comparing `sklearndf-2.2rc0/pypi_description.rst` & `sklearndf-2.2rc1/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/pyproject.toml` & `sklearndf-2.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 author = "Boston Consulting Group (BCG)"
 home-page = "https://github.com/BCG-Gamma/sklearndf"
 description-file = "pypi_description.rst"
 dist-name = "sklearndf"
 license = "Apache Software License v2.0"
 
 requires = [
-    "gamma-pytools  ~=2.1rc",
+    "gamma-pytools  >=2.1rc2,<3a",
     "numpy          >=1.21,<1.24a",  # cannot use ~= due to conda bug
     "packaging      >=20",
-    "pandas         >=1.0,<2a",  # cannot use ~= due to conda bug
+    "pandas         >=1",
     "scikit-learn   >=0.24,<1.3a",
     "scipy          ~=1.4",
 ]
 
 requires-python = ">=3.7,<4a"
 
 classifiers = [
@@ -38,19 +38,19 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.flit.metadata.requires-extra]
 testing = [
-    "boruta ~=0.3",
-    "lightgbm ~= 3.3",
     "pytest ~= 7.1",
-    "pytest-cov ~= 2.8",
-    "xgboost ~= 1.5",
+    "pytest-cov ~= 2.12",
+    # optional requirements for testing sklearndf
+    "lightgbm ~= 3.0",
+    "xgboost ~= 1.0",
 ]
 docs = [
     "sphinx ~= 4.5",
     "sphinx-autodoc-typehints ~= 1.19",
     "pydata-sphinx-theme ~= 0.8.1",
     "jinja2 ~= 2.11",
     "nbsphinx ~= 0.8.9",
@@ -67,15 +67,15 @@
 [build]
 # comma-separated list of packages to be built from source in pip min builds
 no-binary.min = ["matplotlib"]
 
 [build.matrix.min]
 # direct requirements of sklearndf
 boruta         = "~=0.3.0"
-gamma-pytools  = "~=2.1rc"
+gamma-pytools  = "~=2.1rc2"
 lightgbm       = "~=3.0.0"
 numpy          = "==1.21.6"  # cannot use ~= due to conda bug
 packaging      = "~=20.9"
 pandas         = "~=1.1.5"
 python         = ">=3.7.12,<3.8a"    # cannot use ~= due to conda bug
 scipy          = "~=1.4.1"
 scikit-learn   = "~=0.24.2"
@@ -83,21 +83,21 @@
 # additional minimum requirements of gamma-pytools
 joblib         = "~=0.14.1"
 matplotlib     = "~=3.0.3"
 typing_inspect = "~=0.4.0"
 
 [build.matrix.max]
 # direct requirements of sklearndf
-boruta         = "~=0.3"
-gamma-pytools  = "~=2.1rc"
+arfs           = "~=1.0.5"
+gamma-pytools  = ">=2.1rc2,<3a"
 lightgbm       = "~=3.3"
 numpy          = ">=1.23,<1.24a"  # cannot use ~= due to conda bug
 packaging      = ">=20"
-pandas         = "~=1.4"
-python         = ">=3.9,<4a"   # cannot use ~= due to conda bug
+pandas         = "~=2.0"
+python         = ">=3.9,<3.11a"   # cannot use ~= due to conda bug; arfs <=1.0.7 does not support python >=3.11
 scikit-learn   = "~=1.1,<1.3a" # todo: replace with ~=1.2.0 once it is released
 scipy          = "~=1.8"
 xgboost        = "~=1.5"
 # additional maximum requirements of gamma-pytools
 joblib         = "~=1.1"
 matplotlib     = "~=3.5"
 typing_inspect = "~=0.7"
```

### Comparing `sklearndf-2.2rc0/sphinx/auxiliary/Titanic_getting_started_example.ipynb` & `sklearndf-2.2rc1/sphinx/auxiliary/Titanic_getting_started_example.ipynb`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/make.py` & `sklearndf-2.2rc1/sphinx/make.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/_images/gamma_sklearndf_logo.png` & `sklearndf-2.2rc1/sphinx/source/_images/gamma_sklearndf_logo.png`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/_images/sklearndf-class-hierarchy.graffle/data.plist` & `sklearndf-2.2rc1/sphinx/source/_images/sklearndf-class-hierarchy.graffle/data.plist`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/_images/sklearndf-class-hierarchy.svg` & `sklearndf-2.2rc1/sphinx/source/_images/sklearndf-class-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/_images/sklearndf_logo.png` & `sklearndf-2.2rc1/sphinx/source/_images/sklearndf_logo.png`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/api_landing.rst` & `sklearndf-2.2rc1/sphinx/source/api_landing.rst`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/conf.py` & `sklearndf-2.2rc1/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/contribution_guide.rst` & `sklearndf-2.2rc1/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/faqs.rst` & `sklearndf-2.2rc1/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/sphinx/source/tutorial/sklearndf_tutorial.ipynb` & `sklearndf-2.2rc1/sphinx/source/tutorial/sklearndf_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/_sklearn_version.py` & `sklearndf-2.2rc1/src/sklearndf/_sklearn_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 """
 
 from packaging.version import Version
 from sklearn import __version__ as sklearn_version
 
 __all__ = [
     "__sklearn_version__",
-    "__sklearn_0_22__",
-    "__sklearn_0_23__",
     "__sklearn_0_24__",
     "__sklearn_1_0__",
     "__sklearn_1_1__",
     "__sklearn_1_2__",
     "__sklearn_1_3__",
     "__sklearn_1_4__",
 ]
 
 __sklearn_version__ = Version(sklearn_version)
-__sklearn_0_22__ = Version("0.22")
-__sklearn_0_23__ = Version("0.23")
 __sklearn_0_24__ = Version("0.24")
 __sklearn_1_0__ = Version("1.0")
 __sklearn_1_1__ = Version("1.1")
 __sklearn_1_2__ = Version("1.2dev")
 __sklearn_1_3__ = Version("1.3")
 __sklearn_1_4__ = Version("1.4")
```

### Comparing `sklearndf-2.2rc0/src/sklearndf/_sklearndf.py` & `sklearndf-2.2rc1/src/sklearndf/_sklearndf.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/_util.py` & `sklearndf-2.2rc1/src/sklearndf/_util.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/_classification.py` & `sklearndf-2.2rc1/src/sklearndf/classification/_classification.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/_classification_v0_22.py` & `sklearndf-2.2rc1/src/sklearndf/classification/_classification_v0_22.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/_classification_v0_23.py` & `sklearndf-2.2rc1/src/sklearndf/classification/_classification_v0_23.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/_classification_v1_0.py` & `sklearndf-2.2rc1/src/sklearndf/classification/_classification_v1_0.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/extra/_extra.py` & `sklearndf-2.2rc1/src/sklearndf/classification/extra/_extra.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/classification/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/classification/wrapper/_wrapper.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/clustering/_clustering.py` & `sklearndf-2.2rc1/src/sklearndf/clustering/_clustering.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/clustering/_clustering_v1_1.py` & `sklearndf-2.2rc1/src/sklearndf/clustering/_clustering_v1_1.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/clustering/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/clustering/wrapper/_wrapper.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/pipeline/_learner_pipeline.py` & `sklearndf-2.2rc1/src/sklearndf/pipeline/_learner_pipeline.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/pipeline/_pipeline.py` & `sklearndf-2.2rc1/src/sklearndf/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/pipeline/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/pipeline/wrapper/_wrapper.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/_regression.py` & `sklearndf-2.2rc1/src/sklearndf/regression/_regression.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/_regression_v0_22.py` & `sklearndf-2.2rc1/src/sklearndf/regression/_regression_v0_22.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/_regression_v0_23.py` & `sklearndf-2.2rc1/src/sklearndf/regression/_regression_v0_23.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/_regression_v1_0.py` & `sklearndf-2.2rc1/src/sklearndf/regression/_regression_v1_0.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/extra/_extra.py` & `sklearndf-2.2rc1/src/sklearndf/regression/extra/_extra.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/regression/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/regression/wrapper/_wrapper.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/_transformation.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/_transformation.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v0_22.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v0_22.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v0_24.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v0_24.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v1_0.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v1_0.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/_transformation_v1_1.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/_transformation_v1_1.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/transformation/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/transformation/wrapper/_wrapper.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/wrapper/__init__.py` & `sklearndf-2.2rc1/src/sklearndf/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/wrapper/_missing.py` & `sklearndf-2.2rc1/src/sklearndf/wrapper/_missing.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/wrapper/_wrapper.py` & `sklearndf-2.2rc1/src/sklearndf/wrapper/_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,17 @@
     __ARG_FITTED_DELEGATE_CONTEXT = "__EstimatorWrapperDF_fitted"
 
     #: The native estimator that this wrapper delegates to.
     _native_estimator: T_NativeEstimator
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
-        :param args: positional arguments to use when initializing a new new delegate
+        :param args: positional arguments to use when initializing a new delegate
             estimator
-        :param kwargs: keyword arguments to use when initializing a new new delegate
+        :param kwargs: keyword arguments to use when initializing a new delegate
             estimator
         """
         super().__init__()
         self._features_in: Optional[pd.Index] = None
         self._outputs: Optional[List[str]] = None
 
         # check if a fitted estimator was passed by class method is_fitted
@@ -399,15 +399,16 @@
         except Exception as cause:
             self._reset_fit()
             raise self._make_verbose_exception(self.fit.__name__, cause) from cause
 
         return self
 
     def _validate_delegate_estimator(self) -> None:
-        # no validation required by default; to be overloaded as needed
+        # Called as the last step of the estimator wrapper's constructor.
+        # No validation required by default; to be overloaded as needed.
         pass
 
     def _get_features_in(self) -> pd.Index:
         assert self._features_in is not None, "estimator is fitted"
         return self._features_in
 
     def _get_outputs(self) -> Optional[List[str]]:
@@ -596,31 +597,50 @@
                 attr
                 for attr in self._native_estimator.__dir__()
                 if not attr.startswith("_")
             ),
         }
 
     def __getattr__(self, name: str) -> Any:
-        # get a non-private attribute of the delegate estimator
+        # This method is only called if the attribute name is not found in the
+        # instance's dictionary, and __getattribute__() has raised an AttributeError.
+
+        # For private attributes, give up and raise attribute error.
         if name.startswith("_"):
-            # raise attribute error
+            # The following will raise an AttributeError
             self.__getattribute__(name)
         else:
+            # For public attributes, try to get the attribute from the delegate
+            # estimator. If the attribute is not found, raise an attribute error.
             try:
                 return getattr(self._native_estimator, name)
             except AttributeError:
-                # raise attribute error
+                # The following will raise an AttributeError
                 self.__getattribute__(name)
 
     def __setattr__(self, name: str, value: Any) -> None:
-        # set a public attribute of the delegate estimator
+        # This method is called whenever an attribute assignment is attempted.
+
+        # For private attributes, set the attribute in this wrapper object.
         if name.startswith("_"):
             super().__setattr__(name, value)
         else:
-            setattr(self._native_estimator, name, value)
+            # For public attributes, set the attribute in this wrapper object only
+            # if it is already defined. Otherwise, set the attribute in the delegate
+            # estimator.
+
+            try:
+                self.__getattribute__(name)
+            except AttributeError:
+                # The attribute is not defined in this wrapper object, so set it in
+                # the delegate estimator.
+                setattr(self._native_estimator, name, value)
+            else:
+                # The attribute is defined in this wrapper object, so set it here.
+                super().__setattr__(name, value)
 
 
 @inheritdoc(match="[see superclass]")
 class TransformerWrapperDF(
     TransformerDF,
     EstimatorWrapperDF[T_NativeTransformer],
     Generic[T_NativeTransformer],
@@ -1068,15 +1088,15 @@
 
         if classes is None:
             classes = getattr(self.native_estimator, "classes_", None)
             if classes is None:
                 classes = pd.RangeIndex(self._get_n_outputs())
 
         if isinstance(prediction, pd.DataFrame):
-            return prediction.set_axis(classes, axis=1, inplace=False)
+            return prediction.set_axis(classes, axis=1)
 
         elif isinstance(prediction, np.ndarray):
             if len(prediction) == len(X):
                 # predictions of probabilities are usually provided as a NumPy array
                 # the same length as X
                 if prediction.ndim == 1:
                     # for a binary classifier, we get a series with probabilities
@@ -1207,40 +1227,58 @@
     Abstract base class of wrappers for estimators implementing
     :class:`sklearn.base.MetaEstimatorMixin`.
 
     A meta-estimator will call the methods of the embedded estimator using a modified
     copy of the `X` and `y` parameters, so we need to make sure that these are converted
     back to data frames.
 
-    This class covers three variants used in sklearn:
+    We also ensure that the embedded estimator is a native sci-kit learn estimator.
+    If it is a DF estimator, we replace it with its wrapped native estimator and
+    re-assign it to the attribute `estimator` or `base_estimator` (depending on the
+    meta-estimator).
+    In that case, we issue a warning that the wrapped estimator is being used instead
+    of the DF version.
+
+    This class covers three variants used in scikit-learn:
 
     - one delegate estimator in attribute `estimator`
     - one delegate estimator in attribute `base_estimator`
     - multiple delegate estimators in attribute `estimators`
     """
 
     def _validate_delegate_estimator(self) -> None:
-        meta_estimator = self.native_estimator
+        substituted: List[str] = []
 
-        estimator = getattr(meta_estimator, "estimator", None)
+        estimator = getattr(self, "estimator", None)
         if estimator is not None:
-            meta_estimator.estimator = self._native_learner(estimator)
+            self.estimator = self._native_learner(estimator)
+            substituted.append("estimator")
 
-        base_estimator = getattr(meta_estimator, "base_estimator", None)
+        base_estimator = getattr(self, "base_estimator", None)
         # attribute base_estimator is deprecated as of scikit-learn 1.2, with the
         # default value of "deprecated"
         if base_estimator is not None and base_estimator != "deprecated":
-            meta_estimator.base_estimator = self._native_learner(base_estimator)
+            self.base_estimator = self._native_learner(base_estimator)
+            substituted.append("base_estimator")
 
-        estimators = getattr(meta_estimator, "estimators", None)
+        estimators = getattr(self, "estimators", None)
         if estimators is not None:
-            meta_estimator.estimators = [
+            self.estimators = [
                 (name, self._native_learner(estimator))
                 for name, estimator in estimators
             ]
+            substituted.append("estimators")
+
+        if substituted:
+            warnings.warn(
+                f"the following attributes of {type(self).__name__} "
+                f"have been replaced with their native scikit-learn counterparts: "
+                f"{', '.join(substituted)}",
+                stacklevel=-2,
+            )
 
     @staticmethod
     def _native_learner(
         estimator_wrapper: BaseEstimator,
     ) -> Union[RegressorMixin, ClassifierMixin]:
         native_estimator: BaseEstimator = (
             estimator_wrapper.native_estimator
@@ -1270,15 +1308,15 @@
 ) -> None:
 
     wrapper_name = wrapper_class.__name__
     wrapper_attributes: Set[str] = set(dir(wrapper_class))
 
     for name, member in vars(native_estimator).items():
 
-        if member is None or name.startswith("_") or name in wrapper_attributes:
+        if member is None or name in wrapper_attributes:
             continue
 
         alias = _make_alias(
             wrapper_module=wrapper_module,
             wrapper_name=wrapper_name,
             name=name,
             delegate_cls=native_estimator,
```

### Comparing `sklearndf-2.2rc0/src/sklearndf/wrapper/numpy/_numpy.py` & `sklearndf-2.2rc1/src/sklearndf/wrapper/numpy/_numpy.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/src/sklearndf/wrapper/stacking/_stacking.py` & `sklearndf-2.2rc1/src/sklearndf/wrapper/stacking/_stacking.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/conftest.py` & `sklearndf-2.2rc1/test/test/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # noinspection PyPackageRequirements
 import pytest
 import sklearn
 from sklearn import datasets
 from sklearn.utils import Bunch
 
+from sklearndf import __sklearn_1_1__, __sklearn_version__
 from sklearndf.transformation import OneHotEncoderDF
 
 logging.basicConfig(level=logging.DEBUG)
 log = logging.getLogger(__name__)
 
 # todo: Keep this up to date, consider implementing manifold/neighbors
 UNSUPPORTED_SKLEARN_PACKAGES = [sklearn.manifold, sklearn.neighbors]
@@ -32,20 +33,25 @@
 def n_jobs() -> int:
     return -3
 
 
 @pytest.fixture  # type: ignore
 def diabetes_df(diabetes_target: str) -> pd.DataFrame:
     #  load sklearn test-data and convert to pd
-    diabetes: Bunch = datasets.load_diabetes()
+    diabetes: Bunch
+    if __sklearn_version__ >= __sklearn_1_1__:
+        diabetes = datasets.load_diabetes(scaled=False)
+    else:
+        # arg scaled does not exist in scikit-learn < 1.1
+        diabetes = datasets.load_diabetes()
 
     return pd.DataFrame(
         data=np.c_[diabetes.data, diabetes.target],
         columns=[*map(str, diabetes.feature_names), diabetes_target],
-    )
+    ).astype(dtype={"sex": "category"})
 
 
 @pytest.fixture  # type: ignore
 def diabetes_features(diabetes_df: pd.DataFrame, diabetes_target: str) -> pd.DataFrame:
     return diabetes_df.drop(labels=[diabetes_target], axis=1)
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/__init__.py` & `sklearndf-2.2rc1/test/test/sklearndf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 
 import pandas as pd
 import sklearn
 from sklearn.base import BaseEstimator
 from sklearn.compose import ColumnTransformer
 from sklearn.pipeline import FeatureUnion
 
-from sklearndf import (
-    EstimatorDF,
-    LearnerDF,
-    TransformerDF,
-    __sklearn_0_22__,
-    __sklearn_version__,
-)
+from sklearndf import EstimatorDF, LearnerDF, TransformerDF, __sklearn_version__
 from sklearndf.pipeline.wrapper import FeatureUnionSparseFrames
 from sklearndf.transformation.wrapper import ColumnTransformerSparseFrames
 from sklearndf.wrapper import EstimatorWrapperDF
 
 OVERRIDDEN_SKLEARN_CLASSES = {
     ColumnTransformerSparseFrames: ColumnTransformer,
     FeatureUnionSparseFrames: FeatureUnion,
@@ -102,17 +96,15 @@
     except KeyError as cause:
         raise ValueError(
             f"There is no class that wraps '{to_wrap}' in {from_module}"
         ) from cause
 
 
 def check_expected_not_fitted_error(estimator: EstimatorDF) -> None:
-    """Check if transformers & learners raise NotFittedError (since sklearn 0.22)"""
-    if __sklearn_version__ < __sklearn_0_22__:
-        return
+    """Check if transformers & learners raise NotFittedError"""
 
     test_x = pd.DataFrame(data=list(range(10)))
 
     def check_sklearndf_call(
         func_to_call: str, _estimator: Union[LearnerDF, TransformerDF]
     ) -> None:
         try:
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/pipeline/__init__.py` & `sklearndf-2.2rc1/test/test/sklearndf/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_classification_pipeline_df.py` & `sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_classification_pipeline_df.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_clustering_pipeline.py` & `sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_clustering_pipeline.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_pipeline_df.py` & `sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_pipeline_df.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/pipeline/test_regression_pipeline_df.py` & `sklearndf-2.2rc1/test/test/sklearndf/pipeline/test_regression_pipeline_df.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_base.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_base.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_classification.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pytest
 from sklearn.base import is_classifier
 from sklearn.multioutput import ClassifierChain, MultiOutputClassifier
 
 import sklearndf.classification as classification
 from sklearndf import (
     ClassifierDF,
-    __sklearn_0_22__,
     __sklearn_1_0__,
     __sklearn_1_2__,
     __sklearn_version__,
 )
 from test.sklearndf import check_expected_not_fitted_error, iterate_classes
 
 CLASSIFIERS_TO_TEST = iterate_classes(
@@ -24,17 +23,15 @@
 )
 
 
 def test_classifier_count() -> None:
     n = len(CLASSIFIERS_TO_TEST)
 
     print(f"Testing {n} classifiers.")
-    if __sklearn_version__ < __sklearn_0_22__:
-        assert n == 38
-    elif __sklearn_version__ < __sklearn_1_0__:
+    if __sklearn_version__ < __sklearn_1_0__:
         assert n == 40
     else:
         assert n == 41
 
 
 if __sklearn_version__ < __sklearn_1_2__:
     BASE_ESTIMATOR = "base_estimator"
@@ -74,17 +71,16 @@
     classification.MultinomialNBDF,
     classification.PerceptronDF,
     classification.SGDClassifierDF,
     classification.PassiveAggressiveClassifierDF,
     classification.GaussianNBDF,
     classification.ComplementNBDF,
     classification.MultiOutputClassifierDF,
+    classification.CategoricalNBDF,
 ]
-if __sklearn_version__ >= __sklearn_0_22__:
-    CLASSIFIERS_PARTIAL_FIT.append(classification.CategoricalNBDF)
 
 
 @pytest.mark.parametrize(  # type: ignore
     argnames="sklearndf_cls", argvalues=CLASSIFIERS_TO_TEST
 )
 def test_wrapped_fit_predict(
     sklearndf_cls: Type[ClassifierDF],
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_clustering.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_clustering.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_meta_estimators.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_meta_estimators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 import pandas as pd
 import pytest
 from sklearn.base import is_classifier, is_regressor
 from sklearn.impute import SimpleImputer
 
-from sklearndf import __sklearn_0_22__, __sklearn_version__
 from sklearndf.classification import (
     ClassifierChainDF,
     LogisticRegressionCVDF,
     LogisticRegressionDF,
     RandomForestClassifierDF,
     VotingClassifierDF,
 )
@@ -23,60 +22,77 @@
 )
 from sklearndf.transformation import ColumnTransformerDF, StandardScalerDF
 
 log = logging.getLogger(__name__)
 
 
 def test_meta_estimators() -> None:
-    VotingClassifierDF(estimators=[("rf", RandomForestClassifierDF())])
+    with pytest.warns(
+        expected_warning=UserWarning,
+        match=(
+            "^the following attributes of VotingClassifierDF have been replaced with "
+            "their native scikit-learn counterparts: estimators$"
+        ),
+    ):
+        VotingClassifierDF(estimators=[("rf", RandomForestClassifierDF())])
 
     with pytest.raises(
         TypeError,
         match=(
             "sklearndf meta-estimators only accept simple regressors and classifiers, "
             "but got: ClassifierPipelineDF"
         ),
     ):
         VotingClassifierDF(
             estimators=[
                 ("rf", ClassifierPipelineDF(classifier=RandomForestClassifierDF()))
             ]
         )
 
-    regressor = MultiOutputRegressorDF(estimator=RandomForestRegressorDF())
+    with pytest.warns(
+        expected_warning=UserWarning,
+        match=(
+            "^the following attributes of MultiOutputRegressorDF have been replaced "
+            "with their native scikit-learn counterparts: estimator$"
+        ),
+    ):
+        regressor = MultiOutputRegressorDF(estimator=RandomForestRegressorDF())
     assert is_regressor(regressor)
 
     with pytest.raises(
         TypeError,
         match=(
             "sklearndf meta-estimators only accept simple regressors and classifiers, "
             "but got: RegressorPipelineDF"
         ),
     ):
         MultiOutputRegressorDF(
             estimator=RegressorPipelineDF(regressor=RandomForestRegressorDF())
         )
 
-    classifier = ClassifierChainDF(base_estimator=RandomForestClassifierDF())
+    with pytest.warns(
+        expected_warning=UserWarning,
+        match=(
+            "^the following attributes of ClassifierChainDF have been replaced "
+            "with their native scikit-learn counterparts: base_estimator$"
+        ),
+    ):
+        classifier = ClassifierChainDF(base_estimator=RandomForestClassifierDF())
     assert is_classifier(classifier)
 
     with pytest.raises(
         TypeError,
         match=(
             "sklearndf meta-estimators only accept simple regressors and classifiers, "
             "but got: SimpleImputer"
         ),
     ):
         ClassifierChainDF(base_estimator=SimpleImputer())
 
 
-@pytest.mark.skipif(  # type: ignore
-    condition=__sklearn_version__ < __sklearn_0_22__,
-    reason="stacking estimators are not implemented by current version of sklearn",
-)
 def test_stacking_regressor(
     diabetes_features: pd.DataFrame, diabetes_target_sr: pd.Series
 ) -> None:
     from sklearndf.regression import StackingRegressorDF
 
     # basic building blocks
     model1 = LinearRegressionDF()
@@ -138,18 +154,14 @@
     final_estimator_fitted = stack_of_pipelines.final_estimator_
     assert final_estimator_fitted.feature_names_in_.to_list() == [
         "pipeline1",
         "pipeline2",
     ]
 
 
-@pytest.mark.skipif(  # type: ignore
-    condition=__sklearn_version__ < __sklearn_0_22__,
-    reason="stacking estimators are not implemented by current version of sklearn",
-)
 def test_stacking_classifier(
     iris_features: pd.DataFrame, iris_target_sr: pd.Series
 ) -> None:
     from sklearndf.classification import StackingClassifierDF
 
     # basic building blocks
     model1 = LogisticRegressionCVDF()
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_regression.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,15 @@
 
 import pandas as pd
 import pytest
 from sklearn.base import BaseEstimator, is_regressor
 from sklearn.multioutput import MultiOutputRegressor, RegressorChain
 
 import sklearndf.regression
-from sklearndf import (
-    RegressorDF,
-    TransformerDF,
-    __sklearn_0_22__,
-    __sklearn_0_23__,
-    __sklearn_1_0__,
-    __sklearn_version__,
-)
+from sklearndf import RegressorDF, TransformerDF, __sklearn_1_0__, __sklearn_version__
 from sklearndf.regression import (
     SVRDF,
     IsotonicRegressionDF,
     LinearRegressionDF,
     MLPRegressorDF,
     MultiOutputRegressorDF,
     PassiveAggressiveRegressorDF,
@@ -36,19 +29,15 @@
 )
 
 
 def test_regressor_count() -> None:
     n = len(REGRESSORS_TO_TEST)
 
     print(f"Testing {n} regressors.")
-    if __sklearn_version__ < __sklearn_0_22__:
-        assert n == 49
-    elif __sklearn_version__ < __sklearn_0_23__:
-        assert n == 50
-    elif __sklearn_version__ < __sklearn_1_0__:
+    if __sklearn_version__ < __sklearn_1_0__:
         assert n == 53
     else:
         assert n == 55
 
 
 DEFAULT_REGRESSOR_PARAMETERS: Dict[str, Dict[str, Any]] = {
     "MultiOutputRegressorDF": dict(estimator=RandomForestRegressorDF()),
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/test_sklearn_coverage.py` & `sklearndf-2.2rc1/test/test/sklearndf/test_sklearn_coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import sklearndf.classification
 import sklearndf.clustering
 import sklearndf.pipeline
 import sklearndf.regression
 import sklearndf.transformation
 from ..conftest import UNSUPPORTED_SKLEARN_PACKAGES
-from ..sklearndf import find_all_submodules, iterate_classes, sklearn_delegate_classes
-from sklearndf import EstimatorDF, __sklearn_0_23__, __sklearn_version__
+from . import find_all_submodules, iterate_classes, sklearn_delegate_classes
+from sklearndf import EstimatorDF
 
 T = TypeVar("T")
 
 
 GENERAL_COVERAGE_EXCLUSIONS = {
     # exclude all private classes:
     r"^_",
@@ -35,19 +35,17 @@
     r".*Mixin$",
 }
 
 CLASSIFIER_COVERAGE_EXCLUSIONS = {
     *GENERAL_COVERAGE_EXCLUSIONS,
     # Base classes and Mixins not following the convention
     "ForestClassifier",
+    "_IdentityClassifier",
 }
 
-if __sklearn_version__ >= __sklearn_0_23__:
-    added_in_v023 = ("_IdentityClassifier",)
-    CLASSIFIER_COVERAGE_EXCLUSIONS.update(added_in_v023)
 
 REGRESSOR_COVERAGE_EXCLUSIONS = {
     *GENERAL_COVERAGE_EXCLUSIONS,
     # Base classes and mix-ins
     "ForestRegressor",
     "GeneralizedLinearRegressor",
     # Private classes
```

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/transformation/test_imputers.py` & `sklearndf-2.2rc1/test/test/sklearndf/transformation/test_imputers.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/transformation/test_sparse.py` & `sklearndf-2.2rc1/test/test/sklearndf/transformation/test_sparse.py`

 * *Files identical despite different names*

### Comparing `sklearndf-2.2rc0/test/test/sklearndf/transformation/test_transformation.py` & `sklearndf-2.2rc1/test/test/sklearndf/transformation/test_transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, List, Type, cast
 
 import numpy as np
 import pandas as pd
 import pytest
 import sklearn
 from numpy.testing import assert_array_equal
+from pandas.arrays import SparseArray
 from pandas.testing import assert_frame_equal
 from sklearn.base import BaseEstimator, TransformerMixin, is_classifier, is_regressor
 from sklearn.compose import ColumnTransformer
 from sklearn.impute import SimpleImputer
 from sklearn.preprocessing import Normalizer, StandardScaler
 
 import sklearndf.transformation
@@ -17,16 +18,14 @@
     get_sklearndf_wrapper_class,
     iterate_classes,
 )
 from sklearndf import (
     ClassifierDF,
     RegressorDF,
     TransformerDF,
-    __sklearn_0_22__,
-    __sklearn_0_23__,
     __sklearn_0_24__,
     __sklearn_1_0__,
     __sklearn_1_1__,
     __sklearn_version__,
 )
 from sklearndf.classification import RandomForestClassifierDF
 from sklearndf.clustering import FeatureAgglomerationDF
@@ -70,17 +69,15 @@
 TRANSFORMERS_TO_TEST.append(FeatureAgglomerationDF)
 
 
 def test_transformer_count() -> None:
     n = len(TRANSFORMERS_TO_TEST)
 
     print(f"Testing {n} transformers.")
-    if __sklearn_version__ < __sklearn_0_22__:
-        assert n == 55
-    elif __sklearn_version__ < __sklearn_0_24__:
+    if __sklearn_version__ < __sklearn_0_24__:
         assert n == 56
     elif __sklearn_version__ < __sklearn_1_0__:
         assert n == 57
     elif __sklearn_version__ < __sklearn_1_1__:
         assert n == 58
     else:
         assert n == 60
@@ -427,15 +424,15 @@
 
 
 @pytest.mark.parametrize(argnames="sparse", argvalues=[True, False])  # type: ignore
 def test_one_hot_encoding(test_data_categorical: pd.DataFrame, sparse: bool) -> None:
     def _make_frame(data: Dict[str, List[float]]) -> pd.DataFrame:
         if sparse:
             df = pd.DataFrame(
-                data={k: pd.SparseArray(v, fill_value=0) for k, v in data.items()}
+                data={k: SparseArray(v, fill_value=0) for k, v in data.items()}
             )
         else:
             df = pd.DataFrame(data=data)
         return df.rename_axis(columns="feature")
 
     assert_frame_equal(
         OneHotEncoderDF(drop=None, sparse=sparse).fit_transform(test_data_categorical),
@@ -479,31 +476,30 @@
                 "b_green": [0.0, 0.0, 1.0],
                 "c_child": [1.0, 0.0, 0.0],
                 "c_father": [0.0, 1.0, 0.0],
             }
         ),
     )
 
-    if __sklearn_version__ >= __sklearn_0_23__:
-        assert_frame_equal(
-            OneHotEncoderDF(drop="if_binary", sparse=sparse).fit_transform(
-                test_data_categorical
-            ),
-            _make_frame(
-                {
-                    "a_yes": [1.0, 1.0, 0.0],
-                    "b_blue": [0.0, 1.0, 0.0],
-                    "b_green": [0.0, 0.0, 1.0],
-                    "b_red": [1.0, 0.0, 0.0],
-                    "c_child": [1.0, 0.0, 0.0],
-                    "c_father": [0.0, 1.0, 0.0],
-                    "c_mother": [0.0, 0.0, 1.0],
-                }
-            ),
-        )
+    assert_frame_equal(
+        OneHotEncoderDF(drop="if_binary", sparse=sparse).fit_transform(
+            test_data_categorical
+        ),
+        _make_frame(
+            {
+                "a_yes": [1.0, 1.0, 0.0],
+                "b_blue": [0.0, 1.0, 0.0],
+                "b_green": [0.0, 0.0, 1.0],
+                "b_red": [1.0, 0.0, 0.0],
+                "c_child": [1.0, 0.0, 0.0],
+                "c_father": [0.0, 1.0, 0.0],
+                "c_mother": [0.0, 0.0, 1.0],
+            }
+        ),
+    )
 
     if __sklearn_version__ >= __sklearn_1_1__:
 
         assert_frame_equal(
             OneHotEncoderDF(min_frequency=2, sparse=sparse).fit_transform(
                 test_data_categorical
             ),
```

### Comparing `sklearndf-2.2rc0/test/test/test_docs.py` & `sklearndf-2.2rc1/test/test/test_docs.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,20 @@
                     # generated classes, except in the '.extra' subpackages
                     r"(?:classification|clustering|regression|transformation)"
                     r"\.(?!extra\.).*",
                     # LGBM estimators in the '.extra' packages
                     r"(?:classification|regression)\.extra\.LGBM.*",
                     # XGBoost estimators in the '.extra' packages
                     r"(?:classification|regression)\.extra\.XGB.*",
-                    # BorutaDF
+                    # BorutaPy package
                     r"transformation\.extra\.BorutaDF",
+                    # ARFS package
+                    r"transformation\.extra\.BoostAGrootaDF",
+                    r"transformation\.extra\.GrootCVDF",
+                    r"transformation\.extra\.LeshyDF",
                     # scikit-learn pipeline classes
                     r"pipeline\.(PipelineDF|FeatureUnionDF).*",
                     # sparse frames version of FeatureUnion
                     r"pipeline\.wrapper\.FeatureUnion\.",
                 )
             )
             + ")"
```

### Comparing `sklearndf-2.2rc0/tox.ini` & `sklearndf-2.2rc1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -30,24 +30,27 @@
     # print all installed packages to stdout
     python -m pip freeze
     # run the tests
     pytest test/ -s
 
 [testenv:{py3,py37,py38,py39}-custom-deps]
 deps =
-    boruta{env:FACET_V_BORUTA}
+    # install custom dependencies
     gamma-pytools{env:FACET_V_GAMMA_PYTOOLS}
     joblib{env:FACET_V_JOBLIB}
-    lightgbm{env:FACET_V_LIGHTGBM}
     matplotlib{env:FACET_V_MATPLOTLIB}
     numpy{env:FACET_V_NUMPY}
     pandas{env:FACET_V_PANDAS}
     scikit-learn{env:FACET_V_SCIKIT_LEARN}
     scipy{env:FACET_V_SCIPY}
     typing_inspect{env:FACET_V_TYPING_INSPECT}
+    # optional dependencies, for testing only
+    arfs{env:FACET_V_ARFS}
+    boruta{env:FACET_V_BORUTA}
+    lightgbm{env:FACET_V_LIGHTGBM}
     xgboost{env:FACET_V_XGBOOST}
 
 [flake8]
 
 max-line-length = 88
 
 show-source = true
```

### Comparing `sklearndf-2.2rc0/PKG-INFO` & `sklearndf-2.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearndf
-Version: 2.2rc0
+Version: 2.2rc1
 Summary: Data frame support and feature traceability for `scikit-learn`.
 Home-page: https://github.com/BCG-Gamma/sklearndf
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,34 +16,33 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: gamma-pytools  ~=2.1rc
+Requires-Dist: gamma-pytools  >=2.1rc2,<3a
 Requires-Dist: numpy          >=1.21,<1.24a
 Requires-Dist: packaging      >=20
-Requires-Dist: pandas         >=1.0,<2a
+Requires-Dist: pandas         >=1
 Requires-Dist: scikit-learn   >=0.24,<1.3a
 Requires-Dist: scipy          ~=1.4
 Requires-Dist: sphinx ~= 4.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ~= 1.19 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme ~= 0.8.1 ; extra == "docs"
 Requires-Dist: jinja2 ~= 2.11 ; extra == "docs"
 Requires-Dist: nbsphinx ~= 0.8.9 ; extra == "docs"
 Requires-Dist: jupyter == 1 ; extra == "docs"
 Requires-Dist: docutils ~= 0.17 ; extra == "docs"
 Requires-Dist: xlrd ~= 1.2 ; extra == "docs"
 Requires-Dist: m2r ~= 0.2 ; extra == "docs"
-Requires-Dist: boruta ~=0.3 ; extra == "testing"
-Requires-Dist: lightgbm ~= 3.3 ; extra == "testing"
 Requires-Dist: pytest ~= 7.1 ; extra == "testing"
-Requires-Dist: pytest-cov ~= 2.8 ; extra == "testing"
-Requires-Dist: xgboost ~= 1.5 ; extra == "testing"
+Requires-Dist: pytest-cov ~= 2.12 ; extra == "testing"
+Requires-Dist: lightgbm ~= 3.0 ; extra == "testing"
+Requires-Dist: xgboost ~= 1.0 ; extra == "testing"
 Project-URL: Documentation, https://bcg-gamma.github.io/sklearndf/
 Project-URL: Repository, https://github.com/BCG-Gamma/sklearndf
 Provides-Extra: docs
 Provides-Extra: testing
 
 *sklearndf* is an open source library designed to address a common need with
 `scikit-learn <https://github.com/scikit-learn/scikit-learn>`__: the outputs of
```

