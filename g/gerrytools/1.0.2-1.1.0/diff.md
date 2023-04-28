# Comparing `tmp/gerrytools-1.0.2.tar.gz` & `tmp/gerrytools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrytools-1.0.2.tar", last modified: Thu Jul  7 21:54:31 2022, max compression
+gzip compressed data, was "gerrytools-1.1.0.tar", last modified: Fri Apr 28 15:19:53 2023, max compression
```

## Comparing `gerrytools-1.0.2.tar` & `gerrytools-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.480437 gerrytools-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1469 2022-07-07 21:54:22.000000 gerrytools-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       44 2022-07-07 21:54:22.000000 gerrytools-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5924 2022-07-07 21:54:31.480437 gerrytools-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5610 2022-07-07 21:54:22.000000 gerrytools-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.472437 gerrytools-1.0.2/gerrytools/
--rw-r--r--   0 root         (0) root         (0)       47 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.476437 gerrytools-1.0.2/gerrytools/data/
--rw-r--r--   0 root         (0) root         (0)    12316 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/AssignmentCompressor.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/URLs.py
--rw-r--r--   0 root         (0) root         (0)      760 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11399 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/acs.py
--rw-r--r--   0 root         (0) root         (0)     9136 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/census.py
--rw-r--r--   0 root         (0) root         (0)    17154 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/estimatecvap.py
--rw-r--r--   0 root         (0) root         (0)     7650 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/fetch.py
--rw-r--r--   0 root         (0) root         (0)     1542 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/geometries.py
--rw-r--r--   0 root         (0) root         (0)     3612 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/data/remap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.476437 gerrytools-1.0.2/gerrytools/geometry/
--rw-r--r--   0 root         (0) root         (0)      762 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1104 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     1334 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/dissolve.py
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/dualgraph.py
--rw-r--r--   0 root         (0) root         (0)    18505 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/optimize.py
--rw-r--r--   0 root         (0) root         (0)     2330 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/unitmap.py
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/geometry/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.480437 gerrytools-1.0.2/gerrytools/plotting/
--rw-r--r--   0 root         (0) root         (0)      961 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3711 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/annotation.py
--rw-r--r--   0 root         (0) root         (0)     1732 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/bins.py
--rw-r--r--   0 root         (0) root         (0)     3927 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/boxplot.py
--rw-r--r--   0 root         (0) root         (0)     4910 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/choropleth.py
--rw-r--r--   0 root         (0) root         (0)     3494 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     1646 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/districtnumbers.py
--rw-r--r--   0 root         (0) root         (0)     2733 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/drawgraph.py
--rw-r--r--   0 root         (0) root         (0)     2269 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/drawplan.py
--rw-r--r--   0 root         (0) root         (0)     2577 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/gifs.py
--rw-r--r--   0 root         (0) root         (0)     3592 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/histogram.py
--rw-r--r--   0 root         (0) root         (0)    20106 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/latexcolors.json
--rw-r--r--   0 root         (0) root         (0)     2201 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/multidimensional.py
--rw-r--r--   0 root         (0) root         (0)     2120 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/scatterplot.py
--rw-r--r--   0 root         (0) root         (0)     2321 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/sealevel.py
--rw-r--r--   0 root         (0) root         (0)      396 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/utils.py
--rw-r--r--   0 root         (0) root         (0)     4453 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/plotting/violin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.480437 gerrytools-1.0.2/gerrytools/scoring/
--rw-r--r--   0 root         (0) root         (0)     1353 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1539 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/contiguity.py
--rw-r--r--   0 root         (0) root         (0)     1382 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/demographics.py
--rw-r--r--   0 root         (0) root         (0)     5039 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/partisan.py
--rw-r--r--   0 root         (0) root         (0)     1038 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/population.py
--rw-r--r--   0 root         (0) root         (0)     2508 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/reock.py
--rw-r--r--   0 root         (0) root         (0)    24215 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/scores.py
--rw-r--r--   0 root         (0) root         (0)     7058 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/splits.py
--rw-r--r--   0 root         (0) root         (0)      895 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/scoring/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.480437 gerrytools-1.0.2/gerrytools/utilities/
--rw-r--r--   0 root         (0) root         (0)     2986 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/utilities/JSON.py
--rw-r--r--   0 root         (0) root         (0)      192 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1238 2022-07-07 21:54:22.000000 gerrytools-1.0.2/gerrytools/utilities/rename.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 21:54:31.476437 gerrytools-1.0.2/gerrytools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5924 2022-07-07 21:54:31.000000 gerrytools-1.0.2/gerrytools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1634 2022-07-07 21:54:31.000000 gerrytools-1.0.2/gerrytools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-07 21:54:31.000000 gerrytools-1.0.2/gerrytools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      212 2022-07-07 21:54:31.000000 gerrytools-1.0.2/gerrytools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-07 21:54:31.000000 gerrytools-1.0.2/gerrytools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-07 21:54:31.480437 gerrytools-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1129 2022-07-07 21:54:22.000000 gerrytools-1.0.2/setup.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.576531 gerrytools-1.1.0/
+-rw-r--r--   0 pjrule     (501) staff       (20)     1469 2022-12-02 15:49:19.000000 gerrytools-1.1.0/LICENSE
+-rw-r--r--   0 pjrule     (501) staff       (20)       44 2022-12-02 15:49:19.000000 gerrytools-1.1.0/MANIFEST.in
+-rw-r--r--   0 pjrule     (501) staff       (20)     6176 2023-04-28 15:19:53.576336 gerrytools-1.1.0/PKG-INFO
+-rw-r--r--   0 pjrule     (501) staff       (20)     5862 2023-04-28 15:15:18.000000 gerrytools-1.1.0/README.md
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.562779 gerrytools-1.1.0/gerrytools/
+-rw-r--r--   0 pjrule     (501) staff       (20)       46 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/__init__.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.566634 gerrytools-1.1.0/gerrytools/data/
+-rw-r--r--   0 pjrule     (501) staff       (20)    12360 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/AssignmentCompressor.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1629 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/data/URLs.py
+-rw-r--r--   0 pjrule     (501) staff       (20)      760 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/__init__.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    11786 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/acs.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    10384 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/census.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    17386 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/estimatecvap.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     7726 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/fetch.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1563 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/data/geometries.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     3602 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/data/remap.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.568415 gerrytools-1.1.0/gerrytools/geometry/
+-rw-r--r--   0 pjrule     (501) staff       (20)      781 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/__init__.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     4923 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/compactness.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1117 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/dataframe.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     9249 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/dissolve.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1862 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/geometry/dualgraph.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    20337 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/optimize.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2330 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/unitmap.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1302 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/geometry/updater.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.572463 gerrytools-1.1.0/gerrytools/plotting/
+-rw-r--r--   0 pjrule     (501) staff       (20)      961 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/__init__.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     3774 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/annotation.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1732 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/bins.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     4237 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/boxplot.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     4978 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/choropleth.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     3780 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/colors.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1701 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/plotting/districtnumbers.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2721 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/drawgraph.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2352 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/drawplan.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2696 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/gifs.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     3666 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/histogram.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    20106 2022-12-02 15:49:19.000000 gerrytools-1.1.0/gerrytools/plotting/latexcolors.json
+-rw-r--r--   0 pjrule     (501) staff       (20)     2291 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/multidimensional.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2171 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/scatterplot.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     2430 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/sealevel.py
+-rw-r--r--   0 pjrule     (501) staff       (20)      396 2022-12-02 15:49:19.000000 gerrytools-1.1.0/gerrytools/plotting/utils.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     4677 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/plotting/violin.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.574264 gerrytools-1.1.0/gerrytools/scoring/
+-rw-r--r--   0 pjrule     (501) staff       (20)     1589 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/__init__.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1547 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/scoring/contiguity.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1399 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/demographics.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     5406 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/partisan.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1037 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/scoring/population.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    28615 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/scores.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     7151 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/splits.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1012 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/scoring/types.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.575080 gerrytools-1.1.0/gerrytools/utilities/
+-rw-r--r--   0 pjrule     (501) staff       (20)     3026 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/utilities/JSON.py
+-rw-r--r--   0 pjrule     (501) staff       (20)      177 2023-04-28 15:10:56.000000 gerrytools-1.1.0/gerrytools/utilities/__init__.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1238 2023-04-28 15:10:49.000000 gerrytools-1.1.0/gerrytools/utilities/rename.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.563859 gerrytools-1.1.0/gerrytools.egg-info/
+-rw-r--r--   0 pjrule     (501) staff       (20)     6176 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/PKG-INFO
+-rw-r--r--   0 pjrule     (501) staff       (20)     1743 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/SOURCES.txt
+-rw-r--r--   0 pjrule     (501) staff       (20)        1 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/dependency_links.txt
+-rw-r--r--   0 pjrule     (501) staff       (20)      215 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/requires.txt
+-rw-r--r--   0 pjrule     (501) staff       (20)       11 2023-04-28 15:19:53.000000 gerrytools-1.1.0/gerrytools.egg-info/top_level.txt
+-rw-r--r--   0 pjrule     (501) staff       (20)       31 2023-04-28 15:10:19.000000 gerrytools-1.1.0/pyproject.toml
+-rw-r--r--   0 pjrule     (501) staff       (20)       38 2023-04-28 15:19:53.576580 gerrytools-1.1.0/setup.cfg
+-rw-r--r--   0 pjrule     (501) staff       (20)     1105 2023-04-28 15:18:43.000000 gerrytools-1.1.0/setup.py
+drwxr-xr-x   0 pjrule     (501) staff       (20)        0 2023-04-28 15:19:53.576007 gerrytools-1.1.0/tests/
+-rw-r--r--   0 pjrule     (501) staff       (20)    19311 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_data.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     4968 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_geometry.py
+-rw-r--r--   0 pjrule     (501) staff       (20)     1883 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_plotting.py
+-rw-r--r--   0 pjrule     (501) staff       (20)    10529 2023-04-28 15:10:56.000000 gerrytools-1.1.0/tests/test_scoring.py
```

### Comparing `gerrytools-1.0.2/LICENSE` & `gerrytools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gerrytools-1.0.2/PKG-INFO` & `gerrytools-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gerrytools
-Version: 1.0.2
+Version: 1.1.0
 Summary: Tools for processing and visualizing districting plans.
 Home-page: https://github.com/mggg/gerrytools
 Author: MGGG Redistricting Lab
 Author-email: engineering@mggg.org
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
```

### Comparing `gerrytools-1.0.2/README.md` & `gerrytools-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
```

### Comparing `gerrytools-1.0.2/gerrytools/data/AssignmentCompressor.py` & `gerrytools-1.1.0/gerrytools/data/AssignmentCompressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-
-from sortedcontainers import SortedDict, SortedList
 import zlib
 from typing import List
 
+from sortedcontainers import SortedDict, SortedList
+
 
 class AssignmentCompressor:
     """
     A class for compressing and decompressing lots of assignments very, very
-    quickly. Intended for use with ``jsonlines``-like libraries (where assignments
-    are read in line-by-line) or for network requests (where assignments are
-    retrieved one-by-one). When decompressing, yields ``dict``s where keys are
-    in sorted order.
+    quickly. Intended for use with ``jsonlines``-like libraries (where
+    assignments are read in line-by-line) or for network requests (where
+    assignments are retrieved one-by-one). When decompressing, yields ``dict``s
+    where keys are in sorted order.
 
     The compression schema considers the set of unique identifiers, imposes an
-    ordering (lexicographic order) on the identifiers, and matches the assignment
-    to that ordering. We assign all unassigned units to ``"-1"`` and, once the
-    default cache size is hit (or assignments are no longer being read in),
-    compress all assignments in the cache. Assignments are read in and out in
-    the same order, and the keys for each assignment are in the same order.
+    ordering (lexicographic order) on the identifiers, and matches the
+    assignment to that ordering. We assign all unassigned units to ``"-1"``
+    and, once the default cache size is hit (or assignments are no longer being
+    read in), compress all assignments in the cache. Assignments are read in
+    and out in the same order, and the keys for each assignment are in the
+    same order.
 
     Example:
         To compress assignments, we need a set of unique identifiers such that
         each identifier maps one geometric unit to one district.
 
             ...
 
             geoids = blocks["GEOID20"].astype(str)
-            ac = AssignmentCompressor(geoids, location="compressed-assignments.ac")
+            ac = AssignmentCompressor(
+                 geoids, location="compressed-assignments.ac")
 
             with ac as compressor:
                 for assignment in assignments:
                     # Here, ensure that all assignments have string keys and
                     # string values; also ensure that an assignment's keys are
                     # a subset of geoids (or whatever IDs you're passing).
                     compressor.compress(assignment)
@@ -172,16 +174,16 @@
         if not assignment:
             skip = True
             print("`assignment` is empty; skipping.")
 
         if not set(assignment.keys()).issubset(self.identifiers):
             skip = True
             print(
-                "`assignment`'s keys are not a subset of `identifiers`; skipping. " +
-                "Please ensure that all keys and values in `assignment` are strings.",
+                "`assignment`'s keys are not a subset of `identifiers`; skipping. "
+                + "Please ensure that all keys and values in `assignment` are strings.",
             )
 
         # Join the things on the district separator, encode the whole thing, and
         # encode according to the default encoding.
         if not skip:
             indexed = self.match(assignment)
             sep = self.DISTRICT_DELIMITER.decode()
@@ -292,11 +294,13 @@
         # Decompress the chunk and split it on our delimiter.
         decompressed = zlib.decompress(chunk)
         decompressed_parts = decompressed.split(self.ASSIGNMENT_DELIMITER)
 
         # For each of the parts, decode the bytes, make them into lists, and
         # match them to GEOIDs.
         decoded_parts = [part.decode() for part in decompressed_parts]
-        split_parts = [part.split(self.DISTRICT_DELIMITER.decode()) for part in decoded_parts]
+        split_parts = [
+            part.split(self.DISTRICT_DELIMITER.decode()) for part in decoded_parts
+        ]
         indexed_parts = [dict(zip(self.identifiers, part)) for part in split_parts]
 
         return indexed_parts
```

### Comparing `gerrytools-1.0.2/gerrytools/data/URLs.py` & `gerrytools-1.1.0/gerrytools/data/URLs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import us
 
 
 def ids(state):
     """
     URL for accessing districtr identifiers.
```

### Comparing `gerrytools-1.0.2/gerrytools/data/__init__.py` & `gerrytools-1.1.0/gerrytools/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-
 """
 Facilities for processing data and districting plans in a standardized fashion.
 """
-from .acs import cvap, acs5
-from .census import census20, census10, variables
-from .estimatecvap import estimatecvap2010, estimatecvap2020, fetchgeometries
-from .fetch import submissions, tabularized, Submission
-from .remap import remap
-from .URLs import ids, one, csvs
+from .acs import acs5, cvap
 from .AssignmentCompressor import AssignmentCompressor
+from .census import census10, census20, variables
+from .estimatecvap import estimatecvap2010, estimatecvap2020, fetchgeometries
+from .fetch import Submission, submissions, tabularized
 from .geometries import geometries20
+from .remap import remap
+from .URLs import csvs, ids, one
 
 __all__ = [
     "submissions",
     "tabularized",
     "remap",
     "ids",
     "one",
@@ -24,9 +23,9 @@
     "acs5",
     "census20",
     "variables",
     "estimatecvap2010",
     "estimatecvap2020",
     "fetchgeometries",
     "census10",
-    "geometries20"
+    "geometries20",
 ]
```

### Comparing `gerrytools-1.0.2/gerrytools/data/acs.py` & `gerrytools-1.1.0/gerrytools/data/acs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-
-import pandas as pd
-import censusdata
 import io
 from urllib.request import urlopen
 from zipfile import ZipFile
 
+import censusdata
+import pandas as pd
+
 
 def cvap(state, geometry="tract", year=2020) -> pd.DataFrame:
     """
     Retrieves and CSV-formats 5-year CVAP data for the provided state at
-    the specified geometry level. Geometries from the **2010 Census**. Variables
-    and descriptions are [listed here](https://tinyurl.com/3mnrm56s).
+    the specified geometry level. Geometries from the **2010 Census**.
+    Variables and descriptions are [listed here](https://tinyurl.com/3mnrm56s).
 
     Args:
-        state (us.State): The `State` object for which we're retrieving 2019 ACS
-            CVAP Special Tab.
-        geometry (str, optional): Level of geometry for which we're getting data.
-            Accepted values are `"block group"` for 2010 Census Block Groups, and
-            `"tract"` for 2010 Census Tracts. Defaults to `"tract"`.
-        year (int, optional): Year for which data is retrieved. Defaults to 2020.
+        state (us.State): The `State` object for which we're retrieving 2019
+            ACS CVAP Special Tab.
+        geometry (str, optional): Level of geometry for which we're getting
+            data. Accepted values are `"block group"` for 2010 Census Block
+            Groups, and `"tract"` for 2010 Census Tracts. Defaults to `"tract"`.
+        year (int, optional): Year for which data is retrieved. Defaults to
+            2020.
 
     Returns
         A `DataFrame` with a `GEOID` column and corresponding CVAP columns from
         the ACS CVAP Special Tab for the specified year.
     """
     # Maps line numbers to descriptors.
     descriptions = {
@@ -34,87 +35,92 @@
         6: "NHNHPICVAP",
         7: "NHWHITECVAP",
         8: "NHWHITEAMINCVAP",
         9: "NHWHITEASIANCVAP",
         10: "NHWHITEBLACKCVAP",
         11: "NHBLACKAMINCVAP",
         12: "NHOTHCVAP",
-        13: "HCVAP"
+        13: "HCVAP",
     }
 
-    # First, load the raw data requested; allowed geometry values are "block group"
-    # and "tract."
+    # First, load the raw data requested; allowed geometry values are
+    # "block group" and "tract."
     if geometry not in {"block group", "tract"}:
-        print(f"Requested geometry \"{geometry}\" is not allowed; loading tracts.")
+        print(f'Requested geometry "{geometry}" is not allowed; ' "loading tracts.")
         geometry = "tract"
 
     abbrv = geometry if geometry == "tract" else "block group"
 
     # Load the raw data.
     raw = _raw(abbrv, year)
 
     # Create a STATE column for filtering and remove all rows which don't match
     # the state FIPS code.
     raw["GEOID"] = raw["geoid"].str.split("US").str[1]
     raw["STATE"] = raw["GEOID"].str[:2]
     instate = raw[raw["STATE"] == str(state.fips)]
 
-    # Now that we have the in-state data, we aim to pivot the table. Because the
-    # ACS data is in a line-numbered format (i.e. each chunk of 13 lines matches
-    # to an individual geometry, and each of the 13 lines describes an individual
-    # statistic) we need to first collapse each chunk of 13 lines, then build a
-    # dataframe from the resulting collapsed lines. First we send the dataframe
-    # to a list of records.
+    # Now that we have the in-state data, we aim to pivot the table. Because
+    # the ACS data is in a line-numbered format (i.e. each chunk of 13 lines
+    # matches to an individual geometry, and each of the 13 lines describes
+    # an individual statistic) we need to first collapse each chunk of 13
+    # lines, then build a dataframe from the resulting collapsed lines.
+    # First we send the dataframe to a list of records.
     instate_records = instate.to_dict(orient="records")
     collapsed = []
 
     # Get year stuff.
     decade = "10" if year < 2020 else "20"
     yearsuffix = str(year)[2:]
 
     # Next, we collapse these records to a single record.
     for i in range(0, len(instate_records), 13):
         # Create an empty records.
         record = {}
 
         # For each of the records in the block, "collapse" them into a single
         # record.
-        block = instate_records[i:i + 13]
+        block = instate_records[i : i + 13]
         for line in block:
             record[geometry.replace(" ", "").upper() + decade] = line["GEOID"]
             record[descriptions[line["lnnumber"]] + yearsuffix] = line["cvap_est"]
             record[descriptions[line["lnnumber"]] + f"{yearsuffix}e"] = line["cvap_moe"]
 
         collapsed.append(record)
 
     # Create a dataframe and a POCCVAP column; all people minus non-Hispanic
     # White.
     data = pd.DataFrame().from_records(collapsed)
-    data[f"POCCVAP{yearsuffix}"] = data[f"CVAP{yearsuffix}"] - data[f"NHWHITECVAP{yearsuffix}"]
+    data[f"POCCVAP{yearsuffix}"] = (
+        data[f"CVAP{yearsuffix}"] - data[f"NHWHITECVAP{yearsuffix}"]
+    )
 
     return data
 
 
-def acs5(state, geometry="tract", year=2020, columns=[], white="NHWHITEVAP") -> pd.DataFrame:
+def acs5(
+    state, geometry="tract", year=2020, columns=[], white="NHWHITEVAP"
+) -> pd.DataFrame:
     """
     Retrieves ACS 5-year population estimates for the provided state, geometry
-    level, and year. Also retrieves ACS-reported CVAP data, which closely matches
-    that reported by the CVAP special tabulation; CVAP data are only returned at
-    the tract level, and are otherwise reported as 0.
+    level, and year. Also retrieves ACS-reported CVAP data, which closely
+    matches that reported by the CVAP special tabulation; CVAP data are only
+    returned at the tract level, and are otherwise reported as 0.
 
     Args:
         state (us.State): `State` object for the desired state.
         geometry (str, optional): Geometry level at which data is retrieved.
             Acceptable values are `"tract"` and `"block group"`. Defaults to
             `"tract"`, so data is retrieved at the 2020 Census tract level.
-        year (int, optional): Year for which data is retrieved. Defaults to 2020.
+        year (int, optional): Year for which data is retrieved. Defaults to
+            2020.
         columns (list, optional): Columns to retrieve. If `None`, a default set
-            of columns including total populations by race and ethnicity and voting-age
-            populations by race and ethnicity are returned, along with a GEOID
-            column.
+            of columns including total populations by race and ethnicity and
+            voting-age populations by race and ethnicity are returned, along
+            with a GEOID column.
         white (str, optional): The column removed from totals when calculating
             POC populations.
 
     Returns:
         A DataFrame containing the formatted data.
     """
     # Columns for total populations.
