# Comparing `tmp/stagemodel-0.0.4.tar.gz` & `tmp/stagemodel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stagemodel-0.0.4.tar", last modified: Tue Jun 22 17:40:16 2021, max compression
+gzip compressed data, was "stagemodel-0.0.5.tar", last modified: Thu Apr 27 23:36:29 2023, max compression
```

## Comparing `stagemodel-0.0.4.tar` & `stagemodel-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 17:40:16.060032 stagemodel-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2021-06-22 17:39:56.000000 stagemodel-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      602 2021-06-22 17:40:16.060032 stagemodel-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-06-22 17:39:56.000000 stagemodel-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-22 17:40:16.060032 stagemodel-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-06-22 17:39:56.000000 stagemodel-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 17:40:16.060032 stagemodel-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 17:40:16.060032 stagemodel-0.0.4/src/stagemodel/
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-06-22 17:39:56.000000 stagemodel-0.0.4/src/stagemodel/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-06-22 17:39:56.000000 stagemodel-0.0.4/src/stagemodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2021-06-22 17:39:56.000000 stagemodel-0.0.4/src/stagemodel/composite_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    14094 2021-06-22 17:39:56.000000 stagemodel-0.0.4/src/stagemodel/node_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2021-06-22 17:39:56.000000 stagemodel-0.0.4/src/stagemodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 17:40:16.060032 stagemodel-0.0.4/src/stagemodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2021-06-22 17:40:16.000000 stagemodel-0.0.4/src/stagemodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-06-22 17:40:16.000000 stagemodel-0.0.4/src/stagemodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-22 17:40:16.000000 stagemodel-0.0.4/src/stagemodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-22 17:40:15.000000 stagemodel-0.0.4/src/stagemodel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-06-22 17:40:16.000000 stagemodel-0.0.4/src/stagemodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-06-22 17:40:16.000000 stagemodel-0.0.4/src/stagemodel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:36:29.251958 stagemodel-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-27 23:35:34.000000 stagemodel-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-27 23:36:29.251958 stagemodel-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-27 23:35:34.000000 stagemodel-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 23:35:34.000000 stagemodel-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:36:29.251958 stagemodel-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:36:29.247958 stagemodel-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:36:29.251958 stagemodel-0.0.5/src/stagemodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 23:35:34.000000 stagemodel-0.0.5/src/stagemodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-27 23:35:34.000000 stagemodel-0.0.5/src/stagemodel/composite_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-04-27 23:35:34.000000 stagemodel-0.0.5/src/stagemodel/node_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-27 23:35:34.000000 stagemodel-0.0.5/src/stagemodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:36:29.251958 stagemodel-0.0.5/src/stagemodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-27 23:36:29.000000 stagemodel-0.0.5/src/stagemodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 23:36:29.000000 stagemodel-0.0.5/src/stagemodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:36:29.000000 stagemodel-0.0.5/src/stagemodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 23:36:29.000000 stagemodel-0.0.5/src/stagemodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 23:36:29.000000 stagemodel-0.0.5/src/stagemodel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:36:29.251958 stagemodel-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 23:35:34.000000 stagemodel-0.0.5/tests/test_dummy.py
```

### Comparing `stagemodel-0.0.4/LICENSE` & `stagemodel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stagemodel-0.0.4/src/stagemodel/composite_model.py` & `stagemodel-0.0.5/src/stagemodel/composite_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
     composite_model
     ~~~~~~~~~~~~~~~
 """
+from copy import deepcopy
 from pathlib import Path
-from typing import List, Dict, Tuple, Any, Union
+from typing import Any, Dict, List, Tuple, Union
+
 import numpy as np
 import xarray as xr
-from copy import deepcopy
+from mrtool import LinearCovModel, MRData
 
-from mrtool import MRData, LinearCovModel
 from .node_model import NodeModel, OverallModel, StudyModel
 from .utils import result_to_df
 
 
 class StagewiseModel:
-
-    def __init__(self,
-                 data: MRData,
-                 node_models: List[NodeModel]):
+    def __init__(self, data: MRData, node_models: List[NodeModel]):
         self.node_models = node_models
         self.num_models = len(node_models)
         self.data_list = [data]
 
     def _get_next_data(self, model: NodeModel):
         pred = model.predict(self.data_list[-1])
         resi = self.data_list[-1].obs - pred
@@ -41,36 +39,42 @@
         self,
         data: Union[MRData, List[xr.DataArray]] = None,
         slope_quantile: Dict[str, float] = None,
         ref_cov: Tuple[str, Any] = None,
     ) -> Union[np.ndarray, xr.DataArray]:
         if data is None:
             data = self.data_list[0]
-        pred = self.node_models[0].predict(data, slope_quantile=slope_quantile, ref_cov=ref_cov)
+        pred = self.node_models[0].predict(
+            data, slope_quantile=slope_quantile, ref_cov=ref_cov
+        )
         if len(self.node_models) > 1:
             for model in self.node_models[1:]:
-                pred += model.predict(data, slope_quantile=slope_quantile, ref_cov=ref_cov)
+                pred += model.predict(
+                    data, slope_quantile=slope_quantile, ref_cov=ref_cov
+                )
         return pred
 
     def soln_to_df(self, i: int, path: str = None):
         return self.node_models[i].soln_to_df(path)
 
-    def result_to_df(self, i: int = None, path: str = None,
-                     prediction: str = 'prediction',
-                     residual: str = 'residual'):
+    def result_to_df(
+        self,
+        i: int = None,
+        path: str = None,
+        prediction: str = "prediction",
+        residual: str = "residual",
+    ):
         if i is not None:
             df = self.node_models[i].result_to_df(path, prediction, residual)
         else:
-            df = result_to_df(self, self.data_list[0],
-                              path, prediction, residual)
+            df = result_to_df(self, self.data_list[0], path, prediction, residual)
         return df
 
 
 class TwoStageModel:
-
     def __init__(
         self,
         data: MRData,
         cov_models_stage1: List[LinearCovModel],
         cov_models_stage2: List[LinearCovModel],
     ):
         self.cov_models1 = cov_models_stage1
@@ -105,19 +109,21 @@
         slope_quantile: Dict[str, float] = None,
         ref_cov: Tuple[str, Any] = None,
     ):
         if data is None:
             data = self.data1
         data._sort_by_data_id()
         pred1 = self.model1.predict(data)
-        return self.model2.predict(data, slope_quantile=slope_quantile, ref_cov=ref_cov) + pred1
+        return (
+            self.model2.predict(data, slope_quantile=slope_quantile, ref_cov=ref_cov)
+            + pred1
+        )
 
 
 class ReverseTwoStageModel:
-
     def __init__(
         self,
         data: MRData,
         cov_models_stage1: List[LinearCovModel],
         cov_models_stage2: List[LinearCovModel],
     ):
         self.cov_models1 = cov_models_stage1
@@ -151,9 +157,11 @@
         data: MRData = None,
         slope_quantile: Dict[str, float] = None,
         ref_cov: Tuple[str, Any] = None,
     ):
         if data is None:
             data = self.data1
         data._sort_by_data_id()
-        pred1 = self.model1.predict(data, slope_quantile=slope_quantile, ref_cov=ref_cov)
+        pred1 = self.model1.predict(
+            data, slope_quantile=slope_quantile, ref_cov=ref_cov
+        )
         return self.model2.predict(data) + pred1
```

### Comparing `stagemodel-0.0.4/src/stagemodel/node_model.py` & `stagemodel-0.0.5/src/stagemodel/node_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 """
     model
     ~~~~~
 """
-from typing import List, Union, Dict, Tuple, Any
+from typing import Any, Dict, List, Tuple, Union
+from warnings import warn
+
 import numpy as np
 import pandas as pd
 import xarray as xr
-from warnings import warn
-
-from mrtool import MRData, LinearCovModel, MRBRT
+from mrtool import MRBRT, LinearCovModel, MRData
 
-from .utils import solve_ls, solve_ls_b, result_to_df
+from .utils import result_to_df, solve_ls, solve_ls_b
 
 
 class NodeModel:
-    """Node model that carries independent task.
-    """
+    """Node model that carries independent task."""
 
-    def __init__(self,
-                 data: MRData = None,
-                 cov_models: List[LinearCovModel] = None):
+    def __init__(self, data: MRData = None, cov_models: List[LinearCovModel] = None):
         """Constructor of the NodeModel.
 
         Args:
             data (MRData):
                 Data object from MRTool. If ``None``, no data is attached.
                 Default to ``None``.
             cov_models (List[LinearCovModel]):
                 List of linear covariate model from MRTool. If ``None``,
                 intercept model will be added. Default to ``None``.
         """
         self.data = None
-        self.cov_models = [LinearCovModel('intercept')] if cov_models is None else cov_models
+        self.cov_models = (
+            [LinearCovModel("intercept")] if cov_models is None else cov_models
+        )
         self.cov_names = self.get_cov_names()
         self.mat = None
         self.soln = None
 
         self.attach_data(data)
 
     def attach_data(self, data: Union[MRData, None]):
@@ -65,16 +64,15 @@
 
         Raises:
             ValueError: If attribute ``soln`` is ``None``, return value error.
         """
         if self.soln is None:
             raise ValueError("Must fit model!")
 
