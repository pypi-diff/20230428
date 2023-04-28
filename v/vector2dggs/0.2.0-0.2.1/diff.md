# Comparing `tmp/vector2dggs-0.2.0.tar.gz` & `tmp/vector2dggs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.2.0.tar", max compression
+gzip compressed data, was "vector2dggs-0.2.1.tar", max compression
```

## Comparing `vector2dggs-0.2.0.tar` & `vector2dggs-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7644 2023-04-27 01:25:13.759218 vector2dggs-0.2.0/README.md
--rw-r--r--   0        0        0     1092 2023-04-27 01:24:44.707080 vector2dggs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 21:07:25.956152 vector2dggs-0.2.0/vector2dggs/__init__.py
--rw-r--r--   0        0        0      520 2023-04-26 00:14:53.266711 vector2dggs-0.2.0/vector2dggs/cli.py
--rw-r--r--   0        0        0     9325 2023-04-27 01:25:16.919233 vector2dggs-0.2.0/vector2dggs/h3.py
--rw-r--r--   0        0        0     2817 2023-04-26 00:14:53.266711 vector2dggs-0.2.0/vector2dggs/katana.py
--rw-r--r--   0        0        0     9078 1970-01-01 00:00:00.000000 vector2dggs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7920 2023-04-28 03:57:54.021647 vector2dggs-0.2.1/README.md
+-rw-r--r--   0        0        0     1092 2023-04-28 03:58:19.141773 vector2dggs-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-04-28 03:58:04.641700 vector2dggs-0.2.1/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-28 03:53:40.792378 vector2dggs-0.2.1/vector2dggs/cli.py
+-rw-r--r--   0        0        0     9405 2023-04-28 03:53:55.148450 vector2dggs-0.2.1/vector2dggs/h3.py
+-rw-r--r--   0        0        0     2817 2023-04-26 00:14:53.266711 vector2dggs-0.2.1/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.2.1/PKG-INFO
```

### Comparing `vector2dggs-0.2.0/README.md` & `vector2dggs-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 
 Python-based CLI tool to index raster files to DGGS in parallel, writing out to Parquet.
 
 This is the vector equivalent of [raster2dggs](https://github.com/manaakiwhenua/raster2dggs).
 
 Currently only supports H3 DGGS, and probably has other limitations since it has been developed for a specific internal use case, though it is intended as a general-purpose abstraction. Contributions, suggestions, bug reports and strongly worded letters are all welcome.
 
-Currently only supports polygons.
+Currently only supports polygons; but both coverages (strictly non-overlapping polygons), and sets of polygons that do/may overlap, are supported. Overlapping polygons are captured by ensuring that DGGS cell IDs may be non-unique (repeated) in the output.
 
 ![Example use case for vector2dggs, showing parcels indexed to a high H3 resolution](./docs/imgs/vector2dggs-example.png "Example use case for vector2dggs, showing parcels indexed to a high H3 resolution")
 
+## Installation
+
+```bash
+pip install vector2dggs
+```
+
 ## Usage
 
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
@@ -142,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.2.0},
+  version={0.2.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.2.0/pyproject.toml` & `vector2dggs-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.2.0"
+version = "0.2.1"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.2.0/vector2dggs/cli.py` & `vector2dggs-0.2.1/vector2dggs/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import click
 
+from vector2dggs import __version__
 from vector2dggs.h3 import h3
 
 #   If the program does terminal interaction, make it output a short
 # notice like this when it starts in an interactive mode:
 
 #     <program>  Copyright (C) <year>  <name of author>
 #     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
 #     This is free software, and you are welcome to redistribute it
 #     under certain conditions; type `show c' for details.
 
-
 @click.group()
+@click.version_option(version=__version__)
 def cli():
     pass
 
 
 cli.add_command(h3)
```

### Comparing `vector2dggs-0.2.0/vector2dggs/h3.py` & `vector2dggs-0.2.1/vector2dggs/h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import pyproj
 from shapely.geometry import GeometryCollection
 import sqlalchemy
 from tqdm import tqdm
 from tqdm.dask import TqdmCallback
 
 from . import katana
+from vector2dggs import __version__
 
 LOGGER = logging.getLogger(__name__)
 click_log.basic_config(LOGGER)
 MIN_H3, MAX_H3 = 0, 15
 
 warnings.filterwarnings(
     "ignore"
@@ -141,15 +142,15 @@
         with TqdmCallback():
             ddf.to_parquet(tmpdir, overwrite=True)
 
         filepaths = list(map(lambda f: f.absolute(), Path(tmpdir).glob("*")))
 
         # Multithreaded polyfilling
         LOGGER.info(
-            "H3 Indexing on spatial partitions by polyfill with H3 resoltion: %d",
+            "H3 Indexing on spatial partitions by polyfill with H3 resolution: %d",
             resolution,
         )
         with Pool(processes=processes) as pool:
             args = [
                 (filepath, spatial_sort_col, resolution, output_directory)
                 for filepath in filepaths
             ]
@@ -243,14 +244,15 @@
     required=False,
     default="geom",
     type=str,
     help="Column name to use when using a spatial database connection as input",
     nargs=1,
 )
 @click.option("-o", "--overwrite", is_flag=True)
+@click.version_option(version=__version__)
 def h3(
     vector_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
     id_field: str,
     keep_attributes: bool,
     partitions: int,
```

### Comparing `vector2dggs-0.2.0/vector2dggs/katana.py` & `vector2dggs-0.2.1/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.2.0/PKG-INFO` & `vector2dggs-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -39,18 +39,24 @@
 
 Python-based CLI tool to index raster files to DGGS in parallel, writing out to Parquet.
 
 This is the vector equivalent of [raster2dggs](https://github.com/manaakiwhenua/raster2dggs).
 
 Currently only supports H3 DGGS, and probably has other limitations since it has been developed for a specific internal use case, though it is intended as a general-purpose abstraction. Contributions, suggestions, bug reports and strongly worded letters are all welcome.
 
-Currently only supports polygons.
+Currently only supports polygons; but both coverages (strictly non-overlapping polygons), and sets of polygons that do/may overlap, are supported. Overlapping polygons are captured by ensuring that DGGS cell IDs may be non-unique (repeated) in the output.
 
 ![Example use case for vector2dggs, showing parcels indexed to a high H3 resolution](./docs/imgs/vector2dggs-example.png "Example use case for vector2dggs, showing parcels indexed to a high H3 resolution")
 
+## Installation
+
+```bash
+pip install vector2dggs
+```
+
 ## Usage
 
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
@@ -177,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.2.0},
+  version={0.2.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.2.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.2.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

