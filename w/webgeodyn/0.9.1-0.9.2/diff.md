# Comparing `tmp/webgeodyn-0.9.1.tar.gz` & `tmp/webgeodyn-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webgeodyn-0.9.1.tar", last modified: Tue Oct 22 10:45:11 2019, max compression
+gzip compressed data, was "dist/webgeodyn-0.9.2.tar", last modified: Wed Oct 23 13:01:54 2019, max compression
```

## Comparing `webgeodyn-0.9.1.tar` & `webgeodyn-0.9.2.tar`

### file list

```diff
@@ -1,435 +1,435 @@
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       57 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/AUTHORS.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       80 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9054 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/PKG-INFO
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6860 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/README.rst
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/setup.cfg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1465 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/setup.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      125 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2019-10-22 10:33:13.000000 webgeodyn-0.9.1/webgeodyn/_version.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      113 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/constants.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/data/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11097 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/data/GHData.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13534 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/data/TSData.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5121 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/data/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12665 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/data/measuredata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1051 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/data/normPnm.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1119 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/example.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/example_data/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/example_data/CHAOS-6-x4/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   435456 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/example_data/CHAOS-6-x4/CHAOS-6-x4_spline-coefficients.dat
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/filters/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9157 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/filters/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1627 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/filters/spectral.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3399 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/filters/time.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/inout/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2009 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2633 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/archeomag.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3353 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/ced.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3625 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/ced746.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2568 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/chaos.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1326 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/coreflo-ll.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2384 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/covobs.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14789 2019-10-22 10:33:13.000000 webgeodyn-0.9.1/webgeodyn/inout/covobs_splines.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7747 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/default.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2175 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/enscore.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      868 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/lod.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2789 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/midpath.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1873 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/nath.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5434 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_asc.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2461 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_hdf5.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2946 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_hdf5_forecasts.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5704 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/s1fs.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5948 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/s1fs2.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5986 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/inout/zforecast.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/models/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1533 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/models/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32422 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/models/model.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3851 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/models/models.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/obsdata/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1411978 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/GR_OBS_RMM_MF_less_bias.V29
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1148590 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/GR_OBS_RMM_SV.V29
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1185 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/README_GR_OBS_V29
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3764 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/README_VOs_0112.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  2079466 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/VO_CHAMP_MF.0112
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1792310 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/VO_CHAMP_SV.0112
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1323466 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/VO_SWARM_MF.0112
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1140710 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/VO_SWARM_SV.0112
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      798 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6888 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/obsdata.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6383 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/obsdata/observatory.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/processing/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       41 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/README.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5802 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/matrices.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1455 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/plm.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2734 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/psd.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2164 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/radon.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1973 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/processing/spectra.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/server/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       48 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/server/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13710 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/server/datahandlers.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5023 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/server/server.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/tests/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/tests/Spline_benchmark/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1378659 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/tests/Spline_benchmark/real001_mf_int_coefs.dat
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   433612 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/tests/Spline_benchmark/real_001
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       45 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/tests/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3777 2019-10-22 10:43:50.000000 webgeodyn-0.9.1/webgeodyn/tests/test_covobs_splines.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/.jshintrc
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/controller/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7407 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/exportTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14273 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/globeTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      328 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/homePageController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8467 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/lodTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5185 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/mainController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    20688 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/obsTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13785 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/spectraTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    17068 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/spherharmTabController.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7984 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/controller/timeseriesTabController.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/css/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2823 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/css/css.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1111 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/css/flex.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2586 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/css/timeSlider.css
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/error_pages/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      694 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/error_pages/50x.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    72646 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/favicon.png
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/images/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   103978 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/50x.svg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2869 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/arrow.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   103870 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/core.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    42247 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/crosssection.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  2226329 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoAitoff.gif
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   310642 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoCross.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   125401 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoGnm.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   210550 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoLOD.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   250142 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoObs.jpeg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   708055 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoOrtho.gif
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   132199 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/demoSpectra.jpeg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      831 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/downarrow.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4518 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/export.svg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2361 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/home.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   186279 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/lod.svg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    21898 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/logo_CNES.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15506 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/logo_CNRS.jpg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11746 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/logo_ISTerre.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8306 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/logo_UGA.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    19893 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/logo_geodynamo.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   137412 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/observatories.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5027 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/spectra.svg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1018 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/images/spherharm.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12759 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/index.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1054 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/index.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/data/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102116 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/data/110m.json
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   747178 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/data/50m.json
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5285 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   196911 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   216965 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js.map
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3828 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/index.html
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    30507 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.all.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    23913 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    10894 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    16130 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/Whammy.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9534 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9322 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.worker.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7186 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/tar.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   124810 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/API.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1475 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/LICENSE
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2293 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/README.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11758 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3-scale-chromatic.v1.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   463920 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   218926 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1475 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/LICENSE
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    73962 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/README.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   127494 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    57184 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13451 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    29120 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js.map
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    16636 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    55277 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js.map
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    86659 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery-3.2.1.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2771 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery.mousewheel.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12660 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/AUTHORS.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1817 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/LICENSE.txt
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   293430 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/jquery.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      418 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      312 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      262 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      348 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      260 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_20_555555_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      342 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_40_0078a3_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      316 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      207 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3816 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_25_333333_500x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5815 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      278 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      328 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      276 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      275 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_inset-soft_25_000000_1x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      340 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_inset-soft_30_f58400_1x100.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6922 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_222222_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_228ef1_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_a83300_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6975 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ef8c08_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffd27a_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6299 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32588 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/index.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    36665 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   520714 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    31384 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   253668 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    18705 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15548 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    18010 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14284 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1847 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/package.json
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   474776 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/math.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       68 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/.versions
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1080 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/LICENSE
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5084 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    22656 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold2.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5332 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    24132 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic2.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5224 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    24092 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic2.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5148 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    23216 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular2.woff2
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      441 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/README.md
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8611 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19990 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6638 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7307 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3902 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2049 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    39786 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14874 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2043 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1181 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    90016 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    72090 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21171 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14860 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15872 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26082 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11711 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11837 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8436 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3260 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4783 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2891 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2953 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1857 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3922 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20754 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2539 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7956 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7775 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5764 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    34287 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   135475 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    24154 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    49050 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3004 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    19902 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1819 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7822 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5701 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3705 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21286 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18480 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26064 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    52737 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19700 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19739 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    70102 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    55790 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12408 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8401 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    54919 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    42589 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5280 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3649 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11825 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8471 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9382 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6000 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26836 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19670 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21453 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15865 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6771 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4644 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    41846 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    29968 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9674 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6678 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10079 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    28099 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6666 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11255 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2514 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15047 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1430 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5922 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15537 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    48546 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10737 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18027 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10117 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    30274 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7280 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12621 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2495 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1446 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20492 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14362 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18265 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5553 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8442 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2084 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7700 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5625 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8828 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    47051 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5994 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17044 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16394 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11488 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3646 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    28953 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2429 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11312 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15168 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    33474 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10430 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13716 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2676 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14118 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1652 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6310 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20791 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8010 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13228 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9823 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    23040 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18944 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1211 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    30262 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)      600 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11919 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1715 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    32820 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1027 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11699 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22817 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16372 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    45391 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    34982 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    32107 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13248 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2221 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15720 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1319 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6080 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    42849 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.js
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16571 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15625 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5877 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2364 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/lato.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      741 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      506 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.json
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   751187 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.css
--rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   736595 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   548097 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.css
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   278440 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   165742 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.eot
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    93888 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.otf
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   444379 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.svg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   165548 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.ttf
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    98024 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    77160 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff2
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    28123 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/flags.png
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1429 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/LICENSE.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7162 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/README.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    52014 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    20758 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    10653 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/parameters.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2264 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/pointinfo.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3873 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/videoexport.html
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/canvg/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102833 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/canvg/canvg.min.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2547 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/canvg/download.min.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    37914 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-3d.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102729 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-3d.js.map
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32176 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-more.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    74153 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-more.js.map
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   207133 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   507418 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts.js.map
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8923 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/export-data.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9751 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/exporting.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9620 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/heatmap.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5851 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/offline-exporting.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/model/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4286 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/genericData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2045 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/globeData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1321 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/lodData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6721 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/measureUnits.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3116 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/observatoryData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1501 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/spectraData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1697 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/spherHarmData.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2339 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/model/timeSerieData.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/ui/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2347 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/alertUser.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3160 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/dataDropdown.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4051 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/dropdown.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    31495 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/imshowPlot.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14772 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/measureDropdown.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5926 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/modelSelector.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11076 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/ui/timeSlider.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/utils/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      978 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/utils/banner.js
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5614 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/utils/utils.js
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn/www/view/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      879 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/export.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      810 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/globe.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4275 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/home.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3881 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/imshowparameters.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      271 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/lod.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1967 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/observatories.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      277 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/spectra.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1933 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/spherharm.html
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3231 2019-10-04 13:14:43.000000 webgeodyn-0.9.1/webgeodyn/www/view/timeseries.html
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9054 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    21469 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       29 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       10 2019-10-22 10:45:11.000000 webgeodyn-0.9.1/webgeodyn.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       57 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/AUTHORS.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       80 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9054 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6860 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/README.rst
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/setup.cfg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1465 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/setup.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      125 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2019-10-23 12:33:31.000000 webgeodyn-0.9.2/webgeodyn/_version.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      113 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/constants.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/data/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11097 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/data/GHData.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13534 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/data/TSData.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5121 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/data/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12665 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/data/measuredata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1051 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/data/normPnm.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1119 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/example.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/example_data/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/example_data/CHAOS-6-x4/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   435456 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/example_data/CHAOS-6-x4/CHAOS-6-x4_spline-coefficients.dat
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/filters/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9157 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/filters/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1627 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/filters/spectral.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3399 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/filters/time.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/inout/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2009 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2633 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/archeomag.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3353 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/ced.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3625 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/ced746.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2568 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/chaos.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1326 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/coreflo-ll.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2384 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/covobs.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14947 2019-10-23 12:33:31.000000 webgeodyn-0.9.2/webgeodyn/inout/covobs_splines.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7747 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/default.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2175 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/enscore.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      868 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/lod.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2789 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/midpath.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1873 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/nath.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5434 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_asc.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2461 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_hdf5.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2946 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_hdf5_forecasts.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5704 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/s1fs.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5948 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/s1fs2.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5986 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/inout/zforecast.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/models/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1533 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/models/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32422 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/models/model.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3851 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/models/models.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/obsdata/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1411978 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/GR_OBS_RMM_MF_less_bias.V29
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1148590 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/GR_OBS_RMM_SV.V29
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1185 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/README_GR_OBS_V29
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3764 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/README_VOs_0112.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  2079466 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/VO_CHAMP_MF.0112
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1792310 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/VO_CHAMP_SV.0112
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1323466 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/VO_SWARM_MF.0112
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1140710 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/VO_SWARM_SV.0112
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      798 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6888 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/obsdata.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6383 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/obsdata/observatory.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/processing/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       41 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/README.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5802 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/matrices.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1455 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/plm.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2734 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/psd.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2164 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/radon.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1973 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/processing/spectra.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/server/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       48 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/server/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13710 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/server/datahandlers.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5023 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/server/server.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/tests/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/tests/Spline_benchmark/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  1378659 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/tests/Spline_benchmark/real001_mf_int_coefs.dat
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   433612 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/tests/Spline_benchmark/real_001
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       45 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/tests/__init__.py
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3779 2019-10-23 12:33:31.000000 webgeodyn-0.9.2/webgeodyn/tests/test_covobs_splines.py
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/.jshintrc
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/controller/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7407 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/exportTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14273 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/globeTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      328 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/homePageController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8467 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/lodTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5185 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/mainController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    20688 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/obsTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13785 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/spectraTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    17068 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/spherharmTabController.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7984 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/controller/timeseriesTabController.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/css/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2823 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/css/css.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1111 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/css/flex.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2586 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/css/timeSlider.css
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/error_pages/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      694 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/error_pages/50x.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    72646 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/favicon.png
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/images/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   103978 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/50x.svg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2869 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/arrow.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   103870 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/core.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    42247 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/crosssection.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)  2226329 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoAitoff.gif
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   310642 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoCross.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   125401 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoGnm.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   210550 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoLOD.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   250142 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoObs.jpeg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   708055 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoOrtho.gif
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   132199 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/demoSpectra.jpeg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      831 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/downarrow.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4518 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/export.svg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2361 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/home.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   186279 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/lod.svg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    21898 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/logo_CNES.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15506 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/logo_CNRS.jpg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11746 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/logo_ISTerre.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8306 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/logo_UGA.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    19893 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/logo_geodynamo.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   137412 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/observatories.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5027 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/spectra.svg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1018 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/images/spherharm.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12759 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/index.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1054 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/index.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/data/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102116 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/data/110m.json
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   747178 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/data/50m.json
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5285 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   196911 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   216965 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js.map
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3828 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/index.html
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    30507 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.all.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    23913 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    10894 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    16130 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/Whammy.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9534 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9322 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.worker.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7186 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/tar.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   124810 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/API.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1475 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/LICENSE
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2293 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/README.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11758 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3-scale-chromatic.v1.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   463920 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   218926 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1475 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/LICENSE
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    73962 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/README.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   127494 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    57184 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    13451 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    29120 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js.map
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    16636 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    55277 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js.map
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    86659 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery-3.2.1.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2771 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery.mousewheel.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    12660 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/AUTHORS.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1817 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/LICENSE.txt
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   293430 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/jquery.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      418 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_diagonals-thick_18_b81900_40x40.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      312 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_diagonals-thick_20_666666_40x40.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      262 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_100_f6f6f6_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      348 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_100_fdf5ce_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      260 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_20_555555_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      342 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_40_0078a3_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      316 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_40_ffc73d_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      207 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3816 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_25_333333_500x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5815 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_35_f6a828_500x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      278 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      328 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      276 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      275 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_inset-soft_25_000000_1x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      340 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_inset-soft_30_f58400_1x100.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6922 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_228ef1_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_4b8e0b_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_a83300_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6975 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_cccccc_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ef8c08_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4549 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffd27a_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6299 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32588 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/index.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    36665 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   520714 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    31384 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   253668 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    18705 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15548 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    18010 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14284 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1847 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/package.json
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   474776 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/math.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       68 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/.versions
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1080 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/LICENSE
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5084 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    22656 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold2.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5332 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    24132 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic2.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5224 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    24092 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic2.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5148 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    23216 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular2.woff2
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      441 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/README.md
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8611 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19990 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6638 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7307 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3902 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2049 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    39786 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14874 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2043 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1181 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    90016 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    72090 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21171 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14860 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15872 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26082 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11711 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11837 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8436 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3260 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4783 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2891 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2953 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1857 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3922 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20754 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2539 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7956 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7775 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5764 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    34287 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   135475 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    24154 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    49050 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3004 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    19902 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1819 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7822 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5701 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3705 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21286 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18480 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26064 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    52737 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19700 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19739 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    70102 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    55790 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12408 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8401 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    54919 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    42589 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5280 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3649 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11825 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8471 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9382 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6000 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26836 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    19670 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    21453 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15865 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6771 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4644 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    41846 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    29968 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9674 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6678 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10079 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    28099 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6666 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11255 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2514 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15047 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1430 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5922 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15537 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    48546 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10737 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18027 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10117 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    30274 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7280 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12621 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2495 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1446 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20492 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14362 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18265 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5553 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8442 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2084 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     7700 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5625 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8828 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    47051 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5994 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17044 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16394 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11488 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3646 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    28953 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2429 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11312 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15168 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    33474 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10430 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13716 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2676 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    14118 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1652 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6310 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    20791 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8010 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13228 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9823 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    23040 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18944 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1211 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    30262 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)      600 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11919 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1715 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    32820 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1027 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11699 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22817 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16372 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    45391 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    34982 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    32107 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    13248 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2221 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15720 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1319 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6080 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    42849 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.js
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)    16571 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    15625 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5877 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2364 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/lato.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      741 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      506 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.json
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   751187 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.css
+-rwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)   736595 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   548097 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.css
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   278440 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   165742 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.eot
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    93888 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.otf
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   444379 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.svg
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   165548 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.ttf
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    98024 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    77160 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff2
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    28123 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/flags.png
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1429 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/LICENSE.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     7162 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/README.md
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    52014 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    20758 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    10653 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/parameters.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2264 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/pointinfo.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3873 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/videoexport.html
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/canvg/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102833 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/canvg/canvg.min.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2547 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/canvg/download.min.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    37914 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-3d.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   102729 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-3d.js.map
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    32176 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-more.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    74153 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-more.js.map
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   207133 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)   507418 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts.js.map
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     8923 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/export-data.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9751 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/exporting.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9620 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/heatmap.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5851 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/offline-exporting.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/model/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4286 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/genericData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2045 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/globeData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1321 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/lodData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     6721 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/measureUnits.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3116 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/observatoryData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1501 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/spectraData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1697 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/spherHarmData.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2339 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/model/timeSerieData.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/ui/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     2347 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/alertUser.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3160 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/dataDropdown.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4051 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/dropdown.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    31495 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/imshowPlot.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    14772 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/measureDropdown.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5926 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/modelSelector.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    11076 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/ui/timeSlider.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/utils/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      978 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/utils/banner.js
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     5614 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/utils/utils.js
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn/www/view/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      879 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/export.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      810 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/globe.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     4275 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/home.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3881 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/imshowparameters.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      271 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/lod.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1967 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/observatories.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)      277 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/spectra.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     1933 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/spherharm.html
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     3231 2019-10-04 13:14:43.000000 webgeodyn-0.9.2/webgeodyn/www/view/timeseries.html
+drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)     9054 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)    21469 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       29 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (999)       10 2019-10-23 13:01:54.000000 webgeodyn-0.9.2/webgeodyn.egg-info/top_level.txt
```

### Comparing `webgeodyn-0.9.1/PKG-INFO` & `webgeodyn-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webgeodyn
-Version: 0.9.1
+Version: 0.9.2
 Summary: A web-based plot tool to visualize Earth core flows
 Home-page: https://gricad-gitlab.univ-grenoble-alpes.fr/Geodynamo/webgeodyn
 Author: Nicolas Gillet, Loïc Huder, Yannick Martin, Franck Thollard
 Author-email: loic.huder@univ-grenoble-alpes.fr
 License: UNKNOWN
 Description: #########
         webgeodyn