@@ -130,93 +136,131 @@
         "B03002_009E": "2MORE" + yearsuffix,
         "B03002_002E": "NHISP" + yearsuffix,
     }
 
     # Create a dictionary of column groups.
     groups = {}
 
-    # Get VAP columns. The columns listed here are by race, irrespective of ethnicity;
-    # for example, WVAP19 is the group of people who identified White as their *only*
-    # race, including people who identified as Hispanic and White.
+    # Get VAP columns. The columns listed here are by race, irrespective of
+    # ethnicity; for example, WVAP19 is the group of people who identified
+    # White as their *only* race, including people who identified as
+    # Hispanic and White.
     vapnames = [
-        "WHITEVAP", "BLACKVAP", "AMINVAP", "ASIANVAP", "NHPIVAP", "OTHVAP", "2MOREVAP",
-        "NHWHITEVAP", "HVAP"
+        "WHITEVAP",
+        "BLACKVAP",
+        "AMINVAP",
+        "ASIANVAP",
+        "NHPIVAP",
+        "OTHVAP",
+        "2MOREVAP",
+        "NHWHITEVAP",
+        "HVAP",
     ]
-    vaptables = list(zip(
-        [column + yearsuffix for column in vapnames],
-        ["A", "B", "C", "D", "E", "F", "G", "H", "I"]
-    ))
-    groups.update({
-        column: _variables(f"B01001{table}", 7, 16) + _variables(f"B01001{table}", 22, 31)
-        for column, table in vaptables
-    })
+    vaptables = list(
+        zip(
+            [column + yearsuffix for column in vapnames],
+            ["A", "B", "C", "D", "E", "F", "G", "H", "I"],
+        )
+    )
+    groups.update(
+        {
+            column: _variables(f"B01001{table}", 7, 16)
+            + _variables(f"B01001{table}", 22, 31)
+            for column, table in vaptables
+        }
+    )
 
-    # Get CVAP columns; the same goes for these columns as does the above, except
-    # these columns are 18 years and older *and* citizens.
+    # Get CVAP columns; the same goes for these columns as does the above,
+    # except these columns are 18 years and older *and* citizens.
     cvapnames = [
-        "WHITECVAP", "BLACKCVAP", "AMINCVAP", "ASIANCVAP", "NHPICVAP", "OTHCVAP",
-        "2MORECVAP", "NHWHITECVAP", "HCVAP"
+        "WHITECVAP",
+        "BLACKCVAP",
+        "AMINCVAP",
+        "ASIANCVAP",
+        "NHPICVAP",
+        "OTHCVAP",
+        "2MORECVAP",
+        "NHWHITECVAP",
+        "HCVAP",
     ]
-    cvaptables = list(zip(
-        [name + yearsuffix for name in cvapnames],
-        ["A", "B", "C", "D", "E", "F", "G", "H", "I"]
-    ))
-    groups.update({
-        column:
-            _variables(f"B05003{table}", 9, 9) + _variables(f"B05003{table}", 11, 11) +  # men
-            _variables(f"B05003{table}", 20, 20) + _variables(f"B05003{table}", 22, 22)  # women
-        for column, table in cvaptables
-    })
+    cvaptables = list(
+        zip(
+            [name + yearsuffix for name in cvapnames],
+            ["A", "B", "C", "D", "E", "F", "G", "H", "I"],
+        )
+    )
+    groups.update(
+        {
+            column: _variables(f"B05003{table}", 9, 9)
+            + _variables(f"B05003{table}", 11, 11)
+            + _variables(f"B05003{table}", 20, 20)  # men
+            + _variables(f"B05003{table}", 22, 22)  # women
+            for column, table in cvaptables
+        }
+    )
 
     # Get all voting-age people and citizen voting-age people.
-    groups["VAP" + yearsuffix] = _variables("B01001", 7, 25) + _variables("B01001", 31, 49)
-    groups["CVAP" + yearsuffix] = _variables("B05003", 9, 9) + \
-        _variables("B05003", 11, 11) + \
-        _variables("B05003", 20, 20) + \
-        _variables("B05003", 22, 22)
+    groups["VAP" + yearsuffix] = _variables("B01001", 7, 25) + _variables(
+        "B01001", 31, 49
+    )
+    groups["CVAP" + yearsuffix] = (
+        _variables("B05003", 9, 9)
+        + _variables("B05003", 11, 11)
+        + _variables("B05003", 20, 20)
+        + _variables("B05003", 22, 22)
+    )
 
     # TODO: all variables used across the data submodule should be packaged up
     # as a class, so we can access individual dictionaries of variables to add.
-    # For example, we should have a `Variables.acs5.vap` property which gives us
-    # the voting-age population variables for the ACS 5-year estimates.
+    # For example, we should have a `Variables.acs5.vap` property which gives
+    # us the voting-age population variables for the ACS 5-year estimates.
 
     # Get the list of all columns.
-    allcols = list(popcolumns.keys()) + [c for k in groups.values() for c in k] + columns
+    allcols = (
+        list(popcolumns.keys()) + [c for k in groups.values() for c in k] + columns
+    )
 
     # Retrieve the data from the Census API.
     data = censusdata.download(
-        "acs5", year,
+        "acs5",
+        year,
         censusdata.censusgeo(
             [("state", str(state.fips).zfill(2)), ("county", "*"), (geometry, "*")]
         ),
-        ["GEO_ID"] + allcols
+        ["GEO_ID"] + allcols,
     )
 
     # Rework columns.
     data = data.reset_index(drop=True)
     data["GEO_ID"] = data["GEO_ID"].str.split("US").str[1]
-    data = data.rename({"GEO_ID": geometry.replace(" ", "").upper() + ("10" if year < 2020 else "20")}, axis=1)
+    data = data.rename(
+        {"GEO_ID": geometry.replace(" ", "").upper() + ("10" if year < 2020 else "20")},
+        axis=1,
+    )
     data = data.rename(popcolumns, axis=1)
 
     # Collapse column groups.
     for column, group in groups.items():
         data[column] = data[group].sum(axis=1)
         data = data.drop(group, axis=1)
 
     # Create a POCVAP column.
-    data["POCVAP" + yearsuffix] = data["VAP" + yearsuffix] - data[white + yearsuffix]
+    data[f"POCVAP{yearsuffix}"] = (
+        data[f"VAP{yearsuffix}"] - data[f"{white}{yearsuffix}"]
+    )
     return data
 
 
 def _variables(prefix, start, stop, suffix="E") -> list:
     """
     Returns the ACS variable names from the provided prefix, start, stop, and
     suffix parameters. Used to generate batches of names, especially for things
     like voting-age population. Variable names are formatted like
-    `<prefix>_<number identifier><suffix>`, where `<prefix>` is a population grouping,
+    `<prefix>_<number identifier><suffix>`, where `<prefix>` is a
+    population grouping,
     `<number identifier>` is the number of the variable in that grouping, and
     `<suffix>` designates the file used. [Variables are listed
     here ](https://tinyurl.com/43ajptky>).
 
     Args:
         prefix (str): Population grouping; typically "B01001." These prefixes
             change based on subpopulation: for example, the prefix for Black
@@ -225,18 +269,15 @@
         start (int): Where to start numbering.
         stop (int): Where to stop numbering. Inclusive.
         suffix (str): Suffix designating the file. For most purposes, this is "E."
 
     Returns:
         A list of ACS5 variable names.
     """
-    return [
-        f"{prefix}_{str(t).zfill(3)}{suffix}"
-        for t in range(start, stop + 1)
-    ]
+    return [f"{prefix}_{str(t).zfill(3)}{suffix}" for t in range(start, stop + 1)]
 
 
 def _retrieve(year, geometry="tract"):
     """
     Downloads and extracts compressed CVAP data for the specified year.
 
     Args:
@@ -270,19 +311,21 @@
 
 
 def _raw(geometry, year) -> pd.DataFrame:
     """
     Reads raw CVAP data from the local repository.
 
     Args:
-        geometry (str): Level of geometry for which we're getting 2019 CVAP data.
+        geometry (str): Level of geometry for which we're getting 2019 CVAP
+            data.
         year (int): Year for which data is retrieved.
 
     Returns:
         A DataFrame, where each block of 13 rows corresponds to an individual
-        geometric unit (2010 Census Block Group, 2010 Census Tract) and each row
-        in a given block corresponds to a CVAP statistic for that block's
-        geometric unit.
+        geometric unit (2010 Census Block Group, 2010 Census Tract) and
+        each row in a given block corresponds to a CVAP statistic for that
+        block's geometric unit.
+
     """
     # Retrieve the data at the specified geometry level and return
     # it as a dataframe.
     return pd.read_csv(io.StringIO(_retrieve(year, geometry)), encoding="ISO-8859-1")
```

### Comparing `gerrytools-1.0.2/gerrytools/data/census.py` & `gerrytools-1.1.0/gerrytools/data/census.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,131 @@
+from functools import reduce
+from itertools import combinations
+from typing import Iterable
 
+import censusdata
 import pandas as pd
 import requests
-import censusdata
-from itertools import combinations
-from functools import reduce
-from typing import Iterable
 
 
 def _rjoin(df, columns) -> Iterable:
     """
     Private method for elementwise concatenating string dataframe columns.
 
     Args:
         df (pd.DataFrame): DataFrame to which the columns belong.
-        columns (list): List of column names to be concatenated in left-to-right
-            order.
+        columns (list): List of column names to be concatenated in
+            left-to-right order.
 
     Returns:
         An iterable representing the column of concatenated column entries.
     """
     stringified = [df[c].astype(str) for c in columns]
-    return reduce(lambda l, r: l + r, stringified[1:], stringified[0])
+    return reduce(lambda left, right: left + right, stringified[1:], stringified[0])
 
 
-def census10(state, columns={}, geometry="block"):
+def census10(state, table="P8", columns={}, geometry="block"):
     """
     Retrieves `geometry`-level 2010 Summary File 1 data via the Census API.
 
     Args:
         state (State): `us.State` object (e.g. `us.states.WI`).
-        columns (dict, optional): Dictionary which maps Census column names (from
-            the correct table) to human-readable names. We require this to be a
-            dictionary, _not_ a list, as specifying human-readable names will
-            implicitly protect against incorrect column names and excessive API
-            calls.
+        table (string, optional): Table from which we retrieve data.
+           Defaults to the P8 table, which contains population by race
+           regardless of ethnicity.
+        columns (dict, optional): Dictionary which maps Census column names
+            (from the correct table) to human-readable names. We require this
+            to be a dictionary, _not_ a list, as specifying human-readable
+            names will implicitly protect against incorrect column names
+            and excessive API calls.
         geometry (string, optional): Geometry level at which we retrieve data.
             Defaults to `"block"` to retrieve block-level data for the state
-            provided. Accepted values are `"block"`, `"block group`", and `"tract"`.
+            provided. Accepted values are `"block"`, `"block group`", and
+            `"tract"`.
 
     Returns:
         A DataFrame with columns renamed according to their Census description
         designation and a unique identifier column for joining to geometries.
     """
+    # Check whether the geometry is right. If not, warn the user and set it
+    # properly.
+    if geometry not in {"block", "tract", "block group"}:
+        raise ValueError(f'Geometry "{geometry}" not accepted.')
+
+    # Check whether we're providing an appropriate table name.
+    if table not in {"P8", "P9", "P10", "P11"}:
+        raise ValueError(f'Unknown table "{table}".')
+
     # Create the right geometry identifiers.
     geometries = [("state", str(state.fips)), ("county", "*"), ("tract", "*")]
     if geometry in {"block group", "block"}:
         geometries += [(geometry, "*")]
 
     # Create an identifier column.
     identifier = geometry.replace(" ", "").upper() + "10"
 
+    varmap = columns if columns else variables(table)
+    vars = list(varmap.keys())
     # Download data.
     raw = censusdata.download(
-        "sf1", 2010, censusdata.censusgeo(geometries),
-        ["GEO_ID"] + list(columns.keys()),
+        "sf1",
+        2010,
+        censusdata.censusgeo(geometries),
+        ["GEO_ID"] + vars,
     )
 
     # Rename columns and send back to the caller!
     raw = raw.rename({"GEO_ID": identifier, **columns}, axis=1)
     raw[identifier] = raw[identifier].str[9:]
     clean = raw.reset_index(drop=True)
 
+    clean = clean.rename(varmap, axis=1)
     return clean
 
 
 def census20(
-    state, table="P1", columns={}, geometry="block",
-    key="75c0c07e6f0ab7b0a9a1c14c3d8af9d9f13b3d65"
+    state,
+    table="P1",
+    columns={},
+    geometry="block",
+    key="75c0c07e6f0ab7b0a9a1c14c3d8af9d9f13b3d65",
 ) -> pd.DataFrame:
     """
-    Retrieves `geometry`-level 2020 Decennial Census PL94-171 data via the Census
-    API.
+    Retrieves `geometry`-level 2020 Decennial Census PL94-171 data via the
+    Census API.
 
     Args:
         state (State): `us.State` object (e.g. `us.states.WI`).
-        table (string, optional): Table from which we retrieve data. Defaults to
-            the P1 table, which gets populations by race regardless of ethnicity.
-        columns (dict, optional): Dictionary which maps Census column names (from
-            the correct table) to human-readable names. We require this to be a
-            dictionary, _not_ a list, as specifying human-readable names will
-            implicitly protect against incorrect column names and excessive API
-            calls.
+        table (string, optional): Table from which we retrieve data.
+            Defaults to the P1 table, which gets populations by race
+            regardless of ethnicity.
+        columns (dict, optional): Dictionary which maps Census column names
+            (from the correct table) to human-readable names. We require this
+            to be a dictionary, _not_ a list, as specifying human-readable
+            names will implicitly protect against incorrect column names and
+            excessive API calls.
         geometry (string, optional): Geometry level at which we retrieve data.
             Defaults to `"block"` to retrieve block-level data for the state
-            provided. Accepted values are `"block"`, `"block group`", and `"tract"`.
+            provided. Accepted values are `"block"`, `"block group`",
+            and `"tract"`.
         key (string, optional): Census API key.
 
     Returns:
         A DataFrame with columns renamed according to their Census description
         designation and a `GEOID20` column for joining to geometries.
     """
     # Check whether the geometry is right. If not, warn the user and set it
     # properly.
     if geometry not in {"block", "tract", "block group"}:
-        print(f"Geometry \"{geometry}\" not accepted; defaulting to \"block\".")
+        print(f'Geometry "{geometry}" not accepted; defaulting' 'to "block".')
         geometry = "block"
 
     # Check whether we're providing an appropriate table name.
     if table not in {"P1", "P2", "P3", "P4"}:
-        print(f"Table \"{table}\" not accepted; defaulting to \"P1.\"")
+        print(f'Table "{table}" not accepted; defaulting to "P1."')
         table = "P1"
 
     # Set the base Census API URL and get the keys for the provided table.
     base = "https://api.census.gov/data/2020/dec/pl"
     varmap = columns if columns else variables(table)
     vars = list(varmap.keys())
 
@@ -137,90 +160,106 @@
         tail = ["state", "county", "tract"] + last
 
         # Create an unescaped query string.
         unescaped = q.copy()
         unescaped.append(("get", ",".join(varchunk)))
 
         # Create an escaped query string from the previous.
-        escaped = "?" + "&".join(
-            f"{param}={value}" for param, value in unescaped
-        )
+        escaped = "?" + "&".join(f"{param}={value}" for param, value in unescaped)
 
         # Send the request and create a dataframe.
         req = requests.get(base + escaped).json()
         header, data = req[0], req[1:]
         chunk = pd.DataFrame(data, columns=header)
 
         # Get a GEOID column and drop old columns.
         chunk["GEOID20"] = _rjoin(chunk[tail], tail)
         chunk = chunk.drop(tail, axis=1)
         mergeable.append(chunk)
 
-    # Merge the dataframes, rename everything, make the columns ints, and return.
-    merged = reduce(lambda l, r: pd.merge(l, r, on="GEOID20"), mergeable)
+    # Merge the dataframes, rename everything, make the columns
+    # ints, and return.
+    merged = reduce(lambda left, right: pd.merge(left, right, on="GEOID20"), mergeable)
     merged = merged.rename(varmap, axis=1)
     merged = merged.astype({var: int for var in varmap.values()})
 
     # Make the GEOID20 column the first column.
     merged = merged[["GEOID20"] + list(varmap.values())]
 
     return merged
 
 
 def variables(table) -> dict:
     """
     Produces variable names for the 2020 Census PL94-171 tables. Variables are
