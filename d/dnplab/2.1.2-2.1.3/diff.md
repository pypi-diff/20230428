# Comparing `tmp/dnplab-2.1.2.tar.gz` & `tmp/dnplab-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-ojv70wkx\dnplab-2.1.2.tar", last modified: Fri Apr 14 17:52:39 2023, max compression
+gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-i404ggjg\dnplab-2.1.3.tar", last modified: Fri Apr 28 19:23:33 2023, max compression
```

## Comparing `dnplab-2.1.2.tar` & `dnplab-2.1.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.538852 dnplab-2.1.2/
--rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2374 2023-04-14 17:52:39.537854 dnplab-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.175392 dnplab-2.1.2/dnplab/
--rw-rw-rw-   0        0        0      573 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.197361 dnplab-2.1.2/dnplab/analysis/
--rw-rw-rw-   0        0        0      161 2023-03-16 14:57:31.000000 dnplab-2.1.2/dnplab/analysis/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/analysis/enhancement_profiles.py
--rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/analysis/hydration.py
--rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/analysis/relaxation_fit.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.204342 dnplab-2.1.2/dnplab/constants/
--rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/constants/__init__.py
--rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/constants.py
--rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/mrProperties.py
--rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/constants/radicalProperties.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.255776 dnplab-2.1.2/dnplab/core/
--rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/core/__init__.py
--rw-rw-rw-   0        0        0    36820 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/base.py
--rw-rw-rw-   0        0        0     6793 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/coord.py
--rw-rw-rw-   0        0        0     7420 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/core/data.py
--rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/core/ufunc.py
--rw-rw-rw-   0        0        0     1428 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/core/util.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.266744 dnplab-2.1.2/dnplab/fitting/
--rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/fitting/__init__.py
--rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/fitting/general.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.420259 dnplab-2.1.2/dnplab/io/
--rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/__init__.py
--rw-rw-rw-   0        0        0    15036 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/bes3t.py
--rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/cnsi.py
--rw-rw-rw-   0        0        0     5932 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/delta.py
--rw-rw-rw-   0        0        0     5740 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/h5.py
--rw-rw-rw-   0        0        0     6862 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/load.py
--rw-rw-rw-   0        0        0     3730 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/load_csv.py
--rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/io/power.py
--rw-rw-rw-   0        0        0    10252 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/prospa.py
--rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/random.py
--rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/save.py
--rw-rw-rw-   0        0        0     4969 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/specman.py
--rw-rw-rw-   0        0        0     2799 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/io/tnmr.py
--rw-rw-rw-   0        0        0    20170 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/topspin.py
--rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/vna.py
--rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/vnmrj.py
--rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/io/winepr.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.432230 dnplab-2.1.2/dnplab/math/
--rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.2/dnplab/math/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/math/lineshape.py
--rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/math/relaxation.py
--rw-rw-rw-   0        0        0     3985 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/math/window.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.448214 dnplab-2.1.2/dnplab/plotting/
--rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/plotting/__init__.py
--rw-rw-rw-   0        0        0     8149 2023-04-14 17:51:32.000000 dnplab-2.1.2/dnplab/plotting/general.py
--rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/plotting/image.py
--rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/plotting/stack_plot.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.505829 dnplab-2.1.2/dnplab/processing/
--rw-rw-rw-   0        0        0      270 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/__init__.py
--rw-rw-rw-   0        0        0     7427 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/processing/align.py
--rw-rw-rw-   0        0        0     2828 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/apodization.py
--rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/processing/conversion.py
--rw-rw-rw-   0        0        0     5159 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/fft.py
--rw-rw-rw-   0        0        0     8703 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/helpers.py
--rw-rw-rw-   0        0        0     3607 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/integration.py
--rw-rw-rw-   0        0        0     2080 2023-03-16 14:57:24.000000 dnplab-2.1.2/dnplab/processing/offset.py
--rw-rw-rw-   0        0        0     9313 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/processing/phase.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.509846 dnplab-2.1.2/dnplab/reporting/
--rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.2/dnplab/reporting/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-14 17:51:32.000000 dnplab-2.1.2/dnplab/version.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.524788 dnplab-2.1.2/dnplab/widgets/
--rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/widgets/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.2/dnplab/widgets/align_widget.py
--rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.2/dnplab/widgets/phase_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.186391 dnplab-2.1.2/dnplab.egg-info/
--rw-rw-rw-   0        0        0     2374 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-14 17:52:39.000000 dnplab-2.1.2/dnplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 17:52:39.538852 dnplab-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1358 2023-03-24 14:33:33.000000 dnplab-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 17:52:39.536886 dnplab-2.1.2/unittests/
--rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.2/unittests/__init__.py
--rw-rw-rw-   0        0        0     2223 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_data_class.py
--rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_dnp_nmr.py
--rw-rw-rw-   0        0        0     3606 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_dnp_tools.py
--rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_general_fit.py
--rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_hydration.py
--rw-rw-rw-   0        0        0    10338 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_io.py
--rw-rw-rw-   0        0        0     1884 2022-08-30 17:05:30.000000 dnplab-2.1.2/unittests/test_load.py
--rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.2/unittests/test_nddata_core.py
--rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/test_save.py
--rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.2/unittests/testing.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.898574 dnplab-2.1.3/
+-rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2374 2023-04-28 19:23:33.898574 dnplab-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2022-08-30 17:05:30.000000 dnplab-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.800255 dnplab-2.1.3/dnplab/
+-rw-rw-rw-   0        0        0      582 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.824191 dnplab-2.1.3/dnplab/analysis/
+-rw-rw-rw-   0        0        0      170 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/analysis/__init__.py
+-rw-rw-rw-   0        0        0    19663 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/analysis/hydration.py
+-rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/analysis/relaxation_fit.py
+-rw-rw-rw-   0        0        0     3739 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/analysis/simulate_enhancement_profiles.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.827183 dnplab-2.1.3/dnplab/constants/
+-rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.3/dnplab/constants/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/constants/constants.py
+-rw-rw-rw-   0        0        0    13525 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/constants/mrProperties.py
+-rw-rw-rw-   0        0        0     5182 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/constants/radicalProperties.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.831172 dnplab-2.1.3/dnplab/core/
+-rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.3/dnplab/core/__init__.py
+-rw-rw-rw-   0        0        0    36820 2023-04-28 18:05:45.000000 dnplab-2.1.3/dnplab/core/base.py
+-rw-rw-rw-   0        0        0     6793 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/core/coord.py
+-rw-rw-rw-   0        0        0     7420 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/core/data.py
+-rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/core/ufunc.py
+-rw-rw-rw-   0        0        0     3106 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/core/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.832169 dnplab-2.1.3/dnplab/fitting/
+-rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.3/dnplab/fitting/__init__.py
+-rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/fitting/general.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.853694 dnplab-2.1.3/dnplab/io/
+-rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/__init__.py
+-rw-rw-rw-   0        0        0    15036 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/bes3t.py
+-rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/io/cnsi.py
+-rw-rw-rw-   0        0        0     5932 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/io/delta.py
+-rw-rw-rw-   0        0        0     5740 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/h5.py
+-rw-rw-rw-   0        0        0     6862 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/io/load.py
+-rw-rw-rw-   0        0        0     3269 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/io/load_csv.py
+-rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/io/power.py
+-rw-rw-rw-   0        0        0    10252 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/io/prospa.py
+-rw-rw-rw-   0        0        0      814 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/io/random.py
+-rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/save.py
+-rw-rw-rw-   0        0        0     5027 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/io/specman.py
+-rw-rw-rw-   0        0        0     2799 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/io/tnmr.py
+-rw-rw-rw-   0        0        0    20255 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/io/topspin.py
+-rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/vna.py
+-rw-rw-rw-   0        0        0     7086 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/vnmrj.py
+-rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/io/winepr.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.855689 dnplab-2.1.3/dnplab/math/
+-rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.3/dnplab/math/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/math/lineshape.py
+-rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/math/relaxation.py
+-rw-rw-rw-   0        0        0     3985 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/math/window.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.860676 dnplab-2.1.3/dnplab/plotting/
+-rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.3/dnplab/plotting/__init__.py
+-rw-rw-rw-   0        0        0    11014 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/plotting/general.py
+-rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/plotting/image.py
+-rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/plotting/stack_plot.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.872643 dnplab-2.1.3/dnplab/processing/
+-rw-rw-rw-   0        0        0      270 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/processing/__init__.py
+-rw-rw-rw-   0        0        0     7427 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/processing/align.py
+-rw-rw-rw-   0        0        0     2828 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/processing/apodization.py
+-rw-rw-rw-   0        0        0     4073 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/processing/conversion.py
+-rw-rw-rw-   0        0        0     5159 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/processing/fft.py
+-rw-rw-rw-   0        0        0     9442 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/processing/helpers.py
+-rw-rw-rw-   0        0        0     3607 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/processing/integration.py
+-rw-rw-rw-   0        0        0     2080 2023-03-16 14:57:24.000000 dnplab-2.1.3/dnplab/processing/offset.py
+-rw-rw-rw-   0        0        0     9313 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/processing/phase.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.873640 dnplab-2.1.3/dnplab/reporting/
+-rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.3/dnplab/reporting/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-28 19:23:06.000000 dnplab-2.1.3/dnplab/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.884613 dnplab-2.1.3/dnplab/widgets/
+-rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.3/dnplab/widgets/align_widget.py
+-rw-rw-rw-   0        0        0     3567 2023-03-31 19:37:00.000000 dnplab-2.1.3/dnplab/widgets/phase_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.816214 dnplab-2.1.3/dnplab.egg-info/
+-rw-rw-rw-   0        0        0     2374 2023-04-28 19:23:33.000000 dnplab-2.1.3/dnplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1862 2023-04-28 19:23:33.000000 dnplab-2.1.3/dnplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 19:23:33.000000 dnplab-2.1.3/dnplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-28 19:23:33.000000 dnplab-2.1.3/dnplab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-28 19:23:33.000000 dnplab-2.1.3/dnplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 19:23:33.898574 dnplab-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1358 2023-03-24 14:33:33.000000 dnplab-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:23:33.896580 dnplab-2.1.3/unittests/
+-rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.3/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2223 2023-03-31 19:37:00.000000 dnplab-2.1.3/unittests/test_data_class.py
+-rw-rw-rw-   0        0        0     1613 2023-03-31 19:37:00.000000 dnplab-2.1.3/unittests/test_dnp_nmr.py
+-rw-rw-rw-   0        0        0     3676 2023-04-28 19:23:06.000000 dnplab-2.1.3/unittests/test_dnp_tools.py
+-rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.3/unittests/test_general_fit.py
+-rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.3/unittests/test_hydration.py
+-rw-rw-rw-   0        0        0    10320 2023-04-28 19:23:06.000000 dnplab-2.1.3/unittests/test_io.py
+-rw-rw-rw-   0        0        0     1884 2022-08-30 17:05:30.000000 dnplab-2.1.3/unittests/test_load.py
+-rw-rw-rw-   0        0        0     9020 2023-03-31 19:37:00.000000 dnplab-2.1.3/unittests/test_nddata_core.py
+-rw-rw-rw-   0        0        0      914 2023-03-24 14:33:33.000000 dnplab-2.1.3/unittests/test_save.py
+-rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.3/unittests/testing.py
```

### Comparing `dnplab-2.1.2/LICENSE.txt` & `dnplab-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/PKG-INFO` & `dnplab-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.2
+Version: 2.1.3
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.2/README.md` & `dnplab-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/__init__.py` & `dnplab-2.1.3/dnplab/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 
 from .io import *
 from .io.save import save
 from .io.load import load
 
 from .analysis.relaxation_fit import *
 from .analysis.hydration import hydration
