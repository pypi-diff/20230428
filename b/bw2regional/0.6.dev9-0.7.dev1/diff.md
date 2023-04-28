# Comparing `tmp/bw2regional-0.6.dev9.tar.gz` & `tmp/bw2regional-0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2regional-0.6.dev9.tar", last modified: Tue Apr 25 12:25:39 2023, max compression
+gzip compressed data, was "bw2regional-0.7.dev1.tar", last modified: Fri Apr 28 07:50:18 2023, max compression
```

## Comparing `bw2regional-0.6.dev9.tar` & `bw2regional-0.7.dev1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.050553 bw2regional-0.6.dev9/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.036531 bw2regional-0.6.dev9/.github/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 chrismutel   (501) staff       (20)     1203 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.gitignore
--rw-r--r--   0 chrismutel   (501) staff       (20)      142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/.hgignore
--rw-r--r--   0 chrismutel   (501) staff       (20)     1672 2023-04-25 12:25:29.000000 bw2regional-0.6.dev9/CHANGES.md
--rw-r--r--   0 chrismutel   (501) staff       (20)     1457 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/LICENSE.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       81 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 12:25:39.050423 bw2regional-0.6.dev9/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      419 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.040406 bw2regional-0.6.dev9/bw2regional/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2257 2023-04-25 05:20:45.000000 bw2regional-0.6.dev9/bw2regional/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4747 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/base_data.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2130 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/databases.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2157 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/density.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1113 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7298 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/export.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     5358 2023-04-25 12:20:54.000000 bw2regional-0.6.dev9/bw2regional/gis_tasks.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      314 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/hashing.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2549 2023-04-25 05:20:21.000000 bw2regional-0.6.dev9/bw2regional/intersection.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.043002 bw2regional-0.6.dev9/bw2regional/lca/
--rw-r--r--   0 chrismutel   (501) staff       (20)      255 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9619 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/base_class.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    12923 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/extension_tables.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2170 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/one_spatial_scale.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3145 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3656 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales_weighting.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1825 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/loading.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1958 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/meta.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     9405 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/pandarus.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    10293 2023-04-24 21:18:52.000000 bw2regional-0.6.dev9/bw2regional/pandarus_remote.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2818 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/topography.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8910 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1142 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/validate.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       25 2023-04-25 12:21:01.000000 bw2regional-0.6.dev9/bw2regional/version.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1601 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/bw2regional/xtables.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.041365 bw2regional-0.6.dev9/bw2regional.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     1937 2023-04-25 12:25:39.000000 bw2regional-0.6.dev9/bw2regional.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)      138 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-25 12:25:38.000000 bw2regional-0.6.dev9/bw2regional.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.044864 bw2regional-0.6.dev9/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6786 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/Makefile
--rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/base-data.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     1079 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/common.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     9331 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8777 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/formats.rst
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.044998 bw2regional-0.6.dev9/docs/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)   149543 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/images/mnglr.png
--rw-r--r--   0 chrismutel   (501) staff       (20)     8945 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/index.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     4846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/lca.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     1994 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/libraries.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)     6713 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/make.bat
--rw-r--r--   0 chrismutel   (501) staff       (20)      846 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/docs/technical.rst
--rw-r--r--   0 chrismutel   (501) staff       (20)       40 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/pytest.ini
--rw-r--r--   0 chrismutel   (501) staff       (20)        9 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/requirements.rtd.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)      139 2023-04-25 05:23:45.000000 bw2regional-0.6.dev9/requirements.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-25 12:25:39.050590 bw2regional-0.6.dev9/setup.cfg
--rw-r--r--   0 chrismutel   (501) staff       (20)     1562 2023-04-25 05:24:03.000000 bw2regional-0.6.dev9/setup.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.047659 bw2regional-0.6.dev9/tests/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-25 12:25:39.050189 bw2regional-0.6.dev9/tests/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2600 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-cfs.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      213 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-countries.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      491 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/areas-topo.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)     4698 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/density_fixture.tiff
--rw-r--r--   0 chrismutel   (501) staff       (20)     1635 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-countries-cfs.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)      477 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-countries-provinces.json.bz2
--rw-r--r--   0 chrismutel   (501) staff       (20)     4215 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/intersect-topo-cfs.json.bz2
--rwxr-xr-x   0 chrismutel   (501) staff       (20)      523 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/pandarus-commands.sh
--rw-r--r--   0 chrismutel   (501) staff       (20)   131072 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_countries.gpkg
--rw-r--r--   0 chrismutel   (501) staff       (20)   225280 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_provinces.gpkg
--rw-r--r--   0 chrismutel   (501) staff       (20)     3936 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_raster_cfs.tif
--rw-r--r--   0 chrismutel   (501) staff       (20)     1336 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_raster_loading.tif
--rw-r--r--   0 chrismutel   (501) staff       (20)      220 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/data/test_topo_mapping.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     5837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_density.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      861 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_intersections.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1239 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_lca.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1175 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_loading.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2304 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_meta.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4837 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_one_spatial_scale.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1438 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_pandarus.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3054 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_setup.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      185 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_topography.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     6242 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_two_spatial_scales.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7705 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_two_spatial_scales_weighting.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1517 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      212 2023-04-24 18:26:16.000000 bw2regional-0.6.dev9/tests/test_xtables.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.606660 bw2regional-0.7.dev1/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.594136 bw2regional-0.7.dev1/.github/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3220 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1203 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/.gitignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)      142 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/.hgignore
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1762 2023-04-26 07:20:11.000000 bw2regional-0.7.dev1/CHANGES.md
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1457 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/LICENSE.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       81 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-28 07:50:18.606501 bw2regional-0.7.dev1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      419 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.597405 bw2regional-0.7.dev1/bw2regional/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2257 2023-04-25 05:20:45.000000 bw2regional-0.7.dev1/bw2regional/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4747 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/base_data.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2130 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/databases.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2157 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1113 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7298 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/export.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5358 2023-04-25 12:20:54.000000 bw2regional-0.7.dev1/bw2regional/gis_tasks.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      314 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/hashing.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2549 2023-04-25 05:20:21.000000 bw2regional-0.7.dev1/bw2regional/intersection.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.598919 bw2regional-0.7.dev1/bw2regional/lca/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      255 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/lca/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9866 2023-04-26 07:18:05.000000 bw2regional-0.7.dev1/bw2regional/lca/base_class.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13145 2023-04-28 07:49:33.000000 bw2regional-0.7.dev1/bw2regional/lca/extension_tables.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2170 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/lca/one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3145 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/lca/two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3656 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/lca/two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1825 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1958 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9405 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    10293 2023-04-24 21:18:52.000000 bw2regional-0.7.dev1/bw2regional/pandarus_remote.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2818 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8910 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1142 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/validate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       25 2023-04-28 07:49:42.000000 bw2regional-0.7.dev1/bw2regional/version.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1601 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/bw2regional/xtables.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.597965 bw2regional-0.7.dev1/bw2regional.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1357 2023-04-28 07:50:18.000000 bw2regional-0.7.dev1/bw2regional.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1937 2023-04-28 07:50:18.000000 bw2regional-0.7.dev1/bw2regional.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-28 07:50:18.000000 bw2regional-0.7.dev1/bw2regional.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      138 2023-04-28 07:50:18.000000 bw2regional-0.7.dev1/bw2regional.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-04-28 07:50:18.000000 bw2regional-0.7.dev1/bw2regional.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.601372 bw2regional-0.7.dev1/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6786 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/Makefile
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1506 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/base-data.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1079 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/common.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9331 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8777 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/formats.rst
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.601507 bw2regional-0.7.dev1/docs/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   149543 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/images/mnglr.png
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8945 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/index.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4846 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/lca.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1994 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/libraries.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6713 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/make.bat
+-rw-r--r--   0 chrismutel   (501) staff       (20)      846 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/docs/technical.rst
+-rw-r--r--   0 chrismutel   (501) staff       (20)       40 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/pytest.ini
+-rw-r--r--   0 chrismutel   (501) staff       (20)        9 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/requirements.rtd.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)      139 2023-04-25 05:23:45.000000 bw2regional-0.7.dev1/requirements.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       38 2023-04-28 07:50:18.606701 bw2regional-0.7.dev1/setup.cfg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1562 2023-04-25 05:24:03.000000 bw2regional-0.7.dev1/setup.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.603697 bw2regional-0.7.dev1/tests/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-28 07:50:18.606236 bw2regional-0.7.dev1/tests/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2600 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/areas-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      213 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/areas-countries.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      491 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/areas-topo.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4698 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/density_fixture.tiff
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1635 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/intersect-countries-cfs.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)      477 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/intersect-countries-provinces.json.bz2
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4215 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/intersect-topo-cfs.json.bz2
+-rwxr-xr-x   0 chrismutel   (501) staff       (20)      523 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/pandarus-commands.sh
+-rw-r--r--   0 chrismutel   (501) staff       (20)   131072 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/test_countries.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)   225280 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/test_provinces.gpkg
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3936 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/test_raster_cfs.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1336 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/test_raster_loading.tif
+-rw-r--r--   0 chrismutel   (501) staff       (20)      220 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/data/test_topo_mapping.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5837 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_density.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      861 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_intersections.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1239 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_lca.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1175 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_loading.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2304 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_meta.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4837 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_one_spatial_scale.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1438 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_pandarus.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3054 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_setup.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      185 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_topography.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6242 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_two_spatial_scales.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7705 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_two_spatial_scales_weighting.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1517 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      212 2023-04-24 18:26:16.000000 bw2regional-0.7.dev1/tests/test_xtables.py
```

### Comparing `bw2regional-0.6.dev9/.github/CODE_OF_CONDUCT.md` & `bw2regional-0.7.dev1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/.gitignore` & `bw2regional-0.7.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/CHANGES.md` & `bw2regional-0.7.dev1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # regional Changelog
 