-    determined from patterns apparent in PL94 variable [lists for tables P1 through
-    P4](https://tinyurl.com/2s3btptn).
+    determined from patterns apparent in PL94 variable
+    [lists for tables P1 through P4](https://tinyurl.com/2s3btptn).
 
     Args:
         table (string): The table for which we're generating variables.
 
     Returns:
         A dictionary mapping Census variable codes to human-readable ones.
     """
     # List the categories of Census variables and find the combinations in the
-    # correct order. This *should* be the original order in which they're listed,
-    # but these have been spot-checked to verify their correctness. These names
-    # are also modified based on the table passed; for example, if the table
-    # passed is P2 or P4, we prepend an "NH" to the beginning, as these columns
-    # are explicitly non-hispanic people. If the table passed is P3 or P4, we
-    # append a "VAP" to the end to signify these are people of voting age;
-    # otherwise, we add "POP."
+    # correct order. This *should* be the original order in which they're
+    # listed, but these have been spot-checked to verify their correctness.
+    # These names are also modified based on the table passed; for example,
+    # if the table passed is P2 or P4, we prepend an "NH" to the beginning,
+    # as these columns are explicitly non-hispanic people. If the table
+    # passed is P3 or P4, we append a "VAP" to the end to signify these
+    # are people of voting age; otherwise, we add "POP."
     categories = ["WHITE", "BLACK", "AMIN", "ASIAN", "NHPI", "OTH"]
-    prefix = "NH" if table in {"P2", "P4"} else ""
-    suffix = "VAP" if table in {"P3", "P4"} else "POP"
-    combos = list(pd.core.common.flatten(
-        [
-            prefix + "".join(list(combo)) + suffix + "20"
-            for i in range(1, len(categories) + 1)
-            for combo in list(combinations(categories, i))
-        ]
-    ))
+    prefix = "NH" if table in {"P2", "P4", "P9", "P11"} else ""
+    suffix = "VAP" if table in {"P3", "P4", "P10", "P11"} else "POP"
+    year_suff = "20" if table in {"P1", "P2", "P3", "P4"} else "10"
+    combos = list(
+        pd.core.common.flatten(
+            [
+                prefix + "".join(list(combo)) + suffix + year_suff
+                for i in range(1, len(categories) + 1)
+                for combo in list(combinations(categories, i))
+            ]
+        )
+    )
 
-    # Now, for each of the combinations, we map the appropriate variable name to
-    # the descriptor. Each of these tranches should have a width of 6 choose i,
-    # where i is the number of categories in the combination. For example, the
-    # second tranch (from 13 to 27) has width 15, as 6C2=15.
-    if table in {"P1", "P3"}:
+    # Now, for each of the combinations, we map the appropriate variable
+    # name to the descriptor. Each of these tranches should have a width
+    # of 6 choose i, where i is the number of categories in the
+    # combination. For example, the second tranch (from 13 to 27) has
+    # width 15, as 6C2=15.
+    if table in {"P1", "P3", "P8", "P10"}:
         tranches = [(3, 8), (11, 25), (27, 46), (48, 62), (64, 69), (71, 71)]
     else:
         tranches = [(5, 10), (13, 27), (29, 48), (50, 64), (66, 71), (73, 73)]
 
     # Create variable numbers.
     numbers = list(pd.core.common.flatten([list(range(i, j + 1)) for i, j in tranches]))
 
     # Edit these for specific tables. For example, in tables P2 and P3, we want
     # to get the total Hispanic population and the total population.
-    if table in {"P2", "P4"}:
+    if table in {"P2", "P4", "P9", "P11"}:
         numbers = [1, 2] + numbers
-        hcol = "HVAP20" if table == "P4" else "HPOP20"
-        tcol = "VAP20" if table == "P4" else "TOTPOP20"
+        if table in {"P4", "P11"}:
+            hcol = f"HVAP{year_suff}"
+            tcol = f"VAP{year_suff}"
+        else:
+            hcol = f"HPOP{year_suff}"
+            tcol = f"TOTPOP{year_suff}"
         combos = [tcol, hcol] + combos
     else:
         numbers = [1] + numbers
-        tcol = "VAP20" if table in {"P3", "P4"} else "TOTPOP20"
+        if table in {"P3", "P4", "P10", "P11"}:
+            tcol = f"VAP{year_suff}"
+        else:
+            tcol = f"TOTPOP{year_suff}"
         combos = [tcol] + combos
 
-    # Create the variable names and zip the names together with the combinations.
-    names = [f"{table}_{str(n).zfill(3)}N" for n in numbers]
+    # Create the variable names and zip the names together
+    # with the combinations.
+    if year_suff == "20":
+        names = [f"{table}_{str(n).zfill(3)}N" for n in numbers]
+    else:
+        names = [
+            f"P{str(table.split('P')[-1]).zfill(3)}{str(n).zfill(3)}" for n in numbers
+        ]
     return dict(zip(names, combos))
```

### Comparing `gerrytools-1.0.2/gerrytools/data/estimatecvap.py` & `gerrytools-1.1.0/gerrytools/data/estimatecvap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-
-import pandas as pd
 import geopandas as gpd
 import numpy as np
+import pandas as pd
 from pandas import DataFrame
+
+from ..geometry import unitmap
 from .acs import acs5, cvap
 from .census import census20
-from ..geometry import unitmap
 
 
 def estimatecvap2020(state) -> pd.DataFrame:
     """
-    Estimates 2020 CVAP on 2020 blocks using 2020 PL94 data. **This method serves
-    a different purpose than `gerrytools.data.estimatecvap.estimatecvap2010()`:**
-    rather than using geometric procedures to put CVAP data on old geometries,
-    this method takes advantage of the Census's geographic hierarchy, and
-    associates finer-grained 2020 CVAP data with 2020 blocks. _No geometric
-    data or procedures are used here_. The resulting data can then be adjoined
-    to 2020 block geometries (or assigned to VTDs, assigned to districts, etc.)
-    and be used to build other units of varying size.
+    Estimates 2020 CVAP on 2020 blocks using 2020 PL94 data. **This method
+    serves a different purpose than `gerrytools.data.estimatecvap.
+    estimatecvap2010()`:** rather than using geometric procedures to
+    put CVAP data on old geometries, this method takes advantage of the
+    Census's geographic hierarchy, and associates finer-grained 2020 CVAP
+    data with 2020 blocks. _No geometric data or procedures are used here_.
+    The resulting data can then be adjoined to 2020 block geometries (or
+    assigned to VTDs, assigned to districts, etc.) and be used to build
+    other units of varying size.
 
     Args:
         state (State): The `us.State` for which CVAP will be estimated.
 
     Returns:
-        A `DataFrame` of combined Census and ACS data at the Census block level.
+        A `DataFrame` of combined Census and ACS data at the Census
+        block level.
     """
 
     # First, get the Census data for blocks and block groups.
     bg = census20(state, table="P4", geometry="block group")
     block = census20(state, table="P4", geometry="block")
 
-    # Now, get 2020 Census data at the block group level and merging it with the
-    # block group-level Census data.
+    # Now, get 2020 Census data at the block group level and merging it
+    # with the block group-level Census data.
     cvap20 = cvap(state, geometry="block group", year=2020)
     bg = bg.merge(cvap20, left_on="GEOID20", right_on="BLOCKGROUP20")
 
     # Name the VAP columns.
     vapcolumns = [
-        "NHWHITEVAP20", "NHASIANVAP20", "NHBLACKVAP20", "NHNHPIVAP20", "NHAMINVAP20",
-        "NHWHITEASIANVAP20", "NHWHITEAMINVAP20", "NHWHITEBLACKVAP20", "NHBLACKAMINVAP20"
+        "NHWHITEVAP20",
+        "NHASIANVAP20",
+        "NHBLACKVAP20",
+        "NHNHPIVAP20",
+        "NHAMINVAP20",
+        "NHWHITEASIANVAP20",
+        "NHWHITEAMINVAP20",
+        "NHWHITEBLACKVAP20",
+        "NHBLACKAMINVAP20",
     ]
 
     # Create "remainder" column.
     for universe in [block, bg]:
         universe["NHVAP20"] = universe["VAP20"] - universe["HVAP20"]
         universe["OTHVAP20"] = universe["NHVAP20"] - universe[vapcolumns].sum(axis=1)
 
@@ -69,29 +78,33 @@
         block[colpct] = block[vapcolumn] / block[colpct]
 
         # Create a mapping from block group IDs to CVAP groups.
         cvapcolumn = vapcolumn.replace("VAP", "CVAP")
         cvapmap = dict(zip(bg["BLOCKGROUP20"].astype(str), bg[cvapcolumn]))
 
         # Create two temporary columns: the first sets the block's CVAP to the
-        # total CVAP for its block group; the second sets the block's VAP to the
-        # total VAP for its block group. (Note: each of these C/VAP columns are
-        # with respect to the current VAP column.)
+        # total CVAP for its block group; the second sets the block's VAP
+        # to the total VAP for its block group. (Note: each of these C/VAP
+        # columns are with respect to the current VAP column.)
         block["tmp"] = block["BLOCKGROUP20"].map(cvapmap)
         block["BGVAP20"] = block["BLOCKGROUP20"].map(bgtotalvapmap)
 
-        # Next, compute the estimated CVAP by multiplying the VAP column percent
-        # for the block group by the total CVAP population of the block group.
+        # Next, compute the estimated CVAP by multiplying the VAP column
+        # percent for the block group by the total CVAP population of the
+        # block group.
         block[cvapcolumn] = block[colpct] * block["tmp"]
 
-        # If the above doesn't work — which is the case if the VAP column percent
-        # is NaN (0/0) or inf (k/0), we estimate the CVAP of the block using the
-        # VAP ratio outright rather than the column-specific VAP ratio.
+        # If the above doesn't work — which is the case if the VAP column
+        # percent is NaN (0/0) or inf (k/0), we estimate the CVAP of the
+        # block using the VAP ratio outright rather than the column-specific
+        # VAP ratio.
         ni = block[block[colpct].isna()].index
-        block.loc[ni, cvapcolumn] = (block.loc[ni, "VAP20"] / block.loc[ni, "BGVAP20"]) * block.loc[ni, "tmp"]
+        block.loc[ni, cvapcolumn] = (
+            block.loc[ni, "VAP20"] / block.loc[ni, "BGVAP20"]
+        ) * block.loc[ni, "tmp"]
 
         # Assert that our summed disaggregated numbers and totals are close!
         assert np.isclose(bg[cvapcolumn].sum() - block[cvapcolumn].sum(), 0)
 
     # Fill NaNs with 0 and drop unnecessary columns.
     block = block.fillna(0)
     block = block.drop(["tmp", "BGVAP20"], axis=1)
@@ -108,16 +121,16 @@
         state (State): The `us.State` for which CVAP will be estimated.
         geometry10 (str): Level of geometry we're fetching. Accepted values are
             `"tract"` and `"block group"`.
 
     Returns:
         A `GeoDataFrame` of 2010 geometries.
     """
-    # Get a Census locator for the provided State by replacing spaces in its name
-    # with underscores (should they exist).
+    # Get a Census locator for the provided State by replacing spaces in its
+    # name with underscores (should they exist).
     clocator = state.name.replace(" ", "_")
 
     # Validate geometry level indicators.
     if geometry not in {"block group", "tract", "block"}:
         raise ValueError(f"Geometry level {geometry} not supported; aborting.")
 
     if geometry == "block group":
@@ -133,16 +146,16 @@
 
     # Download, extract, and return the geometries from the URL.
     return gpd.read_file(url)
 
 
 def mapbase(base, state, geometry, baseindex="GEOID20"):
     """
-    Maps the provided geometries in `base` to the 2010 Census geometries specified
-    by `geometry`.
+    Maps the provided geometries in `base` to the 2010 Census geometries
+    specified by `geometry`.
 
     Args:
         base (GeoDataFrame): GeoDataFrame with the desired units for cvap to be
             estimated on.
         state (State): The `us.State` for which CVAP will be estimated.
         geometry (str): Level of geometry we're fetching. Accepted values are
             `"tract"` and `"block group"`.
@@ -153,41 +166,41 @@
     # Get the 2010 geometries from the Census.
     geometry10 = fetchgeometries(state, geometry)
 
     # Get the right name and rename the 2010 geometry index this way.
     geometry10id = "TRACT10" if geometry == "tract" else "BLOCKGROUP10"
     geometry10 = geometry10.rename({"GEOID10": geometry10id}, axis=1)
 
-    # Create a unit mapping from the provided base units to those retrieved from
-    # the Census. If the `base` passed has been sliced or could possibly be a
-    # copy, *this will throw a SettingWithCopy warning*.
+    # Create a unit mapping from the provided base units to those retrieved
+    # from the Census. If the `base` passed has been sliced or could possibly
+    # be a copy, *this will throw a SettingWithCopy warning*.
     mapping = unitmap((base, baseindex), (geometry10, geometry10id))
     base[geometry10id] = base[baseindex].map(mapping)
 
     return base
 
 
 def estimatecvap2010(
     base, state, groups, ceiling, zfill, geometry10="tract", year=2019
 ) -> DataFrame:
     r"""
-    Function for turning old (2019) CVAP data on 2010 geometries into estimates
-    for current CVAP data on 2020 geometries. **This method serves a different
-    purpose than `gerrytools.data.estimatecvap.estimatecvap2020()`:** this method
-    is intended to put 2010-era CVAP data on 2020-era geometries, and uses
-    geometric properties to do so.
+    Function for turning old (2019) CVAP data on 2010 geometries into
+    estimates for current CVAP data on 2020 geometries. **This method
+    serves a different purpose than `gerrytools.data.estimatecvap.
+    estimatecvap2020()`:** this method is intended to put 2010-era CVAP
+    data on 2020-era geometries, and uses geometric properties to do so.
 
     Users must supply a base `GeoDataFrame`
     representing their chosen U.S. state. Additionally, users must specify the
-    demographic groups whose CVAP statistics are to be estimated. For each group,
-    users specify a triple \((X, Y, Z)\) where \(X\) is the old CVAP column for
-    that group, \(Y\) is the old VAP column for that group, and \(Z\) is the new VAP
-    column for that group, which must be an existing column on `base`.  Then,
-    the estimated new CVAP for that group will be constructed by multiplying
-    \((X / Y) \cdot Z\) for each new geometry.
+    demographic groups whose CVAP statistics are to be estimated. For each
+    group, users specify a triple \((X, Y, Z)\) where \(X\) is the old CVAP
+    column for that group, \(Y\) is the old VAP column for that group, and
+    \(Z\) is the new VAP column for that group, which must be an existing
+    column on `base`. Then, the estimated new CVAP for that group will be
+    constructed by multiplying \((X / Y) \cdot Z\) for each new geometry.
 
     <div style="text-align: center;">
         </br>
         <img width="75%" src="../images/cvap-estimation.png"/>
     </div>
 
     Args:
@@ -197,106 +210,116 @@
         groups (list): `(X, Y, Z)` triples for each desired CVAP group to be
             estimated, where each of the parameters are column names: `X` is
             the column on the 2010 geometries which contains the relevant CVAP
             data; `Y` is the column on the 2010 geometries which contains the
             relevant VAP data; `Z` is the column on the 2020 geometries to be
             weighted by the ratio of the per-unit ratios in `X` and `Y`. For
             example, if we wish to estimate Black CVAP, this triple would be
-            `(NHBCVAP19, BVAP19, BVAP20)`, which takes the ratios of the `NHBCVAP19`
-            and `BVAP19` columns on the 2010 geometries, and multplies the 2020
-            geometries' respective `BVAP20` values by these ratios.
-        ceiling (float): Number representing where to cap the weighting ratio of
-            CVAP to VAP20. After this percentage ceiling is passed, the percentage
-            will be set to 1. We recommend setting this to 1.
-        zfill (float): Fill in ratio for CVAP to VAP20 when there is 0 CVAP in the
-            area. We recommend setting this parameter to `0.1`.
-        geometry10 (str, optional): The 2010 geometry on which cvap will be pulled.
-            Acceptable values are `"tract"` or `"block group"`. As tracts are
-            less susceptible to change across Census vintages, setting this parameter
-            to `"tract"` is recommended, as it is more likely that the 2020 Census
-            blocks fit neatly into the 2010 Census tracts.
+            `(NHBCVAP19, BVAP19, BVAP20)`, which takes the ratios of the
+            `NHBCVAP19` and `BVAP19` columns on the 2010 geometries, and
+            multplies the 2020 geometries' respective `BVAP20` values
+            by these ratios.
+        ceiling (float): Number representing where to cap the weighting
+            ratio of CVAP to VAP20. After this percentage ceiling is
+            passed, the percentage will be set to 1. We recommend
+            setting this to 1.
+        zfill (float): Fill in ratio for CVAP to VAP20 when there is 0 CVAP
+            in the area. We recommend setting this parameter to `0.1`.
+        geometry10 (str, optional): The 2010 geometry on which cvap will
+            be pulled. Acceptable values are `"tract"` or `"block group"`.
+            As tracts are less susceptible to change across Census vintages,
+            setting this parameter to `"tract"` is recommended, as it is
+            more likely that the 2020 Census blocks fit neatly into the
+            2010 Census tracts.
 
     Returns:
        `base` geometries with 2019 CVAP-weighted 2020 CVAP estimates attached.
     """
     if geometry10 not in {"block group", "tract"}:
-        print(f"Requested geometry \"{geometry10}\" is not allowed; loading tracts.")
+        print(f'Requested geometry "{geometry10}" is not allowed; ' "loading tracts.")
         geometry10 = "tract"
 
     # Grab ACS and CVAP special-tab data, and make sure our triples are correct
     cvap_geoid = "TRACT10" if geometry10 == "tract" else "BLOCKGROUP10"
     acs_source = acs5(state, geometry10, year=year)
     cvap_source = cvap(state, geometry10, year=year)
 
     # Validate the columns passed, issuing user warnings when it's inadvisable
     # to estimate CVAP given the passed columns.
-    for (cvap10, vap10, vap20) in groups:
-        # If any of the CVAP columns passed correspond to columns which tabulate
-        # people of multiple races, notify the user that there isn't an appropriate
-        # 2019 VAP column to match them against.
+    for cvap10, vap10, vap20 in groups:
+        # If any of the CVAP columns passed correspond to columns which
+        # tabulate people of multiple races, notify the user that there
+        # isn't an appropriate 2019 VAP column to match them against.
         if any(substring in cvap10 for substring in {"AIW", "AW", "BW", "AIB"}):
             print(
-                f"Warning: Estimating CVAP among {cvap10} is not advisable, since "
-                "there isn't a reasonable VAP column from which to construct _CVAP "
-                "/ _VAP rates (because you seem to be combining two racial groups)."
+                f"Warning: Estimating CVAP among {cvap10} is not advisable, "
+                "since there isn't a reasonable VAP column from which to "
+                "construct _CVAP / _VAP rates (because you seem to be "
+                "combining two racial groups)."
             )
 
-        # If the CVAP or ACS5 columns passed aren't present in the set of possible
-        # columns, raise an error.
+        # If the CVAP or ACS5 columns passed aren't present in the
+        # set of possible columns, raise an error.
         if not (cvap10 in acs_source or cvap10 in cvap_source):
             possible_columns = set(acs_source).union(set(cvap_source))
             raise ValueError(
-                f"Your CVAP column '{cvap10}' must be contained in either the ACS "
-                f"or Special Tab columns: {possible_columns}"
+                f"Your CVAP column '{cvap10}' must be contained in either "
+                f"the ACS or Special Tab columns: {possible_columns}"
             )
 
         if vap10 not in acs_source:
             raise ValueError(
                 f"Your old VAP column '{vap10}' must be contained in the ACS "
                 "columns: {set(acs_source)}"
             )
 
-        # If the VAP20 column passed doesn't exist on the user-provided geometries,
-        # raise an error.
+        # If the VAP20 column passed doesn't exist on the user-provided
+        # geometries, raise an error.
         if vap20 not in base:
             raise ValueError(
-                f"Your new VAP column '{vap20}' must be contained in your base " +
-                f"dataframe: {set(base)}"
+                f"Your new VAP column '{vap20}' must be contained in your "
+                f"base dataframe: {set(base)}"
             )
 
     # Remove ACS 5 columns that overlap with special-tab ones.
     non_overlaps = list(set(acs_source).difference(set(cvap_source)))
     acs_source = acs_source[[cvap_geoid] + non_overlaps]
     source = cvap_source.merge(acs_source, on=cvap_geoid)
 
-    # Get the right columns from the base geometry, and map the base geometries
-    # to the units with CVAP data. Apparently dropping bad columns by using slicing
-    # incudes a SettingWithCopy warning, so we're just dropping using .drop()
-    # instead.
-    correct = ["geometry"] + [col for col in list(base) if any(sub in col for sub in ["POP", "VAP", "GEOID"])]
+    # Get the right columns from the base geometry, and map the base
+    # geometries to the units with CVAP data. Apparently dropping bad
+    # columns by using slicing incudes a SettingWithCopy warning, so
+    # we're just dropping using .drop() instead.
+    correct = ["geometry"] + [
+        col for col in list(base) if any(sub in col for sub in ["POP", "VAP", "GEOID"])
+    ]
     bads = list(set(base) - set(correct))
 
     # Warn the user of column removal:
     print("Removing the following columns: " + ", ".join(bads))
 
     pared = base.drop(bads, axis=1)
     pared = mapbase(pared, state, geometry10)
 
     # Compute weights.
-    for (cvap10, vap10, _) in groups:
+    for cvap10, vap10, _ in groups:
         source[cvap10 + "%"] = source[cvap10] / source[vap10]
 
     # Fill in values according to the following rules:
     #
-    #   1.  if there are 0 *CVAP reported and 0 *VAP reported, we set the weight to
-    #       the average *CVAP/*VAP ratio within the county;
-    #   2.  if there are 0 *CVAP reported and *VAP > 0, we set the weight to zero_fill;
-    #   3.  if *CVAP > 0 but *VAP = 0 or *CVAP/*VAP > percentage_cap, we set the weight to 1.
+    #   1.  if there are 0 *CVAP reported and 0 *VAP reported, we set the
+    #        weight to the average *CVAP/*VAP ratio within the county;
+    #   2.  if there are 0 *CVAP reported and *VAP > 0, we set the weight to
+    #        zero_fill;
+    #   3.  if *CVAP > 0 but *VAP = 0 or *CVAP/*VAP > percentage_cap, we set
+    #       the weight to 1.
     statewide = {
-        cvap + "%": source[cvap].sum() / source[vap].sum() if source[vap].sum() != 0 else 0
+        cvap + "%": source[cvap].sum() / source[vap].sum()
+        if source[vap].sum() != 0
+        else 0
         for (cvap, vap, _) in groups
     }
 
     # Rename colunms with percentages.
     cvappcts = [cvap + "%" for (cvap, _, _) in groups]
 
     # Get the county names and compute population-weighted CVAP averages. This
@@ -305,33 +328,36 @@
     counties = list(set(source["_county"]))
     countyaverages = {pct: {} for pct in cvappcts}
 
     for county in counties:
         chunk = source[source["_county"] == county]
 
         for cvap19, vap19, _ in groups:
-            # Calculate the CVAP19-to-VAP19 ratio. Set numpy to ignore runtimewarnings,
-            # but warn the user if one is encountered. We do this so that the user
-            # doesn't get spooked by a numpy warning, but we're still noisy about
-            # the weird value encountered.
+            # Calculate the CVAP19-to-VAP19 ratio. Set numpy to ignore
+            # runtimewarnings, but warn the user if one is encountered.
+            # We do this so that the user doesn't get spooked by a numpy
+            # warning, but we're still noisy about the weird value
+            # encountered.
             cvap19total = chunk[cvap19].sum()
             vap19total = chunk[vap19].sum()
 
             np.seterr(divide="ignore", invalid="ignore")
             ratio = cvap19total / vap19total
 
             # Check whether the ratio of the above is less than the ceiling.
             if not np.isfinite(ratio):
-                print(county,
-                      f"Encountered an invalid ratio: there are {cvap19total} {cvap19} "
-                      f"persons and {vap19total} {vap19} persons, for a ratio of "
-                      f"{cvap19total}/{vap19total}. "
-                      f"we have substituted it for the statewide {cvap19}-to-{vap19} "
-                      f"share of {statewide[cvap19 + '%']}."
-                      )
+                print(
+                    county,
+                    f"Encountered an invalid ratio: there are "
+                    f"{cvap19total} {cvap19} persons and {vap19total} "
+                    f"{vap19} persons, for a ratio of {cvap19total}/"
+                    f"{vap19total}. @e have substituted it for the "
+                    f"statewide {cvap19}-to-{vap19} share of "
+                    f"{statewide[cvap19 + '%']}.",
+                )
                 ratio = statewide[cvap19 + "%"]
 
             # Set the county-average ratio.
             countyaverages[cvap19 + "%"][county] = ratio
 
     # Reset the numpy error catching thing.
     np.seterr(all="warn")
@@ -340,49 +366,45 @@
     # by the user.
     for pct in cvappcts:
         # Fill NaNs with the *county-wide* average.
         countywidepcts = countyaverages[pct]
 
         source[pct] = source[pct].replace(np.inf, np.nan)
         nanindices = source[source[pct].isna()].index
-        source.loc[nanindices, pct] = source.loc[nanindices, "_county"].map(countywidepcts)
+        source.loc[nanindices, pct] = source.loc[nanindices, "_county"].map(
+            countywidepcts
+        )
 
         # Fill zeroes with the `zfill` value, and cap all the percentages.
-        source[pct] = source[pct] \
-            .replace(0, zfill) \
-            .apply(lambda c: 1 if c > ceiling else c)
+        source[pct] = (
+            source[pct].replace(0, zfill).apply(lambda c: 1 if c > ceiling else c)
+        )
 
     # Assert we don't have any percentages over percentage_cap.
-    assert all(
-        np.all(source[p + "%"] <= ceiling)
-        for (p, _, __) in groups
-    )
+    assert all(np.all(source[p + "%"] <= ceiling) for (p, _, __) in groups)
 
     # Assert we don't have any zeros.
-    assert all(
-        np.all(source[p + "%"] > 0)
-        for (p, _, __) in groups
-    )
+    assert all(np.all(source[p + "%"] > 0) for (p, _, __) in groups)
 
     # Set indices and create a mapping from IDs to weights.
     source = source.set_index(cvap_geoid)
     source = source[cvappcts]
     weights = source.to_dict(orient="index")
 
     # Group by the CVAP GEOID.
     groupedtogeometry = list(pared.groupby(cvap_geoid))
 
     # Get the year suffix so we can replace columns.
     yearsuffix = str(year)[2:]
 
-    # For each of the geometry groups (e.g. a set of rows of blocks corresponding
-    # to a single tract), and for each of the CVAP groups, apply the appropriate
-    # weight to the blocks' 2020 VAP populations.
+    # For each of the geometry groups (e.g. a set of rows of blocks
+    # corresponding to a single tract), and for each of the CVAP groups,
+    # apply the appropriate weight to the blocks' 2020 VAP populations.
     for ix, group in groupedtogeometry:
-        for (cvap10, vap10, vap20) in groups:
+        for cvap10, vap10, vap20 in groups:
             weight = cvap10 + "%"
             cvap20 = cvap10.replace(yearsuffix, "20_EST")
             group[weight] = weights[ix][weight]
             group[cvap20] = group[weight] * group[vap20]
 
     # Re-create a dataframe and strip out % columns, leaving only the estimate
     # columns.
```

### Comparing `gerrytools-1.0.2/gerrytools/data/fetch.py` & `gerrytools-1.1.0/gerrytools/data/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import io
+import json
+from datetime import datetime
+from typing import List, Tuple, Union
 
 import pandas as pd
 import requests
-import json
-import io
-from datetime import datetime
 from pydantic import BaseModel
-from typing import Tuple, List, Union
 
-from .URLs import ids, csvs, one
+from .URLs import csvs, ids, one
 
 
 class Submission(BaseModel):
     """
     Provides a base model for data retrieved from districtr. Allows us to use
     dot notation when accessing properties rather than dict notation.
     """
+
     link: str
     """A districtr URL."""
     plan: dict
     """districtr plan object."""
     id: str
     """districtr identifier."""
     units: str
@@ -33,16 +34,16 @@
 
 def tabularized(state, submissions) -> Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """
     Returns districtr submission information in a tabular format.
 
     Args:
         state (State): `us.State` object (e.g. `us.states.WI`).
-        submissions (list): List of `Submission` objects returned from a call to
-            `submissions`.
+        submissions (list): List of `Submission` objects returned from a
+            call to `submissions`.
 
     Returns:
         Three dataframes corresponding to plan-based submissions, COI-based
         submissions, and written submissions to the provided state.
 
     Example:
         Prototypical example usage.
@@ -100,16 +101,16 @@
     else:
         plans = pd.DataFrame()
     if not subset_cois.empty:
         cois = cois.merge(subset_cois, on="id")
     else:
         cois = pd.DataFrame()
 
-    # Drop bad columns and rename. Not sure why we have to `inplace` things here,
-    # but... fine.
+    # Drop bad columns and rename. Not sure why we have to `inplace`
+    # things here, but... fine.
     for df in [plans, cois]:
         if not df.empty:
             # Remove columns we don't necessarily care about.
             for col in ["type_x", "link_x", "coalition"]:
                 if col in list(df):
                     df.drop(col, axis=1, inplace=True)
 
@@ -127,25 +128,25 @@
     Args:
         state (State): `us.State` object (e.g. `us.states.WI`).
         sample (int, optional): The number of sample plans to retrieve.
 
     Returns:
         A list of `Submissions`, either to be interpreted raw or tabularized.
     """
-    # Get the appropriate URL and send the request. Made some basic ASCII art with
-    # the second three variable names... it's like the request is loading letter
-    # by letter.
+    # Get the appropriate URL and send the request. Made some basic ASCII
+    # art with the second three variable names... it's like the request
+    # is loading letter by letter.
     url = ids(state)
     __w = requests.get(url).text
     _aw = json.loads(__w)["ids"]
     raw = _aw[:sample] if sample else _aw
 
-    # Create `Submission` objects for each of the retrieved objects. Getting the
-    # individual plans is the bottleneck here, and unfortunately we can't retrieve
-    # them in bulk (... or can we?).
+    # Create `Submission` objects for each of the retrieved objects.
+    # Getting the individual plans is the bottleneck here, and
+    # unfortunately we can't retrieve them in bulk (... or can we?).
     submissions = []
     for entity in raw:
         # Retrieve the required data points.
         identifier = parse_id(entity["link"], df=False)
         districtr = individual(identifier)
 
         # Force all plan keys and values to strings.
@@ -155,23 +156,25 @@
                 for k, v in districtr["plan"]["assignment"].items()
             }
             units = districtr["plan"]["units"]["name"]
             unitsType = districtr["plan"]["units"]["unitType"]
             tileset = districtr["plan"]["units"]["tilesets"][0]["sourceLayer"]
 
             # Create a new Submission.
-            submissions.append(Submission(
-                link=entity["link"],
-                id=identifier,
-                plan=plan,
-                units=units,
-                unitsType=unitsType,
-                tileset=tileset,
-                type=entity["type"]
-            ))
+            submissions.append(
+                Submission(
+                    link=entity["link"],
+                    id=identifier,
+                    plan=plan,
+                    units=units,
+                    unitsType=unitsType,
+                    tileset=tileset,
+                    type=entity["type"],
+                )
+            )
         except BaseException:
             pass
 
     return submissions
 
 
 def as_dataframe(url) -> pd.DataFrame:
@@ -201,15 +204,16 @@
 
 
 def parse_id(link, df=True) -> Union[str, pd.Series]:
     """
     Given a districtr link, parse out the districtr identifier.
 
     Args:
-        l (str): districtr url containing the districtr ID of the provided plan.
+        l (str): districtr url containing the districtr ID of the provided
+            plan.
         df (bool, optional): If `l` is a dataframe, then we use pandas string
             operations rather than built-in ones.
 
     Returns:
         districtr ID.
     """
     if df:
```

### Comparing `gerrytools-1.0.2/gerrytools/data/geometries.py` & `gerrytools-1.1.0/gerrytools/data/geometries.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import requests
 
 
 def geometries20(state, filepath, geometry="tract"):
     """
     Retrieves Lab-processed geometric data for the provided state and geometry
     level and writes it to the provided filepath.
@@ -23,24 +22,26 @@
         "congress": "cd116",
         "county": "county",
         "cousub": "cousub",
         "place": "place",
         "senate": "sldu",
         "house": "sldl",
         "tract": "tract",
-        "vtd": "vtd"
+        "vtd": "vtd",
     }
 
     # Check that the passed geometry is allowable.
     if geometry not in set(geometrymap.keys()):
-        print(f"Requested geometry \"{geometry}\" is not allowed; loading tracts.")
+        print(f'Requested geometry "{geometry}" is not allowed; ' "loading tracts.")
         geometry = "tract"
 
     # Specify the base url.
     base = "https://s3.us-east-2.amazonaws.com/data.mggg.org/census-2020/"
-    suffix = f"{state.abbr.lower()}/{state.abbr.lower()}_{geometrymap[geometry]}.zip"
+    suffix = (
+        f"{state.abbr.lower()}/{state.abbr.lower()}_" f"{geometrymap[geometry]}.zip"
+    )
 
     # Send the request!
     request = requests.get(base + suffix)
 
     with open(filepath, "wb") as w:
         w.write(request.content)
```

### Comparing `gerrytools-1.0.2/gerrytools/data/remap.py` & `gerrytools-1.1.0/gerrytools/data/remap.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-
-from typing import Callable
 import ast
+from typing import Callable
 
 
 def remap(plans, unitmaps, popmap=None) -> Callable:
     """
     Re-maps assignments to the specified set of units.
 
     Args:
         plans (DataFrame): The Pandas DataFrame produced by ``tabularized()``.
-        unitmaps (dict): A dictionary whose keys are unit types appearing in the
-            `unitsType` column, and whose values are dictionaries mapping unique
-            identifiers of one set of geometries to unique identifiers (or lists
-            of unique identifiers) of another set of geometries; these correspond
-            to mappings generated by `unitmap()` and the inverse mapping generated
-            by `invert()`.
+        unitmaps (dict): A dictionary whose keys are unit types appearing
+            in the `unitsType` column, and whose values are dictionaries
+            mapping unique identifiers of one set of geometries to unique
+            identifiers (or lists of unique identifiers) of another set of
+            geometries; these correspond to mappings generated by `unitmap()`
+            and the inverse mapping generated by `invert()`.
         popmap (dict, optional): A mapping from unit unique identifiers to
             population values. Only applies when we are mapping from smaller
             units to larger ones.
 
     Returns:
         A function
     """
+
     def _(row):
         # Get the assignment for the row.
         assignment = ast.literal_eval(row["plan"])
 
-        # Attempt to get the type of units specified by the row; if we can't – i.e.
-        # the user didn't specify a unit mapping corresponding to that unit type
-        # in `unitmaps` – we leave the assignment alone and warn the user.
+        # Attempt to get the type of units specified by the row; if we
+        # can't – i.e.the user didn't specify a unit mapping corresponding
+        # to that unit typein `unitmaps` – we leave the assignment alone and warn the user.
         try:
             unitsType = row["units"]
             unitmap = unitmaps[unitsType]
         except BaseException:
             print(f"No unit mapping provided for {row['units']}; skipping.")
             return assignment
 
         # What kind of mapping do we have? If `mapping` is from a single key
-        # to a single value, then we're mapping units one-to-one (e.g. block IDs
-        # to VTD IDs); otherwise, we're mapping units one-to-many (e.g. VTD IDs
-        # to blocks). If `mapping` is of the former type, then it's possible that
-        # some larger units may comprise smaller units in multiple districts. If
-        # this is the case, then we assign larger units to the district in which
-        # most of the larger unit's population resides; otherwise, we simply
-        # assign all smaller units to whichever district the larger unit's in.
+        # to a single value, then we're mapping units one-to-one (e.g. block
+        # IDs to VTD IDs); otherwise, we're mapping units one-to-many (e.g.
+        # VTD IDs to blocks). If `mapping` is of the former type, then
+        # it's possible that some larger units may comprise smaller units
+        # in multiple districts. If this is the case, then we assign larger
+        # units to the district in which most of the larger unit's population
+        # resides; otherwise, we simply assign all smaller units to whichever
+        # district the larger unit's in.
         firstvalue = next(iter(unitmap.values()))
         unitmapdirection = "down"
 
         # Mark which kind of mapping we have.
         if isinstance(firstvalue, list):
             unitmapdirection = "down"
         else:
@@ -60,35 +61,33 @@
 
     plans["plan"] = plans.apply(_, axis=1)
     return plans
 
 
 def _down(unitmap, assignment) -> dict:
     """
-    Maps districting assignments from larger units to smaller units (which nest
-    in the larger units).
+    Maps districting assignments from larger units to smaller
+        units (which nest in the larger units).
 
     Args:
-        unitmap (dict): Dictionary which maps larger unit identifiers to lists of
-            smaller unit identifiers (e.g. VTD identifiers to block identifiers).
+        unitmap (dict): Dictionary which maps larger unit identifiers to
+            lists of smaller unit identifiers (e.g. VTD identifiers to
+            block identifiers).
         assignment (dict): Maps larger unit identifiers to districts.
 
     Returns:
         Maps smaller unit identifiers to districts according to `assignment`.
     """
     # Create an empty mapping.
     mapped = {}
 
     # For each of the keys in the provided assignment, get the units to which
     # the keys correspond, and assign them appropriately.
     for bigger, district in assignment.items():
         smallers = unitmap[bigger]
-        mapped.update({
-            smaller: district
-            for smaller in smallers
-        })
+        mapped.update({smaller: district for smaller in smallers})
 
     return mapped
 
 
 def _up(unitmap, assignment, popmap):
     return assignment
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/__init__.py` & `gerrytools-1.1.0/gerrytools/geometry/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-
 """
 Provides ease-of-use functionality for geographic and geometric operations.
 """
 
+from .dataframe import dataframe
 from .dissolve import dissolve
 from .dualgraph import dualgraph
-from .unitmap import unitmap, invert
-from .dataframe import dataframe
-
 from .optimize import (
-    minimize_dispersion, minimize_dispersion_with_parity, minimize_parity,
-    calculate_dispersion, populationoverlap, arealoverlap, optimalrelabeling
+    arealoverlap,
+    calculate_dispersion,
+    minimize_dispersion,
+    minimize_dispersion_with_parity,
+    minimize_parity,
+    optimalrelabeling,
+    populationoverlap,
 )
-
+from .unitmap import invert, unitmap
 from .updater import dispersion_updater_closure
 
 __all__ = [
     "minimize_dispersion",
     "minimize_dispersion_with_parity",
     "minimize_parity",
     "calculate_dispersion",
@@ -24,9 +26,9 @@
     "dissolve",
     "dualgraph",
     "unitmap",
     "invert",
     "dataframe",
     "populationoverlap",
     "optimalrelabeling",
-    "arealoverlap"
+    "arealoverlap",
 ]
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/dataframe.py` & `gerrytools-1.1.0/gerrytools/geometry/dataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-
-from gerrychain import Partition
 import pandas as pd
+from gerrychain import Partition
 
 
 def dataframe(
     P: Partition, index: str = "id", assignment: str = "DISTRICT", columns: list = None
 ) -> pd.DataFrame:
     """
     Converts a `Partition` into a `DataFrame`.
@@ -18,15 +17,17 @@
             including the index. If `None` (or another falsy value), gets all
             columns.
 
     Returns:
         `DataFrame` with attached graph data.
     """
     # Create dataframe.
-    gdf = pd.DataFrame.from_records({index: v, **d} for v, d in P.graph.nodes(data=True))
+    gdf = pd.DataFrame.from_records(
+        {index: v, **d} for v, d in P.graph.nodes(data=True)
+    )
 
     # Assign vertices.
     assignedvertices = P.assignment.to_dict()
     gdf[assignment] = gdf[index].map(assignedvertices)
 
     # Drop columns if necessary.
     if columns:
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/dualgraph.py` & `gerrytools-1.1.0/gerrytools/geometry/dualgraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-
 from gerrychain.graph import Graph
 
 
 def dualgraph(
-    geometries, index=None, geometrycolumn="geometry", colmap={}, buffer=0,
-    edges_to_add=[], edges_to_cut=[]
+    geometries,
+    index=None,
+    geometrycolumn="geometry",
+    colmap={},
+    buffer=0,
+    edges_to_add=[],
+    edges_to_cut=[],
 ) -> Graph:
     """
     Generates a graph dual to the provided geometric data.
 
     Args:
         geometries (GeoDataFrame): Geometric data represented as a GeoDataFrame.
         index (str, optional): Unique identifiers; indexing column of `geometries`.
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/optimize.py` & `gerrytools-1.1.0/gerrytools/geometry/optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import math
+from typing import Any, Callable, Dict, List
 
-from typing import Dict, List, Any, Callable
 import geopandas as gpd
-import tqdm
 import gurobipy as gp
+import pandas as pd
+import tqdm
 from gurobipy import GRB
 from scipy.optimize import linear_sum_assignment as lsa
-import math
-import pandas as pd
 
 
 def arealoverlap(
-    left: gpd.GeoDataFrame, right: gpd.GeoDataFrame, assignment: str = "DISTRICT",
-    crs=None
+    left: gpd.GeoDataFrame,
+    right: gpd.GeoDataFrame,
+    assignment: str = "DISTRICT",
+    crs=None,
 ) -> pd.DataFrame:
     r"""
     Given two GeoDataFrames, each encoding districting plans, computes the areal
     overlap between each pair of districts. `left` is the districting plan to be
     relabeled (e.g. a proposed districting plan) and `right` is the districting
     plan with district labels we're trying to match (e.g. an enacted districting
     plan). If `left` (denoted \(L\)) has \(n\) districts and `right` (denoted \(R\)) has
