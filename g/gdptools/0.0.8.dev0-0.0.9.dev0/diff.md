# Comparing `tmp/gdptools-0.0.8.dev0.tar.gz` & `tmp/gdptools-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdptools-0.0.8.dev0.tar", max compression
+gzip compressed data, was "gdptools-0.0.9.dev0.tar", max compression
```

## Comparing `gdptools-0.0.8.dev0.tar` & `gdptools-0.0.9.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1640 2022-07-02 18:16:27.070240 gdptools-0.0.8.dev0/LICENSE.md
--rw-r--r--   0        0        0     2246 2022-07-02 18:16:27.070240 gdptools-0.0.8.dev0/README.md
--rw-r--r--   0        0        0     3135 2022-07-05 16:37:22.222064 gdptools-0.0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-02 18:16:27.109240 gdptools-0.0.8.dev0/src/_pygeoapi_process/__init__.py
--rw-r--r--   0        0        0     5831 2022-07-02 18:16:27.109240 gdptools-0.0.8.dev0/src/_pygeoapi_process/calc_weights_catalog.py
--rw-r--r--   0        0        0      222 2022-07-05 16:37:22.224063 gdptools-0.0.8.dev0/src/gdptools/__init__.py
--rw-r--r--   0        0        0      206 2022-05-04 23:24:42.180911 gdptools-0.0.8.dev0/src/gdptools/__main__.py
--rw-r--r--   0        0        0    22993 2022-07-02 18:16:27.110240 gdptools-0.0.8.dev0/src/gdptools/ancillary.py
--rw-r--r--   0        0        0     3728 2022-07-02 18:16:27.110240 gdptools-0.0.8.dev0/src/gdptools/fill_missing_vals_nearest_neighbor.py
--rw-r--r--   0        0        0     1528 2022-07-02 18:16:27.110240 gdptools-0.0.8.dev0/src/gdptools/genweights.py
--rw-r--r--   0        0        0    28138 2022-07-05 15:56:29.957483 gdptools-0.0.8.dev0/src/gdptools/helpers.py
--rw-r--r--   0        0        0     6825 2022-07-02 18:16:27.112240 gdptools-0.0.8.dev0/src/gdptools/helpers_for_test.py
--rw-r--r--   0        0        0    14755 2022-07-04 21:47:52.121145 gdptools-0.0.8.dev0/src/gdptools/run_weights_engine.py
--rw-r--r--   0        0        0     1255 2022-07-02 18:16:27.113240 gdptools-0.0.8.dev0/src/gdptools/stats.py
--rw-r--r--   0        0        0     3048 2022-07-02 18:16:27.114240 gdptools-0.0.8.dev0/src/gdptools/weighted_intersection.py
--rw-r--r--   0        0        0     3654 2022-07-05 16:37:29.782333 gdptools-0.0.8.dev0/setup.py
--rw-r--r--   0        0        0     3776 2022-07-05 16:37:29.782915 gdptools-0.0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1640 2022-07-02 18:16:27.070240 gdptools-0.0.9.dev0/LICENSE.md
+-rw-r--r--   0        0        0     2246 2022-07-02 18:16:27.070240 gdptools-0.0.9.dev0/README.md
+-rw-r--r--   0        0        0     3135 2022-07-05 17:10:49.767944 gdptools-0.0.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-02 18:16:27.109240 gdptools-0.0.9.dev0/src/_pygeoapi_process/__init__.py
+-rw-r--r--   0        0        0     5831 2022-07-02 18:16:27.109240 gdptools-0.0.9.dev0/src/_pygeoapi_process/calc_weights_catalog.py
+-rw-r--r--   0        0        0      222 2022-07-05 17:10:49.770944 gdptools-0.0.9.dev0/src/gdptools/__init__.py
+-rw-r--r--   0        0        0      206 2022-05-04 23:24:42.180911 gdptools-0.0.9.dev0/src/gdptools/__main__.py
+-rw-r--r--   0        0        0    22993 2022-07-02 18:16:27.110240 gdptools-0.0.9.dev0/src/gdptools/ancillary.py
+-rw-r--r--   0        0        0     3728 2022-07-02 18:16:27.110240 gdptools-0.0.9.dev0/src/gdptools/fill_missing_vals_nearest_neighbor.py
+-rw-r--r--   0        0        0     1528 2022-07-02 18:16:27.110240 gdptools-0.0.9.dev0/src/gdptools/genweights.py
+-rw-r--r--   0        0        0    27969 2022-07-05 17:09:52.371719 gdptools-0.0.9.dev0/src/gdptools/helpers.py
+-rw-r--r--   0        0        0     6825 2022-07-02 18:16:27.112240 gdptools-0.0.9.dev0/src/gdptools/helpers_for_test.py
+-rw-r--r--   0        0        0    14755 2022-07-04 21:47:52.121145 gdptools-0.0.9.dev0/src/gdptools/run_weights_engine.py
+-rw-r--r--   0        0        0     1255 2022-07-02 18:16:27.113240 gdptools-0.0.9.dev0/src/gdptools/stats.py
+-rw-r--r--   0        0        0     3048 2022-07-02 18:16:27.114240 gdptools-0.0.9.dev0/src/gdptools/weighted_intersection.py
+-rw-r--r--   0        0        0     3654 2022-07-05 17:12:25.132332 gdptools-0.0.9.dev0/setup.py
+-rw-r--r--   0        0        0     3776 2022-07-05 17:12:25.132916 gdptools-0.0.9.dev0/PKG-INFO
```

### Comparing `gdptools-0.0.8.dev0/LICENSE.md` & `gdptools-0.0.9.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/README.md` & `gdptools-0.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/pyproject.toml` & `gdptools-0.0.9.dev0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdptools"
-version = "0.0.8-dev0"
+version = "0.0.9-dev0"
 description = "Gdptools"
 authors = ["Richard McDonald <rmcd@usgs.gov>"]
 license = "LICENSE.md"
 readme = "README.md"
 homepage = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools"
 repository = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools"
 documentation = "https://gdptools.readthedocs.io"