+## 0.6.DEV10 (2023-04-26)
+
+* Add `extra_data_objs` parameter to regionalized LCA classes
+
 ## 0.6.DEV9 (2023-04-25)
 
 * Fix bug in calling Geopandas
 
 ## 0.6.DEV8 (2023-04-24)
 
 * Add `calculate_needed_intersections` function
```

### Comparing `bw2regional-0.6.dev9/LICENSE.txt` & `bw2regional-0.7.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/PKG-INFO` & `bw2regional-0.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev9
+Version: 0.7.dev1
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2regional-0.6.dev9/bw2regional/__init__.py` & `bw2regional-0.7.dev1/bw2regional/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/base_data.py` & `bw2regional-0.7.dev1/bw2regional/base_data.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/databases.py` & `bw2regional-0.7.dev1/bw2regional/databases.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/density.py` & `bw2regional-0.7.dev1/bw2regional/density.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/errors.py` & `bw2regional-0.7.dev1/bw2regional/errors.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/export.py` & `bw2regional-0.7.dev1/bw2regional/export.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/gis_tasks.py` & `bw2regional-0.7.dev1/bw2regional/gis_tasks.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/intersection.py` & `bw2regional-0.7.dev1/bw2regional/intersection.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/lca/base_class.py` & `bw2regional-0.7.dev1/bw2regional/lca/base_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         "flow_categories": str(flow.get("categories", "")),
     }
 
 
 class RegionalizationBase(LCA):
     def __init__(self, demand, *args, **kwargs):
         self.databases = get_dependent_databases(demand)