@@ -49,29 +51,34 @@
     # Figure out the image as we go along.
     image = []
 
     # Now, iterate over each dissolved district, finding the areal overlap with
     # enacted districts.
     for pid, pdistrict in zip(left[assignment], left["geometry"]):
         image.append(pid)
-        records.append({
-            eid: pdistrict.intersection(edistrict).area
-            for eid, edistrict in zip(right[assignment], right["geometry"])
-        })
+        records.append(
+            {
+                eid: pdistrict.intersection(edistrict).area
+                for eid, edistrict in zip(right[assignment], right["geometry"])
+            }
+        )
 
     # Create a dataframe from that!
     weighted = pd.DataFrame.from_records(records)
     weighted.index = image
 
     return weighted
 
 
 def populationoverlap(
-    left: pd.DataFrame, right: pd.DataFrame, identifier: str = "GEOID20",
-    population: str = "TOTPOP20", assignment: str = "DISTRICT"
+    left: pd.DataFrame,
+    right: pd.DataFrame,
+    identifier: str = "GEOID20",
+    population: str = "TOTPOP20",
+    assignment: str = "DISTRICT",
 ) -> pd.DataFrame:
     r"""
     Given two unit-level DataFrames — i.e. two dataframes where each row represents
     an atomic unit like Census blocks or VTDs, and each row contains a district
     assignment — computes the amount of population shared by each pair of districts.
     `left` is the districting plan to be relabeled (e.g. a proposed districting
     plan) and `right` is the districting plan with district labels we're trying
@@ -117,28 +124,30 @@
         subleft = left[left[assignment] == fromlabel]
         subright = right[right[identifier].isin(subleft[identifier])]
 
         # Aggregate shared blocks based on district label.
         agg = subright.groupby(assignment, as_index=False).sum()
 
         # Now figure out the shared populations.
-        records.append({
-            i: shared for i, shared in zip(agg[assignment], agg[population])
-        })
+        records.append(
+            {i: shared for i, shared in zip(agg[assignment], agg[population])}
+        )
 
     # Create the cost matrix!
     C = pd.DataFrame.from_records(records).fillna(0)
     C.index = preimage
 
     return C
 
 
 def optimalrelabeling(
-    left: Any, right: Any, maximize: bool = True,
-    costmatrix: Callable = populationoverlap
+    left: Any,
+    right: Any,
+    maximize: bool = True,
+    costmatrix: Callable = populationoverlap,
 ) -> dict:
     r"""
     Finds the optimal relabeling for two districting plans.
 
     Args:
         left (Any): Data structure which can be passed to `costmatrix` to construct
             a cost matrix. District labels will be the preimage of the relabeling.
@@ -220,16 +229,17 @@
     image = [image[i] for i in imageindices]
 
     # Zip the preimage and image into a dict, and we're done!
     return dict(zip(preimage, image))
 
 
 def ensure_column_types(
-    units: gpd.GeoDataFrame, columns: List[str],
-    expression: Callable[[Any], bool] = lambda x: x.startswith("int")
+    units: gpd.GeoDataFrame,
+    columns: List[str],
+    expression: Callable[[Any], bool] = lambda x: x.startswith("int"),
 ) -> bool:
     """
     Ensure that the given columns in the GeoDataFrame have a type matching the
     filtering expression. This gives more flexibility over other type checking
     methods.
 
     Args:
@@ -240,16 +250,20 @@
     Returns:
         A boolean indicating if all the columns checked match the expression.
     """
     return all([expression(x.name) for x in units[columns].dtypes])
 
 
 def minimize_dispersion(
-    units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str,
-    extra_constraints=None, verbose: bool = False
+    units: gpd.GeoDataFrame,
+    enacted_col: str,
+    proposed_col: str,
+    pop_col: str,
+    extra_constraints=None,
+    verbose: bool = False,
 ) -> Dict[str, str]:
     """
     Minimize core dispersion in a state given an column with enacted districts
     and a column with proposed numberings. Returns a dictionary relabeling the
     proposed cols. Used in WI. Assumes that district labels are 1-indexed.
 
     Args:
@@ -262,40 +276,61 @@
 
     Returns:
         A dictionary mapping proposed labels to optimized labels.
     """
     if not ensure_column_types(units, [enacted_col, proposed_col]):
         raise TypeError("Your enacted and proposed columns must be an int type!")
 
-    if not ensure_column_types(units, [pop_col], lambda x: x.startswith("int") or x.startswith("float")):
+    if not ensure_column_types(
+        units, [pop_col], lambda x: x.startswith("int") or x.startswith("float")
+    ):
         raise TypeError("Your pop col must be an int or float type!")
 
     districts = list(set(units[proposed_col].astype(int)))
     model = gp.Model("state_model")
-    model.setParam('OutputFlag', int(verbose))
+    model.setParam("OutputFlag", int(verbose))
 
-    numbering = model.addVars(len(districts), len(districts), vtype=GRB.BINARY, name="numbering")
+    numbering = model.addVars(
+        len(districts), len(districts), vtype=GRB.BINARY, name="numbering"
+    )
 
     exprs = []
     if verbose:
-        def wrapper(x): return tqdm.tqdm(x)
+
+        def wrapper(x):
+            return tqdm.tqdm(x)
+
     else:
-        def wrapper(x): return x
 
-    for district in wrapper(districts):  # iter over proposed
-        enacted_intersection = units[units[proposed_col] == district].groupby(enacted_col).sum()[pop_col].to_dict()
+        def wrapper(x):
+            return x
 
-        for enacted, overlap_pop in enacted_intersection.items():  # maximize overlap; minimize dispersion
+    for district in wrapper(districts):  # iter over proposed
+        enacted_intersection = (
+            units[units[proposed_col] == district]
+            .groupby(enacted_col)
+            .sum()[pop_col]
+            .to_dict()
+        )
+
+        for (
+            enacted,
+            overlap_pop,
+        ) in enacted_intersection.items():  # maximize overlap; minimize dispersion
             exprs.append(numbering[district - 1, enacted - 1] * overlap_pop)
 
         if extra_constraints is not None:
             extra_constraints(model, numbering, district, districts)
 
-    model.addConstrs((numbering.sum("*", v) == 1 for v in range(len(districts))), name="v")
-    model.addConstrs((numbering.sum(v, "*") == 1 for v in range(len(districts))), name="h")
+    model.addConstrs(
+        (numbering.sum("*", v) == 1 for v in range(len(districts))), name="v"
+    )
+    model.addConstrs(
+        (numbering.sum(v, "*") == 1 for v in range(len(districts))), name="h"
+    )
 
     obj = gp.quicksum(exprs)
     model.setObjective(obj, GRB.MAXIMIZE)
 
     model.optimize()
 
     solution = model.getVars()
@@ -306,49 +341,63 @@
             if solution[i * len(districts) + j].x:
                 numbering_mapping[districts[i]] = districts[j]
 
     return numbering_mapping
 
 
 def minimize_parity(
-    units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str,
-    verbose: bool = False
+    units: gpd.GeoDataFrame,
+    enacted_col: str,
+    proposed_col: str,
+    pop_col: str,
+    verbose: bool = False,
 ) -> Dict[str, bool]:
     """
     Minimize odd->even parity shift in a state given an column with enacted districts
     and a column with proposed numberings. Returns a dictionary with the parity of the
     proposed cols. Used in WI. Assumes that district labels are 1-indexed.
 
     Args:
         units: The units to optimize on. E.g. Census blocks.
         enacted_col: The column in the GeoDataFrame with the enacted districts.
         proposed_col: The column in the GeoDataFrame with the proposed districts.
+        pop_col: The column in the GeoDataFrame with population counts.
         verbose: If true, do not suppress solver output. Otherwise, stay quiet.
 
     Returns:
         A dictionary mapping proposed labels to booleans values representing the optimal parity.
         (True if even, False odd).
     """
     if not ensure_column_types(units, [enacted_col, proposed_col]):
         raise TypeError("Your enacted and proposed columns must be an int type!")
 
-    if not ensure_column_types(units, [pop_col], lambda x: x.startswith("int") or x.startswith("float")):
+    if not ensure_column_types(
+        units, [pop_col], lambda x: x.startswith("int") or x.startswith("float")
+    ):
         raise TypeError("Your pop col must be an int or float type!")
 
     model = gp.Model("parity_model")
-    model.setParam('OutputFlag', int(verbose))
+    model.setParam("OutputFlag", int(verbose))
 
     districts = list(set(units[proposed_col].astype(int)))
-    districts_even = model.addVars(len(districts), vtype=GRB.BINARY, name="districts_even")
+    districts_even = model.addVars(
+        len(districts), vtype=GRB.BINARY, name="districts_even"
+    )
 
     exprs = []
     if verbose:
-        def wrapper(x): return tqdm.tqdm(x)
+
+        def wrapper(x):
+            return tqdm.tqdm(x)
+
     else:
-        def wrapper(x): return x
+
+        def wrapper(x):
+            return x
+
     for i, block in wrapper(units[[enacted_col, proposed_col, pop_col]].iterrows()):
         district = districts.index(int(block[proposed_col]))
         isOdd = bool((int(block[enacted_col]) % 2) == 1)
         exprs.append(isOdd * districts_even[district] * block[pop_col])
 
     obj = gp.quicksum(exprs)
     model.addConstr(gp.quicksum(districts_even) == math.floor(len(districts) / 2), "c0")
@@ -360,57 +409,101 @@
     for i, v in enumerate(model.getVars()):
         mapping[districts[i]] = bool(v.x)
 
     return mapping
 
 
 def minimize_dispersion_with_parity(
-    units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str,
-    extra_constraints=None
+    units: gpd.GeoDataFrame,
+    enacted_col: str,
+    proposed_col: str,
+    pop_col: str,
+    extra_constraints=None,
 ) -> Dict[str, str]:
     """
     Minimize dispersion and odd->even parity shift in a state given an column with
     enacted districts and a column with proposed numberings. Returns a dictionary
     relabeling the proposed cols. Used in WI. Assumes that district labels are 1-indexed.
 
     Args:
         units: The units to optimize on. E.g. Census blocks.
         enacted_col: The column in the GeoDataFrame with the enacted districts.
         proposed_col: The column in the GeoDataFrame with the proposed districts.
+        pop_col: The column in the GeoDataFrame with population counts.
         extra_constraints: Optional; A function that can add extra constraints
             to the model, such as parity (in the case of WI).
 
     Returns:
         A dictionary mapping proposed labels to optimized labels.
     """
     optimal_parity_mapping = minimize_parity(units, enacted_col, proposed_col, pop_col)
 
     def parity_constraint(model, numbering, district, districts):
         if optimal_parity_mapping[district]:
             model.addConstr(
                 gp.quicksum(
-                    numbering[district - 1, x - 1] for x in range(1, len(districts) + 1) if x % 2 == 0
-                ) == 1
+                    numbering[district - 1, x - 1]
+                    for x in range(1, len(districts) + 1)
+                    if x % 2 == 0
+                )
+                == 1
             )
 
         extra_constraints(model, numbering, district, districts)
 
-    return minimize_dispersion(units, enacted_col, proposed_col, pop_col, parity_constraint)
+    return minimize_dispersion(
+        units, enacted_col, proposed_col, pop_col, parity_constraint
+    )
 
 
-def calculate_dispersion(units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str) -> int:
+def calculate_dispersion(
+    units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str
+) -> int:
     """
     Calculates core dispersion in a state given an column with enacted districts
     and a column with proposed numberings. Used in WI.
 
     Args:
         units: The units to optimize on. E.g. Census blocks.
         enacted_col: The column in the GeoDataFrame with the enacted districts.
         proposed_col: The column in the GeoDataFrame with the proposed districts.
+        pop_col: The column in the GeoDataFrame with population counts.
 
     Returns:
         An integer of the absolute number of people who changed districts.
     """
     if units[enacted_col].dtype != units[proposed_col].dtype:
         raise TypeError("Your enacted and proposed columns must have the same type!")
 
     return units[units[enacted_col] != units[proposed_col]][pop_col].sum()
+
+
+def calculate_dispersion_per_district(
+    units: gpd.GeoDataFrame, enacted_col: str, proposed_col: str, pop_col: str
+) -> Dict[int, int]:
+    """
+    Calculates dispersion per district in a state given a column with enacted districts
+    and a column with proposed districts. Used in GA.
+
+    Args:
+        units: The units to optimize on. E.g. census blocks.
+        enacted_col: The column in the GeoDataFrame with the enacted districts.
+        proposed_col: The column in the GeoDataFrame with the proposed districts.
+        pop_col: The column in the GeoDataFrame with population counts.
+
+    Returns:
+        A dictionary with keys as districts, and values as the number of
+        people displaced from the enacted plan to the proposed plan.
+    """
+    if units[enacted_col].dtype != units[proposed_col].dtype:
+        raise TypeError("Your enacted and proposed columns must have the same type!")
+
+    dispersion_dict = {
+        district: sum(
+            units[pop_col][
+                (units[enacted_col] == district) & (units[proposed_col] != district)
+            ]
+        )
+        for district in sorted(units[enacted_col].unique())
+    }
+
+    return dispersion_dict
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/unitmap.py` & `gerrytools-1.1.0/gerrytools/geometry/unitmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import warnings
+from typing import Dict, List, TypeVar
 
-from typing import List, Dict, TypeVar
 import maup
-import warnings
 
 A = TypeVar("A")
 B = TypeVar("B")
 
 
 def unitmap(source, target) -> dict:
     """
```

### Comparing `gerrytools-1.0.2/gerrytools/geometry/updater.py` & `gerrytools-1.1.0/gerrytools/geometry/updater.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import geopandas as gpd
 import gerrychain
-from .optimize import minimize_dispersion, calculate_dispersion
 
+from .optimize import calculate_dispersion, minimize_dispersion
 
-def dispersion_updater_closure(units: gpd.GeoDataFrame, enacted_col: str, pop_col: str, verbose: bool = False):
+
+def dispersion_updater_closure(
+    units: gpd.GeoDataFrame, enacted_col: str, pop_col: str, verbose: bool = False
+):
     """
     An updater to calculate best possible dispersion for a `gerrychain.Partition` object.
 
     Args:
         units: The units to optimize on. E.g. Census blocks.
         enacted_col: The column in the GeoDataFrame with the enacted districts.
         proposed_col: The column in the GeoDataFrame with the proposed districts.
         extra_constraints: Optional; A function that can add extra constraints
             to the model, such as parity (in the case of WI).
         verbose: If true, do not suppress solver output. Otherwise, stay quiet.
 
     Returns:
         An updater that calculates the minimal core dispersion of a Partition object.
     """
+
     def updater(partition: gerrychain.Partition):
         units["partition"] = partition.assignment.to_series()
 
-        relabeling = minimize_dispersion(units, enacted_col, "partition", pop_col, verbose=verbose)
+        relabeling = minimize_dispersion(
+            units, enacted_col, "partition", pop_col, verbose=verbose
+        )
         units["partition"] = units["partition"].apply(lambda x: relabeling[x])
 
         return calculate_dispersion(units, enacted_col, "partition", pop_col)
 
     return updater
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/__init__.py` & `gerrytools-1.1.0/gerrytools/plotting/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-
 """
 Makes pretty pictures of districting plans, dual graphs, histograms, boxplots,
 and violin plots 🎻.
 """
 
-from .drawplan import drawplan
+from .annotation import arrow, ideal
+from .bins import bins
+from .boxplot import boxplot
+from .choropleth import choropleth
+from .colors import districtr, flare, latex, purples, redbluecmap
+from .districtnumbers import districtnumbers
 from .drawgraph import drawgraph
-from .colors import redbluecmap, flare, purples, districtr, latex
+from .drawplan import drawplan
+from .gifs import gif_multidimensional
 from .histogram import histogram
-from .violin import violin
-from .boxplot import boxplot
+from .multidimensional import multidimensional
 from .scatterplot import scatterplot
 from .sealevel import sealevel
-from .multidimensional import multidimensional
-from .gifs import gif_multidimensional
-from .bins import bins
-from .annotation import arrow, ideal
-from .districtnumbers import districtnumbers
-from .choropleth import choropleth
+from .violin import violin
 
 __all__ = [
     "drawplan",
     "drawgraph",
     "redbluecmap",
     "flare",
     "purples",
@@ -34,9 +33,9 @@
     "multidimensional",
     "gif_multidimensional",
     "arrow",
     "ideal",
     "bins",
     "districtnumbers",
     "latex",
-    "choropleth"
+    "choropleth",
 ]
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/annotation.py` & `gerrytools-1.1.0/gerrytools/plotting/annotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-
 from matplotlib.axes import Axes
+
 from .colors import defaultGray
 
 
-def arrow(
-    ax, text, orientation="horizontal", color=defaultGray, padding=0.1
-) -> Axes:
+def arrow(ax, text, orientation="horizontal", color=defaultGray, padding=0.1) -> Axes:
     """
     For some partisan metrics, we want to draw an arrow showing where the POV-party's
     advantage is. Depending on the orientation of the scores (histograms have
     scores arranged horizontally, violinplots have scores arranged vertically),
     we either place the arrow at the bottom left, pointing rightward, or in the
     middle of the y-axis, pointing up.
 
@@ -34,20 +32,28 @@
     elif orientation == "vertical":
         x = ax.get_xlim()[0] - padding * (sum(map(lambda x: abs(x), ax.get_xlim())))
         y = sum(ax.get_ylim()) / 2
         horizontal_align = "center"
         rotation = 90
 
     ax.text(
-        x, y, text, ha=horizontal_align, va="center", color="white", rotation=rotation,
-        size=10, bbox=dict(
-            boxstyle="rarrow,pad=0.3", fc=color,
+        x,
+        y,
+        text,
+        ha=horizontal_align,
+        va="center",
+        color="white",
+        rotation=rotation,
+        size=10,
+        bbox=dict(
+            boxstyle="rarrow,pad=0.3",
+            fc=color,
             alpha=1,
             ec="black",
-        )
+        ),
     )
 
     return ax
 
 
 def ideal(ax, label, placement, orientation, color=defaultGray, alpha=0.1):
     """
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/bins.py` & `gerrytools-1.1.0/gerrytools/plotting/bins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import List, Tuple, Union
 
 import numpy as np
 from numpy import array
-from typing import Tuple, List, Union
 
 
 def bins(scores, width=None, labels=8) -> Tuple[array, List, List, Union[float, int]]:
     """
     Get necessary information for histograms. If we're working with only a few
     discrete, floating point values, then set the bin width to be relatively thin.
     Otherwise, adaptively set the bin width to the scale of our data.
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/boxplot.py` & `gerrytools-1.1.0/gerrytools/plotting/boxplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+import random
 
 from matplotlib.axes import Axes
-import random
-from .colors import defaultGray, citizenBlue, districtr
+
+from .colors import citizenBlue, defaultGray, districtr
 
 
 def boxplot(
-    ax, scores, xticklabels=None, labels=None, proposed_info={}, percentiles=(1, 99),
-    rotation=0, ticksize=12, jitter=1 / 3
+    ax,
+    scores,
+    xticklabels=None,
+    labels=None,
+    proposed_info={},
+    percentiles=(1, 99),
+    rotation=0,
+    ticksize=12,
+    jitter=1 / 3,
 ) -> Axes:
     r"""
     Plot boxplots, which takes `scores` — a dictionary where each value
     (corresponding to an ensemble, citizens' ensemble, or proposed plans),
     will be a list of lists, where each sublist will be its own box. Proposed
     scores will be plotted as colored circles on their respective box. Color the
     boxplots conditioned on the kind of the scores (ensemble or citizen), and
@@ -35,20 +43,20 @@
         labels (list, optional): x- and y-axis labels, if desired.
         xticklabels (list, optional): Labels for the boxes, default to integers.
 
     Returns:
         `Axes` object on which the violins are plotted.
     """
     # Get all the scores into one list; pick a face color.
-    ensemble = scores["ensemble"] if scores["ensemble"] else scores["citizen"]
-    facecolor = defaultGray if scores["ensemble"] else citizenBlue
+    ensemble = scores["ensemble"] if "ensemble" in scores else scores["citizen"]
+    facecolor = defaultGray if "ensemble" in scores else citizenBlue
 
     # Specify the boxplots' style.
     boxstyle = {
-        "lw": 2,
+        "lw": 1 / 2,
         "color": facecolor,
     }
 
     # Plot boxplots.
     ax.boxplot(
         ensemble,
         whis=percentiles,
@@ -57,38 +65,46 @@
         capprops=boxstyle,
         medianprops=boxstyle,
         showfliers=False,
     )
 
     # Set xticks, xlabels, and x-axis limits
     if not xticklabels:
-        xticklabels = range(1, len(scores['ensemble']) + 1)
+        xticklabels = range(1, len(scores["ensemble"]) + 1)
     ax.set_xticks(range(1, len(ensemble) + 1))
     ax.set_xticklabels(xticklabels, fontsize=ticksize, rotation=rotation)
     ax.set_xlim(0.5, len(ensemble) + 0.5)
 
     # Plot each proposed plan individually, adjusting its detail points by
     # a value drawn from the uniform distribution of specified width centered on
     # the index of the violin.
-    if scores["proposed"]:
+    if "proposed" in scores:
         for boxplot in range(len(scores["proposed"])):
             for plan, score in enumerate(scores["proposed"][boxplot]):
                 # Horizontally jitter proposed scores if there are multiple scores
                 # at the same height.
-                jitter_val = random.uniform(-jitter, jitter) if scores["proposed"][boxplot].count(score) > 1 else 0
+                jitter_val = (
+                    random.uniform(-jitter, jitter)
+                    if scores["proposed"][boxplot].count(score) > 1
+                    else 0
+                )
+                color_val = ""
+                if "colors" in scores["proposed"]:
+                    color_val = scores["proposed"]["colors"][boxplot]
+                else:
+                    color_val = districtr(plan + 1).pop()
                 ax.scatter(
                     boxplot + 1 + jitter_val,
                     score,
-                    color=districtr(plan + 1).pop(),
-                    edgecolor='black',
+                    color=color_val,
+                    edgecolor="black",
                     s=100,
                     alpha=0.9,
                     label=proposed_info["names"][plan] if boxplot == 0 else None,
                 )
         ax.legend()
-        ax.grid(axis='x')
 
     if labels:
         ax.set_xlabel(labels[0], fontsize=24)
         ax.set_ylabel(labels[1], fontsize=24)
 
     return ax
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/choropleth.py` & `gerrytools-1.1.0/gerrytools/plotting/choropleth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.axes import Axes
 import numpy as np
+from matplotlib.axes import Axes
 
 from .colors import overlays as overlaycolors
 from .districtnumbers import districtnumbers
 
 
 def choropleth(
-    geometries, districts=None, assignment=None, demographic="BVAP",
-    overlays=[], cmap="Purples", cbartitle=None, numbers=True, lw=1 / 8,
-    fontsize=15, min=0, max=1, interval=1 / 10, colorbar=True
+    geometries,
+    districts=None,
+    assignment=None,
+    demographic="BVAP",
+    overlays=[],
+    cmap="Purples",
+    cbartitle=None,
+    numbers=True,
+    lw=1 / 8,
+    fontsize=15,
+    min=0,
+    max=1,
+    interval=1 / 10,
+    colorbar=True,
 ) -> Axes:
     r"""
     Visualization of population shares or totals in a state's map.
 
     Args:
         geometries (GeoDataFrame): Base geometries for the state. Population
             shares or totals will be drawn at this level (i.e. statistics are
@@ -79,43 +89,45 @@
     geometries.plot(
         column=demographic,
         cmap=cmap,
         edgecolor="lightgray",
         linewidth=lw,
         vmin=min,
         vmax=max,
-        ax=base
+        ax=base,
     )
 
     # Create and plot the colorbar on the right side of the figure.
     if colorbar:
         cbar = fig.colorbar(
-            plt.cm.ScalarMappable(cmap=colorbarmap, norm=norm), shrink=0.5,
-            location="right", ax=base, ticks=ticks
+            plt.cm.ScalarMappable(cmap=colorbarmap, norm=norm),
+            shrink=0.5,
+            location="right",
+            ax=base,
+            ticks=ticks,
         )
         cbar.ax.set_yticklabels(labels)
         cbar.ax.set_ylabel(cbartitle)
         cbar.ax.yaxis.set_label_position("left")
         cbar.ax.tick_params(size=0)
 
     # Plot each of the overlays, adjusting CRSes and applying colors as we go.
     for idx, geom in enumerate(overlays):
         geom = geom.to_crs(geometries.crs)
-        geom.boundary.plot(edgecolor=overlaycolors[-(idx + 1)], linewidth=1 / 4, ax=base)
+        geom.boundary.plot(
+            edgecolor=overlaycolors[-(idx + 1)], linewidth=1 / 4, ax=base
+        )
 
     # If district geometries are provided, plot them as well.
     if districts is not None:
-        districts.plot(
-            edgecolor="black",
-            linewidth=3 / 2,
-            ax=base,
-            color="None"
-        )
+        districts.plot(edgecolor="black", linewidth=3 / 2, ax=base, color="None")
 
     # If district numbers are to be plotted, plot those too!
     if numbers:
-        base = districtnumbers(base, districts, assignment=assignment, fontsize=fontsize)
+        base = districtnumbers(
+            base, districts, assignment=assignment, fontsize=fontsize
+        )
 
     # Turn plot vertical/horizontal axes off and return base Axes.
     base.set_axis_off()
 
     return base, None if not colorbar else cbar
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/colors.py` & `gerrytools-1.1.0/gerrytools/plotting/colors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-
-import seaborn as sns
-import math
 import json
-from typing import List, Tuple
+import math
+import pkgutil
 from random import choice
 from string import hexdigits as hex
-import pkgutil
+from typing import List, Tuple
+
+import seaborn as sns
 
+defaultGray = "#5c676f"
 """
 Default gray plotting color; used in histograms, violin plots, and arrows.
 """
-defaultGray = "#5c676f"
 
+citizenBlue = "#4693b3"
 """
 Citizen ensemble blue color; used in histograms, violin plots, and arrows. (Aka
 Citizen Kane).
 """
-citizenBlue = "#4693b3"
 
+overlays = ["gainsboro", "silver", "darkgray", "gray", "dimgrey"]
 """
 Overlay colors for choropleth maps.
 """
-overlays = ["gainsboro", "silver", "darkgray", "gray", "dimgrey"]
 
+latex = json.loads(pkgutil.get_data(__name__, "latexcolors.json"))
 """