-    def get_cov_names(self,
-                      cov_models: List[LinearCovModel] = None) -> List[str]:
+    def get_cov_names(self, cov_models: List[LinearCovModel] = None) -> List[str]:
         """Get covariates names.
 
         Args:
             cov_models (List[LinearCovModel], optional):
                 List of covariate models. If ``None`` ues the attribute
                 ``cov_models``. Defaults to None.
 
@@ -96,47 +94,50 @@
                 the attribute ``self.data``. Defaults to None.
 
         Returns:
             np.ndarray: Design matrix.
         """
         data = self.data if data is None else data
         assert isinstance(data, MRData)
-        return np.hstack([cov_model.create_design_mat(data)[0]
-                          for cov_model in self.cov_models])
+        return np.hstack(
+            [cov_model.create_design_mat(data)[0] for cov_model in self.cov_models]
+        )
 
     def create_design_mat_from_xarray(self, covs: List[xr.DataArray]) -> np.ndarray:
         var_coord = "variable"
         for cov in covs:
             if "year_id" in cov.coords:
                 year_id = cov.year_id
                 year_id.name = "year_id_"
                 covs.append(year_id)
                 break
         da = xr.merge(covs).to_array()
-        data = MRData(covs={
-            cov.strip("_"): da.values[i].ravel()
-            for i, cov in enumerate(da.coords[var_coord].values)
-        })
+        data = MRData(
+            covs={
+                cov.strip("_"): da.values[i].ravel()
+                for i, cov in enumerate(da.coords[var_coord].values)
+            }
+        )
         del da.coords[var_coord]
         return self.create_design_mat(data), da[0].coords, da[0].dims, da[0].shape
 
     @staticmethod