```

### Comparing `webgeodyn-0.9.1/README.rst` & `webgeodyn-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/setup.py` & `webgeodyn-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/data/GHData.py` & `webgeodyn-0.9.2/webgeodyn/data/GHData.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/data/TSData.py` & `webgeodyn-0.9.2/webgeodyn/data/TSData.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/data/__init__.py` & `webgeodyn-0.9.2/webgeodyn/data/__init__.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/data/measuredata.py` & `webgeodyn-0.9.2/webgeodyn/data/measuredata.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/data/normPnm.py` & `webgeodyn-0.9.2/webgeodyn/data/normPnm.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/example.py` & `webgeodyn-0.9.2/webgeodyn/example.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/example_data/CHAOS-6-x4/CHAOS-6-x4_spline-coefficients.dat` & `webgeodyn-0.9.2/webgeodyn/example_data/CHAOS-6-x4/CHAOS-6-x4_spline-coefficients.dat`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/filters/__init__.py` & `webgeodyn-0.9.2/webgeodyn/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/filters/spectral.py` & `webgeodyn-0.9.2/webgeodyn/filters/spectral.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/filters/time.py` & `webgeodyn-0.9.2/webgeodyn/filters/time.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/__init__.py` & `webgeodyn-0.9.2/webgeodyn/inout/__init__.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/archeomag.py` & `webgeodyn-0.9.2/webgeodyn/inout/archeomag.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/ced.py` & `webgeodyn-0.9.2/webgeodyn/inout/ced.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/ced746.py` & `webgeodyn-0.9.2/webgeodyn/inout/ced746.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/chaos.py` & `webgeodyn-0.9.2/webgeodyn/inout/chaos.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/coreflo-ll.py` & `webgeodyn-0.9.2/webgeodyn/inout/coreflo-ll.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/covobs.py` & `webgeodyn-0.9.2/webgeodyn/inout/covobs.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/covobs_splines.py` & `webgeodyn-0.9.2/webgeodyn/inout/covobs_splines.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,30 +39,30 @@
     for i, t_i in enumerate(t_gnm):
         for j, t_j in enumerate(t_spl):
             A[i, j] = spl_eval_fc(date_to_eval=t_i, center_date=t_j, spl_order=spl_order, knot_spacing=knot_spacing)
 
     return A
 
 
-def build_gnm_from_file(file_name, dt=0.5, with_derivative=False):
+def build_gnm_from_file(file_name, dt=0.5, with_derivatives=False):
     """
     Builds gnm from the spline coeffs stored in a file. The timestep of the resulting dates can be changed.
 
     :param file_name: Name of the file where the spline coeffs are stored
     :type file_name: str
     :param dt: Timestep of the evaluation dates (default: 0.5)
     :type dt: float
-    :param with_derivative: If True, returns the reconstructed dgnm/dt evaluated from derivative of splines
-    :type with_derivative: bool
-    :return: evaluation dates and the reconstructed gnm at these dates
-    :rtype: np.array (dim: n_dates), np.array (dim: n_dates x n_gnm)
+    :param with_derivatives: If True, returns as well dgnm/dt and d2gnm/dt2 evaluated from derivative of splines
+    :type with_derivatives: bool
+    :return: evaluation dates and the gnm at these dates (and its first and second derivative if with_derivatives is True)
+    :rtype: np.array (dim: n_dates), np.array (dim: n_dates x n_gnm) (, np.array (dim: n_dates), np.array (dim: n_dates x n_gnm))
     """
     center_dates, spl_coeffs, spl_order, knot_sp = read_spline_coeffs_file(file_name)
     eval_dates = np.arange(center_dates[spl_order//2+1], center_dates[-spl_order//2-1], dt)
-    return build_gnm_from_spline_coeffs(eval_dates, center_dates, spl_coeffs, spl_order, with_derivative)
+    return build_gnm_from_spline_coeffs(eval_dates, center_dates, spl_coeffs, spl_order, with_derivatives)
 
 
 def eval_spline(date_to_eval, center_date, spl_order, knot_spacing):
     """ Evaluates a spline at date_to_eval.
     The spline is of order spl_order, spacing knot_spacing and centered on center_date."""
     normalised_X = (date_to_eval - center_date) / knot_spacing
     return scipy.signal.bspline(normalised_X, spl_order)
@@ -157,40 +157,40 @@
 
     if with_derivative:
         return dates_for_eval, gnm, dgnm
     else:
         return dates_for_eval, gnm
 
 
-def build_gnm_from_spline_coeffs(dates_for_eval, spl_dates, spl_coeffs, spl_order, with_derivative):
+def build_gnm_from_spline_coeffs(dates_for_eval, spl_dates, spl_coeffs, spl_order, with_derivatives):
     """
     Method to build the gnm from the spline coeffs and the parameters of splines (center_dates, order, spacing).
     This method uses the class scipy.interpolate.BSpline.
 
     :param dates_for_eval: Dates where the splines must be computed
     :type dates_for_eval: np.array (dim: Nt)
     :param spl_dates: Dates of the splines (knots)
     :type spl_dates: np.array (dim: Nspl)
     :param spl_coeffs: Coefficients of the data in the Bspline basis
     :type spl_coeffs: np.array (dim: Nspl x Nb)
     :param spl_order: Order of the used splines
     :type spl_order: int
-    :param with_derivative: If True, returns the reconstructed dgnm/dt evaluated from derivative of splines
-    :type with_derivative: bool
-    :return: Dates, gnm evaluated from splines (and derivative of gnm evaluated from the derivative of splines if with_derivative is True)
-    :rtype: np.array (dim: Nt), np.array (dim: Nt x Nb) (, np.array (dim: Nt x Nb))
+    :param with_derivatives: If True, returns the reconstructed dgnm/dt and d2gnm/dt2 evaluated from derivatives of splines
+    :type with_derivatives: bool
+    :return: Dates, gnm evaluated from splines (and derivatives of gnm if with_derivatives is True)
+    :rtype: np.array (dim: Nt), np.array (dim: Nt x Nb) (, np.array (dim: Nt x Nb), np.array (dim: Nt x Nb))
     """
     import scipy.interpolate
 
     full_knots = get_full_knots(spl_dates, spl_order, len(spl_coeffs))
     bsplines = scipy.interpolate.BSpline(full_knots, spl_coeffs, spl_order, extrapolate=False)
 
     gnm = bsplines(dates_for_eval)
-    if with_derivative:
-        return dates_for_eval, gnm, bsplines(dates_for_eval, nu=1)
+    if with_derivatives:
+        return dates_for_eval, gnm, bsplines(dates_for_eval, nu=1), bsplines(dates_for_eval, nu=2)
     else:
         return dates_for_eval, gnm
 
 
 def read_spline_coeffs_file(file_name):
     """
     Extracts the spline coeffs and the spline parameters from a file
@@ -253,74 +253,76 @@
     :param keepRealisations: if True, searches for files matching real*mod* to load mean and RMS. Else, loads the latest mod* file.
     :type keepRealisations: bool (default: False)
     :return: 0 if everything went well, -1 otherwise
     :rtype: int
     """
     pattern = 'real*mod*' if keepRealisations else 'mod*'
 
-    measures_folders = {'MF': os.path.join(dataDirectory, 'models'),
-                        'EF': os.path.join(dataDirectory, 'models_ext')
-                        }
     # MF
     gnm_times = None
     measureFolder = os.path.join(dataDirectory, 'models')
     generic_model_path = os.path.join(measureFolder, pattern)
     model_files = glob.glob(str(generic_model_path))
 
     if len(model_files) == 0:
         print('No spline files matching {} were found in {} ! Aborting loading...'.format(pattern, measureFolder))
         return -1
 
     if keepRealisations:
         # Loads all the real files and computes the mean and rms
-        real_data = {'MF': [], 'SV': []}
+        real_data = {'MF': [], 'SV': [], 'SA': []}
         for real_file in model_files:
             # print(os.path.basename(real_file))
-            times, gnm, dgnm = build_gnm_from_file(real_file, with_derivative=True)
+            times, gnm, dgnm, d2gnm = build_gnm_from_file(real_file, with_derivatives=True)
             real_data['MF'].append(gnm)
             real_data['SV'].append(dgnm)
+            real_data['SA'].append(d2gnm)
             if gnm_times is None:
                 gnm_times = times
             else:
                 assert np.allclose(times, gnm_times)
 
-        mean_data = {}
-        rms_data = {}
+        model_data = {}
         for measure, data in real_data.items():
             data_as_array = np.array(data)
-            mean_data[measure] = np.mean(data_as_array, axis=0)
-            rms_data[measure] = np.std(data_as_array, axis=0)
+            # Real model data must have the shape (nb_times, nb_coeffs, nb_reals)
+            model_data[measure] = np.moveaxis(data_as_array, 0, 2)
     else:
         # Load the latest model in the directory
         model_files.sort(reverse=True)
-        print(os.path.basename(model_files[0]))
-        mean_data = {}
-        gnm_times, mean_data['MF'], mean_data['SV'] = build_gnm_from_file(model_files[0], with_derivative=True)
-        rms_data = {'MF': None, 'SV': None}
+        model_data = {}
+        # If no realisation, the model data has the shape (nb_times, nb_coeffs)
+        gnm_times, model_data['MF'], model_data['SV'], model_data['SA'] = build_gnm_from_file(model_files[0], with_derivatives=True)
 
     # EF
     gnm_times = None
     measureFolder = os.path.join(dataDirectory, 'models_ext')
 
     generic_model_path = os.path.join(measureFolder, pattern)
     model_files = glob.glob(str(generic_model_path))
 
     if len(model_files) == 0:
         print('No spline files matching {} were found in {} ! Aborting loading...'.format(pattern, measureFolder))
         return -1
 
+    # Get the mean dipolar coefficients
+    if keepRealisations:
+        mean_dip = model_data['MF'].mean(axis=2)[:, :3]
+    else:
+        mean_dip = model_data['MF'][:, :3]
+
     # Internal dipole to project from q10_cd to [q10, q11, s11]_geocentric
-    internal_dip = mean_data['MF'][:, :3] / np.linalg.norm(mean_data['MF'][:, :3], axis=1).reshape(len(mean_data['MF']), 1)
+    internal_dip = mean_dip / np.linalg.norm(mean_dip, axis=1).reshape(len(mean_dip), 1)
 
     if keepRealisations:
         # Loads all the real files and computes the mean and rms
         q10_data = []
         for real_file in model_files:
             # print(os.path.basename(real_file))
-            times, gnm = build_gnm_from_file(real_file, with_derivative=False)
+            times, gnm = build_gnm_from_file(real_file, with_derivatives=False)
             q10_data.append(gnm)
             if gnm_times is None:
                 gnm_times = times
             else:
                 assert np.allclose(times, gnm_times)
 
         q10_data = np.array(q10_data)
@@ -329,40 +331,39 @@
         nb_reals = q10_data.shape[0]
 
         real_ef_data = np.zeros((nb_reals, len(gnm_times), 3))
         # Transform q10_cd into [q10, q11, s11]_geocentric for every time
         for i_t in range(len(gnm_times)):
             real_ef_data[:, i_t] = - q10_data[:, i_t]*internal_dip[i_t]
 
-        mean_data['EF'] = np.mean(real_ef_data, axis=0)
-        rms_data['EF'] = np.std(real_ef_data, axis=0)
-
+        model_data['EF'] = np.moveaxis(real_ef_data, 0, 2)
     else:
         # Load the latest model in the directory
         model_files.sort(reverse=True)
 
-        gnm_times, q10_data = build_gnm_from_file(model_files[0], with_derivative=False)
+        gnm_times, q10_data = build_gnm_from_file(model_files[0], with_derivatives=False)
         q10_data = scaling_EF(q10_data)
 
         # Transform q10_cd into [q10, q11, s11]_geocentric for every time
         ef_data = - q10_data * internal_dip
 
-        mean_data['EF'] = ef_data
-        rms_data['EF'] = None
+        model_data['EF'] = ef_data
 
-    for measureName in mean_data.keys():
+    for measure_name, measure_data in model_data.items():
 
-        if measureName == "SV":
+        if measure_name == "SV":
             units = "nT/yr"
-        elif measureName.endswith('F'):
+        elif measure_name == "SA":
+            units = "nT/yr^2"
+        elif measure_name.endswith('F'):
             units = "nT"
         else:
             units = ""
 
-        Nb = mean_data[measureName].shape[-1]
+        Nb = measure_data.shape[1]
         Lb = np.sqrt(Nb + 1) - 1
         lmax = int(Lb)
         # Assert that Nb gives an integer Lb
         assert Lb == lmax
-        dataModel.addMeasure(measureName, measureName, lmax, units, data=mean_data[measureName], rmsdata=rms_data[measureName], times=gnm_times)
+        dataModel.addMeasure(measure_name, measure_name, lmax, units, data=measure_data, times=gnm_times)
 
     return 0
```

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/default.py` & `webgeodyn-0.9.2/webgeodyn/inout/default.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/enscore.py` & `webgeodyn-0.9.2/webgeodyn/inout/enscore.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/lod.py` & `webgeodyn-0.9.2/webgeodyn/inout/lod.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/midpath.py` & `webgeodyn-0.9.2/webgeodyn/inout/midpath.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/nath.py` & `webgeodyn-0.9.2/webgeodyn/inout/nath.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_asc.py` & `webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_asc.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_hdf5.py` & `webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_hdf5.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/pygeodyn_hdf5_forecasts.py` & `webgeodyn-0.9.2/webgeodyn/inout/pygeodyn_hdf5_forecasts.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/s1fs.py` & `webgeodyn-0.9.2/webgeodyn/inout/s1fs.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/s1fs2.py` & `webgeodyn-0.9.2/webgeodyn/inout/s1fs2.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/inout/zforecast.py` & `webgeodyn-0.9.2/webgeodyn/inout/zforecast.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/models/__init__.py` & `webgeodyn-0.9.2/webgeodyn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/models/model.py` & `webgeodyn-0.9.2/webgeodyn/models/model.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/models/models.py` & `webgeodyn-0.9.2/webgeodyn/models/models.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/GR_OBS_RMM_MF_less_bias.V29` & `webgeodyn-0.9.2/webgeodyn/obsdata/GR_OBS_RMM_MF_less_bias.V29`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/GR_OBS_RMM_SV.V29` & `webgeodyn-0.9.2/webgeodyn/obsdata/GR_OBS_RMM_SV.V29`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/README_GR_OBS_V29` & `webgeodyn-0.9.2/webgeodyn/obsdata/README_GR_OBS_V29`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/README_VOs_0112.txt` & `webgeodyn-0.9.2/webgeodyn/obsdata/README_VOs_0112.txt`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/VO_CHAMP_MF.0112` & `webgeodyn-0.9.2/webgeodyn/obsdata/VO_CHAMP_MF.0112`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/VO_CHAMP_SV.0112` & `webgeodyn-0.9.2/webgeodyn/obsdata/VO_CHAMP_SV.0112`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/VO_SWARM_MF.0112` & `webgeodyn-0.9.2/webgeodyn/obsdata/VO_SWARM_MF.0112`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/VO_SWARM_SV.0112` & `webgeodyn-0.9.2/webgeodyn/obsdata/VO_SWARM_SV.0112`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/__init__.py` & `webgeodyn-0.9.2/webgeodyn/obsdata/__init__.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/obsdata.py` & `webgeodyn-0.9.2/webgeodyn/obsdata/obsdata.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/obsdata/observatory.py` & `webgeodyn-0.9.2/webgeodyn/obsdata/observatory.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/processing/matrices.py` & `webgeodyn-0.9.2/webgeodyn/processing/matrices.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/processing/plm.py` & `webgeodyn-0.9.2/webgeodyn/processing/plm.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/processing/psd.py` & `webgeodyn-0.9.2/webgeodyn/processing/psd.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/processing/radon.py` & `webgeodyn-0.9.2/webgeodyn/processing/radon.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/processing/spectra.py` & `webgeodyn-0.9.2/webgeodyn/processing/spectra.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/server/datahandlers.py` & `webgeodyn-0.9.2/webgeodyn/server/datahandlers.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/server/server.py` & `webgeodyn-0.9.2/webgeodyn/server/server.py`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/tests/Spline_benchmark/real001_mf_int_coefs.dat` & `webgeodyn-0.9.2/webgeodyn/tests/Spline_benchmark/real001_mf_int_coefs.dat`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/tests/Spline_benchmark/real_001` & `webgeodyn-0.9.2/webgeodyn/tests/Spline_benchmark/real_001`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/tests/test_covobs_splines.py` & `webgeodyn-0.9.2/webgeodyn/tests/test_covobs_splines.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,27 +42,27 @@
         for j, center_date in enumerate(self.spl_dates):
             with self.subTest(date=center_date):
                 if j not in required_date_indexes:
                     self.assertEqual(covspl.eval_spline(eval_date, center_date, self.spl_order, self.knot_sp), 0.)
 
     def test_building_gnm_few_splines(self):
         """ Test the method building from the splines  """
-        dates_gnm, gnm = covspl.build_gnm_from_spline_coeffs(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivative=False)
+        dates_gnm, gnm = covspl.build_gnm_from_spline_coeffs(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivatives=False)
         self.assertTrue(np.alltrue(np.abs(gnm - self.gnm_benchmark) < ABS_TOL))
 
     def test_building_gnm_all_splines(self):
         """ Test the old method building from all the splines """
         dates_gnm, gnm = covspl.build_gnm_from_spline_coeffs_old(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivative=False, all_splines=True)
         self.assertTrue(np.alltrue(np.abs(gnm - self.gnm_benchmark) < ABS_TOL))
 
     def test_building_methods(self):
         """ Test that all methods give the same result """
         dates_gnm, gnm = covspl.build_gnm_from_spline_coeffs_old(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivative=False, all_splines=False)
         dates_gnm_2, gnm_2 = covspl.build_gnm_from_spline_coeffs_old(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivative=False, all_splines=True)
-        dates_gnm_3, gnm_3 = covspl.build_gnm_from_spline_coeffs(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivative=False)
+        dates_gnm_3, gnm_3 = covspl.build_gnm_from_spline_coeffs(self.dates_benchmark, self.spl_dates, self.spl_coeffs, self.spl_order, with_derivatives=False)
         np.testing.assert_equal(gnm, gnm_2)
         # Almost_equal as it uses different implementation of the bsplines (sp.signal.bspline vs. sp.interpolate.Bspline)
         np.testing.assert_almost_equal(gnm, gnm_3)
 
 
 if __name__ == '__main__':
     SUITE = unittest.TestLoader().loadTestsFromTestCase(TestBuildingFromSplines)
```

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/exportTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/exportTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/globeTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/globeTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/lodTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/lodTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/mainController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/mainController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/obsTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/obsTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/spectraTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/spectraTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/spherharmTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/spherharmTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/controller/timeseriesTabController.js` & `webgeodyn-0.9.2/webgeodyn/www/controller/timeseriesTabController.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/css/css.css` & `webgeodyn-0.9.2/webgeodyn/www/css/css.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/css/flex.css` & `webgeodyn-0.9.2/webgeodyn/www/css/flex.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/css/timeSlider.css` & `webgeodyn-0.9.2/webgeodyn/www/css/timeSlider.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/error_pages/50x.html` & `webgeodyn-0.9.2/webgeodyn/www/error_pages/50x.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/favicon.png` & `webgeodyn-0.9.2/webgeodyn/www/favicon.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/50x.svg` & `webgeodyn-0.9.2/webgeodyn/www/images/50x.svg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/arrow.png` & `webgeodyn-0.9.2/webgeodyn/www/images/arrow.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/core.png` & `webgeodyn-0.9.2/webgeodyn/www/images/core.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/crosssection.png` & `webgeodyn-0.9.2/webgeodyn/www/images/crosssection.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoAitoff.gif` & `webgeodyn-0.9.2/webgeodyn/www/images/demoAitoff.gif`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoCross.png` & `webgeodyn-0.9.2/webgeodyn/www/images/demoCross.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoGnm.png` & `webgeodyn-0.9.2/webgeodyn/www/images/demoGnm.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoLOD.png` & `webgeodyn-0.9.2/webgeodyn/www/images/demoLOD.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoObs.jpeg` & `webgeodyn-0.9.2/webgeodyn/www/images/demoObs.jpeg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoOrtho.gif` & `webgeodyn-0.9.2/webgeodyn/www/images/demoOrtho.gif`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/demoSpectra.jpeg` & `webgeodyn-0.9.2/webgeodyn/www/images/demoSpectra.jpeg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/downarrow.png` & `webgeodyn-0.9.2/webgeodyn/www/images/downarrow.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/export.svg` & `webgeodyn-0.9.2/webgeodyn/www/images/export.svg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/home.png` & `webgeodyn-0.9.2/webgeodyn/www/images/home.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/lod.svg` & `webgeodyn-0.9.2/webgeodyn/www/images/lod.svg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/logo_CNES.png` & `webgeodyn-0.9.2/webgeodyn/www/images/logo_CNES.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/logo_CNRS.jpg` & `webgeodyn-0.9.2/webgeodyn/www/images/logo_CNRS.jpg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/logo_ISTerre.png` & `webgeodyn-0.9.2/webgeodyn/www/images/logo_ISTerre.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/logo_UGA.png` & `webgeodyn-0.9.2/webgeodyn/www/images/logo_UGA.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/logo_geodynamo.png` & `webgeodyn-0.9.2/webgeodyn/www/images/logo_geodynamo.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/observatories.png` & `webgeodyn-0.9.2/webgeodyn/www/images/observatories.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/spectra.svg` & `webgeodyn-0.9.2/webgeodyn/www/images/spectra.svg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/images/spherharm.png` & `webgeodyn-0.9.2/webgeodyn/www/images/spherharm.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/index.html` & `webgeodyn-0.9.2/webgeodyn/www/index.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/index.js` & `webgeodyn-0.9.2/webgeodyn/www/index.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/data/110m.json` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/data/110m.json`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/data/50m.json` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/data/50m.json`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/earthcorevisu.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/index.html` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/index.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.all.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.all.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/CCapture.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/Whammy.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/Whammy.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.worker.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/gif.worker.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/tar.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/ccapture/tar.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/API.md` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/API.md`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/LICENSE` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/LICENSE`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/README.md` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/README.md`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3-scale-chromatic.v1.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/LICENSE` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/LICENSE`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/README.md` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/README.md`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/d3.geo.projection/d3-geo-projection.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/gif/gif.worker.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery-3.2.1.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery.mousewheel.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jquery/jquery.mousewheel.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/AUTHORS.txt` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/LICENSE.txt` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/jquery.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_25_333333_500x100.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_25_333333_500x100.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_35_f6a828_500x100.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-bg_gloss-wave_35_f6a828_500x100.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_222222_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_228ef1_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_228ef1_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_4b8e0b_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_4b8e0b_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_a83300_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_a83300_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_cccccc_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_cccccc_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ef8c08_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ef8c08_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffd27a_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffd27a_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffffff_256x240.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/index.html` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/index.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/package.json` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/jqueryui/package.json`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/math.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/mathjs/math.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/LICENSE` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/LICENSE`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold2.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Bold2.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic2.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-BoldItalic2.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic2.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Italic2.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular2.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/Lato-Regular2.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/accordion.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/ad.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/api.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/breadcrumb.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/button.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/card.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/checkbox.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/colorize.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/comment.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/container.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dimmer.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/divider.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/dropdown.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/embed.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/feed.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/flag.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/form.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/grid.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/header.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/icon.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/image.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/input.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/item.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/label.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/list.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/loader.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/menu.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/message.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/modal.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/nag.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/popup.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/progress.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rail.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/rating.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reset.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/reveal.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/search.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/segment.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/shape.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sidebar.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/site.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/state.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/statistic.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/step.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/sticky.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/tab.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/table.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/transition.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/video.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visibility.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/components/visit.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/lato.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/lato.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/package.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.css` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.css`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/semantic.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.eot` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.otf` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.svg` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.ttf` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff2` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/flags.png` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/semantic/themes/default/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/LICENSE.md` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/README.md` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/README.md`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/libs/topojson/topojson.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/parameters.html` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/parameters.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/pointinfo.html` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/pointinfo.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/EarthCoreVisu/view/videoexport.html` & `webgeodyn-0.9.2/webgeodyn/www/libs/EarthCoreVisu/view/videoexport.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/canvg/canvg.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/canvg/canvg.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/canvg/download.min.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/canvg/download.min.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-3d.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-3d.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-3d.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-3d.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-more.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts-more.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts-more.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/highcharts.js.map` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/highcharts.js.map`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/export-data.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/export-data.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/exporting.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/exporting.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/heatmap.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/heatmap.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/libs/highcharts/modules/offline-exporting.js` & `webgeodyn-0.9.2/webgeodyn/www/libs/highcharts/modules/offline-exporting.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/genericData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/genericData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/globeData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/globeData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/lodData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/lodData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/measureUnits.js` & `webgeodyn-0.9.2/webgeodyn/www/model/measureUnits.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/observatoryData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/observatoryData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/spectraData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/spectraData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/spherHarmData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/spherHarmData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/model/timeSerieData.js` & `webgeodyn-0.9.2/webgeodyn/www/model/timeSerieData.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/alertUser.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/alertUser.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/dataDropdown.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/dataDropdown.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/dropdown.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/dropdown.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/imshowPlot.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/imshowPlot.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/measureDropdown.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/measureDropdown.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/modelSelector.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/modelSelector.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/ui/timeSlider.js` & `webgeodyn-0.9.2/webgeodyn/www/ui/timeSlider.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/utils/banner.js` & `webgeodyn-0.9.2/webgeodyn/www/utils/banner.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/utils/utils.js` & `webgeodyn-0.9.2/webgeodyn/www/utils/utils.js`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/export.html` & `webgeodyn-0.9.2/webgeodyn/www/view/export.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/globe.html` & `webgeodyn-0.9.2/webgeodyn/www/view/globe.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/home.html` & `webgeodyn-0.9.2/webgeodyn/www/view/home.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/imshowparameters.html` & `webgeodyn-0.9.2/webgeodyn/www/view/imshowparameters.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/observatories.html` & `webgeodyn-0.9.2/webgeodyn/www/view/observatories.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/spherharm.html` & `webgeodyn-0.9.2/webgeodyn/www/view/spherharm.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn/www/view/timeseries.html` & `webgeodyn-0.9.2/webgeodyn/www/view/timeseries.html`

 * *Files identical despite different names*

### Comparing `webgeodyn-0.9.1/webgeodyn.egg-info/PKG-INFO` & `webgeodyn-0.9.2/webgeodyn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webgeodyn
-Version: 0.9.1
+Version: 0.9.2
 Summary: A web-based plot tool to visualize Earth core flows
 Home-page: https://gricad-gitlab.univ-grenoble-alpes.fr/Geodynamo/webgeodyn
 Author: Nicolas Gillet, Loïc Huder, Yannick Martin, Franck Thollard
 Author-email: loic.huder@univ-grenoble-alpes.fr
 License: UNKNOWN
 Description: #########
         webgeodyn
```

### Comparing `webgeodyn-0.9.1/webgeodyn.egg-info/SOURCES.txt` & `webgeodyn-0.9.2/webgeodyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