+        self.extra_data_objs = kwargs.pop("extra_data_objs", [])
         super(RegionalizationBase, self).__init__(demand, *args, **kwargs)
 
     def get_inventory_geocollections(self):
         """Get the set of all needed inventory geocollections.
 
         Raise UnprocessedDatabase if any database is missing the required metadata."""
         missing, present = [], set()
@@ -65,15 +66,17 @@
 
         Uses ``self.technosphere_mm.row_mapper`` and ``self.databases``.
 
         Creates ``self.inv_mapping_mm``, ``self.inv_mapping_matrix``, and ``self.dicts.inv_spatial``/
 
         """
         self.inv_mapping_mm = mu.MappedMatrix(
-            packages=[dp(Database(x).filepath_processed()) for x in self.databases],
+            packages=[
+                dp(Database(x).filepath_processed()) for x in self.databases
+            ] + self.extra_data_objs,
             matrix="inv_geomapping_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             row_mapper=self.technosphere_mm.col_mapper,
         )
         self.inv_mapping_matrix = self.inv_mapping_mm.matrix
@@ -103,15 +106,15 @@
             * ``geo_transform_matrix``: The matrix **G**
 
         """
         self.geo_transform_mm = mu.MappedMatrix(
             packages=[
                 dp(Intersection(name).filepath_processed())
                 for name in self.needed_intersections()
-            ],
+            ] + self.extra_data_objs,
             matrix="intersection_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             col_mapper=self.reg_cf_mm.row_mapper,
             row_mapper=self.inv_mapping_mm.col_mapper,
         )