-    def get_study_ids_from_xarray(covs: List[xr.DataArray],
-                                  coord_name: str = "location_id") -> np.ndarray:
+    def get_study_ids_from_xarray(
+        covs: List[xr.DataArray], coord_name: str = "location_id"
+    ) -> np.ndarray:
         cov = covs[np.argmax([cov.size for cov in covs])]
         return cov.coords.to_index().to_frame(index=False)[coord_name].to_numpy()
 
     def fit_model(self):
-        """Fit the model.
-        """
+        """Fit the model."""
         raise NotImplementedError()
 
-    def predict(self,
-                data: Union[MRData, List[xr.DataArray]] = None,
-                **kwargs) -> Union[np.ndarray, xr.DataArray]:
+    def predict(
+        self, data: Union[MRData, List[xr.DataArray]] = None, **kwargs
+    ) -> Union[np.ndarray, xr.DataArray]:
         """Predict from fitting result.
 
         Args:
             data (Union[MRData, List[xr.DataArray]], optional):
                 Given data object to predict, if ``None`` use the attribute
                 ``self.data`` Defaults to None.
             kwargs (Dict): Other keyword arguments.
@@ -156,18 +157,20 @@
                 frame. Defaults to None.
 
         Returns:
             pd.DataFrame: Data frame that contains the result.
         """
         raise NotImplementedError()
 