-from .analysis.enhancement_profiles import *
+from .analysis.simulate_enhancement_profiles import *
 
 from .processing import *
 from .widgets import *
 from .plotting import *
 from .reporting import *
 from .version import __version__
```

### Comparing `dnplab-2.1.2/dnplab/analysis/enhancement_profiles.py` & `dnplab-2.1.3/dnplab/analysis/simulate_enhancement_profiles.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/analysis/hydration.py` & `dnplab-2.1.3/dnplab/analysis/hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/analysis/relaxation_fit.py` & `dnplab-2.1.3/dnplab/analysis/relaxation_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/constants/mrProperties.py` & `dnplab-2.1.3/dnplab/constants/mrProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/constants/radicalProperties.py` & `dnplab-2.1.3/dnplab/constants/radicalProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/core/base.py` & `dnplab-2.1.3/dnplab/core/base.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/core/coord.py` & `dnplab-2.1.3/dnplab/core/coord.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/core/data.py` & `dnplab-2.1.3/dnplab/core/data.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/core/ufunc.py` & `dnplab-2.1.3/dnplab/core/ufunc.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/fitting/general.py` & `dnplab-2.1.3/dnplab/fitting/general.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/bes3t.py` & `dnplab-2.1.3/dnplab/io/bes3t.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/cnsi.py` & `dnplab-2.1.3/dnplab/io/cnsi.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/delta.py` & `dnplab-2.1.3/dnplab/io/delta.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/h5.py` & `dnplab-2.1.3/dnplab/io/h5.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/load.py` & `dnplab-2.1.3/dnplab/io/load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/load_csv.py` & `dnplab-2.1.3/dnplab/io/load_csv.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,67 +11,53 @@
 # define logger
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 handler = logging.StreamHandler(stream=sys.stdout)
 handler.setLevel(logging.INFO)
 logger.addHandler(handler)
 
