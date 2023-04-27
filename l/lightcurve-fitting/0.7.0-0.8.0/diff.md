# Comparing `tmp/lightcurve-fitting-0.7.0.tar.gz` & `tmp/lightcurve-fitting-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurve-fitting-0.7.0.tar", last modified: Tue Oct 25 19:45:25 2022, max compression
+gzip compressed data, was "lightcurve-fitting-0.8.0.tar", last modified: Thu Apr 27 23:06:47 2023, max compression
```

## Comparing `lightcurve-fitting-0.7.0.tar` & `lightcurve-fitting-0.8.0.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    35149 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/LICENSE
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      411 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/MANIFEST.in
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/PKG-INFO
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      650 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/README.md
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.343836 lightcurve-fitting-0.7.0/docs/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      673 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/docs/Makefile
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      797 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/docs/make.bat
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.343836 lightcurve-fitting-0.7.0/docs/source/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1065 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/docs/source/api.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6603 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/docs/source/conf.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1764 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/docs/source/index.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      382 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/docs/source/installation.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5565 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/docs/source/release-history.rst
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    11426 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/docs/source/usage.rst
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/lightcurve_fitting/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       93 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/__init__.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      497 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/lightcurve_fitting/_version.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    31334 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/bolometric.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.343836 lightcurve-fitting-0.7.0/lightcurve_fitting/example/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    39520 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/example/SN2016bkv.txt
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/ATLAS_cyan.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/ATLAS_orange.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3760 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4565 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.g.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5036 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.i.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5017 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.r.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4937 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7261 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    26420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    15466 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8800 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    17644 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      473 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Cousins.I.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      583 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Cousins.R.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      220 2021-11-29 19:14:50.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Johnson.B.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      260 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Johnson.U.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      300 2021-11-29 19:14:58.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Johnson.V.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6447 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4767 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8458 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    11362 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    14404 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    20246 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    20613 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4329 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     6967 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3256 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     4137 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5171 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7703 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9324 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    13773 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    15841 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    17399 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    22099 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/KAF-1001E.asci
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2990 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/KAF-1001E.csv
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    13083 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     5068 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2295 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1664 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1729 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1500 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      940 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2870 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3129 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.B.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2247 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.U.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3486 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8547 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     7623 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3066 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.V.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     9139 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/TESS_TESS.Red.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)   276480 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      218 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/json2txt.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    22364 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/orange.asci
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     8768 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/orange.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       72 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/pseudobolometric.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       38 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters/white.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    19684 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/filters.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    17815 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/fitting.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    27280 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/lightcurve.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/lightcurve_fitting/models/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    10653 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/models/sifto.dat
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    33577 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/models.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      165 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/serif.mplstyle
--rwxrwxr-x   0 griffin   (1002) griffin   (1002)    23674 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/lightcurve_fitting/speccal.py
-drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2022-10-25 19:45:25.343836 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/PKG-INFO
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     3648 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/SOURCES.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)        1 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/dependency_links.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       20 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/entry_points.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       62 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/requires.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)       19 2022-10-25 19:45:25.000000 lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/top_level.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      117 2022-03-18 17:02:27.000000 lightcurve-fitting-0.7.0/requirements.txt
--rw-rw-r--   0 griffin   (1002) griffin   (1002)      200 2022-10-25 19:45:25.351837 lightcurve-fitting-0.7.0/setup.cfg
--rw-rw-r--   0 griffin   (1002) griffin   (1002)     2183 2022-10-25 19:41:42.000000 lightcurve-fitting-0.7.0/setup.py
--rw-rw-r--   0 griffin   (1002) griffin   (1002)    68611 2021-09-29 18:54:17.000000 lightcurve-fitting-0.7.0/versioneer.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    35149 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/LICENSE
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      411 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/MANIFEST.in
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/PKG-INFO
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      650 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/README.md
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.798112 lightcurve-fitting-0.8.0/docs/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      673 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/Makefile
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      797 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/make.bat
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/docs/source/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1065 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/docs/source/api.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6603 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/docs/source/conf.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1764 2023-01-27 00:13:14.000000 lightcurve-fitting-0.8.0/docs/source/index.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      382 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/docs/source/installation.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8437 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/docs/source/release-history.rst
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    12589 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/docs/source/usage.rst
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       93 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/__init__.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      497 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/_version.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    31353 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/bolometric.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/lightcurve_fitting/example/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    41040 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/example/SN2016bkv.txt
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_cyan.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      570 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_orange.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3760 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4565 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.g.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5036 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.i.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5017 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.r.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4937 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7261 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    26420 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    15466 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8800 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    17644 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      473 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.I.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      583 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.R.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      220 2021-11-29 19:14:50.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.B.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      260 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.U.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      300 2021-11-29 19:14:58.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Johnson.V.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6447 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4767 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8458 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    11362 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    14404 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    20246 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    20613 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4329 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     6967 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3256 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     4137 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5171 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7703 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9324 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    13773 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7999 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F300M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9858 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F335M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    15841 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9708 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F360M.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    17399 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    22099 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.asci
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2990 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.csv
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    13083 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     5068 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2295 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1664 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1729 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1780 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1500 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      940 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2870 2022-03-18 17:02:27.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3129 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.B.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2247 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.U.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3486 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8547 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     7623 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3066 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.V.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     9139 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/TESS_TESS.Red.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)   276480 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      218 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/json2txt.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    22364 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.asci
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     8768 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       72 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/pseudobolometric.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       38 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters/white.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    21381 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/filters.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    19574 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/fitting.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    38783 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/lightcurve.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/lightcurve_fitting/models/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    10653 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/models/sifto.dat
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    37345 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/models.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      165 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/serif.mplstyle
+-rwxrwxr-x   0 griffin   (1002) griffin   (1002)    23773 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/lightcurve_fitting/speccal.py
+drwxrwxr-x   0 griffin   (1002) griffin   (1002)        0 2023-04-27 23:06:47.802112 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     1177 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/PKG-INFO
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     3795 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/SOURCES.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)        1 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/dependency_links.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       20 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/entry_points.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       65 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/requires.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)       19 2023-04-27 23:06:47.000000 lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/top_level.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      122 2023-04-27 23:03:45.000000 lightcurve-fitting-0.8.0/requirements.txt
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)      200 2023-04-27 23:06:47.810112 lightcurve-fitting-0.8.0/setup.cfg
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)     2183 2022-10-25 19:41:42.000000 lightcurve-fitting-0.8.0/setup.py
+-rw-rw-r--   0 griffin   (1002) griffin   (1002)    68611 2021-09-29 18:54:17.000000 lightcurve-fitting-0.8.0/versioneer.py
```

### Comparing `lightcurve-fitting-0.7.0/LICENSE` & `lightcurve-fitting-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/PKG-INFO` & `lightcurve-fitting-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurve-fitting
-Version: 0.7.0
+Version: 0.8.0
 Summary: Tools to fit analytical models to multiband light curves of astronomical transients
 Home-page: https://github.com/griffin-h/lightcurve_fitting
 Author: Griffin Hosseinzadeh
 Author-email: griffin0@arizona.edu
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lightcurve-fitting-0.7.0/README.md` & `lightcurve-fitting-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/Makefile` & `lightcurve-fitting-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/make.bat` & `lightcurve-fitting-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/source/api.rst` & `lightcurve-fitting-0.8.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/source/conf.py` & `lightcurve-fitting-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/source/index.rst` & `lightcurve-fitting-0.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/docs/source/usage.rst` & `lightcurve-fitting-0.8.0/docs/source/usage.rst`

 * *Files 7% similar despite different names*

```diff
@@ -19,72 +19,75 @@
 The following column names are used by the package, although the light curve can have extra columns
 [alternative column names are given in square brackets]:
 
  * MJD (required): modified Julian date of the observation [mjd, JD, jd (JD/jd are converted)]
  * mag (required): magnitude of the observation [Magnitude, Mag, ab_mag, PSFmag, MAG, omag, magnitude, apparent_mag]
  * dmag (required): uncertainty on the magnitude [Magnitude_Error, magerr, MagErr, mag_err, e_mag, Error, err, PSFerr,
    MAGERR, e_omag, e_magnitude, apparent_mag_err, Mag_Err, emag]
- * filt (required): name of the filter [filter, Filter, band, FLT, Band]
- * filter (automatic): the filter object (see :ref:`Filters` below)
+ * filter (required): name of the filter [filter, filt Filter, band, FLT, Band] (see :ref:`Filters` below)
  * nondet: True if the magnitude is an upper limit, False otherwise [Is_Limit, UL, l_omag, upper_limit, upperlimit]
  * flux: the spectral flux density (:math:`F_ν`, arbitrary units) of the observation [FLUXCAL]
  * dflux: uncertainty on the flux [FLUXCALERR]
  * phase: time since a reference date (e.g., peak or explosion) in rest-frame days [Phase, PHASE]
  * absmag: absolute magnitude of the observation
  * lum: the spectral luminosity density (:math:`L_ν`, in watts/hertz) of the observation
  * dlum: the uncertainty on the spectral luminosity density
  * telescope: the name of the telescope/instrument where this observation was carried out [Telescope, Tel, tel+inst]
  * source: the data source, either a telescope/instrument name or a literature reference [Source]
 
-The :attr:`LC.meta` attribute contains information needed to calculate absolute magnitudes and luminosities:
+The :attr:`LC.meta` attribute contains information needed to calculate absolute magnitudes, luminosities, and rest-frame phases:
 
  * dm: the distance modulus
- * extinction: a dictionary containing Milky Way extinction corrections for each filter
- * hostext: a dictionary containing host galaxy extinction corrections for each filter
+ * ebv: the selective extinction due to dust in the Milky Way
+ * host_ebv: the selective extinction due to dust in the host galaxy (applied at the target redshift)
+ * redshift: the redshift (also used to calculate distance if the distance modulus is not given)
 
 .. code-block:: python
 
     lc.meta['dm'] = 30.79
-    lc.meta['extinction'] = {
-     'U': 0.069,
-     'B': 0.061,
-     'g': 0.055,
-     'V': 0.045,
-     '0': 0.035,
-     'r': 0.038,
-     'R': 0.035,
-     'i': 0.028,
-     'I': 0.025,
-    }
+    lc.meta['ebv'] = 0.016
+    lc.meta['host_ebv'] = 0.
+    lc.meta['redshift'] = 0.002
 
 The :class:`.LC` object has several methods for converting between the columns above,
 as well as a method for plotting the light curve in a single command:
 
 .. code-block:: python
 
     lc.calcAbsMag()
-    lc.plot(xcol='MJD')
+    lc.calcPhase()
+    lc.plot()
 
 Filters
 -------
-The :mod:`.filters` submodule defines a :class:`.Filter` object that stores information about the broadband filters: transmission
-function, photometric system, and styles for plotting. You mostly won't have to touch this module, unless you are
-adding new filters.
+The :mod:`.filters` submodule defines a :class:`.Filter` object that stores information about the broadband filters: transmission function, photometric system, and styles for plotting.
+You mostly won't have to touch this module, unless you are adding or modifying filters.
+
+The ``'filter'`` column in a :class:`.LC` object contains :class:`.Filter` objects, rather than strings.
+However, you can use filter names directly in most places, including the :meth:`.LC.where` method, and they will be parsed into :class:`.Filter` objects.
+For example, ``lc.where(filter='r')`` will return photometry points in bands labeled both 'r' and 'rp' in your input file.
+
+If you ever need direct access to the :class:`.Filter` objects by name, you can use the filter lookup dictionary.
+
+.. code-block:: python
+
+    from lightcurve_fitting.filters import filtdict
+
+    g = filtdict['g']
+    print(g)
 
 Bolometric Light Curves
 -----------------------
 You can make a bolometric light curve and color curves from the photometry table with the :mod:`.bolometric` module.
 
 .. code-block:: python
 
     from lightcurve_fitting.bolometric import calculate_bolometric, plot_bolometric_results, plot_color_curves
 
-    redshift = 0.002
-    outpath = '/Users/griffin/Desktop/SN2016bkv_bolometric'
-    t = calculate_bolometric(lc, redshift, outpath, colors=['B-V', 'g-r', 'r-i'])
+    t = calculate_bolometric(lc, outpath='./SN2016bkv_bolometric', colors=['B-V', 'g-r', 'r-i'])
     print(t)
     plot_bolometric_results(t)
     plot_color_curves(t)
 
 The light curve is divided into epochs (defined by the ``bin`` and ``also_group_by`` arguments to :func:`.calculate_bolometric`), and processed four different ways:
 
  * Fitting the Planck function using :func:`scipy.optimize.curve_fit`. This is very fast but may not give reliable uncertainties.
@@ -133,25 +136,27 @@
 .. math::
     \sigma_{i,\mathrm{eff}} = \sqrt{ \sigma_i^2 + \left( \sigma * \bar{\sigma} \right)^2 }
 
 For bolometric light curve fitting, you can also set a maximum for this intrinsic scatter using the ``sigma_max`` keyword (default: 10). (For model fitting, you can set a maximum using the ``priors`` keyword.)
 
 Model Fitting
 -------------
-The :mod:`.models` and :mod:`.fitting` submodules allow you to fit analytical models to the observed data. Right now, the only choices are:
+The :mod:`.models` and :mod:`.fitting` submodules allow you to fit analytical models to the observed data.
+Right now, there are two classes of models: :class:`.BaseCompanionShocking`, which is the SiFTO Type Ia supernova template [C08]_ plus a shock component from [K10]_, and :class:`.BaseShockCooling`, which is the [SW17]_ model for shock cooling in a core-collapse supernova.
+The variations on these classes are as follows:
 
- * :class:`.CompanionShocking`, which is the SiFTO Type Ia supernova template [C08]_ plus a shock component from [K10]_, with factors on the r and i SiFTO models and a factor on the U shock component.
+ * :class:`.CompanionShocking` uses factors on the r and i SiFTO models and a factor on the U shock component.
    This was used in my paper on SN 2017cbv [H17]_.
- * :class:`.CompanionShocking2`, which is the same SiFTO Type Ia supernova template [C08]_ plus a shock component [K10]_, but with time offsets for the U and i SiFTO models instead of the three multiplicative factors.
+ * :class:`.CompanionShocking2` uses time offsets for the U and i SiFTO models.
    This was used in my paper on SN 2021aefx [H22a]_.
- * :data:`.ShockCooling`, which is the [SW17]_ model for shock cooling in a core-collapse supernova,
-   formulated in terms of :math:`v_s, M_\mathrm{env}, f_ρ M, R`.
- * :data:`.ShockCooling2`, which is the same [SW17]_ model but formulated in terms of scaling parameters :math:`T_1, L_1, t_\mathrm{tr}`.
+ * :class:`.CompanionShocking3` is the same as :class:`.CompanionShocking2` but includes viewing angle dependence.
+ * :class:`.ShockCooling` is formulated in terms of physical parameters :math:`v_s, M_\mathrm{env}, f_ρ M, R`.
+ * :class:`.ShockCooling2` is formulated in terms of scaling parameters :math:`T_1, L_1, t_\mathrm{tr}`.
    This was used in my paper on SN 2016bkv [H18]_.
- * :data:`.ShockCooling3`, which is the same as :data:`.ShockCooling` but with :math:`d_L` and :math:`E(B-V)` as free parameters. (Therefore it fits the flux instead of the luminosity.) This was used in my paper on SN 2021yja [H22b]_.
+ * :class:`.ShockCooling3` is the same as :class:`.ShockCooling` but with :math:`d_L` and :math:`E(B-V)` as free parameters. (Therefore it fits the flux instead of the luminosity.) This was used in my paper on SN 2021yja [H22b]_.
 
 **Note on the shock cooling models:**
 There are degeneracies between many of the physical parameters that make them difficult to fit independently.
 This led us to fit develop the :data:`.ShockCooling2` model just to see if the model could fit the data at all.
 Since it did not fit well, we concluded that the physical parameters we could have obtained by fitting the :data:`.ShockCooling` model were irrelevant.
 However, in order to measure, for example, the progenitor radius, one must use the :data:`.ShockCooling` model.
 
@@ -170,37 +175,47 @@
         UniformPrior(0., 100.),
         UniformPrior(0., 100.),
         UniformPrior(57468., 57468.7),
     ]
     p_lo = [20., 2., 20., 57468.5]
     p_up = [50., 5., 50., 57468.7]
 
-    redshift = 0.002
+    # Initialize the model
+    model = ShockCooling2(lc_early)
 
-    sampler = fitting.lightcurve_mcmc(lc_early, ShockCooling2, model_kwargs={'z': redshift},
-                                      priors=priors, p_lo=p_lo, p_up=p_up,
-                                      nwalkers=10, nsteps=100, nsteps_burnin=100, show=True)
-    lightcurve_corner(lc_early, ShockCooling2, sampler.flatchain, model_kwargs={'z': redshift})
+    # Run the fit
+    sampler = lightcurve_mcmc(lc_early, model, priors=priors, p_lo=p_lo, p_up=p_up,
+                              nwalkers=10, nsteps=100, nsteps_burnin=100, show=True)
+
+    # Plot the results
+    fig, ax_corner, ax_model = lightcurve_corner(lc_early, model, sampler.flatchain)
 
 **Another note on the shock cooling models:**
 The shock cooling models are only valid for temperatures above 0.7 eV = 8120 K [SW17]_,
 so you should check that you have not included observations where the model goes below that.
 If you have, you should rerun the fit without those points.
 If you used the [RW11]_ option, the model fails even earlier, but you will have to check that manually.
 
 .. code-block:: python
 
     p_mean = sampler.flatchain.mean(axis=0)
-    t_max = ShockCooling2.t_max(p_mean)
+    t_max = model.t_max(p_mean)
     print(t_max)
     if lc_early['MJD'].max() > t_max:
         print('Warning: your model is not valid for all your observations')
 
 Note that you can add an :ref:`Intrinsic Scatter` to your model fits as well.
 
+Defining New Models (Advanced)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+If you want to define a new model, all you need to do is subclass the :class:`.Model` class.
+Implement the model in the :meth:`.Model.evaluate` method, which takes an array of times and an array of filters as the first two arguments, followed by the physical parameters of the model.
+If there are keyword arguments (parameters that are *not* fit for) that need to be specified, you may have to override the :meth:`.Model.__init__` method.
+You must also provide ``input_names`` and ``units`` as class variables.
+
 Calibrating Spectra to Photometry
 ---------------------------------
 The :mod:`.speccal` module (somewhat experimental right now) can be used to calibrate spectra to observed photometry.
 
 .. code-block:: python
 
     from lightcurve_fitting.speccal import calibrate_spectra
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/bolometric.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/bolometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from .filters import all_filters, filtdict, extinction_law
+from .filters import filtdict, extinction_law
 from .models import planck_fast, UniformPrior, LogUniformPrior, GaussianPrior
 from .lightcurve import LC
 
 from astropy import constants as const
 from astropy import units as u
 
 import numpy as np
 import matplotlib.pyplot as plt
-from matplotlib.ticker import AutoLocator
 from scipy.optimize import curve_fit, OptimizeWarning
 from scipy.stats import gaussian_kde
 import emcee
 import corner
 import os
 from pkg_resources import resource_filename
 import warnings
 
-for filt in all_filters:
-    filt.read_curve()
-
 plt.style.use(resource_filename('lightcurve_fitting', 'serif.mplstyle'))
 
 
 def pseudo(temp, radius, z, filter0=filtdict['I'], filter1=filtdict['U'], cutoff_freq=np.inf):
     """
     Integrate a blackbody spectrum between two broadband filters to produce a pseudobolometric luminosity
 
@@ -582,17 +578,17 @@
                          save_chains=False, use_sigma=False, sigma_type='relative', also_group_by=()):
     """
     Calculate the full bolometric light curve from a table of broadband photometry
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
-        Table of broadband photometry including columns "MJD", "mag", "dmag", "filt"
+        Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
     z : float, optional
-        Redshift between the emission source and the observed filter. Default: 0.
+        DEPRECATED: Include the redshift in `lc.meta['redshift']` instead.
     outpath : str, optional
         Directory to which to save the corner plots and MCMC chains. Default: current directory
     res : float, optional
         Approximate resolution for grouping, in days. Default: 1 day.
     nwalkers : int, optional
         Number of walkers (chains) to use for fitting. Default: 10
     burnin_steps : int, optional