```

### Comparing `gdptools-0.0.8.dev0/src/_pygeoapi_process/calc_weights_catalog.py` & `gdptools-0.0.9.dev0/src/_pygeoapi_process/calc_weights_catalog.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/ancillary.py` & `gdptools-0.0.9.dev0/src/gdptools/ancillary.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/fill_missing_vals_nearest_neighbor.py` & `gdptools-0.0.9.dev0/src/gdptools/fill_missing_vals_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/genweights.py` & `gdptools-0.0.9.dev0/src/gdptools/genweights.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/helpers.py` & `gdptools-0.0.9.dev0/src/gdptools/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,20 +350,18 @@
         geom_id (str): _description_
 
     Returns:
         Tuple[gpd.GeoDataFrame, npt.NDArray[Any]]: _description_
     """
     wghts = _get_wieght_df(wght_file, geom_id)
 
-    gdf = shp
-    # gdf.reset_index(drop=True, inplace=True)
-    # gdf1 = gdf.sort_values(geom_id).dissolve(by=geom_id)
-    gdf1 = gdf.dissolve(by=geom_id)
+    shp.reset_index(drop=True, inplace=True)
+    gdf = shp.sort_values(geom_id).dissolve(by=geom_id)
 
-    geo_index = np.asarray(gdf1.index, dtype=str)
+    geo_index = np.asarray(gdf.index, dtype=type(gdf.index.values[0]))
     n_geo = len(geo_index)
 
     print_on = _get_print_on(n_geo)
     unique_geom_ids = wghts.groupby(geom_id)
     ds_vars = [i for i in ds.data_vars]
     # if var not in ds_vars:
     #     raise KeyError(f"var: {var} not in ds vars: {ds_vars}")
@@ -380,15 +378,15 @@
 
     # for t in np.arange(nts):
     #     # val_flat_interp = (
     #     #     ds[var].values[t, 1 : grd_shp[1] - 1, 1 : grd_shp[2] - 1].flatten()
     #     # )
     print(f"processing time for var: {var}")
     for i in np.arange(len(geo_index)):
-        weight_id_rows = unique_geom_ids.get_group(geo_index[i])
+        weight_id_rows = unique_geom_ids.get_group(str(geo_index[i]))
         tw = weight_id_rows.wght.values
         i_ind = np.array(weight_id_rows.i.values)
         j_ind = np.array(weight_id_rows.j.values)
 
         vals = var_vals[:, i_ind, j_ind]
 
         # tgid = weight_id_rows.grid_ids.values
@@ -402,15 +400,15 @@
         except KeyError:
             val_interp[i, :] = netCDF4.default_fillvals["f8"]
 
         if i % print_on == 0:
             print(f"    Processing {var} for feature {geo_index[i]}", flush=True)
 
     # print(val_interp)
-    return gdf1, val_interp
+    return gdf, val_interp
 
 
 def build_subset(
     bounds: npt.NDArray[np.double],
     xname: str,
     yname: str,
     tname: str,
@@ -756,26 +754,24 @@
         Union[gpd.GeoDataFrame, np.ndarray]: _description_
     """
     params_json = _get_dataframe(params_json)
     grid_json = _get_dataframe(grid_json)
 
     # read shapefile, calculate total_bounds, and project to grid's projection
     shp, gdf_bounds = _get_shp_file(shp_file=shp_file, grid_json=grid_json)
+    poly_idx = shp_poly_idx
+        if poly_idx not in shp.columns[:]:
+            raise ValueError(
+                (f"shp_poly_idx: {poly_idx}" " not in gdf columns: {shp.columns}")
+            )
 
     # run check on intersection of shape features and gridded data
     is_intersect, is_degrees, is_0_360 = _check_for_intersection(
         params_json=params_json, grid_json=grid_json, gdf=shp_file
     )