@@ -127,15 +130,17 @@
         Returns:
             * ``reg_cf_params``: Parameter array with row/col of IA locations/biosphere flows
             * ``ia_spatial_dict``: Dictionary linking impact assessment locations to matrix rows
             * ``reg_cf_matrix``: The matrix **R**
 
         """
         self.reg_cf_mm = mu.MappedMatrix(
-            packages=[dp(Method(self.method).filepath_processed())],
+            packages=[
+                dp(Method(self.method).filepath_processed())
+            ] + self.extra_data_objs,
             matrix="characterization_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             col_mapper=self.biosphere_mm.row_mapper,
             row_mapper=row_mapper,
             transpose=True,
@@ -147,15 +152,17 @@
     def create_loading_matrix(self):
         """Get diagonal regionalized loading matrix, **L**, which gives location-specific background loading factors. Dimensions are impact assessment spatial units.
 
         Uses ``self.dicts.ia_spatial``.
 
         """
         self.loading_mm = mu.MappedMatrix(
-            packages=[dp(self.loading.filepath_processed())],
+            packages=[
+                dp(self.loading.filepath_processed())
+            ] + self.extra_data_objs,
             matrix="loading_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             diagonal=True,
             row_mapper=self.reg_cf_mm.row_mapper,
         )
```

### Comparing `bw2regional-0.6.dev9/bw2regional/lca/extension_tables.py` & `bw2regional-0.7.dev1/bw2regional/lca/extension_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,40 +123,45 @@
                 error_text += "\n"
             if missing_xtable_ia_inters:
                 error_text += "Intersections between extension tables and IA method:"
                 error_text += "\n\t".join([str(x) for x in missing_xtable_ia_inters])
             raise MissingIntersection(error_text)
 
     def get_xtable_geodata(self):
-        gc = self.xtable_meta["geocollection"]
+        if "geocollection" in self.xtable_meta:
+            gcs = [self.xtable_meta["geocollections"]]
+        else:
+            gcs = self.xtable_meta["geocollections"]
         return (
-            [gc],  # Only one geocollection per extension table, but need list
-            {x for x in intersections if x[1] == gc},
+            gcs,  # Only one geocollection per extension table, but need list
+            {x for x in intersections if x[1] in gcs},
         )
 
     def create_distribution_matrix(self):
         """Get distribution matrix, **D**, which provides the area of inventory spatial units in each extension table spatial unit. Rows are inventory spatial units and columns are extension table spatial units."""
         self.distribution_mm = mu.MappedMatrix(
             packages=[
                 dp(Intersection(name).filepath_processed())
                 for name in self.inv_xtable_intersections
-            ],
+            ] + self.extra_data_objs,
             matrix="intersection_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             row_mapper=self.inv_mapping_mm.col_mapper,
         )
         self.distribution_matrix = self.distribution_mm.matrix
         self.dicts.xtable_spatial = partial(self.distribution_mm.col_mapper.to_dict)
 
     def create_xtable_matrix(self):
         """Diagonal extension table matrix that indicates the extension table density value in each extension table spatial unit."""
         self.xtable_mm = mu.MappedMatrix(
-            packages=[dp(self.xtable.filepath_processed())],
+            packages=[
+                dp(self.xtable.filepath_processed())
+            ] + self.extra_data_objs,
             matrix="xtable_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             diagonal=True,
             row_mapper=self.distribution_mm.col_mapper,
         )
@@ -187,15 +192,15 @@
         return diags(vector, [0], format="csr", dtype=np.float32)
 
     def create_geo_transform_matrix(self):
         self.geo_transform_mm = mu.MappedMatrix(
             packages=[
                 dp(Intersection(name).filepath_processed())
                 for name in self.xtable_ia_intersections
-            ],
+            ] + self.extra_data_objs,
             matrix="intersection_matrix",
             use_arrays=self.use_arrays,
             use_distributions=self.use_distributions,
             seed_override=self.seed_override,
             col_mapper=self.reg_cf_mm.row_mapper,
             row_mapper=self.distribution_mm.col_mapper,
         )
```

### Comparing `bw2regional-0.6.dev9/bw2regional/lca/one_spatial_scale.py` & `bw2regional-0.7.dev1/bw2regional/lca/one_spatial_scale.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales.py` & `bw2regional-0.7.dev1/bw2regional/lca/two_spatial_scales.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/lca/two_spatial_scales_weighting.py` & `bw2regional-0.7.dev1/bw2regional/lca/two_spatial_scales_weighting.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/loading.py` & `bw2regional-0.7.dev1/bw2regional/loading.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/meta.py` & `bw2regional-0.7.dev1/bw2regional/meta.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/pandarus.py` & `bw2regional-0.7.dev1/bw2regional/pandarus.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/pandarus_remote.py` & `bw2regional-0.7.dev1/bw2regional/pandarus_remote.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/topography.py` & `bw2regional-0.7.dev1/bw2regional/topography.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/utils.py` & `bw2regional-0.7.dev1/bw2regional/utils.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/validate.py` & `bw2regional-0.7.dev1/bw2regional/validate.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional/xtables.py` & `bw2regional-0.7.dev1/bw2regional/xtables.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/bw2regional.egg-info/PKG-INFO` & `bw2regional-0.7.dev1/bw2regional.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2regional
-Version: 0.6.dev9
+Version: 0.7.dev1
 Home-page: https://github.com/brightway-lca/brightway2-regional
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2regional-0.6.dev9/bw2regional.egg-info/SOURCES.txt` & `bw2regional-0.7.dev1/bw2regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/Makefile` & `bw2regional-0.7.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/base-data.rst` & `bw2regional-0.7.dev1/docs/base-data.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/common.rst` & `bw2regional-0.7.dev1/docs/common.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/conf.py` & `bw2regional-0.7.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/formats.rst` & `bw2regional-0.7.dev1/docs/formats.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/images/mnglr.png` & `bw2regional-0.7.dev1/docs/images/mnglr.png`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/index.rst` & `bw2regional-0.7.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/lca.rst` & `bw2regional-0.7.dev1/docs/lca.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/libraries.rst` & `bw2regional-0.7.dev1/docs/libraries.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/make.bat` & `bw2regional-0.7.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/docs/technical.rst` & `bw2regional-0.7.dev1/docs/technical.rst`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/setup.py` & `bw2regional-0.7.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/areas-cfs.json.bz2` & `bw2regional-0.7.dev1/tests/data/areas-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/density_fixture.tiff` & `bw2regional-0.7.dev1/tests/data/density_fixture.tiff`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/intersect-countries-cfs.json.bz2` & `bw2regional-0.7.dev1/tests/data/intersect-countries-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/intersect-topo-cfs.json.bz2` & `bw2regional-0.7.dev1/tests/data/intersect-topo-cfs.json.bz2`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/pandarus-commands.sh` & `bw2regional-0.7.dev1/tests/data/pandarus-commands.sh`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/test_countries.gpkg` & `bw2regional-0.7.dev1/tests/data/test_countries.gpkg`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/test_provinces.gpkg` & `bw2regional-0.7.dev1/tests/data/test_provinces.gpkg`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/test_raster_cfs.tif` & `bw2regional-0.7.dev1/tests/data/test_raster_cfs.tif`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/data/test_raster_loading.tif` & `bw2regional-0.7.dev1/tests/data/test_raster_loading.tif`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_density.py` & `bw2regional-0.7.dev1/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_intersections.py` & `bw2regional-0.7.dev1/tests/test_intersections.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_lca.py` & `bw2regional-0.7.dev1/tests/test_lca.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_loading.py` & `bw2regional-0.7.dev1/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_meta.py` & `bw2regional-0.7.dev1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_one_spatial_scale.py` & `bw2regional-0.7.dev1/tests/test_one_spatial_scale.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_pandarus.py` & `bw2regional-0.7.dev1/tests/test_pandarus.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_setup.py` & `bw2regional-0.7.dev1/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_two_spatial_scales.py` & `bw2regional-0.7.dev1/tests/test_two_spatial_scales.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_two_spatial_scales_weighting.py` & `bw2regional-0.7.dev1/tests/test_two_spatial_scales_weighting.py`

 * *Files identical despite different names*

### Comparing `bw2regional-0.6.dev9/tests/test_utils.py` & `bw2regional-0.7.dev1/tests/test_utils.py`

 * *Files identical despite different names*