-    def result_to_df(self,
-                     path: str = None,
-                     prediction: str = 'prediction',
-                     residual: str = 'residual') -> pd.DataFrame:
+    def result_to_df(
+        self,
+        path: str = None,
+        prediction: str = "prediction",
+        residual: str = "residual",
+    ) -> pd.DataFrame:
         """Create result data frame.
 
         Args:
             path (Union[str, None], optional):
                 Address that save the result, include the file name.
                 If ``None`` do not save the result, only return the result data
                 frame. Defaults to None.
@@ -177,104 +180,101 @@
                 Column name of the residual. Defaults to 'residual'.
 
         Returns:
             pd.DataFrame: Result data frame.
         """
         self._assert_has_data()
         self._assert_has_soln()
-        return result_to_df(self, self.data,
-                            path=path, prediction=prediction, residual=residual)
+        return result_to_df(
+            self, self.data, path=path, prediction=prediction, residual=residual
+        )
 
 
 class OverallModel(NodeModel):
     """Overall model in charge of fit all location together without
     random effects.
     """
 
     def fit_model(self, **fit_options):
-        """Fit the model
-        """
+        """Fit the model"""
         self._assert_has_data()
         beta_init = solve_ls(self.mat, self.data.obs, self.data.obs_se)
         model = MRBRT(self.data, self.cov_models)
         gamma_init = np.zeros(model.num_z_vars)
 
         default_fit_options = dict(
             x0=np.hstack((beta_init, gamma_init)),
-            inner_max_iter=500,
-            inner_print_level=5,
         )
         fit_options = {**default_fit_options, **fit_options}
         model.fit_model(**fit_options)
         self.soln = model.beta_soln
 
-    def predict(self,
-                data: Union[MRData, List[xr.DataArray]] = None,
-                **kwargs) -> Union[np.ndarray, xr.DataArray]:
-        """Predict from fitting result.
-        """
+    def predict(
+        self, data: Union[MRData, List[xr.DataArray]] = None, **kwargs
+    ) -> Union[np.ndarray, xr.DataArray]:
+        """Predict from fitting result."""
         self._assert_has_soln()
         data = self.data if data is None else data
         if isinstance(data, MRData):
             data._sort_by_data_id()
             mat = self.create_design_mat(data)
             pred = mat.dot(self.soln)
         else:
             mat, coords, dims, shape = self.create_design_mat_from_xarray(data)
-            pred = xr.DataArray(mat.dot(self.soln).reshape(shape),
-                                coords=coords,
-                                dims=dims)
+            pred = xr.DataArray(
+                mat.dot(self.soln).reshape(shape), coords=coords, dims=dims
+            )
 
         return pred
 
     def soln_to_df(self, path: str = None) -> pd.DataFrame:
-        """Write solution.
-        """
+        """Write solution."""
         names = []
         for cov_model in self.cov_models:
-            names.extend([cov_model.name + '_' + str(i)
-                          for i in range(cov_model.num_x_vars)])
+            names.extend(
+                [cov_model.name + "_" + str(i) for i in range(cov_model.num_x_vars)]
+            )
         assert len(names) == len(self.soln)
-        df = pd.DataFrame(list(zip(names, self.soln)),
-                          columns=['name', 'value'])
+        df = pd.DataFrame(list(zip(names, self.soln)), columns=["name", "value"])
         if path is not None:
             df.to_csv(path)
         return df
 
 
 class StudyModel(NodeModel):
-    """Study specific Model.
-    """
+    """Study specific Model."""
 
     def fit_model(self):
-        """Fit the model.
-        """
+        """Fit the model."""
         self._assert_has_data()
         self.soln = {}
