# Comparing `tmp/gerrytools-1.1.0.tar.gz` & `tmp/gerrytools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrytools-1.1.0.tar", last modified: Fri Apr 28 15:19:53 2023, max compression
+gzip compressed data, was "gerrytools-1.1.1.tar", last modified: Fri Apr 28 15:28:10 2023, max compression
```

## Comparing `gerrytools-1.1.0.tar` & `gerrytools-1.1.1.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.576531 gerrytools-1.1.0/
--rw-r--r--   0 pjrule     (501) staff       (20)     1469 2022-12-02 15:49:19.000000 gerrytools-1.1.0/LICENSE
--rw-r--r--   0 pjrule     (501) staff       (20)       44 2022-12-02 15:49:19.000000 gerrytools-1.1.0/MANIFEST.in
--rw-r--r--   0 pjrule     (501) staff       (20)     6176 2023-04-28 15:19:53.576336 gerrytools-1.1.0/PKG-INFO
--rw-r--r--   0 pjrule     (501) staff       (20)     5862 2023-04-28 15:15:18.000000 gerrytools-1.1.0/README.md
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.562779 gerrytools-1.1.0/gerrytools/
--rw-r--r--   0 pjrule     (501) staff       (20)       46 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/__init__.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.566634 gerrytools-1.1.0/gerrytools/data/
--rw-r--r--   0 pjrule     (501) staff       (20)    12360 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/AssignmentCompressor.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1629 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/data/URLs.py
--rw-r--r--   0 pjrule     (501) staff       (20)      760 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/__init__.py
--rw-r--r--   0 pjrule     (501) staff       (20)    11786 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/acs.py
--rw-r--r--   0 pjrule     (501) staff       (20)    10384 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/census.py
--rw-r--r--   0 pjrule     (501) staff       (20)    17386 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/estimatecvap.py
--rw-r--r--   0 pjrule     (501) staff       (20)     7726 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/fetch.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1563 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/data/geometries.py
--rw-r--r--   0 pjrule     (501) staff       (20)     3602 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/remap.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.568415 gerrytools-1.1.0/gerrytools/geometry/
--rw-r--r--   0 pjrule     (501) staff       (20)      781 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/__init__.py
--rw-r--r--   0 pjrule     (501) staff       (20)     4923 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/compactness.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1117 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/dataframe.py
--rw-r--r--   0 pjrule     (501) staff       (20)     9249 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/dissolve.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1862 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/geometry/dualgraph.py
--rw-r--r--   0 pjrule     (501) staff       (20)    20337 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/optimize.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2330 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/unitmap.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1302 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/updater.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.572463 gerrytools-1.1.0/gerrytools/plotting/
--rw-r--r--   0 pjrule     (501) staff       (20)      961 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/__init__.py
--rw-r--r--   0 pjrule     (501) staff       (20)     3774 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/annotation.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1732 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/bins.py
--rw-r--r--   0 pjrule     (501) staff       (20)     4237 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/boxplot.py
--rw-r--r--   0 pjrule     (501) staff       (20)     4978 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/choropleth.py
--rw-r--r--   0 pjrule     (501) staff       (20)     3780 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/colors.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1701 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/plotting/districtnumbers.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2721 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/drawgraph.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2352 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/drawplan.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2696 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/gifs.py
--rw-r--r--   0 pjrule     (501) staff       (20)     3666 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/histogram.py
--rw-r--r--   0 pjrule     (501) staff       (20)    20106 2022-12-02 15:49:19.000000 gerrytools-1.1.0/gerrytools/plotting/latexcolors.json
--rw-r--r--   0 pjrule     (501) staff       (20)     2291 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/multidimensional.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2171 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/scatterplot.py
--rw-r--r--   0 pjrule     (501) staff       (20)     2430 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/sealevel.py
--rw-r--r--   0 pjrule     (501) staff       (20)      396 2022-12-02 15:49:19.000000 gerrytools-1.1.0/gerrytools/plotting/utils.py
--rw-r--r--   0 pjrule     (501) staff       (20)     4677 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/violin.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.574264 gerrytools-1.1.0/gerrytools/scoring/
--rw-r--r--   0 pjrule     (501) staff       (20)     1589 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/__init__.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1547 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/scoring/contiguity.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1399 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/demographics.py
--rw-r--r--   0 pjrule     (501) staff       (20)     5406 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/partisan.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1037 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/scoring/population.py
--rw-r--r--   0 pjrule     (501) staff       (20)    28615 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/scores.py
--rw-r--r--   0 pjrule     (501) staff       (20)     7151 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/splits.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1012 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/types.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.575080 gerrytools-1.1.0/gerrytools/utilities/
--rw-r--r--   0 pjrule     (501) staff       (20)     3026 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/utilities/JSON.py
--rw-r--r--   0 pjrule     (501) staff       (20)      177 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/utilities/__init__.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1238 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/utilities/rename.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.563859 gerrytools-1.1.0/gerrytools.egg-info/
--rw-r--r--   0 pjrule     (501) staff       (20)     6176 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/PKG-INFO
--rw-r--r--   0 pjrule     (501) staff       (20)     1743 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/SOURCES.txt
--rw-r--r--   0 pjrule     (501) staff       (20)        1 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/dependency_links.txt
--rw-r--r--   0 pjrule     (501) staff       (20)      215 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/requires.txt
--rw-r--r--   0 pjrule     (501) staff       (20)       11 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/top_level.txt
--rw-r--r--   0 pjrule     (501) staff       (20)       31 2023-04-28 15:10:19.000000 gerrytools-1.1.0/pyproject.toml
--rw-r--r--   0 pjrule     (501) staff       (20)       38 2023-04-28 15:19:53.576580 gerrytools-1.1.0/setup.cfg
--rw-r--r--   0 pjrule     (501) staff       (20)     1105 2023-04-28 15:18:43.000000 gerrytools-1.1.0/setup.py
-drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.576007 gerrytools-1.1.0/tests/
--rw-r--r--   0 pjrule     (501) staff       (20)    19311 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_data.py
--rw-r--r--   0 pjrule     (501) staff       (20)     4968 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_geometry.py
--rw-r--r--   0 pjrule     (501) staff       (20)     1883 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_plotting.py
--rw-r--r--   0 pjrule     (501) staff       (20)    10529 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_scoring.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.624028 gerrytools-1.1.1/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1469 2023-01-23 15:04:17.000000 gerrytools-1.1.1/LICENSE
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)       44 2023-01-23 15:04:17.000000 gerrytools-1.1.1/MANIFEST.in
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     6176 2023-04-28 15:28:10.622264 gerrytools-1.1.1/PKG-INFO
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     5862 2023-04-28 15:26:34.000000 gerrytools-1.1.1/README.md
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.288438 gerrytools-1.1.1/gerrytools/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)       46 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/__init__.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.363536 gerrytools-1.1.1/gerrytools/data/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    12360 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/AssignmentCompressor.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1629 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/URLs.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      760 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/__init__.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    11786 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/acs.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    10384 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/census.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    17386 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/estimatecvap.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     7726 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/fetch.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1563 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/geometries.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     3602 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/remap.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.407685 gerrytools-1.1.1/gerrytools/geometry/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      781 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/__init__.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     4923 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/compactness.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1117 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dataframe.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     9249 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dissolve.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1862 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dualgraph.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    20337 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/optimize.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2330 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/unitmap.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1302 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/updater.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.513960 gerrytools-1.1.1/gerrytools/plotting/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      961 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/__init__.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     3774 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/annotation.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1732 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/bins.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     4237 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/boxplot.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     4978 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/choropleth.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     3780 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/colors.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1701 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/districtnumbers.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2721 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/drawgraph.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2352 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/drawplan.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2696 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/gifs.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     3666 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/histogram.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    20106 2023-01-23 15:04:17.000000 gerrytools-1.1.1/gerrytools/plotting/latexcolors.json
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2291 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/multidimensional.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2171 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/scatterplot.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     2430 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/sealevel.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      396 2023-01-23 15:04:17.000000 gerrytools-1.1.1/gerrytools/plotting/utils.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     4677 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/violin.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.566645 gerrytools-1.1.1/gerrytools/scoring/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1589 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/__init__.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1547 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/contiguity.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1399 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/demographics.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     5406 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/partisan.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1037 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/population.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    28615 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/scores.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     7151 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/splits.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1012 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/types.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.584368 gerrytools-1.1.1/gerrytools/utilities/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     3026 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/JSON.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      177 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/__init__.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1238 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/rename.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.314274 gerrytools-1.1.1/gerrytools.egg-info/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     6176 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/PKG-INFO
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1728 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/SOURCES.txt
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)        1 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/dependency_links.txt
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)      215 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/requires.txt
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)       11 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/top_level.txt
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)       38 2023-04-28 15:28:10.626540 gerrytools-1.1.1/setup.cfg
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1105 2023-04-28 15:27:54.000000 gerrytools-1.1.1/setup.py
+drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.615783 gerrytools-1.1.1/tests/
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    19311 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_data.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     4968 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_geometry.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)     1883 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_plotting.py
+-rw-rw----   0 cricha10 (31944) cricha10  (6417)    10529 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_scoring.py
```

### Comparing `gerrytools-1.1.0/LICENSE` & `gerrytools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/PKG-INFO` & `gerrytools-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrytools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for processing and visualizing districting plans.
 Home-page: https://github.com/mggg/gerrytools
 Author: MGGG Redistricting Lab
 Author-email: engineering@mggg.org
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `gerrytools-1.1.0/README.md` & `gerrytools-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/AssignmentCompressor.py` & `gerrytools-1.1.1/gerrytools/data/AssignmentCompressor.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/URLs.py` & `gerrytools-1.1.1/gerrytools/data/URLs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/__init__.py` & `gerrytools-1.1.1/gerrytools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/acs.py` & `gerrytools-1.1.1/gerrytools/data/acs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/census.py` & `gerrytools-1.1.1/gerrytools/data/census.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/estimatecvap.py` & `gerrytools-1.1.1/gerrytools/data/estimatecvap.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/fetch.py` & `gerrytools-1.1.1/gerrytools/data/fetch.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/geometries.py` & `gerrytools-1.1.1/gerrytools/data/geometries.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/data/remap.py` & `gerrytools-1.1.1/gerrytools/data/remap.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/__init__.py` & `gerrytools-1.1.1/gerrytools/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/compactness.py` & `gerrytools-1.1.1/gerrytools/geometry/compactness.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/dataframe.py` & `gerrytools-1.1.1/gerrytools/geometry/dataframe.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/dissolve.py` & `gerrytools-1.1.1/gerrytools/geometry/dissolve.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/dualgraph.py` & `gerrytools-1.1.1/gerrytools/geometry/dualgraph.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/optimize.py` & `gerrytools-1.1.1/gerrytools/geometry/optimize.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/unitmap.py` & `gerrytools-1.1.1/gerrytools/geometry/unitmap.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/geometry/updater.py` & `gerrytools-1.1.1/gerrytools/geometry/updater.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/__init__.py` & `gerrytools-1.1.1/gerrytools/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/annotation.py` & `gerrytools-1.1.1/gerrytools/plotting/annotation.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/bins.py` & `gerrytools-1.1.1/gerrytools/plotting/bins.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/boxplot.py` & `gerrytools-1.1.1/gerrytools/plotting/boxplot.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/choropleth.py` & `gerrytools-1.1.1/gerrytools/plotting/choropleth.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/colors.py` & `gerrytools-1.1.1/gerrytools/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/districtnumbers.py` & `gerrytools-1.1.1/gerrytools/plotting/districtnumbers.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/drawgraph.py` & `gerrytools-1.1.1/gerrytools/plotting/drawgraph.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/drawplan.py` & `gerrytools-1.1.1/gerrytools/plotting/drawplan.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/gifs.py` & `gerrytools-1.1.1/gerrytools/plotting/gifs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/histogram.py` & `gerrytools-1.1.1/gerrytools/plotting/histogram.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/latexcolors.json` & `gerrytools-1.1.1/gerrytools/plotting/latexcolors.json`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/multidimensional.py` & `gerrytools-1.1.1/gerrytools/plotting/multidimensional.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/scatterplot.py` & `gerrytools-1.1.1/gerrytools/plotting/scatterplot.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/sealevel.py` & `gerrytools-1.1.1/gerrytools/plotting/sealevel.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/plotting/violin.py` & `gerrytools-1.1.1/gerrytools/plotting/violin.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/__init__.py` & `gerrytools-1.1.1/gerrytools/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/contiguity.py` & `gerrytools-1.1.1/gerrytools/scoring/contiguity.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/demographics.py` & `gerrytools-1.1.1/gerrytools/scoring/demographics.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/partisan.py` & `gerrytools-1.1.1/gerrytools/scoring/partisan.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/population.py` & `gerrytools-1.1.1/gerrytools/scoring/population.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/scores.py` & `gerrytools-1.1.1/gerrytools/scoring/scores.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/splits.py` & `gerrytools-1.1.1/gerrytools/scoring/splits.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/scoring/types.py` & `gerrytools-1.1.1/gerrytools/scoring/types.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/utilities/JSON.py` & `gerrytools-1.1.1/gerrytools/utilities/JSON.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools/utilities/rename.py` & `gerrytools-1.1.1/gerrytools/utilities/rename.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/gerrytools.egg-info/PKG-INFO` & `gerrytools-1.1.1/gerrytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrytools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for processing and visualizing districting plans.
 Home-page: https://github.com/mggg/gerrytools
 Author: MGGG Redistricting Lab
 Author-email: engineering@mggg.org
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `gerrytools-1.1.0/gerrytools.egg-info/SOURCES.txt` & `gerrytools-1.1.1/gerrytools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 gerrytools/__init__.py
 gerrytools.egg-info/PKG-INFO
 gerrytools.egg-info/SOURCES.txt
 gerrytools.egg-info/dependency_links.txt
 gerrytools.egg-info/requires.txt
 gerrytools.egg-info/top_level.txt
```

### Comparing `gerrytools-1.1.0/setup.py` & `gerrytools-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "pydantic",
     "censusdata",
     "seaborn",
     "maup",
 ]
 
 # Set the version --- ensure that the latest tag matches this value.
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 
 # Description.
 here = Path(__file__).parent
 DESCRIPTION = (here / "README.md").read_text()
 
 setup(
     name="gerrytools",
```

### Comparing `gerrytools-1.1.0/tests/test_data.py` & `gerrytools-1.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/tests/test_geometry.py` & `gerrytools-1.1.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/tests/test_plotting.py` & `gerrytools-1.1.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.0/tests/test_scoring.py` & `gerrytools-1.1.1/tests/test_scoring.py`

 * *Files identical despite different names*

