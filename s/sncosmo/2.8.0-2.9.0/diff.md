# Comparing `tmp/sncosmo-2.8.0.tar.gz` & `tmp/sncosmo-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sncosmo-2.8.0.tar", last modified: Thu Mar 17 03:48:14 2022, max compression
+gzip compressed data, was "sncosmo-2.9.0.tar", last modified: Tue Sep 27 17:57:52 2022, max compression
```

## Comparing `sncosmo-2.8.0.tar` & `sncosmo-2.9.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.249413 sncosmo-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-03-17 03:47:58.000000 sncosmo-2.8.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-03-17 03:47:58.000000 sncosmo-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-03-17 03:48:14.253413 sncosmo-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-03-17 03:47:58.000000 sncosmo-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-17 03:47:58.000000 sncosmo-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-03-17 03:48:14.253413 sncosmo-2.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      605 2022-03-17 03:47:58.000000 sncosmo-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.241413 sncosmo-2.8.0/sncosmo/
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8259 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    16460 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/bandpasses.py
--rw-r--r--   0 runner    (1001) docker     (121)    58149 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.237413 sncosmo-2.8.0/sncosmo/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.237413 sncosmo-2.8.0/sncosmo/data/bandpasses/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.241413 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/bessell_b.dat
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/bessell_i.dat
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/bessell_r.dat
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/bessell_ux.dat
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/bandpasses/bessell/bessell_v.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.245413 sncosmo-2.8.0/sncosmo/data/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/examples/example_photometric_data.dat
--rw-r--r--   0 runner    (1001) docker     (121)    45020 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/examples/example_spectrum.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.245413 sncosmo-2.8.0/sncosmo/data/models/
--rw-r--r--   0 runner    (1001) docker     (121)    46080 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/data/models/Hsiao_SED_V3_subsampled.fits
--rw-r--r--   0 runner    (1001) docker     (121)    54600 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)    26327 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/magsystems.py
--rw-r--r--   0 runner    (1001) docker     (121)    74672 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/photdata.py
--rw-r--r--   0 runner    (1001) docker     (121)    18613 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4429 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    16363 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/salt2utils.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     8520 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)    18444 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/snanaio.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/sncosmo.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7445 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/snfitio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/specmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    19547 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.245413 sncosmo-2.8.0/sncosmo/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.249413 sncosmo-2.8.0/sncosmo/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.249413 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_g.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_i.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_r.dat
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_z.dat
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lightfile
--rw-r--r--   0 runner    (1001) docker     (121)    26232 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/covmat_lc-03D4ag.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.249413 sncosmo-2.8.0/sncosmo/tests/data/dust_subsection/
--rw-r--r--   0 runner    (1001) docker     (121)    46080 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/dust_subsection/SFD_dust_4096_ngp.fits
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_evalx.dat
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_evaly.dat
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_input.dat
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_result.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/lc-03D4ag.list
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_params_times.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSg.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSi.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSr.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_2.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_3.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_4.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_ascii_example.dat
--rw-r--r--   0 runner    (1001) docker     (121)    17280 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_fits_example_head.fits
--rw-r--r--   0 runner    (1001) docker     (121)    20160 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_fits_example_phot.fits
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example.dat
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_coadd.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_doc.dat
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_invalid.dat
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_noend.dat
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snfit_filter_g_0.dat
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snfit_filter_g_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snfit_filter_z_0.dat
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/data/snfit_filter_z_1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     3841 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_bandpasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_download_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     7596 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6727 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_magsystems.py
--rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_photdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_salt2source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_salt2utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_snanaio.py
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_sugarsource.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16623 2022-03-17 03:47:58.000000 sncosmo-2.8.0/sncosmo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 03:48:14.241413 sncosmo-2.8.0/sncosmo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-03-17 03:48:13.000000 sncosmo-2.8.0/sncosmo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-03-17 03:48:14.000000 sncosmo-2.8.0/sncosmo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 03:48:13.000000 sncosmo-2.8.0/sncosmo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 03:48:12.000000 sncosmo-2.8.0/sncosmo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-03-17 03:48:13.000000 sncosmo-2.8.0/sncosmo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-17 03:48:14.000000 sncosmo-2.8.0/sncosmo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.984500 sncosmo-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-09-27 17:57:41.000000 sncosmo-2.9.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-27 17:57:41.000000 sncosmo-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-09-27 17:57:52.984500 sncosmo-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-09-27 17:57:41.000000 sncosmo-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-27 17:57:41.000000 sncosmo-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-09-27 17:57:52.984500 sncosmo-2.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      605 2022-09-27 17:57:41.000000 sncosmo-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.976500 sncosmo-2.9.0/sncosmo/
+-rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8259 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16460 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/bandpasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59169 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.972500 sncosmo-2.9.0/sncosmo/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.972500 sncosmo-2.9.0/sncosmo/data/bandpasses/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.976500 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/bessell_b.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/bessell_i.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/bessell_r.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/bessell_ux.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/bandpasses/bessell/bessell_v.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.976500 sncosmo-2.9.0/sncosmo/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2360 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/examples/example_photometric_data.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    45020 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/examples/example_spectrum.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.976500 sncosmo-2.9.0/sncosmo/data/models/
+-rw-r--r--   0 runner    (1001) docker     (121)    46080 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/data/models/Hsiao_SED_V3_subsampled.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    54600 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26327 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/magsystems.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74672 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/photdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18613 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4429 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16363 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/salt2utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     8520 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18444 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/snanaio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/sncosmo.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7445 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/snfitio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/specmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19547 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.980500 sncosmo-2.9.0/sncosmo/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.984500 sncosmo-2.9.0/sncosmo/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.984500 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_g.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_i.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_r.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_z.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lightfile
+-rw-r--r--   0 runner    (1001) docker     (121)    26232 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/covmat_lc-03D4ag.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.984500 sncosmo-2.9.0/sncosmo/tests/data/dust_subsection/
+-rw-r--r--   0 runner    (1001) docker     (121)    46080 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/dust_subsection/SFD_dust_4096_ngp.fits
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_evalx.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_evaly.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_input.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_result.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/lc-03D4ag.list
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_params_times.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSg.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSi.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSr.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_2.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_3.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_4.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_ascii_example.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    17280 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_fits_example_head.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    20160 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_fits_example_phot.fits
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_coadd.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_doc.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_invalid.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_noend.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snfit_filter_g_0.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snfit_filter_g_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snfit_filter_z_0.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/data/snfit_filter_z_1.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     3841 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_bandpasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_download_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7596 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6727 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_magsystems.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_photdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4599 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_salt2source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_salt2utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_snanaio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6782 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_sugarsource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16623 2022-09-27 17:57:41.000000 sncosmo-2.9.0/sncosmo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 17:57:52.976500 sncosmo-2.9.0/sncosmo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-27 17:57:52.000000 sncosmo-2.9.0/sncosmo.egg-info/top_level.txt
```

### Comparing `sncosmo-2.8.0/LICENSE.rst` & `sncosmo-2.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/PKG-INFO` & `sncosmo-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sncosmo
-Version: 2.8.0
+Version: 2.9.0
 Summary: Package for supernova cosmology based on astropy
 Home-page: https://sncosmo.readthedocs.org
 Author: The SNCosmo Developers
 Author-email: kylebarbary@gmail.com
 License: BSD 3-Clause License
 Keywords: supernova,cosmology
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -35,9 +34,7 @@
 [![PyPI](https://img.shields.io/pypi/v/sncosmo.svg?style=flat-square)](https://pypi.python.org/pypi/sncosmo)
 [![Anaconda](https://anaconda.org/conda-forge/sncosmo/badges/version.svg)](https://anaconda.org/conda-forge/sncosmo)
 [![ASCL](https://img.shields.io/badge/ascl-1611.017-blue.svg?colorB=262255)](https://ascl.net/1611.017)
 
 **Documentation:** http://sncosmo.readthedocs.io
 
 **Citing sncosmo:** [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.592747.svg)](https://doi.org/10.5281/zenodo.592747)
-
-
```

### Comparing `sncosmo-2.8.0/README.md` & `sncosmo-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/setup.cfg` & `sncosmo-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/setup.py` & `sncosmo-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/__init__.py` & `sncosmo-2.9.0/sncosmo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import os
 
 from astropy.config import ConfigItem, ConfigNamespace
 from astropy.config.configuration import update_default_config
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 
 
 def test(package=None, test_path=None, args=None, plugins=None,
          verbose=False, pastebin=None, pep8=False,
          pdb=False, coverage=False, open_files=False, **kwargs):
     """
     Run the tests using py.test. A proper set of arguments is constructed and
```

### Comparing `sncosmo-2.8.0/sncosmo/_registry.py` & `sncosmo-2.9.0/sncosmo/_registry.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/bandpasses.py` & `sncosmo-2.9.0/sncosmo/bandpasses.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/builtins.py` & `sncosmo-2.9.0/sncosmo/builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,14 +496,28 @@
                     'and atmosphere.)')}
 for filt in ['J', 'H', 'Ks']:
     name = '2mass' + filt.lower()
     relpath = 'bandpasses/2mass/2mass.{}'.format(filt)
     _BANDPASSES.register_loader(name, load_bandpass_remote_aa,
                                 args=(relpath,), meta=twomass_meta)
 
+# Gaia
+gaia_meta = {
+    'filterset': 'gaia',
+    'retrieved': '27 Sep 2022',
+    'dataurl': ('http://svo2.cab.inta-csic.es/svo/theory/fps/getdata.php?'
+                'format=ascii&id=Misc'),
+    'description': ('eDR3 Gaia filters from SVO (includes filter, instrument,'
+                    'and optics.)')}
+for filt in ['Gbp', 'G', 'Grp', 'Grvs']:
+    name = 'gaia::' + filt.lower()
+    relpath = 'bandpasses/gaia/gaia.{}'.format(filt)
+    _BANDPASSES.register_loader(name, load_bandpass_remote_aa,
+                                args=(relpath,), meta=gaia_meta)
+
 # =============================================================================
 # interpolators
 
 megacam_meta = {'filterset': 'megacampsf'}
 
 
 def load_megacampsf(letter, name=None):
@@ -704,21 +718,32 @@
        '<https://arxiv.org/abs/1808.02534>')
 meta = {'type': 'SN Ia',
         'subclass': '`~sncosmo.SALT2Source`', 'ref': ref}
 _SOURCES.register_loader('salt2-extended', load_salt2model,
                          args=('models/pierel/salt2-extended',), version='2.0',
                          meta=meta)
 
+# SALT3-NIR
+meta = {'type': 'SN Ia',
+        'subclass': '`~sncosmo.SALT3Source`',
+        'url': 'https://doi.org/10.5281/zenodo.7068818',
+        'note': """See Pierel et al. 2022, ApJ."""}
+_SOURCES.register_loader('salt3-nir', load_salt3model,
+                         args=('models/salt3-nir/salt3nir-p22',),
+                         version='1.0',
+                         meta=meta)
+
 # SALT3
 meta = {'type': 'SN Ia',
         'subclass': '`~sncosmo.SALT3Source`',
         'url': 'https://salt3.readthedocs.io/en/latest/',
-        'note': "See Kenworthy et al. 2021, ApJ, submitted."}
+        'note': """See Kenworthy et al. 2021, ApJ, 923, 265K.
+Revised with Fragilistic calibration (Brout et al., 2022)"""}
 _SOURCES.register_loader('salt3', load_salt3model,
-                         args=('models/salt3/salt3-k21',), version='1.0',
+                         args=('models/salt3/salt3-f22',), version='2.0',
                          meta=meta)
 
 meta = {'type': 'SN Ia',
         'subclass': '`~sncosmo.SALT2Source`',
         'url': 'http://snana.uchicago.edu/',
         'note': "extracted from SNANA's SNDATA_ROOT on 24 April 2018. SALT2"
         " model with wide wavelength range, Hounsell et al. 2017",
```

### Comparing `sncosmo-2.8.0/sncosmo/conftest.py` & `sncosmo-2.9.0/sncosmo/conftest.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/data/examples/example_photometric_data.dat` & `sncosmo-2.9.0/sncosmo/data/examples/example_photometric_data.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/data/examples/example_spectrum.dat` & `sncosmo-2.9.0/sncosmo/data/examples/example_spectrum.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/data/models/Hsiao_SED_V3_subsampled.fits` & `sncosmo-2.9.0/sncosmo/data/models/Hsiao_SED_V3_subsampled.fits`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/fitting.py` & `sncosmo-2.9.0/sncosmo/fitting.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/io.py` & `sncosmo-2.9.0/sncosmo/io.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/magsystems.py` & `sncosmo-2.9.0/sncosmo/magsystems.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/models.py` & `sncosmo-2.9.0/sncosmo/models.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/photdata.py` & `sncosmo-2.9.0/sncosmo/photdata.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/plotting.py` & `sncosmo-2.9.0/sncosmo/plotting.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/registry.py` & `sncosmo-2.9.0/sncosmo/registry.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/salt2utils.pyx` & `sncosmo-2.9.0/sncosmo/salt2utils.pyx`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/simulation.py` & `sncosmo-2.9.0/sncosmo/simulation.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/snanaio.py` & `sncosmo-2.9.0/sncosmo/snanaio.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/snfitio.py` & `sncosmo-2.9.0/sncosmo/snfitio.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/specmodel.py` & `sncosmo-2.9.0/sncosmo/specmodel.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/spectrum.py` & `sncosmo-2.9.0/sncosmo/spectrum.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_g.dat` & `sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_g.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_i.dat` & `sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_i.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_r.dat` & `sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_r.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_z.dat` & `sncosmo-2.9.0/sncosmo/tests/data/SNLS3-04D3gx/lc2fit_z.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/covmat_lc-03D4ag.dat` & `sncosmo-2.9.0/sncosmo/tests/data/covmat_lc-03D4ag.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/dust_subsection/SFD_dust_4096_ngp.fits` & `sncosmo-2.9.0/sncosmo/tests/data/dust_subsection/SFD_dust_4096_ngp.fits`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_input.dat` & `sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_input.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/interpolation_test_result.dat` & `sncosmo-2.9.0/sncosmo/tests/data/interpolation_test_result.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/lc-03D4ag.list` & `sncosmo-2.9.0/sncosmo/tests/data/lc-03D4ag.list`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSg.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSg.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSi.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSi.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSr.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_rcov_snfit_SDSSr.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_1.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_1.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_2.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_2.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_3.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_3.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/salt2_timeseries_4.dat` & `sncosmo-2.9.0/sncosmo/tests/data/salt2_timeseries_4.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_ascii_example.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_ascii_example.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_fits_example_head.fits` & `sncosmo-2.9.0/sncosmo/tests/data/snana_fits_example_head.fits`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_fits_example_phot.fits` & `sncosmo-2.9.0/sncosmo/tests/data/snana_fits_example_phot.fits`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_coadd.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_coadd.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_doc.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_doc.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_invalid.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_invalid.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/data/snana_simlib_example_noend.dat` & `sncosmo-2.9.0/sncosmo/tests/data/snana_simlib_example_noend.dat`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_bandpasses.py` & `sncosmo-2.9.0/sncosmo/tests/test_bandpasses.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_builtins.py` & `sncosmo-2.9.0/sncosmo/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_download_builtins.py` & `sncosmo-2.9.0/sncosmo/tests/test_download_builtins.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_fitting.py` & `sncosmo-2.9.0/sncosmo/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_io.py` & `sncosmo-2.9.0/sncosmo/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_magsystems.py` & `sncosmo-2.9.0/sncosmo/tests/test_magsystems.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_models.py` & `sncosmo-2.9.0/sncosmo/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_photdata.py` & `sncosmo-2.9.0/sncosmo/tests/test_photdata.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_plotting.py` & `sncosmo-2.9.0/sncosmo/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_registry.py` & `sncosmo-2.9.0/sncosmo/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_salt2source.py` & `sncosmo-2.9.0/sncosmo/tests/test_salt2source.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_salt2utils.py` & `sncosmo-2.9.0/sncosmo/tests/test_salt2utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         extinction[idx_between] = np.polyval(np.flipud(coeffs), l[idx_between])
 
         return -extinction
 
     colorlaw = SALT2ColorLaw(colorlaw_range, colorlaw_coeffs)
 
     wave = np.linspace(2000., 9200., 201)
-    assert np.all(colorlaw(wave) == colorlaw_python(wave))
+    np.testing.assert_allclose(colorlaw(wave), colorlaw_python(wave))
 
 
 def test_salt2colorlaw_pickle():
 
     colorlaw_coeffs = [-0.504294, 0.787691, -0.461715, 0.0815619]
     colorlaw_range = (2800., 7000.)
     colorlaw = SALT2ColorLaw(colorlaw_range, colorlaw_coeffs)
```

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_simulation.py` & `sncosmo-2.9.0/sncosmo/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_snanaio.py` & `sncosmo-2.9.0/sncosmo/tests/test_snanaio.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_spectrum.py` & `sncosmo-2.9.0/sncosmo/tests/test_spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     wave = np.logspace(np.log10(3000), np.log10(8000), 100)
     flux = np.ones_like(wave)
     spec = sncosmo.Spectrum(wave, flux)
 
     assert_allclose(wave, spec.wave, rtol=1.e-5)
 
 
+@pytest.mark.might_download
 class TestSpectrum:
     def setup_class(self):
         # Simulate a spectrum
         model = sncosmo.Model(source='hsiao-subsampled')
         params = {'t0': 10., 'amplitude': 1.e-7, 'z': 0.2}
         start_params = {'t0': 0., 'amplitude': 1., 'z': 0.}
         model.set(**params)
```

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_sugarsource.py` & `sncosmo-2.9.0/sncosmo/tests/test_sugarsource.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/tests/test_utils.py` & `sncosmo-2.9.0/sncosmo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo/utils.py` & `sncosmo-2.9.0/sncosmo/utils.py`

 * *Files identical despite different names*

### Comparing `sncosmo-2.8.0/sncosmo.egg-info/PKG-INFO` & `sncosmo-2.9.0/sncosmo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sncosmo
-Version: 2.8.0
+Version: 2.9.0
 Summary: Package for supernova cosmology based on astropy
 Home-page: https://sncosmo.readthedocs.org
 Author: The SNCosmo Developers
 Author-email: kylebarbary@gmail.com
 License: BSD 3-Clause License
 Keywords: supernova,cosmology
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -35,9 +34,7 @@
 [![PyPI](https://img.shields.io/pypi/v/sncosmo.svg?style=flat-square)](https://pypi.python.org/pypi/sncosmo)
 [![Anaconda](https://anaconda.org/conda-forge/sncosmo/badges/version.svg)](https://anaconda.org/conda-forge/sncosmo)
 [![ASCL](https://img.shields.io/badge/ascl-1611.017-blue.svg?colorB=262255)](https://ascl.net/1611.017)
 
 **Documentation:** http://sncosmo.readthedocs.io
 
 **Citing sncosmo:** [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.592747.svg)](https://doi.org/10.5281/zenodo.592747)
-
-
```

### Comparing `sncosmo-2.8.0/sncosmo.egg-info/SOURCES.txt` & `sncosmo-2.9.0/sncosmo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