-LaTeX colors, [borrowed from here.](http://latexcolor.com/)
+A dictionary of nice LaTeX colors, [borrowed from here.](http://latexcolor.com/)
 """
-latex = json.loads(pkgutil.get_data(__name__, "latexcolors.json"))
 
 
 def hexshift(color) -> str:
     """
     Randomly modifies the provided hexadecimal color.
 
     Args:
@@ -51,20 +51,53 @@
 
     # Return the subbed string.
     return color.replace(char, sub)
 
 
 def districtr(N):
     colors = [
-        "#0099cd", "#ffca5d", "#00cd99", "#99cd00", "#cd0099", "#9900cd", "#8dd3c7",
-        "#bebada", "#fb8072", "#80b1d3", "#fdb462", "#b3de69", "#fccde5", "#bc80bd",
-        "#ccebc5", "#ffed6f", "#ffffb3", "#a6cee3", "#1f78b4", "#b2df8a", "#33a02c",
-        "#fb9a99", "#e31a1c", "#fdbf6f", "#ff7f00", "#cab2d6", "#6a3d9a", "#b15928",
-        "#64ffda", "#00B8D4", "#A1887F", "#76FF03", "#DCE775", "#B388FF", "#FF80AB",
-        "#D81B60", "#26A69A", "#FFEA00", "#6200EA"
+        "#0099cd",
+        "#ffca5d",
+        "#00cd99",
+        "#99cd00",
+        "#cd0099",
+        "#9900cd",
+        "#8dd3c7",
+        "#bebada",
+        "#fb8072",
+        "#80b1d3",
+        "#fdb462",
+        "#b3de69",
+        "#fccde5",
+        "#bc80bd",
+        "#ccebc5",
+        "#ffed6f",
+        "#ffffb3",
+        "#a6cee3",
+        "#1f78b4",
+        "#b2df8a",
+        "#33a02c",
+        "#fb9a99",
+        "#e31a1c",
+        "#fdbf6f",
+        "#ff7f00",
+        "#cab2d6",
+        "#6a3d9a",
+        "#b15928",
+        "#64ffda",
+        "#00B8D4",
+        "#A1887F",
+        "#76FF03",
+        "#DCE775",
+        "#B388FF",
+        "#FF80AB",
+        "#D81B60",
+        "#26A69A",
+        "#FFEA00",
+        "#6200EA",
     ]
 
     repeats = math.ceil(N / len(colors))
     tail = [hexshift(c) for c in colors * (repeats - 1)]
     return (colors + (tail if tail else []))[:N]
 
 
@@ -79,20 +112,20 @@
     Returns:
         List of RGB tuples.
     """
     midpoint = math.ceil(n / 2)
 
     # To get the appropriately-toned blues and reds, we create a list of colors,
     # then select the first section of each color.
-    blues = list(
-        sns.color_palette("coolwarm", as_cmap=False, n_colors=n + 2)
-    )[:midpoint]
-    reds = list(
-        sns.color_palette("coolwarm", as_cmap=False, n_colors=n + 2)
-    )[-midpoint:]
+    blues = list(sns.color_palette("coolwarm", as_cmap=False, n_colors=n + 2))[
+        :midpoint
+    ]
+    reds = list(sns.color_palette("coolwarm", as_cmap=False, n_colors=n + 2))[
+        -midpoint:
+    ]
 
     return list(reversed(reds)) + list(reversed(blues))
 
 
 def flare(n) -> list:
     """
     Returns a list of colors based on the `flare` Matplotlib/seaborn colormap.
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/districtnumbers.py` & `gerrytools-1.1.0/gerrytools/plotting/districtnumbers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-
 from matplotlib.axes import Axes
 
 # If district numbers are to be plotted, plot those too!
 
 
 def districtnumbers(
-    base, districts, assignment="DISTRICTN", boxstyle="circle,pad=0.2",
-    fc="wheat", ec="black", lw=1 / 6, fontsize=15
+    base,
+    districts,
+    assignment="DISTRICTN",
+    boxstyle="circle,pad=0.2",
+    fc="wheat",
+    ec="black",
+    lw=1 / 6,
+    fontsize=15,
 ) -> Axes:
     """
     Plots district numbers on top of overlaid district geometries.
 
     TODO: change (x,y) coordinate pairs to representative points rather than
     centroids.
 
@@ -29,15 +34,18 @@
 
     Returns:
         Base axes object.
     """
     for district, identifier in zip(districts["geometry"], districts[assignment]):
         x, y = list(district.representative_point().coords)[0]
         base.annotate(
-            identifier, (x, y), xytext=(x, y), xycoords="data", fontsize=fontsize,
-            ha="center", va="center",
-            bbox=dict(
-                boxstyle=boxstyle, fc=fc, ec=ec, alpha=1, linewidth=lw
-            )
+            identifier,
+            (x, y),
+            xytext=(x, y),
+            xycoords="data",
+            fontsize=fontsize,
+            ha="center",
+            va="center",
+            bbox=dict(boxstyle=boxstyle, fc=fc, ec=ec, alpha=1, linewidth=lw),
         )
 
     return base
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/drawgraph.py` & `gerrytools-1.1.0/gerrytools/plotting/drawgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import networkx as nx
-from matplotlib.figure import Figure
 from matplotlib.axes import Axes
-from typing import Union, Tuple, List
+from matplotlib.figure import Figure
 
 
 def drawgraph(
-    G, ax=None, x="INTPTLON20", y="INTPTLAT20", components=False, node_size=1,
-    **kwargs
+    G, ax=None, x="INTPTLON20", y="INTPTLAT20", components=False, node_size=1, **kwargs
 ) -> Union[Axes, List[Tuple[Figure, Axes]]]:
     """
     Draws a gerrychain Graph object. Returns a single Axes object (for dual
     graphs drawn whole) and lists of `(Figure, Axes)` pairs for graphs drawn
     component-wise.
 
     Args:
@@ -32,16 +31,15 @@
     Returns:
         A tuple of `matplotlib` `(Figure, Axes)` objects, or if `components` is
         `True`, returns a list of `(Figure, Axes)` objects corresponding to each
         component.
     """
     # Create a mapping from identifiers to positions.
     positions = {
-        v: (properties[x], properties[y])
-        for v, properties in G.nodes(data=True)
+        v: (properties[x], properties[y]) for v, properties in G.nodes(data=True)
     }
 
     # If `components` is true, plot the graph component-wise. Otherwise plot
     # normally. First, set some properties common to both graphs.
     properties = {"pos": positions, "node_size": node_size}
 
     # Initialize `pairs` to None.
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/drawplan.py` & `gerrytools-1.1.0/gerrytools/plotting/drawplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
+
 from .colors import districtr
 from .districtnumbers import districtnumbers
 
 
 def drawplan(
-    districts, assignment, overlays=[], colors=None, numbers=False, lw=1 / 2,
-    fontsize=15, edgecolor="black"
+    districts,
+    assignment,
+    overlays=[],
+    colors=None,
+    numbers=False,
+    lw=1 / 2,
+    fontsize=15,
+    edgecolor="black",
 ) -> Axes:
     """
     Visualizes the districting plan defined by `assignment`.
 
     Args:
         districts (GeoDataFrame): Geometries for the districting plan. Assumes
             there is one geometry for each district.
@@ -30,33 +36,36 @@
     """
     # Sort districts by their assignment and add a column specifying the color
     # index.
     N = len(districts)
     districts = districts.to_crs("epsg:3857")
     districts[assignment] = districts[assignment].astype(int)
     districts = districts.sort_values(by=assignment)
-    districts["colorindex"] = list(range(N))
+    if colors is None:
+        districts["colorindex"] = list(range(N))
 
-    # Assign colors.
-    districts["color"] = districtr(N)
+        # Assign colors.
+        districts["color"] = districtr(N)
 
     # Plot the districts.
     base = districts.plot(
         color=districts[colors if colors else "color"],
         edgecolor="black",
-        linewidth=lw if lw is not None else 1
+        linewidth=lw if lw is not None else 1,
     )
 
     # If we have overlaid geometries, plot those too.
     if overlays:
         for overlay in overlays:
             overlay = overlay.to_crs(districts.crs)
             overlay.plot(color="None", edgecolor=edgecolor, linewidth=1 / 8, ax=base)
 
     # If the `numbers` flag is passed, plot the numbers for each district.
     if numbers:
-        base = districtnumbers(base, districts, assignment=assignment, fontsize=fontsize)
+        base = districtnumbers(
+            base, districts, assignment=assignment, fontsize=fontsize
+        )
 
     # Turn plot axes off.
     plt.axis("off")
 
     return base
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/gifs.py` & `gerrytools-1.1.0/gerrytools/plotting/gifs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import imageio
+from tqdm import tqdm
 
 from .multidimensional import multidimensional
-from tqdm import tqdm
-import imageio
 
 
 def gif_multidimensional(
-    data, proposed_info={}, labels=["X values", "Y values", "Histogram values"],
-    filename="testfile", folder="test", limits=None, DPI=150, figsize=(12, 8),
+    data,
+    proposed_info={},
+    labels=["X values", "Y values", "Histogram values"],
+    filename="testfile",
+    folder="test",
+    limits=None,
+    DPI=150,
+    figsize=(12, 8),
 ):
     r"""
     Plot many multidimensional figures in their own `{folder}/{filename}/` directory. Each
     file will represent one ensemble of plans, and this will be stitched together to create
     a gif.
 
     Args:
@@ -23,41 +29,50 @@
         filename (str): Name for the final gif, and for the folder the gif's frames are stored in
         folder (str): Folder containing all the frames/gifs.
         figsize (tuple, optional): Figure size.
 
     Returns: None.
     """
     # Get the x- and y-values.
-    xs = data['xs']
-    ys = data['ys']
+    xs = data["xs"]
+    ys = data["ys"]
 
     # TODO: Check what's actually happening here.
-    hists = data['hists']
+    hists = data["hists"]
     assert len(xs) == len(ys) == len(hists)
 
     lower_bound = 1
     upper_bound = 1
     x_limits = (lower_bound * min_of_min(xs), upper_bound * max_of_max(xs))
     y_limits = (lower_bound * min_of_min(ys), upper_bound * max_of_max(ys))
-    hist_limits = (int(lower_bound * min_of_min(hists)), int(upper_bound * max_of_max(hists)))
+    hist_limits = (
+        int(lower_bound * min_of_min(hists)),
+        int(upper_bound * max_of_max(hists)),
+    )
     limits = [x_limits, y_limits, hist_limits] if not limits else limits
 
     save = {
         "folder": folder,
         "filename": filename,
         "DPI": DPI,
     }
 
     print("Generating PNGs...")
 
     for i in tqdm(range(len(xs))):
         save["frame"] = i
         multidimensional(
-            xs[i], ys[i], hists[i], labels=labels, limits=limits,
-            proposed_info=proposed_info, figsize=figsize, save=save,
+            xs[i],
+            ys[i],
+            hists[i],
+            labels=labels,
+            limits=limits,
+            proposed_info=proposed_info,
+            figsize=figsize,
+            save=save,
         )
 
     print("Generating gif...")
     images = []
     path = f"{save['folder']}/{save['filename']}/{save['filename']}_"
     output = f"{save['folder']}/{save['filename']}.gif"
     for i in tqdm(range(len(xs))):
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/histogram.py` & `gerrytools-1.1.0/gerrytools/plotting/histogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+import random
 
 from matplotlib.axes import Axes
-import random
+
 from .bins import bins
-from .colors import defaultGray, citizenBlue, districtr
+from .colors import citizenBlue, defaultGray, districtr
 
 
 def histogram(
-    ax, scores, label=None, limits=tuple(), proposed_info={}, ticksize=12,
-    fontsize=24, jitter=False, bin_width=None
+    ax,
+    scores,
+    label=None,
+    limits=tuple(),
+    proposed_info={},
+    ticksize=12,
+    fontsize=24,
+    jitter=False,
+    bin_width=None,
 ) -> Axes:
     r"""
     Plot a histogram with the ensemble scores in bins and the proposed plans'
     scores as vertical lines. If there are many unique values, use a white border
     on the bins to distinguish, otherwise reduce the bin width to 80%.
 
     TODO: refactor `proposed_info` later to use more python builtin tools.
@@ -34,17 +42,21 @@
     Returns:
         Axes object on which the histogram is plotted.
     """
     # Put all scores into a single list.
     all_scores = scores["ensemble"] + scores["citizen"] + scores["proposed"]
     if not bin_width:
         # Get the necessary bins, ticks, labels, and bin width.
-        hist_bins, tick_bins, tick_labels, bin_width = bins(set(all_scores).union(limits))
+        hist_bins, tick_bins, tick_labels, bin_width = bins(
+            set(all_scores).union(limits)
+        )
     else:
-        hist_bins, tick_bins, tick_labels, bin_width = bins(set(all_scores).union(limits), bin_width)
+        hist_bins, tick_bins, tick_labels, bin_width = bins(
+            set(all_scores).union(limits), bin_width
+        )
 
     # Set xticks and xticklabels.
     ax.set_xticks(tick_bins)
     ax.set_xticklabels(tick_labels, fontsize=ticksize)
 
     # Adjust the visual width of the bins according to the number of observations;
     # if we have few scores, we want to adjust the look of the bins to make the
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/latexcolors.json` & `gerrytools-1.1.0/gerrytools/plotting/latexcolors.json`

 * *Files identical despite different names*

### Comparing `gerrytools-1.0.2/gerrytools/plotting/multidimensional.py` & `gerrytools-1.1.0/gerrytools/plotting/multidimensional.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from typing import Tuple
 
+import matplotlib.pyplot as plt
+from matplotlib import gridspec
 from matplotlib.axes import Axes
-from typing import Tuple
-from .scatterplot import scatterplot
+
 from .histogram import histogram
-from matplotlib import gridspec
-import matplotlib.pyplot as plt
+from .scatterplot import scatterplot
 
 
 def multidimensional(
-    x, y, hist, labels=["X values", "Y values", "Histogram values"], bin_width=1,
-    limits=None, proposed_info={}, figsize=(12, 8)
+    x,
+    y,
+    hist,
+    labels=["X values", "Y values", "Histogram values"],
+    bin_width=1,
+    limits=None,
+    proposed_info={},
+    figsize=(12, 8),
 ) -> Tuple[Axes, Axes]:
     r"""
     Plot a multidimensional figure, comparing two metrics as a scatterplot above
     and one metric as a histogram, below.
 
     Args:
         ax (Axes): `Axes` object on which the histogram is plotted.
@@ -33,31 +40,39 @@
     _ = plt.subplots(figsize=figsize)
     gs = gridspec.GridSpec(2, 1, height_ratios=[2, 1])
 
     scatter_limits = limits[:2] if limits else set()
     scatter_labels = labels[:2]
     scatter_ax = plt.subplot(gs[0])
     scatter_ax = scatterplot(
-        scatter_ax, x, y, labels=scatter_labels, limits=scatter_limits,
+        scatter_ax,
+        x,
+        y,
+        labels=scatter_labels,
+        limits=scatter_limits,
         proposed_info=proposed_info,
     )
 
     scores = {
         "ensemble": hist,
         "citizen": [],
         "proposed": proposed_info["hist"] if proposed_info else [],
     }
 
     hist_limits = limits[-1] if limits else set()
     hist_label = labels[-1]
     hist_ax = plt.subplot(gs[1])
     hist_ax = histogram(
-        hist_ax, scores, label=hist_label, limits=hist_limits, proposed_info=proposed_info,
+        hist_ax,
+        scores,
+        label=hist_label,
+        limits=hist_limits,
+        proposed_info=proposed_info,
         bin_width=bin_width,
     )
 
     hist_ax.get_yaxis().set_visible(False)
-    hist_ax.spines['top'].set_visible(False)
-    hist_ax.spines['right'].set_visible(False)
-    hist_ax.spines['left'].set_visible(False)
+    hist_ax.spines["top"].set_visible(False)
+    hist_ax.spines["right"].set_visible(False)
+    hist_ax.spines["left"].set_visible(False)
 
     return scatter_ax, hist_ax
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/scatterplot.py` & `gerrytools-1.1.0/gerrytools/plotting/scatterplot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-from matplotlib.axes import Axes
 import numpy as np
+from matplotlib.axes import Axes
+
+from .colors import districtr
 
 
-def scatterplot(ax, x, y, labels=None, limits=set(), proposed_info={}, bins=None, axis_range=None) -> Axes:
+def scatterplot(
+    ax, x, y, labels=None, limits=set(), bins=None, axis_range=None
+) -> Axes:
     r"""
     Plot a scatterplot comparing two scores, with the proposed plans'
     scores as points.
 
     Args:
         ax (Axes): `Axes` object on which the histogram is plotted.
-        x (list): Score on the x-axis.
-        y (list): score on the y-axis.
+        x (list): Score on the x-axis. This will be a list of lists, where each
+           sub-list corresponds to the scores for an individual plan.
+        y (list): Score on the y-axis. This will be a list of lsits where each
+           sub-list corresponds to the scores for an individual plan.
         labels (list, optional): Strings for x- and y-axis labels.
         limits (tuple, optional): Axis limits (specify to force plot to extend to
             these limits).
-        proposed_info (dict, optional): Dictionary with keys of `colors`, `names`,
-            `x`, `y`; the \(i\)th color in `color` corresponds to the \(i\)th name
-            in `names`, which corresponds to the \(i\)th value in `x` and `y`.
-
+        colors (list, optional): A list of colors where the ith color corresponds
+          to the ith score sub-list.
     Returns:
         Axes object on which the scatterplot is plotted.
     """
-    if not bins:
-        bins = [
-            np.arange(int(min(x)), int(max(x)) + 1),
-            np.arange(int(min(y)), int(max(y)) + 1)
-        ]
-
-    h, xedges, yedges, image = ax.hist2d(
-        x, y, bins=bins, cmap='Greys', range=axis_range,
-    )
 
-    # Shift bins over by 0.5 to center labels in the middle of the bin.
-    # TODO: This only works for bins of width 1 — need to fix for general bid width.
-    ax.set_xticks([x + 0.5 for x in xedges])
-    ax.set_xticklabels(xedges)
-    ax.set_yticks([y + 0.5 for y in yedges])
-    ax.set_yticklabels(yedges)
-
-    if proposed_info:
-        for i in range(len(proposed_info['names'])):
-            x = proposed_info['x'][i]
-            y = proposed_info['y'][i]
+    for x_score, y_score in zip(x, y):
+        for i in range(len(x_score)):
+            x = x_score[i]
+            y = y_score[i]
             ax.scatter(
                 x + 0.5,
                 y + 0.5,
-                label=f"{proposed_info['names'][i]} ({x}, {y})",
-                color=proposed_info['colors'][i],
+                color=f"{districtr(i).pop()}",
                 s=150,
-                edgecolor='black',
+                edgecolor="black",
             )
-        ax.legend()
+    ax.legend()
 
     if labels:
         ax.set_xlabel(labels[0], fontsize=24)
         ax.set_ylabel(labels[1], fontsize=24)
     if limits:
         ax.set_xlim(limits[0])
         ax.set_ylim(limits[1])
+
+    # Shift bins over by 0.5 to center labels in the middle of the bin.
+    x_min = min([min(x_point) for x_point in x])
+    x_max = max([max(x_point) for x_point in x])
+    y_min = min([min(y_point) for y_point in y])
+    y_max = max([max(y_point) for y_point in y])
+    xedges = np.arange(x_min, x_max + 1, 1)
+    yedges = np.arange(y_min, y_max + 1, 1)
+    # TODO: This only works for bins of width 1 — need to fix for general bid width.
+    ax.set_xticks([x + 0.5 for x in xedges])
+    ax.set_xticklabels(xedges)
+    ax.set_yticks([y + 0.5 for y in yedges])
+    ax.set_yticklabels(yedges)
+
     return ax
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/sealevel.py` & `gerrytools-1.1.0/gerrytools/plotting/sealevel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import random
 
+import numpy as np
 from matplotlib.axes import Axes
+
 from .colors import defaultGray
 from .utils import sort_elections
-import numpy as np
-import random
 
 
 def sealevel(ax, scores, num_districts, proposed_info, ticksize=12) -> Axes:
     r"""
     Plot a sea level plot: Each plan is a line across our elections on the
     x-axis, with Democratic vote share on the y-axis. The statewide Dem. vote
     share (proportionality) is plotted as a thick blue line.
@@ -25,29 +26,38 @@
     elections = sort_elections(scores["statewide"].keys())
     shares_by_plan = {plan: [] for plan in scores}
     for plan in scores:
         for election in elections:
             shares_by_plan[plan].append(scores[plan][election])
 
     ax.plot(
-        shares_by_plan['statewide'], marker='o', markersize=10, lw=5,
+        shares_by_plan["statewide"],
+        marker="o",
+        markersize=10,
+        lw=5,
         label="Proportionality",
     )
 
-    for i, plan in enumerate(proposed_info['names']):
+    for i, plan in enumerate(proposed_info["names"]):
         for j in range(len(shares_by_plan[plan])):
-            if len(set([shares_by_plan[plan][j] for plan in shares_by_plan.keys()])) > 1:
+            if (
+                len(set([shares_by_plan[plan][j] for plan in shares_by_plan.keys()]))
+                > 1
+            ):
                 jitter = random.uniform(-0.02, 0.02)
             else:
                 0
 
             shares_by_plan[plan][j] = shares_by_plan[plan][j] + jitter
 
         ax.plot(
-            shares_by_plan[plan], marker='o', linestyle='--', color=proposed_info['colors'][i],
+            shares_by_plan[plan],
+            marker="o",
+            linestyle="--",
+            color=proposed_info["colors"][i],
             label=plan,
         )
 
     ax.legend()
 
     if num_districts <= 20:
         yticks = np.arange(0, 1 + 1 / num_districts, 1 / num_districts)
```

### Comparing `gerrytools-1.0.2/gerrytools/plotting/violin.py` & `gerrytools-1.1.0/gerrytools/plotting/violin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+import random
 
-from matplotlib.axes import Axes
 import numpy as np
-import random
-from .colors import defaultGray, citizenBlue, districtr
+from matplotlib.axes import Axes
+
+from .colors import citizenBlue, defaultGray, districtr
 
 
 def violin(
-    ax, scores, xticklabels=None, labels=None, proposed_info={}, percentiles=(1, 99), rotation=0,
-    ticksize=12, jitter=1 / 3
+    ax,
+    scores,
+    xticklabels=None,
+    labels=None,
+    proposed_info={},
+    percentiles=(1, 99),
+    rotation=0,
+    ticksize=12,
+    jitter=1 / 3,
 ) -> Axes:
     r"""
     Plot a violin plot, which takes `scores` — a dictionary where each value (corresponding to
     an ensemble, citizens' ensemble, or proposed plans), will be a list of lists, where each
     sublist will be its own violin. Proposed scores will be plotted as colored circles on
     their respective violin. Color the violins conditioned on the kind of the scores
     (ensemble or citizen), and trim each sublist to only the values between the percentiles.
@@ -62,38 +70,44 @@
     for pc in parts["bodies"]:
         pc.set_facecolor(facecolor)
         pc.set_edgecolor("black")
         pc.set_alpha(1)
 
     # Set xticks, xlabels, and x-axis limits.
     if not xticklabels:
-        xticklabels = range(1, len(scores['ensemble']) + 1)
+        xticklabels = range(1, len(scores["ensemble"]) + 1)
     ax.set_xticks(range(1, len(ensemble) + 1))
     ax.set_xticklabels(xticklabels, fontsize=ticksize, rotation=rotation)
     ax.set_xlim(0.5, len(ensemble) + 0.5)
 
     # Plot each proposed plan individually, adjusting its detail points by
     # a value drawn from the uniform distribution of specified width centered on
     # the index of the violin.
     if scores["proposed"]:
         for violin in range(len(scores["proposed"])):
             for plan, score in enumerate(scores["proposed"][violin]):
                 # Horizontally jitter proposed scores if there are multiple scores
                 # at the same height.
-                jitter_val = random.uniform(-jitter, jitter) if scores["proposed"][violin].count(score) > 1 else 0
+                jitter_val = (
+                    random.uniform(-jitter, jitter)
+                    if scores["proposed"][violin].count(score) > 1
+                    else 0
+                )
                 ax.scatter(
                     violin + 1 + jitter_val,
                     score,
-                    color=districtr(plan + 1).pop(),
-                    edgecolor='black',
+                    color=scores["proposed"]["colors"][violin]
+                    if scores["proposed"]["colors"]
+                    else districtr(plan + 1).pop(),
+                    edgecolor="black",
                     s=100,
                     alpha=0.9,
                     label=proposed_info["names"][plan] if violin == 0 else None,
                 )
         ax.legend()
-        ax.grid(axis='x')
+        ax.grid(axis="x")
 
     if labels:
         ax.set_xlabel(labels[0], fontsize=24)
         ax.set_ylabel(labels[1], fontsize=24)
 
     return ax
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/__init__.py` & `gerrytools-1.1.0/gerrytools/scoring/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,45 @@
-
 """
 Basic functionality for evaluating districting plans.
 """
 
+from .contiguity import contiguous, unassigned_units
+from .demographics import demographic_updaters
+from .population import deviations, unassigned_population
 from .scores import (
-    splits, pieces, competitive_contests, swing_districts, party_districts,
-    opp_party_districts, party_wins_by_district, seats, aggregate_seats,
-    responsive_proportionality, stable_proportionality, efficiency_gap,
-    simplified_efficiency_gap, mean_median, partisan_bias, partisan_gini,
-    summarize, summarize_many, demographic_shares, demographic_tallies,
-    gingles_districts, max_deviation, eguia
+    aggregate_seats,
+    competitive_contests,
+    convex_hull,
+    cut_edges,
+    demographic_shares,
+    demographic_tallies,
+    efficiency_gap,
+    eguia,
+    gingles_districts,
+    max_deviation,
+    mean_median,
+    opp_party_districts,
+    partisan_bias,
+    partisan_gini,
+    party_districts,
+    party_wins_by_district,
+    pieces,
+    polsby_popper,
+    pop_polygon,
+    reock,
+    responsive_proportionality,
+    schwartzberg,
+    seats,
+    simplified_efficiency_gap,
+    splits,
+    stable_proportionality,
+    summarize,
+    summarize_many,
+    swing_districts,
 )
-from .population import deviations, unassigned_population
-from .contiguity import unassigned_units, contiguous
-from .demographics import demographic_updaters
-from .reock import reock
 
 __all__ = [
     "splits",
     "pieces",
     "competitive_contests",
     "swing_districts",
     "party_districts",
@@ -42,8 +63,13 @@
     "reock",
     "demographic_updaters",
     "demographic_tallies",
     "demographic_shares",
     "gingles_districts",
     "max_deviation",
     "eguia",
+    "polsby_popper",
+    "schwartzberg",
+    "convex_hull",
+    "pop_polygon",
+    "cut_edges",
 ]
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/contiguity.py` & `gerrytools-1.1.0/gerrytools/scoring/contiguity.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,13 +37,14 @@
 
     # Retrive the length of the assignment; this corresponds to the number of
     # units which have an assignment key.
     total = len(P.graph.nodes())
 
     # Next, check for "bad" assignments for units: this includes empty strings
     # and NaNs, for now.
-    units_assigned_well = len({
-        k: v
-        for k, v in assignment.items() if v not in ["nan", "NaN", ""]
-    })
+    units_assigned_well = len(
+        {k: v for k, v in assignment.items() if v not in ["nan", "NaN", ""]}
+    )
 
-    return 1 - (units_assigned_well / total) if not raw else (total - units_assigned_well)
+    return (
+        1 - (units_assigned_well / total) if not raw else (total - units_assigned_well)
+    )
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/demographics.py` & `gerrytools-1.1.0/gerrytools/scoring/demographics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+from typing import Iterable
 
-from gerrychain.updaters import Tally
 from gerrychain import Partition
-from typing import Iterable
-from .types import DistrictWideScoreValue, PlanWideScoreValue, Numeric
+from gerrychain.updaters import Tally
+
+from .types import DistrictWideScoreValue, Numeric, PlanWideScoreValue
 
 
-def demographic_updaters(demographic_keys: Iterable[str], aliases: Iterable[str] = None):
+def demographic_updaters(
+    demographic_keys: Iterable[str], aliases: Iterable[str] = None
+):
     updaters = {}
     aliases = aliases if aliases else demographic_keys
-    for (key, alias) in zip(demographic_keys, aliases):
+    for key, alias in zip(demographic_keys, aliases):
         updaters[alias] = Tally(key, alias=alias)
     return updaters
 
 
 def _tally_pop(part: Partition, pop_col: str) -> DistrictWideScoreValue:
     return part[pop_col]
 
 
-def _pop_shares(part: Partition, subpop_col: str, totpop_col: str) -> DistrictWideScoreValue:
+def _pop_shares(
+    part: Partition, subpop_col: str, totpop_col: str
+) -> DistrictWideScoreValue:
     total_pops = part[totpop_col]
     return {d: part[subpop_col][d] / pop for d, pop in total_pops.items()}
 
 
-def _gingles_districts(part: Partition, subpop_col: str, totpop_col: str, threshold: float = 0.5) -> PlanWideScoreValue:
+def _gingles_districts(
+    part: Partition, subpop_col: str, totpop_col: str, threshold: float = 0.5
+) -> PlanWideScoreValue:
     subpop_shares = _pop_shares(part, subpop_col, totpop_col)
     return sum([share >= threshold for share in subpop_shares.values()])
 
 
 def _max_deviation(part: Partition, totpop_col: str, pct: bool = False) -> Numeric:
     totpop_counts = _tally_pop(part, totpop_col)
     ideal_population = sum(totpop_counts.values()) / len(part)
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/population.py` & `gerrytools-1.1.0/gerrytools/scoring/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from gerrychain.constraints.validity import deviation_from_ideal as deviation
 from gerrychain.updaters import Tally
 
 
 def deviations(P, popcolumn) -> dict:
     """
     Determines the districting plan's population deviation percentages.
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/scores.py` & `gerrytools-1.1.0/gerrytools/scoring/scores.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,109 +1,173 @@
-from .splits import _splits, _pieces
-from .demographics import (
-    _pop_shares,
-    _tally_pop,
-    _gingles_districts,
-    _max_deviation,
+import gzip
+import json
+from functools import partial
+from typing import Dict, Iterable, List, Mapping, Optional, Union
+
+from geopandas import GeoDataFrame
+from gerrychain import Graph, Partition
+from tqdm import tqdm
+
+from gerrytools.geometry.compactness import (
+    _convex_hull,
+    _cut_edges,
+    _polsby_popper,
+    _pop_polygon,
+    _reock,
+    _schwartzberg,
 )
+
+from .demographics import _gingles_districts, _max_deviation, _pop_shares, _tally_pop
 from .partisan import (
-    _competitive_contests,
-    _swing_districts,
-    _party_districts,
-    _opp_party_districts,
-    _party_wins_by_district,
-    _seats,
     _aggregate_seats,
+    _competitive_contests,
     _efficiency_gap,
-    _simplified_efficiency_gap,
+    _eguia,
     _mean_median,
+    _opp_party_districts,
     _partisan_bias,
     _partisan_gini,
-    _eguia,
-    _stable_proportionality,
+    _party_districts,
+    _party_wins_by_district,
     _responsive_proportionality,
+    _seats,
+    _simplified_efficiency_gap,
+    _stable_proportionality,
+    _swing_districts,
 )
-from functools import partial
-from gerrychain import Partition, Graph
-from typing import Iterable, List, Mapping, Dict, Union
-from tqdm import tqdm
-import gzip
-import json
-from .types import Score, ScoreValue, Callable
+from .splits import _pieces, _splits
+from .types import Callable, Score, ScoreValue
 
 
-def summarize(part: Partition, scores: Iterable[Score]) -> Dict[str, ScoreValue]:
+def summarize(
+    part: Partition,
+    scores: Iterable[Score],
+    gdf: Optional[GeoDataFrame] = None,
+    join_on: Optional[str] = None,
+) -> Dict[str, ScoreValue]:
     """
     Summarize the given partition by the passed scores.
 
     Args:
         part (Partition): The plan to summarize.
         scores (Iterable[Score]): Which scores to include in the summary.
+        gdf (GeoDataFrame): Geometries of nodes in the dual graph used by `part`.
+            Only necessary when using scoring functions that rely on dissolved
+            district geometries (most geometric scoring functions).
+        join_on (str): Field used to join `part.graph` to `gdf`.
+            If not specified, geometries are joined by matching the index of `gdf`
+            to the node keys of `part.graph`.
+
+    Raises:
+        ValueError: If `gdf` is not specified and at least one score in `scores`
+            is dissolved.
 
     Returns:
         A dictionary that maps score names to the corresponding ScoreValues of the score functions
         applied to the plan.
 
         ie.
         `{"cut_edges": 4050, "num_party_seats": 3, ... }`
     """
+    if any(score.dissolved for score in scores):
+        if gdf is None:
+            raise ValueError("Geometries must be provided for dissolved scores.")
+
+        if join_on is None:
+            assignment = dict(part.assignment)
+            gdf = gdf.copy(deep=False)
+        else:
+            assignment = {
+                part.graph.nodes[node][join_on]: label
+                for node, label in part.assignment.items()
+            }
+            gdf = gdf.set_index(join_on)
+
+        gdf["assignment"] = assignment
+        dissolved_gdf = gdf.dissolve(by="assignment")
+    else:
+        dissolved_gdf = None
+
     summary = {}
     for score in scores:
-        summary[score.name] = score.apply(part)
+        if score.dissolved:
+            summary[score.name] = score.apply(dissolved_gdf)
+        else:
+            summary[score.name] = score.apply(part)
     return summary
 
 
 def summarize_many(
-    parts: Iterable[Partition], scores: Iterable[Score], plan_names: List[str] = [],
-    output_file: str = None, compress: bool = False, verbose: bool = False
+    parts: Iterable[Partition],
+    scores: Iterable[Score],
+    gdf: Optional[GeoDataFrame] = None,
+    join_on: Optional[str] = None,
+    plan_names: List[str] = None,
+    output_file: str = None,
+    compress: bool = False,
+    verbose: bool = False,
 ) -> Union[List[Dict[str, ScoreValue]], None]:
     """
     Summarize the given partitions by the passed scores.
 
     Args:
         parts (Iterable[Partition]): The plans to summarize.
         scores (Iterable[Score]): Which scores to include in the summaries.
+        gdf (GeoDataFrame): Geometries of nodes in the dual graph used by each partition
+            in `parts`. Only necessary when using scoring functions that rely on
+            dissolved district geometries (most geometric scoring functions).
+        join_on (str): Field used to join the graph associated with the partitions
+            in `parts` to `gdf`.  If not specified, geometries are joined by matching
+            the index of `gdf` to the node keys of the graph.
         plan_names (Iterable[str], optional): Plan identifiers, corresponding to
             plan by index. If no plan name exists for a given plan's index, the
-            plan's index is used as the identifier. Default is `[]`, plans
+            plan's index is used as the identifier. Default is `None`, plans
             identified by index.
         output_file (str, optional): Name of file to save the results jsonl
             encoding of the scores. If None, returns a list of the dictionary
             summary of each plan. Defaults to None.
         compress (bool, optional): Whether to compress the output file with gzip.
             Default is False.
 
     Returns:
         A list dictionaries that maps score names to the corresponding ScoreValues
         of the score functions applied to each plan, if NO output file is passed.
         If an output file IS specified, the plan summaries are written to file
         and the function is void.
     """
+    if plan_names is None:
+        plan_names = []
+
     if output_file is None:
         if verbose:
             result = []
             for part in tqdm(parts):
-                result.append(summarize(part, scores=scores))
+                result.append(summarize(part, scores=scores, gdf=gdf, join_on=join_on))
             return result
         return [summarize(part, scores=scores) for part in parts]
     else:
-        with gzip.open(f"{output_file}.gz", "wt") if compress else open(output_file, "w") as fout:
+        with gzip.open(f"{output_file}.gz", "wt") if compress else open(
+            output_file, "w"
+        ) as fout:
             iterator = tqdm(enumerate(parts)) if verbose else enumerate(parts)
             for i, part in iterator:
-                plan_details = summarize(part, scores=scores)
+                plan_details = summarize(part, scores=scores, gdf=gdf, join_on=join_on)
                 try:
                     plan_details["id"] = plan_names[i]
                 except BaseException:
                     plan_details["id"] = i
                 fout.write(json.dumps(plan_details) + "\n")
 
 
 def splits(
-    unit: str, names: bool = False, popcol: str = None, how: str = "pandas",
-    alias: str = None
+    unit: str,
+    names: bool = False,
+    popcol: str = None,
+    how: str = "pandas",
+    alias: str = None,
 ) -> Score:
     """
     Score representing the number of units split by the districting plan.
 
     Bear in mind that this calculates the number of *unit splits*, not the number
     of *units split*: for example, if a district divides a county into three
     pieces, the former reports two splits (as a unit divided into three pieces is
@@ -127,21 +191,24 @@
         partition and returns a PlanWideScoreValue for the number of splits.
     """
     if alias is None:
         alias = unit
 
     return Score(
         f"{alias}_splits",
-        partial(_splits, unit=unit, how=how, popcol=popcol, names=names)
+        partial(_splits, unit=unit, how=how, popcol=popcol, names=names),
     )
 
 
 def pieces(
-    unit: str, names: bool = False, popcol: str = None, how: str = "pandas",
-    alias: str = None
+    unit: str,
+    names: bool = False,
+    popcol: str = None,
+    how: str = "pandas",
+    alias: str = None,
 ) -> Score:
     """
     Score representing the number of "unit pieces" produced by the plan. For example,
     consider a state with 100 counties. Suppose that one county is split twice,
     and another once. Then, there are 3 + 2 = 5 "pieces," disregarding the
     counties kept whole.
 
@@ -168,21 +235,23 @@
         partition and returns a PlanWideScoreValue for the number of pieces.
     """
     if alias is None:
         alias = unit
 
     return Score(
         f"{alias}_pieces",
-        partial(_pieces, unit=unit, how=how, popcol=popcol, names=names)
+        partial(_pieces, unit=unit, how=how, popcol=popcol, names=names),
     )
 
 
 def competitive_contests(
-    election_cols: Iterable[str], party: str, points_within: float = 0.03,
-    alias: str = None
+    election_cols: Iterable[str],
+    party: str,
+    points_within: float = 0.03,
+    alias: str = None,
 ) -> Score:
     """
     Score representing the number of competitive contests in a plan.
 
     Args:
         election_cols (Iterable[str]): The names of the election updaters over which to compute
             results for.
@@ -195,17 +264,19 @@
         partition and returns a PlanWideScoreValue for the number of competitive districts.
     """
     if alias is None:
         alias = f"competitive_contests_{points_within}"
     return Score(
         alias,
         partial(
-            _competitive_contests, election_cols=election_cols, party=party,
-            points_within=points_within
-        )
+            _competitive_contests,
+            election_cols=election_cols,
+            party=party,
+            points_within=points_within,
+        ),
     )
 
 
 def swing_districts(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing the number of swing districts in a plan.  A swing districts is one that is
     not solely won by a single party over a set of elections.
@@ -217,15 +288,15 @@
 
     Returns:
         A score object with name `"swing_districts"` and associated function that takes a partition
         and returns a PlanWideScoreValue for the number of swing districts.
     """
     return Score(
         "swing_districts",
-        partial(_swing_districts, election_cols=election_cols, party=party)
+        partial(_swing_districts, election_cols=election_cols, party=party),
     )
 
 
 def party_districts(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing the number of districts in a plan that are always won by the POV party over
     a set of elections.
@@ -237,15 +308,15 @@
 
     Returns:
         A score object with name `"party_districts"` and associated function that takes a partition
         and returns a PlanWideScoreValue for the number of safe POV party districts.
     """
     return Score(
         "party_districts",
-        partial(_party_districts, election_cols=election_cols, party=party)
+        partial(_party_districts, election_cols=election_cols, party=party),
     )
 
 
 def opp_party_districts(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing the number of districts in a plan that are always won by the opposition party
     over a set of elections.
@@ -260,15 +331,15 @@
 
     Returns:
         A score object with name `"opp_party_districts"` and associated function that takes a
         partition and returns a PlanWideScoreValue for the number of safe opposition party districts.
     """
     return Score(
         "opp_party_districts",
-        partial(_opp_party_districts, election_cols=election_cols, party=party)
+        partial(_opp_party_districts, election_cols=election_cols, party=party),
     )
 
 
 def party_wins_by_district(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing how many elections the POV party won in each district in a given plan.
 
@@ -280,15 +351,15 @@
     Returns:
         A score object with name `"party_wins_by_district"` and associated function that takes a
         partition and returns a DistrictWideScoreValue for the number of elections won by the POV
         party in each district.
     """
     return Score(
         "party_wins_by_district",
-        partial(_party_wins_by_district, election_cols=election_cols, party=party)
+        partial(_party_wins_by_district, election_cols=election_cols, party=party),
     )
 
 
 def seats(election_cols: Iterable[str], party: str, mean: bool = False) -> Score:
     """
     Score representing how many seats (districts) within a given plan the POV party won in each
     election
@@ -304,15 +375,15 @@
         A score object with name `"{party}_seats"` and associated function that takes a partition and
         returns an ElectionWideScoreValue for the number of seats won by the POV party for each
         election.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}{party}_seats",
-        partial(_seats, election_cols=election_cols, party=party, mean=mean)
+        partial(_seats, election_cols=election_cols, party=party, mean=mean),
     )
 
 
 def aggregate_seats(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing how many total seats (districts) within a given plan the POV party won across
     elections.
@@ -325,15 +396,15 @@
     Returns:
         A score object with name `"aggregate_{party}_seats"` and associated function that takes a
         partition and returns an PlanWideScoreValue for the total number of seats won by the POV
         party across elections.
     """
     return Score(
         f"aggregate_{party}_seats",
-        partial(_aggregate_seats, election_cols=election_cols, party=party)
+        partial(_aggregate_seats, election_cols=election_cols, party=party),
     )
 
 
 def responsive_proportionality(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing how many the responsive proportionality across a set of elections.
 
@@ -345,17 +416,15 @@
     Returns:
         A score object with name `"responsive_proportionality"` and associated function that takes a
         partition and returns an PlanWideScoreValue for the responsive proportionality across the
         elections.
     """
     return Score(
         "responsive_proportionality",
-        partial(
-            _responsive_proportionality, election_cols=election_cols, party=party
-        )
+        partial(_responsive_proportionality, election_cols=election_cols, party=party),
     )
 
 
 def stable_proportionality(election_cols: Iterable[str], party: str) -> Score:
     """
     Score representing how many the stable proportionality across a set of elections.
 
@@ -367,15 +436,15 @@
     Returns:
         A score object with name `"stable_proportionality"` and associated function that takes a
         partition and returns an PlanWideScoreValue for the stable proportionality across the
         elections.
     """
     return Score(
         "stable_proportionality",
-        partial(_stable_proportionality, election_cols=election_cols, party=party)
+        partial(_stable_proportionality, election_cols=election_cols, party=party),
     )
 
 
 def efficiency_gap(election_cols: Iterable[str], mean: bool = False) -> Score:
     """
     Score representing the efficiency gap metric of a plan with respect to a set of elections.
 
@@ -388,19 +457,21 @@
     Returns:
         A score object with name `"efficiency_gap"`  and associated function that takes a partition
         and returns a PlanWideScoreValue for efficiency gap metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}efficiency_gap",
-        partial(_efficiency_gap, election_cols=election_cols, mean=mean)
+        partial(_efficiency_gap, election_cols=election_cols, mean=mean),
     )
 
 
-def simplified_efficiency_gap(election_cols: Iterable[str], party: str, mean: bool = False) -> Score:
+def simplified_efficiency_gap(
+    election_cols: Iterable[str], party: str, mean: bool = False
+) -> Score:
     """
     Score representing the simplified efficiency gap metric of a plan with respect to a set of elections.
     The original formulation of efficiency gap quantifies the difference in "wasted" votes for the two
     parties across the state, as a share of votes cast. This is sensitive to turnout effects. The
     simplified score is equal to standard efficiency gap when the districts have equal turnout.
     Args:
         election_cols (Iterable[str]): The names of the election updaters over which to compute
@@ -412,16 +483,19 @@
         A score object with name `"efficiency_gap"`  and associated function that takes a partition
         and returns a PlanWideScoreValue for efficiency gap metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}simplified_efficiency_gap",
         partial(
-            _simplified_efficiency_gap, election_cols=election_cols, party=party, mean=mean
-        )
+            _simplified_efficiency_gap,
+            election_cols=election_cols,
+            party=party,
+            mean=mean,
+        ),
     )
 
 
 def mean_median(election_cols: Iterable[str], mean: bool = False) -> Score:
     """
     Score representing the mean median metric of a plan with respect to a set of elections.
 
@@ -434,15 +508,15 @@
     Returns:
         A score object with name `"mean_median"` and associated function that takes a partition and
         returns a PlanWideScoreValue for the mean median metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}mean_median",
-        partial(_mean_median, election_cols=election_cols, mean=mean)
+        partial(_mean_median, election_cols=election_cols, mean=mean),
     )
 
 
 def partisan_bias(election_cols: Iterable[str], mean: bool = False) -> Score:
     """
     Score representing the partitisan bias metric of a plan with respect to a set of elections.
 
@@ -454,15 +528,15 @@
     Returns:
         A score object with name `"partisan_bias"` and associated function that takes a partition and
         returns a PlanWideScoreValue for partisan bias metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}partisan_bias",
-        partial(_partisan_bias, election_cols=election_cols, mean=mean)
+        partial(_partisan_bias, election_cols=election_cols, mean=mean),
     )
 
 
 def partisan_gini(election_cols: Iterable[str], mean: bool = False) -> Score:
     """
     Score representing the partisan gini metric of a plan with respect to a set
     of elections.
@@ -478,22 +552,26 @@
         A score object with name `"partisan_gini"` and associated function that
         takes a partition and
         returns a PlanWideScoreValue for the partisan gini metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}partisan_gini",
