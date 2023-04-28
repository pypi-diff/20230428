# Comparing `tmp/SciFiReaders-0.0.8.tar.gz` & `tmp/SciFiReaders-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciFiReaders-0.0.8.tar", last modified: Sat Feb  4 22:52:16 2023, max compression
+gzip compressed data, was "SciFiReaders-0.0.9.tar", last modified: Fri Apr 28 20:58:44 2023, max compression
```

## Comparing `SciFiReaders-0.0.8.tar` & `SciFiReaders-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.327714 SciFiReaders-0.0.8/SciFiReaders/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.327714 SciFiReaders-0.0.8/SciFiReaders/readers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/SID/
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/SID/Nsid_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/SID/Usid_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/SID/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/converters/hyperspy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/generic/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/dm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/emd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/nion_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/stem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/stem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/ion/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/ion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
--rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/pifm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/SciFiReaders/readers/spectroscopy/
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/spectroscopy/SpeReader.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/SciFiReaders/readers/spectroscopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 22:52:16.327714 SciFiReaders-0.0.8/SciFiReaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-04 22:52:16.000000 SciFiReaders-0.0.8/SciFiReaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-02-04 22:52:16.000000 SciFiReaders-0.0.8/SciFiReaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 22:52:16.000000 SciFiReaders-0.0.8/SciFiReaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-04 22:52:16.000000 SciFiReaders-0.0.8/SciFiReaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-04 22:52:16.000000 SciFiReaders-0.0.8/SciFiReaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-04 22:52:16.331714 SciFiReaders-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-04 22:50:27.000000 SciFiReaders-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.637819 SciFiReaders-0.0.9/SciFiReaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/SID/
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/Nsid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/Usid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/SID/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/converters/hyperspy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/generic/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/dm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/emd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/nion_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/stem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/stem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/ion/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/ion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20352 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/mdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/pifm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/SpeReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:58:44.641819 SciFiReaders-0.0.9/SciFiReaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 20:58:44.000000 SciFiReaders-0.0.9/SciFiReaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 20:58:44.645819 SciFiReaders-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-28 20:56:39.000000 SciFiReaders-0.0.9/setup.py
```

### Comparing `SciFiReaders-0.0.8/LICENSE` & `SciFiReaders-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/PKG-INFO` & `SciFiReaders-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciFiReaders
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for extracting data and metadata from scientific data files
 Home-page: https://pycroscopy.github.io/SciFiReaders/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific
 Platform: Linux
```

### Comparing `SciFiReaders-0.0.8/README.rst` & `SciFiReaders-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/ingestor.py` & `SciFiReaders-0.0.9/SciFiReaders/ingestor.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/SID/Nsid_reader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/SID/Nsid_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/SID/Usid_reader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/SID/Usid_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/converters/hyperspy.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/converters/hyperspy.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/generic/image.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/generic/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Translates data from an image file to a sidpy dataset
     """
 
     def __init__(self, file_path, *args, **kwargs):
         super().__init__(file_path, *args, **kwargs)
         image_path = self._parse_file_path(self._input_file_path)
         ext = os.path.splitext(image_path)[-1]
-        if ext not in ['jpg', 'jpeg', 'png', 'bmp', '.tif', '.tiff']:
+        if ext not in ['.jpg', '.jpeg', '.png', '.bmp', '.tif', '.tiff']:
             raise NotImplementedError(
                 'The provided file type {} is not supported by the reader as of now \n'.format(ext)
                 + 'Please provide one of "jpg", "jpeg", "png", "bmp", ".tif", ".tiff" file types')
 
     @staticmethod
     def _parse_file_path(image_path):
         """