-# config for load_csv file, can be adjusted to add more options (dialect?)
-# could also be checked for userconfig, bt this is not implemented right now
-parent_dir = pathlib.Path(pathlib.Path(__file__).absolute().parents[1])
-p0 = parent_dir.joinpath("config/io_config.conf")
-config_io = configparser.ConfigParser()
-config_io.read(str(p0))
-
 
 def load_csv(
     filename,
     tcol=0,
     real=1,
     imag=2,
     skiprows=0,
     maxrows=-1,
-    convert_time=lambda x: float(x.replace(",", ".")) / 1e6,
+    convert_time=lambda x: float(x.replace(",", ".")),
     convert_data=lambda x: float(x.replace(",", ".")),
     **kwargs
 ):
-    """
-    load_csv files function
+    """function that loads load_csv files
 
     Args:
-        filename: str/path like
-        tcol: column index for time data (default=0), None = not applicable, will count from 0 to npoints and then apply covert_time!
-        real: column index for real part (default=1), None = not applicable, will be set to zero
-        imag: column index for imaginary part (default=2), None = not applicable, will be set to zero
-        skiprows: number of rows to skip at beginning (default=0)
-        maxrows: if this is larger than zeros read at most maxrows rows
-        convert_time: callable that converts the time strings to a number (default: assumes us and converts into s)
-        convert_data: callable that converts data to a number (default: replaces , with .)
+        filename (str): String or path like file that is read
+        tcol (int): column index for time data (default=0), None = not applicable, will count from 0 to npoints and then apply covert_time!
+        real (int): column index for real part (default=1), None = not applicable, will be set to zero
+        imag (int): column index for imaginary part (default=2), None = not applicable, will be set to zero
+        skiprows (int): number of rows to skip at beginning (default=0)
+        maxrows (int): if this is larger than zero, read at most maxrows rows. (default: -1)
+        convert_time (callable): callable that converts the time strings to a number (default: replaces , with .)
+        convert_data (callable): callable that converts data to a number (default: replaces , with .)
 