-        partial(_partisan_gini, election_cols=election_cols, mean=mean)
+        partial(_partisan_gini, election_cols=election_cols, mean=mean),
     )
 
 
 def eguia(
-    election_cols: Iterable[str], party: str, graph: Graph,
+    election_cols: Iterable[str],
+    party: str,
+    graph: Graph,
     updaters: Mapping[str, Callable[[Partition], ScoreValue]],
-    county_col: str, totpop_col: str = "population", mean: bool = False
+    county_col: str,
+    totpop_col: str = "population",
+    mean: bool = False,
 ) -> Score:
     """
     Score representing the Equia metric of a plan with respect to a set of elections.
 
     Args:
         election_cols (Iterable[str]): The names of the election updaters over which to compute
             results for.
@@ -516,35 +594,36 @@
     """
     county_part = Partition(graph, county_col, updaters=updaters)
     prefix = "mean_" if mean else ""
 
     return Score(
         f"{prefix}eguia",
         partial(
-            _eguia, election_cols=election_cols, party=party, county_part=county_part,
-            totpop_col=totpop_col, mean=mean
-        )
+            _eguia,
+            election_cols=election_cols,
+            party=party,
+            county_part=county_part,
+            totpop_col=totpop_col,
+            mean=mean,
+        ),
     )
 
 
 def demographic_tallies(population_cols: Iterable[str]) -> List[Score]:
     """
     A list of scores representing population tallies.
 
     Args:
         population_cols (Iterable[str]): The population column to create tallies for.
 
     Returns:
         A list of score objects named by `"{column}"` and with associated functions that take a partition
         and return a DistrictWideScoreValue for the demographic totals of each district.
     """