@@ -119,15 +119,15 @@
         Array containing the image from the file `image_path`.
     """
 
     # As of now we are not trying to read any metadata from these image formats.
     # We will cross that bridge when someone raises an issue
     ext = os.path.splitext(image_path)[-1]
     original_metadata, metadata, dimensions = {}, {}, []
-    if ext in ['jpg', 'jpeg', 'png', 'bmp']:
+    if ext in ['.jpg', '.jpeg', '.png', '.bmp']:
         img_data = np.asarray(PIL.Image.open(image_path))
         # Colored images, color channel last
         # Here we assume that the file path provided has a single image and not a stack
         # For stacks we turn our attention to tiff
         if len(img_data.shape) == 3:
             dimensions.append(Dimension(np.arange(img_data.shape[0]), 'y',
                                         units='generic', quantity='Length',
```

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/dm_reader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/dm_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/emd_reader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/emd_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/em/tem/nion_reader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/em/tem/nion_reader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,31 +69,34 @@
             data_filepath = os.path.abspath(file_path)
             ARh5_file = h5py.File(data_filepath, 'r')
         except:
             print('Unable to open the file', data_filepath)
             raise
 
         # Get info from the origin file like Notes and Segments
-        decode_text = True
-        if type(ARh5_file.attrs['Note']) is str: decode_text = False
-        
-        if decode_text: self.notes = ARh5_file.attrs['Note'].decode('utf-8')
-        else: self.notes = ARh5_file.attrs['Note']
+        try:
+            self.notes = ARh5_file.attrs['Note'].decode('utf-8')
+        except AttributeError:
+            self.notes = ARh5_file.attrs['Note']
 
         self.segments = ARh5_file['ForceMap']['0']['Segments']
         segments_name = list(ARh5_file['ForceMap']['0'].attrs['Segments'])
-        
-        if decode_text: self.segments_name = [name.decode('utf-8') for name in segments_name]
-        else: self.segments_name = [name for name in segments_name]
+        try:
+            self.segments_name = [name.decode('utf-8') for name in segments_name]
+        except AttributeError:
+            self.segments_name = [name for name in segments_name]
 
         self.map_size['X'] = ARh5_file['ForceMap']['0']['Segments'].shape[0]
         self.map_size['Y'] = ARh5_file['ForceMap']['0']['Segments'].shape[1]
         channels_name = list(ARh5_file['ForceMap']['0'].attrs['Channels'])
-        if decode_text: self.channels_name = [name.decode('utf-8') for name in channels_name]
-        else: self.channels_name = [name for name in channels_name]
+        
+        try:
+            self.channels_name = [name.decode('utf-8') for name in channels_name]
+        except AttributeError:
+            self.channels_name = [name for name in channels_name]
 
         try:
             self.points_per_sec = np.float(self.note_value('ARDoIVPointsPerSec'))
         except NameError:
             self.points_per_sec = np.float(self.note_value('NumPtsPerSec'))
 
         if self.verbose:
```

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/base_utils.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/base_utils.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/gwyddion.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 if sys.version_info.major == 3:
     unicode = str
 
 try:
     import gwyfile
 except ModuleNotFoundError:
+    print("You don't have gwyfile installed. \
+    If you wish to open .gwy files, you will need to \
+     install it (pip install gwyfile) before attempting.")
     gwyfile = None
 
 class GwyddionReader(Reader):
     """
     Extracts data and metadata from Igor Binary Wave (.ibw) files containing
     images or force curves
     """
```

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/afm/pifm.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/afm/pifm.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders/readers/spectroscopy/SpeReader.py` & `SciFiReaders-0.0.9/SciFiReaders/readers/spectroscopy/SpeReader.py`

 * *Files identical despite different names*

### Comparing `SciFiReaders-0.0.8/SciFiReaders.egg-info/PKG-INFO` & `SciFiReaders-0.0.9/SciFiReaders.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciFiReaders
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for extracting data and metadata from scientific data files
 Home-page: https://pycroscopy.github.io/SciFiReaders/about.html
 Author: Pycroscopy contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Keywords: imaging,spectra,multidimensional,scientific
 Platform: Linux
```

### Comparing `SciFiReaders-0.0.8/SciFiReaders.egg-info/SOURCES.txt` & `SciFiReaders-0.0.9/SciFiReaders.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 SciFiReaders/readers/microscopy/spm/__init__.py
 SciFiReaders/readers/microscopy/spm/afm/AR_hdf5.py
 SciFiReaders/readers/microscopy/spm/afm/__init__.py
 SciFiReaders/readers/microscopy/spm/afm/base_utils.py
 SciFiReaders/readers/microscopy/spm/afm/bruker_nano.py
 SciFiReaders/readers/microscopy/spm/afm/gwyddion.py
 SciFiReaders/readers/microscopy/spm/afm/igor_ibw.py
+SciFiReaders/readers/microscopy/spm/afm/mdt.py
 SciFiReaders/readers/microscopy/spm/afm/pifm.py
 SciFiReaders/readers/microscopy/spm/stm/__init__.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_3ds.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_dat.py
 SciFiReaders/readers/microscopy/spm/stm/nanonis_sxm.py
 SciFiReaders/readers/microscopy/spm/stm/omicron_asc.py
 SciFiReaders/readers/spectroscopy/SpeReader.py
```

### Comparing `SciFiReaders-0.0.8/setup.py` & `SciFiReaders-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 requirements = [  # basic
                 'numpy>=1.10',
                 'toolz',  # dask installation failing without this
                 'cytoolz',  # dask installation failing without this
                 'dask>=2.20.0',
                 'sidpy>=0.11.2',
                 'numba',
+                'ipython==7.1.0'
                 # generic:
                 # Reader specific ones go to extras
                ]
 
 setup(
     name='SciFiReaders',
     version=__version__,
```