-    # read shapefile, calculate total_bounds, and project to grid's projection
-    shp, gdf_bounds = _get_shp_file(shp_file=shp_file, grid_json=grid_json)
-    poly_idx = shp_poly_idx
-    if poly_idx not in shp.columns[:]:
-        raise ValueError(
-            (f"shp_poly_idx: {poly_idx}" " not in gdf columns: {shp.columns}")
-        )
 
     wghts = _get_wieght_df(wght_file, poly_idx)
 
     # get sub-setted xarray dataset
     if (not is_intersect) & is_degrees & (not is_0_360):
         rotate_ds = True
     else:
```

### Comparing `gdptools-0.0.8.dev0/src/gdptools/helpers_for_test.py` & `gdptools-0.0.9.dev0/src/gdptools/helpers_for_test.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/run_weights_engine.py` & `gdptools-0.0.9.dev0/src/gdptools/run_weights_engine.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/stats.py` & `gdptools-0.0.9.dev0/src/gdptools/stats.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/src/gdptools/weighted_intersection.py` & `gdptools-0.0.9.dev0/src/gdptools/weighted_intersection.py`

 * *Files identical despite different names*

### Comparing `gdptools-0.0.8.dev0/setup.py` & `gdptools-0.0.9.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'zarr>=2.11.3,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['gdptools = gdptools.__main__:main']}
 
 setup_kwargs = {
     'name': 'gdptools',
-    'version': '0.0.8.dev0',
+    'version': '0.0.9.dev0',
     'description': 'Gdptools',
     'long_description': "---\n\ntitle: README\n---Gdptools\n========\n\n[![PyPI](https://img.shields.io/pypi/v/gdptools.svg)](https://pypi.org/project/gdptools/)\n[![Status](https://img.shields.io/pypi/status/gdptools.svg)](https://pypi.org/project/gdptools/)\n[![Python Version](https://img.shields.io/pypi/pyversions/gdptools)](https://pypi.org/project/gdptools)\n[![License](https://img.shields.io/pypi/l/gdptools)](https://creativecommons.org/publicdomain/zero/1.0/legalcode)\n\n[![Read the documentation at https://gdptools.readthedocs.io/](https://img.shields.io/readthedocs/gdptools/latest.svg?label=Read%20the%20Docs)](https://gdptools.readthedocs.io/)\n[![Tests](https://code.usgs.gov/wma/nhgf/toolsteam/gdptools/workflows/Tests/badge.svg)](https://code.usgs.gov/wma/nhgf/toolsteam/gdptools/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/wma/nhgf/toolsteam/gdptools/branch/main/graph/badge.svg)](https://codecov.io/gh/wma/nhgf/toolsteam/gdptools)\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://code.usgs.gov/pre-commit/pre-commit)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://code.usgs.gov/psf/black)\n[![Poetry](https://img.shields.io/badge/poetry-enabled-blue)](https://python-poetry.org/)\n[![Conda](https://img.shields.io/badge/conda-enabled-green)](https://anaconda.org/)\n\n# Features\n\n- TODO\n\n# Requirements\n\n- TODO\n\n# Installation\n\nYou can install _Gdptools_ via [pip](https://pip.pypa.io/) from [PyPI](https://pypi.org/):\n\n        pip install gdptools\n\n# Usage\n\nPlease see the [Command-line Reference](Usage_) for details.\n\n# Contributing\n\nContributions are very welcome. To learn more, see the Contributor Guide\\_.\n\n# License\n\nDistributed under the terms of the [CC0 1.0 Universal license](https://creativecommons.org/publicdomain/zero/1.0/legalcode), _Gdptools_ is free and open source software.\n\n# Issues\n\nIf you encounter any problems, please [file an issue](https://code.usgs.gov/wma/nhgf/toolsteam/gdptools/issues) along with a detailed description.\n\n# Credits\n\nThis project was generated from [@hillc-usgs](https://code.usgs.gov/hillc-usgs)'s [Pygeoapi Plugin Cookiecutter](https://code.usgs.gov/wma/nhgf/pygeoapi-plugin-cookiecutter) template.\n",
     'author': 'Richard McDonald',
     'author_email': 'rmcd@usgs.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://code.usgs.gov/wma/nhgf/toolsteam/gdptools',
```

### Comparing `gdptools-0.0.8.dev0/PKG-INFO` & `gdptools-0.0.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdptools
-Version: 0.0.8.dev0
+Version: 0.0.9.dev0
 Summary: Gdptools
 Home-page: https://code.usgs.gov/wma/nhgf/toolsteam/gdptools
 License: LICENSE.md
 Author: Richard McDonald
 Author-email: rmcd@usgs.gov
 Requires-Python: >=3.9,<3.10
 Classifier: Development Status :: 1 - Planning
```

