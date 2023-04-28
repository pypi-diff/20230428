# Comparing `tmp/textdescriptives-2.5.1.tar.gz` & `tmp/textdescriptives-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.5.1.tar", last modified: Wed Apr 26 12:41:05 2023, max compression
+gzip compressed data, was "textdescriptives-2.6.0.tar", last modified: Fri Apr 28 08:37:10 2023, max compression
```

## Comparing `textdescriptives-2.5.1.tar` & `textdescriptives-2.6.0.tar`

### file list

```diff
@@ -1,99 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.892270 textdescriptives-2.5.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.872270 textdescriptives-2.5.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.872270 textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.872270 textdescriptives-2.5.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2261 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)     7553 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23997 2023-04-26 12:41:05.888270 textdescriptives-2.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9640 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.876270 textdescriptives-2.5.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.880271 textdescriptives-2.5.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3548 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2784 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      349 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.880271 textdescriptives-2.5.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96689 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7465 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.880271 textdescriptives-2.5.1/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     3059 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:41:05.892270 textdescriptives-2.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.868270 textdescriptives-2.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.880271 textdescriptives-2.5.1/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.884271 textdescriptives-2.5.1/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     7504 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5515 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22254 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10426 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.884271 textdescriptives-2.5.1/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6126 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/extractors.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.884271 textdescriptives-2.5.1/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23997 2023-04-26 12:41:05.000000 textdescriptives-2.5.1/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2365 2023-04-26 12:41:05.000000 textdescriptives-2.5.1/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:41:05.000000 textdescriptives-2.5.1/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-26 12:41:05.000000 textdescriptives-2.5.1/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-26 12:41:05.000000 textdescriptives-2.5.1/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:41:05.888270 textdescriptives-2.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-26 12:40:55.000000 textdescriptives-2.5.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.759298 textdescriptives-2.6.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.743297 textdescriptives-2.6.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23971 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-28 08:37:00.000000 textdescriptives-2.6.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.747298 textdescriptives-2.6.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    17211 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:37:10.759298 textdescriptives-2.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.739297 textdescriptives-2.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22254 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6126 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.751298 textdescriptives-2.6.0/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23971 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 08:37:10.000000 textdescriptives-2.6.0/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:37:10.755298 textdescriptives-2.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-28 08:37:01.000000 textdescriptives-2.6.0/tests/test_utils.py
```

### Comparing `textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.6.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/dependabot.yml` & `textdescriptives-2.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.6.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/documentation.yml` & `textdescriptives-2.6.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/draft-pdf.yml` & `textdescriptives-2.6.0/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/release.yml` & `textdescriptives-2.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/stale.yml` & `textdescriptives-2.6.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.github/workflows/tests.yml` & `textdescriptives-2.6.0/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   pytest-and-notebooks:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.9", "3.8", "3.7"]
+        python-version: ["3.9", "3.8"]
 
     # This allows a subsequently queued workflow run to interrupt previous runs
     concurrency:
       group: "${{ github.workflow }} - ${{ matrix.python-version}} - ${{ matrix.os }} @ ${{ github.ref }}"
       cancel-in-progress: true
 
     steps:
```

### Comparing `textdescriptives-2.5.1/.gitignore` & `textdescriptives-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.pre-commit-config.yaml` & `textdescriptives-2.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/.zenodo.json` & `textdescriptives-2.6.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/CHANGELOG.md` & `textdescriptives-2.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.6.0 (2023-04-28)
+### Feature
+* Add sklearn transformer ([`be733c6`](https://github.com/HLasse/TextDescriptives/commit/be733c6161993deb6e284475224d6363c99a8962))
+
+### Documentation
+* Add sklearn to requirements in docs ([`33194c9`](https://github.com/HLasse/TextDescriptives/commit/33194c937803acdd2abb4198b97ead3981958fd1))
+* Minor docstring changes ([`375d3e0`](https://github.com/HLasse/TextDescriptives/commit/375d3e03a8792b54f5dfd6080e27ca34925628c3))
+* Add sklearn tutorial ([`4220072`](https://github.com/HLasse/TextDescriptives/commit/42200725c2c89c738a07fffdc1b8f7b6d111fc6c))
+
 ## v2.5.1 (2023-04-26)
 ### Fix
 * Don't subtract 1 from counts if `add_all_tags` is False ([`02b61a6`](https://github.com/HLasse/TextDescriptives/commit/02b61a6358764af5901891e002bc4e3771c777c6))
 
 ## v2.5.0 (2023-04-26)
 ### Feature
 * Add proportions of all pos tags ([`664c0e8`](https://github.com/HLasse/TextDescriptives/commit/664c0e886a4ff075ea15ec08c9acf1e76a785477))
```

### Comparing `textdescriptives-2.5.1/CITATION.cff` & `textdescriptives-2.6.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/CODE_OF_CONDUCT.md` & `textdescriptives-2.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/CONTRIBUTING.md` & `textdescriptives-2.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/LICENSE` & `textdescriptives-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/PKG-INFO` & `textdescriptives-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.5.1
+Version: 2.6.0
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,23 +216,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: tutorials
+Provides-Extra: sklearn
 License-File: LICENSE
 
 
 <a href="https://github.com/HLasse/TextDescriptives"><img src="https://github.com/HLasse/TextDescriptives/raw/main/docs/_static/icon.png" width="175" height="175" align="right" /></a>
 
 
 # TextDescriptives
```

### Comparing `textdescriptives-2.5.1/README.md` & `textdescriptives-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/Makefile` & `textdescriptives-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/_static/icon.png` & `textdescriptives-2.6.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/_static/icon_dark_old.png` & `textdescriptives-2.6.0/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/_static/icon_old.png` & `textdescriptives-2.6.0/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/coherence.rst` & `textdescriptives-2.6.0/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/conf.py` & `textdescriptives-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/dependencydistance.rst` & `textdescriptives-2.6.0/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/descriptivestats.rst` & `textdescriptives-2.6.0/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/faq.rst` & `textdescriptives-2.6.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/index.rst` & `textdescriptives-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/information_theory.rst` & `textdescriptives-2.6.0/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/installation.rst` & `textdescriptives-2.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/make.bat` & `textdescriptives-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/news.rst` & `textdescriptives-2.6.0/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/posstats.rst` & `textdescriptives-2.6.0/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/quality.rst` & `textdescriptives-2.6.0/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/readability.rst` & `textdescriptives-2.6.0/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.6.0/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.6.0/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/docs/usingthepackage.rst` & `textdescriptives-2.6.0/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/paper/paper.bib` & `textdescriptives-2.6.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/paper/paper.md` & `textdescriptives-2.6.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/paper/paper_quarto.pdf` & `textdescriptives-2.6.0/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/paper/paper_quarto.qmd` & `textdescriptives-2.6.0/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/pyproject.toml` & `textdescriptives-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [project]
 name = "textdescriptives"
-version = "2.5.1"
+version = "2.6.0"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"},
              {name = "Kenneth Enevoldsen"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 keywords = [
     "NLP",
     "spaCy",
@@ -36,15 +35,15 @@
     "spacy[lookups]>=3.1.0,<3.6.0",
     "numpy>=1.20.0,<1.25.0",
     "pandas>=1.0.0,<1.6.0",
     "pyphen>=0.11.0,<0.15.0",
     "ftfy>=6.0.3,<6.1.0",
 ]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://hlasse.github.io/TextDescriptives/"
 repository = "https://github.com/HLasse/textdescriptives"
 documentation = "https://hlasse.github.io/TextDescriptives/"
 
 [project.optional-dependencies]
@@ -67,15 +66,19 @@
     "sphinx_design>=0.3.0,<0.3.1",
     "autodoc_pydantic>=1.1.0,<1.9.0",
 ]
 tutorials = [
     "jupyter",
     "seaborn",
     "matplotlib",
-    "datasets>=2.8.0,<2.11.0",
+    "datasets>=2.8.0",
+    "scikit-learn>=1.1.1",
+]
+sklearn = [
+    "scikit-learn>=1.1.1",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.license]
```

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/coherence.py` & `textdescriptives-2.6.0/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.6.0/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.6.0/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.6.0/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.6.0/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/quality.py` & `textdescriptives-2.6.0/src/textdescriptives/components/quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.6.0/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/readability.py` & `textdescriptives-2.6.0/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/components/utils.py` & `textdescriptives-2.6.0/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/data/spam.csv` & `textdescriptives-2.6.0/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/extractors.py` & `textdescriptives-2.6.0/src/textdescriptives/extractors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -115,24 +115,24 @@
     spacy_model: Optional[str] = None,
     spacy_model_size: str = "lg",
 ) -> pd.DataFrame:
     """Extract metrics from a text or a list of texts to a Pandas dataframe.
 
     Args:
         text (Union[str, List[str]]): A text or a list of texts.
-        spacy_model (str, optional): The spacy model to use. If not set,
-            will download one based on lang. Defaults to None.
         lang (str, optional): Language of the text. If lang is set and no spacy
             model is provided, will automatically download and use a spacy
             model for the language. Defaults to None.
         metrics (List[str]): Which metrics to extract.
             One or more of ["descriptive_stats", "readability",
             "dependency_distance", "pos_proportions", "coherence", "quality",
             "information_theory"]. If None, will extract all metrics from
             textdescriptives. Defaults to None.
+        spacy_model (str, optional): The spacy model to use. If not set,
+            will download one based on lang. Defaults to None.
         spacy_model_size (str, optional): Size of the spacy model to download.
 
     Returns:
         pd.DataFrame: DataFrame with a row for each text and column for each metric.
     """
     if isinstance(metrics, str):
         metrics = [metrics]
```

### Comparing `textdescriptives-2.5.1/src/textdescriptives/load_components.py` & `textdescriptives-2.6.0/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives/utils.py` & `textdescriptives-2.6.0/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.6.0/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.5.1
+Version: 2.6.0
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,23 +216,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: style
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: tutorials
+Provides-Extra: sklearn
 License-File: LICENSE
 
 
 <a href="https://github.com/HLasse/TextDescriptives"><img src="https://github.com/HLasse/TextDescriptives/raw/main/docs/_static/icon.png" width="175" height="175" align="right" /></a>
 
 
 # TextDescriptives
```

### Comparing `textdescriptives-2.5.1/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.6.0/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 docs/usingthepackage.rst
 docs/_static/icon.png
 docs/_static/icon_dark_old.png
 docs/_static/icon_old.png
 docs/tutorials/filter_corpus_using_quality.ipynb
 docs/tutorials/introductory_tutorial.ipynb
 docs/tutorials/requirements.txt
+docs/tutorials/sklearn_integration.ipynb
 paper/paper.bib
 paper/paper.md
 paper/paper_quarto.pdf
 paper/paper_quarto.qmd
 paper/readme.md
 src/textdescriptives/__init__.py
 src/textdescriptives/about.py
@@ -64,14 +65,16 @@
 src/textdescriptives/components/information_theory.py
 src/textdescriptives/components/pos_proportions.py
 src/textdescriptives/components/quality.py
 src/textdescriptives/components/quality_data_classes.py
 src/textdescriptives/components/readability.py
 src/textdescriptives/components/utils.py
 src/textdescriptives/data/spam.csv
+src/textdescriptives/integrations/__init__.py
+src/textdescriptives/integrations/sklearn_featurizer.py
 tests/__init__.py
 tests/books.py
 tests/requirements.txt
 tests/test_coherence.py
 tests/test_dependency_distance.py
 tests/test_descriptive_stats.py
 tests/test_extractors.py
```

### Comparing `textdescriptives-2.5.1/tests/books.py` & `textdescriptives-2.6.0/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_coherence.py` & `textdescriptives-2.6.0/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_dependency_distance.py` & `textdescriptives-2.6.0/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_descriptive_stats.py` & `textdescriptives-2.6.0/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_extractors.py` & `textdescriptives-2.6.0/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_information.py` & `textdescriptives-2.6.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_load_components.py` & `textdescriptives-2.6.0/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_pos_proportions.py` & `textdescriptives-2.6.0/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_quality.py` & `textdescriptives-2.6.0/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_readability.py` & `textdescriptives-2.6.0/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.5.1/tests/test_utils.py` & `textdescriptives-2.6.0/tests/test_utils.py`

 * *Files identical despite different names*