@@ -627,14 +623,17 @@
         Group by these columns in addition to epoch
 
     Returns
     -------
     t0 : lightcurve_fitting.lightcurve.LC
         Table containing the blackbody parameters, bolometric luminosities, and (optionally) colors
     """
+    if z:
+        warnings.warn('The z keyword is deprecated. Include the reshift in `lc.meta["redshift"]` instead.')
+    z = lc.meta.get('redshift', z)
 
     if colors is None:
         colors = []
 
     use_src = 'source' in lc.colnames
     t0 = LC(names=['MJD', 'dMJD0', 'dMJD1',
                    'temp', 'radius', 'dtemp', 'dradius',  # best fit from scipy.curve_fit
@@ -655,15 +654,14 @@
         priors = [UniformPrior(1., 100.), LogUniformPrior(0.01, 1000.)]
         if use_sigma:
             priors.append(GaussianPrior(0., 10.))
 
     sampler = None
     lc = lc[np.isfinite(lc['dmag']) & (lc['dmag'] > 0.)]
     for epoch1 in group_by_epoch(lc, res, also_group_by):
-        epoch1.sn = lc.sn
         epoch1.calcFlux()
         epoch1 = epoch1.bin(delta=np.inf)
         epoch1.calcMag()
         epoch1.calcAbsMag()
         epoch1.calcLum()
 
         epoch1['freq'] = u.Quantity([f.freq_eff for f in epoch1['filter']])
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/example/SN2016bkv.txt` & `lightcurve-fitting-0.8.0/lightcurve_fitting/example/SN2016bkv.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,760 +1,760 @@
-         MJD     mag   dmag filt      source nondet
------------- ------- ------ ---- ----------- ------
-   57468.703   17.53   0.16    0     Itagaki  False
-   57469.627   16.87   0.11    0     Itagaki  False
-  57470.3372 14.9383  0.012    U Las Cumbres  False
-  57470.3423 14.9143 0.0119    U Las Cumbres  False
-  57470.3476 16.0306 0.0373    B Las Cumbres  False
-  57470.3504 16.0132 0.0378    B Las Cumbres  False
-  57470.3534 15.9702 0.0362    V Las Cumbres  False
-  57470.3553 15.9877 0.0369    V Las Cumbres  False
-  57470.3574 15.8015 0.1125    g Las Cumbres  False
-  57470.3602 15.8182 0.1123    g Las Cumbres  False
-  57470.3633  16.116 0.0495    r Las Cumbres  False
-  57470.3652 16.0548  0.049    r Las Cumbres  False
-  57470.3673 16.3185 0.0635    i Las Cumbres  False
-  57470.3691 16.4189 0.0661    i Las Cumbres  False
-   57470.596   15.75   0.04    0     Itagaki  False
-57470.633579  15.689  0.013    V         TNT  False
-57470.633579  15.726  0.022    R         TNT  False
-57470.633579  15.735   0.02    I         TNT  False
-57470.633579  15.745  0.023    B         TNT  False
-   57471.423   15.34   0.03    0     Itagaki  False
-   57471.484   15.45   0.02    0     Itagaki  False
- 57471.60544  15.346  0.024    R         TNT  False
- 57471.60544  15.304  0.012    V         TNT  False
- 57471.60544  15.179  0.015    B         TNT  False
- 57471.60544  15.378  0.018    I         TNT  False
-  57472.0954 13.9765  0.014    U Las Cumbres  False
-  57472.0994 13.9698 0.0141    U Las Cumbres  False
-  57472.1037 15.0841 0.0246    B Las Cumbres  False
-  57472.1056 15.0806 0.0246    B Las Cumbres  False
-  57472.1076 15.2876 0.0161    V Las Cumbres  False
-  57472.1092 15.2664 0.0161    V Las Cumbres  False
-  57472.1179 13.9737 0.0169    U Las Cumbres  False
-  57472.1218 14.0148 0.0172    U Las Cumbres  False
-   57472.126 15.1316 0.0248    B Las Cumbres  False
-  57472.1278 15.1107 0.0248    B Las Cumbres  False
-  57472.1299 15.2811 0.0171    V Las Cumbres  False
-  57472.1314 15.2747 0.0171    V Las Cumbres  False
-  57472.1331 14.9552 0.1093    g Las Cumbres  False
-   57472.135 14.9651 0.1093    g Las Cumbres  False
-  57472.1371 15.3823 0.0296    r Las Cumbres  False
-  57472.1386 15.3536 0.0296    r Las Cumbres  False
-  57472.1403 15.5671 0.0407    i Las Cumbres  False
-  57472.1419 15.7132 0.0411    i Las Cumbres  False
-  57472.1451 14.0307 0.0198    U Las Cumbres  False
-  57472.1509 14.0526 0.0205    U Las Cumbres  False
-  57472.1549 14.0547 0.0199    U Las Cumbres  False
-   57472.159 15.1155 0.0248    B Las Cumbres  False
-  57472.1608 15.1021 0.0248    B Las Cumbres  False
-   57472.163 15.2592 0.0171    V Las Cumbres  False
-  57472.1645 15.2945 0.0166    V Las Cumbres  False
-  57472.1664 14.9396 0.1093    g Las Cumbres  False
-  57472.1683 14.9601 0.1093    g Las Cumbres  False
-  57472.1704 15.3706 0.0296    r Las Cumbres  False
-  57472.1719 15.3817 0.0296    r Las Cumbres  False
-  57472.1736 15.6175 0.0411    i Las Cumbres  False
-  57472.1751 15.5746 0.0407    i Las Cumbres  False
-  57472.1781 14.0458 0.0148    U Las Cumbres  False
-  57472.1837 14.0976 0.0246    U Las Cumbres  False
-  57472.1877 14.0827 0.0192    U Las Cumbres  False
-  57472.1942 14.0238 0.0162    U Las Cumbres  False
-  57472.1982 14.0354 0.0186    U Las Cumbres  False
-  57472.2024 15.0924 0.0248    B Las Cumbres  False
-  57472.2065 15.2437 0.0166    V Las Cumbres  False
-   57472.208 15.2757 0.0166    V Las Cumbres  False
-  57472.2098 14.9417 0.1092    g Las Cumbres  False
-  57472.2116 14.9297 0.1092    g Las Cumbres  False
-  57472.2137 15.3567 0.0296    r Las Cumbres  False
-  57472.2152 15.3116 0.0293    r Las Cumbres  False
-   57472.217 15.5654 0.0407    i Las Cumbres  False
-  57472.2185 15.5834 0.0411    i Las Cumbres  False
-    57472.42   15.17   0.02    0     Itagaki  False
-  57473.2103 13.8475 0.0074    U Las Cumbres  False
-  57473.2143 13.8502 0.0075    U Las Cumbres  False
-  57473.2184 14.9265 0.0246    B Las Cumbres  False
-  57473.2203 14.9224 0.0246    B Las Cumbres  False
-  57473.2225 15.0945 0.0156    V Las Cumbres  False
-   57473.224 15.0954 0.0156    V Las Cumbres  False
-  57473.2257 14.7559 0.1092    g Las Cumbres  False
-  57473.2276 14.7557 0.1092    g Las Cumbres  False
-  57473.2354 13.8383 0.0086    U Las Cumbres  False
-  57473.2397 14.8866 0.0246    B Las Cumbres  False
-  57473.2436 15.0923  0.016    V Las Cumbres  False
-  57473.2451  15.101  0.016    V Las Cumbres  False
-  57473.2469 14.7595 0.1092    g Las Cumbres  False
-  57473.2488 14.7791 0.1092    g Las Cumbres  False
-  57473.2508 15.1653 0.0289    r Las Cumbres  False
-  57473.2524 15.3521 0.0291    r Las Cumbres  False
-  57473.2541 15.5449 0.0401    i Las Cumbres  False
-  57473.2556 15.5238 0.0401    i Las Cumbres  False
-  57473.2651 13.8145 0.0085    U Las Cumbres  False
-  57473.2691 13.8089 0.0086    U Las Cumbres  False
-  57473.2734 14.8989 0.0246    B Las Cumbres  False
-  57473.2753 14.9021 0.0246    B Las Cumbres  False
-  57473.2773 15.0927  0.016    V Las Cumbres  False
-  57473.2788 15.0752  0.016    V Las Cumbres  False
-  57473.2807 14.7366 0.1092    g Las Cumbres  False
-  57473.2826 14.7288 0.1092    g Las Cumbres  False
-  57473.2846 15.1865 0.0291    r Las Cumbres  False
-  57473.2861 15.1721 0.0289    r Las Cumbres  False
-  57473.2878 15.4708 0.0401    i Las Cumbres  False
-  57473.2893 15.4026 0.0397    i Las Cumbres  False
-  57473.2978 13.7532 0.0089    U Las Cumbres  False
-  57473.3018  13.791 0.0097    U Las Cumbres  False
-  57473.3059  14.865 0.0246    B Las Cumbres  False
-  57473.3078 14.8646 0.0247    B Las Cumbres  False
-  57473.3098 15.0766  0.016    V Las Cumbres  False
-  57473.3114 15.0608  0.016    V Las Cumbres  False
-  57473.3132 14.7124 0.1092    g Las Cumbres  False
-  57473.3151  14.711 0.1092    g Las Cumbres  False
-  57473.3171 15.1418 0.0289    r Las Cumbres  False
-  57473.3187 15.1652 0.0291    r Las Cumbres  False
-  57473.3204 15.4497 0.0401    i Las Cumbres  False
-   57473.322 15.4474 0.0401    i Las Cumbres  False
-57476.575918  14.783  0.014    I         TNT  False
-57476.575918  14.775  0.021    R         TNT  False
-57476.575918  14.761  0.014    V         TNT  False
-57476.575918  14.834  0.014    B         TNT  False
-57477.593588  14.865  0.011    V         TNT  False
-57477.593588   14.89  0.022    R         TNT  False
-57477.593588  14.964  0.013    B         TNT  False
-57477.593588  14.865  0.016    I         TNT  False
-57477.593588   13.35  0.264    U         TNT  False
-57481.643748  15.188  0.024    R         TNT  False
-57481.643748  15.096  0.016    I         TNT  False
-57481.643748  15.226  0.012    V         TNT  False
-57481.643748  15.427  0.016    B         TNT  False
-57481.643748  13.744  0.263    U         TNT  False
-  57482.1006 14.5399 0.0116    U Las Cumbres  False
-  57482.1034 14.4856 0.0112    U Las Cumbres  False
-  57482.1064 15.4371 0.0256    B Las Cumbres  False
-  57482.1079 15.4248 0.0256    B Las Cumbres  False
-  57482.1096 15.3246 0.0176    V Las Cumbres  False
-57482.645295    15.3  0.012    V         TNT  False
-57482.645295  15.511  0.016    B         TNT  False
-57482.645295  15.221  0.026    R         TNT  False
-57482.645295  15.126  0.016    I         TNT  False
-57482.645295  14.203  0.254    U         TNT  False
-  57483.3497 14.6901 0.0141    U Las Cumbres  False
-  57483.3524 14.7305  0.015    U Las Cumbres  False
-  57483.3554 15.3658 0.0258    B Las Cumbres  False
-  57483.3569 15.3485 0.0258    B Las Cumbres  False
-  57483.3586 15.2849 0.0178    V Las Cumbres  False
-  57483.3598 15.3422 0.0178    V Las Cumbres  False
-  57483.3612 15.1809 0.1094    g Las Cumbres  False
-  57483.3628 15.1828 0.1094    g Las Cumbres  False
-  57483.3645  15.373 0.0316    r Las Cumbres  False
-  57483.3657 15.3807 0.0316    r Las Cumbres  False
-   57483.367 15.5451 0.0428    i Las Cumbres  False
-  57483.3682 15.5785 0.0432    i Las Cumbres  False
-  57487.1033 15.0075 0.0118    U Las Cumbres  False
-  57487.1061 14.9903 0.0118    U Las Cumbres  False
-  57489.2466 15.1748 0.0109    U Las Cumbres  False
-  57489.2493 15.1471   0.01    U Las Cumbres  False
-  57489.2523 15.9063 0.0269    B Las Cumbres  False
-  57489.2538 15.9053 0.0266    B Las Cumbres  False
-  57489.2556 15.6455 0.0194    V Las Cumbres  False
-  57489.2569 15.6609 0.0194    V Las Cumbres  False
-  57489.2582 15.6253 0.1095    g Las Cumbres  False
-  57489.2597 15.6073 0.1095    g Las Cumbres  False
-  57489.2614 15.6425 0.0322    r Las Cumbres  False
-  57489.2626 15.6172 0.0322    r Las Cumbres  False
-  57489.2639 15.7431 0.0434    i Las Cumbres  False
-  57489.2651 15.7289 0.0434    i Las Cumbres  False
-  57490.1527  15.251 0.0118    U Las Cumbres  False
-  57490.1555 15.2541 0.0116    U Las Cumbres  False
-  57490.1584 16.0249 0.0271    B Las Cumbres  False
-  57490.1599 16.0029 0.0271    B Las Cumbres  False
-  57490.1616 15.7059 0.0203    V Las Cumbres  False
-  57490.1628 15.7009 0.0203    V Las Cumbres  False
-  57490.1641 15.7022 0.1096    g Las Cumbres  False
-  57490.1656 15.7091 0.1096    g Las Cumbres  False
-  57490.1673 15.6717 0.0331    r Las Cumbres  False
-  57490.1685 15.6957 0.0334    r Las Cumbres  False
-  57490.1698 15.7308 0.0443    i Las Cumbres  False
-  57490.1709 15.8258 0.0448    i Las Cumbres  False
-  57491.2782  15.344 0.0148    U Las Cumbres  False
-   57491.281 15.3738 0.0145    U Las Cumbres  False
-  57491.2855 15.9779 0.0279    B Las Cumbres  False
-  57491.2872  15.648 0.0219    V Las Cumbres  False
-  57491.2883 15.7342 0.0219    V Las Cumbres  False
-  57491.2897 15.6847 0.1097    g Las Cumbres  False
-  57491.2912 15.7002 0.1098    g Las Cumbres  False
-  57491.2928 15.6685 0.0338    r Las Cumbres  False
-   57491.294 15.6609 0.0338    r Las Cumbres  False
-  57491.2953 15.7567 0.0451    i Las Cumbres  False
-  57491.2965 15.7024 0.0456    i Las Cumbres  False
-57491.578365  15.369  0.019    I         TNT  False
-57491.578365  16.031  0.017    B         TNT  False
-57491.578365  15.501  0.023    R         TNT  False
-57491.578365   15.05  0.297    U         TNT  False
-57491.578365  15.658  0.015    V         TNT  False
-   57492.243 15.4876 0.0136    U Las Cumbres  False
-  57492.2457 15.4021 0.0129    U Las Cumbres  False
-  57492.2487 16.0975 0.0292    B Las Cumbres  False
-  57492.2502 16.1095 0.0292    B Las Cumbres  False
-  57492.2518 15.7298 0.0228    V Las Cumbres  False
-   57492.253 15.7393 0.0234    V Las Cumbres  False
-  57492.2544 15.7825   0.11    g Las Cumbres  False
-  57492.2559 15.7635   0.11    g Las Cumbres  False
-  57492.2575 15.7023 0.0346    r Las Cumbres  False
-  57492.2587 15.7249 0.0349    r Las Cumbres  False
-    57492.26 15.8382 0.0459    i Las Cumbres  False
-  57492.2612  15.864 0.0459    i Las Cumbres  False
-  57494.2802 15.6466 0.0159    U Las Cumbres  False
-   57494.283 15.6557 0.0174    U Las Cumbres  False
-  57494.2859 16.1629  0.036    B Las Cumbres  False
-  57494.2875 16.1811 0.0365    B Las Cumbres  False
-  57494.2891 15.7704 0.0303    V Las Cumbres  False
-  57494.2903 15.7524 0.0297    V Las Cumbres  False
-  57494.2916 15.8363 0.1112    g Las Cumbres  False
-  57494.2931 15.8175 0.1112    g Las Cumbres  False
-  57494.2948 15.7117 0.0397    r Las Cumbres  False
-   57494.296  15.731 0.0397    r Las Cumbres  False
-  57494.2973 15.8523 0.0505    i Las Cumbres  False
-  57494.2984  15.805 0.0505    i Las Cumbres  False
-57494.627855  16.174  0.022    B         TNT  False
-57494.627855  15.542  0.025    R         TNT  False
-57494.627855  15.434  0.023    I         TNT  False
-57494.627855  15.755  0.014    V         TNT  False
-  57496.2915 15.7822 0.0463    U Las Cumbres  False
-  57496.2943 15.8017 0.0403    U Las Cumbres  False
-  57496.2972 16.5733  0.054    B Las Cumbres  False
-  57496.2987   16.52 0.0564    B Las Cumbres  False
-  57496.3016 15.9073  0.051    V Las Cumbres  False
-  57496.3086 15.9384 0.0517    i Las Cumbres  False
-  57498.2186 16.0172 0.0295    U Las Cumbres  False
-  57498.2214 15.9732 0.0243    U Las Cumbres  False
-  57498.2243 16.4274 0.0462    B Las Cumbres  False
-  57498.2258 16.4265  0.045    B Las Cumbres  False
-  57498.2275 15.9785 0.0406    V Las Cumbres  False
-  57498.2287  15.874 0.0392    V Las Cumbres  False
-    57498.23 16.0364 0.1127    g Las Cumbres  False
-  57498.2315 16.0326 0.1128    g Las Cumbres  False
-  57498.2333  15.798  0.043    r Las Cumbres  False
-  57498.2345 15.8217 0.0434    r Las Cumbres  False
-  57498.2358 15.8616 0.0551    i Las Cumbres  False
-   57498.237 15.8664 0.0551    i Las Cumbres  False
-57498.625483  15.823  0.012    V         TNT  False
-57498.625483   15.44  0.021    I         TNT  False
-57498.625483  15.646  0.028    R         TNT  False
-57498.625483   16.44  0.024    B         TNT  False
-  57500.1844 16.1327 0.0298    U Las Cumbres  False
-  57500.1872 16.0613 0.0294    U Las Cumbres  False
-  57500.1902 16.5307  0.058    B Las Cumbres  False
-  57500.1917 16.5291 0.0559    B Las Cumbres  False
-  57500.1934  15.931 0.0478    V Las Cumbres  False
-  57500.1946 15.9987 0.0484    V Las Cumbres  False
-   57500.196 16.1066  0.115    g Las Cumbres  False
-  57500.1975   16.09 0.1146    g Las Cumbres  False
-  57500.1993 15.8489 0.0502    r Las Cumbres  False
-  57500.2004 15.8787 0.0512    r Las Cumbres  False
-  57500.2017 15.9051 0.0602    i Las Cumbres  False
-  57500.2029  15.949 0.0748    i Las Cumbres  False
-57500.618378  15.441  0.021    I         TNT  False
-57500.618378  16.503  0.033    B         TNT  False
-57500.618378  15.858  0.016    V         TNT  False
-57500.618378  15.634  0.025    R         TNT  False
-57501.620423  15.869  0.013    V         TNT  False
-57501.620423  15.414  0.017    I         TNT  False
-57501.620423  16.491  0.018    B         TNT  False
-57501.620423  15.635  0.026    R         TNT  False
-57501.620423  17.168  0.375    U         TNT  False
-  57502.1117  16.402 0.0339    U Las Cumbres  False
-  57502.1146    16.4 0.0397    U Las Cumbres  False
-  57502.1175 16.5647 0.0451    B Las Cumbres  False
-   57502.119 16.5748 0.0451    B Las Cumbres  False
-  57502.1207 15.9322 0.0395    V Las Cumbres  False
-  57503.1979 16.4077 0.0239    U Las Cumbres  False
-  57503.2007 16.3992 0.0245    U Las Cumbres  False
-  57503.2036 16.5655 0.0368    B Las Cumbres  False
-  57503.2051 16.6427 0.0379    B Las Cumbres  False
-  57503.2068 15.9645   0.03    V Las Cumbres  False
-   57503.208   15.99   0.03    V Las Cumbres  False
-  57503.2093 16.1823 0.1109    g Las Cumbres  False
-  57503.2108 16.1746 0.1109    g Las Cumbres  False
-  57503.2125 15.8838 0.0372    r Las Cumbres  False
-  57503.2137 15.8595 0.0368    r Las Cumbres  False
-  57503.2151  15.889  0.049    i Las Cumbres  False
-  57503.2162 15.8288 0.0485    i Las Cumbres  False
-  57504.1843 16.5057 0.0238    U Las Cumbres  False
-  57504.1872  16.521  0.028    U Las Cumbres  False
-  57504.1902 16.6124 0.0344    B Las Cumbres  False
-  57504.1917 16.6207 0.0338    B Las Cumbres  False
-  57504.1934 15.9988 0.0271    V Las Cumbres  False
-  57504.1946 15.9485 0.0271    V Las Cumbres  False
-  57504.1961 16.2135 0.1104    g Las Cumbres  False
-  57504.1977 16.2148 0.1106    g Las Cumbres  False
-  57504.1995 15.8648 0.0369    r Las Cumbres  False
-  57504.2008 15.9055 0.0369    r Las Cumbres  False
-  57504.2021 15.9256 0.0496    i Las Cumbres  False
-  57504.2033 15.8654 0.0485    i Las Cumbres  False
-  57505.2678  16.498 0.0333    U Las Cumbres  False
-  57505.2708 16.5583 0.0378    U Las Cumbres  False
-  57505.2739  16.574 0.0416    B Las Cumbres  False
-  57505.2754 16.6056 0.0429    B Las Cumbres  False
-  57505.2771 15.9298 0.0336    V Las Cumbres  False
-  57505.2783 15.9216 0.0336    V Las Cumbres  False
-  57505.2798 16.1891 0.1115    g Las Cumbres  False
-  57505.2814 16.1606 0.1115    g Las Cumbres  False
-  57505.2838 15.8836 0.0435    r Las Cumbres  False
-  57505.2851 15.8416 0.0435    r Las Cumbres  False
-  57505.2865 15.9387 0.0547    i Las Cumbres  False
-  57506.2537 16.7218 0.0252    U Las Cumbres  False
-  57506.2565 16.6866 0.0253    U Las Cumbres  False
-  57506.2595 16.6303 0.0334    B Las Cumbres  False
-   57506.261 16.6623 0.0334    B Las Cumbres  False
-  57506.2627  15.938 0.0253    V Las Cumbres  False
-  57506.2638  15.984 0.0259    V Las Cumbres  False
-  57506.2652 16.1868 0.1103    g Las Cumbres  False
-  57506.2667 16.1829 0.1103    g Las Cumbres  False
-  57506.2684 15.8172 0.0355    r Las Cumbres  False
-  57506.2695 15.8294 0.0355    r Las Cumbres  False
-  57506.2709 15.8158 0.0468    i Las Cumbres  False
-  57506.2721 15.7944 0.0473    i Las Cumbres  False
-  57508.1076 16.7838 0.0583    U Las Cumbres  False
-  57508.1106 16.7567 0.0406    B Las Cumbres  False
-  57508.1121 16.8007 0.0381    B Las Cumbres  False
-  57508.1138 16.0219 0.0285    V Las Cumbres  False
-  57508.1149 16.0689 0.0285    V Las Cumbres  False
-  57508.1163 16.3285 0.1108    g Las Cumbres  False
-  57508.1178 16.3504  0.111    g Las Cumbres  False
-  57508.1195 15.7281 0.0529    r Las Cumbres  False
-  57508.1206 15.8821 0.0355    r Las Cumbres  False
-   57508.122 15.8901 0.0466    i Las Cumbres  False
-  57508.1231  15.863  0.047    i Las Cumbres  False
-  57512.2401 16.8905 0.0377    U Las Cumbres  False
-  57512.2429 16.9686 0.0407    U Las Cumbres  False
-  57512.2458 16.8504 0.0369    B Las Cumbres  False
-  57512.2473 16.8123 0.0374    B Las Cumbres  False
-   57512.249   15.97 0.0276    V Las Cumbres  False
-  57512.2502 15.9749 0.0276    V Las Cumbres  False
-  57512.2516 16.3494 0.1106    g Las Cumbres  False
-  57512.2531 16.2754 0.1106    g Las Cumbres  False
-  57512.2548 15.7885 0.0352    r Las Cumbres  False
-   57512.256 15.7987 0.0355    r Las Cumbres  False
-  57512.2573 15.8455 0.0468    i Las Cumbres  False
-  57512.2585 15.8351 0.0478    i Las Cumbres  False
-57515.625795  16.935  0.034    B         TNT  False
-57515.625795  15.353  0.018    I         TNT  False
-57515.625795  15.926  0.013    V         TNT  False
-57515.625795  15.604  0.025    R         TNT  False
-  57517.1771 17.2135  0.042    U Las Cumbres  False
-    57517.18 17.2304 0.0503    U Las Cumbres  False
-  57517.1833 16.4835 0.0375    B Las Cumbres  False
-  57517.1848 16.5284  0.037    B Las Cumbres  False
-  57517.1865 16.0593 0.0278    V Las Cumbres  False
-  57517.1877 16.0567 0.0283    V Las Cumbres  False
-  57517.1891 16.4414 0.1106    g Las Cumbres  False
-  57517.1907 16.4913 0.1106    g Las Cumbres  False
-  57517.1924 15.8162 0.0345    r Las Cumbres  False
-  57517.1936 15.8108 0.0345    r Las Cumbres  False
-  57517.1949 15.7234 0.0453    i Las Cumbres  False
-  57517.1961 15.8121 0.0463    i Las Cumbres  False
-  57519.1194 17.3701 0.0514    U Las Cumbres  False
-  57519.1221 17.3135 0.0471    U Las Cumbres  False
-  57519.1251 17.1154 0.0386    B Las Cumbres  False
-  57519.1266 17.1389   0.04    B Las Cumbres  False
-  57519.1283 16.0316 0.0252    V Las Cumbres  False
-  57519.1295 16.0454 0.0257    V Las Cumbres  False
-  57519.1319 17.4122 0.0321    U Las Cumbres  False
-  57519.1346 17.2981 0.0361    U Las Cumbres  False
-  57519.1399 17.2792 0.0425    U Las Cumbres  False
-  57519.1427 17.5594 0.0606    U Las Cumbres  False
-  57519.1457 17.1332 0.0393    B Las Cumbres  False
-  57519.1472 17.1575   0.04    B Las Cumbres  False
-  57519.1489 16.0677 0.0257    V Las Cumbres  False
-  57519.1501 16.0503 0.0263    V Las Cumbres  False
-  57519.1516 16.5189 0.1104    g Las Cumbres  False
-  57519.1531 16.5103 0.1105    g Las Cumbres  False
-  57519.1548 15.8177 0.0334    r Las Cumbres  False
-  57519.1559 15.8014 0.0338    r Las Cumbres  False
-  57519.1573 15.7774 0.0439    i Las Cumbres  False
-  57519.1585 15.7843 0.0448    i Las Cumbres  False
-  57520.1233 17.5626 0.0748    U Las Cumbres  False
-  57520.1261 17.3713 0.0605    U Las Cumbres  False
-   57524.219 17.5308 0.1368    U Las Cumbres  False
-  57524.2218 17.8168 0.1503    U Las Cumbres  False
-  57524.2247 17.1324 0.0711    B Las Cumbres  False
-  57524.2263 17.0558 0.0682    B Las Cumbres  False
-   57524.228 16.0318 0.0521    V Las Cumbres  False
-  57524.2293 15.9815 0.0515    V Las Cumbres  False
-  57524.2322 16.5076 0.1188    g Las Cumbres  False
-   57524.235 15.7275 0.0509    r Las Cumbres  False
-  57524.2364 16.0481 0.0629    i Las Cumbres  False
-  57529.1401 17.8568 0.0535    U Las Cumbres  False
-  57529.1475 17.5866 0.0637    U Las Cumbres  False
-  57529.1551 17.2909 0.0899    B Las Cumbres  False
-  57529.1566 17.2987 0.0899    B Las Cumbres  False
-  57529.1582 16.1064 0.0614    V Las Cumbres  False
-  57529.1594 16.0538  0.061    V Las Cumbres  False
-  57529.1608 16.5989 0.1158    g Las Cumbres  False
-  57529.1623 16.6758 0.1163    g Las Cumbres  False
-   57529.164 15.8185 0.0393    r Las Cumbres  False
-  57529.1652 15.8071 0.0388    r Las Cumbres  False
-  57529.1666 15.7437 0.0496    i Las Cumbres  False
-  57529.1678 15.7215 0.0496    i Las Cumbres  False
-57540.545546  15.224  0.016    I         TNT  False
-57540.545546  18.715  0.314    U         TNT  False
-57540.545546  17.431  0.025    B         TNT  False
-57540.545546   16.07  0.014    V         TNT  False
-57540.545546  15.586  0.031    R         TNT  False
-  57556.1306 17.7635  0.117    B Las Cumbres  False
-  57556.1325 17.6177 0.0946    B Las Cumbres  False
-  57556.1346 16.1934 0.0549    V Las Cumbres  False
-  57556.1362 16.1709 0.0549    V Las Cumbres  False
-  57556.1379 16.9356 0.1147    g Las Cumbres  False
-  57556.1398 16.8479 0.1144    g Las Cumbres  False
-  57556.1419 15.7665 0.0343    r Las Cumbres  False
-  57556.1434 15.7323 0.0339    r Las Cumbres  False
-  57556.1502 17.9671  0.117    B Las Cumbres  False
-  57556.1521 17.8594 0.1082    B Las Cumbres  False
-  57556.1542 16.2084 0.0558    V Las Cumbres  False
-  57556.1558 16.1104 0.0549    V Las Cumbres  False
-  57556.1575 16.9335 0.1152    g Las Cumbres  False
-  57556.1594 16.8759 0.1152    g Las Cumbres  False
-  57556.1614 15.7605 0.0347    r Las Cumbres  False
-   57556.163 15.7489 0.0343    r Las Cumbres  False
-  57556.1647 15.6482 0.0437    i Las Cumbres  False
-  57556.1662 15.6344 0.0446    i Las Cumbres  False
-57557.535687  15.175  0.019    I         TNT  False
-57557.535687   17.58  0.031    B         TNT  False
-57557.535687  16.133  0.016    V         TNT  False
-57557.535687  15.576  0.028    R         TNT  False
-  57558.1365 17.6111 0.1539    B Las Cumbres  False
-  57558.1381 17.9324 0.1788    B Las Cumbres  False
-  57558.1398 16.2053 0.1045    V Las Cumbres  False
-  57558.1409 16.1249 0.1024    V Las Cumbres  False
-   57673.469 21.1534 0.8887    B Las Cumbres  False
-  57673.4718 19.8874 0.3658    B Las Cumbres  False
-  57673.4748 18.5588 0.3004    V Las Cumbres  False
-  57673.4766 18.8357 0.3172    V Las Cumbres  False
-  57673.4815 19.8136 0.3281    g Las Cumbres  False
-  57673.4845 17.8727 0.1103    r Las Cumbres  False
-  57673.4863 17.9603 0.1154    r Las Cumbres  False
-  57673.4883 17.5858 0.1324    i Las Cumbres  False
-  57673.4902 17.4805 0.1273    i Las Cumbres  False
-  57674.4813 18.6738 0.1776    V Las Cumbres  False
-  57674.4832 18.1513 0.2085    V Las Cumbres  False
-   57674.488    19.2  0.905    g Las Cumbres  False
-  57674.4926 17.5752 0.1454    r Las Cumbres  False
-  57674.4944 17.6976 0.1431    r Las Cumbres  False
-  57674.4964  17.667 0.1881    i Las Cumbres  False
-  57674.4983 17.8357 0.1858    i Las Cumbres  False
-  57679.4725  20.915 2.0742    B Las Cumbres  False
-  57679.4782 18.7554 1.4826    V Las Cumbres  False
-  57679.4801 18.1945 1.4697    V Las Cumbres  False
-  57679.4821 20.8627 1.1073    g Las Cumbres  False
-  57679.4849 21.4387 1.5362    g Las Cumbres  False
-  57679.4878 17.8407  0.149    r Las Cumbres  False
-  57679.4897 18.0179 0.1589    r Las Cumbres  False
-  57679.4917 17.7578 0.1712    i Las Cumbres  False
-  57679.4935 17.7364 0.1719    i Las Cumbres  False
-  57680.4541 20.8478 1.9707    B Las Cumbres  False
-   57680.458 22.4199 4.9667    B Las Cumbres  False
-  57680.4622 18.4156 1.4968    V Las Cumbres  False
-   57680.465 18.5194 1.4975    V Las Cumbres  False
-  57680.4679 19.1815 0.2785    g Las Cumbres  False
-  57680.4719  19.746 0.3341    g Las Cumbres  False
-   57680.476  18.119 0.1443    r Las Cumbres  False
-  57680.4788 18.0681 0.1418    r Las Cumbres  False
-  57680.4817 17.9673 0.1748    i Las Cumbres  False
-  57680.4845 17.8122 0.1673    i Las Cumbres  False
-  57688.4292 20.5924 0.4195    B Las Cumbres  False
-  57688.4332 20.2091 0.4099    B Las Cumbres  False
-  57688.4373 18.7214 0.2723    V Las Cumbres  False
-  57688.4401 18.7504 0.2774    V Las Cumbres  False
-  57688.4431 22.6568 2.2698    g Las Cumbres  False
-   57688.447 21.2946 1.0653    g Las Cumbres  False
-  57688.4511 18.4416  0.133    r Las Cumbres  False
-  57688.4539 18.5158 0.1392    r Las Cumbres  False
-  57688.4569 18.0088  0.154    i Las Cumbres  False
-  57688.4597 18.1888 0.1719    i Las Cumbres  False
-57696.906824  17.728  0.038    R         TNT  False
-57696.906824  18.598  0.039    V         TNT  False
-57696.906824  17.209  0.034    I         TNT  False
-  57699.4068 20.4431 0.3375    B Las Cumbres  False
-  57699.4108 19.5627 0.2289    B Las Cumbres  False
-  57699.4149 18.9921 0.2194    V Las Cumbres  False
-  57699.4177 17.8577 0.1834    V Las Cumbres  False
-  57699.4345 18.4145   0.19    i Las Cumbres  False
-57706.807542  17.867  0.053    R         TNT  False
-57706.807542  17.351  0.043    I         TNT  False
-  57707.3848 20.0002 0.7507    B Las Cumbres  False
-  57707.3887 19.1218  0.438    B Las Cumbres  False
-  57707.3929 19.2638 0.5016    V Las Cumbres  False
-  57707.3957 18.4894  0.385    V Las Cumbres  False
-  57707.3986 19.7339 0.4316    g Las Cumbres  False
-  57707.4026  18.844 0.2948    g Las Cumbres  False
-  57707.4067   18.02 0.1713    r Las Cumbres  False
-  57707.4094  18.382 0.1963    r Las Cumbres  False
-  57707.4124 17.9194 0.1914    i Las Cumbres  False
-  57707.4152 18.0853 0.2051    i Las Cumbres  False
-57708.768464  17.337  0.141    I         TNT  False
-57708.768464  18.074  0.201    R         TNT  False
-57714.825623  17.296  0.078    I         TNT  False
-    57715.49 20.8948 0.4886    B Las Cumbres  False
-  57715.4939 20.2211 0.3241    B Las Cumbres  False
-   57715.498 18.7717 0.2517    V Las Cumbres  False
-  57715.5008 18.7452   0.25    V Las Cumbres  False
-  57715.5038 19.9626  0.264    g Las Cumbres  False
-  57715.5078 19.9024 0.2598    g Las Cumbres  False
-  57715.5119 18.1421 0.1232    r Las Cumbres  False
-  57715.5147 18.1883 0.1259    r Las Cumbres  False
-  57715.5177 18.0163 0.1752    i Las Cumbres  False
-  57715.5204 17.8004 0.1569    i Las Cumbres  False
- 57715.90839  17.327   0.04    I         TNT  False
- 57715.90839  20.392    0.1    B         TNT  False
- 57715.90839  18.488  0.036    V         TNT  False
- 57715.90839  17.875  0.039    R         TNT  False
-57722.818443   18.53  0.049    V         TNT  False
-57722.818443  17.273  0.039    I         TNT  False
-57722.818443  17.883  0.042    R         TNT  False
-  57723.3684 22.8285 2.8164    B Las Cumbres  False
-  57723.3724 21.1664 0.9232    B Las Cumbres  False
-  57723.3765 18.7387 0.7082    V Las Cumbres  False
-  57723.3793 18.7662 0.7093    V Las Cumbres  False
-  57723.3823 20.1744 0.3124    g Las Cumbres  False
-  57723.3862 20.0576 0.2843    g Las Cumbres  False
-  57723.3904 18.4058 0.1547    r Las Cumbres  False
-  57723.3931 18.5471 0.1559    r Las Cumbres  False
-  57723.3961 18.3702 0.1978    i Las Cumbres  False
-  57723.3989 18.0438 0.1717    i Las Cumbres  False
-57723.675749  17.928  0.037    R         TNT  False
-57723.675749  20.237  0.099    B         TNT  False
-57723.675749  17.401  0.031    I         TNT  False
-57723.675749  18.666  0.038    V         TNT  False
-57727.787505    18.0  0.047    R         TNT  False
-57727.787505  18.639  0.038    V         TNT  False
-57727.787505    20.0   0.08    B         TNT  False
-57727.787505  17.471  0.033    I         TNT  False
-57728.907253  20.155  0.098    B         TNT  False
-57728.907253  18.657  0.043    V         TNT  False
-57728.907253  17.984  0.039    R         TNT  False
-57728.907253   17.41  0.039    I         TNT  False
-57730.896945  17.379  0.031    I         TNT  False
-57730.896945  18.008  0.049    R         TNT  False
-57730.896945  18.758  0.069    V         TNT  False
-57730.896945  20.206  0.113    B         TNT  False
-57731.793337  20.061  0.103    B         TNT  False
-57731.793337  17.521  0.043    I         TNT  False
-57731.793337  18.694  0.035    V         TNT  False
-57731.793337  17.941  0.037    R         TNT  False
-  57732.3233 21.6992 2.7869    B Las Cumbres  False
-  57732.3273  22.071 3.1274    B Las Cumbres  False
-  57732.3315 19.3308 1.7215    V Las Cumbres  False
-  57732.3342  18.833  1.713    V Las Cumbres  False
-  57732.3373 19.8076 0.3557    g Las Cumbres  False
-  57732.3413 19.4733 0.2982    g Las Cumbres  False
-  57732.3454 18.3222 0.1736    r Las Cumbres  False
-  57732.3482  18.284 0.1712    r Las Cumbres  False
-  57732.3512 18.1615 0.2176    i Las Cumbres  False
-   57732.354 18.1794   0.21    i Las Cumbres  False
-57732.781453  17.927   0.04    R         TNT  False
-57732.781453  18.634  0.039    V         TNT  False
-57732.781453  20.276  0.098    B         TNT  False
-57732.781453  17.428  0.036    I         TNT  False
-57736.832265  18.003  0.046    R         TNT  False
-57736.832265  18.763  0.061    V         TNT  False
-57736.832265  17.462  0.035    I         TNT  False
-57737.793884   18.66  0.076    V         TNT  False
-57737.793884   18.06  0.042    R         TNT  False
-57737.793884  17.536  0.047    I         TNT  False
-  57738.4594 21.0256 1.7417    B Las Cumbres  False
-  57738.4634  22.066 3.5607    B Las Cumbres  False
-  57738.4675 18.6401 1.2579    V Las Cumbres  False
-  57738.4703 19.0732 1.2727    V Las Cumbres  False
-  57738.4733 20.3567 0.6506    g Las Cumbres  False
-  57738.4772 19.6308 0.4061    g Las Cumbres  False
-  57738.4814  18.444 0.2041    r Las Cumbres  False
-  57738.4841  18.496 0.2001    r Las Cumbres  False
-  57738.4871 18.1265   0.22    i Las Cumbres  False
-  57738.4899 18.2485 0.2303    i Las Cumbres  False
-57739.871799  20.154  0.116    B         TNT  False
-57739.871799  18.505  0.035    V         TNT  False
-57739.871799  17.544  0.041    I         TNT  False
-57739.871799  18.023  0.038    R         TNT  False
- 57740.85571  17.633  0.054    I         TNT  False
- 57740.85571  18.669  0.051    V         TNT  False
- 57740.85571   20.19  0.095    B         TNT  False
- 57740.85571  18.059  0.039    R         TNT  False
-57741.903241  17.969  0.041    R         TNT  False
-57741.903241  20.004  0.081    B         TNT  False
-57741.903241   18.75  0.034    V         TNT  False
-57741.903241  17.584  0.038    I         TNT  False
-57744.810645  17.727  0.062    I         TNT  False
-57744.810645  18.062  0.052    R         TNT  False
-57744.810645  18.588  0.068    V         TNT  False
-57745.925413   17.51  0.034    I         TNT  False
-57745.925413  18.046  0.039    R         TNT  False
-57745.925413  18.718   0.05    V         TNT  False
-57745.925413  20.177  0.117    B         TNT  False
-    57746.49 22.3326 1.7927    B Las Cumbres  False
-  57746.4939 21.1568 0.8145    B Las Cumbres  False
-   57746.498 19.1673 0.6068    V Las Cumbres  False
-  57746.5008 19.0169 0.6057    V Las Cumbres  False
-  57746.5038 20.2377  0.286    g Las Cumbres  False
-  57746.5078 20.1206 0.2774    g Las Cumbres  False
-  57746.5119 18.9481   0.22    r Las Cumbres  False
-  57746.5147 19.1696 0.2331    r Las Cumbres  False
-  57746.5176 18.7021 0.2597    i Las Cumbres  False
-  57746.5204 18.8688 0.2939    i Las Cumbres  False
- 57748.82233   17.58  0.045    I         TNT  False
- 57748.82233  20.352  0.117    B         TNT  False
- 57748.82233  18.155  0.046    R         TNT  False
- 57748.82233  18.643  0.041    V         TNT  False
-57750.698686  20.156  0.098    B         TNT  False
-57750.698686  18.146  0.044    R         TNT  False
-57750.698686  17.546  0.045    I         TNT  False
-57750.698686  18.682  0.049    V         TNT  False
-57751.716248  17.542  0.036    I         TNT  False
-57751.716248  20.216  0.111    B         TNT  False
-57751.716248  18.131  0.045    R         TNT  False
-57751.716248  18.713  0.039    V         TNT  False
-57753.794307  18.731  0.035    V         TNT  False
-57753.794307  18.136  0.041    R         TNT  False
-57753.794307  19.945  0.083    B         TNT  False
-57753.794307  17.593  0.028    I         TNT  False
-  57754.3303 20.3375 0.3363    B Las Cumbres  False
-  57754.3343 20.3826 0.3324    B Las Cumbres  False
-  57754.3384 19.0015 0.2465    V Las Cumbres  False
-  57754.3412 18.9038 0.2432    V Las Cumbres  False
-  57754.3442 19.4622 0.2125    g Las Cumbres  False
-  57754.3482 19.4304 0.2277    g Las Cumbres  False
-  57754.3523 18.7175 0.2072    r Las Cumbres  False
-  57754.3551 18.8432 0.2161    r Las Cumbres  False
-  57754.3581  18.668 0.2808    i Las Cumbres  False
-  57754.3609 18.5053 0.2563    i Las Cumbres  False
-57754.864937   18.77  0.046    V         TNT  False
-57754.864937  17.538  0.034    I         TNT  False
-57754.864937   18.18  0.051    R         TNT  False
-57754.864937  20.174  0.097    B         TNT  False
-57755.704894  18.644  0.048    V         TNT  False
-57755.704894  17.595  0.051    I         TNT  False
-57755.704894  18.098  0.045    R         TNT  False
-  57757.4305 20.4754 0.3589    B Las Cumbres  False
-  57757.4344 20.5292 0.3951    B Las Cumbres  False
-  57757.4386 19.3142 0.9676    V Las Cumbres  False
-  57757.4414  18.755 0.3024    V Las Cumbres  False
-  57757.4444 19.7011 0.3106    g Las Cumbres  False
-57757.783408  17.786  0.069    I         TNT  False
-57757.783408  18.222  0.046    R         TNT  False
-57757.783408  18.877  0.044    V         TNT  False
-57757.783408  20.442  0.174    B         TNT  False
-  57758.3641  20.155 0.3232    B Las Cumbres  False
-  57758.3681 21.7585  0.961    B Las Cumbres  False
-  57758.3722 19.2541 0.3004    V Las Cumbres  False
-   57758.375 19.2438 0.2993    V Las Cumbres  False
-   57758.378 19.7486 0.2316    g Las Cumbres  False
-  57758.3819 19.6856 0.2355    g Las Cumbres  False
-  57758.3861 18.6252 0.1488    r Las Cumbres  False
-  57758.3888 18.6595 0.1558    r Las Cumbres  False
-  57758.3918 18.2208 0.1958    i Las Cumbres  False
-  57758.3946  18.302 0.1958    i Las Cumbres  False
-  57758.4094  21.255 0.6251    B Las Cumbres  False
-  57758.4133 22.1673 1.3297    B Las Cumbres  False
-  57758.4175 19.3989 0.3109    V Las Cumbres  False
-  57758.4203 19.3459 0.3115    V Las Cumbres  False
-  57758.4314 18.6353 0.1508    r Las Cumbres  False
-  57758.4342 18.6552 0.1558    r Las Cumbres  False
-  57758.4372 18.4895   0.23    i Las Cumbres  False
-    57758.44 18.5385 0.2265    i Las Cumbres  False
-57758.883741  17.696  0.057    I         TNT  False
-57758.883741  18.228  0.049    R         TNT  False
-57758.883741  20.324  0.116    B         TNT  False
-57758.883741  18.911  0.039    V         TNT  False
-57762.655904  17.679  0.051    I         TNT  False
-57762.655904  18.701  0.095    V         TNT  False
-57762.655904  18.333  0.053    R         TNT  False
-57775.590604  17.731   0.07    I         TNT  False
-57775.590604  18.444  0.075    R         TNT  False
-57775.590604  18.801  0.093    V         TNT  False
-  57782.4936 21.9845 1.3972    B Las Cumbres  False
-  57782.4975 21.2106 0.7839    B Las Cumbres  False
-  57782.5017 19.5279 0.5987    V Las Cumbres  False
-  57782.5045 19.7124 0.6139    V Las Cumbres  False
-  57782.5076 21.2163 0.8647    g Las Cumbres  False
-  57782.5157 19.0507 0.2759    r Las Cumbres  False
-  57782.5215 18.5641   0.31    i Las Cumbres  False
-  57782.5243 18.9661 0.3722    i Las Cumbres  False
-57797.531826  18.831  0.068    R         TNT  False
-57797.531826  18.373  0.069    I         TNT  False
-57800.630929  18.383  0.076    I         TNT  False
-57800.630929  18.847  0.087    R         TNT  False
-  57801.3635 22.4579 2.2635    B Las Cumbres  False
-  57801.3686 21.3339 1.0451    B Las Cumbres  False
-  57801.3739 20.0618 0.8374    V Las Cumbres  False
-  57801.3779 19.7686 0.8133    V Las Cumbres  False
-   57801.382 22.7567 3.0849    g Las Cumbres  False
-  57801.3871 21.0674 0.6138    g Las Cumbres  False
-  57801.4044 19.4755 0.4514    i Las Cumbres  False
-57803.737585  18.196  0.081    I         TNT  False
-57803.737585  18.988  0.109    R         TNT  False
-  57807.4016 20.6804 0.4934    B Las Cumbres  False
-   57807.412 20.6052 0.6375    V Las Cumbres  False
-   57807.416 19.4096  0.412    V Las Cumbres  False
-  57807.4201   21.96  1.345    g Las Cumbres  False
-  57807.4252 20.9629 0.8273    g Las Cumbres  False
-  57807.4305 20.8064 1.0049    r Las Cumbres  False
-  57807.4345 20.2652 0.7862    r Las Cumbres  False
-  57807.4386 20.3894 1.2539    i Las Cumbres  False
-  57807.4426 19.6751 0.8647    i Las Cumbres  False
-  57814.1558 20.5039 0.5189    B Las Cumbres  False
-  57814.1609 24.2255 8.3704    B Las Cumbres  False
-  57814.1662 19.7947 0.5263    V Las Cumbres  False
-  57814.1701 19.9087 0.5246    V Las Cumbres  False
-  57814.1795 21.8048 1.5513    g Las Cumbres  False
-  57814.1848 20.1846 0.5811    r Las Cumbres  False
-  57814.1888 19.4576 0.4449    r Las Cumbres  False
-  57814.1929 19.3681 0.5591    i Las Cumbres  False
-  57814.1969 19.5115 0.6109    i Las Cumbres  False
-  57816.1214 21.0726 1.9984    B Las Cumbres  False
-  57816.1319 19.5557 1.5166    V Las Cumbres  False
-  57816.1359 19.7717 1.5648    V Las Cumbres  False
-    57816.14 19.9113 0.8441    g Las Cumbres  False
-  57816.1451 20.6999 1.2018    g Las Cumbres  False
-  57816.1504 18.6592 0.6725    r Las Cumbres  False
-  57816.1544 20.3278  2.073    r Las Cumbres  False
-  57816.1585 18.3005 0.7592    i Las Cumbres  False
-  57822.1245   19.11  2.696    B Las Cumbres  False
-  57822.1349 21.0632 3.7725    V Las Cumbres  False
-  57822.1481 21.1737 3.3656    g Las Cumbres  False
-  57822.1534 19.7683 1.4092    r Las Cumbres  False
-  57822.1574 19.0655 1.2399    r Las Cumbres  False
-  57822.1655  19.705 1.5702    i Las Cumbres  False
-  57831.3669 21.1507   1.33    B Las Cumbres  False
-  57831.3722 21.0642 1.5076    V Las Cumbres  False
-  57831.3762 21.1854 1.6728    V Las Cumbres  False
-  57831.3804 23.0996 5.0928    g Las Cumbres  False
-  57831.3855 20.4333 1.0164    g Las Cumbres  False
-  57831.3908 20.5795   0.68    r Las Cumbres  False
-  57831.3947 21.0693   1.11    r Las Cumbres  False
-  57832.1173 20.7821  0.609    B Las Cumbres  False
-  57832.1224  21.164   0.68    B Las Cumbres  False
-  57832.1317 20.3252 0.6191    V Las Cumbres  False
-  57832.1544 21.0201 1.8544    i Las Cumbres  False
-  57832.1583 21.3014 2.4243    i Las Cumbres  False
-  57840.2301 21.2524  1.527    B Las Cumbres  False
-  57840.2394   21.66 1.8993    V Las Cumbres  False
-  57846.3281 22.5914 3.4365    B Las Cumbres  False
-  57846.3385 20.7249   2.56    V Las Cumbres  False
-  57846.3427 21.4896 2.8461    V Las Cumbres  False
-  57846.3469 19.8849 1.2986    g Las Cumbres  False
-  57846.3615 21.1752 1.6475    r Las Cumbres  False
-  57846.3657 19.7331 1.3488    i Las Cumbres  False
-  57846.3697 20.3611 1.5982    i Las Cumbres  False
-  57847.3232 20.5777 3.3603    B Las Cumbres  False
-  57847.3285  22.459 4.7326    V Las Cumbres  False
-  57847.3552 21.7386 3.8672    i Las Cumbres  False
-  57847.3592 21.7117 3.8542    i Las Cumbres  False
-  57853.2989 19.4533 2.3217    B Las Cumbres  False
-  57853.3042  20.485 2.5486    V Las Cumbres  False
-  57853.3123 18.9198 1.5881    g Las Cumbres  False
-  57853.3267 19.0449 1.0132    r Las Cumbres  False
-  57853.3347 17.4111 0.9368    i Las Cumbres  False
-  57918.1261 21.0509 2.5703    i Las Cumbres  False
-    57918.13 21.4048 3.0262    i Las Cumbres  False
-  57918.1342 21.8719 2.4022    B Las Cumbres  False
-  57918.1632 21.1615  2.163    V Las Cumbres  False
+         MJD     mag   dmag filter      source nondet
+------------ ------- ------ ------ ----------- ------
+   57468.703   17.53   0.16      0     Itagaki  False
+   57469.627   16.87   0.11      0     Itagaki  False
+  57470.3372 14.9383  0.012      U Las Cumbres  False
+  57470.3423 14.9143 0.0119      U Las Cumbres  False
+  57470.3476 16.0306 0.0373      B Las Cumbres  False
+  57470.3504 16.0132 0.0378      B Las Cumbres  False
+  57470.3534 15.9702 0.0362      V Las Cumbres  False
+  57470.3553 15.9877 0.0369      V Las Cumbres  False
+  57470.3574 15.8015 0.1125      g Las Cumbres  False
+  57470.3602 15.8182 0.1123      g Las Cumbres  False
+  57470.3633  16.116 0.0495      r Las Cumbres  False
+  57470.3652 16.0548  0.049      r Las Cumbres  False
+  57470.3673 16.3185 0.0635      i Las Cumbres  False
+  57470.3691 16.4189 0.0661      i Las Cumbres  False
+   57470.596   15.75   0.04      0     Itagaki  False
+57470.633579  15.689  0.013      V         TNT  False
+57470.633579  15.726  0.022      R         TNT  False
+57470.633579  15.735   0.02      I         TNT  False
+57470.633579  15.745  0.023      B         TNT  False
+   57471.423   15.34   0.03      0     Itagaki  False
+   57471.484   15.45   0.02      0     Itagaki  False
+ 57471.60544  15.346  0.024      R         TNT  False
+ 57471.60544  15.304  0.012      V         TNT  False
+ 57471.60544  15.179  0.015      B         TNT  False
+ 57471.60544  15.378  0.018      I         TNT  False
+  57472.0954 13.9765  0.014      U Las Cumbres  False
+  57472.0994 13.9698 0.0141      U Las Cumbres  False
+  57472.1037 15.0841 0.0246      B Las Cumbres  False
+  57472.1056 15.0806 0.0246      B Las Cumbres  False
+  57472.1076 15.2876 0.0161      V Las Cumbres  False
+  57472.1092 15.2664 0.0161      V Las Cumbres  False
+  57472.1179 13.9737 0.0169      U Las Cumbres  False
+  57472.1218 14.0148 0.0172      U Las Cumbres  False
+   57472.126 15.1316 0.0248      B Las Cumbres  False
+  57472.1278 15.1107 0.0248      B Las Cumbres  False
+  57472.1299 15.2811 0.0171      V Las Cumbres  False
+  57472.1314 15.2747 0.0171      V Las Cumbres  False
+  57472.1331 14.9552 0.1093      g Las Cumbres  False
+   57472.135 14.9651 0.1093      g Las Cumbres  False
+  57472.1371 15.3823 0.0296      r Las Cumbres  False
+  57472.1386 15.3536 0.0296      r Las Cumbres  False
+  57472.1403 15.5671 0.0407      i Las Cumbres  False
+  57472.1419 15.7132 0.0411      i Las Cumbres  False
+  57472.1451 14.0307 0.0198      U Las Cumbres  False
+  57472.1509 14.0526 0.0205      U Las Cumbres  False
+  57472.1549 14.0547 0.0199      U Las Cumbres  False
+   57472.159 15.1155 0.0248      B Las Cumbres  False
+  57472.1608 15.1021 0.0248      B Las Cumbres  False
+   57472.163 15.2592 0.0171      V Las Cumbres  False
+  57472.1645 15.2945 0.0166      V Las Cumbres  False
+  57472.1664 14.9396 0.1093      g Las Cumbres  False
+  57472.1683 14.9601 0.1093      g Las Cumbres  False
+  57472.1704 15.3706 0.0296      r Las Cumbres  False
+  57472.1719 15.3817 0.0296      r Las Cumbres  False
+  57472.1736 15.6175 0.0411      i Las Cumbres  False
+  57472.1751 15.5746 0.0407      i Las Cumbres  False
+  57472.1781 14.0458 0.0148      U Las Cumbres  False
+  57472.1837 14.0976 0.0246      U Las Cumbres  False
+  57472.1877 14.0827 0.0192      U Las Cumbres  False
+  57472.1942 14.0238 0.0162      U Las Cumbres  False
+  57472.1982 14.0354 0.0186      U Las Cumbres  False
+  57472.2024 15.0924 0.0248      B Las Cumbres  False
+  57472.2065 15.2437 0.0166      V Las Cumbres  False
+   57472.208 15.2757 0.0166      V Las Cumbres  False
+  57472.2098 14.9417 0.1092      g Las Cumbres  False
+  57472.2116 14.9297 0.1092      g Las Cumbres  False
+  57472.2137 15.3567 0.0296      r Las Cumbres  False
+  57472.2152 15.3116 0.0293      r Las Cumbres  False
+   57472.217 15.5654 0.0407      i Las Cumbres  False
+  57472.2185 15.5834 0.0411      i Las Cumbres  False
+    57472.42   15.17   0.02      0     Itagaki  False
+  57473.2103 13.8475 0.0074      U Las Cumbres  False
+  57473.2143 13.8502 0.0075      U Las Cumbres  False
+  57473.2184 14.9265 0.0246      B Las Cumbres  False
+  57473.2203 14.9224 0.0246      B Las Cumbres  False
+  57473.2225 15.0945 0.0156      V Las Cumbres  False
+   57473.224 15.0954 0.0156      V Las Cumbres  False
+  57473.2257 14.7559 0.1092      g Las Cumbres  False
+  57473.2276 14.7557 0.1092      g Las Cumbres  False
+  57473.2354 13.8383 0.0086      U Las Cumbres  False
+  57473.2397 14.8866 0.0246      B Las Cumbres  False
+  57473.2436 15.0923  0.016      V Las Cumbres  False
+  57473.2451  15.101  0.016      V Las Cumbres  False
+  57473.2469 14.7595 0.1092      g Las Cumbres  False
+  57473.2488 14.7791 0.1092      g Las Cumbres  False
+  57473.2508 15.1653 0.0289      r Las Cumbres  False
+  57473.2524 15.3521 0.0291      r Las Cumbres  False
+  57473.2541 15.5449 0.0401      i Las Cumbres  False
+  57473.2556 15.5238 0.0401      i Las Cumbres  False
+  57473.2651 13.8145 0.0085      U Las Cumbres  False
+  57473.2691 13.8089 0.0086      U Las Cumbres  False
+  57473.2734 14.8989 0.0246      B Las Cumbres  False
+  57473.2753 14.9021 0.0246      B Las Cumbres  False
+  57473.2773 15.0927  0.016      V Las Cumbres  False
+  57473.2788 15.0752  0.016      V Las Cumbres  False
+  57473.2807 14.7366 0.1092      g Las Cumbres  False
+  57473.2826 14.7288 0.1092      g Las Cumbres  False
+  57473.2846 15.1865 0.0291      r Las Cumbres  False
+  57473.2861 15.1721 0.0289      r Las Cumbres  False
+  57473.2878 15.4708 0.0401      i Las Cumbres  False
+  57473.2893 15.4026 0.0397      i Las Cumbres  False
+  57473.2978 13.7532 0.0089      U Las Cumbres  False
+  57473.3018  13.791 0.0097      U Las Cumbres  False
+  57473.3059  14.865 0.0246      B Las Cumbres  False
+  57473.3078 14.8646 0.0247      B Las Cumbres  False
+  57473.3098 15.0766  0.016      V Las Cumbres  False
+  57473.3114 15.0608  0.016      V Las Cumbres  False
+  57473.3132 14.7124 0.1092      g Las Cumbres  False
+  57473.3151  14.711 0.1092      g Las Cumbres  False
+  57473.3171 15.1418 0.0289      r Las Cumbres  False
+  57473.3187 15.1652 0.0291      r Las Cumbres  False
+  57473.3204 15.4497 0.0401      i Las Cumbres  False
+   57473.322 15.4474 0.0401      i Las Cumbres  False
+57476.575918  14.783  0.014      I         TNT  False
+57476.575918  14.775  0.021      R         TNT  False
+57476.575918  14.761  0.014      V         TNT  False
+57476.575918  14.834  0.014      B         TNT  False
+57477.593588  14.865  0.011      V         TNT  False
+57477.593588   14.89  0.022      R         TNT  False
+57477.593588  14.964  0.013      B         TNT  False
+57477.593588  14.865  0.016      I         TNT  False
+57477.593588   13.35  0.264      U         TNT  False
+57481.643748  15.188  0.024      R         TNT  False
+57481.643748  15.096  0.016      I         TNT  False
+57481.643748  15.226  0.012      V         TNT  False
+57481.643748  15.427  0.016      B         TNT  False
+57481.643748  13.744  0.263      U         TNT  False
+  57482.1006 14.5399 0.0116      U Las Cumbres  False
+  57482.1034 14.4856 0.0112      U Las Cumbres  False
+  57482.1064 15.4371 0.0256      B Las Cumbres  False
+  57482.1079 15.4248 0.0256      B Las Cumbres  False
+  57482.1096 15.3246 0.0176      V Las Cumbres  False
+57482.645295    15.3  0.012      V         TNT  False
+57482.645295  15.511  0.016      B         TNT  False
+57482.645295  15.221  0.026      R         TNT  False
+57482.645295  15.126  0.016      I         TNT  False
+57482.645295  14.203  0.254      U         TNT  False
+  57483.3497 14.6901 0.0141      U Las Cumbres  False
+  57483.3524 14.7305  0.015      U Las Cumbres  False
+  57483.3554 15.3658 0.0258      B Las Cumbres  False
+  57483.3569 15.3485 0.0258      B Las Cumbres  False
+  57483.3586 15.2849 0.0178      V Las Cumbres  False
+  57483.3598 15.3422 0.0178      V Las Cumbres  False
+  57483.3612 15.1809 0.1094      g Las Cumbres  False
+  57483.3628 15.1828 0.1094      g Las Cumbres  False
+  57483.3645  15.373 0.0316      r Las Cumbres  False
+  57483.3657 15.3807 0.0316      r Las Cumbres  False
+   57483.367 15.5451 0.0428      i Las Cumbres  False
+  57483.3682 15.5785 0.0432      i Las Cumbres  False
+  57487.1033 15.0075 0.0118      U Las Cumbres  False
+  57487.1061 14.9903 0.0118      U Las Cumbres  False
+  57489.2466 15.1748 0.0109      U Las Cumbres  False
+  57489.2493 15.1471   0.01      U Las Cumbres  False
+  57489.2523 15.9063 0.0269      B Las Cumbres  False
+  57489.2538 15.9053 0.0266      B Las Cumbres  False
+  57489.2556 15.6455 0.0194      V Las Cumbres  False
+  57489.2569 15.6609 0.0194      V Las Cumbres  False
+  57489.2582 15.6253 0.1095      g Las Cumbres  False
+  57489.2597 15.6073 0.1095      g Las Cumbres  False
+  57489.2614 15.6425 0.0322      r Las Cumbres  False
+  57489.2626 15.6172 0.0322      r Las Cumbres  False
+  57489.2639 15.7431 0.0434      i Las Cumbres  False
+  57489.2651 15.7289 0.0434      i Las Cumbres  False
+  57490.1527  15.251 0.0118      U Las Cumbres  False
+  57490.1555 15.2541 0.0116      U Las Cumbres  False
+  57490.1584 16.0249 0.0271      B Las Cumbres  False
+  57490.1599 16.0029 0.0271      B Las Cumbres  False
+  57490.1616 15.7059 0.0203      V Las Cumbres  False
+  57490.1628 15.7009 0.0203      V Las Cumbres  False
+  57490.1641 15.7022 0.1096      g Las Cumbres  False
+  57490.1656 15.7091 0.1096      g Las Cumbres  False
+  57490.1673 15.6717 0.0331      r Las Cumbres  False
+  57490.1685 15.6957 0.0334      r Las Cumbres  False
+  57490.1698 15.7308 0.0443      i Las Cumbres  False
+  57490.1709 15.8258 0.0448      i Las Cumbres  False
+  57491.2782  15.344 0.0148      U Las Cumbres  False
+   57491.281 15.3738 0.0145      U Las Cumbres  False
+  57491.2855 15.9779 0.0279      B Las Cumbres  False
+  57491.2872  15.648 0.0219      V Las Cumbres  False
+  57491.2883 15.7342 0.0219      V Las Cumbres  False
+  57491.2897 15.6847 0.1097      g Las Cumbres  False
+  57491.2912 15.7002 0.1098      g Las Cumbres  False
+  57491.2928 15.6685 0.0338      r Las Cumbres  False
+   57491.294 15.6609 0.0338      r Las Cumbres  False
+  57491.2953 15.7567 0.0451      i Las Cumbres  False
+  57491.2965 15.7024 0.0456      i Las Cumbres  False
+57491.578365  15.369  0.019      I         TNT  False
+57491.578365  16.031  0.017      B         TNT  False
+57491.578365  15.501  0.023      R         TNT  False
+57491.578365   15.05  0.297      U         TNT  False
+57491.578365  15.658  0.015      V         TNT  False
+   57492.243 15.4876 0.0136      U Las Cumbres  False
+  57492.2457 15.4021 0.0129      U Las Cumbres  False
+  57492.2487 16.0975 0.0292      B Las Cumbres  False
+  57492.2502 16.1095 0.0292      B Las Cumbres  False
+  57492.2518 15.7298 0.0228      V Las Cumbres  False
+   57492.253 15.7393 0.0234      V Las Cumbres  False
+  57492.2544 15.7825   0.11      g Las Cumbres  False
+  57492.2559 15.7635   0.11      g Las Cumbres  False
+  57492.2575 15.7023 0.0346      r Las Cumbres  False
+  57492.2587 15.7249 0.0349      r Las Cumbres  False
+    57492.26 15.8382 0.0459      i Las Cumbres  False
+  57492.2612  15.864 0.0459      i Las Cumbres  False
+  57494.2802 15.6466 0.0159      U Las Cumbres  False
+   57494.283 15.6557 0.0174      U Las Cumbres  False
+  57494.2859 16.1629  0.036      B Las Cumbres  False
+  57494.2875 16.1811 0.0365      B Las Cumbres  False
+  57494.2891 15.7704 0.0303      V Las Cumbres  False
+  57494.2903 15.7524 0.0297      V Las Cumbres  False
+  57494.2916 15.8363 0.1112      g Las Cumbres  False
+  57494.2931 15.8175 0.1112      g Las Cumbres  False
+  57494.2948 15.7117 0.0397      r Las Cumbres  False
+   57494.296  15.731 0.0397      r Las Cumbres  False
+  57494.2973 15.8523 0.0505      i Las Cumbres  False
+  57494.2984  15.805 0.0505      i Las Cumbres  False
+57494.627855  16.174  0.022      B         TNT  False
+57494.627855  15.542  0.025      R         TNT  False
+57494.627855  15.434  0.023      I         TNT  False
+57494.627855  15.755  0.014      V         TNT  False
+  57496.2915 15.7822 0.0463      U Las Cumbres  False
+  57496.2943 15.8017 0.0403      U Las Cumbres  False
+  57496.2972 16.5733  0.054      B Las Cumbres  False
+  57496.2987   16.52 0.0564      B Las Cumbres  False
+  57496.3016 15.9073  0.051      V Las Cumbres  False
+  57496.3086 15.9384 0.0517      i Las Cumbres  False
+  57498.2186 16.0172 0.0295      U Las Cumbres  False
+  57498.2214 15.9732 0.0243      U Las Cumbres  False
+  57498.2243 16.4274 0.0462      B Las Cumbres  False
+  57498.2258 16.4265  0.045      B Las Cumbres  False
+  57498.2275 15.9785 0.0406      V Las Cumbres  False
+  57498.2287  15.874 0.0392      V Las Cumbres  False
+    57498.23 16.0364 0.1127      g Las Cumbres  False
+  57498.2315 16.0326 0.1128      g Las Cumbres  False
+  57498.2333  15.798  0.043      r Las Cumbres  False
+  57498.2345 15.8217 0.0434      r Las Cumbres  False
+  57498.2358 15.8616 0.0551      i Las Cumbres  False
+   57498.237 15.8664 0.0551      i Las Cumbres  False
+57498.625483  15.823  0.012      V         TNT  False
+57498.625483   15.44  0.021      I         TNT  False
+57498.625483  15.646  0.028      R         TNT  False
+57498.625483   16.44  0.024      B         TNT  False
+  57500.1844 16.1327 0.0298      U Las Cumbres  False
+  57500.1872 16.0613 0.0294      U Las Cumbres  False
+  57500.1902 16.5307  0.058      B Las Cumbres  False
+  57500.1917 16.5291 0.0559      B Las Cumbres  False
+  57500.1934  15.931 0.0478      V Las Cumbres  False
+  57500.1946 15.9987 0.0484      V Las Cumbres  False
+   57500.196 16.1066  0.115      g Las Cumbres  False
+  57500.1975   16.09 0.1146      g Las Cumbres  False
+  57500.1993 15.8489 0.0502      r Las Cumbres  False
+  57500.2004 15.8787 0.0512      r Las Cumbres  False
+  57500.2017 15.9051 0.0602      i Las Cumbres  False
+  57500.2029  15.949 0.0748      i Las Cumbres  False
+57500.618378  15.441  0.021      I         TNT  False
+57500.618378  16.503  0.033      B         TNT  False
+57500.618378  15.858  0.016      V         TNT  False
+57500.618378  15.634  0.025      R         TNT  False
+57501.620423  15.869  0.013      V         TNT  False
+57501.620423  15.414  0.017      I         TNT  False
+57501.620423  16.491  0.018      B         TNT  False
+57501.620423  15.635  0.026      R         TNT  False
+57501.620423  17.168  0.375      U         TNT  False
+  57502.1117  16.402 0.0339      U Las Cumbres  False
+  57502.1146    16.4 0.0397      U Las Cumbres  False
+  57502.1175 16.5647 0.0451      B Las Cumbres  False
+   57502.119 16.5748 0.0451      B Las Cumbres  False
+  57502.1207 15.9322 0.0395      V Las Cumbres  False
+  57503.1979 16.4077 0.0239      U Las Cumbres  False
+  57503.2007 16.3992 0.0245      U Las Cumbres  False
+  57503.2036 16.5655 0.0368      B Las Cumbres  False
+  57503.2051 16.6427 0.0379      B Las Cumbres  False
+  57503.2068 15.9645   0.03      V Las Cumbres  False
+   57503.208   15.99   0.03      V Las Cumbres  False
+  57503.2093 16.1823 0.1109      g Las Cumbres  False
+  57503.2108 16.1746 0.1109      g Las Cumbres  False
+  57503.2125 15.8838 0.0372      r Las Cumbres  False
+  57503.2137 15.8595 0.0368      r Las Cumbres  False
+  57503.2151  15.889  0.049      i Las Cumbres  False
+  57503.2162 15.8288 0.0485      i Las Cumbres  False
+  57504.1843 16.5057 0.0238      U Las Cumbres  False
+  57504.1872  16.521  0.028      U Las Cumbres  False
+  57504.1902 16.6124 0.0344      B Las Cumbres  False
+  57504.1917 16.6207 0.0338      B Las Cumbres  False
+  57504.1934 15.9988 0.0271      V Las Cumbres  False
+  57504.1946 15.9485 0.0271      V Las Cumbres  False
+  57504.1961 16.2135 0.1104      g Las Cumbres  False
+  57504.1977 16.2148 0.1106      g Las Cumbres  False
+  57504.1995 15.8648 0.0369      r Las Cumbres  False
+  57504.2008 15.9055 0.0369      r Las Cumbres  False
+  57504.2021 15.9256 0.0496      i Las Cumbres  False
+  57504.2033 15.8654 0.0485      i Las Cumbres  False
+  57505.2678  16.498 0.0333      U Las Cumbres  False
+  57505.2708 16.5583 0.0378      U Las Cumbres  False
+  57505.2739  16.574 0.0416      B Las Cumbres  False
+  57505.2754 16.6056 0.0429      B Las Cumbres  False
+  57505.2771 15.9298 0.0336      V Las Cumbres  False
+  57505.2783 15.9216 0.0336      V Las Cumbres  False
+  57505.2798 16.1891 0.1115      g Las Cumbres  False
+  57505.2814 16.1606 0.1115      g Las Cumbres  False
+  57505.2838 15.8836 0.0435      r Las Cumbres  False
+  57505.2851 15.8416 0.0435      r Las Cumbres  False
+  57505.2865 15.9387 0.0547      i Las Cumbres  False
+  57506.2537 16.7218 0.0252      U Las Cumbres  False
+  57506.2565 16.6866 0.0253      U Las Cumbres  False
+  57506.2595 16.6303 0.0334      B Las Cumbres  False
+   57506.261 16.6623 0.0334      B Las Cumbres  False
+  57506.2627  15.938 0.0253      V Las Cumbres  False
+  57506.2638  15.984 0.0259      V Las Cumbres  False
+  57506.2652 16.1868 0.1103      g Las Cumbres  False
+  57506.2667 16.1829 0.1103      g Las Cumbres  False
+  57506.2684 15.8172 0.0355      r Las Cumbres  False
+  57506.2695 15.8294 0.0355      r Las Cumbres  False
+  57506.2709 15.8158 0.0468      i Las Cumbres  False
+  57506.2721 15.7944 0.0473      i Las Cumbres  False
+  57508.1076 16.7838 0.0583      U Las Cumbres  False
+  57508.1106 16.7567 0.0406      B Las Cumbres  False
+  57508.1121 16.8007 0.0381      B Las Cumbres  False
+  57508.1138 16.0219 0.0285      V Las Cumbres  False
+  57508.1149 16.0689 0.0285      V Las Cumbres  False
+  57508.1163 16.3285 0.1108      g Las Cumbres  False
+  57508.1178 16.3504  0.111      g Las Cumbres  False
+  57508.1195 15.7281 0.0529      r Las Cumbres  False
+  57508.1206 15.8821 0.0355      r Las Cumbres  False
+   57508.122 15.8901 0.0466      i Las Cumbres  False
+  57508.1231  15.863  0.047      i Las Cumbres  False
+  57512.2401 16.8905 0.0377      U Las Cumbres  False
+  57512.2429 16.9686 0.0407      U Las Cumbres  False
+  57512.2458 16.8504 0.0369      B Las Cumbres  False
+  57512.2473 16.8123 0.0374      B Las Cumbres  False
+   57512.249   15.97 0.0276      V Las Cumbres  False
+  57512.2502 15.9749 0.0276      V Las Cumbres  False
+  57512.2516 16.3494 0.1106      g Las Cumbres  False
+  57512.2531 16.2754 0.1106      g Las Cumbres  False
+  57512.2548 15.7885 0.0352      r Las Cumbres  False
+   57512.256 15.7987 0.0355      r Las Cumbres  False
+  57512.2573 15.8455 0.0468      i Las Cumbres  False
+  57512.2585 15.8351 0.0478      i Las Cumbres  False
+57515.625795  16.935  0.034      B         TNT  False
+57515.625795  15.353  0.018      I         TNT  False
+57515.625795  15.926  0.013      V         TNT  False
+57515.625795  15.604  0.025      R         TNT  False
+  57517.1771 17.2135  0.042      U Las Cumbres  False
+    57517.18 17.2304 0.0503      U Las Cumbres  False
+  57517.1833 16.4835 0.0375      B Las Cumbres  False
+  57517.1848 16.5284  0.037      B Las Cumbres  False
+  57517.1865 16.0593 0.0278      V Las Cumbres  False
+  57517.1877 16.0567 0.0283      V Las Cumbres  False
+  57517.1891 16.4414 0.1106      g Las Cumbres  False
+  57517.1907 16.4913 0.1106      g Las Cumbres  False
+  57517.1924 15.8162 0.0345      r Las Cumbres  False
+  57517.1936 15.8108 0.0345      r Las Cumbres  False
+  57517.1949 15.7234 0.0453      i Las Cumbres  False
+  57517.1961 15.8121 0.0463      i Las Cumbres  False
+  57519.1194 17.3701 0.0514      U Las Cumbres  False
+  57519.1221 17.3135 0.0471      U Las Cumbres  False
+  57519.1251 17.1154 0.0386      B Las Cumbres  False
+  57519.1266 17.1389   0.04      B Las Cumbres  False
+  57519.1283 16.0316 0.0252      V Las Cumbres  False
+  57519.1295 16.0454 0.0257      V Las Cumbres  False
+  57519.1319 17.4122 0.0321      U Las Cumbres  False
+  57519.1346 17.2981 0.0361      U Las Cumbres  False
+  57519.1399 17.2792 0.0425      U Las Cumbres  False
+  57519.1427 17.5594 0.0606      U Las Cumbres  False
+  57519.1457 17.1332 0.0393      B Las Cumbres  False
+  57519.1472 17.1575   0.04      B Las Cumbres  False
+  57519.1489 16.0677 0.0257      V Las Cumbres  False
+  57519.1501 16.0503 0.0263      V Las Cumbres  False
+  57519.1516 16.5189 0.1104      g Las Cumbres  False
+  57519.1531 16.5103 0.1105      g Las Cumbres  False
+  57519.1548 15.8177 0.0334      r Las Cumbres  False
+  57519.1559 15.8014 0.0338      r Las Cumbres  False
+  57519.1573 15.7774 0.0439      i Las Cumbres  False
+  57519.1585 15.7843 0.0448      i Las Cumbres  False
+  57520.1233 17.5626 0.0748      U Las Cumbres  False
+  57520.1261 17.3713 0.0605      U Las Cumbres  False
+   57524.219 17.5308 0.1368      U Las Cumbres  False
+  57524.2218 17.8168 0.1503      U Las Cumbres  False
+  57524.2247 17.1324 0.0711      B Las Cumbres  False
+  57524.2263 17.0558 0.0682      B Las Cumbres  False
+   57524.228 16.0318 0.0521      V Las Cumbres  False
+  57524.2293 15.9815 0.0515      V Las Cumbres  False
+  57524.2322 16.5076 0.1188      g Las Cumbres  False
+   57524.235 15.7275 0.0509      r Las Cumbres  False
+  57524.2364 16.0481 0.0629      i Las Cumbres  False
+  57529.1401 17.8568 0.0535      U Las Cumbres  False
+  57529.1475 17.5866 0.0637      U Las Cumbres  False
+  57529.1551 17.2909 0.0899      B Las Cumbres  False
+  57529.1566 17.2987 0.0899      B Las Cumbres  False
+  57529.1582 16.1064 0.0614      V Las Cumbres  False
+  57529.1594 16.0538  0.061      V Las Cumbres  False
+  57529.1608 16.5989 0.1158      g Las Cumbres  False
+  57529.1623 16.6758 0.1163      g Las Cumbres  False
+   57529.164 15.8185 0.0393      r Las Cumbres  False
+  57529.1652 15.8071 0.0388      r Las Cumbres  False
+  57529.1666 15.7437 0.0496      i Las Cumbres  False
+  57529.1678 15.7215 0.0496      i Las Cumbres  False
+57540.545546  15.224  0.016      I         TNT  False
+57540.545546  18.715  0.314      U         TNT  False
+57540.545546  17.431  0.025      B         TNT  False
+57540.545546   16.07  0.014      V         TNT  False
+57540.545546  15.586  0.031      R         TNT  False
+  57556.1306 17.7635  0.117      B Las Cumbres  False
+  57556.1325 17.6177 0.0946      B Las Cumbres  False
+  57556.1346 16.1934 0.0549      V Las Cumbres  False
+  57556.1362 16.1709 0.0549      V Las Cumbres  False
+  57556.1379 16.9356 0.1147      g Las Cumbres  False
+  57556.1398 16.8479 0.1144      g Las Cumbres  False
+  57556.1419 15.7665 0.0343      r Las Cumbres  False
+  57556.1434 15.7323 0.0339      r Las Cumbres  False
+  57556.1502 17.9671  0.117      B Las Cumbres  False
+  57556.1521 17.8594 0.1082      B Las Cumbres  False
+  57556.1542 16.2084 0.0558      V Las Cumbres  False
+  57556.1558 16.1104 0.0549      V Las Cumbres  False
+  57556.1575 16.9335 0.1152      g Las Cumbres  False
+  57556.1594 16.8759 0.1152      g Las Cumbres  False
+  57556.1614 15.7605 0.0347      r Las Cumbres  False
+   57556.163 15.7489 0.0343      r Las Cumbres  False
+  57556.1647 15.6482 0.0437      i Las Cumbres  False
+  57556.1662 15.6344 0.0446      i Las Cumbres  False
+57557.535687  15.175  0.019      I         TNT  False
+57557.535687   17.58  0.031      B         TNT  False
+57557.535687  16.133  0.016      V         TNT  False
+57557.535687  15.576  0.028      R         TNT  False
+  57558.1365 17.6111 0.1539      B Las Cumbres  False
+  57558.1381 17.9324 0.1788      B Las Cumbres  False
+  57558.1398 16.2053 0.1045      V Las Cumbres  False
+  57558.1409 16.1249 0.1024      V Las Cumbres  False
+   57673.469 21.1534 0.8887      B Las Cumbres  False
+  57673.4718 19.8874 0.3658      B Las Cumbres  False
+  57673.4748 18.5588 0.3004      V Las Cumbres  False
+  57673.4766 18.8357 0.3172      V Las Cumbres  False
+  57673.4815 19.8136 0.3281      g Las Cumbres  False
+  57673.4845 17.8727 0.1103      r Las Cumbres  False
+  57673.4863 17.9603 0.1154      r Las Cumbres  False
+  57673.4883 17.5858 0.1324      i Las Cumbres  False
+  57673.4902 17.4805 0.1273      i Las Cumbres  False
+  57674.4813 18.6738 0.1776      V Las Cumbres  False
+  57674.4832 18.1513 0.2085      V Las Cumbres  False
+   57674.488    19.2  0.905      g Las Cumbres  False
+  57674.4926 17.5752 0.1454      r Las Cumbres  False
+  57674.4944 17.6976 0.1431      r Las Cumbres  False
+  57674.4964  17.667 0.1881      i Las Cumbres  False
+  57674.4983 17.8357 0.1858      i Las Cumbres  False
+  57679.4725  20.915 2.0742      B Las Cumbres  False
+  57679.4782 18.7554 1.4826      V Las Cumbres  False
+  57679.4801 18.1945 1.4697      V Las Cumbres  False
+  57679.4821 20.8627 1.1073      g Las Cumbres  False
+  57679.4849 21.4387 1.5362      g Las Cumbres  False
+  57679.4878 17.8407  0.149      r Las Cumbres  False
+  57679.4897 18.0179 0.1589      r Las Cumbres  False
+  57679.4917 17.7578 0.1712      i Las Cumbres  False
+  57679.4935 17.7364 0.1719      i Las Cumbres  False
+  57680.4541 20.8478 1.9707      B Las Cumbres  False
+   57680.458 22.4199 4.9667      B Las Cumbres  False
+  57680.4622 18.4156 1.4968      V Las Cumbres  False
+   57680.465 18.5194 1.4975      V Las Cumbres  False
+  57680.4679 19.1815 0.2785      g Las Cumbres  False
+  57680.4719  19.746 0.3341      g Las Cumbres  False
+   57680.476  18.119 0.1443      r Las Cumbres  False
+  57680.4788 18.0681 0.1418      r Las Cumbres  False
+  57680.4817 17.9673 0.1748      i Las Cumbres  False
+  57680.4845 17.8122 0.1673      i Las Cumbres  False
+  57688.4292 20.5924 0.4195      B Las Cumbres  False
+  57688.4332 20.2091 0.4099      B Las Cumbres  False
+  57688.4373 18.7214 0.2723      V Las Cumbres  False
+  57688.4401 18.7504 0.2774      V Las Cumbres  False
+  57688.4431 22.6568 2.2698      g Las Cumbres  False
+   57688.447 21.2946 1.0653      g Las Cumbres  False
+  57688.4511 18.4416  0.133      r Las Cumbres  False
+  57688.4539 18.5158 0.1392      r Las Cumbres  False
+  57688.4569 18.0088  0.154      i Las Cumbres  False
+  57688.4597 18.1888 0.1719      i Las Cumbres  False
+57696.906824  17.728  0.038      R         TNT  False
+57696.906824  18.598  0.039      V         TNT  False
+57696.906824  17.209  0.034      I         TNT  False
+  57699.4068 20.4431 0.3375      B Las Cumbres  False
+  57699.4108 19.5627 0.2289      B Las Cumbres  False
+  57699.4149 18.9921 0.2194      V Las Cumbres  False
+  57699.4177 17.8577 0.1834      V Las Cumbres  False
+  57699.4345 18.4145   0.19      i Las Cumbres  False
+57706.807542  17.867  0.053      R         TNT  False
+57706.807542  17.351  0.043      I         TNT  False
+  57707.3848 20.0002 0.7507      B Las Cumbres  False
+  57707.3887 19.1218  0.438      B Las Cumbres  False
+  57707.3929 19.2638 0.5016      V Las Cumbres  False
+  57707.3957 18.4894  0.385      V Las Cumbres  False
+  57707.3986 19.7339 0.4316      g Las Cumbres  False
+  57707.4026  18.844 0.2948      g Las Cumbres  False
+  57707.4067   18.02 0.1713      r Las Cumbres  False
+  57707.4094  18.382 0.1963      r Las Cumbres  False
+  57707.4124 17.9194 0.1914      i Las Cumbres  False
+  57707.4152 18.0853 0.2051      i Las Cumbres  False
+57708.768464  17.337  0.141      I         TNT  False
+57708.768464  18.074  0.201      R         TNT  False
+57714.825623  17.296  0.078      I         TNT  False
+    57715.49 20.8948 0.4886      B Las Cumbres  False
+  57715.4939 20.2211 0.3241      B Las Cumbres  False
+   57715.498 18.7717 0.2517      V Las Cumbres  False
+  57715.5008 18.7452   0.25      V Las Cumbres  False
+  57715.5038 19.9626  0.264      g Las Cumbres  False
+  57715.5078 19.9024 0.2598      g Las Cumbres  False
+  57715.5119 18.1421 0.1232      r Las Cumbres  False
+  57715.5147 18.1883 0.1259      r Las Cumbres  False
+  57715.5177 18.0163 0.1752      i Las Cumbres  False
+  57715.5204 17.8004 0.1569      i Las Cumbres  False
+ 57715.90839  17.327   0.04      I         TNT  False
+ 57715.90839  20.392    0.1      B         TNT  False
+ 57715.90839  18.488  0.036      V         TNT  False
+ 57715.90839  17.875  0.039      R         TNT  False
+57722.818443   18.53  0.049      V         TNT  False
+57722.818443  17.273  0.039      I         TNT  False
+57722.818443  17.883  0.042      R         TNT  False
+  57723.3684 22.8285 2.8164      B Las Cumbres  False
+  57723.3724 21.1664 0.9232      B Las Cumbres  False
+  57723.3765 18.7387 0.7082      V Las Cumbres  False
+  57723.3793 18.7662 0.7093      V Las Cumbres  False
+  57723.3823 20.1744 0.3124      g Las Cumbres  False
+  57723.3862 20.0576 0.2843      g Las Cumbres  False
+  57723.3904 18.4058 0.1547      r Las Cumbres  False
+  57723.3931 18.5471 0.1559      r Las Cumbres  False
+  57723.3961 18.3702 0.1978      i Las Cumbres  False
+  57723.3989 18.0438 0.1717      i Las Cumbres  False
+57723.675749  17.928  0.037      R         TNT  False
+57723.675749  20.237  0.099      B         TNT  False
+57723.675749  17.401  0.031      I         TNT  False
+57723.675749  18.666  0.038      V         TNT  False
+57727.787505    18.0  0.047      R         TNT  False
+57727.787505  18.639  0.038      V         TNT  False
+57727.787505    20.0   0.08      B         TNT  False
+57727.787505  17.471  0.033      I         TNT  False
+57728.907253  20.155  0.098      B         TNT  False
+57728.907253  18.657  0.043      V         TNT  False
+57728.907253  17.984  0.039      R         TNT  False
+57728.907253   17.41  0.039      I         TNT  False
+57730.896945  17.379  0.031      I         TNT  False
+57730.896945  18.008  0.049      R         TNT  False
+57730.896945  18.758  0.069      V         TNT  False
+57730.896945  20.206  0.113      B         TNT  False
+57731.793337  20.061  0.103      B         TNT  False
+57731.793337  17.521  0.043      I         TNT  False
+57731.793337  18.694  0.035      V         TNT  False
+57731.793337  17.941  0.037      R         TNT  False
+  57732.3233 21.6992 2.7869      B Las Cumbres  False
+  57732.3273  22.071 3.1274      B Las Cumbres  False
+  57732.3315 19.3308 1.7215      V Las Cumbres  False
+  57732.3342  18.833  1.713      V Las Cumbres  False
+  57732.3373 19.8076 0.3557      g Las Cumbres  False
+  57732.3413 19.4733 0.2982      g Las Cumbres  False
+  57732.3454 18.3222 0.1736      r Las Cumbres  False
+  57732.3482  18.284 0.1712      r Las Cumbres  False
+  57732.3512 18.1615 0.2176      i Las Cumbres  False
+   57732.354 18.1794   0.21      i Las Cumbres  False
+57732.781453  17.927   0.04      R         TNT  False
+57732.781453  18.634  0.039      V         TNT  False
+57732.781453  20.276  0.098      B         TNT  False
+57732.781453  17.428  0.036      I         TNT  False
+57736.832265  18.003  0.046      R         TNT  False
+57736.832265  18.763  0.061      V         TNT  False
+57736.832265  17.462  0.035      I         TNT  False
+57737.793884   18.66  0.076      V         TNT  False
+57737.793884   18.06  0.042      R         TNT  False
+57737.793884  17.536  0.047      I         TNT  False
+  57738.4594 21.0256 1.7417      B Las Cumbres  False
+  57738.4634  22.066 3.5607      B Las Cumbres  False
+  57738.4675 18.6401 1.2579      V Las Cumbres  False
+  57738.4703 19.0732 1.2727      V Las Cumbres  False
+  57738.4733 20.3567 0.6506      g Las Cumbres  False
+  57738.4772 19.6308 0.4061      g Las Cumbres  False
+  57738.4814  18.444 0.2041      r Las Cumbres  False
+  57738.4841  18.496 0.2001      r Las Cumbres  False
+  57738.4871 18.1265   0.22      i Las Cumbres  False
+  57738.4899 18.2485 0.2303      i Las Cumbres  False
+57739.871799  20.154  0.116      B         TNT  False
+57739.871799  18.505  0.035      V         TNT  False
+57739.871799  17.544  0.041      I         TNT  False
+57739.871799  18.023  0.038      R         TNT  False
+ 57740.85571  17.633  0.054      I         TNT  False
+ 57740.85571  18.669  0.051      V         TNT  False
+ 57740.85571   20.19  0.095      B         TNT  False
+ 57740.85571  18.059  0.039      R         TNT  False
+57741.903241  17.969  0.041      R         TNT  False
+57741.903241  20.004  0.081      B         TNT  False
+57741.903241   18.75  0.034      V         TNT  False
+57741.903241  17.584  0.038      I         TNT  False
+57744.810645  17.727  0.062      I         TNT  False
+57744.810645  18.062  0.052      R         TNT  False
+57744.810645  18.588  0.068      V         TNT  False
+57745.925413   17.51  0.034      I         TNT  False
+57745.925413  18.046  0.039      R         TNT  False
+57745.925413  18.718   0.05      V         TNT  False
+57745.925413  20.177  0.117      B         TNT  False
+    57746.49 22.3326 1.7927      B Las Cumbres  False
+  57746.4939 21.1568 0.8145      B Las Cumbres  False
+   57746.498 19.1673 0.6068      V Las Cumbres  False
+  57746.5008 19.0169 0.6057      V Las Cumbres  False
+  57746.5038 20.2377  0.286      g Las Cumbres  False
+  57746.5078 20.1206 0.2774      g Las Cumbres  False
+  57746.5119 18.9481   0.22      r Las Cumbres  False
+  57746.5147 19.1696 0.2331      r Las Cumbres  False
+  57746.5176 18.7021 0.2597      i Las Cumbres  False
+  57746.5204 18.8688 0.2939      i Las Cumbres  False
+ 57748.82233   17.58  0.045      I         TNT  False
+ 57748.82233  20.352  0.117      B         TNT  False
+ 57748.82233  18.155  0.046      R         TNT  False
+ 57748.82233  18.643  0.041      V         TNT  False
+57750.698686  20.156  0.098      B         TNT  False
+57750.698686  18.146  0.044      R         TNT  False
+57750.698686  17.546  0.045      I         TNT  False
+57750.698686  18.682  0.049      V         TNT  False
+57751.716248  17.542  0.036      I         TNT  False
+57751.716248  20.216  0.111      B         TNT  False
+57751.716248  18.131  0.045      R         TNT  False
+57751.716248  18.713  0.039      V         TNT  False
+57753.794307  18.731  0.035      V         TNT  False
+57753.794307  18.136  0.041      R         TNT  False
+57753.794307  19.945  0.083      B         TNT  False
+57753.794307  17.593  0.028      I         TNT  False
+  57754.3303 20.3375 0.3363      B Las Cumbres  False
+  57754.3343 20.3826 0.3324      B Las Cumbres  False
+  57754.3384 19.0015 0.2465      V Las Cumbres  False
+  57754.3412 18.9038 0.2432      V Las Cumbres  False
+  57754.3442 19.4622 0.2125      g Las Cumbres  False
+  57754.3482 19.4304 0.2277      g Las Cumbres  False
+  57754.3523 18.7175 0.2072      r Las Cumbres  False
+  57754.3551 18.8432 0.2161      r Las Cumbres  False
+  57754.3581  18.668 0.2808      i Las Cumbres  False
+  57754.3609 18.5053 0.2563      i Las Cumbres  False
+57754.864937   18.77  0.046      V         TNT  False
+57754.864937  17.538  0.034      I         TNT  False
+57754.864937   18.18  0.051      R         TNT  False
+57754.864937  20.174  0.097      B         TNT  False
+57755.704894  18.644  0.048      V         TNT  False
+57755.704894  17.595  0.051      I         TNT  False
+57755.704894  18.098  0.045      R         TNT  False
+  57757.4305 20.4754 0.3589      B Las Cumbres  False
+  57757.4344 20.5292 0.3951      B Las Cumbres  False
+  57757.4386 19.3142 0.9676      V Las Cumbres  False
+  57757.4414  18.755 0.3024      V Las Cumbres  False
+  57757.4444 19.7011 0.3106      g Las Cumbres  False
+57757.783408  17.786  0.069      I         TNT  False
+57757.783408  18.222  0.046      R         TNT  False
+57757.783408  18.877  0.044      V         TNT  False
+57757.783408  20.442  0.174      B         TNT  False
+  57758.3641  20.155 0.3232      B Las Cumbres  False
+  57758.3681 21.7585  0.961      B Las Cumbres  False
+  57758.3722 19.2541 0.3004      V Las Cumbres  False
+   57758.375 19.2438 0.2993      V Las Cumbres  False
+   57758.378 19.7486 0.2316      g Las Cumbres  False
+  57758.3819 19.6856 0.2355      g Las Cumbres  False
+  57758.3861 18.6252 0.1488      r Las Cumbres  False
+  57758.3888 18.6595 0.1558      r Las Cumbres  False
+  57758.3918 18.2208 0.1958      i Las Cumbres  False
+  57758.3946  18.302 0.1958      i Las Cumbres  False
+  57758.4094  21.255 0.6251      B Las Cumbres  False
+  57758.4133 22.1673 1.3297      B Las Cumbres  False
+  57758.4175 19.3989 0.3109      V Las Cumbres  False
+  57758.4203 19.3459 0.3115      V Las Cumbres  False
+  57758.4314 18.6353 0.1508      r Las Cumbres  False
+  57758.4342 18.6552 0.1558      r Las Cumbres  False
+  57758.4372 18.4895   0.23      i Las Cumbres  False
+    57758.44 18.5385 0.2265      i Las Cumbres  False
+57758.883741  17.696  0.057      I         TNT  False
+57758.883741  18.228  0.049      R         TNT  False
+57758.883741  20.324  0.116      B         TNT  False
+57758.883741  18.911  0.039      V         TNT  False
+57762.655904  17.679  0.051      I         TNT  False
+57762.655904  18.701  0.095      V         TNT  False
+57762.655904  18.333  0.053      R         TNT  False
+57775.590604  17.731   0.07      I         TNT  False
+57775.590604  18.444  0.075      R         TNT  False
+57775.590604  18.801  0.093      V         TNT  False
+  57782.4936 21.9845 1.3972      B Las Cumbres  False
+  57782.4975 21.2106 0.7839      B Las Cumbres  False
+  57782.5017 19.5279 0.5987      V Las Cumbres  False
+  57782.5045 19.7124 0.6139      V Las Cumbres  False
+  57782.5076 21.2163 0.8647      g Las Cumbres  False
+  57782.5157 19.0507 0.2759      r Las Cumbres  False
+  57782.5215 18.5641   0.31      i Las Cumbres  False
+  57782.5243 18.9661 0.3722      i Las Cumbres  False
+57797.531826  18.831  0.068      R         TNT  False
+57797.531826  18.373  0.069      I         TNT  False
+57800.630929  18.383  0.076      I         TNT  False
+57800.630929  18.847  0.087      R         TNT  False
+  57801.3635 22.4579 2.2635      B Las Cumbres  False
+  57801.3686 21.3339 1.0451      B Las Cumbres  False
+  57801.3739 20.0618 0.8374      V Las Cumbres  False
+  57801.3779 19.7686 0.8133      V Las Cumbres  False
+   57801.382 22.7567 3.0849      g Las Cumbres  False
+  57801.3871 21.0674 0.6138      g Las Cumbres  False
+  57801.4044 19.4755 0.4514      i Las Cumbres  False
+57803.737585  18.196  0.081      I         TNT  False
+57803.737585  18.988  0.109      R         TNT  False
+  57807.4016 20.6804 0.4934      B Las Cumbres  False
+   57807.412 20.6052 0.6375      V Las Cumbres  False
+   57807.416 19.4096  0.412      V Las Cumbres  False
+  57807.4201   21.96  1.345      g Las Cumbres  False
+  57807.4252 20.9629 0.8273      g Las Cumbres  False
+  57807.4305 20.8064 1.0049      r Las Cumbres  False
+  57807.4345 20.2652 0.7862      r Las Cumbres  False
+  57807.4386 20.3894 1.2539      i Las Cumbres  False
+  57807.4426 19.6751 0.8647      i Las Cumbres  False
+  57814.1558 20.5039 0.5189      B Las Cumbres  False
+  57814.1609 24.2255 8.3704      B Las Cumbres  False
+  57814.1662 19.7947 0.5263      V Las Cumbres  False
+  57814.1701 19.9087 0.5246      V Las Cumbres  False
+  57814.1795 21.8048 1.5513      g Las Cumbres  False
+  57814.1848 20.1846 0.5811      r Las Cumbres  False
+  57814.1888 19.4576 0.4449      r Las Cumbres  False
+  57814.1929 19.3681 0.5591      i Las Cumbres  False
+  57814.1969 19.5115 0.6109      i Las Cumbres  False
+  57816.1214 21.0726 1.9984      B Las Cumbres  False
+  57816.1319 19.5557 1.5166      V Las Cumbres  False
+  57816.1359 19.7717 1.5648      V Las Cumbres  False
+    57816.14 19.9113 0.8441      g Las Cumbres  False
+  57816.1451 20.6999 1.2018      g Las Cumbres  False
+  57816.1504 18.6592 0.6725      r Las Cumbres  False
+  57816.1544 20.3278  2.073      r Las Cumbres  False
+  57816.1585 18.3005 0.7592      i Las Cumbres  False
+  57822.1245   19.11  2.696      B Las Cumbres  False
+  57822.1349 21.0632 3.7725      V Las Cumbres  False
+  57822.1481 21.1737 3.3656      g Las Cumbres  False
+  57822.1534 19.7683 1.4092      r Las Cumbres  False
+  57822.1574 19.0655 1.2399      r Las Cumbres  False
+  57822.1655  19.705 1.5702      i Las Cumbres  False
+  57831.3669 21.1507   1.33      B Las Cumbres  False
+  57831.3722 21.0642 1.5076      V Las Cumbres  False
+  57831.3762 21.1854 1.6728      V Las Cumbres  False
+  57831.3804 23.0996 5.0928      g Las Cumbres  False
+  57831.3855 20.4333 1.0164      g Las Cumbres  False
+  57831.3908 20.5795   0.68      r Las Cumbres  False
+  57831.3947 21.0693   1.11      r Las Cumbres  False
+  57832.1173 20.7821  0.609      B Las Cumbres  False
+  57832.1224  21.164   0.68      B Las Cumbres  False
+  57832.1317 20.3252 0.6191      V Las Cumbres  False
+  57832.1544 21.0201 1.8544      i Las Cumbres  False
+  57832.1583 21.3014 2.4243      i Las Cumbres  False
+  57840.2301 21.2524  1.527      B Las Cumbres  False
+  57840.2394   21.66 1.8993      V Las Cumbres  False
+  57846.3281 22.5914 3.4365      B Las Cumbres  False
+  57846.3385 20.7249   2.56      V Las Cumbres  False
+  57846.3427 21.4896 2.8461      V Las Cumbres  False
+  57846.3469 19.8849 1.2986      g Las Cumbres  False
+  57846.3615 21.1752 1.6475      r Las Cumbres  False
+  57846.3657 19.7331 1.3488      i Las Cumbres  False
+  57846.3697 20.3611 1.5982      i Las Cumbres  False
+  57847.3232 20.5777 3.3603      B Las Cumbres  False
+  57847.3285  22.459 4.7326      V Las Cumbres  False
+  57847.3552 21.7386 3.8672      i Las Cumbres  False
+  57847.3592 21.7117 3.8542      i Las Cumbres  False
+  57853.2989 19.4533 2.3217      B Las Cumbres  False
+  57853.3042  20.485 2.5486      V Las Cumbres  False
+  57853.3123 18.9198 1.5881      g Las Cumbres  False
+  57853.3267 19.0449 1.0132      r Las Cumbres  False
+  57853.3347 17.4111 0.9368      i Las Cumbres  False
+  57918.1261 21.0509 2.5703      i Las Cumbres  False
+    57918.13 21.4048 3.0262      i Las Cumbres  False
+  57918.1342 21.8719 2.4022      B Las Cumbres  False
+  57918.1632 21.1615  2.163      V Las Cumbres  False
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/ATLAS_cyan.txt` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_cyan.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/ATLAS_orange.txt` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/ATLAS_orange.txt`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.Y.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.g.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.g.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.i.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.i.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.r.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.r.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/CTIO_DECam.z.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/CTIO_DECam.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GAIA_GAIA0.G.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.FUV.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/GALEX_GALEX.NUV.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.H.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.J.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Gemini_Flamingos2.Ks.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Generic_Cousins.R.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Generic_Cousins.R.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1000W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1130W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1280W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1500W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F1800W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2100W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F2550W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F560W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_MIRI.F770W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F070W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F090W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F115W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F150W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F200W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F277W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F356W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/JWST_NIRCam.F444W.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/KAF-1001E.asci` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.asci`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/KAF-1001E.csv` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/KAF-1001E.csv`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Kepler_Kepler.K.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/QE_E2V_MBBBUV_Broadband.csv`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.g.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.i.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.r.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.u.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/SLOAN_SDSS.z.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.B.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.B.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.U.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.U.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVM2.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW1.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.UVW2.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/Swift_UVOT.V.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/Swift_UVOT.V.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/TESS_TESS.Red.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/TESS_TESS.Red.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/alpha_lyr_stis_008.fits`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/orange.asci` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.asci`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters/orange.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters/orange.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/filters.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Ratio of total to selective extinction :math:`R_V`. Default: 3.1.
 
     Returns
     -------
     extinction : array-like
         Extinction factor :math:`10^{A/-2.5}` at each input wavelength.
     """