-        delimiter: optional, sets the delimiter in the csv file (default ; ), can be set in ../config/io_config.conf
-        dims: optional, sets name for dimension (default: t2)
+        delimiter (str): optional, sets the delimiter in the csv file (default ; )
+        dims (str,list): optional, sets name for dimension (default: ["t2"])
         **kwargs are forwarded to csv.reader object
 
 
     Returns:
-        DNPData: data object with values,coords and dim
+       data (dnpData): Data object with values,coords and dim
 
 
     example:
 
         data=load_csv('csv_arrLNA_data.csv',imag=2,skiprows=1)
     """
 
-    # standards from config (?)
-    delimiter = config_io.get(
-        "load_csv", "delimiter"
-    )  # or config_io['load_csv']['delimiter']
-
-    if "delimiter" in kwargs.keys():
-        delimiter = kwargs.pop("delimiter")
+    delimiter = kwargs.pop("delimiter", ";")
 
     dims = kwargs.pop("dims", ["t2"])
 
     def _checknone(x, row, ind=None):
         if x is None and (ind is not None):
             return str(ind)
         if x is None:
```

### Comparing `dnplab-2.1.2/dnplab/io/power.py` & `dnplab-2.1.3/dnplab/io/power.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/prospa.py` & `dnplab-2.1.3/dnplab/io/prospa.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/random.py` & `dnplab-2.1.3/dnplab/io/random.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/save.py` & `dnplab-2.1.3/dnplab/io/save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/specman.py` & `dnplab-2.1.3/dnplab/io/specman.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
         file_name_d01 = path
     else:
         raise TypeError("Incorrect file type, must be .d01 or .exp")
 
     attrs = load_specman_exp(file_name_exp)
     data, dims, coords, attrs = load_specman_d01(file_name_d01, attrs)
 
+    # Add import path
+    attrs["import_path"] = path
+
     # Assign data/spectrum type
     attrs["experiment_type"] = "epr_spectrum"
 
     specman_data = _dnp.DNPData(data, dims, coords, attrs)
 
     return specman_data
 
@@ -115,15 +118,15 @@
 
     data = float_read[attrs["dataStartIndex"] : -1]
 
     if attrs["dims"] == 1:
         data = _np.reshape(data, (attrs["numberOfVariables"], uint_read[3]))
 
     elif attrs["dims"] == 2:
-        data = _np.reshape(data, (uint_read[2], uint_read[3], uint_read[4]))
+        data = _np.reshape(data, (uint_read[2], uint_read[4], uint_read[3]))
 
     elif attrs["dims"] == 3:
         data = _np.reshape(
             data, (uint_read[2], uint_read[3], uint_read[4], uint_read[5])
         )
 
     elif attrs["dims"] == 4:
```

### Comparing `dnplab-2.1.2/dnplab/io/tnmr.py` & `dnplab-2.1.3/dnplab/io/tnmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/topspin.py` & `dnplab-2.1.3/dnplab/io/topspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,17 @@
 
     # Handle group delay
     values = values[..., slice(group_delay, int(acqus_params["TD"] / 2))]
 
     # create data object
     topspin_data = DNPData(values, dims, coords, attrs=acqus_params)
 
+    # Add import path to attributes
+    topspin_data.attrs["import_path"] = path
+
     # Add NMR Frequency to attrs
     topspin_data.attrs["nmr_frequency"] = acqus_params["SFO1"] * 1e6
 
     # Assign data/spectrum type
     topspin_data.attrs["experiment_type"] = "nmr_spectrum"
 
     # reorder so that 't2' is first
```

### Comparing `dnplab-2.1.2/dnplab/io/vna.py` & `dnplab-2.1.3/dnplab/io/vna.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/vnmrj.py` & `dnplab-2.1.3/dnplab/io/vnmrj.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/io/winepr.py` & `dnplab-2.1.3/dnplab/io/winepr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/math/lineshape.py` & `dnplab-2.1.3/dnplab/math/lineshape.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/math/relaxation.py` & `dnplab-2.1.3/dnplab/math/relaxation.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/math/window.py` & `dnplab-2.1.3/dnplab/math/window.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/plotting/image.py` & `dnplab-2.1.3/dnplab/plotting/image.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/plotting/stack_plot.py` & `dnplab-2.1.3/dnplab/plotting/stack_plot.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/align.py` & `dnplab-2.1.3/dnplab/processing/align.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/apodization.py` & `dnplab-2.1.3/dnplab/processing/apodization.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/conversion.py` & `dnplab-2.1.3/dnplab/processing/conversion.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/fft.py` & `dnplab-2.1.3/dnplab/processing/fft.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/helpers.py` & `dnplab-2.1.3/dnplab/processing/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,44 @@
     if return_complex_values == True:
         return enhancements
 
     elif return_complex_values == False:
         return enhancements.real
 
 
+def create_complex(data, real, imag):
+    """Create complex array from input
+
+    This function can be used to concatenate a two dimensions of a DNPData object into a complex array. The unused dims and coords will be removed from the input DNPData object.
+
+    Args:
+        data (DNPData): DNPData input object
+        real (array): Real data
+        imag (array): Imaginary data
+
+    Returns:
+        data (DNPData): New DNPData object
+    """
+
+    complexData = _np.vectorize(complex)(real, imag)
+
+    dims = data.dims
+    dims.pop(-1)
+
+    coords = data.coords
+    coords = list(coords)
+    coords.pop(-1)
+
+    attrs = data.attrs
+
+    out = dnp.DNPData(complexData, dims, coords, attrs)
+
+    return out
+
+
 def signal_to_noise(
     data: DNPData,
     signal_region: list = slice(0, None),
     noise_region: list = (None, None),
     dim: str = "f2",
     remove_background: list = None,
     **kwargs
```

### Comparing `dnplab-2.1.2/dnplab/processing/integration.py` & `dnplab-2.1.3/dnplab/processing/integration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/offset.py` & `dnplab-2.1.3/dnplab/processing/offset.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/processing/phase.py` & `dnplab-2.1.3/dnplab/processing/phase.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/widgets/align_widget.py` & `dnplab-2.1.3/dnplab/widgets/align_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab/widgets/phase_widget.py` & `dnplab-2.1.3/dnplab/widgets/phase_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/dnplab.egg-info/PKG-INFO` & `dnplab-2.1.3/dnplab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.2
+Version: 2.1.3
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.2/dnplab.egg-info/SOURCES.txt` & `dnplab-2.1.3/dnplab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 dnplab/version.py
 dnplab.egg-info/PKG-INFO
 dnplab.egg-info/SOURCES.txt
 dnplab.egg-info/dependency_links.txt
 dnplab.egg-info/requires.txt
 dnplab.egg-info/top_level.txt
 dnplab/analysis/__init__.py
-dnplab/analysis/enhancement_profiles.py
 dnplab/analysis/hydration.py
 dnplab/analysis/relaxation_fit.py
+dnplab/analysis/simulate_enhancement_profiles.py
 dnplab/constants/__init__.py
 dnplab/constants/constants.py
 dnplab/constants/mrProperties.py
 dnplab/constants/radicalProperties.py
 dnplab/core/__init__.py
 dnplab/core/base.py
 dnplab/core/coord.py
```

### Comparing `dnplab-2.1.2/setup.py` & `dnplab-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_data_class.py` & `dnplab-2.1.3/unittests/test_data_class.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_dnp_nmr.py` & `dnplab-2.1.3/unittests/test_dnp_nmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_dnp_tools.py` & `dnplab-2.1.3/unittests/test_dnp_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self.data = dnp.io.load_csv.load_csv(
             p.joinpath("csv_example.csv"),
             skiprows=1,
             maxrows=1000,
             tcol=0,
             real=1,
             imag=3,
+            convert_time=lambda x: float(x.replace(",", ".")) / 1e6,
         )
         self.data.attrs["nmr_frequency"] = 14.86e6
 
     def test_000_funcionality_signal_to_noise(self):
         """
         check only whether the function raises no error with DNPData input, not whether rsults are useful
         alot of simple tests lumped together
