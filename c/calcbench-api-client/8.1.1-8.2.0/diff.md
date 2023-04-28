# Comparing `tmp/calcbench_api_client-8.1.1.tar.gz` & `tmp/calcbench_api_client-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calcbench_api_client-8.1.1.tar", last modified: Thu Jan 26 15:32:49 2023, max compression
+gzip compressed data, was "dist\calcbench_api_client-8.2.0.tar", last modified: Fri Apr 28 12:58:01 2023, max compression
```

## Comparing `calcbench_api_client-8.1.1.tar` & `calcbench_api_client-8.2.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.222135 calcbench_api_client-8.1.1/
--rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-8.1.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.018133 calcbench_api_client-8.1.1/.vscode/
--rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-8.1.1/.vscode/launch.json
--rw-rw-rw-   0        0        0     1989 2023-01-26 15:32:49.221135 calcbench_api_client-8.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      985 2022-08-18 20:47:28.000000 calcbench_api_client-8.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.047134 calcbench_api_client-8.1.1/calcbench/
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.049135 calcbench_api_client-8.1.1/calcbench/.vscode/
--rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/calcbench/.vscode/launch.json
--rw-rw-rw-   0        0        0     1810 2023-01-26 15:30:12.000000 calcbench_api_client-8.1.1/calcbench/__init__.py
--rw-rw-rw-   0        0        0    11884 2022-11-07 16:43:08.000000 calcbench_api_client-8.1.1/calcbench/api_client.py
--rw-rw-rw-   0        0        0     2279 2023-01-24 18:56:25.000000 calcbench_api_client-8.1.1/calcbench/api_query_params.py
--rw-rw-rw-   0        0        0    15620 2021-11-18 16:53:55.000000 calcbench_api_client-8.1.1/calcbench/business_combinations.py
--rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-8.1.1/calcbench/companies.py
--rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-8.1.1/calcbench/dimensional.py
--rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-8.1.1/calcbench/disclosures.py
--rw-rw-rw-   0        0        0     5224 2023-01-26 15:27:57.000000 calcbench_api_client-8.1.1/calcbench/downloaders.py
--rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-8.1.1/calcbench/face_statements.py
--rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-8.1.1/calcbench/filing.py
--rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-8.1.1/calcbench/listener.py
--rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-8.1.1/calcbench/metrics.py
--rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-8.1.1/calcbench/press_release.py
--rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-8.1.1/calcbench/raw_numeric_XBRL.py
--rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-8.1.1/calcbench/raw_numeric_non_XBRL.py
--rw-rw-rw-   0        0        0    18896 2023-01-24 18:54:52.000000 calcbench_api_client-8.1.1/calcbench/standardized_numeric.py
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.071135 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/
--rw-rw-rw-   0        0        0     1989 2023-01-26 15:32:48.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2023-01-26 15:32:48.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 15:32:48.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dependency_links.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.075133 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dist/
--rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
--rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
--rw-rw-rw-   0        0        0      270 2023-01-26 15:32:48.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-26 15:32:48.000000 calcbench_api_client-8.1.1/calcbench_api_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.077134 calcbench_api_client-8.1.1/conda-recipe/
--rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-8.1.1/conda-recipe/meta.yaml
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.084133 calcbench_api_client-8.1.1/docs/
--rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/.nojekyll
--rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.144133 calcbench_api_client-8.1.1/docs/html/
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.146138 calcbench_api_client-8.1.1/docs/html/_sources/
--rw-rw-rw-   0        0        0     1248 2022-11-02 16:00:32.000000 calcbench_api_client-8.1.1/docs/html/_sources/getting-started.rst.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.192133 calcbench_api_client-8.1.1/docs/html/_static/
--rw-rw-rw-   0        0        0    11885 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/_static/alabaster.css
--rw-rw-rw-   0        0        0    15541 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/_static/basic.css
--rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-8.1.1/docs/html/_static/custom.css
--rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-8.1.1/docs/html/_static/doctools.js
--rw-rw-rw-   0        0        0      361 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/html/_static/file.png
--rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/html/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-8.1.1/docs/html/_static/jquery-3.4.1.js
--rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-8.1.1/docs/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-8.1.1/docs/html/_static/jquery.js
--rw-rw-rw-   0        0        0    11151 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/html/_static/plus.png
--rw-rw-rw-   0        0        0     4874 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/_static/pygments.css
--rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-8.1.1/docs/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-8.1.1/docs/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-8.1.1/docs/html/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-8.1.1/docs/html/_static/underscore.js
--rw-rw-rw-   0        0        0    20664 2023-01-26 15:02:05.000000 calcbench_api_client-8.1.1/docs/html/business-combinations.html
--rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-8.1.1/docs/html/companies.html
--rw-rw-rw-   0        0        0   116341 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/dimensional.html
--rw-rw-rw-   0        0        0    65621 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/disclosures.html
--rw-rw-rw-   0        0        0    18893 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/downloaders.html
--rw-rw-rw-   0        0        0    35986 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/face-statements.html
--rw-rw-rw-   0        0        0    46164 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/filings.html
--rw-rw-rw-   0        0        0   107809 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/genindex.html
--rw-rw-rw-   0        0        0    14084 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/getting-started.html
--rw-rw-rw-   0        0        0     7429 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/index.html
--rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-8.1.1/docs/html/metrics.html
--rw-rw-rw-   0        0        0    37067 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/numeric-data.html
--rw-rw-rw-   0        0        0    20870 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/press-release.html
--rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-8.1.1/docs/html/push-notification.html
--rw-rw-rw-   0        0        0     7083 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/py-modindex.html
--rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-8.1.1/docs/html/raw-numeric-XBRL.html
--rw-rw-rw-   0        0        0    36953 2023-01-26 15:02:06.000000 calcbench_api_client-8.1.1/docs/html/raw-numeric-non-XBRL.html
--rw-rw-rw-   0        0        0     4370 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/search.html
--rw-rw-rw-   0        0        0    47355 2023-01-26 15:28:10.000000 calcbench_api_client-8.1.1/docs/html/searchindex.js
--rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/index.html
--rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-8.1.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-01-26 15:32:49.220135 calcbench_api_client-8.1.1/docs/source/
--rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-8.1.1/docs/source/business-combinations.rst
--rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-8.1.1/docs/source/companies.rst
--rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-8.1.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-8.1.1/docs/source/dimensional.rst
--rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-8.1.1/docs/source/disclosures.rst
--rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-8.1.1/docs/source/downloaders.rst
--rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-8.1.1/docs/source/face-statements.rst
--rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-8.1.1/docs/source/filings.rst
--rw-rw-rw-   0        0        0     1248 2022-08-31 17:06:59.000000 calcbench_api_client-8.1.1/docs/source/getting-started.rst
--rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-8.1.1/docs/source/index.rst
--rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-8.1.1/docs/source/metrics.rst
--rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-8.1.1/docs/source/numeric-data.rst
--rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-8.1.1/docs/source/press-release.rst
--rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-8.1.1/docs/source/push-notification.rst
--rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-8.1.1/docs/source/raw-numeric-XBRL.rst
--rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-8.1.1/docs/source/raw-numeric-non-XBRL.rst
--rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-8.1.1/publish.PS1
--rw-rw-rw-   0        0        0       42 2023-01-26 15:32:49.222135 calcbench_api_client-8.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-8.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.503794 calcbench_api_client-8.2.0/
+-rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-8.2.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.493781 calcbench_api_client-8.2.0/.vscode/
+-rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-8.2.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1989 2023-04-28 12:58:01.500783 calcbench_api_client-8.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2022-08-18 20:47:28.000000 calcbench_api_client-8.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.528788 calcbench_api_client-8.2.0/calcbench/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.542789 calcbench_api_client-8.2.0/calcbench/.vscode/
+-rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/calcbench/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1810 2023-04-28 12:57:50.000000 calcbench_api_client-8.2.0/calcbench/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-8.2.0/calcbench/api_client.py
+-rw-rw-rw-   0        0        0     2279 2023-01-24 18:56:25.000000 calcbench_api_client-8.2.0/calcbench/api_query_params.py
+-rw-rw-rw-   0        0        0    15620 2021-11-18 16:53:55.000000 calcbench_api_client-8.2.0/calcbench/business_combinations.py
+-rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-8.2.0/calcbench/companies.py
+-rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-8.2.0/calcbench/dimensional.py
+-rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-8.2.0/calcbench/disclosures.py
+-rw-rw-rw-   0        0        0     5478 2023-03-22 16:00:49.000000 calcbench_api_client-8.2.0/calcbench/downloaders.py
+-rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-8.2.0/calcbench/face_statements.py
+-rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-8.2.0/calcbench/filing.py
+-rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-8.2.0/calcbench/listener.py
+-rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-8.2.0/calcbench/metrics.py
+-rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-8.2.0/calcbench/press_release.py
+-rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-8.2.0/calcbench/raw_numeric_XBRL.py
+-rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-8.2.0/calcbench/raw_numeric_non_XBRL.py
+-rw-rw-rw-   0        0        0    18769 2023-04-28 12:56:36.000000 calcbench_api_client-8.2.0/calcbench/standardized_numeric.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.579780 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/
+-rw-rw-rw-   0        0        0     1989 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.600779 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/
+-rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
+-rw-rw-rw-   0        0        0      270 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.611782 calcbench_api_client-8.2.0/conda-recipe/
+-rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-8.2.0/conda-recipe/meta.yaml
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.632779 calcbench_api_client-8.2.0/docs/
+-rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/.nojekyll
+-rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.878780 calcbench_api_client-8.2.0/docs/html/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.889785 calcbench_api_client-8.2.0/docs/html/_sources/
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-8.2.0/docs/html/_sources/getting-started.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.373804 calcbench_api_client-8.2.0/docs/html/_static/
+-rw-rw-rw-   0        0        0    11885 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15541 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/basic.css
+-rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-8.2.0/docs/html/_static/custom.css
+-rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-8.2.0/docs/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      361 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/file.png
+-rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.4.1.js
+-rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery.js
+-rw-rw-rw-   0        0        0    11151 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4874 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    20664 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/business-combinations.html
+-rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-8.2.0/docs/html/companies.html
+-rw-rw-rw-   0        0        0   116341 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/dimensional.html
+-rw-rw-rw-   0        0        0    65621 2023-04-12 21:26:04.000000 calcbench_api_client-8.2.0/docs/html/disclosures.html
+-rw-rw-rw-   0        0        0    18893 2023-04-12 21:26:04.000000 calcbench_api_client-8.2.0/docs/html/downloaders.html
+-rw-rw-rw-   0        0        0    35986 2023-01-26 15:02:06.000000 calcbench_api_client-8.2.0/docs/html/face-statements.html
+-rw-rw-rw-   0        0        0    46164 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/filings.html
+-rw-rw-rw-   0        0        0   107809 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/genindex.html
+-rw-rw-rw-   0        0        0    14252 2023-04-12 21:26:05.000000 calcbench_api_client-8.2.0/docs/html/getting-started.html
+-rw-rw-rw-   0        0        0     7429 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/index.html
+-rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-8.2.0/docs/html/metrics.html
+-rw-rw-rw-   0        0        0    37691 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/numeric-data.html
+-rw-rw-rw-   0        0        0    20870 2023-04-12 21:26:05.000000 calcbench_api_client-8.2.0/docs/html/press-release.html
+-rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-8.2.0/docs/html/push-notification.html
+-rw-rw-rw-   0        0        0     7083 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/py-modindex.html
+-rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-8.2.0/docs/html/raw-numeric-XBRL.html
+-rw-rw-rw-   0        0        0    36953 2023-01-26 15:02:06.000000 calcbench_api_client-8.2.0/docs/html/raw-numeric-non-XBRL.html
+-rw-rw-rw-   0        0        0     4370 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/search.html
+-rw-rw-rw-   0        0        0    47468 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/searchindex.js
+-rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/index.html
+-rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.498784 calcbench_api_client-8.2.0/docs/source/
+-rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-8.2.0/docs/source/business-combinations.rst
+-rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-8.2.0/docs/source/companies.rst
+-rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-8.2.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-8.2.0/docs/source/dimensional.rst
+-rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-8.2.0/docs/source/disclosures.rst
+-rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-8.2.0/docs/source/downloaders.rst
+-rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-8.2.0/docs/source/face-statements.rst
+-rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-8.2.0/docs/source/filings.rst
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-8.2.0/docs/source/getting-started.rst
+-rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-8.2.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-8.2.0/docs/source/metrics.rst
+-rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-8.2.0/docs/source/numeric-data.rst
+-rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-8.2.0/docs/source/press-release.rst
+-rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-8.2.0/docs/source/push-notification.rst
+-rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-8.2.0/docs/source/raw-numeric-XBRL.rst
+-rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-8.2.0/docs/source/raw-numeric-non-XBRL.rst
+-rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-8.2.0/publish.PS1
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:58:01.504781 calcbench_api_client-8.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-8.2.0/setup.py
```

### Comparing `calcbench_api_client-8.1.1/PKG-INFO` & `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calcbench_api_client
-Version: 8.1.1
+Name: calcbench-api-client
+Version: 8.2.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -45,14 +45,14 @@
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Listener
-Provides-Extra: Keyring
+Provides-Extra: Backoff
 Provides-Extra: tqdm
 Provides-Extra: BeautifulSoup