-        bounds = np.vstack([cov_model.prior_beta_uniform.T
-                            for cov_model in self.cov_models])
-        use_bounds = (not np.isneginf(bounds[:, 0]).all()) or \
-            (not np.isposinf(bounds[:, 1]).all())
-        gprior = np.hstack([cov_model.prior_beta_gaussian
-                            for cov_model in self.cov_models])
+        bounds = np.vstack(
+            [cov_model.prior_beta_uniform.T for cov_model in self.cov_models]
+        )
+        use_bounds = (not np.isneginf(bounds[:, 0]).all()) or (
+            not np.isposinf(bounds[:, 1]).all()
+        )
+        gprior = np.hstack(
+            [cov_model.prior_beta_gaussian for cov_model in self.cov_models]
+        )
         if np.isinf(gprior[1]).all():
             gprior = None
         for study_id in self.data.studies:
             index = self.data.study_id == study_id
             mat = self.mat[index, :]
             obs = self.data.obs[index]
             obs_se = self.data.obs_se[index]
             if use_bounds:
-                self.soln[study_id] = solve_ls_b(mat, obs, obs_se, bounds,
-                                                 gprior=gprior)
+                self.soln[study_id] = solve_ls_b(
+                    mat, obs, obs_se, bounds, gprior=gprior
+                )
             else:
-                self.soln[study_id] = solve_ls(mat, obs, obs_se,
-                                               gprior=gprior)
+                self.soln[study_id] = solve_ls(mat, obs, obs_se, gprior=gprior)
 