-    A = np.squeeze([fitzpatrick99(c / freq, rv * e) for e in np.atleast_1d(ebv)])
+    A = np.squeeze([fitzpatrick99(c / freq, rv * e, rv) for e in np.atleast_1d(ebv)])
     return 10. ** (A / -2.5)
 
 
 @total_ordering
 class Filter:
     """
     A broadband photometric filter described by its transmission function and its associated photometric system
@@ -43,44 +43,45 @@
     names : str, list
         One or more names for the filter. The first name is used by default but other names are recognized.
     color : str, tuple, optional
         The color used when plotting photometry in this filter. Default: black.
     offset : float, optional
         When plotting, offset photometry in this filter by this amount (in magnitudes if plotting magnitudes)
     system : str, optional
-        Photometric system. If one of ``['Gunn', 'ATLAS', 'Gaia', 'MOSFiT']``, magnitudes are assumed to be AB.
-        If ``'Johnson'``, plot markers with a black edge. Otherwise, ignored except for grouping filters in legends.
+        Photometric system. Only used for grouping filters in legends.
     fnu : float, optional
         Zero-point flux for magnitudes in this filter, in W/(m^2 Hz). If ``fnu = None`` and ``system in ['Gunn',
         'ATLAS', 'Gaia', 'MOSFiT']``, assume the AB zero point. Otherwise if ``fnu = None``, converting to flux will raise
         an error.
     filename : str, optional
         Filename containing the transmission function. If none is supplied, converting to flux will raise an error.
     angstrom : bool, optional
         If False (default), the transmission function wavelengths are assumed to be in nanometers. If True, they are
         given in ångströms.
     linecolor : str, tuple, optional
         The line color used when plotting photometry in this filter. Default: same as ``color``.
     textcolor : str, tuple, optional
         The color used when printing the name of this filter. Default: same as ``linecolor``.
+    mec : str, tuple, optional
+        The marker edge color used when plotting photometry in this filter. Default: same as ``linecolor``.
     italics : bool, optional
         Italicize the filter name when used with LaTeX. Default: True.
 
     Attributes
     ----------
     name : str
         The default name of the filter
     names : list
         A list of aliases for the filter
     char : str
         A single-character identifier for the filter
     color : str, tuple
         The color used when plotting photometry in this filter
     linecolor : str, tuple
-        The line color used when plotting photometry in this filter
+        The line and marker edge color used when plotting photometry in this filter
     textcolor : str, tuple
         The color used when printing the name of this filter
     italics : bool
         Italicize the filter name when used with LaTeX
     mec : str, tuple
         The marker edge color used when plotting photometry in this filter
     plotstyle : dict
@@ -110,15 +111,15 @@
         The approximate edges of the filter transmission function (in terahertz), i.e., :math:`ν_0 \\pm Δν`
     """
 
     order = None
     """The names of recognized filters listed in (approximate) decreasing order of effective frequency"""
 
     def __init__(self, names, color='k', offset=0, system=None, fnu=3.631e-23, filename='', angstrom=False,
-                 linecolor=None, textcolor=None, italics=True):
+                 linecolor=None, textcolor=None, mec=None, italics=True):
         if type(names) == list:
             self.name = names[0]
             self.names = names
         else:
             self.name = names
             self.names = [names]
         if len(self.name) == 1:
@@ -134,20 +135,19 @@
             self.linecolor = linecolor
         else:
             self.linecolor = self.color
         if textcolor:
             self.textcolor = textcolor
         else:
             self.textcolor = self.linecolor
-        self.italics = italics
-        self.system = system
-        if self.system in ['Johnson', 'JWST MIRI']:
-            self.mec = 'k'
+        if mec:
+            self.mec = mec
         else:
             self.mec = self.linecolor
+        self.italics = italics
         self.offset = offset
         self.system = system
         self.plotstyle = {'color': self.linecolor, 'mfc': self.color, 'mec': self.mec}
         self.fnu = fnu  # * u.W * u.m**-2 * u.Hz**-1
         if self.fnu is None:
             self.m0 = np.nan
             self.M0 = np.nan
@@ -155,84 +155,139 @@
             self.m0 = 2.5 * np.log10(self.fnu)
             self.M0 = self.m0 + 90.19
         if filename:
             self.filename = resource_filename('lightcurve_fitting', os.path.join('filters', filename))
         else:
             self.filename = ''
         self.angstrom = angstrom
-        self.trans = None
-        self.freq_eff = None
-        self.dfreq = None
-        self.freq_range = None
-        self.wl_eff = None
-        self.dwl = None
-        self.wl_range = None
+        self._trans = None
+        self._freq_eff = None
+        self._dfreq = None
+        self._freq_range = None
+        self._wl_eff = None
+        self._dwl = None
+        self._wl_range = None
 
     def read_curve(self, show=False, force=False):
         """
         Read the transmission function from ``self.filename`` and store it in ``self.trans``
 
         Parameters
         ----------
         show : bool, optional
             If True, also plot the transmission function
         force : bool, optional
             If True, reread the transmission function from ``self.filename`` even if is already stored in ``self.trans``
         """
-        if (self.trans is None or force) and self.filename:
+        if (self._trans is None or force) and self.filename:
             i = Filter.order.index(self.name) / float(len(Filter.order))
-            self.trans = Table.read(self.filename, format='ascii', names=('wl', 'T'))
+            trans = Table.read(self.filename, format='ascii', names=('wl', 'T'))
             if self.angstrom:
-                self.trans['wl'] = self.trans['wl'] / 10.
-            self.trans['wl'].unit = u.nm
-            self.trans.sort('wl')
-            self.trans['T'] /= np.max(self.trans['T'])
-            self.trans['freq'] = (const.c / self.trans['wl']).to(u.THz)
-
-            dwl = np.trapz(self.trans['T'].quantity, self.trans['wl'].quantity)
-            wl_eff = np.trapz(self.trans['T'].quantity * self.trans['wl'].quantity, self.trans['wl'].quantity) / dwl
-            left = self.trans[(self.trans['wl'] < wl_eff.value) & (self.trans['T'] >= 0.1) * (self.trans['T'] <= 0.9)]
-            left.sort('T')
+                trans['wl'] = trans['wl'] / 10.
+            trans['wl'].unit = u.nm
+            trans.sort('wl')
+            trans['T'] /= np.max(trans['T'])
+            trans['freq'] = (const.c / trans['wl']).to(u.THz)
+
+            dwl = np.trapz(trans['T'].quantity, trans['wl'].quantity)
+            wl_eff = np.trapz(trans['T'].quantity * trans['wl'].quantity, trans['wl'].quantity) / dwl
+            wl0_guess = trans[trans['T'] > 0.5]['wl'].min()
+            left = trans[(trans['wl'] <= wl0_guess) & (trans['T'] >= 0.1)]
             wl0 = np.interp(0.5, left['T'], left['wl'])
-            right = self.trans[(self.trans['wl'] > wl_eff.value) & (self.trans['T'] >= 0.1) * (self.trans['T'] <= 0.9)]
-            right.sort('T')
+            wl1_guess = trans[trans['T'] > 0.5]['wl'].max()
+            right = trans[(trans['wl'] >= wl1_guess) & (trans['T'] >= 0.1)][::-1]  # must be increasing
             wl1 = np.interp(0.5, right['T'], right['wl'])
             if show:
                 plt.figure(1)
                 ax1 = plt.gca()