-Provides-Extra: Pandas
+Provides-Extra: Keyring
 Provides-Extra: pyarrow
-Provides-Extra: Backoff
+Provides-Extra: Pandas
+Provides-Extra: Listener
```

### Comparing `calcbench_api_client-8.1.1/README.md` & `calcbench_api_client-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/__init__.py` & `calcbench_api_client-8.2.0/calcbench/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The "public" properties on the cb module
 
 """
-__version__ = "8.1.1"
+__version__ = "8.2.0"
 from datetime import datetime
 import logging
 from .api_client import (
     enable_backoff,
     html_diff,
     set_credentials,
     set_proxies,
```

### Comparing `calcbench_api_client-8.1.1/calcbench/api_client.py` & `calcbench_api_client-8.2.0/calcbench/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 else:
     try:
         from typing import TypedDict
     except ImportError:
         from typing_extensions import TypedDict
 
 from requests.sessions import Session
+from requests import HTTPError
 
 from calcbench.api_query_params import APIQueryParams
 
 
 import requests
 from requests import RequestException
 
@@ -286,15 +287,15 @@
     _SESSION_STUFF["calcbench_user_name"] = cb_username
     _SESSION_STUFF["calcbench_password"] = cb_password
     _calcbench_session()  # Make sure credentials work.
 
 
 def enable_backoff(
     backoff_on: bool = True,
-    giveup: Callable[[RequestException], bool] = lambda e: hasattr(e, "response")
+    giveup: Callable[[RequestException], bool] = lambda e: isinstance(e, HTTPError)
     and e.response.status_code == 404,
 ):
     """Re-try failed requests with exponential back-off
 
     Requires the backoff package. ``pip install backoff``
 
     If processes make many requests, failures are inevitable.  Call this to retry failed requests.