-    return [
-        Score(col, partial(_tally_pop, pop_col=col))
-        for col in population_cols
-    ]
+    return [Score(col, partial(_tally_pop, pop_col=col)) for col in population_cols]
 
 
 def demographic_shares(population_cols: Mapping[str, Iterable[str]]) -> List[Score]:
     """
     A list of scores representing subgroup population shares.
 
     Args:
@@ -557,22 +636,29 @@
         A list of score objects named with the pattern `"{column}_share"` and with associated
         functions that take a partition and return a DistrictWideScoreValue for the demographic
         share of each district.
     """
     scores = []
 
     for totalpop_col, subpop_cols in population_cols.items():
-        scores.extend([
-            Score(f"{col}_share", partial(_pop_shares, subpop_col=col, totpop_col=totalpop_col))
-            for col in subpop_cols
-        ])
+        scores.extend(
+            [
+                Score(
+                    f"{col}_share",
+                    partial(_pop_shares, subpop_col=col, totpop_col=totalpop_col),
+                )
+                for col in subpop_cols
+            ]
+        )
     return scores
 
 
-def gingles_districts(population_cols: Mapping[str, Iterable[str]], threshold: float = 0.5) -> List[Score]:
+def gingles_districts(
+    population_cols: Mapping[str, Iterable[str]], threshold: float = 0.5
+) -> List[Score]:
     """
     A list of scores representing the number of districts where a sub-population share is above
     a given threshold.  When the threshold is 50% these are commonly called Gingles' Districts.
 
     Args:
         population_cols (Mapping[str, Iterable[str]]): A mapping encoding the total population group
             divisor as well as the subgroups to create gingles district counters for.  The mapping
@@ -583,27 +669,101 @@
         A list of score objects named with the pattern `"{column}_gingles_districts"` and with
         associated functions that take a partition and return a PlanWideScoreValue for the number of
         districts above the population share threshold.
     """
     scores = []
 
     for totalpop_col, subpop_cols in population_cols.items():
-        scores.extend([
-            Score(f"{col}_gingles_districts", partial(_gingles_districts, subpop_col=col,
-                                                      totpop_col=totalpop_col, threshold=threshold))
-            for col in subpop_cols
-        ])
+        scores.extend(
+            [
+                Score(
+                    f"{col}_gingles_districts",
+                    partial(
+                        _gingles_districts,
+                        subpop_col=col,
+                        totpop_col=totalpop_col,
+                        threshold=threshold,
+                    ),
+                )
+                for col in subpop_cols
+            ]
+        )
     return scores
 
 
+def reock() -> Score:
+    """
+    Returns the reock score for each district in a plan.
+    Returns:
+        A dictionary with districts as keys and reock scores as values.
+    """
+    return Score("reock", _reock, dissolved=True)
+
+
+def polsby_popper() -> Score:
+    """
+    Returns the polsby-popper score for each district in a plan.
+
+    Returns:
+        A dictionary with districts as keys and polsby-popper scores as values.
+    """
+
+    return Score("polsby_popper", _polsby_popper, dissolved=True)
+
+
+def schwartzberg() -> Score:
+    """
+    Returns the schwartzberg score for each district in a plan.
+    Returns:
+        A dictionary with districts as keys and schwartzberg scores as values.
+    """
+    return Score("schwartzberg", _schwartzberg, dissolved=True)
+
+
+def convex_hull() -> Score:
+    """
+    Returns the convex-hull score for each district in a plan.
+
+    Returns:
+        A dictionary with districts as keys and convex-hull scores as values.
+    """
+    return Score("convex_hull", _convex_hull, dissolved=True)
+
+
+def pop_polygon(block_gdf: GeoDataFrame, pop_col: str = "TOTPOP20") -> Score:
+    """
+    Returns the population polygon compactness metric for each district in a plan.
+    Args:
+        block_gdf (GeoDataFrame): Block level shapefile for the state.
+        pop_col (str): Population column reflected in block_gdf and gdf.
+    Returns:
+        A dictionary with districts as keys and population polygon scores as values.
+    """
+    return Score(
+        "pop_polygon",
+        partial(_pop_polygon, block_gdf=block_gdf, pop_col=pop_col),
+        dissolved=True,
+    )
+
+
+def cut_edges() -> Score:
+    """
+    Returns the number of cut edges in a plan.
+    """
+    return Score("cut_edges", partial(_cut_edges))
+
+
 def max_deviation(totpop_col: str, pct: bool = False) -> Score:
     """
     Returns the maximum deviation from ideal population size among all the districts.
     If `pct`, return the deviation as a percentage of ideal population size.
 
     Args:
         totpop_col (str, optional): The name of the updater that computes total population by
             district.
         pct (bool): Whether to return the maximum deviation as a count or as a percentage of
                     ideal district size.
     """
-    return Score(f"{totpop_col}_max_deviation", partial(_max_deviation, totpop_col=totpop_col, pct=pct))
+    return Score(
+        f"{totpop_col}_max_deviation",
+        partial(_max_deviation, totpop_col=totpop_col, pct=pct),
+    )
```

### Comparing `gerrytools-1.0.2/gerrytools/scoring/splits.py` & `gerrytools-1.1.0/gerrytools/scoring/splits.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from typing import List, Union
 
 from gerrychain import Partition
 from gerrychain.updaters import CountySplit
-from typing import List, Union
 
 from ..geometry import dataframe
 
 
 def _grouper(P: Partition, unit: str, popcol: str = None) -> list:
     """
     A nice little subroutine for doing the necessary pandas operations that we
@@ -26,31 +26,36 @@
         child geometries of a single parent geometry; for example, the identifier
         could be a VTD identifier, and the `DataFrame` the data attached to blocks
         belonging to that VTD.
     """
     # Not to be confused with a probability distribution function. That's not what
     # this is.
     pdf = dataframe(
-        P, index="id", assignment="DISTRICT",
-        columns=[unit] + ([popcol] if popcol else [])
+        P,
+        index="id",
+        assignment="DISTRICT",
+        columns=[unit] + ([popcol] if popcol else []),
     )
 
     # Group by unit, then get the units split.
     groups = list(pdf.groupby(by=unit))
 
-    for _, group in groups:
-        group = group.drop(group[group[popcol] < 1].index) if popcol else group
-
-    # Return the groups.
-    return groups
+    return [
+        (identifier, group[group[popcol] > 0].copy()) if popcol else (identifier, group)
+        for identifier, group in groups
+    ]
 
 
 def _splits(
-    P: Partition, unit: str, names: bool = False, popcol: str = None, how: str = "pandas",
-    unit_info_updater_col: str = None
+    P: Partition,
+    unit: str,
+    names: bool = False,
+    popcol: str = None,
+    how: str = "pandas",
+    unit_info_updater_col: str = None,
 ) -> Union[int, List[str]]:
     """
     Determines the number of units split by the districting plan.
 
     Bear in mind that this calculates the number of *unit splits*, not the number
     of *units split*: for example, if a district divides a county into three
     pieces, the former reports two splits (as a unit divided into three pieces is
@@ -74,24 +79,25 @@
             and not specified defaults to the name of unit.
 
     Returns:
         The number of splits or the list of things split.
     """
     # Validate the `how` parameter.
     if how not in {"pandas", "gerrychain"}:
-        print(f"\"{how}\" is not a valid parameter to `how`. Defaulting to pandas.")
+        print(f'"{how}" is not a valid parameter to `how`. Defaulting to pandas.')
         how = "pandas"
 
     # If we're calculating splits from a dataframe, create the dataframe and do
     # the required operations.
     if how == "pandas":
         # Get the groups for each unit, then do the appropriate calculations.
         groups = _grouper(P, unit, popcol)
         geometrysplits = [
-            identifier for identifier, group in groups
+            identifier
+            for identifier, group in groups
             if len(group["DISTRICT"].unique()) > 1
         ]
 
     # Otherwise, do things the normal way!
     if how == "gerrychain":
         if unit_info_updater_col is None:
             unit_info_updater_col = unit
@@ -101,16 +107,20 @@
             if split.split != CountySplit.NOT_SPLIT
         ]
 
     return geometrysplits if names else len(geometrysplits)
 
 
 def _pieces(
-    P: Partition, unit: str, names: bool = False, popcol: str = None, how: str = "pandas",
-    unit_info_updater_col: str = None
+    P: Partition,
+    unit: str,
+    names: bool = False,
+    popcol: str = None,
+    how: str = "pandas",
+    unit_info_updater_col: str = None,
 ) -> Union[int, List[str]]:
     """
     Determines the number of "unit pieces" produced by the plan. For example,
     consider a state with 100 counties. Suppose that one county is split twice,
     and another once. Then, there are 3 + 2 = 5 "pieces," disregarding the
     counties kept whole.
 
@@ -137,30 +147,32 @@
             of unit.
 
     Returns:
         The number of pieces or the list of things split.
     """
     # Validate the `how` parameter.
     if how not in {"pandas", "gerrychain"}:
-        print(f"\"{how}\" is not a valid parameter to `how`. Defaulting to pandas.")
+        print(f'"{how}" is not a valid parameter to `how`. Defaulting to pandas.')
         how = "pandas"
 
     # If they just want the list of names, return the splits.
     if names:
         return _splits(P, unit, names=names, popcol=popcol, how=how)
 
     # Otherwise, do some similar stuff to the splitting except that we're getting
     # the number of pieces instead of whether the unit's split.
     if how == "pandas":
         groups = _grouper(P, unit, popcol=popcol)
-        geometrypieces = sum([
-            len(group["DISTRICT"].unique())
-            for _, group in groups
-            if len(group["DISTRICT"].unique()) > 1
-        ])
+        geometrypieces = sum(
+            [
+                len(group["DISTRICT"].unique())
+                for _, group in groups
+                if len(group["DISTRICT"].unique()) > 1
+            ]
+        )
 
     if how == "gerrychain":
         if unit_info_updater_col is None:
             unit_info_updater_col = unit
         geometrypieces = sum(
             len(split.contains)
             for split in P[unit_info_updater_col].values()
```

### Comparing `gerrytools-1.0.2/gerrytools/utilities/JSON.py` & `gerrytools-1.1.0/gerrytools/utilities/JSON.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-
 import json
-from pydantic import BaseModel, validator
 from typing import Any
 
+from pydantic import BaseModel, validator
+
 
 class JSONtoObject(BaseModel):
     """
     Plan specification models. To better work with multiple plans at once, this
     plan specification allows users to specify information which should remain
     consistent across all operations; for example, the `column` field should be
     the name of the column in which the corresponding plan's assignment is
@@ -77,18 +77,20 @@
         # plans individually and return the list.
         if isinstance(data, list):
             return [
                 JSONtoObject(
                     column=p["column"],
                     locator=p["locator"],
                     title=p["title"] if p.get("title", False) else None,
-                    type=p["type"] if p.get("type", False) else None
+                    type=p["type"] if p.get("type", False) else None,
                 )
                 for p in data
             ]
 
         # Otherwise, return a singleton list with a single plan.
-        return [JSONtoObject(
-            column=data["column"],
-            locator=data["locator"],
-            title=data["title"] if data.get("title", False) else None
-        )]
+        return [
+            JSONtoObject(
+                column=data["column"],
+                locator=data["locator"],
+                title=data["title"] if data.get("title", False) else None,
+            )
+        ]
```

### Comparing `gerrytools-1.0.2/gerrytools/utilities/rename.py` & `gerrytools-1.1.0/gerrytools/utilities/rename.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import os
 from os import path
 
 
 def rename(old, new):
     """
     Renames all files in the path specified by `old` to `new`; intended for use
@@ -23,15 +22,15 @@
     Args:
         old (str): _Directory_ where files to be renamed are located.
         new (str): New name to be applied to the directory and all files in it.
     """
     for file in os.listdir(old):
         # Check whether the file has an extension.
         if "." in file:
-            extension = file[file.index("."):]
+            extension = file[file.index(".") :]
             os.rename(path.join(old, file), path.join(old, new + extension))
 
     # Rename the root directory.
     split = old.split("/")
     _base = split[:-1] if split[-1] != "" else split[:-2]
     base = "/".join(_base)
     new_root = path.join(base, new)
```

### Comparing `gerrytools-1.0.2/gerrytools.egg-info/PKG-INFO` & `gerrytools-1.1.0/gerrytools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gerrytools
-Version: 1.0.2
+Version: 1.1.0
 Summary: Tools for processing and visualizing districting plans.
 Home-page: https://github.com/mggg/gerrytools
 Author: MGGG Redistricting Lab
 Author-email: engineering@mggg.org
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
```

### Comparing `gerrytools-1.0.2/gerrytools.egg-info/SOURCES.txt` & `gerrytools-1.1.0/gerrytools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 gerrytools/__init__.py
 gerrytools.egg-info/PKG-INFO
 gerrytools.egg-info/SOURCES.txt
 gerrytools.egg-info/dependency_links.txt
 gerrytools.egg-info/requires.txt
 gerrytools.egg-info/top_level.txt
@@ -14,14 +15,15 @@
 gerrytools/data/acs.py
 gerrytools/data/census.py
 gerrytools/data/estimatecvap.py
 gerrytools/data/fetch.py
 gerrytools/data/geometries.py
 gerrytools/data/remap.py
 gerrytools/geometry/__init__.py
+gerrytools/geometry/compactness.py
 gerrytools/geometry/dataframe.py
 gerrytools/geometry/dissolve.py
 gerrytools/geometry/dualgraph.py
 gerrytools/geometry/optimize.py
 gerrytools/geometry/unitmap.py
 gerrytools/geometry/updater.py
 gerrytools/plotting/__init__.py
@@ -42,14 +44,17 @@
 gerrytools/plotting/utils.py
 gerrytools/plotting/violin.py
 gerrytools/scoring/__init__.py
 gerrytools/scoring/contiguity.py
 gerrytools/scoring/demographics.py
 gerrytools/scoring/partisan.py
 gerrytools/scoring/population.py
-gerrytools/scoring/reock.py
 gerrytools/scoring/scores.py
 gerrytools/scoring/splits.py
 gerrytools/scoring/types.py
 gerrytools/utilities/JSON.py
 gerrytools/utilities/__init__.py
-gerrytools/utilities/rename.py
+gerrytools/utilities/rename.py
+tests/test_data.py
+tests/test_geometry.py
+tests/test_plotting.py
+tests/test_scoring.py
```

### Comparing `gerrytools-1.0.2/setup.py` & `gerrytools-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-
-from setuptools import setup, find_packages
 from pathlib import Path
 
+from setuptools import find_packages, setup
+
 requirements = [
-    "pandas", "scipy", "networkx", "geopandas", "shapely", "matplotlib",
-    "gerrychain", "sortedcontainers", "gurobipy", "jsonlines", "opencv-python-headless",
-    "imageio", "us", "pydantic", "censusdata", "seaborn", "maup"
+    "pandas",
+    "scipy",
+    "networkx",
+    "geopandas",
+    "shapely",
+    "matplotlib",
+    "gerrychain",
+    "sortedcontainers",
+    "jsonlines",
+    "opencv-python-headless",
+    "imageio",
+    "us",
+    "pydantic",
+    "censusdata",
+    "seaborn",
+    "maup",
 ]
 
 # Set the version --- ensure that the latest tag matches this value.
-VERSION = "1.0.2"
+VERSION = "1.1.0"
 
 # Description.
 here = Path(__file__).parent
 DESCRIPTION = (here / "README.md").read_text()
 
 setup(
     name="gerrytools",
@@ -23,17 +36,9 @@
     description="Tools for processing and visualizing districting plans.",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mggg/gerrytools",
     packages=find_packages(exclude=["tests", "tutorials"]),
     install_requires=requirements,
     include_package_data=True,
-    extras_require={
-        "dev": [
-            "pdoc3",
-            "flake8",
-            "pytest",
-            "autopep8",
-            "pytest-cov"
-        ]
-    }
+    extras_require={"dev": ["pdoc3", "flake8", "pytest", "autopep8", "pytest-cov", "black", "isort"]},
 )
```