-                ax1.plot(self.trans['wl'], self.trans['T'], self.color if self.color != 'w' else 'k',
-                         label=self.system + ' ' + self.name)
+                ax1.plot(trans['wl'], trans['T'], self.linecolor, label=self.name)
                 ax1.errorbar(wl_eff.value, i, xerr=[[wl_eff.value - wl0], [wl1 - wl_eff.value]], marker='o',
                              **self.plotstyle)
                 ax1.set_xlabel('Wavelength (nm)')
                 ax1.set_ylabel('Transmission')
 
-            dfreq = np.trapz(self.trans['T'].quantity, self.trans['freq'].quantity)
-            freq_eff = np.trapz(self.trans['T'].quantity * self.trans['freq'].quantity,
-                                self.trans['freq'].quantity) / dfreq
+            dfreq = np.trapz(trans['T'].quantity, trans['freq'].quantity)
+            freq_eff = np.trapz(trans['T'].quantity * trans['freq'].quantity,
+                                trans['freq'].quantity) / dfreq
             freq0 = np.interp(0.5, right['T'], right['freq'])
             freq1 = np.interp(0.5, left['T'], left['freq'])
-            T_per_freq = self.trans['T'].quantity / self.trans['freq'].quantity
-            self.trans['T_norm_per_freq'] = (T_per_freq / np.trapz(T_per_freq, self.trans['freq'].quantity))
+            T_per_freq = trans['T'].quantity / trans['freq'].quantity
+            trans['T_norm_per_freq'] = (T_per_freq / np.trapz(T_per_freq, trans['freq'].quantity))
             if show:
                 plt.figure(2)
                 ax2 = plt.gca()
-                ax2.plot(self.trans['freq'], self.trans['T'], self.color if self.color != 'w' else 'k',
-                         label=self.system + ' ' + self.name)
+                ax2.plot(trans['freq'], trans['T'], self.linecolor, label=self.name)
                 ax2.errorbar(freq_eff.value, i, xerr=[[freq_eff.value - freq0], [freq1 - freq_eff.value]], marker='o',
                              **self.plotstyle)
                 ax2.set_xlabel('Frequency (THz)')
                 ax2.set_ylabel('Transmission')
 
-            self.wl_eff = wl_eff
-            self.dwl = dwl
-            self.wl_range = (wl_eff.value - wl0, wl1 - wl_eff.value)
-            self.freq_eff = freq_eff
-            self.dfreq = -dfreq
-            self.freq_range = (freq_eff.value - freq0, freq1 - freq_eff.value)
+            self._trans = trans
+            self._wl_eff = wl_eff
+            self._dwl = dwl
+            self._wl_range = (wl_eff.value - wl0, wl1 - wl_eff.value)
+            self._freq_eff = freq_eff
+            self._dfreq = -dfreq
+            self._freq_range = (freq_eff.value - freq0, freq1 - freq_eff.value)
+
+    @property
+    def trans(self):
+        self.read_curve()
+        return self._trans
+
+    @property
+    def wl_eff(self):
+        self.read_curve()
+        return self._wl_eff
+
+    @property
+    def dwl(self):
+        self.read_curve()
+        return self._dwl
+
+    @property
+    def wl_range(self):
+        self.read_curve()
+        return self._wl_range
+
+    @property
+    def freq_eff(self):
+        self.read_curve()
+        return self._freq_eff
+
+    @property
+    def dfreq(self):
+        self.read_curve()
+        return self._dfreq
+
+    @property
+    def freq_range(self):
+        self.read_curve()
+        return self._freq_range
+
+    def extinction(self, ebv, rv=3.1, z=0.):
+        """
+        Extinction :math:`A_\lambda` at the effective wavelength of this filter
+
+        Parameters
+        ----------
+        ebv : array-like
+            Selective extinction :math:`E(B-V)` in magnitudes
+        rv : float, optional
+            Ratio of total to selective extinction :math:`R_V`. Default: 3.1.
+        z : float, optional
+            Redshift between the dust and the observed filter. Default: 0 (appropriate for Milky Way extinction).
+
+        Returns
+        -------
+        extinction : float
+            Extinction at the effective wavelength of this filter in magnitudes
+        """
+        if self.wl_eff is not None:
+            return fitzpatrick99(np.array([self.wl_eff.to(u.angstrom).value / (1. + z)]), ebv * rv, rv)[0]
 
     def synthesize(self, spectrum, *args, z=0., ebv=0., **kwargs):
         """
         Returns the average Lnu of the given spectrum in this filter
 
         Parameters
         ----------
@@ -313,66 +368,69 @@
 #  * Table 1 of https://heasarc.gsfc.nasa.gov/docs/heasarc/caldb/swift/docs/uvot/uvot_caldb_AB_10wa.pdf for Swift
 all_filters = [
     Filter('FUV', 'b', 8, 'GALEX', filename='GALEX_GALEX.FUV.dat', angstrom=True),
     Filter('NUV', 'r', 8, 'GALEX', filename='GALEX_GALEX.NUV.dat', angstrom=True),
     Filter(['UVW2', 'uvw2', 'W2', '2', 'uw2'], '#FF007F', 8, 'Swift', 7.379e-24, 'Swift_UVOT.UVW2.dat', angstrom=True),
     Filter(['UVM2', 'uvm2', 'M2', 'M', 'um2'], 'm', 8, 'Swift', 7.656e-24, 'Swift_UVOT.UVM2.dat', angstrom=True),
     Filter(['UVW1', 'uvw1', 'W1', '1', 'uw1'], '#7F00FF', 4, 'Swift', 9.036e-24, 'Swift_UVOT.UVW1.dat', angstrom=True),
-    Filter(['u', "u'", 'up'], '#4700CC', 3, 'Gunn', filename='SLOAN_SDSS.u.dat', angstrom=True),  # brightened from '#080017'
+    Filter(['u', "u'", 'up', 'uprime'], '#4700CC', 3, 'Gunn', filename='SLOAN_SDSS.u.dat', angstrom=True),  # brightened from '#080017'
     Filter(['U_S', 's', 'us'], '#230047', 3, 'Swift', 1.419e-23, filename='Swift_UVOT.U.dat', angstrom=True),
-    Filter('U', '#3C0072', 3, 'Johnson', 1.790e-23, filename='Generic_Johnson.U.dat', angstrom=True),
-    Filter('B', '#0057FF', 2, 'Johnson', 4.063e-23, filename='Generic_Johnson.B.dat', angstrom=True),
+    Filter('U', '#3C0072', 3, 'Johnson', 1.790e-23, filename='Generic_Johnson.U.dat', angstrom=True, mec='k'),
+    Filter('B', '#0057FF', 2, 'Johnson', 4.063e-23, filename='Generic_Johnson.B.dat', angstrom=True, mec='k'),
     Filter(['B_S', 'b', 'bs'], '#4B00FF', 2, 'Swift', 4.093e-23, filename='Swift_UVOT.B.dat', angstrom=True),
-    Filter(['g', "g'", 'gp', 'F475W'], '#00CCFF', 1, 'Gunn', filename='SLOAN_SDSS.g.dat', angstrom=True),
+    Filter(['g', "g'", 'gp', 'gprime', 'F475W'], '#00CCFF', 1, 'Gunn', filename='SLOAN_SDSS.g.dat', angstrom=True),
     Filter('g-DECam', '#00CCFF', 1, 'DECam', filename='CTIO_DECam.g.dat', angstrom=True),
     Filter(['c', 'cyan'], 'c', 1, 'ATLAS', filename='ATLAS_cyan.txt'),
-    Filter('V', '#79FF00', 1, 'Johnson', 3.636e-23, filename='Generic_Johnson.V.dat', angstrom=True, textcolor='#46CC00'),
+    Filter('V', '#79FF00', 1, 'Johnson', 3.636e-23, filename='Generic_Johnson.V.dat', angstrom=True, mec='k', textcolor='#46CC00'),
     Filter(['V_S', 'v', 'vs'], '#00FF30', 1, 'Swift', 3.664e-23, filename='Swift_UVOT.V.dat', angstrom=True),
     Filter('Itagaki', 'w', 0, 'Itagaki', filename='KAF-1001E.asci', linecolor='k', italics=False),
     Filter('white', 'w', 0, 'MOSFiT', filename='white.txt', linecolor='k', italics=False),
-    Filter(['unfilt.', '0', 'Clear', 'C', 'clear', 'pseudobolometric', 'griz'], 'w', 0, 'MOSFiT',
+    Filter(['unfilt.', '0', 'C', 'clear', 'pseudobolometric', 'griz'], 'w', 0, 'MOSFiT',
            filename='pseudobolometric.txt', linecolor='k', italics=False),
     Filter('G', 'w', 0, 'Gaia', filename='GAIA_GAIA0.G.dat', angstrom=True, linecolor='k'),
     Filter('Kepler', 'r', 0, 'Kepler', filename='Kepler_Kepler.K.dat', angstrom=True, italics=False),
     Filter('TESS', 'r', 0, 'TESS', filename='TESS_TESS.Red.dat', angstrom=True, italics=False),
-    Filter('DLT40', 'w', 0, 'DLT40', filename='QE_E2V_MBBBUV_Broadband.csv', linecolor='k', italics=False),
+    Filter(['DLT40', 'Open', 'Clear'], 'w', 0, 'DLT40', filename='QE_E2V_MBBBUV_Broadband.csv', linecolor='k', italics=False),
     Filter('w', 'w', 0, 'Gunn', filename='PAN-STARRS_PS1.w.dat', angstrom=True, linecolor='k'),
     Filter(['o', 'orange'], 'orange', 0, 'ATLAS', filename='ATLAS_orange.txt'),
-    Filter(['r', "r'", 'rp', 'F625W'], '#FF7D00', 0, 'Gunn', filename='SLOAN_SDSS.r.dat', angstrom=True),
+    Filter(['r', "r'", 'rp', 'rprime', 'F625W'], '#FF7D00', 0, 'Gunn', filename='SLOAN_SDSS.r.dat', angstrom=True),
     Filter('r-DECam', '#FF7D00', 0, 'DECam', filename='CTIO_DECam.r.dat', angstrom=True),
-    Filter(['R', 'Rc', 'R_s'], '#FF7000', 0, 'Johnson', 3.064e-23, filename='Generic_Cousins.R.dat', angstrom=True),  # '#CC5900'
-    Filter(['i', "i'", 'ip', 'F775W'], '#90002C', -1, 'Gunn', filename='SLOAN_SDSS.i.dat', angstrom=True),
+    Filter(['R', 'Rc', 'R_s'], '#FF7000', 0, 'Johnson', 3.064e-23, filename='Generic_Cousins.R.dat', mec='k', angstrom=True),  # '#CC5900'
+    Filter(['i', "i'", 'ip', 'iprime', 'F775W'], '#90002C', -1, 'Gunn', filename='SLOAN_SDSS.i.dat', angstrom=True),
     Filter('i-DECam', '#90002C', -1, 'DECam', filename='CTIO_DECam.i.dat', angstrom=True),
-    Filter(['I', 'Ic'], '#66000B', -1, 'Johnson', 2.416e-23, filename='Generic_Cousins.I.dat', angstrom=True),  # brightened from '#1C0003'
+    Filter(['I', 'Ic'], '#66000B', -1, 'Johnson', 2.416e-23, filename='Generic_Cousins.I.dat', mec='k', angstrom=True),  # brightened from '#1C0003'
     Filter('zs', '#000000', -2, 'Gunn', filename='PAN-STARRS_PS1.z.dat', angstrom=True),
-    Filter(['z', "z'", 'zp'], '#000000', -2, 'Gunn', filename='SLOAN_SDSS.z.dat', angstrom=True),
+    Filter(['z', "z'", 'zp', 'zprime'], '#000000', -2, 'Gunn', filename='SLOAN_SDSS.z.dat', angstrom=True),
     Filter('z-DECam', '#000000', -2, 'DECam', filename='CTIO_DECam.z.dat', angstrom=True),
     Filter('y', 'y', -3, 'Gunn', filename='PAN-STARRS_PS1.y.dat', angstrom=True),
     Filter('y-DECam', 'y', -3, 'DECam', filename='CTIO_DECam.Y.dat', angstrom=True),
     Filter('J', '#444444', -2, 'UKIRT', 1.589e-23, filename='Gemini_Flamingos2.J.dat', angstrom=True),
     Filter('H', '#888888', -3, 'UKIRT', 1.021e-23, filename='Gemini_Flamingos2.H.dat', angstrom=True),
     Filter(['K', 'Ks'], '#CCCCCC', -4, 'UKIRT', 0.640e-23, filename='Gemini_Flamingos2.Ks.dat', angstrom=True),
     Filter('L', 'r', -4, 'UKIRT', 0.285e-23),
     # JWST
     Filter('F070W', 'C7', 0, 'JWST NIRCam', filename='JWST_NIRCam.F070W.dat', angstrom=True, italics=False),
     Filter('F090W', 'C0', 0, 'JWST NIRCam', filename='JWST_NIRCam.F090W.dat', angstrom=True, italics=False),
     Filter('F115W', 'C8', 0, 'JWST NIRCam', filename='JWST_NIRCam.F115W.dat', angstrom=True, italics=False),
     Filter('F150W', 'C1', 0, 'JWST NIRCam', filename='JWST_NIRCam.F150W.dat', angstrom=True, italics=False),
     Filter('F200W', 'C2', 0, 'JWST NIRCam', filename='JWST_NIRCam.F200W.dat', angstrom=True, italics=False),
     Filter('F277W', 'C3', 0, 'JWST NIRCam', filename='JWST_NIRCam.F277W.dat', angstrom=True, italics=False),
+    Filter('F300M', 'maroon', 0, 'JWST NIRCam', filename='JWST_NIRCam.F300M.dat', angstrom=True, italics=False),
+    Filter('F335M', 'salmon', 0, 'JWST NIRCam', filename='JWST_NIRCam.F335M.dat', angstrom=True, italics=False),
     Filter('F356W', 'C4', 0, 'JWST NIRCam', filename='JWST_NIRCam.F356W.dat', angstrom=True, italics=False),
+    Filter('F360M', 'crimson', 0, 'JWST NIRCam', filename='JWST_NIRCam.F360M.dat', angstrom=True, italics=False),
     Filter('F444W', 'C5', 0, 'JWST NIRCam', filename='JWST_NIRCam.F444W.dat', angstrom=True, italics=False),
-    Filter('F560W', 'C9', 0, 'JWST MIRI', filename='JWST_MIRI.F560W.dat', angstrom=True, italics=False),
-    Filter('F770W', 'C6', 0, 'JWST MIRI', filename='JWST_MIRI.F770W.dat', angstrom=True, italics=False),
-    Filter('F1000W', 'C7', 0, 'JWST MIRI', filename='JWST_MIRI.F1000W.dat', angstrom=True, italics=False),
-    Filter('F1130W', 'C0', 0, 'JWST MIRI', filename='JWST_MIRI.F1130W.dat', angstrom=True, italics=False),
-    Filter('F1280W', 'C8', 0, 'JWST MIRI', filename='JWST_MIRI.F1280W.dat', angstrom=True, italics=False),
-    Filter('F1500W', 'C1', 0, 'JWST MIRI', filename='JWST_MIRI.F1500W.dat', angstrom=True, italics=False),
-    Filter('F1800W', 'C9', 0, 'JWST MIRI', filename='JWST_MIRI.F1800W.dat', angstrom=True, italics=False),
-    Filter('F2100W', 'C2', 0, 'JWST MIRI', filename='JWST_MIRI.F2100W.dat', angstrom=True, italics=False),
-    Filter('F2550W', 'C3', 0, 'JWST MIRI', filename='JWST_MIRI.F2550W.dat', angstrom=True, italics=False),
+    Filter('F560W', 'C9', 0, 'JWST MIRI', filename='JWST_MIRI.F560W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F770W', 'C6', 0, 'JWST MIRI', filename='JWST_MIRI.F770W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F1000W', 'C7', 0, 'JWST MIRI', filename='JWST_MIRI.F1000W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F1130W', 'C0', 0, 'JWST MIRI', filename='JWST_MIRI.F1130W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F1280W', 'C8', 0, 'JWST MIRI', filename='JWST_MIRI.F1280W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F1500W', 'C1', 0, 'JWST MIRI', filename='JWST_MIRI.F1500W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F1800W', 'C9', 0, 'JWST MIRI', filename='JWST_MIRI.F1800W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F2100W', 'C2', 0, 'JWST MIRI', filename='JWST_MIRI.F2100W.dat', angstrom=True, mec='k', italics=False),
+    Filter('F2550W', 'C3', 0, 'JWST MIRI', filename='JWST_MIRI.F2550W.dat', angstrom=True, mec='k', italics=False),
     Filter(['unknown', '?'], 'w', 0, 'unknown', linecolor='k', italics=False)]
 Filter.order = [f.name for f in all_filters]
 filtdict = {}
 for filt in all_filters:
     for name in filt.names:
         filtdict[name] = filt
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/fitting.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/fitting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import astropy.units as u
 import emcee
 import corner
-from .models import CompanionShocking, CompanionShocking2, scale_sifto, UniformPrior
+from .models import UniformPrior, CompanionShocking, BaseCompanionShocking
+from .lightcurve import filter_legend, flux2mag
+from .filters import filtdict
 from pkg_resources import resource_filename
 import warnings
 
 PRIOR_WARNING = 'The p_max/p_min keywords are deprecated. Use the priors keyword instead.'
+MODEL_KWARGS_WARNING = 'The model_kwargs keyword is deprecated. These are now included in the model intialization.'
 
 
 def lightcurve_mcmc(lc, model, priors=None, p_min=None, p_max=None, p_lo=None, p_up=None,
                     nwalkers=100, nsteps=1000, nsteps_burnin=1000, model_kwargs=None,
                     show=False, save_plot_as='', save_sampler_as='', use_sigma=False, sigma_type='relative'):
     """
     Fit an analytical model to observed photometry using a Markov-chain Monte Carlo routine
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
-        Table of broadband photometry including columns "MJD", "mag", "dmag", "filt"
+        Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
     model : lightcurve_fitting.models.Model
         The model to fit to the light curve. Available models: :class:`.models.ShockCooling`,
         :class:`.models.ShockCooling2`, :class:`.models.ShockCooling3`, :class:`.models.CompanionShocking`,
-        :class:`.models.CompanionShocking2`
+        :class:`.models.CompanionShocking2`, :class:`.models.CompanionShocking3`
     priors : list, optional
         Prior probability distributions for each model parameter. Available priors:
         :class:`.models.UniformPrior` (default), :class:`.models.LogUniformPrior`, :class:`.models.GaussianPrior`
     p_min, p_max : list, optional
         DEPRECATED: Use `priors` instead
     p_lo : list
         Lower bounds on the starting guesses for each paramter
@@ -36,15 +39,15 @@
     nwalkers : int, optional
         Number of walkers (chains) for the MCMC routine. Default: 100
     nsteps : int, optional
         Number of steps (iterations) for the MCMC routine, excluding burn-in. Default: 1000
     nsteps_burnin : int, optional
         Number of steps (iterations) for the MCMC routine during burn-in. Default: 1000
     model_kwargs : dict, optional
-        Keyword arguments to be passed to the model
+        DEPRECATED: Keyword arguments are now included in the model initialization
     show : bool, optional
         If True, plot and display the chain histories
     save_plot_as : str, optional
         Save a plot of the chain histories to this filename
     save_sampler_as : str, optional
         Save the aggregated chain histories to this filename
     use_sigma : bool, optional
@@ -55,35 +58,28 @@
 
     Returns
     -------
     sampler : emcee.EnsembleSampler
         EnsembleSampler object containing the results of the fit
     """
 
-    if model_kwargs is None:
-        model_kwargs = {}
+    if model_kwargs is not None:
+        raise Exception(MODEL_KWARGS_WARNING)
 
     if model.output_quantity == 'flux':
         lc.calcFlux()
     elif model.output_quantity == 'lum':
         lc.calcAbsMag()
         lc.calcLum()
 
-    f = lc['filter'].data
-    t = lc['MJD'].data
-    y = lc[model.output_quantity].data
-    dy = lc['d'+model.output_quantity].data
+    if use_sigma and model.input_names[-1] != '\\sigma':
+        model.input_names.append('\\sigma')
+        model.units.append(u.dimensionless_unscaled)
 
-    if model in [CompanionShocking, CompanionShocking2]:
-        scale_sifto(lc)
-
-    if use_sigma:
-        model.axis_labels.append('$\\sigma$')
-
-    ndim = model.nparams + use_sigma
+    ndim = model.nparams
 
     # DEPRECATED
     if p_min is None:
         p_min = np.tile(-np.inf, ndim)
     elif len(p_min) == ndim:
         p_min = np.array(p_min, float)
         warnings.warn(PRIOR_WARNING)
@@ -118,30 +114,21 @@
 
     for param, prior, p0, p1 in zip(model.input_names, priors, p_lo, p_up):
         if p0 < prior.p_min:
             raise Exception(f'starting guess for {param} (p_lo = {p0}) is outside prior (p_min = {prior.p_min})')
         if p1 > prior.p_max:
             raise Exception(f'starting guess for {param} (p_up = {p1}) is outside prior (p_max = {prior.p_max})')
 
-    if sigma_type == 'relative':
-        sigma_units = dy
-    elif sigma_type == 'absolute':
-        sigma_units = np.median(dy)
-    else:
-        raise Exception('sigma_type must either be "relative" or "absolute"')
-
     def log_posterior(p):
         log_prior = 0.
         for prior, p_i in zip(priors, p):
             log_prior += prior(p_i)
         if np.isinf(log_prior):
             return log_prior
-        y_fit = model(t, f, *p, **model_kwargs)
-        sigma = np.sqrt(dy ** 2. + (p[-1] * sigma_units) ** 2.) if use_sigma else dy
-        log_likelihood = -0.5 * np.sum(np.log(2 * np.pi * sigma ** 2.) + ((y - y_fit) / sigma) ** 2.)
+        log_likelihood = model.log_likelihood(lc, p, use_sigma=use_sigma, sigma_type=sigma_type)
         return log_prior + log_likelihood
 
     sampler = emcee.EnsembleSampler(nwalkers, ndim, log_posterior)
 
     starting_guesses = np.random.rand(nwalkers, ndim) * (p_up - p_lo) + p_lo
     pos, _, _ = sampler.run_mcmc(starting_guesses, nsteps_burnin, progress=True, progress_kwargs={'desc': ' Burn-in'})
 
@@ -179,176 +166,218 @@
             plt.show()
 
     return sampler
 
 
 def lightcurve_corner(lc, model, sampler_flatchain, model_kwargs=None,
                       num_models_to_plot=100, lcaxis_posn=(0.7, 0.55, 0.2, 0.4),
-                      filter_spacing=0.5, tmin=None, tmax=None, t0_offset=None, save_plot_as='', ycol=None,
-                      textsize='medium', param_textsize='large'):
+                      filter_spacing=1., tmin=None, tmax=None, t0_offset=None, save_plot_as='', ycol=None,
+                      textsize='medium', param_textsize='large', use_sigma=False, xscale='linear'):
     """
     Plot the posterior distributions in a corner (pair) plot, with an inset showing the observed and model light curves.
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
-        Table of broadband photometry including columns "MJD", "mag", "dmag", "filt"
+        Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
     model : lightcurve_fitting.models.Model
         The model that was fit to the light curve.
     sampler_flatchain : array-like
         2D array containing the aggregated MCMC chain histories
     model_kwargs : dict, optional
-        Keyword arguments to be passed to the model
+        DEPRECATED: Keyword arguments are now included in the model initialization
     num_models_to_plot : int, optional
         Number of model realizations to plot in the light curve inset. Default: 100
     lcaxis_posn : tuple, optional
         Light curve inset position and size specification in figure units: (left, bottom, width, height)
     filter_spacing : float, optional
         Spacing between filters in the light curve inset, in units determined by the order of magnitude of the
-        luminosities. Default: 0.5
+        luminosities. Default: 1.
     tmin, tmax : float, optional
         Starting and ending times for which to plot the models in the light curve inset. Default: determined by the
         time range of the observed light curve.
     t0_offset : float, optional
         Reference time for the explosion time in the corner plot. Default: the earliest explosion time in
         `sampler_flatchain`, rounded down.
     save_plot_as : str, optional
         Filename to which to save the resulting plot
     ycol : str, optional
         Quantity to plot on the light curve inset. Choices: "lum", "flux", or "absmag". Default: model.output_quantity
     textsize : str, optional
         Font size for the x- and y-axis labels, as well as the tick labels. Default: 'medium'
     param_textsize : str, optional
         Font size for the parameter text. Default: 'large'
+    use_sigma : bool, optional
+        If True, treat the last parameter as an intrinsic scatter parameter that does not get passed to the model
+    xscale : str, optional
+        Scale for the x-axis of the model plot. Choices: "linear" (default) or "log".
 
     Returns
     -------
     fig : matplotlib.pyplot.Figure
         Figure object containing the plot
     corner_ax : array-like
         Array of matplotlib.pyplot.Axes objects corresponding to the corner plot
     ax : matplotlib.pyplot.Axes
         Axes object for the light curve inset
     """
-    if model_kwargs is None:
-        model_kwargs = {}
+    if model_kwargs is not None:
+        raise Exception(MODEL_KWARGS_WARNING)
     if ycol is None:
         ycol = model.output_quantity
     plt.style.use(resource_filename('lightcurve_fitting', 'serif.mplstyle'))
 
     sampler_flatchain_corner = sampler_flatchain.copy()
-    if 't_0' in model.input_names:
-        i_t0 = model.input_names.index('t_0')
-        if t0_offset is None:
-            t0_offset = np.floor(sampler_flatchain_corner[:, i_t0].min())
-        if t0_offset != 0.:
-            sampler_flatchain_corner[:, i_t0] -= t0_offset
-            model.axis_labels[i_t0] = '$t_0 - {:.0f}$ (d)'.format(t0_offset)
+    axis_labels_corner = model.axis_labels
+    for var in ['t_0', 't_\\mathrm{max}']:
+        if var in model.input_names:
+            i_t0 = model.input_names.index(var)
+            if t0_offset is None:
+                mjd_offset = np.floor(sampler_flatchain_corner[:, i_t0].min())
+            else:
+                mjd_offset = t0_offset
+            if mjd_offset != 0.:
+                sampler_flatchain_corner[:, i_t0] -= mjd_offset
+                axis_labels_corner[i_t0] = f'${var} - {mjd_offset:.0f}$ (d)'
 
-    fig = corner.corner(sampler_flatchain_corner, labels=model.axis_labels, label_kwargs={'size': textsize})
+    fig = corner.corner(sampler_flatchain_corner, labels=axis_labels_corner, label_kwargs={'size': textsize})
     corner_axes = np.array(fig.get_axes()).reshape(sampler_flatchain.shape[-1], sampler_flatchain.shape[-1])
     for i in range(sampler_flatchain.shape[-1]):
         corner_axes[i, 0].tick_params(labelsize=textsize)
         corner_axes[-1, i].tick_params(labelsize=textsize)
 
     for ax in np.diag(corner_axes):
         ax.spines['top'].set_visible(False)
         ax.spines['left'].set_visible(False)
         ax.spines['right'].set_visible(False)
         ax.xaxis.set_ticks_position('bottom')
         ax.yaxis.set_ticks_position('none')
 
     ax = fig.add_axes(lcaxis_posn)
     lightcurve_model_plot(lc, model, sampler_flatchain, model_kwargs, num_models_to_plot, filter_spacing,
-                          tmin, tmax, ycol, textsize, ax)
+                          tmin, tmax, ycol, textsize, ax, use_sigma=use_sigma, xscale=xscale)
 
     paramtexts = format_credible_interval(sampler_flatchain, varnames=model.input_names, units=model.units)
     fig.text(0.45, 0.95, '\n'.join(paramtexts), va='top', ha='center', fontdict={'size': param_textsize})
     if save_plot_as:
         fig.savefig(save_plot_as)
         print('saving figure as ' + save_plot_as)
 
     return fig, corner_axes, ax
 
 
-def lightcurve_model_plot(lc, model, sampler_flatchain, model_kwargs=None, num_models_to_plot=100, filter_spacing=0.5,
-                          tmin=None, tmax=None, ycol=None, textsize='medium', ax=None, mjd_offset=None):
+def lightcurve_model_plot(lc, model, sampler_flatchain, model_kwargs=None, num_models_to_plot=100, filter_spacing=1.,
+                          tmin=None, tmax=None, ycol=None, textsize='medium', ax=None, mjd_offset=None, use_sigma=False,
+                          xscale='linear'):
     """
     Plot the observed and model light curves.
 
     Parameters
     ----------
     lc : lightcurve_fitting.lightcurve.LC
-        Table of broadband photometry including columns "MJD", "mag", "dmag", "filt"
+        Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
     model : lightcurve_fitting.models.Model
         The model that was fit to the light curve.
     sampler_flatchain : array-like
         2D array containing the aggregated MCMC chain histories
     model_kwargs : dict, optional
-        Keyword arguments to be passed to the model
+        DEPRECATED: Keyword arguments are now included in the model initialization.
     num_models_to_plot : int, optional
         Number of model realizations to plot in the light curve inset. Default: 100
     filter_spacing : float, optional
         Spacing between filters in the light curve inset, in units determined by the order of magnitude of the
-        luminosities. Default: 0.5
+        luminosities. Default: 1.
     tmin, tmax : float, optional
         Starting and ending times for which to plot the models in the light curve inset. Default: determined by the
         time range of the observed light curve.
     ycol : str, optional
         Quantity to plot on the light curve inset. Choices: "lum", "flux", or "absmag". Default: model.output_quantity
     textsize : str, optional
         Font size for the x- and y-axis labels, as well as the tick labels. Default: 'medium'
     ax : matplotlib.pyplot.Axes
         Axis on which to plot the light curves
     mjd_offset : float, optional
         Reference time on the horizontal axis of the light curve inset. Default: determined by the starting time of
         the model light curve.