```

### Comparing `calcbench_api_client-8.1.1/calcbench/api_query_params.py` & `calcbench_api_client-8.2.0/calcbench/api_query_params.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/business_combinations.py` & `calcbench_api_client-8.2.0/calcbench/business_combinations.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/companies.py` & `calcbench_api_client-8.2.0/calcbench/companies.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/dimensional.py` & `calcbench_api_client-8.2.0/calcbench/dimensional.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/disclosures.py` & `calcbench_api_client-8.2.0/calcbench/disclosures.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/downloaders.py` & `calcbench_api_client-8.2.0/calcbench/downloaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Callable, List, Literal, Optional, Sequence, TypeVar, Union
 from pathlib import Path
 
+from requests import HTTPError
+
 
 import calcbench as cb
 import pandas as pd
 from tqdm.auto import tqdm
 
 
 cb.enable_backoff(
-    giveup=lambda e: hasattr(e, "response") and (e.response.status_code in [404, 500])
+    giveup=lambda e: isinstance(e, HTTPError) and (e.response.status_code in [404, 500])
 )
 
 T = TypeVar("T")
 
 
 def iterate_to_dataframe(
     arguments: Sequence[T],
@@ -142,17 +144,24 @@
     >>> msft_data = table.filter(expr).to_pandas()
 
     """
     import pyarrow as pa
     import pyarrow.parquet as pq
 
     for argument in tqdm(list(arguments)):
-        df = f(argument)
-        if df.empty:
-            continue
-        table = pa.Table.from_pandas(df)
-        pq.write_to_dataset(
-            table=table,
-            root_path=root_path,
-            partition_cols=partition_cols,
-            **{"allow_truncated_timestamps": True, "coerce_timestamps": "us"},
-        )
+        try:
+
+            df = f(argument)
+            if df.empty:
+                continue
+        except KeyboardInterrupt:
+            raise
+        except Exception as e:
+            tqdm.write(f"Exception getting {argument} {e}")
+        else:
+            table = pa.Table.from_pandas(df)
+            pq.write_to_dataset(
+                table=table,
+                root_path=root_path,
+                partition_cols=partition_cols,
+                **{"allow_truncated_timestamps": True, "coerce_timestamps": "us"},
+            )
```

### Comparing `calcbench_api_client-8.1.1/calcbench/face_statements.py` & `calcbench_api_client-8.2.0/calcbench/face_statements.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/filing.py` & `calcbench_api_client-8.2.0/calcbench/filing.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/listener.py` & `calcbench_api_client-8.2.0/calcbench/listener.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/metrics.py` & `calcbench_api_client-8.2.0/calcbench/metrics.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/press_release.py` & `calcbench_api_client-8.2.0/calcbench/press_release.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/raw_numeric_XBRL.py` & `calcbench_api_client-8.2.0/calcbench/raw_numeric_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/raw_numeric_non_XBRL.py` & `calcbench_api_client-8.2.0/calcbench/raw_numeric_non_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench/standardized_numeric.py` & `calcbench_api_client-8.2.0/calcbench/standardized_numeric.py`

 * *Files 6% similar despite different names*

```diff
@@ -284,14 +284,17 @@
     "calcbench_entity_id",
     "period_start",
     "period_end",
     "calendar_year",
     "calendar_period",
     "filing_accession_number",
     "trace_url",
+    "date_modified",
+    "date_XBRL_confirmed",
+    "original_value",
 ]
 
 
 def _build_data_frame(raw_data: Sequence[StandardizedPoint]) -> "pd.DataFrame":
     """
     The order of the columns should remain constant
     """
@@ -324,16 +327,16 @@
 
     Example https://github.com/calcbench/notebooks/blob/master/python_client_api_demo.ipynb
 
     :param company_identifiers: Tickers/CIK codes. eg. ['msft', 'goog', 'appl', '0000066740'].  If not specified get data for all companies.
     :param metrics: Standardized metrics.  Full list @ https://www.calcbench.com/home/standardizedmetrics eg. ['revenue', 'accountsreceivable'].  If not specified get all metrics.
     :param fiscal_year: Fiscal year for which to get data.  If not specified get all history.
     :param fiscal_period: Fiscal period for which to get data.  If not specified get all history.
-    :param start_date:  Restrict to records received on or after (inclusive) this date/datetime
-    :param end_date:  Restric to records received prior (exclusive) thie date/datetime
+    :param start_date:  Restrict to records modified on or after (inclusive) this date/datetime
+    :param end_date:  Restric to records modified prior (exclusive) thie date/datetime
     :param point_in_time: Include timestamps when data was published and revision chains.
     :param filing_id: Filing ID for which to get data.  Get all of the data reported in this filing.
     :param exclude_unconfirmed_preliminary: Exclude points from press-releases or 8-Ks that have not been "confirmed" in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.
     :param pit_V2: Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.
     :return: Dataframe
 
 
@@ -368,14 +371,18 @@
        0 indicates an original, unrevised value for this fact. 1, 2, 3... indicates subsequent revisions to the fact value.  https://knowledge.calcbench.com/hc/en-us/search?utf8=%E2%9C%93&query=revisions&commit=Search
     preliminary
         True indicates the number was parsed from non-XBRL 8-K or press release from the wire
     XBRL
         Indicates the number was parsed from XBRL.
 
         The case where preliminary and XBRL are both true indicates the number was first parsed from a non-XBRL document then "confirmed" in an XBRL document.
+    date_XBRL_confirmed
+        Time at which the point was confirmed by an point from an XBRL filing.
+        If the point originally came from an XBRL filing this will be the original write time.
+        If this is null, for points post April 2023, the point has not been confirmed.
     period_start
        First day of the fiscal period for this fact
     period_end
        Last day of the fiscal period for this fact
     calendar_year
        The calendar year for this fact.  https://knowledge.calcbench.com/hc/en-us/articles/223267767-What-are-Calendar-Years-and-Periods-What-is-TTM-
     calendar_period
@@ -386,32 +393,42 @@
        Internal Calcbench identifier for reporting company
     filing_type
        The document type this fact came from, 10-K|Q, S-1 etc...
     date_modified (PIT only)
         The datetime Calcbench wrote/modified this value.
 
         Post November 2022 if this differs from the date_reported the fact was modified by Calcbench subsequent to the filing first being processed.
+    fling_accession_number
+        Accession number as assigned by the SEC for the filing from which this value came.
+    trace_url
+        URL for a page showing the source document for this value.
     original_value (PIT only)
         The value that Calcbench extracted when it first processed the filing.
 
         Post November 2022, if this differs from the value Calcbench the fact was modified by Calcbench subsequent to the filing first being processed.
+    standardized_id
+        A unique identifier Calcbench assigns to each standardized value.
     date_downloaded
         The timestamp on your computer when you downloaded this data.
 
+
+
     Usage::
 
       >>> d = calcbench.standardized(company_identifiers=['msft'],
       >>>                                 point_in_time=True,)
       >>> )
       >>> # Put the data in a format amiable to arithmetic on columns
       >>> d = calcbench.standardized(company_identifiers=['msft', 'orcl'], metrics=['StockholdersEquity', 'NetIncome'])
       >>> d = d.unstack("metric")["value"]
       >>> return_on_equity = d['NetIncome'] / d['StockholdersEquity']
 
     """
+
+    company_identifiers = list(company_identifiers)
     if point_in_time and pit_V2 is None:
         pit_V2 = True
     data = standardized_raw(
         company_identifiers=company_identifiers,
         all_history=not fiscal_year,
         year=fiscal_year,
         period=fiscal_period,
@@ -438,15 +455,21 @@
 
     if "calendar_period" in data.columns:
         data.calendar_period = data.calendar_period.astype(period_number)
 
     if "calendar_period" in data.columns:
         data.calendar_period = data.calendar_period.astype(period_number)
 
-    for date_column in ["date_reported", "period_end", "period_start", "date_modified"]:
+    for date_column in [
+        "date_reported",
+        "period_end",
+        "period_start",
+        "date_modified",
+        "date_XBRL_confirmed",
+    ]:
         if date_column in data.columns:
             data[date_column] = pd.to_datetime(data[date_column], errors="coerce")
     for string_column in [
         "ticker",
         "metric",
         "CIK",
         "filing_type",
@@ -463,35 +486,7 @@
     ]
     if point_in_time:
         index_columns = index_columns + ["date_reported"]
         data["date_downloaded"] = datetime.now()
     data = data.set_index(index_columns)
     data = data.sort_index()
     return data
-
-
-def _build_quarter_period(
-    data_point: StandardizedPoint, use_fiscal_period: bool
-) -> "pd.Period":
-    try:
-        return pd.Period(  # type: ignore
-            year=data_point.pop(
-                "fiscal_year" if use_fiscal_period else "calendar_year"
-            ),
-            quarter=data_point.pop(
-                "fiscal_period" if use_fiscal_period else "calendar_period"
-            ),
-            freq="q",
-        )
-    except ValueError:
-        # DEI points (entity_name) etc, don't have periods.
-        return pd.Period()  # type: ignore
-
-
-def _build_annual_period(
-    data_point: StandardizedPoint, use_fiscal_period: bool
-) -> "pd.Period":
-    data_point.pop("fiscal_period" if use_fiscal_period else "calendar_period")
-    return pd.Period(  # type: ignore
-        year=data_point.pop("fiscal_year" if use_fiscal_period else "calendar_year"),
-        freq="a",
-    )
```

### Comparing `calcbench_api_client-8.1.1/calcbench_api_client.egg-info/PKG-INFO` & `calcbench_api_client-8.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calcbench-api-client
-Version: 8.1.1
+Name: calcbench_api_client
+Version: 8.2.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -45,14 +45,14 @@
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Listener
-Provides-Extra: Keyring
+Provides-Extra: Backoff
 Provides-Extra: tqdm
 Provides-Extra: BeautifulSoup
-Provides-Extra: Pandas
+Provides-Extra: Keyring
 Provides-Extra: pyarrow
-Provides-Extra: Backoff
+Provides-Extra: Pandas
+Provides-Extra: Listener
```

### Comparing `calcbench_api_client-8.1.1/calcbench_api_client.egg-info/SOURCES.txt` & `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl` & `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz` & `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/conda-recipe/meta.yaml` & `calcbench_api_client-8.2.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/Makefile` & `calcbench_api_client-8.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_sources/getting-started.rst.txt` & `calcbench_api_client-8.2.0/docs/html/_sources/getting-started.rst.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Getting Started
 ===============
 
 .. warning::
-     Calcbench data is not free and API access is not included in the standard Calcbench subscription.
+     Calcbench data is not free and API access is not included in the standard Calcbench subscription.  Talk to us@calcbench.com before you start coding.
 
 .. _install:
 
 Installing the Client
 ---------------------
```

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/alabaster.css` & `calcbench_api_client-8.2.0/docs/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/basic.css` & `calcbench_api_client-8.2.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/doctools.js` & `calcbench_api_client-8.2.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/jquery-3.2.1.js` & `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/jquery-3.4.1.js` & `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/jquery-3.5.1.js` & `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/jquery.js` & `calcbench_api_client-8.2.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/language_data.js` & `calcbench_api_client-8.2.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/pygments.css` & `calcbench_api_client-8.2.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/searchtools.js` & `calcbench_api_client-8.2.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/underscore-1.13.1.js` & `calcbench_api_client-8.2.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/underscore-1.3.1.js` & `calcbench_api_client-8.2.0/docs/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/_static/underscore.js` & `calcbench_api_client-8.2.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/business-combinations.html` & `calcbench_api_client-8.2.0/docs/html/business-combinations.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/companies.html` & `calcbench_api_client-8.2.0/docs/html/companies.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/dimensional.html` & `calcbench_api_client-8.2.0/docs/html/dimensional.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/disclosures.html` & `calcbench_api_client-8.2.0/docs/html/disclosures.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/downloaders.html` & `calcbench_api_client-8.2.0/docs/html/downloaders.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/face-statements.html` & `calcbench_api_client-8.2.0/docs/html/face-statements.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/filings.html` & `calcbench_api_client-8.2.0/docs/html/filings.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/genindex.html` & `calcbench_api_client-8.2.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/getting-started.html` & `calcbench_api_client-8.2.0/docs/html/getting-started.html`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
           <div class="body" role="main">
             
   <div class="section" id="getting-started">
 <h1>Getting Started<a class="headerlink" href="#getting-started" title="Permalink to this headline">¶</a></h1>
 <div class="admonition warning">
 <p class="admonition-title">Warning</p>
-<p>Calcbench data is not free and API access is not included in the standard Calcbench subscription.</p>
+<p>Calcbench data is not free and API access is not included in the standard Calcbench subscription.  Talk to <a class="reference external" href="mailto:us&#37;&#52;&#48;calcbench&#46;com">us<span>&#64;</span>calcbench<span>&#46;</span>com</a> before you start coding.</p>
 </div>
 <div class="section" id="installing-the-client">
 <span id="install"></span><h2>Installing the Client<a class="headerlink" href="#installing-the-client" title="Permalink to this headline">¶</a></h2>
 <p>Install the Calcbench client from pip:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ pip install calcbench-api-client
 </pre></div>
 </div>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 
 
 ****** Getting StartedÂ¶ ******
 Warning
 Calcbench data is not free and API access is not included in the standard
-Calcbench subscription.
+Calcbench subscription. Talk to us@calcbench.com before you start coding.
 ***** Installing the ClientÂ¶ *****
 Install the Calcbench client from pip:
 $ pip install calcbench-api-client
 ***** Obtain CredentialsÂ¶ *****
 The API uses the same credentials as calcbench.com. If you do not have
 Calcbench credentials you can sign up for free two-week trial @ https://
 www.calcbench.com/join.
```

### Comparing `calcbench_api_client-8.1.1/docs/html/index.html` & `calcbench_api_client-8.2.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/metrics.html` & `calcbench_api_client-8.2.0/docs/html/metrics.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/numeric-data.html` & `calcbench_api_client-8.2.0/docs/html/numeric-data.html`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – Tickers/CIK codes. eg. [‘msft’, ‘goog’, ‘appl’, ‘0000066740’].  If not specified get data for all companies.</p></li>
 <li><p><strong>metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>]) – Standardized metrics.  Full list &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a> eg. [‘revenue’, ‘accountsreceivable’].  If not specified get all metrics.</p></li>
 <li><p><strong>fiscal_year</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Fiscal year for which to get data.  If not specified get all history.</p></li>
 <li><p><strong>fiscal_period</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">Period</span></code>, <code class="xref py py-data docutils literal notranslate"><span class="pre">Literal</span></code>[0, 1, 2, 3, 4], <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Fiscal period for which to get data.  If not specified get all history.</p></li>
-<li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restrict to records received on or after (inclusive) this date/datetime</p></li>
-<li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restric to records received prior (exclusive) thie date/datetime</p></li>
+<li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restrict to records modified on or after (inclusive) this date/datetime</p></li>
+<li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restric to records modified prior (exclusive) thie date/datetime</p></li>
 <li><p><strong>point_in_time</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – Include timestamps when data was published and revision chains.</p></li>
 <li><p><strong>filing_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Filing ID for which to get data.  Get all of the data reported in this filing.</p></li>
 <li><p><strong>exclude_unconfirmed_preliminary</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Exclude points from press-releases or 8-Ks that have not been “confirmed” in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.</p></li>
 <li><p><strong>pit_V2</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns</dt>
@@ -86,14 +86,18 @@
 <dt>revision_number</dt><dd><p>0 indicates an original, unrevised value for this fact. 1, 2, 3… indicates subsequent revisions to the fact value.  <a class="reference external" href="https://knowledge.calcbench.com/hc/en-us/search?utf8=%E2%9C%93&amp;query=revisions&amp;commit=Search">https://knowledge.calcbench.com/hc/en-us/search?utf8=%E2%9C%93&amp;query=revisions&amp;commit=Search</a></p>
 </dd>
 <dt>preliminary</dt><dd><p>True indicates the number was parsed from non-XBRL 8-K or press release from the wire</p>
 </dd>
 <dt>XBRL</dt><dd><p>Indicates the number was parsed from XBRL.</p>
 <p>The case where preliminary and XBRL are both true indicates the number was first parsed from a non-XBRL document then “confirmed” in an XBRL document.</p>
 </dd>
+<dt>date_XBRL_confirmed</dt><dd><p>Time at which the point was confirmed by an point from an XBRL filing.
+If the point originally came from an XBRL filing this will be the original write time.
+If this is null, for points post April 2023, the point has not been confirmed.</p>
+</dd>
 <dt>period_start</dt><dd><p>First day of the fiscal period for this fact</p>
 </dd>
 <dt>period_end</dt><dd><p>Last day of the fiscal period for this fact</p>
 </dd>
 <dt>calendar_year</dt><dd><p>The calendar year for this fact.  <a class="reference external" href="https://knowledge.calcbench.com/hc/en-us/articles/223267767-What-are-Calendar-Years-and-Periods-What-is-TTM">https://knowledge.calcbench.com/hc/en-us/articles/223267767-What-are-Calendar-Years-and-Periods-What-is-TTM</a>-</p>
 </dd>
 <dt>calendar_period</dt><dd><p>The calendar period for this fact</p>
@@ -103,17 +107,23 @@
 <dt>calcbench_entity_id</dt><dd><p>Internal Calcbench identifier for reporting company</p>
 </dd>
 <dt>filing_type</dt><dd><p>The document type this fact came from, 10-K|Q, S-1 etc…</p>
 </dd>
 <dt>date_modified (PIT only)</dt><dd><p>The datetime Calcbench wrote/modified this value.</p>
 <p>Post November 2022 if this differs from the date_reported the fact was modified by Calcbench subsequent to the filing first being processed.</p>
 </dd>
+<dt>fling_accession_number</dt><dd><p>Accession number as assigned by the SEC for the filing from which this value came.</p>
+</dd>
+<dt>trace_url</dt><dd><p>URL for a page showing the source document for this value.</p>
+</dd>
 <dt>original_value (PIT only)</dt><dd><p>The value that Calcbench extracted when it first processed the filing.</p>
 <p>Post November 2022, if this differs from the value Calcbench the fact was modified by Calcbench subsequent to the filing first being processed.</p>
 </dd>
+<dt>standardized_id</dt><dd><p>A unique identifier Calcbench assigns to each standardized value.</p>
+</dd>
 <dt>date_downloaded</dt><dd><p>The timestamp on your computer when you downloaded this data.</p>
 </dd>
 </dl>
 <p>Usage:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="n">d</span> <span class="o">=</span> <span class="n">calcbench</span><span class="o">.</span><span class="n">standardized</span><span class="p">(</span><span class="n">company_identifiers</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;msft&#39;</span><span class="p">],</span>
 <span class="gp">&gt;&gt;&gt; </span>                                <span class="n">point_in_time</span><span class="o">=</span><span class="kc">True</span><span class="p">,)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="p">)</span>
```

#### html2text {}

```diff
@@ -33,17 +33,17 @@
                   get all metrics.
                 * fiscal_year (Optional[int]) â Fiscal year for which to get
                   data. If not specified get all history.
                 * fiscal_period (Union[Period, Literal[0, 1, 2, 3, 4], None])
                   â Fiscal period for which to get data. If not specified get
                   all history.
                 * start_date (Union[datetime, date, None]) â Restrict to
-                  records received on or after (inclusive) this date/datetime
+                  records modified on or after (inclusive) this date/datetime
                 * end_date (Union[datetime, date, None]) â Restric to records
-                  received prior (exclusive) thie date/datetime
+                  modified prior (exclusive) thie date/datetime
                 * point_in_time (bool) â Include timestamps when data was
                   published and revision chains.
                 * filing_id (Optional[int]) â Filing ID for which to get
                   data. Get all of the data reported in this filing.
                 * exclude_unconfirmed_preliminary (Optional[bool]) â Exclude
                   points from press-releases or 8-Ks that have not been
                   âconfirmedâ in an XBRL filing. Preliminary points have a
@@ -92,14 +92,19 @@
             True indicates the number was parsed from non-XBRL 8-K or press
             release from the wire
         XBRL
             Indicates the number was parsed from XBRL.
             The case where preliminary and XBRL are both true indicates the
             number was first parsed from a non-XBRL document then
             âconfirmedâ in an XBRL document.
+        date_XBRL_confirmed
+            Time at which the point was confirmed by an point from an XBRL
+            filing. If the point originally came from an XBRL filing this will
+            be the original write time. If this is null, for points post April
+            2023, the point has not been confirmed.
         period_start
             First day of the fiscal period for this fact
         period_end
             Last day of the fiscal period for this fact
         calendar_year
             The calendar year for this fact. https://knowledge.calcbench.com/
             hc/en-us/articles/223267767-What-are-Calendar-Years-and-Periods-
@@ -113,20 +118,27 @@
         filing_type
             The document type this fact came from, 10-K|Q, S-1 etcâ¦
         date_modified (PIT only)
             The datetime Calcbench wrote/modified this value.
             Post November 2022 if this differs from the date_reported the fact
             was modified by Calcbench subsequent to the filing first being
             processed.
+        fling_accession_number
+            Accession number as assigned by the SEC for the filing from which
+            this value came.
+        trace_url
+            URL for a page showing the source document for this value.
         original_value (PIT only)
             The value that Calcbench extracted when it first processed the
             filing.
             Post November 2022, if this differs from the value Calcbench the
             fact was modified by Calcbench subsequent to the filing first being
             processed.
+        standardized_id
+            A unique identifier Calcbench assigns to each standardized value.
         date_downloaded
             The timestamp on your computer when you downloaded this data.
       Usage:
       >>> d = calcbench.standardized(company_identifiers=['msft'],
       >>>                                 point_in_time=True,)
       >>> )
       >>> # Put the data in a format amiable to arithmetic on columns
```

### Comparing `calcbench_api_client-8.1.1/docs/html/press-release.html` & `calcbench_api_client-8.2.0/docs/html/press-release.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/push-notification.html` & `calcbench_api_client-8.2.0/docs/html/push-notification.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/py-modindex.html` & `calcbench_api_client-8.2.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/raw-numeric-XBRL.html` & `calcbench_api_client-8.2.0/docs/html/raw-numeric-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/raw-numeric-non-XBRL.html` & `calcbench_api_client-8.2.0/docs/html/raw-numeric-non-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/search.html` & `calcbench_api_client-8.2.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/html/searchindex.js` & `calcbench_api_client-8.2.0/docs/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -700,14 +700,15 @@
         "200": 8,
         "2015": 8,
         "2017": 4,
         "2018": [1, 4],
         "2019": 11,
         "2021": 11,
         "2022": 8,
+        "2023": 8,
         "20fr12g": 5,
         "21": 1,
         "22": 1,
         "223267767": 8,
         "23": 1,
         "24": 1,
         "25": 1,
@@ -809,14 +810,15 @@
         "default": [6, 8],
         "do": [5, 6, 8],
         "float": [0, 1, 5, 11],
         "function": [3, 6, 10],
         "import": [2, 3, 5],
         "int": [0, 1, 2, 4, 5, 8, 9, 11],
         "new": 7,
+        "null": 8,
         "public": [2, 10],
         "return": [0, 1, 2, 3, 4, 5, 6, 8, 9, 10, 11],
         "throw": 10,
         "true": [1, 2, 3, 4, 5, 6, 8, 10, 11],
         "try": 6,
         "while": [5, 8],
         A: [1, 2, 5, 8, 10, 11],
@@ -837,15 +839,15 @@
         The: [1, 2, 4, 5, 6, 8, 11],
         There: 5,
         To: 8,
         With: 2,
         _effvalu: 1,
         _point_in_time_mod: [],
         abov: [],
-        access: [0, 2, 5, 6, 11],
+        access: [0, 2, 5, 6, 8, 11],
         accession_id: [0, 2, 5, 10],
         account: 2,
         accountingpolici: 2,
         accountsreceiv: 8,
         acquiredfinitelivedintangibleassetsweightedaverageusefullif: 1,
         acquisit: 0,
         acquisition_d: 0,
@@ -890,14 +892,15 @@
         api_query_param: [1, 2, 5, 8, 11],
         appear: [5, 11],
         append: 3,
         appl: [1, 8],
         appli: [3, 8],
         applic: [1, 2],
         applymap: 2,
+        april: 8,
         ar: [0, 1, 2, 5, 6, 8],
         arg: [1, 5],
         argument: 3,
         arithmet: 8,
         articl: 8,
         as_originally_report: 1,
         as_reported_raw: [],
@@ -1019,15 +1022,15 @@
         chain: 8,
         chang: [4, 8],
         changeinequ: 4,
         cik: [1, 2, 4, 5, 8, 9, 11],
         classmethod: 4,
         claus: 11,
         client: [0, 3, 10],
-        code: [1, 2, 4, 5, 8, 11],
+        code: [1, 2, 4, 5, 6, 8, 11],
         column: [0, 1, 3, 4, 5, 8, 11],
         column_label: 11,
         com: [1, 2, 4, 5, 6, 7, 8, 10, 11],
         combin: [2, 4, 7, 8],
         commentlett: [2, 5],
         commentletterrespons: 5,
         commit: [2, 8],
@@ -1078,14 +1081,15 @@
         dataset: 3,
         date: [2, 4, 5, 8, 9, 11],
         date_download: 8,
         date_modifi: 8,
         date_originally_report: 0,
         date_rang: 4,
         date_report: [0, 1, 2, 8, 9],
+        date_xbrl_confirm: 8,
         datetim: [0, 2, 4, 5, 8, 9, 11],
         debt: 2,
         debtinstrumentcarryingamount: 1,
         debtinstrumentfaceamount: 1,
         debtinstrumentinterestrateeffectivepercentag: 1,
         debtinstrumentinterestratestatedpercentag: 1,
         debtinstrumentmaturityd: 1,
@@ -1318,14 +1322,15 @@
         fiscal_period: [1, 2, 4, 5, 8, 9, 11],
         fiscal_period_period: 4,
         fiscal_period_typ: 4,
         fiscal_period_year: 4,
         fiscal_year: [1, 2, 5, 8, 9, 11],
         fiscal_year_end_d: 9,
         fiscalyear: 11,
+        fling_accession_numb: 8,
         flow: [],
         focu: 4,
         focus_neg: 4,
         focusn: 5,
         footnot: [2, 8],
         footnote_fact_id: 4,
         footnote_typ: 2,
@@ -1370,15 +1375,15 @@
         giveup: 6,
         go: 8,
         goodwil: 2,
         goog: [1, 2, 8],
         guidanc: [4, 11],
         guide_link: 2,
         h1: 8,
-        ha: 5,
+        ha: [5, 8],
         half: 8,
         halfyear: 5,
         handl: [6, 8, 10],
         handle_fil: 10,
         handler: 10,
         has_been_revis: 4,
         has_dimens: 4,
@@ -1709,15 +1714,15 @@
         realestateandaccumulateddepreciationamountofencumbr: 1,
         realestateandaccumulateddepreciationcarryingamountofbuildingsandimprov: 1,
         realestateandaccumulateddepreciationcarryingamountofland: 1,
         realestateandaccumulateddepreciationcostscapitalizedsubsequenttoacquisitioncarryingcost: 1,
         realestateandaccumulateddepreciationinitialcostofbuildingsandimprov: 1,
         realestateandaccumulateddepreciationinitialcostofland: 1,
         realestategrossatcarryingvalu: 1,
-        receiv: [4, 5, 8],
+        receiv: [4, 5],
         received_d: [2, 5],
         received_data: [],
         reciev: [5, 10],
         record: [5, 8],
         refer: [4, 11],
         relat: 2,
         relateddocu: 2,
@@ -1806,35 +1811,36 @@
         sharebasedcompensationsharesauthorizedunderstockoptionplansexercisepricerangeoutstandingoptionsweightedaverageremainingcontractualterm: 1,
         sharebasedcompensationsharesauthorizedunderstockoptionplansexercisepricerangeupperrangelimit: 1,
         sharedaccesskei: 10,
         sharedaccesskeynam: 10,
         sheet: 4,
         shell: 6,
         should: [5, 8],
-        show: [1, 5],
+        show: [1, 5, 8],
         sign: 6,
         sinc: [],
         singl: [2, 8],
         single_d: 11,
         so6q: 10,
         so: 3,
         some: 8,
         someth: [8, 10],
         sort: 3,
-        sourc: 1,
+        sourc: [1, 8],
         sp500: 2,
         sp: 5,
         special_fact_typ: [4, 11],
         specif: [2, 11],
         specifi: 8,
         split: 2,
         stack: [],
         standar: [],
         standard: [0, 3, 5, 6, 7, 11],
         standardized_data: [],
+        standardized_id: 8,
         standardized_numer: [0, 1],
         standardized_pit_arrow: 3,
         standardized_ppa_point: 0,
         standardized_raw: 8,
         standardized_xbrl: [5, 10],
         standardizedmetr: 8,
         standardizedpoint: [0, 8],
@@ -1870,15 +1876,15 @@
         t: [3, 10],
         tabl: [1, 3, 5],
         table_id: 9,
         table_list: 2,
         tabular_item: 11,
         tag: [2, 4, 8, 11],
         take: 8,
-        talk: [8, 10],
+        talk: [6, 8, 10],
         target: 0,
         tax: 2,
         text: [7, 9],
         text_fact_id: 4,
         textblock: 2,
         tf: 2,
         than: [1, 8],
@@ -1895,43 +1901,43 @@
         to_panda: 3,
         todai: 5,
         toggl: 6,
         tqdm: [2, 3],
         trace_fact: 1,
         trace_hyperlink: [],
         trace_link: 0,
-        trace_url: 1,
+        trace_url: [1, 8],
         tracedata: 1,
         trailingtwelvemonth: 8,
         tree_depth: 4,
         trial: 6,
         ttm: 8,
         tupl: 1,
         turn: 6,
         turn_on_log: 6,
         two: [6, 8],
         type: [0, 1, 2, 3, 4, 5, 6, 8, 9, 11],
         under: [],
         understand: [],
         unformat: 1,
         union: [0, 1, 2, 3, 4, 5, 8, 11],
-        uniqu: 11,
+        uniqu: [8, 11],
         unique_id: 4,
         unit: 11,
         unit_of_measur: 4,
         unrevis: 8,
         unset: 11,
         unstack: 8,
         until: 8,
         uom: [9, 11],
         up: 6,
         update_d: [],
         updated_from: 2,
         upload: 5,
-        url: [1, 4, 9, 11],
+        url: [1, 4, 8, 9, 11],
         us: [0, 2, 3, 6, 8, 11],
         usag: [1, 2, 3, 4, 5, 6, 8, 10, 11],
         usd: 11,
         use_fiscal_period: [2, 8],
         useful_life_lower_rang: 0,
         useful_life_upper_rang: 0,
         user: 6,
@@ -1959,15 +1965,15 @@
         window: [6, 10],
         wire: [5, 8, 10],
         wirepr: 5,
         wirepress: [],
         word_count: 2,
         work: [],
         would: 11,
-        write: [3, 10],
+        write: [3, 8, 10],
         write_index: 3,
         write_mod: 3,
         written: 3,
         wrong: 8,
         wrote: 8,
         www: [1, 2, 4, 5, 6, 8, 11],
         x: 5,
```

### Comparing `calcbench_api_client-8.1.1/docs/make.bat` & `calcbench_api_client-8.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/source/conf.py` & `calcbench_api_client-8.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/source/getting-started.rst` & `calcbench_api_client-8.2.0/docs/source/getting-started.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Getting Started
 ===============
 
 .. warning::
-     Calcbench data is not free and API access is not included in the standard Calcbench subscription.
+     Calcbench data is not free and API access is not included in the standard Calcbench subscription.  Talk to us@calcbench.com before you start coding.
 
 .. _install:
 
 Installing the Client
 ---------------------
```

### Comparing `calcbench_api_client-8.1.1/docs/source/index.rst` & `calcbench_api_client-8.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/source/numeric-data.rst` & `calcbench_api_client-8.2.0/docs/source/numeric-data.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/docs/source/push-notification.rst` & `calcbench_api_client-8.2.0/docs/source/push-notification.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.1.1/setup.py` & `calcbench_api_client-8.2.0/setup.py`

 * *Files identical despite different names*