```

### Comparing `dnplab-2.1.2/unittests/test_general_fit.py` & `dnplab-2.1.3/unittests/test_general_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_hydration.py` & `dnplab-2.1.3/unittests/test_hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_io.py` & `dnplab-2.1.3/unittests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             maxrows=115,
             tcol=0,
             real=1,
             imag=3,
         )
         self.assertEqual(data.dims[0], "t2")
         self.assertEqual(data.values[1], 5e3 + 1j * 25000)
-        self.assertEqual(data.coords[0][1], 20 / 1e6)
+        self.assertEqual(data.coords[0][1], 20)
         self.assertEqual(data.values.size, 115)
 
     def test_remove_data_csv_arrLNA_fid(self):
         import pathlib
 
         p = pathlib.Path(self.testdata)
         data = dnp.io.load_csv.load_csv(
@@ -225,15 +225,15 @@
             maxrows=115,
             tcol=None,
             real=1,
             imag=3,
         )
         self.assertEqual(data.dims[0], "t2")
         self.assertEqual(data.values[1], 5e3 + 1j * 25000)
-        self.assertEqual(data.coords[0][100], 100 / 1e6)
+        self.assertEqual(data.coords[0][100], 100)
         self.assertEqual(data.values.size, 115)
 
     def test_set_imag_to_zero(self):
         import pathlib
 
         p = pathlib.Path(self.testdata)
         data = dnp.io.load_csv.load_csv(
@@ -242,14 +242,14 @@
             maxrows=115,
             tcol=None,
             real=1,
             imag=None,
         )
         self.assertEqual(data.dims[0], "t2")
         self.assertEqual(data.values[1], 5e3)
-        self.assertEqual(data.coords[0][100], 100 / 1e6)
+        self.assertEqual(data.coords[0][100], 100)
         self.assertEqual(data.values.size, 115)
 
 
 if __name__ == "__main__":
     unittest.main()
     pass
```

### Comparing `dnplab-2.1.2/unittests/test_load.py` & `dnplab-2.1.3/unittests/test_load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_nddata_core.py` & `dnplab-2.1.3/unittests/test_nddata_core.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/test_save.py` & `dnplab-2.1.3/unittests/test_save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.2/unittests/testing.py` & `dnplab-2.1.3/unittests/testing.py`

 * *Files identical despite different names*