+    use_sigma : bool, optional
+        If True, treat the last parameter as an intrinsic scatter parameter that does not get passed to the model
+    xscale : str, optional
+        Scale for the x-axis. Choices: "linear" (default) or "log".
     """
+    if model_kwargs is not None:
+        raise Exception(MODEL_KWARGS_WARNING)
+    if ycol is None:
+        ycol = model.output_quantity
     if ax is None:
         ax = plt.axes()
 
     choices = np.random.choice(sampler_flatchain.shape[0], num_models_to_plot)
     ps = sampler_flatchain[choices].T
 
     if tmin is None:
         tmin = np.min(lc['MJD'])
     if tmax is None:
         tmax = np.max(lc['MJD'])
-    xfit = np.arange(tmin, tmax, 0.1)
+    xfit = np.geomspace(tmin, tmax, 1000) if xscale == 'log' else np.linspace(tmin, tmax, 1000)
     ufilts = np.unique(lc['filter'])
-    y_fit = model(xfit, ufilts, *ps, **model_kwargs)
+    if use_sigma:
+        y_fit = model(xfit, ufilts, *ps[:-1])
+    else:
+        y_fit = model(xfit, ufilts, *ps)
+
+    # for CompanionShocking, add SiFTO model as dashed lines
+    if isinstance(model, CompanionShocking):
+        y_fit1 = model.stretched_sifto(xfit, ufilts, *ps[3:5])
+        y_fit1[ufilts == filtdict['r']] *= ps[5]
+        y_fit1[ufilts == filtdict['i']] *= ps[6]
+    elif isinstance(model, BaseCompanionShocking):
+        y_fit1 = model.stretched_sifto(xfit, ufilts, *ps[3:7])
+    else:
+        y_fit1 = [None] * len(ufilts)
 
     if mjd_offset is None:
         mjd_offset = np.floor(tmin)
     if ycol == 'lum':
         dycol = 'dlum'
         yscale = 10. ** np.round(np.log10(y_fit.max()))
         ylabel = 'Luminosity $L_\\nu$ (10$^{{{:.0f}}}$ erg s$^{{-1}}$ Hz$^{{-1}}$) + Offset'.format(
             np.log10(yscale) + 7)  # W --> erg / s
     elif ycol == 'absmag':
         dycol = 'dmag'
         yscale = 1.
         ylabel = 'Absolute Magnitude + Offset'
-        y_fit = [[[filt.M0]] for filt in ufilts] - 2.5 * np.log10(y_fit)
+        y_fit, _ = flux2mag(y_fit, zp=[[[filt.M0]] for filt in ufilts])
+        if y_fit1[0] is not None:
+            y_fit1, _ = flux2mag(y_fit1, zp=[[[filt.M0]] for filt in ufilts])
         ax.invert_yaxis()
     elif ycol == 'flux':
         dycol = 'dflux'
         yscale = 10. ** np.round(np.log10(y_fit.max()))
         ylabel = 'Flux $F_\\nu$ (10$^{{{:.0f}}}$ erg s$^{{-1}}$ m$^{{-2}}$ Hz$^{{-1}}$) + Offset'.format(
             np.log10(yscale) + 7)  # W --> erg / s
     else:
         raise ValueError(f'ycol="{ycol}" is not recognized. Use "lum", "absmag", "flux".')
-    offset = -len(ufilts) // 2 * filter_spacing
-    for filt, yfit in zip(ufilts, y_fit):
-        offset += filter_spacing
-        lc_filt = lc.where(filter=filt)
-        ax.errorbar(lc_filt['MJD'] - mjd_offset, lc_filt[ycol] / yscale + offset, lc_filt[dycol] / yscale,
-                    ls='none', marker='o', **filt.plotstyle)
+
+    if xscale == 'log':
+        ax.set_xscale('log')
+        ax.xaxis.set_major_formatter(plt.FormatStrFormatter('%g'))
+        lc = lc.where(MJD_min=mjd_offset)
+    else:
+        lc = lc.copy()
+    lc['MJD'] -= mjd_offset
+    lc[ycol] /= yscale
+    lc[dycol] /= yscale
+    lc.plot(xcol='MJD', ycol=ycol, offset_factor=filter_spacing, appmag_axis=False, tight_layout=False)
+    plt.autoscale(False)
+    _, labels, _ = filter_legend(np.array(ufilts), filter_spacing)
+    for yfit, yfit1, filt, txt in zip(y_fit, y_fit1, ufilts, labels):
+        offset = -filt.offset * filter_spacing
         ax.plot(xfit - mjd_offset, yfit / yscale + offset, color=filt.linecolor, alpha=0.05)
-        txt = f'${filt.name}{offset:+g}$' if filt.italics else rf'$\mathrm{{{filt.name}}}{offset:+g}$'
+        if yfit1 is not None:
+            ax.plot(xfit - mjd_offset, np.median(yfit1, axis=1) / yscale + offset, color=filt.linecolor, ls='--')
         ax.text(1.03, yfit[-1, 0] / yscale + offset, txt, color=filt.textcolor, fontdict={'size': textsize},
                 ha='left', va='center', transform=ax.get_yaxis_transform())
     ax.set_xlabel('MJD $-$ {:f}'.format(mjd_offset).rstrip('0').rstrip('.'), size=textsize)
     ax.set_ylabel(ylabel, size=textsize)
     ax.tick_params(labelsize=textsize)
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/lightcurve.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/lightcurve.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.path import Path
 from astropy.table import Table, vstack, MaskedColumn
+from astropy.cosmology import Planck18
 from .filters import filtdict
 import itertools
 from matplotlib.markers import MarkerStyle
+from matplotlib.patches import Patch
 try:
     from config import markers
 except ModuleNotFoundError:
     markers = {}
 
 
 class Arrow(Path):
@@ -31,15 +33,15 @@
 othermarkers = ('o', *MarkerStyle.filled_markers[2:])
 itermarkers = itertools.cycle(othermarkers)
 usedmarkers = []
 itercolors = itertools.cycle(plt.rcParams['axes.prop_cycle'].by_key()['color'])
 
 # if you edit this list, also add the new names to usage.rst
 column_names = {
-    'Filter': ['filt', 'filter', 'Filter', 'band', 'FLT', 'Band'],
+    'Filter': ['filter', 'filt', 'Filter', 'band', 'FLT', 'Band'],
     'Telescope': ['telescope', 'Telescope', 'Tel', 'tel+inst'],
     'Source': ['source', 'Source'],
     'Apparent Magnitude': ['mag', 'Magnitude', 'Mag', 'ab_mag', 'PSFmag', 'MAG', 'omag', 'magnitude', 'apparent_mag'],
     'Apparent Magnitude Uncertainty': [
         'dmag', 'Magnitude_Error', 'magerr', 'MagErr', 'mag_err', 'e_mag', 'Error', 'err', 'PSFerr', 'MAGERR', 'e_omag',
         'e_magnitude', 'apparent_mag_err', 'Mag_Err', 'emag',
     ],
@@ -58,26 +60,28 @@
 
 class LC(Table):
     """
     A broadband light curve, stored as an :class:`astropy.table.Table`
 
     Attributes
     ----------
-    sn : object
-        Astronomical transient with which this light curve is associated
     nondetSigmas : float
         Significance level implied by nondetections in the light curve. Default: 3σ
     groupby : set
-        Column names to group by when binning the light curve. Default: ``{'filt', 'filter', 'source'}``
+        Column names to group by when binning the light curve. Default: ``{'filter', 'source'}``
+    markers : dict
+        Mapping of some light curve property (default: ``'source'`` or ``'telescope'``) to marker shapes
     """
     def __init__(self, *args, **kwargs):
         Table.__init__(self, *args, **kwargs)
-        self.sn = None
+        self.normalize_column_names()
+        if 'filter' in self.colnames and self['filter'].dtype != object:
+            self.filters_to_objects()
         self.nondetSigmas = 3.
-        self.groupby = {'filt', 'filter', 'source'}
+        self.groupby = {'filter', 'source'}
         self.markers = markers.copy()
 
     def where(self, **kwargs):
         """
         Select the subset of a light curve matching some criteria, given as keyword arguments, e.g., ``colname=value``.
 
         The keyword ``colname`` can be any of the following:
@@ -88,14 +92,19 @@
 
         ``value`` must match the data type of the column ``colname`` and can either be a single value or a list of
         values. If ``value`` is a list, rows must match at least one of the values. If ``value`` is a list and
         ``colname`` ends in ``_not``, rows must not match any of the values.
         """
         use = np.tile(True, len(self))
         for col, val in kwargs.items():
+            if col.startswith('filter'):  # allow constraints like filter='r' so the user does not need to use filtdict
+                if isinstance(val, str):
+                    val = filtdict[val]
+                elif isinstance(val, list):
+                    val = [filtdict[v] if isinstance(v, str) else v for v in val]
             if isinstance(val, list):
                 if '_not' in col:
                     use1 = np.tile(True, len(self))
                     for v in val:
                         use1 &= self[col.replace('_not', '')] != v
                 else:
                     use1 = np.tile(False, len(self))
@@ -113,16 +122,14 @@
             else:
                 if val is None:
                     use1 = np.array([v is None for v in self[col]])
                 else:
                     use1 = self[col] == val
             use &= use1
         selected = self[use]
-        selected.sn = self.sn
-        selected.meta = self.meta
         selected.markers = self.markers
         return selected
 
     def get(self, key, default=None):
         return self[key] if key in self.colnames else default
 
     def normalize_column_names(self):
@@ -138,42 +145,34 @@
         if 'MJD' not in self.colnames and 'JD' in self.colnames:
             self['MJD'] = self['JD'] - 2400000.5
             self.remove_column('JD')
         if 'nondet' in self.colnames and self['nondet'].dtype != bool:
             if isinstance(self['nondet'], MaskedColumn):
                 self['nondet'] = self['nondet'].filled()
             nondet = (self['nondet'] == 'True') | (self['nondet'] == 'T') | (self['nondet'] == '>')
-            self.remove_column('nondet')
-            self['nondet'] = nondet
+            self.replace_column('nondet', nondet)
 
-    def filters_to_objects(self, read_curve=True):
+    def filters_to_objects(self):
         """
-        Parse the ``'filt'`` column into :class:`filters.Filter` objects and store in the ``'filter'`` column
-
-        Parameters
-        ----------
-        read_curve : bool, optional
-            Read in the transmission function for each filter encountered (default)
+        Parse the ``'filter'`` column into :class:`filters.Filter` objects
         """
-        self['filter'] = [filtdict['?'] if np.ma.is_masked(f) or str(f) not in filtdict else filtdict[str(f)]
-                          for f in self['filt']]
+        filters = np.array([filtdict['?'] if np.ma.is_masked(f) or str(f) not in filtdict else filtdict[str(f)]
+                            for f in self['filter']])
         is_swift = np.zeros(len(self), bool)
         if 'telescope' in self.colnames:
             is_swift |= self['telescope'] == 'Swift'
             is_swift |= self['telescope'] == 'UVOT'
             is_swift |= self['telescope'] == 'Swift/UVOT'
             is_swift |= self['telescope'] == 'Swift+UVOT'
         if 'source' in self.colnames:
             is_swift |= self['source'] == 'SOUSA'
         if is_swift.any():
             for filt, swiftfilt in zip('UBV', 'sbv'):
-                self['filter'][is_swift & (self['filt'] == filt)] = filtdict[swiftfilt]
-        if read_curve:
-            for filt in np.unique(self['filter']):
-                filt.read_curve()
+                filters[is_swift & (self['filter'] == filt)] = filtdict[swiftfilt]
+        self.replace_column('filter', filters)
 
     @property
     def zp(self):
         """
         Returns an array of zero points for each filter in the ``'filter'`` column
         """
         return np.array([f.m0 for f in self['filter']])
@@ -200,15 +199,15 @@
         Bin the light curve by averaging points within ``delta`` days of each other
 
         Parameters
         ----------
         delta : float, optional
             Bin size, in days. Default: 0.3 days
         groupby : set, optional
-            Column names to group by before binning. Default: ``{'filt', 'filter', 'source'}``
+            Column names to group by before binning. Default: ``{'filter', 'source'}``
 
         Returns
         -------
         lc : lightcurve_fitting.lightcurve.LC
             Binned light curve
         """
         if groupby is not None:
@@ -222,15 +221,14 @@
         for g, k in zip(grouped.groups, grouped.groups.keys):
             mjd, flux, dflux = binflux(g['MJD'], g['flux'], g['dflux'], delta)
             binned = LC([mjd, flux, dflux], names=['MJD', 'flux', 'dflux'])
             for key in self.groupby:
                 binned[key] = k[key]
             subtabs.append(binned)
         lc = vstack(subtabs)
-        lc.sn = self.sn
         lc.meta = self.meta
         return lc
 
     def findNondet(self, nondetSigmas=None):
         """
         Add a boolean column ``'nondet'`` indicating flux measurements that are below the detection threshold
 
@@ -257,50 +255,74 @@
         if nondetSigmas is not None:
             self.nondetSigmas = nondetSigmas
         self.findNondet()
         if zp is None:
             zp = self.zp
         self['mag'], self['dmag'] = flux2mag(self['flux'], self['dflux'], zp, self.get('nondet'), self.nondetSigmas)
 
-    def calcAbsMag(self, dm=None, extinction=None, hostext=None):
+    def calcAbsMag(self, dm=None, extinction=None, hostext=None, ebv=None, rv=None, host_ebv=None, host_rv=None,
+                   redshift=None):
         """
         Calculate the ``'absmag'`` column from the ``'mag'`` column by correcting for distance and extinction
 
         Parameters
         ----------
         dm : float, optional
-            Distance modulus. Default: use the distance modulus of ``self.sn``, if any. Otherwise do not correct for
-            distance.
+            Distance modulus. Default: calculate from ``redshift``.
         extinction : dict, optional
-            Milky Way extinction coefficients :math:`A_λ` for each filter. Default: use the extinction of ``self.sn``,
-            if any. Otherwise do not correct for Milky Way extinction.
+            Milky Way extinction coefficients :math:`A_λ` for each filter. Default: calculate from ``ebv`` and ``rv``.
         hostext : dict, optional
-            Host galaxy extinction coefficients :math:`A_λ` for each filter. Default: use the extinction of ``self.sn``,
-            if any. Otherwise do not correct for host galaxy extinction.
-        """
+            Host galaxy extinction coefficients :math:`A_λ` for each filter. Default: calculate from ``host_ebv`` and
+            ``host_rv``.
+        ebv : float, optional
+            Milky Way selective extinction :math:`E(B-V)`, used if ``extinction`` is not given. Default: 0.
+        host_ebv : float, optional
+            Host galaxy selective extinction :math:`E(B-V)`, used if ``hostext`` is not given. Default: 0.
+        rv : float, optional
+            Ratio of total to selective Milky Way extinction :math:`R_V`, used with the ``ebv`` argument. Default: 3.1.
+        host_rv : float, optional
+            Ratio of total to selective host-galaxy extinction :math:`R_V`, used with the ``host_ebv`` argument.
+            Default: 3.1.
+        redshift : float, optional
+            Redshift of the host galaxy. Used to redshift the filters for host galaxy extinction. If no distance
+            modulus is given, a redshift-dependent distance is calculated using the Planck18 cosmology. Default: 0.
+        """
+        if redshift is not None:
+            self.meta['redshift'] = redshift
+        elif 'redshift' not in self.meta:
+            self.meta['redshift'] = 0.
+
         if dm is not None:
             self.meta['dm'] = dm
-        elif self.sn is not None:
-            self.meta['dm'] = self.sn.dm
+        elif 'dm' not in self.meta and self.meta.get('redshift'):
+            self.meta['dm'] = Planck18.distmod(self.meta['redshift']).value
+            print('using a redshift-dependent distance modulus')
         elif 'dm' not in self.meta:
             self.meta['dm'] = 0.
 
+        if ebv is None:
+            ebv = self.meta.get('ebv')
+        if host_ebv is None:
+            host_ebv = self.meta.get('host_ebv')
+        if rv is None:
+            rv = self.meta.get('rv', 3.1)
+        if host_rv is None:
+            host_rv = self.meta.get('host_rv', 3.1)
+
         if extinction is not None:
             self.meta['extinction'] = extinction
-        elif self.sn is not None:
-            self.meta['extinction'] = self.sn.extinction
         elif 'extinction' not in self.meta:
-            self.meta['extinction'] = {}
+            self.meta['extinction'] = {f.name: f.extinction(ebv, rv)
+                                       for f in set(self['filter']) if f.wl_eff is not None and ebv is not None}
 
         if hostext is not None:
             self.meta['hostext'] = hostext
-        elif self.sn is not None:
-            self.meta['hostext'] = self.sn.hostext
         elif 'hostext' not in self.meta:
-            self.meta['hostext'] = {}
+            self.meta['hostext'] = {f.name: f.extinction(host_ebv, host_rv, self.meta.get('z', 0.))
+                                    for f in set(self['filter']) if f.wl_eff is not None and host_ebv is not None}
 
         self['absmag'] = self['mag'].data - self.meta['dm']
         for filtobj in set(self['filter']):
             for filt in filtobj.names:
                 if filt in self.meta['extinction']:
                     self['absmag'][self['filter'] == filtobj] -= self.meta['extinction'][filt]
                     break
@@ -325,73 +347,71 @@
         if nondetSigmas is not None:
             self.nondetSigmas = nondetSigmas
         self['lum'], self['dlum'] = mag2flux(self['absmag'], self['dmag'], self.zp + 90.19, self.get('nondet'),
                                              self.nondetSigmas)
 
     def findPeak(self, **criteria):
         """
-        Find the peak of the light curve and store it in ``self.sn.peakdate``
+        Find the peak of the light curve and store it in ``.meta['peakdate']``
 
         Parameters
         ----------
         criteria : dict, optional
             Use only a subset of the light curve matching some criteria when calculating the peak date (stored in
-            ``self.sn.peakcriteria``
+            ``.meta['peakcriteria']``)
         """
         if 'nondet' in self.colnames:
             criteria['nondet'] = False
         peaktable = self.where(**criteria)
         if len(peaktable):
             imin = np.argmin(peaktable['mag'])
             self.meta['peakdate'] = peaktable['MJD'][imin]
+            self.meta['peakcriteria'] = criteria
         else:
-            self.meta['peakdate'] = np.nan
-        if self.sn is not None:
-            self.meta['redshift'] = self.sn.z  # needed for calcPhase
-            self.sn.peakdate = self.meta['peakdate']
-            self.sn.peakcriteria = criteria
+            print(f'no data match these criteria: {criteria}')
 
     def calcPhase(self, rdsp=False, hours=False):
         """
-        Calculate the rest-frame ``'phase'`` column from the ``'MJD'`` column and ``self.sn.refmjd`` and ``self.sn.z``
+        Calculate the rest-frame ``'phase'`` column from ``'MJD'``, ``.meta['refmjd']``, and ``.meta['redshift']``
 
         Parameters
         ----------
         rdsp : bool, optional
             Define phase as rest-frame days since peak, rather than rest-frame days since explosion
+        hours : bool, optional
+            Give the phase in rest-frame hours instead of rest-frame days
         """
-        if 'refmjd' not in self.meta and self.sn is not None:
-            if rdsp and self.sn.peakdate is None:
-                raise Exception('must run sn.findPeak() first')
+        if 'refmjd' not in self.meta:
+            if rdsp and self.meta.get('peakdate') is None:
+                raise Exception('must run lc.findPeak() first')
             elif rdsp:
-                self.sn.refmjd = self.sn.peakdate
-            elif self.sn.explosion is not None:
-                self.sn.refmjd = self.sn.explosion
+                self.meta['refmjd'] = self.meta['peakdate']
+            elif self.meta.get('explosion') is not None:
+                self.meta['refmjd'] = self.meta['explosion']
             else:
                 if 'nondet' in self.colnames:
                     detections = self.where(nondet=False)
                 else:
                     detections = self
-                self.sn.refmjd = np.min(detections['MJD'].data)
-            self.meta['refmjd'] = self.sn.refmjd
-            self.meta['redshift'] = self.sn.z
+                self.meta['refmjd'] = np.min(detections['MJD'].data)
         self['phase'] = (self['MJD'].data - self.meta['refmjd']) / (1 + self.meta['redshift'])
         if 'dMJD0' in self.colnames:
             self['dphase0'] = self['dMJD0'] / (1. + self.meta['redshift'])
         if 'dMJD1' in self.colnames:
             self['dphase1'] = self['dMJD1'] / (1. + self.meta['redshift'])
         if hours:
             self['phase'] *= 24.
             if 'dphase0' in self.colnames:
                 self['dphase0'] *= 24.
             if 'dphase1' in self.colnames:
                 self['dphase1'] *= 24.
 
     def plot(self, xcol='phase', ycol='absmag', offset_factor=1., color='filter', marker=None, use_lines=False,
-             normalize=False, fillmark=True, **kwargs):
+             normalize=False, fillmark=True, mjd_axis=True, appmag_axis=True, loc_mark=None, loc_filt=None, ncol_mark=1,
+             lgd_filters=None, tight_layout=True, **kwargs):
         """
         Plot the light curve, with nondetections marked with a downward-pointing arrow
 
         Parameters
         ----------
         xcol : str, optional
             Column to plot on the horizontal axis. Default: ``'phase'``
@@ -405,15 +425,32 @@
             Column that controls the marker shape. Default: ``'source'`` or ``'telescope'``
         use_lines : bool, optional
             Connect light curve points with lines. Default: False
         normalize : bool, optional
             Normalize all light curves to peak at 0. Default: False
         fillmark : bool, optional
             Fill each marker with color. Default: True
-        kwargs : dict, optional
+        mjd_axis : bool, optional
+            Plot MJD on the upper x-axis. Must have ``.meta['redshift']`` and ``.meta['refmjd']``. Default: True.
+        appmag_axis : bool, optional
+            Plot extinction-corrected apparent magnitude on the right y-axis. Must have ``.meta['dm']``. Default: True.
+        loc_mark, loc_filt : str, optional
+            Location for the marker and filter legends, respectively. Set to 'none' to omit them. Three new options are
+            available: 'above', 'above left', and 'above right'. ``mjd_axis`` and/or ``appmag_axis`` must be used to
+            add these legends. Otherwise run ``plt.legend()`` after plotting for a single simple legend. Default: no
+            legend.
+        ncol_mark : int, optional
+            Number of columns in the marker legend. Default: 1.
+        lgd_filters : list, array-like, optional
+            Customize the arrangement of filters in the legend by providing a list of filters for each column. ``None``
+            can be used to leave a blank space in the column. Only filters given here will be used. The default
+            arrangement shows all filters arranged by ``.system`` (columns) and ``.offset`` (rows).
+        tight_layout : bool, optional
+            Adjust the figure margins to look beautiful. Default: True.
+        kwargs
             Keyword arguments matching column names in the light curve are used to specify a subset of points to plot.
             Additional keyword arguments passed to :func:`matplotlib.pyplot.plot`.
         """
         if xcol.startswith('filter'):
             unit = xcol.split(':')[-1] if ':' in xcol else None
             xcol = 'wl_eff'
             self[xcol] = [f.wl_eff.to(unit) if unit else f.wl_eff for f in self['filter']]
@@ -449,33 +486,30 @@
         if marker in plottable.keys():
             groupby.add(marker)
         if groupby:
             plottable = plottable.group_by(list(groupby))
             keys = plottable.groups.keys
         else:
             keys = [Table()]
-        if self.sn is None:
-            linestyle = plot_kwargs.pop('linestyle') if 'linestyle' in plot_kwargs else None
-            linewidth = plot_kwargs.pop('linewidth') if 'linewidth' in plot_kwargs else None
-        else:
-            linestyle = self.sn.linestyle
-            linewidth = self.sn.linewidth
+        linestyle = plot_kwargs.pop('linestyle', plot_kwargs.pop('ls', self.meta.get('linestyle', self.meta.get('ls'))))
+        linewidth = plot_kwargs.pop('linewidth', plot_kwargs.pop('lw', self.meta.get('linewidth', self.meta.get('lw'))))
+        ms = plot_kwargs.pop('markersize', plot_kwargs.pop('ms', plt.rcParams['lines.markersize']))
         for g, k in zip(plottable.groups, keys):
             filt = g['filter'][0]
             if color == 'filter':
                 col = filt.color
-                mec = 'k' if filt.system == 'Johnson' else filt.linecolor
-            elif color == 'name':
-                col = self.sn.plotcolor
+                mec = filt.mec
+            elif color == 'name' and 'plotcolor' in self.meta:
+                col = self.meta['plotcolor']
                 mec = col if col not in ['w', '#FFFFFF'] else 'k'
             else:
                 col = mec = next(itercolors)
             mfc = col if fillmark else 'none'
-            if marker == 'name':
-                mark = self.sn.marker
+            if marker == 'name' and 'marker' in self.meta:
+                mark = self.meta['marker']
             elif marker in plottable.keys():
                 if g[marker][0] not in self.markers:
                     for nextmarker in othermarkers:
                         if nextmarker not in usedmarkers:
                             self.markers[g[marker][0]] = nextmarker
                             break
                     else:
@@ -493,57 +527,289 @@
             elif 'mag' in ycol:
                 yerr = g['dmag']
             else:
                 yerr = g['d' + ycol]
             x = g[xcol].data
             y = g[ycol].data - filt.offset * offset_factor
             if normalize and ycol == 'mag':
-                y -= self.sn.peakmag
+                if 'peakmag' in self.meta:
+                    y -= self.meta['peakmag']
+                else:
+                    print("must set .meta['peakmag'] to use normalize")
             elif normalize and ycol == 'absmag':
-                y -= self.sn.peakabsmag
+                if 'peakabsmag' in self.meta:
+                    y -= self.meta['peakmag']
+                else:
+                    print("must set .meta['peakabsmag'] to use normalize")
             if 'mag' in ycol and 'nondet' in g.keys() and marker:  # don't plot if no markers used
-                plt.plot(x[g['nondet']], y[g['nondet']], marker=arrow, linestyle='none', ms=25, mec=mec, **plot_kwargs)
+                plt.plot(x[g['nondet']], y[g['nondet']], marker=arrow, linestyle='none', ms=ms / 6. * 25., mec=mec,
+                         **plot_kwargs)
             if 'filter' in k.colnames:
                 if len(filt.name) >= 4 and not filt.offset:
                     k['filter'] = filt.name
                 elif offset_factor:
                     k['filter'] = '${}{:+.0f}$'.format(filt.name, -filt.offset * offset_factor)
                 else:
                     k['filter'] = '${}$'.format(filt.name)
             label = ' '.join([str(kv) for kv in k.values()])
             if not use_lines:
-                plt.errorbar(x, y, yerr, color=mec, mfc=mfc, mec=mec, marker=mark, linestyle='none', label=label,
+                plt.errorbar(x, y, yerr, color=mec, mfc=mfc, mec=mec, ms=ms, marker=mark, linestyle='none', label=label,
                              **plot_kwargs)
             elif 'mag' in ycol and 'nondet' in g.colnames:
-                plt.plot(x[~g['nondet']], y[~g['nondet']], color=col, mfc=mfc, mec=mec, marker=mark, label=label,
+                plt.plot(x[~g['nondet']], y[~g['nondet']], color=col, mfc=mfc, mec=mec, ms=ms, marker=mark, label=label,
                          linestyle=linestyle, linewidth=linewidth, **plot_kwargs)
-                plt.plot(x[g['nondet']], y[g['nondet']], color=mec, mfc=mfc, mec=mec, marker=mark, linestyle='none',
-                         **plot_kwargs)
+                plt.plot(x[g['nondet']], y[g['nondet']], color=mec, mfc=mfc, mec=mec, ms=ms, marker=mark,
+                         linestyle='none', **plot_kwargs)
             else:
-                plt.plot(x, y, color=col, mfc=mfc, mec=mec, marker=mark, label=label, linestyle=linestyle,
+                plt.plot(x, y, color=col, mfc=mfc, mec=mec, ms=ms, marker=mark, label=label, linestyle=linestyle,
                          linewidth=linewidth, **plot_kwargs)
+
+        # format axes
         ymin, ymax = plt.ylim()
         if 'mag' in ycol and ymax > ymin:
             plt.ylim(ymax, ymin)
+        lgd_title = None
         for axlabel, keys in column_names.items():
             if xcol in keys:
                 plt.xlabel(axlabel)
             elif ycol in keys:
                 plt.ylabel(axlabel)
+            elif marker in keys:
+                lgd_title = axlabel
+
+        # add auxiliary axes
+        mjd_axis = mjd_axis and xcol == 'phase' and 'redshift' in self.meta and 'refmjd' in self.meta
+        appmag_axis = appmag_axis and ycol == 'absmag' and 'dm' in self.meta
+        if mjd_axis or appmag_axis:
+            top, right = aux_axes(self._phase2mjd if mjd_axis else None, self._abs2app if appmag_axis else None)
+            if mjd_axis:
+                top.xaxis.get_major_formatter().set_useOffset(False)
+                top.set_xlabel('MJD')
+            if appmag_axis:
+                right.set_ylabel('Apparent Magnitude')
+
+        # add legends
+            if marker in self.colnames:
+                labels = sorted(set(self[marker]))
+                lines = [plt.Line2D([], [], mec='k', mfc='none', ms=ms, marker=self.markers[label], linestyle='none')
+                         for label in labels]
+                custom_legend(top, lines, labels, ncol=ncol_mark, loc=loc_mark, title=lgd_title, frameon=True)
+
+            if color == 'filter':
+                if lgd_filters is None:
+                    lgd_filters = set(self['filter'])
+                lines, labels, ncol = filter_legend(lgd_filters, offset_factor)
+                custom_legend(right, lines, labels, loc=loc_filt, ncol=ncol, title='Filter', frameon=True)
+
+        if tight_layout:
+            plt.tight_layout()
+
+    def _phase2mjd(self, phase, hours=False):
+        return phase * (1. + self.meta['redshift']) / (24. if hours else 1.) + self.meta['refmjd']
+
+    def _abs2app(self, absmag):
+        return absmag + self.meta['dm']  # extinction-corrected apparent magnitude
 
     @classmethod
     def read(cls, filepath, format='ascii', fill_values=None, **kwargs):
         if fill_values is None:
             fill_values = [('--', '0'), ('', '0')]
         t = super(LC, cls).read(filepath, format=format, fill_values=fill_values, **kwargs)
-        t.normalize_column_names()
-        if 'filt' in t.colnames:
-            t.filters_to_objects()
         return t
 
+    def write(self, *args, **kwargs):
+        # Filter is not serializable, so produce a copy of the LC object with 'filter' as a string
+        out = Table(self)
+        if 'filter' in out.colnames:
+            out.replace_column('filter', self['filter'].astype(str))
+        out.write(*args, **kwargs)
+
+
+def aux_axes(xfunc=None, yfunc=None, ax0=None, xfunc_args=None, yfunc_args=None):
+    """
+    Add auxiliary axes to a plot that are linear transformations of the existing axes
+
+    Parameters
+    ----------
+    xfunc : function, optional
+        Function that transforms the lower x-axis to the upper x-axis. Default: do not add an upper x-axis.
+    yfunc : function, optional
+        Function that transforms the left y-axis to the right y-axis. Default: do not add a right y-axis.
+    ax0 : matplotlib.pyplot.Axes, optional
+        Existing axes object. Default: use the current Axes.
+    xfunc_args, yfunc_args : dict, optional
+        Keyword arguments for ``xfunc`` and ``yfunc``, respectively
+
+    Returns
+    -------
+    top : matplotlib.pyplot.Axes
+        The upper x-axis, if any. Otherwise, None.
+    right : matplotlib.pyplot.Axes
+        The right y-axis, if any. Otherwise, None.
+    """
+    if xfunc_args is None:
+        xfunc_args = {}
+    if yfunc_args is None:
+        yfunc_args = {}
+    if not ax0:
+        ax0 = plt.gca()
+    lims = np.array(ax0.axis())
+    if xfunc is not None:
+        ax0.xaxis.tick_bottom()
+        lims[:2] = xfunc(lims[:2], **xfunc_args)
+        top = ax0.twiny()
+        top.axis(lims)
+    else:
+        top = ax0
+    if yfunc is not None:
+        ax0.yaxis.tick_left()
+        lims[2:] = yfunc(lims[2:], **yfunc_args)
+        right = top.twinx()
+        right.axis(lims)
+    else:
+        right = None
+    plt.sca(ax0)
+    return top, right
+
+
+def custom_legend(ax, handles, labels, top_axis=True, **kwargs):
+    """
+    Add a legend to the axes with options for ``loc='above'``, ``loc='above left'``, and ``loc='above right'``
+
+    Parameters
+    ----------
+    ax : matplotlib.pyplot.Axes, matplotlib.pyplot.Figure
+        Axes or Figure object to which to add the legend
+    handles : list of matplotlib.pyplot.Artist
+        A list of Artists (lines, patches) to be added to the legend
+    labels : list of str
+        A list of labels to show next to the handles
+    top_axis : bool, optional
+        For legends above the top of the plot, add extra padding to the upper x-axis labels. Default: True.
+    kwargs
+        Keyword arguments to be passed to :func:`matplotlib.pyplot.legend`
+
+    Returns
+    -------
+    lgd : matplotlib.legend.Legend
+        The Legend object
+    """
+    loc = kwargs.pop('loc', None)
+    bbox_to_anchor = kwargs.pop('bbox_to_anchor', None)
+    if top_axis:
+        top_of_axis = 1.15
+    else:
+        top_of_axis = 1.
+    if loc is None or loc.lower() == 'none':
+        return
+    elif loc == 'above':
+        loc = 'lower center'
+        bbox_to_anchor = (0.5, top_of_axis)
+    elif loc == 'above left':
+        loc = 'lower left'
+        bbox_to_anchor = (0., top_of_axis)
+    elif loc == 'above right':
+        loc = 'lower right'
+        bbox_to_anchor = (1., top_of_axis)
+    lgd = ax.legend(handles, labels, loc=loc, bbox_to_anchor=bbox_to_anchor, **kwargs)
+    plt.tight_layout()  # adjusts the top of the axes to make room for 'above' legends
+    return lgd
+
+
+def filter_legend(filts, offset_factor=1.):
+    """
+    Creates dummy artists and labels for the filter legend using the filter properties
+
+    Parameters
+    ----------
+    filts : set, list, array-like
+        If a list or array of strings, the arrangement of filters in the legend, with columns in the first dimension and
+        rows in the second. If a set of :class:`.Filter` objects, they will first be arranged using :func:`.filtsetup`.
+    offset_factor : float, optional
+        Increase or decrease the filter offsets by a constant factor. Default: 1.
+
+    Returns
+    -------
+    lines : list of matplotlib.pyplot.Artist
+        A list of Artists (lines, patches) to be added to the legend
+    labels : list of str
+        A list of labels to show next to the handles
+    ncol : int
+        Number of columns needed for the filter legend
+    """
+    lines = []
+    labels = []
+    if isinstance(filts, set):
+        filts = filtsetup(filts)
+    elif isinstance(filts[0], str):
+        filts = np.vectorize(filtdict.get)(filts)
+    for filt in filts.flatten():
+        if filt is None:
+            labels.append('')
+            lines.append(Patch(color='none', ec='none'))
+        else:
+            col = filt.color
+            ec = filt.mec
+            off = filt.offset * offset_factor
+            if not filt.italics:
+                labels.append(filt.name)
+            elif offset_factor:
+                labels.append('${}{:+g}$'.format(filt.name, -off))
+            else:
+                labels.append('${}$'.format(filt.name))
+            lines.append(Patch(fc=col, ec=ec))
+    return lines, labels, filts.shape[0]
+
+
+def filtsetup(filts):
+    """
+    Arrange filters in a grid according to their system (columns) and offset (rows)
+
+    Parameters
+    ----------
+    filts : set
+        A set of :class:`.Filter` objects to be arranged
+
+    Returns
+    -------
+    lgnd : numpy.array
+        A 2D array of :class:`.Filter` objects
+    """
+    sysrows = dict()
+    for filt in filts:
+        if filt.system in sysrows:
+            sysrows[filt.system].add(filt.offset)
+        else:
+            sysrows[filt.system] = {filt.offset}
+    syscols = dict()
+    rowcols = []
+    for sys in list(sysrows.keys()):
+        for i, rows in enumerate(rowcols):
+            if not rows & sysrows[sys]:
+                syscols[sys] = i
+                rows |= sysrows[sys]
+                break
+        else:
+            syscols[sys] = len(rowcols)
+            rowcols.append(sysrows[sys])
+    offs = sorted({filt.offset for filt in filts}, reverse=True)
+    lgnd = np.tile(None, (len(rowcols), len(offs)))
+    for filt in filts:
+        if lgnd[syscols[filt.system], offs.index(filt.offset)] is None:
+            lgnd[syscols[filt.system], offs.index(filt.offset)] = filt
+        else:
+            offind = offs.index(filt.offset) + 1
+            offs.insert(offind, filt.offset)
+            newrow = np.tile(None, lgnd.shape[0])
+            newrow[syscols[filt.system]] = filt
+            lgnd = np.insert(lgnd, offind, newrow, 1)
+    while lgnd[0, 0] is None:
+        lgnd = np.roll(lgnd, 1, axis=0)
+    return lgnd
+
 
 def flux2mag(flux, dflux=np.array(np.nan), zp=0., nondet=None, nondetSigmas=3.):
     """
     Convert flux (and uncertainty) to magnitude (and uncertainty). Nondetections are converted to limiting magnitudes.
 
     Parameters
     ----------
@@ -566,15 +832,15 @@
         Uncertainty on the output magnitude
     """
     flux = flux.copy()
     dflux = dflux.copy()
     if nondet is not None:
         flux[nondet] = nondetSigmas * dflux[nondet]
         dflux[nondet] = np.nan
-    mag = -2.5 * np.log10(flux) + zp
+    mag = -2.5 * np.log10(flux, out=np.full_like(flux, -np.inf), where=flux > 0.) + zp
     dmag = 2.5 * dflux / (flux * np.log(10))
     return mag, dmag
 
 
 def mag2flux(mag, dmag=np.nan, zp=0., nondet=None, nondetSigmas=3.):
     """
     Convert magnitude (and uncertainty) to flux (and uncertainty). Nondetections are assumed to imply zero flux.
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/models/sifto.dat` & `lightcurve-fitting-0.8.0/lightcurve_fitting/models/sifto.dat`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/models.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 import astropy.constants as const
 import astropy.units as u
 from astropy.table import Table
 from pkg_resources import resource_filename
 from abc import ABCMeta, abstractmethod
+from scipy.interpolate import CubicSpline
+from .filters import filtdict
 
 k_B = const.k_B.to("eV / kK").value
 c3 = (4. * np.pi * const.sigma_sb.to("erg s-1 Rsun-2 kK-4").value) ** -0.5 / 1000.  # Rsun --> kiloRsun
 c4 = 1. / (4. * np.pi * u.Mpc.to(u.m) ** 2.)
 
 
 def format_unit(unit):
@@ -33,736 +35,859 @@
             unit_str = '$10^{{{value:.0f}}}$ {unit:latex_inline}'
     else:
         value = None
         unit_str = '{unit:latex_inline}'
     return unit_str.format(value=value, unit=unit)
 
 
-class Model:
-    """
-    An analytical model, defined by a function and its parameters
-
-    Parameters
-    ----------
-    func : function
-        A function that defines the analytical model
-    input_names : iterable
-        A list of parameter names
-    units : iterable
-        A list of units (:class:`astropy.unit.Unit`) for each parameter
-
-    Attributes
-    ----------
-    func : function
-        The function that defines the analytical model
-    input_names : iterable
-        A list of the parameter names
-    units : iterable
-        A list of the units for each parameter
-    nparams : int
-        The number of parameters in the model
-    axis_labels : list
-        Axis labels for each paramter (including name and unit)
-    output_quantity : str, optional
-        Quantity output by the model: 'lum' (default) or 'flux'
-    """
-    def __init__(self, func, input_names, units, output_quantity='lum'):
-        self.func = func
-        self.input_names = input_names
-        self.units = units
-        self.nparams = len(input_names)
-        self.axis_labels = ['${}$ ({})'.format(var, format_unit(unit))
-                            if unit is not u.dimensionless_unscaled else '${}$'.format(var)
-                            for var, unit in zip(input_names, units)]
-        self.output_quantity = output_quantity
+def power(base, exp):
+    """Power function that returns zero for any nonpositive base"""
+    broadcast = np.broadcast(base, exp)
+    zeros = np.zeros(broadcast.shape, float)
+    positive = base > 0.
+    power = np.power(base, exp, out=zeros, where=positive)
+    return power
 
-    def __call__(self, *args, **kwargs):
-        return self.func(*args[:self.nparams+2], **kwargs)  # +2 for times and filters
 
+class Model:
+    """An analytical model, defined by a function and its parameters"""
 
-def shock_cooling_temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1., n=1.5, RW=False):
-    """
-    The shock cooling model of Sapir & Waxman (https://doi.org/10.3847/1538-4357/aa64df).
+    input_names = []
+    """A list of the parameter names"""
 
-    This version of the model is written in terms of physical parameters :math:`v_s, M_\\mathrm{env}, f_ρ M, R`:
+    units = []
+    """A list of the units for each parameter"""
 
-    :math:`T(t) = \\frac{T_\\mathrm{col}}{T_\\mathrm{ph}} T_0 \\left(\\frac{v_s^2 t^2}{f_ρ M κ}\\right)^{ε_1}
-    \\frac{R^{1/4}}{κ^{1/4}} t^{-1/2}` (Eq. 23)
+    output_quantity = 'lum'
+    """Quantity output by the model: 'lum' or 'flux'"""
+
+    @property
+    def nparams(self):
+        """The number of parameters in the model"""
+        return len(self.input_names)
+
+    @property
+    def axis_labels(self):
+        """Axis labels for each paramter (including name and unit)"""
+        return ['${}$ ({})'.format(var, format_unit(unit))
+                if unit is not u.dimensionless_unscaled else '${}$'.format(var)
+                for var, unit in zip(self.input_names, self.units)]
+
+    def __init__(self, lc=None, redshift=0.):
+        if redshift:
+            self.z = redshift
+        elif lc is not None and 'redshift' in lc.meta:
+            self.z = lc.meta['redshift']
+        else:
+            self.z = 0.
 
-    :math:`L(t) = A \\exp\\left[-\\left(\\frac{a t}{t_\\mathrm{tr}}\\right)^α\\right]
-    L_0 \\left(\\frac{v_s t^2}{f_ρ M κ}\\right)^{-ε_2} \\frac{v_s^2 R}{κ}` (Eq. 18-19)
+    def __call__(self, *args, **kwargs):
+        return self.evaluate(*args, **kwargs)
 
-    :math:`t_\\mathrm{tr} = (19.5\\,\\mathrm{d}) \\left(\\frac{κ * M_\\mathrm{env}}{v_s} \\right)^{1/2}` (Eq. 20)
+    @abstractmethod
+    def evaluate(self, *args, **kwargs):
+        return NotImplemented
 
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    v_s : float, array-like
-        The shock speed in :math:`10^{8.5}` cm/s
-    M_env : float, array-like
-        The envelope mass in solar masses
-    f_rho_M : float, array-like
-        The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
-        envelope structure" and :math:`M` is the ejecta mass in solar masses
-    R : float, array-like
-        The progenitor radius in :math:`10^{13}` cm
-    t_exp : float, array-like
-        The explosion epoch
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    n : float, array-like
-        The polytropic index of the progenitor. Must be either 1.5 or 3.
-    RW : bool, optional
-        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63)
+    def log_likelihood(self, lc, p, use_sigma=False, sigma_type='relative'):
+        """
+        The log of the likelihood function of the model given data contained in `lc` and parameters contained in `p`
+
+        Parameters
+        ----------
+        lc : lightcurve_fitting.lightcurve.LC
+            Table of broadband photometry including columns "MJD", "mag", "dmag", "filter"
+        p : array-like
+            Model parameters for which to calculate the likelihood. The first dimension should have the same length as
+            the number of parameters, or one more if sigma is used.
+        use_sigma : bool, optional
+            If True, treat the last parameter as an intrinsic scatter parameter that does not get passed to the model
+        sigma_type : str, optional
+            If 'relative' (default), sigma will be in units of the individual photometric uncertainties.
+            If 'absolute', sigma will be in units of the median photometric uncertainty.
+
+        Returns
+        -------
+        log_likelihood : float, array-like
+            The natural log of the likelihood function. If `p` is 1D, `log_likelihood` is a float. Otherwise, its shape
+            is determined by the remaining dimensions of `p`.
+        """
+        f = lc['filter'].data
+        t = lc['MJD'].data
+        y = lc[self.output_quantity].data
+        dy = lc['d' + self.output_quantity].data
+
+        if sigma_type == 'relative':
+            sigma_units = dy
+        elif sigma_type == 'absolute':
+            sigma_units = np.median(dy)
+        else:
+            raise Exception('sigma_type must either be "relative" or "absolute"')
 
-    Returns
-    -------
-    T_K : array-like
-        The model blackbody temperatures in units of kilokelvins
-    R_bb : array-like
-        The model blackbody radii in units of 1000 solar radii
-    """
-    if n == 1.5:
-        A = 0.94
-        a = 1.67
-        alpha = 0.8
-        epsilon_1 = 0.027
-        epsilon_2 = 0.086
-        L_0 = 2.0e42
-        T_0 = 1.61
-        Tph_to_Tcol = 1.1
-    elif n == 3.:
-        A = 0.79
-        a = 4.57
-        alpha = 0.73
-        epsilon_1 = 0.016
-        epsilon_2 = 0.175
-        L_0 = 2.1e42
-        T_0 = 1.69
-        Tph_to_Tcol = 1.0
-    else:
-        raise ValueError('n can only be 1.5 or 3')
+        if use_sigma:
+            y_fit = self(t, f, *p[:-1])
+            sigma = np.sqrt(dy ** 2. + (p[-1] * sigma_units) ** 2.)
+        else:
+            y_fit = self(t, f, *p)
+            sigma = dy
 
-    if RW:
-        a = 0.
-        Tph_to_Tcol = 1.2
-
-    t = t_in.reshape(-1, 1) - t_exp
-    L_RW = L_0 * (t ** 2 * v_s / (f_rho_M * kappa)) ** -epsilon_2 * v_s ** 2 * R / kappa
-    t_tr = 19.5 * (kappa * M_env / v_s) ** 0.5
-    L = L_RW * A * np.exp(-(a * t / t_tr) ** alpha)
-    T_ph = T_0 * (t ** 2 * v_s ** 2 / (f_rho_M * kappa)) ** epsilon_1 * kappa ** -0.25 * t ** -0.5 * R ** 0.25
-    T_col = T_ph * Tph_to_Tcol
-    T_K = np.squeeze(T_col) / k_B
-    R_bb = c3 * np.squeeze(L) ** 0.5 * T_K ** -2
-    return T_K, R_bb
+        log_likelihood = -0.5 * np.sum(np.log(2 * np.pi * sigma ** 2.) + ((y - y_fit) / sigma) ** 2.)
+        return log_likelihood
 
 
-def shock_cooling(t_in, f, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1., n=1.5, RW=False, z=0.):
+class BaseShockCooling(Model):
     """
     The shock cooling model of Sapir & Waxman (https://doi.org/10.3847/1538-4357/aa64df).
 
-    This version of the model is written in terms of physical parameters :math:`v_s, M_\\mathrm{env}, f_ρ M, R`:
-
     :math:`T(t) = \\frac{T_\\mathrm{col}}{T_\\mathrm{ph}} T_0 \\left(\\frac{v_s^2 t^2}{f_ρ M κ}\\right)^{ε_1}
     \\frac{R^{1/4}}{κ^{1/4}} t^{-1/2}` (Eq. 23)
 
     :math:`L(t) = A \\exp\\left[-\\left(\\frac{a t}{t_\\mathrm{tr}}\\right)^α\\right]
     L_0 \\left(\\frac{v_s t^2}{f_ρ M κ}\\right)^{-ε_2} \\frac{v_s^2 R}{κ}` (Eq. 18-19)
 
     :math:`t_\\mathrm{tr} = (19.5\\,\\mathrm{d}) \\left(\\frac{κ * M_\\mathrm{env}}{v_s} \\right)^{1/2}` (Eq. 20)
 
     Parameters
     ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    v_s : float, array-like
-        The shock speed in :math:`10^{8.5}` cm/s
-    M_env : float, array-like
-        The envelope mass in solar masses
-    f_rho_M : float, array-like
-        The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
-        envelope structure" and :math:`M` is the ejecta mass in solar masses
-    R : float, array-like
-        The progenitor radius in :math:`10^{13}` cm
-    t_exp : float, array-like
-        The explosion epoch
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    n : float, array-like
-        The polytropic index of the progenitor. Must be either 1.5 or 3.
+    lc : lightcurve_fitting.lightcurve.LC, optional
+        The light curve to which the model will be fit. Only used to get the redshift if `redshift` is not given.
+    redshift : float, optional
+        The redshift between blackbody source and the observed filters. Default: 0.
+    n : float, optional
+        The polytropic index of the progenitor. Must be either 1.5 (default) or 3.
     RW : bool, optional
-        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63)
-    z : float, optional
-        The redshift between blackbody source and the observed filters
+        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63).
+        Default: False.
 
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
+    Attributes
+    ----------
+    z : float
+        The redshift between blackbody source and the observed filters
+    n : float
+        The polytropic index of the progenitor
+    A : float
+        Coefficient on the luminosity suppression factor (Eq. 19)
+    a : float
+        Coefficient on the transparency timescale (Eq. 19)
+    alpha : float
+        Exponent on the transparency timescale (Eq. 19)
+    epsilon_1 : float
+        Exponent in the temperature expression (Eq. 23)
+    epsilon_2 : float
+        Exponent in the luminosity expression (Eq. 18)
+    L_0 : float
+        Coefficient on the luminosity expression in erg/s (Eq. 18)
+    T_0 : float
+        Coefficient on the temperature expression in eV (Eq. 23)
+    Tph_to_Tcol : float
+        Ratio of the color temperature to the photospheric temperature
+    epsilon_T : float
+        Exponent on time in the temperature expression
+    epsilon_L : float
+        Exponent on time in the luminosity expression
+    RW : bool
+        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63)
     """
-    T_K, R_bb = shock_cooling_temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp, kappa, n, RW)
-    y_fit = blackbody_to_filters(f, T_K, R_bb, z)
-    return y_fit
+    def __init__(self, lc=None, redshift=0., n=1.5, RW=False):
+        super().__init__(lc, redshift=redshift)
 
+        if n == 1.5:
+            self.n = 1.5
+            self.A = 0.94
+            self.a = 1.67
+            self.alpha = 0.8
+            self.epsilon_1 = 0.027
+            self.epsilon_2 = 0.086
+            self.L_0 = 2.0e42
+            self.T_0 = 1.61
+            self.Tph_to_Tcol = 1.1
+        elif n == 3.:
+            self.n = 3.
+            self.A = 0.79
+            self.a = 4.57
+            self.alpha = 0.73
+            self.epsilon_1 = 0.016
+            self.epsilon_2 = 0.175
+            self.L_0 = 2.1e42
+            self.T_0 = 1.69
+            self.Tph_to_Tcol = 1.0
+        else:
+            raise ValueError('n can only be 1.5 or 3')
 
-def t_min(p, kappa=1.):
-    """
-    The minimum validity time for the :func:`shock_cooling` model
-
-    :math:`t_\\mathrm{min} = (0.2\\,\\mathrm{d}) \\frac{R}{v_s}
-    \\max\\left[0.5, \\frac{R^{0.4}}{(f_ρ M κ)^{0.2} v_s^{-0.7}}\\right] + t_\\mathrm{exp}` (Eq. 17)
-    """
-    v_s = p[0]
-    f_rho_M = p[2]
-    R = p[3]
-    t_exp = p[4] if len(p) > 4 else 0.
-    return 0.2 * R / v_s * np.maximum(0.5, R ** 0.4 * (f_rho_M * kappa) ** -0.2 * v_s ** -0.7) + t_exp
+        self.epsilon_T = 2 * self.epsilon_1 - 0.5
+        self.epsilon_L = -2 * self.epsilon_2
 
+        if RW:
+            self.RW = True
+            self.a = 0.
+            self.Tph_to_Tcol = 1.2
+        else:
+            self.RW = False
 
-def t_max(p, kappa=1.):
-    """
-    The maximum validity time for the :func:`shock_cooling` model
+    def __repr__(self):
+        return f'<{self.__class__.__name__}: z={self.z:.3f}, n={self.n:.1f}, RW={self.RW}>'
 
-    :math:`t_\\mathrm{max} = (7.4\\,\\mathrm{d}) \\left(\\frac{R}{κ}\\right)^{0.55} + t_\\mathrm{exp}` (Eq. 24)
-    """
-    R = p[3]
-    t_exp = p[4] if len(p) > 4 else 0.
-    return 7.4 * (R / kappa) ** 0.55 + t_exp
+    def temperature_radius(self, t_in, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1.):
+        """
+        Evaluate the color temperature and photospheric radius as a function of time for a set of parameters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        v_s : float, array-like
+            The shock speed in :math:`10^{8.5}` cm/s
+        M_env : float, array-like
+            The envelope mass in solar masses
+        f_rho_M : float, array-like
+            The product :math:`f_ρ M`, where :math:`f_ρ` is a numerical factor of order unity that depends on the inner
+            envelope structure and :math:`M` is the ejecta mass in solar masses
+        R : float, array-like
+            The progenitor radius in :math:`10^{13}` cm
+        t_exp : float, array-like
+            The explosion epoch
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        T_K : array-like
+            The model blackbody temperatures in units of kilokelvins
+        R_bb : array-like
+            The model blackbody radii in units of 1000 solar radii
+        """
+        t = np.reshape(t_in, (-1, 1)) - t_exp
+        L_RW = self.L_0 * power(t ** 2 * v_s / (f_rho_M * kappa), -self.epsilon_2) * v_s ** 2 * R / kappa
+        t_tr = 19.5 * (kappa * M_env / v_s) ** 0.5
+        L = L_RW * self.A * np.exp(-power(self.a * t / t_tr, self.alpha))
+        T_ph = self.T_0 * power(t ** 2 * v_s ** 2 / (f_rho_M * kappa), self.epsilon_1) \
+               * kappa ** -0.25 * power(t, -0.5) * R ** 0.25
+        T_col = T_ph * self.Tph_to_Tcol
+        T_K = np.squeeze(T_col) / k_B
+        R_bb = c3 * np.squeeze(L) ** 0.5 * power(T_K, -2.)
+        return T_K, R_bb
 
+    @abstractmethod
+    def evaluate(self, *args, **kwargs):
+        return NotImplemented
 
-ShockCooling = Model(shock_cooling,
-                     [
-                         'v_\\mathrm{s*}',
-                         'M_\\mathrm{env}',
-                         'f_\\rho M',
-                         'R',
-                         't_0'
-                     ],
-                     [
-                         10. ** 8.5 * u.cm / u.s,
-                         u.Msun,
-                         u.Msun,
-                         1e13 * u.cm,
-                         u.d
-                     ]
-                     )
-ShockCooling.t_min = t_min
-ShockCooling.t_max = t_max
+    @staticmethod
+    def t_min(p, kappa=1.):
+        """
+        The minimum time at which the model is valid
+
+        :math:`t_\\mathrm{min} = (0.2\\,\\mathrm{d}) \\frac{R}{v_s}
+        \\max\\left[0.5, \\frac{R^{0.4}}{(f_ρ M κ)^{0.2} v_s^{-0.7}}\\right] + t_\\mathrm{exp}` (Eq. 17)
+        """
+        v_s = p[0]
+        f_rho_M = p[2]
+        R = p[3]
+        t_exp = p[4] if len(p) > 4 else 0.
+        return 0.2 * R / v_s * np.maximum(0.5, R ** 0.4 * (f_rho_M * kappa) ** -0.2 * v_s ** -0.7) + t_exp
+
+    @staticmethod
+    def t_max(p, kappa=1.):
+        """
+        The maximum time at which the model is valid
+
+        :math:`t_\\mathrm{max} = (7.4\\,\\mathrm{d}) \\left(\\frac{R}{κ}\\right)^{0.55} + t_\\mathrm{exp}` (Eq. 24)
+        """
+        R = p[3]
+        t_exp = p[4] if len(p) > 4 else 0.
+        return 7.4 * (R / kappa) ** 0.55 + t_exp
 
 
-def shock_cooling3(t_in, f, v_s, M_env, f_rho_M, R, dist, ebv=0., t_exp=0., kappa=1., n=1.5, RW=False, z=0.):
+class ShockCooling(BaseShockCooling):
     """
     The shock cooling model of Sapir & Waxman (https://doi.org/10.3847/1538-4357/aa64df).
 
-    This version of the model is written in terms of physical parameters :math:`v_s, M_\\mathrm{env}, f_ρ M, R`:
-
-    :math:`T(t) = \\frac{T_\\mathrm{col}}{T_\\mathrm{ph}} T_0 \\left(\\frac{v_s^2 t^2}{f_ρ M κ}\\right)^{ε_1}
-    \\frac{R^{1/4}}{κ^{1/4}} t^{-1/2}` (Eq. 23)
-
-    :math:`L(t) = A \\exp\\left[-\\left(\\frac{a t}{t_\\mathrm{tr}}\\right)^α\\right]
-    L_0 \\left(\\frac{v_s t^2}{f_ρ M κ}\\right)^{-ε_2} \\frac{v_s^2 R}{κ}` (Eq. 18-19)
-
-    :math:`t_\\mathrm{tr} = (19.5\\,\\mathrm{d}) \\left(\\frac{κ * M_\\mathrm{env}}{v_s} \\right)^{1/2}` (Eq. 20)
-
-    This is the same as :func:`shock_cooling` but with distance and reddening as free parameters.
-
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    v_s : float, array-like
-        The shock speed in :math:`10^{8.5}` cm/s
-    M_env : float, array-like
-        The envelope mass in solar masses
-    f_rho_M : float, array-like
-        The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
-        envelope structure" and :math:`M` is the ejecta mass in solar masses
-    R : float, array-like
-        The progenitor radius in :math:`10^{13}` cm
-    dist : float, array-like
-        The luminosity distance to the supernova in Mpc
-    ebv : float, array-like
-        The reddening :math:`E(B-V)` to apply to the blackbody spectrum before integration
-    t_exp : float, array-like
-        The explosion epoch
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    n : float, array-like
-        The polytropic index of the progenitor. Must be either 1.5 or 3.
-    RW : bool, optional
-        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63)
-    z : float, optional
-        The redshift between blackbody source and the observed filters
-
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
+    This version of the model is written in terms of physical parameters :math:`v_s, M_\\mathrm{env}, f_ρ M, R`.
     """
-    T_K, R_bb = shock_cooling_temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp, kappa, n, RW)
-    lum = blackbody_to_filters(f, T_K, R_bb, z, ebv=ebv)
-    flux = c4 * lum / dist ** 2.
-    return flux
-
+    input_names = [
+        'v_\\mathrm{s*}',
+        'M_\\mathrm{env}',
+        'f_\\rho M',
+        'R',
+        't_0'
+    ]
+    units = [
+        10. ** 8.5 * u.cm / u.s,
+        u.Msun,
+        u.Msun,
+        1e13 * u.cm,
+        u.d
+    ]
+
+    def evaluate(self, t_in, f, v_s, M_env, f_rho_M, R, t_exp=0., kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        v_s : float, array-like
+            The shock speed in :math:`10^{8.5}` cm/s
+        M_env : float, array-like
+            The envelope mass in solar masses
+        f_rho_M : float, array-like
+            The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
+            envelope structure" and :math:`M` is the ejecta mass in solar masses
+        R : float, array-like
+            The progenitor radius in :math:`10^{13}` cm
+        t_exp : float, array-like, optional
+            The explosion epoch. Default: 0.
+        kappa : float, array-like, optional
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g). Default: 1.
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        T_K, R_bb = self.temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp, kappa)
+        y_fit = blackbody_to_filters(f, T_K, R_bb, self.z)
+        return y_fit
 
-def t_min3(p, kappa=1.):
-    """
-    The minimum validity time for the :func:`shock_cooling` model
 
-    :math:`t_\\mathrm{min} = (0.2\\,\\mathrm{d}) \\frac{R}{v_s}
-    \\max\\left[0.5, \\frac{R^{0.4}}{(f_ρ M κ)^{0.2} v_s^{-0.7}}\\right] + t_\\mathrm{exp}` (Eq. 17)
-    """
-    return t_min([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa)
-
-
-def t_max3(p, kappa=1.):
-    """
-    The maximum validity time for the :func:`shock_cooling` model
-
-    :math:`t_\\mathrm{max} = (7.4\\,\\mathrm{d}) \\left(\\frac{R}{κ}\\right)^{0.55} + t_\\mathrm{exp}` (Eq. 24)
-    """
-    return t_max([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa)
-
-
-ShockCooling3 = Model(shock_cooling3,
-                      [
-                          'v_\\mathrm{s*}',
-                          'M_\\mathrm{env}',
-                          'f_\\rho M',
-                          'R',
-                          'd_L',
-                          'E(B-V)',
-                          't_0',
-                      ],
-                      [
-                          10. ** 8.5 * u.cm / u.s,
-                          u.Msun,
-                          u.Msun,
-                          1e13 * u.cm,
-                          u.Mpc,
-                          u.mag,
-                          u.d,
-                      ],
-                      output_quantity='flux')
-ShockCooling3.t_min = t_min3
-ShockCooling3.t_max = t_max3
-
-
-def shock_cooling2(t_in, f, T_1, L_1, t_tr, t_exp=0., n=1.5, RW=False, z=0.):
+class ShockCooling2(BaseShockCooling):
     """
     The shock cooling model of Sapir & Waxman (https://doi.org/10.3847/1538-4357/aa64df).
 
     This version of the model is written in terms of scaling parameters :math:`T_1, L_1, t_\\mathrm{tr}`:
 
-    :math:`T(t) = T_1 t^{2 ε_1 - 0.5}` and
-    :math:`L(t) = L_1 \\exp\\left[-\\left(\\frac{a t}{t_\\mathrm{tr}}\\right)^α\\right] t^{-2 ε_2}`
-
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    T_1 : float, array-like
-        The blackbody temperature 1 day after explosion in kilokelvins
-    L_1 : float, array-like
-        The approximate blackbody luminosity 1 day after explosion in :math:`10^{42}` erg/s
-    t_tr : float, array-like
-        The time at which the envelope becomes transparent in rest-frame days
-    t_exp : float, array-like
-        The explosion epoch
-    n : float, array-like
-        The polytropic index of the progenitor. Must be either 1.5 or 3.
-    RW : bool, optional
-        Reduce the model to the simpler form of Rabinak & Waxman (https://doi.org/10.1088/0004-637X/728/1/63)
-    z : float, optional
-        The redshift between blackbody source and the observed filters
-
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
-    """
-    if n == 1.5:
-        a = 1.67
-        alpha = 0.8
-        epsilon_1 = 0.027
-        epsilon_2 = 0.086
-    elif n == 3.:
-        a = 4.57
-        alpha = 0.73
-        epsilon_1 = 0.016
-        epsilon_2 = 0.175
-    else:
-        raise ValueError('n can only be 1.5 or 3')
-
-    if RW:
-        a = 0.
-
-    t = t_in.reshape(-1, 1) - t_exp
-
-    epsilon_T = 2 * epsilon_1 - 0.5
-    epsilon_L = -2 * epsilon_2
-
-    T_K = np.squeeze(T_1 * t ** epsilon_T)
-    L = np.squeeze(L_1 * np.exp(-(a * t / t_tr) ** alpha) * t ** epsilon_L) * 1e42
-    R_bb = c3 * L ** 0.5 * T_K ** -2
-
-    y_fit = blackbody_to_filters(f, T_K, R_bb, z)
-
-    return y_fit
-
-
-def t_min2(*args):
-    """
-    The maximum validity time for the :func:`shock_cooling2` model
-
-    Raises
-    ------
-    NotImplementedError
+    :math:`T(t) = T_1 t^{ε_T}` and
+    :math:`L(t) = L_1 t^{ε_L} \\exp\\left[-\\left(\\frac{a t}{t_\\mathrm{tr}}\\right)^α\\right]`
     """
-    raise NotImplementedError('t_min cannot be translated to these parameters')
+    input_names = [
+        'T_1',
+        'L_1',
+        't_\\mathrm{tr}',
+        't_0'
+    ]
+    units = [
+        u.kK,
+        1e42 * u.erg / u.s,
+        u.d,
+        u.d
+    ]
+
+    def evaluate(self, t_in, f, T_1, L_1, t_tr, t_exp=0.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        T_1 : float, array-like
+            The blackbody temperature 1 day after explosion in kilokelvins
+        L_1 : float, array-like
+            The approximate blackbody luminosity 1 day after explosion in :math:`10^{42}` erg/s
+        t_tr : float, array-like
+            The time at which the envelope becomes transparent in rest-frame days
+        t_exp : float, array-like
+            The explosion epoch
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+
+        t = np.reshape(t_in, (-1, 1)) - t_exp
+
+        T_K = np.squeeze(T_1 * power(t, self.epsilon_T))
+        L = np.squeeze(L_1 * np.exp(-power(self.a * t / t_tr, self.alpha)) * power(t, self.epsilon_L)) * 1e42
+        R_bb = c3 * L ** 0.5 * power(T_K, -2.)
+
+        y_fit = blackbody_to_filters(f, T_K, R_bb, self.z)
+
+        return y_fit
+
+    @staticmethod
+    def t_min(p, kappa=1.):
+        """
+        The minimum time at which the model is valid
+
+        This expression cannot be translated to the parameters of :class:`ShockCooling2`
+        """
+        return NotImplemented
+
+    def t_max(self, p, kappa=1.):
+        """
+        The maximum time at which the model is valid
+
+        :math:`t_\\mathrm{max} = \\left(\\frac{8.12\\,\\mathrm{kK}}{T_1}\\right)^{1/(2 ε_1 - 0.5)} + t_\\mathrm{exp}`
+        """
+        T_1 = p[0]
+        t_exp = p[3] if len(p) > 3 else 0.
+        return (8.12 / T_1) ** (self.epsilon_T ** -1) + t_exp
 
 
-def t_max2(p, n=1.5):
+class ShockCooling3(BaseShockCooling):
     """
-    The maximum validity time for the :func:`shock_cooling2` model
+    The shock cooling model of Sapir & Waxman (https://doi.org/10.3847/1538-4357/aa64df).
 
-    :math:`t_\\mathrm{max} = \\left(\\frac{8.12\\,\\mathrm{kK}}{T_1}\\right)^{1/(2 ε_1 - 0.5)} + t_\\mathrm{exp}`
+    This version of the model is written in terms of physical parameters :math:`v_s, M_\\mathrm{env}, f_ρ M, R` and
+    includes distance :math:`d_L` and reddening :math:`E(B-V)` as free parameters.
     """
-    T_1 = p[0]
-    t_exp = p[3] if len(p) > 3 else 0.
-
-    if n == 1.5:
-        epsilon_1 = 0.027
-    elif n == 3.:
-        epsilon_1 = 0.016
-    else:
-        raise ValueError('n can only be 1.5 or 3')
+    input_names = [
+        'v_\\mathrm{s*}',
+        'M_\\mathrm{env}',
+        'f_\\rho M',
+        'R',
+        'd_L',
+        'E(B-V)',
+        't_0',
+    ]
+    units = [
+        10. ** 8.5 * u.cm / u.s,
+        u.Msun,
+        u.Msun,
+        1e13 * u.cm,
+        u.Mpc,
+        u.mag,
+        u.d,
+    ]
+    output_quantity = 'flux'
+
+    def evaluate(self, t_in, f, v_s, M_env, f_rho_M, R, dist, ebv=0., t_exp=0., kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        v_s : float, array-like
+            The shock speed in :math:`10^{8.5}` cm/s
+        M_env : float, array-like
+            The envelope mass in solar masses
+        f_rho_M : float, array-like
+            The product :math:`f_ρ M`, where ":math:`f_ρ` is a numerical factor of order unity that depends on the inner
+            envelope structure" and :math:`M` is the ejecta mass in solar masses
+        R : float, array-like
+            The progenitor radius in :math:`10^{13}` cm
+        dist : float, array-like
+            The luminosity distance in Mpc
+        ebv : float, array-like, optional
+            The reddening :math:`E(B-V)` to apply to the blackbody spectrum before integration. Default: 0.
+        t_exp : float, array-like, optional
+            The explosion epoch. Default: 0.
+        kappa : float, array-like, optional
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g). Default: 1.
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        T_K, R_bb = self.temperature_radius(t_in, v_s, M_env, f_rho_M, R, t_exp, kappa)
+        lum = blackbody_to_filters(f, T_K, R_bb, self.z, ebv=ebv)
+        flux = c4 * lum / dist ** 2.
+        return flux
+
+    @staticmethod
+    def t_min(p, kappa=1.):
+        return super().t_min([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa=kappa)
+
+    @staticmethod
+    def t_max(p, kappa=1.):
+        return super().t_max([p[0], p[1], p[2], p[3], p[6] if len(p) > 6 else 0.], kappa=kappa)
 
-    epsilon_T = 2 * epsilon_1 - 0.5
-
-    return (8.12 / T_1) ** (epsilon_T ** -1) + t_exp
-
-
-ShockCooling2 = Model(shock_cooling2,
-                      [
-                          'T_1',
-                          'L_1',
-                          't_\\mathrm{tr}',
-                          't_0'
-                      ],
-                      [
-                          u.kK,
-                          1e42 * u.erg / u.s,
-                          u.d,
-                          u.d
-                      ]
-                      )
-ShockCooling2.t_min = t_min2
-ShockCooling2.t_max = t_max2
 
 sifto_filename = resource_filename('lightcurve_fitting', 'models/sifto.dat')
-sifto = Table.read(sifto_filename, format='ascii')
-sifto['x'] = sifto['r']  # assume DLT40 = r for now
-
-
-def scale_sifto(sn_lc):
-    """
-    Scale the SiFTO model to match your supernova's luminosity and colors
-
-    Parameters
-    ----------
-    sn_lc : lightcurve_fitting.lightcurve.LC
-        Your supernova's light curve
-    """
-    for filt in set(sn_lc['filter']):
-        if filt.char not in sifto.colnames:
-            raise Exception('No SiFTO template for filter ' + filt.char)
-        lc_filt = sn_lc.where(filter=filt)
-        sifto[filt.char] *= np.max(lc_filt['lum']) / np.max(sifto[filt.char])
+sifto = Table.read(sifto_filename, format='ascii')[3:]  # the first three points are ~0
+M_chandra = u.def_unit('M_chandra', 1.4 * u.Msun, format={'latex': 'M_\\mathrm{Ch}'})
 
 
-def companion_shocking_temperature_radius(t_in, t_exp, a13, Mc_v9_7, kappa=1.):
+class BaseCompanionShocking(Model):
     """
-    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025)
+    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model.
 
     As written by Hosseinzadeh et al. (https://doi.org/10.3847/2041-8213/aa8402), the shock component is defined by:
 
     :math:`R_\\mathrm{phot}(t) = (2700\\,R_\\odot) (M_c v_9^7)^{1/9} κ^{1/9} t^{7/9}` (Eq. 1)
 
     :math:`T_\\mathrm{eff}(t) = (25\\,\\mathrm{kK}) a_{13}^{1/4} (M_c v_9^7)^{1/144} κ^{-35/144} t^{37/72}` (Eq. 2)
 
+    The SiFTO model (https://doi.org/10.1086/588518) is currently only available in the UBVgri filters.
+
     Parameters
     ----------
-    t_in : float, array-like
-        Time in days
-    t_exp : float, array-like
-        The explosion epoch
-    a13 : float, array-like
-        The binary separation in :math:`10^{13}` cm
-    Mc_v9_7 : float, array-like
-        The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
-        the ejecta velocity in units of :math:`10^9` cm/s
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-
-    Returns
-    -------
-    T_kasen : array-like
-        The model blackbody temperatures in units of kilokelvins
-    R_kasen : array-like
-        The model blackbody radii in units of 1000 solar radii
-    """
-    t_wrt_exp = t_in.reshape(-1, 1) - t_exp
-    T_kasen = np.squeeze(25. * (a13 ** 36 * Mc_v9_7 * kappa ** -35 * t_wrt_exp ** -74) ** (1 / 144.))  # kK
-    R_kasen = np.squeeze(2.7 * (kappa * Mc_v9_7 * t_wrt_exp ** 7) ** (1 / 9.))  # kiloRsun
-    return T_kasen, R_kasen
-
-
-def companion_shocking(t_in, f, t_exp, a13, Mc_v9_7, kappa=1., z=0., cutoff_freq=np.inf):
-    """
-    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025)
-
-    As written by Hosseinzadeh et al. (https://doi.org/10.3847/2041-8213/aa8402), the shock component is defined by:
-
-    :math:`R_\\mathrm{phot}(t) = (2700\\,R_\\odot) (M_c v_9^7)^{1/9} κ^{1/9} t^{7/9}` (Eq. 1)
+    lc : lightcurve_fitting.lightcurve.LC, optional
+        The light curve to which the model will be fit. Only used for `lc.meta['redshift']` if `z` is not given.
+    redshift : float, optional
+        The redshift between blackbody source and the observed filters. Default: 0.
 
-    :math:`T_\\mathrm{eff}(t) = (25\\,\\mathrm{kK}) a_{13}^{1/4} (M_c v_9^7)^{1/144} κ^{-35/144} t^{37/72}` (Eq. 2)
-
-    Parameters
+    Attributes
     ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    t_exp : float, array-like
-        The explosion epoch
-    a13 : float, array-like
-        The binary separation in :math:`10^{13}` cm
-    Mc_v9_7 : float, array-like
-        The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
-        the ejecta velocity in units of :math:`10^9` cm/s
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    z : float, optional
+    z : float
         The redshift between blackbody source and the observed filters
-    cutoff_freq : float, optional
-        Cutoff frequency (in terahertz) for a modified blackbody spectrum (see https://doi.org/10.3847/1538-4357/aa9334)
+    sifto : astropy.table.Table
+        A copy of the SiFTO model scaled to match the observed peak luminosity in each filter
 
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
     """
-    T_kasen, R_kasen = companion_shocking_temperature_radius(t_in, t_exp, a13, Mc_v9_7, kappa)
-    Lnu_kasen = blackbody_to_filters(f, T_kasen, R_kasen, z, cutoff_freq)
-    return Lnu_kasen
+    def __init__(self, lc, redshift=0.):
+        super().__init__(lc, redshift=redshift)
 
+        # make sure input light curve has luminosities
+        if 'lum' not in lc.colnames:
+            if 'absmag' not in lc.colnames:
+                lc.calcAbsMag()
+            lc.calcLum()
+
+        self.sifto = {}
+        dlt40 = filtdict['DLT40']
+        unfilt = filtdict['unfilt.']
+        for filt in set(lc['filter']):
+            if filt.char in sifto.colnames or filt == dlt40:
+                char = 'r' if filt == dlt40 else filt.char
+                lc_filt = lc.where(filter=filt)
+                sifto_scaled = sifto[char] * np.max(lc_filt['lum']) / np.max(sifto[char])
+                self.sifto[filt] = CubicSpline(sifto['Epoch'], sifto_scaled, extrapolate=False)
+            elif filt != unfilt:
+                raise Exception('No SiFTO template for filter ' + filt.name)
 
-def stretched_sifto(t_in, f, t_peak, stretch, dtU=None, dti=None):
-    """
-    The SiFTO SN Ia model (https://doi.org/10.1086/588518), offset and stretched by the input parameters
+        # assume unfiltered = DLT40 for now
+        self.sifto[unfilt] = self.sifto[dlt40]
 
-    The SiFTO model is currently only available in the UBVgri filters. We assume DLT40 can be modeled as r.
+    def __repr__(self):
+        return f'<{self.__class__.__name__}: z={self.z:.3f}>'
 
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    t_peak : float, array-like
-        The epoch of maximum light for the SiFTO model
-    stretch : float, array-like
-        The stretch for the SiFTO model
-    dtU, dti : float, array-like
-        Time offsets for the U- and i-band models relative to the other bands
+    @abstractmethod
+    def evaluate(self, *args, **kwargs):
+        return NotImplemented
 
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
-    """
-    dt_peak = {'U': np.zeros_like(stretch) if dtU is None else dtU, 'i': np.zeros_like(stretch) if dti is None else dti}
-    t_wrt_peak = np.squeeze(t_in.reshape(-1, 1) - t_peak)
-    if t_wrt_peak.ndim <= 1 and len(t_wrt_peak) == len(f):  # pointwise
-        Lnu_sifto = np.array([np.interp(t - dt_peak.get(filt.char, 0.), sifto['Epoch'] * stretch, sifto[filt.char])
-                              for t, filt in zip(t_wrt_peak, f)])
-    elif t_wrt_peak.ndim <= 1:
-        Lnu_sifto = np.array([np.interp(t_wrt_peak - dt_peak.get(filt.char, 0.), sifto['Epoch'] * stretch, sifto[filt.char])
-                              for filt in f])
-    else:
-        Lnu_sifto = np.array([np.array([np.interp(t - dt, sifto['Epoch'] * s, sifto[filt.char])
-                                        for t, s, dt in zip(t_wrt_peak.T, stretch, dt_peak.get(filt.char, np.zeros_like(stretch)))]).T
-                              for filt in f])
-    return Lnu_sifto
+    @staticmethod
+    def temperature_radius(t_in, t_exp, a13, Mc_v9_7, kappa=1.):
+        """
+        Evaluate the color temperature and photospheric radius of the shock component as a function of time
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        t_exp : float, array-like
+            The explosion epoch
+        a13 : float, array-like
+            The binary separation in :math:`10^{13}` cm
+        Mc_v9_7 : float, array-like
+            The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9`
+            is the ejecta velocity in units of :math:`10^9` cm/s
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        T_kasen : array-like
+            The model blackbody temperatures in units of kilokelvins
+        R_kasen : array-like
+            The model blackbody radii in units of 1000 solar radii
+        """
+        t = np.reshape(t_in, (-1, 1)) - t_exp
+        T_kasen = np.squeeze(25. * power(a13 ** 36. * Mc_v9_7 * kappa ** -35. * power(t, -74.), 1. / 144.))  # kK
+        R_kasen = np.squeeze(2.7 * power(kappa * Mc_v9_7 * t ** 7., 1. / 9.))  # kiloRsun
+        return T_kasen, R_kasen
+
+    def companion_shocking(self, t_in, f, t_exp, a13, Mc_v9_7, kappa=1.):
+        """
+        Evaluate the shock component only at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        t_exp : float, array-like
+            The explosion epoch
+        a13 : float, array-like
+            The binary separation in :math:`10^{13}` cm
+        Mc_v9_7 : float, array-like
+            The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
+            the ejecta velocity in units of :math:`10^9` cm/s
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        T_kasen, R_kasen = self.temperature_radius(t_in, t_exp, a13, Mc_v9_7, kappa)
+        Lnu_kasen = blackbody_to_filters(f, T_kasen, R_kasen, self.z)
+        return Lnu_kasen
+
+    def stretched_sifto(self, t_in, f, t_peak, stretch, dtU=None, dti=None):
+        """
+        The SiFTO SN Ia model (https://doi.org/10.1086/588518), offset and stretched by the input parameters
+
+        The SiFTO model is currently only available in the UBVgri filters. We assume unfiltered photometry can be
+        modeled as r.
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        t_peak : float, array-like
+            The epoch of maximum light for the SiFTO model
+        stretch : float, array-like
+            The stretch for the SiFTO model
+        dtU, dti : float, array-like
+            Time offsets for the U- and i-band models relative to the other bands
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        dt_peak = {}
+        if dtU is not None:
+            dt_peak[filtdict['U']] = dtU
+        if dti is not None:
+            dt_peak[filtdict['i']] = dti
+        t_wrt_peak = np.squeeze(np.reshape(t_in, (-1, 1)) - t_peak)
+        if t_wrt_peak.ndim <= 1 and len(t_wrt_peak) == len(f):  # pointwise
+            Lnu_sifto = np.array([self.sifto[filt]((t - dt_peak.get(filt, 0.)) / stretch)
+                                  for t, filt in zip(t_wrt_peak, f)])
+        elif t_wrt_peak.ndim <= 1:
+            Lnu_sifto = np.array([self.sifto[filt]((t_wrt_peak - dt_peak.get(filt, 0.)) / stretch) for filt in f])
+        else:
+            Lnu_sifto = np.array([np.transpose([self.sifto[filt]((t - dt) / s) for t, dt, s in
+                                                zip(t_wrt_peak.T, dt_peak.get(filt, np.zeros_like(stretch)), stretch)])
+                                  for filt in f])
+        Lnu_sifto[np.isnan(Lnu_sifto)] = 0.  # extrapolate all filters as zero
+        return Lnu_sifto
+
+    @staticmethod
+    def t_min(p):
+        """
+        The minimum time at which the model is valid
+
+        This is the first epoch at which the stretched SiFTO model is computed
+        """
+        return p[3] + p[4] * sifto['Epoch'].min()
+
+    @staticmethod
+    def t_max(p):
+        """
+        The maximum time at which the model is valid
+
+        This is the last epoch at which the stretched SiFTO model is computed
+        """
+        return p[3] + p[4] * sifto['Epoch'].max()
 
 
-def companion_shocking_plus_sifto(t_in, f, t_exp, a13, Mc_v9_7, t_peak, stretch, rr=1., ri=1., rU=1., kappa=1., z=0.):
+class CompanionShocking(BaseCompanionShocking):
     """
-    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model
-
-    As written by Hosseinzadeh et al. (https://doi.org/10.3847/2041-8213/aa8402), the shock component is defined by:
-
-    :math:`R_\\mathrm{phot}(t) = (2700\\,R_\\odot) (M_c v_9^7)^{1/9} κ^{1/9} t^{7/9}` (Eq. 1)
-
-    :math:`T_\\mathrm{eff}(t) = (25\\,\\mathrm{kK}) a_{13}^{1/4} (M_c v_9^7)^{1/144} κ^{-35/144} t^{37/72}` (Eq. 2)
-
-    The SiFTO model (https://doi.org/10.1086/588518) is currently only available in the UBVgri filters.
+    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model.
 
     This version of the model includes factors on the r and i SiFTO models, and a factor on the U shock component.
-
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    t_exp : float, array-like
-        The explosion epoch
-    a13 : float, array-like
-        The binary separation in :math:`10^{13}` cm
-    Mc_v9_7 : float, array-like
-        The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
-        the ejecta velocity in units of :math:`10^9` cm/s
-    t_peak : float, array-like
-        The epoch of maximum light for the SiFTO model
-    stretch : float, array-like
-        The stretch for the SiFTO model
-    rr : float, array-like
-        A scale factor for the r-band SiFTO model
-    ri : float, array-like
-        A scale factor for the i-band SiFTO model
-    rU : float, aray-like
-        A scale factor for the U-band of the shock component
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    z : float, optional
-        The redshift between blackbody source and the observed filters
-
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
     """
-    Lnu_kasen = companion_shocking(t_in, f, t_exp, a13, Mc_v9_7, kappa, z)
-    Lnu_sifto = stretched_sifto(t_in, f, t_peak, stretch)
-
-    sifto_factors = {'r': rr, 'i': ri}
-    kasen_factors = {'U': rU}
-    y_fit = np.array([L1 * kasen_factors.get(filt.char, 1.) + L2 * sifto_factors.get(filt.char, 1.)
-                      for L1, L2, filt in zip(Lnu_kasen, Lnu_sifto, f)])
+    input_names = [
+        't_0',
+        'a',
+        'M v^7',
+        't_\\mathrm{max}',
+        's',
+        'r_r',
+        'r_i',
+        'r_U'
+    ]
+    units = [
+        u.d,
+        10. ** 13. * u.cm,
+        M_chandra * (1e9 * u.cm / u.s) ** 7,
+        u.d,
+        u.dimensionless_unscaled,
+        u.dimensionless_unscaled,
+        u.dimensionless_unscaled,
+        u.dimensionless_unscaled
+    ]
+
+    def evaluate(self, t_in, f, t_exp, a13, Mc_v9_7, t_peak, stretch, rr=1., ri=1., rU=1., kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        t_exp : float, array-like
+            The explosion epoch
+        a13 : float, array-like
+            The binary separation in :math:`10^{13}` cm
+        Mc_v9_7 : float, array-like
+            The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
+            the ejecta velocity in units of :math:`10^9` cm/s
+        t_peak : float, array-like
+            The epoch of maximum light for the SiFTO model
+        stretch : float, array-like
+            The stretch for the SiFTO model
+        rr : float, array-like
+            A scale factor for the r-band SiFTO model
+        ri : float, array-like
+            A scale factor for the i-band SiFTO model
+        rU : float, aray-like
+            A scale factor for the U-band of the shock component
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        Lnu_kasen = self.companion_shocking(t_in, f, t_exp, a13, Mc_v9_7, kappa)
+        Lnu_sifto = self.stretched_sifto(t_in, f, t_peak, stretch)
+
+        sifto_factors = {'r': rr, 'i': ri}
+        kasen_factors = {'U': rU}
+        y_fit = np.array([L1 * kasen_factors.get(filt.char, 1.) + L2 * sifto_factors.get(filt.char, 1.)
+                          for L1, L2, filt in zip(Lnu_kasen, Lnu_sifto, f)])
 
-    return y_fit
+        return y_fit
 
 
-M_chandra = u.def_unit('M_chandra', 1.4 * u.Msun, format={'latex': 'M_\\mathrm{Ch}'})
-CompanionShocking = Model(companion_shocking_plus_sifto,
-                          [
-                              't_0',
-                              'a',
-                              'M v^7',
-                              't_\\mathrm{max}',
-                              's',
-                              'r_r',
-                              'r_i',
-                              'r_U'
-                          ],
-                          [
-                              u.d,
-                              10. ** 13. * u.cm,
-                              M_chandra * (1e9 * u.cm / u.s) ** 7,
-                              u.d,
-                              u.dimensionless_unscaled,
-                              u.dimensionless_unscaled,
-                              u.dimensionless_unscaled,
-                              u.dimensionless_unscaled
-                          ]
-                          )
-
-
-def companion_shocking_plus_sifto2(t_in, f, t_exp, a13, Mc_v9_7, t_peak, stretch, dtU=0., dti=0., kappa=1., z=0.):
+class CompanionShocking2(BaseCompanionShocking):
     """
-    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model
-
-    As written by Hosseinzadeh et al. (https://doi.org/10.3847/2041-8213/aa8402), the shock component is defined by:
-
-    :math:`R_\\mathrm{phot}(t) = (2700\\,R_\\odot) (M_c v_9^7)^{1/9} κ^{1/9} t^{7/9}` (Eq. 1)
-
-    :math:`T_\\mathrm{eff}(t) = (25\\,\\mathrm{kK}) a_{13}^{1/4} (M_c v_9^7)^{1/144} κ^{-35/144} t^{37/72}` (Eq. 2)
-
-    The SiFTO model (https://doi.org/10.1086/588518) is currently only available in the UBVgri filters.
+    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model.
 
     This version of the model includes time offsets for the U and i SiFTO models.
-
-    Parameters
-    ----------
-    t_in : float, array-like
-        Time in days
-    f : lightcurve_fitting.filter.Filter, array-like
-        Filters for which to calculate the model
-    t_exp : float, array-like
-        The explosion epoch
-    a13 : float, array-like
-        The binary separation in :math:`10^{13}` cm
-    Mc_v9_7 : float, array-like
-        The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
-        the ejecta velocity in units of :math:`10^9` cm/s
-    t_peak : float, array-like
-        The epoch of maximum light for the SiFTO model
-    stretch : float, array-like
-        The stretch for the SiFTO model
-    dtU, dti : float, array-like
-        Time offsets for the U- and i-band SiFTO models relative to the other bands
-    kappa : float, array-like
-        The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
-    z : float, optional
-        The redshift between blackbody source and the observed filters
-
-    Returns
-    -------
-    y_fit : array-like
-        The filtered model light curves
     """
-    Lnu_kasen = companion_shocking(t_in, f, t_exp, a13, Mc_v9_7, kappa, z)
-    Lnu_sifto = stretched_sifto(t_in, f, t_peak, stretch, dtU, dti)
-
-    kasen_factors = {'U': 1.}
-    y_fit = np.array([L1 * kasen_factors.get(filt.char, 1.) + L2 for L1, L2, filt in zip(Lnu_kasen, Lnu_sifto, f)])
-
-    return y_fit
-
-
-CompanionShocking2 = Model(companion_shocking_plus_sifto2,
-                          [
-                              't_0',
-                              'a',
-                              'M v^7',
-                              't_\\mathrm{max}',
-                              's',
-                              '\\Delta t_U',
-                              '\\Delta t_i',
-                          ],
-                          [
-                              u.d,
-                              10. ** 13. * u.cm,
-                              M_chandra * (1e9 * u.cm / u.s) ** 7,
-                              u.d,
-                              u.dimensionless_unscaled,
-                              u.d,
-                              u.d,
-                          ]
-                          )
+    input_names = [
+        't_0',
+        'a',
+        'M v^7',
+        't_\\mathrm{max}',
+        's',
+        '\\Delta t_U',
+        '\\Delta t_i',
+    ]
+    units = [
+        u.d,
+        10. ** 13. * u.cm,
+        M_chandra * (1e9 * u.cm / u.s) ** 7,
+        u.d,
+        u.dimensionless_unscaled,
+        u.d,
+        u.d,
+    ]
+
+    def evaluate(self, t_in, f, t_exp, a13, Mc_v9_7, t_peak, stretch, dtU=0., dti=0., kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        t_exp : float, array-like
+            The explosion epoch
+        a13 : float, array-like
+            The binary separation in :math:`10^{13}` cm
+        Mc_v9_7 : float, array-like
+            The product :math:`M_c v_9^7`, where :math:`M_c` is the ejecta mass in Chandrasekhar masses and :math:`v_9` is
+            the ejecta velocity in units of :math:`10^9` cm/s
+        t_peak : float, array-like
+            The epoch of maximum light for the SiFTO model
+        stretch : float, array-like
+            The stretch for the SiFTO model
+        dtU, dti : float, array-like
+            Time offsets for the U- and i-band SiFTO models relative to the other bands
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        Lnu_kasen = self.companion_shocking(t_in, f, t_exp, a13, Mc_v9_7, kappa)
+        Lnu_sifto = self.stretched_sifto(t_in, f, t_peak, stretch, dtU, dti)
+        y_fit = Lnu_kasen + Lnu_sifto
+        return y_fit
+
+
+class CompanionShocking3(BaseCompanionShocking):
+    """
+    The companion shocking model of Kasen (https://doi.org/10.1088/0004-637X/708/2/1025) plus the SiFTO SN Ia model.
+
+    This version of the model includes time offsets for the U and i SiFTO models, as well as the viewing angle
+    dependence parametrized by Brown et al. (https://doi.org/10.1088/0004-637X/749/1/18).
+    """
+    input_names = [
+        't_0',
+        'a',
+        '\\theta',
+        't_\\mathrm{max}',
+        's',
+        '\\Delta t_U',
+        '\\Delta t_i',
+    ]
+    units = [
+        u.d,
+        10. ** 13. * u.cm,
+        u.deg,
+        u.d,
+        u.dimensionless_unscaled,
+        u.d,
+        u.d,
+    ]
+
+    def evaluate(self, t_in, f, t_exp, a13, theta, t_peak, stretch, dtU, dti, kappa=1.):
+        """
+        Evaluate this model at a range of times and filters
+
+        Parameters
+        ----------
+        t_in : float, array-like
+            Time in days
+        f : lightcurve_fitting.filter.Filter, array-like
+            Filters for which to calculate the model
+        t_exp : float, array-like
+            The explosion epoch
+        a13 : float, array-like
+            The binary separation in :math:`10^{13}` cm
+        theta : float, array-like
+            The angle between the binary axis and the line to the observer in degrees. 0° means the binary companion
+            is along the line of sight.
+        t_peak : float, array-like
+            The epoch of maximum light for the SiFTO model
+        stretch : float, array-like
+            The stretch for the SiFTO model
+        dtU, dti : float, array-like
+            Time offsets for the U- and i-band SiFTO models relative to the other bands
+        kappa : float, array-like
+            The ejecta opacity in units of the electron scattering opacity (0.34 cm^2/g)
+
+        Returns
+        -------
+        y_fit : array-like
+            The filtered model light curves
+        """
+        Lnu_kasen = self.companion_shocking(t_in, f, t_exp, a13, 1., kappa)
+        Lnu_sifto = self.stretched_sifto(t_in, f, t_peak, stretch, dtU, dti)
+        theta_rad = np.deg2rad(theta)
+        fractional_flux = (0.5 * np.cos(theta_rad) + 0.5) * (0.14 * theta_rad ** 2. - 0.4 * theta_rad + 1.)
+        y_fit = Lnu_kasen * fractional_flux + Lnu_sifto
+        return y_fit
 
 
 class Prior:
     __metaclass__ = ABCMeta
 
     def __init__(self, p_min=-np.inf, p_max=np.inf):
         self.p_min = p_min
@@ -837,15 +962,15 @@
 
     Returns
     -------
     float, array-like
         The spectral luminosity density (:math:`L_ν`) of the source in watts per hertz
     """
     return c2 * np.squeeze(np.multiply.outer(R ** 2, nu ** 3 * np.minimum(1., cutoff_freq / nu))
-                           / (np.exp(c1 * np.multiply.outer(T ** -1, nu)) - 1))
+                           * power(np.exp(c1 * np.multiply.outer(power(T, -1.), nu)) - 1., -1.))
 
 
 def blackbody_to_filters(filters, T, R, z=0., cutoff_freq=np.inf, ebv=0.):
     """
     The average spectral luminosity density (:math:`L_ν`) of a blackbody as observed through one or more filters
 
     Parameters
@@ -869,15 +994,15 @@
     y_fit : float, array-like
         The average spectral luminosity density in each filter in watts per hertz
     """
     T = np.array(T)
     R = np.array(R)
     if T.shape != R.shape:
         raise Exception('T & R must have the same shape')
-    np.broadcast(T, ebv)  # check if T and ebv are brodcastable, otherwise raise a ValueError
+    np.broadcast(T, ebv)  # check if T and ebv are broadcastable, otherwise raise a ValueError
     if T.ndim == 1 and len(T) == len(filters):  # pointwise
         y_fit = np.array([f.synthesize(planck_fast, t, r, cutoff_freq, z=z, ebv=ebv) for f, t, r in zip(filters, T, R)])
     else:
         y_fit = np.array([f.synthesize(planck_fast, T, R, cutoff_freq, z=z, ebv=ebv) for f in filters])
     return y_fit
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting/speccal.py` & `lightcurve-fitting-0.8.0/lightcurve_fitting/speccal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 
 import numpy as np
 from .lightcurve import LC
-from .filters import filtdict
 from astropy import constants as const, units as u
 from astropy.io import fits, ascii
 from astropy.wcs import WCS
 from astropy.time import Time
 from astropy.table import Table
 import argparse
 import matplotlib.pyplot as plt
@@ -141,15 +140,15 @@
         warnings.simplefilter('ignore')
         flux = u.Quantity(flux, bunit).to(default_bunit, u.equivalencies.spectral_density(wl))
     return wl.value, flux.value
 
 
 def readOSCspec(filepath):
     """
-    Read spectra from a JSON file from the Open Supernova Catalog (https://sne.space)
+    Read spectra from a JSON file in the Open Astronomy Catalog schema (https://github.com/astrocatalogs/schema)
 
     Parameters
     ----------
     filepath : str
         Path to the JSON file containing the spectra
 
     Returns
@@ -342,23 +341,27 @@
         Polynomial order for the calibration function. Default: 0 (constant factor)
     subtract_percentile : float, optional
         Subtract flux corresponding to this percentile of the spectrum before calibration. Default: no subtraction
     max_extrapolate : float, optional
         Assume constant flux in a filter for this many days after the last observed point. Default: 1 day.
     show : bool, optional
         Plot the observed light curve and the uncalibrated and calibrated spectra, and ask whether to save the results
+
+    Returns
+    -------
+    fig : matplotlib.pyplot.Figure
+        If `show=True`, the Figure object is returned
     """
     if filters is not None:
-        lc = lc.where(filter=[filtdict[f] for f in filters])
+        lc = lc.where(filter=filters)
     lc.calcFlux()
     lc.sort('MJD')
     filts = set(lc['filter'])
 
     for filt in filts:
-        filt.read_curve()
         filt.trans.sort('freq')
 
     plt.ion()
     fig = plt.figure(figsize=(8., 6.))
 
     for spec in spectra:
         wl, flux, time, _, _ = readspec(spec)
@@ -407,31 +410,33 @@
             continue
         scale = np.mean(ratios)
         if order:
             p = np.polyfit(freqs, np.array(ratios) / scale, order)
             corr = np.polyval(p, nu) * scale
             print(spec, scale, p[:-1])
         else:
-            corr = scale
+            corr = np.array([scale])
             print(spec, scale)
         if show:
             ax2.plot(nu, Fnu * scale, label='rescaled')
             ax2.set_xlabel('Frequency (THz)')
             ax2.set_ylabel('$F_\\nu$ (W Hz$^{-1}$)')
             if order:
                 ax2.plot(nu, Fnu * corr, color='C2', label='rescaled & warped')
                 plt.legend(loc='best')
             plt.pause(0.1)
             ans = input('accept this scale? [Y/n] ')
         if not show or ans.lower() != 'n':
-            data_out = np.array([wl[good], flux[good] * corr]).T
+            data_out = np.array([wl[good], flux[good] * corr[::-1]]).T
             path_in, filename_in = os.path.split(spec)
             filename_out = os.path.join(path_in, 'photcal_' + filename_in).replace('.fits', '.txt')
             np.savetxt(filename_out, data_out, fmt='%.1f %.2e')
             print(filename_out)
+    if show:
+        return fig
 
 
 def create_wiserep_tsv(specpaths, wiserep_dir, verbose=False):
     """
     Prepares a TSV file for uploading spectra to WISeREP (see https://www.wiserep.org/content/wiserep-getting-started).
 
     Also copies all the spectrum files to a single directory, and converts any FITS files to ASCII.
@@ -568,17 +573,17 @@
         f.write('\n'.join(lines) + '\n')
     if verbose:
         print(f'\nwrote {wiserep_dir}.tsv')
     return t
 
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Calibrate spectra of a supernova to photometry.')
+    parser = argparse.ArgumentParser(description='Calibrate spectra to photometry.')
     parser.add_argument('spectra', nargs='+', help='filenames of spectra')
-    parser.add_argument('--lc', help='filename of photometry table (must have columns "MJD", "filt", "mag"/"flux", and'
+    parser.add_argument('--lc', help='filename of photometry table (must have columns "MJD", "filter", "mag"/"flux", and'
                                      '"dmag"/"dflux")')
     parser.add_argument('--lc-format', default='ascii',
                         help='format of photometry table (passed to :func:`astropy.table.Table.read`)')
     parser.add_argument('-f', '--filters', nargs='+', help='filters to use for calibration')
     parser.add_argument('-o', '--order', type=int, default=0, help='polynomial order of correction function')
     parser.add_argument('--subtract-percentile', type=float, help='subtract continuum from spectrum before correcting')
     parser.add_argument('--max-extrapolate', type=float,
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/PKG-INFO` & `lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurve-fitting
-Version: 0.7.0
+Version: 0.8.0
 Summary: Tools to fit analytical models to multiband light curves of astronomical transients
 Home-page: https://github.com/griffin-h/lightcurve_fitting
 Author: Griffin Hosseinzadeh
 Author-email: griffin0@arizona.edu
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lightcurve-fitting-0.7.0/lightcurve_fitting.egg-info/SOURCES.txt` & `lightcurve-fitting-0.8.0/lightcurve_fitting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,18 @@
 lightcurve_fitting/filters/JWST_MIRI.F770W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F070W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F090W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F115W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F150W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F200W.dat
 lightcurve_fitting/filters/JWST_NIRCam.F277W.dat
+lightcurve_fitting/filters/JWST_NIRCam.F300M.dat
+lightcurve_fitting/filters/JWST_NIRCam.F335M.dat
 lightcurve_fitting/filters/JWST_NIRCam.F356W.dat
+lightcurve_fitting/filters/JWST_NIRCam.F360M.dat
 lightcurve_fitting/filters/JWST_NIRCam.F444W.dat
 lightcurve_fitting/filters/KAF-1001E.asci
 lightcurve_fitting/filters/KAF-1001E.csv
 lightcurve_fitting/filters/Kepler_Kepler.K.dat
 lightcurve_fitting/filters/PAN-STARRS_PS1.w.dat
 lightcurve_fitting/filters/PAN-STARRS_PS1.y.dat
 lightcurve_fitting/filters/PAN-STARRS_PS1.z.dat
```

### Comparing `lightcurve-fitting-0.7.0/setup.py` & `lightcurve-fitting-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightcurve-fitting-0.7.0/versioneer.py` & `lightcurve-fitting-0.8.0/versioneer.py`

 * *Files identical despite different names*