-        self.soln['mean'] = np.array(list(self.soln.values())).mean(axis=0)
+        self.soln["mean"] = np.array(list(self.soln.values())).mean(axis=0)
 
     def predict(
         self,
         data: Union[MRData, List[xr.DataArray]] = None,
         slope_quantile: Dict[str, float] = None,
         ref_cov: Tuple[str, Any] = None,
         **kwargs,
@@ -285,100 +285,105 @@
             slope_quantile (Dict[str, float]):
                 Dictionary with key as the covariate name and value the
                 quantile. If ``None`` will predict for specific group, else
                 use the quantile or more extreme slope. Default to ``None``.
         """
         self._assert_has_soln()
         data = self.data if data is None else data
+        df = self.data.to_df()
         if isinstance(data, MRData):
             data._sort_by_data_id()
             mat = self.create_design_mat(data)
             study_ids = data.study_id
             if ref_cov is not None:
                 ref_cov_values = data.covs[ref_cov[0]]
         else:
             mat, coords, dims, shape = self.create_design_mat_from_xarray(data)
             study_ids = self.get_study_ids_from_xarray(data)
             if ref_cov is not None:
-                ref_cov_values = self.get_study_ids_from_xarray(data, coord_name=ref_cov[0])
+                ref_cov_values = self.get_study_ids_from_xarray(
+                    data, coord_name=ref_cov[0]
+                )
 
         if slope_quantile is not None:
             _, soln = self.get_soln_quantile(slope_quantile, mask_soln=True)
         else:
             soln = self.soln
 
-        coefs = np.vstack([
-            soln[study_id]
-            if study_id in self.data.studies else soln['mean']
-            for study_id in study_ids
-        ])
+        coefs = np.vstack(
+            [
+                soln[study_id] if study_id in self.data.studies else soln["mean"]
+                for study_id in study_ids
+            ]
+        )
         intercept_shift = {study_id: 0.0 for study_id in study_ids}
         if ref_cov is not None:
             for study_id in np.unique(study_ids):
-                sub_mat = mat[(study_ids == study_id) &
-                              (ref_cov_values == ref_cov[1])]
+                sub_mat = mat[(study_ids == study_id) & (ref_cov_values == ref_cov[1])]
+                ref_value = df.loc[
+                    (df.study_id == study_id) & (df[ref_cov[0]] == ref_cov[1]), "obs"
+                ].values[0]
                 if sub_mat.shape[0] != 1:
-                    warn(f'Multiple ref value for study {study_id} found. Using mean instead.')
-                study_name = study_id if study_id in study_ids else 'mean'
-                intercept_shift[study_id] = np.mean(sub_mat.dot(self.soln[study_name] - soln[study_name]))
-
+                    warn(
+                        f"Multiple ref value for study {study_id} found. Using mean instead."
+                    )
+                study_name = study_id if study_id in study_ids else "mean"
+                intercept_shift[study_id] = np.mean(
+                    ref_value - sub_mat.dot(soln[study_name])
+                )
         shifts = np.array([intercept_shift[study_id] for study_id in study_ids])
-        pred = np.sum(mat*coefs, axis=1) + shifts
+        pred = np.sum(mat * coefs, axis=1) + shifts
         if not isinstance(data, MRData):
             pred = xr.DataArray(pred.reshape(shape), coords=coords, dims=dims)
 
         return pred
 
-    def get_soln_quantile(self,
-                          slope_quantile: Dict[str, float],
-                          mask_soln: bool = False) -> Union[Dict[str, float],
-                                                            Tuple[Dict[str, float], Dict[Any, np.ndarray]]]:
+    def get_soln_quantile(
+        self, slope_quantile: Dict[str, float], mask_soln: bool = False
+    ) -> Union[Dict[str, float], Tuple[Dict[str, float], Dict[Any, np.ndarray]]]:
         """Get solution quantile
 
         Args:
             slope_quantile (Dict[str, float]): Solution quantile.
             mask_soln (bool, optional):
                 If ``True``, return masked solution. Default to ``False``.
 
         Returns:
             Union[Dict[str, float], Tuple[Dict[str, float], Dict[Any, np.ndarray]]]:
                 Quantile of the solution or with the masked solution.
         """
-        coefs = np.array([self.soln[study_id]
-                          for study_id in self.data.studies])
+        coefs = np.array([self.soln[study_id] for study_id in self.data.studies])
         quantile_value = {}
         for cov_name, q in slope_quantile.items():
             if cov_name not in self.cov_names:
-                warn(f"{cov_name} not in the model, "
-                     f"ignore it in slope_quantile.")
+                warn(f"{cov_name} not in the model, " f"ignore it in slope_quantile.")
             else:
                 quantile_value[cov_name] = np.quantile(
                     coefs[:, self.cov_names.index(cov_name)], q
                 )
         if mask_soln:
-            masked_coefs = np.vstack([coefs, self.soln['mean']])
+            masked_coefs = np.vstack([coefs, self.soln["mean"]])
             for cov_name, v in quantile_value.items():
                 index = self.cov_names.index(cov_name)
                 if slope_quantile[cov_name] >= 0.5:
                     masked_coefs[:, index] = np.maximum(masked_coefs[:, index], v)
                 else:
                     masked_coefs[:, index] = np.minimum(masked_coefs[:, index], v)
             masked_soln = {
                 study_id: masked_coefs[i]
                 for i, study_id in enumerate(self.data.studies)
             }
-            masked_soln['mean'] = masked_coefs[-1]
+            masked_soln["mean"] = masked_coefs[-1]
             return quantile_value, masked_soln
         else:
             return quantile_value
 
     def soln_to_df(self, path: str = None) -> pd.DataFrame:
-        """Write solution.
-        """
-        df = pd.DataFrame.from_dict(
-            self.soln,
-            orient='index',
-            columns=self.cov_names
-        ).reset_index().rename(columns={'index': 'study_id'})
+        """Write solution."""
+        df = (
+            pd.DataFrame.from_dict(self.soln, orient="index", columns=self.cov_names)
+            .reset_index()
+            .rename(columns={"index": "study_id"})
+        )
         if path is not None:
             df.to_csv(path)
         return df
```

### Comparing `stagemodel-0.0.4/src/stagemodel/utils.py` & `stagemodel-0.0.5/src/stagemodel/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """
     utils
     ~~~~~
 """
 from typing import Dict, Union
+
 import numpy as np
 import pandas as pd
-from scipy.optimize import minimize, OptimizeResult
+from scipy.optimize import OptimizeResult, minimize
 
 
-def solve_ls(mat: np.ndarray,
-             obs: np.ndarray,
-             obs_se: np.ndarray,
-             gprior: np.ndarray = None) -> np.ndarray:
+def solve_ls(
+    mat: np.ndarray, obs: np.ndarray, obs_se: np.ndarray, gprior: np.ndarray = None
+) -> np.ndarray:
     """Solve least square problem
 
     Args:
         mat(np.ndarray): Data matrix
         obs(np.ndarray): Observations
         obs_se(np.ndarray): Observation standard error.
         gprior(np.ndarray): Gaussian prior. Default to ``None``.
 
     Returns:
         np.ndarray: Solution.
     """
     v = obs_se**2
-    eq_mat = (mat.T/v).dot(mat)
-    eq_vec = (mat.T/v).dot(obs)
+    eq_mat = (mat.T / v).dot(mat)
+    eq_vec = (mat.T / v).dot(obs)
     if gprior is not None:
-        eq_mat += np.diag(1.0/gprior[1]**2)
-        eq_vec += gprior[0]/gprior[1]**2
+        eq_mat += np.diag(1.0 / gprior[1] ** 2)
+        eq_vec += gprior[0] / gprior[1] ** 2
     return np.linalg.solve(eq_mat, eq_vec)
 
 
-def solve_ls_b(mat: np.ndarray,
-               obs: np.ndarray, obs_se: np.ndarray,
-               bounds: np.ndarray,
-               gprior: np.ndarray = None,
-               options: Dict = None,
-               return_info: bool = False) -> Union[np.ndarray, OptimizeResult]:
+def solve_ls_b(
+    mat: np.ndarray,
+    obs: np.ndarray,
+    obs_se: np.ndarray,
+    bounds: np.ndarray,
+    gprior: np.ndarray = None,
+    options: Dict = None,
+    return_info: bool = False,
+) -> Union[np.ndarray, OptimizeResult]:
     """Solve least square with bounds problem
 
     Args:
         mat(np.ndarray): Data matrix
         obs(np.ndarray): Observations
         obs_se(np.ndarray): Observation standard error.
         bounds(np.ndarray): Bounds for the variable.
@@ -54,46 +57,56 @@
     Returns:
         np.ndarray: Solution.
     """
     x_init = solve_ls(mat, obs, obs_se)
     v = obs_se**2
 
     if gprior is None:
+
         def objective(x):
             r = obs - mat.dot(x)
-            return 0.5*np.sum(r**2/v)
+            return 0.5 * np.sum(r**2 / v)
 
         def gradient(x):
             r = obs - mat.dot(x)
-            return (mat.T/v).dot(r)
+            return (mat.T / v).dot(r)
+
     else:
+
         def objective(x):
             r = obs - mat.dot(x)
-            return 0.5*np.sum(r**2/v) + 0.5*np.sum((x - gprior[0])**2/gprior[1]**2)
+            return 0.5 * np.sum(r**2 / v) + 0.5 * np.sum(
+                (x - gprior[0]) ** 2 / gprior[1] ** 2
+            )
 
         def gradient(x):
             r = obs - mat.dot(x)
-            return -(mat.T/v).dot(r) + (x - gprior[0])/gprior[1]**2
+            return -(mat.T / v).dot(r) + (x - gprior[0]) / gprior[1] ** 2
 
-    opt_result = minimize(objective,
-                          x0=x_init,
-                          jac=gradient,
-                          method='L-BFGS-B',
-                          bounds=bounds,
-                          options=options)
+    opt_result = minimize(
+        objective,
+        x0=x_init,
+        jac=gradient,
+        method="L-BFGS-B",
+        bounds=bounds,
+        options=options,
+    )
 
     result = opt_result if return_info else opt_result.x
 
     return result
 
 
-def result_to_df(model, data,
-                 path: str = None,
-                 prediction: str = 'prediction',
-                 residual: str = 'residual') -> pd.DataFrame:
+def result_to_df(
+    model,
+    data,
+    path: str = None,
+    prediction: str = "prediction",
+    residual: str = "residual",
+) -> pd.DataFrame:
     """Create result data frame.
 
     Args:
         model (Union[NodeModel, StagewiseModel]): Model instance.
         data (MRData): Data object try to predict.s
         prediction (str, optional):
             Column name of the prediction. Defaults to 'prediction'.
```

