# Comparing `tmp/ionics_fits-1.0.4.tar.gz` & `tmp/ionics_fits-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionics_fits-1.0.4.tar", max compression
+gzip compressed data, was "ionics_fits-1.0.5.tar", max compression
```

## Comparing `ionics_fits-1.0.4.tar` & `ionics_fits-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/LICENSE
--rw-r--r--   0        0        0     9752 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/README.md
--rw-r--r--   0        0        0      124 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/__init__.py
--rw-r--r--   0        0        0    31655 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/common.py
--rw-r--r--   0        0        0      434 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/__init__.py
--rw-r--r--   0        0        0     4794 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/aggregate_model.py
--rw-r--r--   0        0        0     4705 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/benchmarking.py
--rw-r--r--   0        0        0     4015 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/exponential.py
--rw-r--r--   0        0        0     5507 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/gaussian.py
--rw-r--r--   0        0        0     3235 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/lorentzian.py
--rw-r--r--   0        0        0    12420 2023-04-25 15:19:04.850460 ionics_fits-1.0.4/ionics_fits/models/polynomial.py
--rw-r--r--   0        0        0    16336 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/rabi.py
--rw-r--r--   0        0        0     4332 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/rectangle.py
--rw-r--r--   0        0        0     6081 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/sinc.py
--rw-r--r--   0        0        0     6849 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/sinusoid.py
--rw-r--r--   0        0        0     7341 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/triangle.py
--rw-r--r--   0        0        0    11659 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/models/utils.py
--rw-r--r--   0        0        0     4855 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/normal.py
--rw-r--r--   0        0        0      655 2023-04-25 15:19:04.854460 ionics_fits-1.0.4/ionics_fits/utils.py
--rw-r--r--   0        0        0     1032 2023-04-25 15:19:19.130362 ionics_fits-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10840 1970-01-01 00:00:00.000000 ionics_fits-1.0.4/setup.py
--rw-r--r--   0        0        0    10434 1970-01-01 00:00:00.000000 ionics_fits-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/LICENSE
+-rw-r--r--   0        0        0    10406 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/README.md
+-rw-r--r--   0        0        0      124 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/__init__.py
+-rw-r--r--   0        0        0    31893 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/common.py
+-rw-r--r--   0        0        0      444 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/__init__.py
+-rw-r--r--   0        0        0     4705 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/benchmarking.py
+-rw-r--r--   0        0        0    18022 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/containers.py
+-rw-r--r--   0        0        0     4015 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/exponential.py
+-rw-r--r--   0        0        0     5507 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/gaussian.py
+-rw-r--r--   0        0        0     3235 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/lorentzian.py
+-rw-r--r--   0        0        0    12425 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/polynomial.py
+-rw-r--r--   0        0        0    16336 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/rabi.py
+-rw-r--r--   0        0        0     4332 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/rectangle.py
+-rw-r--r--   0        0        0     6081 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/sinc.py
+-rw-r--r--   0        0        0     6849 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/sinusoid.py
+-rw-r--r--   0        0        0     7341 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/triangle.py
+-rw-r--r--   0        0        0     5208 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/models/utils.py
+-rw-r--r--   0        0        0     4855 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/normal.py
+-rw-r--r--   0        0        0      655 2023-04-27 20:37:18.064410 ionics_fits-1.0.5/ionics_fits/utils.py
+-rw-r--r--   0        0        0     1032 2023-04-27 20:37:35.156451 ionics_fits-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11513 1970-01-01 00:00:00.000000 ionics_fits-1.0.5/setup.py
+-rw-r--r--   0        0        0    11088 1970-01-01 00:00:00.000000 ionics_fits-1.0.5/PKG-INFO
```

### Comparing `ionics_fits-1.0.4/LICENSE` & `ionics_fits-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/README.md` & `ionics_fits-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -129,17 +129,16 @@
 The library is designed to be extensible and ergonomic to user. Want to use different
 statistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some
 custom post-fit processing? Override the `calculate_derived_parameters` method. Want to
 tweak the parameter estimator for a model? Create a new model class that inherits from
 the original model and modify away. If you're struggling to do what you want, it's
 probably a bug in the library so please report it.
 
-`ionics_fits` provides a number of tools to make it easier to extend models (see, for
-example in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...
-
+`ionics_fits` provides a number of tools to make it easier to extend models. See, for
+example [`models.utils`](../master/ionics_fits/models/utils.py) and [`models.containers`](../master/ionics_fits/models/containers.py). Suppose you want to...
 ## Rescaling models
 
 ...fit some frequency-domain Rabi oscillation data. However, the model works in angular
 units, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`
 tool.
 
 ```python
@@ -169,15 +168,15 @@
         derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB
 
         return derived_params, derived_uncertainties
 
 RabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)
 ```
 
-## Aggregating models
+## Containers
 
 ...fit multiple independent models simultaneously and do some post-processing on the
 results. Use an `AggregateModel`.
 
 ```python
 class LineAndTriange(fits.models.AggregateModel):
   def __init__(self):
@@ -193,14 +192,34 @@
       fit_uncertainties: Dict[str, float],
   ) -> Tuple[Dict[str, float], Dict[str, float]]:
       derived_params, derived_uncertainties = super().calculate_derived_params()
       # derive new results from the two fits
       return derived_params, derived_uncertainties
 ```
 
+...use the single-qubit Rabi flop model to fit simultaneous Rabi flopping on multiple
+qubits at once with some parameters shared and some independent.
+
+```python
+class MultiRabiFreq(fits.models.RepeatedModel):
+    def __init__(self, n_qubits):
+        super().__init__(
+            inner=fits.models.RabiFlopFreq(start_excited=True),
+            common_params=[
+                "P_readout_e",
+                "P_readout_g",
+                "t_pulse",
+                "omega",
+                "tau",
+                "t_dead",
+            ],
+            num_repetitions=n_qubits,
+        )
+
+```
 ## And more!
 
 At present the library is still an MVP. Further work will be driven by use cases, so
 please open an issue if you find you can't easily extend the library in the way you
 want.
 
 # Ontology
```

### Comparing `ionics_fits-1.0.4/ionics_fits/common.py` & `ionics_fits-1.0.5/ionics_fits/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,17 +575,24 @@
             None if sigma is None else np.logical_and(np.isfinite(sigma), sigma != 0)
         )
 
         if model.get_num_y_channels() > 1:
             valid_y = np.all(valid_y, axis=1)
             valid_sigma = None if sigma is None else np.all(valid_sigma, axis=1)
 
+        valid_x = np.atleast_2d(valid_x.T).T
+        valid_y = np.atleast_2d(valid_y.T).T
+
+        if valid_sigma is not None:
+            valid_sigma = np.atleast_2d(np.isfinite(valid_sigma).T).T
+
         valid_pts = np.logical_and(valid_x, valid_y)
         if sigma is not None:
             valid_pts = np.logical_and(valid_pts, valid_sigma)
+        valid_pts = valid_pts.squeeze()
 
         x = x[valid_pts]
         y = y[valid_pts]
         sigma = None if sigma is None else sigma[valid_pts]
 
         inds = np.argsort(x)
         x = x[inds]
```

### Comparing `ionics_fits-1.0.4/ionics_fits/models/aggregate_model.py` & `ionics_fits-1.0.5/ionics_fits/models/benchmarking.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,135 @@
-from typing import Dict, List, Optional, Tuple, TYPE_CHECKING
+from typing import Dict, Tuple, TYPE_CHECKING
 
 import numpy as np
 
 from .. import Model, ModelParameter
 from ..utils import Array
 
-
 if TYPE_CHECKING:
     num_samples = float
-    num_y_channels = float
-
 
-class AggregateModel(Model):
-    """Model formed by aggregating one or more models"""
 
-    def __init__(
-        self,
-        models: List[Tuple[str, Model]],
-        common_params: Optional[List[str]] = None,
-    ):
-        """
-        :param models: The models to be aggregated. This should be a list of tuples,
-          with each element containing a model name string and a model instance. The
-          model names are used as prefixes for names of model parameters and derived
-          results. For example, if one of the aggregated models named `foo` has a
-          parameter `bar`, the aggregate model will have a parameter `foo_bar`. The
-          aggregated model instances are considered to be "owned" by the aggregate model
-          and may be mutated by it - for example to set heuristic values.
-
-        At present this class only supports models with a single y channel. This is just
-        because no one got around to implementing it yet rather than any fundamental
-        difficulty.
-
-        A possible future extension of this class would be to introduce a notion of
-        "common parameters", whose value is the same for all of the aggregated models. A
-        design question here is where the common parameters should get their properties
-        (bounds, scale factors, etc) from and how we should deal with their heuristics.
-        """
-        self.models = models
+def _scale_func(x_scale, y_scale, model):
+    # Prevent rescaling
+    return None
+
+
+def _generate_benchmarking_parameters(num_qubits):
+    params = {
+        "p": ModelParameter(lower_bound=0.0, upper_bound=1.0, scale_func=_scale_func),
+        "y0": ModelParameter(
+            lower_bound=0.0,
+            upper_bound=1.0,
+            scale_func=lambda x_scale, y_scale, _: y_scale,
+        ),
+        "y_inf": ModelParameter(
+            fixed_to=1 / 2**num_qubits,
+            lower_bound=0,
+            upper_bound=1,
+            scale_func=lambda x_scale, y_scale, _: y_scale,
+        ),
+    }
+    return params
+
+
+class Benchmarking(Model):
+    """Benchmarking success probability decay model
+
+    y = (y0 - y_inf)*p^x + y_inf
+    for sequence length x.
+
+    Fit parameters (all floated by default unless stated otherwise):
+      - p: depolarisation parameter
+      - y0: SPAM fidelity estimate
+      - y_inf: depolarisation offset (y-axis asymptote) (fixed to 1/2^n by default)
+
+    Derived parameters:
+      - e: error per Clifford = (1 - p) / alpha_n where alpha_n = 2^n / (2^n - 1)
+      - e_spam: estimated SPAM error = 1 - y0
+    """
 
-        parameters = {}
-        for model_name, model in self.models:
-            if model.get_num_y_channels() != 1:
-                raise ValueError(
-                    "AggregateModel only supports models with a single y channel"
-                )
-            parameters.update(
-                {
-                    f"{model_name}_{param_name}": param
-                    for param_name, param in model.parameters.items()
-                }
-            )
+    def __init__(self, num_qubits):
+        """Init
 
-        super().__init__(parameters=parameters)
-
-    def get_num_y_channels(self) -> int:
-        return len(self.models)
+        :param num_qubits: The number of qubits involved in the benchmarking sequence.
+        """
+        self.num_qubits = num_qubits
+        self.alpha = 2**num_qubits / (2**num_qubits - 1)
+        super().__init__(parameters=_generate_benchmarking_parameters(num_qubits))
 
     def func(
-        self,
-        x: Array[("num_samples",), np.float64],
-        param_values: Dict[str, float],
-    ) -> Array[("num_samples", "num_y_channels"), np.float64]:
-        ys = []
-        for model_name, model in self.models:
-            model_params = {
-                param_name: param_values[f"{model_name}_{param_name}"]
-                for param_name in model.parameters.keys()
-            }
-            ys.append(model.func(x, model_params))
-
-        return np.stack(ys).T
+        self, x: Array[("num_samples",), np.float64], params: Dict[str, float]
+    ) -> Array[("num_samples",), np.float64]:
+        """Evaluates the model at a given set of x-axis points and with a given
+        parameter set and returns the result."""
+        p = params["p"]
+        y0 = params["y0"]
+        y_inf = params["y_inf"]
+        y = (y0 - y_inf) * p**x + y_inf
+        return y
 
     def estimate_parameters(
         self,
         x: Array[("num_samples",), np.float64],
-        y: Array[("num_samples", "num_y_channels"), np.float64],
+        y: Array[("num_samples",), np.float64],
         model_parameters: Dict[str, ModelParameter],
     ):
-        for idx, (model_name, model) in enumerate(self.models):
-            params = {
-                param_name: model_parameters[f"{model_name}_{param_name}"]
-                for param_name in model.parameters.keys()
-            }
-            model.estimate_parameters(x, y[:, idx], params)
+        """Set heuristic values for model parameters.
+
+        Typically called during `Fitter.fit`. This method may make use of information
+        supplied by the user for some parameters (via the `fixed_to` or
+        `user_estimate` attributes) to find initial guesses for other parameters.
+
+        The datasets must be sorted in order of increasing x-axis values and must not
+        contain any infinite or nan values. If all parameters of the model allow
+        rescaling, then `x`, `y` and `model_parameters` will contain rescaled values.
+
+        :param x: x-axis data, rescaled if allowed.
+        :param y: y-axis data, rescaled if allowed.
+        :param model_parameters: dictionary mapping model parameter names to their
+            metadata, rescaled if allowed.
+        """
+        model_parameters["p"].heuristic = 1.0
+        model_parameters["y0"].heuristic = max(y)
+        model_parameters["y_inf"].heuristic = 1 / 2**self.num_qubits
 
     def calculate_derived_params(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         fitted_params: Dict[str, float],
         fit_uncertainties: Dict[str, float],
     ) -> Tuple[Dict[str, float], Dict[str, float]]:
+        """
+        Returns dictionaries of values and uncertainties for the derived model
+        parameters (parameters which are calculated from the fit results rather than
+        being directly part of the fit) based on values of the fitted parameters and
+        their uncertainties.
+
+        :param x: x-axis data
+        :param y: y-axis data
+        :param: fitted_params: dictionary mapping model parameter names to their
+            fitted values.
+        :param fit_uncertainties: dictionary mapping model parameter names to
+            their fit uncertainties.
+        :returns: tuple of dictionaries mapping derived parameter names to their
+            values and uncertainties.
+        """
+        p = fitted_params["p"]
+        y0 = fitted_params["y0"]
+
+        e = (1 - p) / self.alpha
+        e_spam = 1 - y0
+
+        p_err = fit_uncertainties["p"]
+        y0_err = fit_uncertainties["y0"]
+
         derived_params = {}
-        derived_uncertainties = {}
+        derived_params["e"] = e
+        derived_params["e_spam"] = e_spam
 
-        for idx, (model_name, model) in enumerate(self.models):
-            model_fitted_params = {
-                param_name: fitted_params[f"{model_name}_{param_name}"]
-                for param_name in model.parameters.keys()
-            }
-            model_fitted_uncertainties = {
-                param_name: fit_uncertainties[f"{model_name}_{param_name}"]
-                for param_name in model.parameters.keys()
-            }
-
-            derived = model.calculate_derived_params(
-                x=x,
-                y=y[:, idx],
-                fitted_params=model_fitted_params,
-                fit_uncertainties=model_fitted_uncertainties,
-            )
-            model_derived_params, model_derived_uncertainties = derived
-
-            derived_params.update(
-                {
-                    f"{model_name}_{param_name}": value
-                    for param_name, value in model_derived_params.items()
-                }
-            )
-            derived_uncertainties.update(
-                {
-                    f"{model_name}_{param_name}": value
-                    for param_name, value in model_derived_uncertainties.items()
-                }
-            )
+        derived_uncertainties = {}
+        derived_uncertainties["e"] = p_err / self.alpha
+        derived_uncertainties["e_spam"] = y0_err
 
         return derived_params, derived_uncertainties
```

### Comparing `ionics_fits-1.0.4/ionics_fits/models/benchmarking.py` & `ionics_fits-1.0.5/ionics_fits/models/gaussian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,58 @@
 from typing import Dict, Tuple, TYPE_CHECKING
-
 import numpy as np
 
+from .utils import get_spectrum
 from .. import Model, ModelParameter
 from ..utils import Array
 
+
 if TYPE_CHECKING:
     num_samples = float
 
 
-def _scale_func(x_scale, y_scale, model):
-    # Prevent rescaling
-    return None
-
-
-def _generate_benchmarking_parameters(num_qubits):
-    params = {
-        "p": ModelParameter(lower_bound=0.0, upper_bound=1.0, scale_func=_scale_func),
-        "y0": ModelParameter(
-            lower_bound=0.0,
-            upper_bound=1.0,
-            scale_func=lambda x_scale, y_scale, _: y_scale,
-        ),
-        "y_inf": ModelParameter(
-            fixed_to=1 / 2**num_qubits,
-            lower_bound=0,
-            upper_bound=1,
-            scale_func=lambda x_scale, y_scale, _: y_scale,
-        ),
-    }
-    return params
-
-
-class Benchmarking(Model):
-    """Benchmarking success probability decay model
-
-    y = (y0 - y_inf)*p^x + y_inf
-    for sequence length x.
+class Gaussian(Model):
+    """Gaussian model according to:
+    y = a / (sigma * sqrt(2*pi)) * exp(-(x-x0)^2/(2*sigma)^2) + y0
 
     Fit parameters (all floated by default unless stated otherwise):
-      - p: depolarisation parameter
-      - y0: SPAM fidelity estimate
-      - y_inf: depolarisation offset (y-axis asymptote) (fixed to 1/2^n by default)
+      - x0: x-axis offset
+      - y0: y-axis offset
+      - a: y-axis scale factor. The Gaussian is normalized such that its integral is
+        equal to a.
+      - sigma: distribution half-width at 1/e of maximum height is 2*sigma (sigma is the
+        1/sqrt(e) radius).
 
     Derived parameters:
-      - e: error per Clifford = (1 - p) / alpha_n where alpha_n = 2^n / (2^n - 1)
-      - e_spam: estimated SPAM error = 1 - y0
+      - FWHMH: full width at half-maximum height
+      - peak: peak height above y0
+      - w0: full width at 1/e max height. For Gaussian beams this is the beam waist
     """
 
-    def __init__(self, num_qubits):
-        """Init
-
-        :param num_qubits: The number of qubits involved in the benchmarking sequence.
-        """
-        self.num_qubits = num_qubits
-        self.alpha = 2**num_qubits / (2**num_qubits - 1)
-        super().__init__(parameters=_generate_benchmarking_parameters(num_qubits))
-
-    def func(
-        self, x: Array[("num_samples",), np.float64], params: Dict[str, float]
+    # pytype: disable=invalid-annotation
+    def _func(
+        self,
+        x: Array[("num_samples",), np.float64],
+        x0: ModelParameter(scale_func=lambda x_scale, y_scale, _: x_scale),
+        y0: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale),
+        a: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale * x_scale),
+        sigma: ModelParameter(
+            lower_bound=0, scale_func=lambda x_scale, y_scale, _: x_scale
+        ),
     ) -> Array[("num_samples",), np.float64]:
-        """Evaluates the model at a given set of x-axis points and with a given
-        parameter set and returns the result."""
-        p = params["p"]
-        y0 = params["y0"]
-        y_inf = params["y_inf"]
-        y = (y0 - y_inf) * p**x + y_inf
+        y = (
+            a
+            / (sigma * np.sqrt(2 * np.pi))
+            * np.exp(-np.power((x - x0) / (2 * sigma), 2))
+            + y0
+        )
         return y
 
+    # pytype: enable=invalid-annotation
+
     def estimate_parameters(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         model_parameters: Dict[str, ModelParameter],
     ):
         """Set heuristic values for model parameters.
@@ -85,17 +66,52 @@
         rescaling, then `x`, `y` and `model_parameters` will contain rescaled values.
 
         :param x: x-axis data, rescaled if allowed.
         :param y: y-axis data, rescaled if allowed.
         :param model_parameters: dictionary mapping model parameter names to their
             metadata, rescaled if allowed.
         """
-        model_parameters["p"].heuristic = 1.0
-        model_parameters["y0"].heuristic = max(y)
-        model_parameters["y_inf"].heuristic = 1 / 2**self.num_qubits
+        # Gaussian Fourier Transform:
+        #   F[A * exp(-(x/w)^2)](k) = A * sqrt(pi) * w * exp(-(pi*k*w)^2)
+        #
+        # Half-width at 1/e when k = 1/(pi*w)
+        omega, spectrum = get_spectrum(x, y, trim_dc=True)
+        abs_spectrum = np.abs(spectrum)
+
+        k = omega / (2 * np.pi)
+
+        peak = np.max(abs_spectrum)
+        W = peak / np.exp(1)
+        width = 1 / (np.pi * k[np.argmin(np.abs(abs_spectrum - W))])
+
+        sigma = width / 2
+        a = peak * np.pi * np.sqrt(2)
+
+        model_parameters["y0"].heuristic = np.mean([y[0], y[-1]])
+        y0 = model_parameters["y0"].get_initial_value()
+        peak_idx = np.argmax(np.abs(y - y0))
+        y_peak = y[peak_idx]
+        sgn = 1 if y_peak > y0 else -1
+
+        model_parameters["a"].heuristic = a * sgn
+        model_parameters["sigma"].heuristic = sigma
+
+        cut_off = 2 * omega[np.argmin(np.abs(abs_spectrum - W))]
+
+        x0 = self.find_x_offset_sym_peak(
+            x=x,
+            y=y,
+            parameters=model_parameters,
+            omega=omega,
+            spectrum=spectrum,
+            omega_cut_off=cut_off,
+            test_pts=x[peak_idx],
+        )
+
+        model_parameters["x0"].heuristic = x0
 
     def calculate_derived_params(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         fitted_params: Dict[str, float],
         fit_uncertainties: Dict[str, float],
@@ -111,25 +127,25 @@
         :param: fitted_params: dictionary mapping model parameter names to their
             fitted values.
         :param fit_uncertainties: dictionary mapping model parameter names to
             their fit uncertainties.
         :returns: tuple of dictionaries mapping derived parameter names to their
             values and uncertainties.
         """
-        p = fitted_params["p"]
-        y0 = fitted_params["y0"]
-
-        e = (1 - p) / self.alpha
-        e_spam = 1 - y0
-
-        p_err = fit_uncertainties["p"]
-        y0_err = fit_uncertainties["y0"]
+        sigma = fitted_params["sigma"]
+        a = fitted_params["a"]
 
         derived_params = {}
-        derived_params["e"] = e
-        derived_params["e_spam"] = e_spam
+        derived_params["FWHMH"] = 2.35482 * sigma
+        derived_params["peak"] = a / (sigma * np.sqrt(2 * np.pi))
+        derived_params["w0"] = 4 * sigma
 
         derived_uncertainties = {}
-        derived_uncertainties["e"] = p_err / self.alpha
-        derived_uncertainties["e_spam"] = y0_err
+        derived_uncertainties["FWHMH"] = 2.35482 * fit_uncertainties["sigma"]
+        derived_uncertainties["peak"] = (
+            fit_uncertainties["a"] / (sigma * np.sqrt(2 * np.pi))
+        ) ** 2 + (
+            fit_uncertainties["sigma"] * a / (sigma**2 * np.sqrt(2 * np.pi))
+        ) ** 2
+        derived_uncertainties["w0"] = 4 * fit_uncertainties["sigma"]
 
         return derived_params, derived_uncertainties
```

### Comparing `ionics_fits-1.0.4/ionics_fits/models/exponential.py` & `ionics_fits-1.0.5/ionics_fits/models/exponential.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/models/gaussian.py` & `ionics_fits-1.0.5/ionics_fits/models/sinusoid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,73 @@
-from typing import Dict, Tuple, TYPE_CHECKING
+import copy
 import numpy as np
+from typing import Dict, Tuple, TYPE_CHECKING
 
-from .utils import get_spectrum
 from .. import Model, ModelParameter
 from ..utils import Array
-
+from . import utils
 
 if TYPE_CHECKING:
     num_samples = float
 
 
-class Gaussian(Model):
-    """Gaussian model according to:
-    y = a / (sigma * sqrt(2*pi)) * exp(-(x-x0)^2/(2*sigma)^2) + y0
+class Sinusoid(Model):
+    """Generalised sinusoid fit according to:
+    y = Gamma * a * sin[omega * (x - x0) + phi] + y0
+    where Gamma = exp(-x / tau).
 
     Fit parameters (all floated by default unless stated otherwise):
-      - x0: x-axis offset
+      - a: initial (x = 0) amplitude of the sinusoid
+      - omega: angular frequency
+      - phi: phase offset (radians)
       - y0: y-axis offset
-      - a: y-axis scale factor. The Gaussian is normalized such that its integral is
-        equal to a.
-      - sigma: distribution half-width at 1/e of maximum height is 2*sigma (sigma is the
-        1/sqrt(e) radius).
+      - x0: x-axis offset (fixed to 0 by default)
+      - tau: decay/growth constant (fixed to np.inf by default)
 
     Derived parameters:
-      - FWHMH: full width at half-maximum height
-      - peak: peak height above y0
-      - w0: full width at 1/e max height. For Gaussian beams this is the beam waist
+      - f: frequency
+      - phi_cosine: cosine phase (phi + pi/2)
+      - contrast: peak-to-peak amplitude of the pure sinusoid
+      - min/max: min / max values of the pure sinusoid
+      - period: period of oscillation
+      - TODO: peak values of the damped sinusoid as well as `x` value that the peak
+          occurs at.
+
+    All phases are in radians, frequencies are in angular units.
+
+    x0 and phi0 are equivalent parametrisations for the phase offset, but in some cases
+    it works out convenient to have access to both (e.g. one as a fixed offset, the
+    other floated). At most one of them should be floated at once. By default, x0 is
+    fixed at 0 and phi0 is floated.
     """
 
     # pytype: disable=invalid-annotation
     def _func(
         self,
         x: Array[("num_samples",), np.float64],
-        x0: ModelParameter(scale_func=lambda x_scale, y_scale, _: x_scale),
+        a: ModelParameter(
+            lower_bound=0, scale_func=lambda x_scale, y_scale, _: y_scale
+        ),
+        omega: ModelParameter(
+            lower_bound=0, scale_func=lambda x_scale, y_scale, _: 1 / x_scale
+        ),
+        phi: utils.PeriodicModelParameter(
+            period=2 * np.pi,
+            offset=-np.pi,
+        ),
         y0: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale),
-        a: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale * x_scale),
-        sigma: ModelParameter(
-            lower_bound=0, scale_func=lambda x_scale, y_scale, _: x_scale
+        x0: ModelParameter(fixed_to=0, scale_func=lambda x_scale, y_scale, _: x_scale),
+        tau: ModelParameter(
+            lower_bound=0,
+            fixed_to=np.inf,
+            scale_func=lambda x_scale, y_scale, _: x_scale,
         ),
     ) -> Array[("num_samples",), np.float64]:
-        y = (
-            a
-            / (sigma * np.sqrt(2 * np.pi))
-            * np.exp(-np.power((x - x0) / (2 * sigma), 2))
-            + y0
-        )
+        Gamma = np.exp(-x / tau)
+        y = Gamma * a * np.sin(omega * (x - x0) + phi) + y0
         return y
 
     # pytype: enable=invalid-annotation
 
     def estimate_parameters(
         self,
         x: Array[("num_samples",), np.float64],
@@ -66,52 +85,47 @@
         rescaling, then `x`, `y` and `model_parameters` will contain rescaled values.
 
         :param x: x-axis data, rescaled if allowed.
         :param y: y-axis data, rescaled if allowed.
         :param model_parameters: dictionary mapping model parameter names to their
             metadata, rescaled if allowed.
         """
-        # Gaussian Fourier Transform:
-        #   F[A * exp(-(x/w)^2)](k) = A * sqrt(pi) * w * exp(-(pi*k*w)^2)
-        #
-        # Half-width at 1/e when k = 1/(pi*w)
-        omega, spectrum = get_spectrum(x, y, trim_dc=True)
-        abs_spectrum = np.abs(spectrum)
-
-        k = omega / (2 * np.pi)
-
-        peak = np.max(abs_spectrum)
-        W = peak / np.exp(1)
-        width = 1 / (np.pi * k[np.argmin(np.abs(abs_spectrum - W))])
-
-        sigma = width / 2
-        a = peak * np.pi * np.sqrt(2)
-
-        model_parameters["y0"].heuristic = np.mean([y[0], y[-1]])
-        y0 = model_parameters["y0"].get_initial_value()
-        peak_idx = np.argmax(np.abs(y - y0))
-        y_peak = y[peak_idx]
-        sgn = 1 if y_peak > y0 else -1
-
-        model_parameters["a"].heuristic = a * sgn
-        model_parameters["sigma"].heuristic = sigma
-
-        cut_off = 2 * omega[np.argmin(np.abs(abs_spectrum - W))]
-
-        x0 = self.find_x_offset_sym_peak(
+        # We don't have good heuristics for these parameters
+        model_parameters["y0"].heuristic = np.mean(y)
+        model_parameters["tau"].heuristic = np.max(x)
+
+        omega, spectrum = utils.get_spectrum(x, y, density_units=False, trim_dc=True)
+        spectrum = np.abs(spectrum)
+        peak = np.argmax(spectrum)
+
+        model_parameters["a"].heuristic = spectrum[peak] * 2
+        model_parameters["omega"].heuristic = omega[peak]
+
+        phi_params = copy.deepcopy(model_parameters)
+        phi_params["x0"].heuristic = 0.0
+        phi, _ = self.param_min_sqrs(
             x=x,
             y=y,
-            parameters=model_parameters,
-            omega=omega,
-            spectrum=spectrum,
-            omega_cut_off=cut_off,
-            test_pts=x[peak_idx],
+            parameters=phi_params,
+            scanned_param="phi",
+            scanned_param_values=np.linspace(-np.pi, np.pi, num=20),
         )
+        phi = model_parameters["phi"].clip(phi)
 
-        model_parameters["x0"].heuristic = x0
+        if model_parameters["x0"].fixed_to is None:
+            if model_parameters["phi"].fixed_to is None:
+                raise ValueError("Only one of 'x0' and 'phi' may be floated at once")
+
+            model_parameters["phi"].heuristic = 0
+            model_parameters["x0"].heuristic = (
+                -phi / model_parameters["omega"].get_initial_value()
+            )
+        else:
+            model_parameters["phi"].heuristic = phi
+            model_parameters["x0"].heuristic = 0.0
 
     def calculate_derived_params(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         fitted_params: Dict[str, float],
         fit_uncertainties: Dict[str, float],
@@ -127,25 +141,30 @@
         :param: fitted_params: dictionary mapping model parameter names to their
             fitted values.
         :param fit_uncertainties: dictionary mapping model parameter names to
             their fit uncertainties.
         :returns: tuple of dictionaries mapping derived parameter names to their
             values and uncertainties.
         """
-        sigma = fitted_params["sigma"]
-        a = fitted_params["a"]
-
         derived_params = {}
-        derived_params["FWHMH"] = 2.35482 * sigma
-        derived_params["peak"] = a / (sigma * np.sqrt(2 * np.pi))
-        derived_params["w0"] = 4 * sigma
+        derived_params["f"] = fitted_params["omega"] / (2 * np.pi)
+        derived_params["phi_cosine"] = fitted_params["phi"] + np.pi / 2
+        derived_params["contrast"] = 2 * np.abs(fitted_params["a"])
+        derived_params["min"] = fitted_params["y0"] - np.abs(fitted_params["a"])
+        derived_params["max"] = fitted_params["y0"] + np.abs(fitted_params["a"])
+        derived_params["period"] = 2 * np.pi / fitted_params["omega"]
 
         derived_uncertainties = {}
-        derived_uncertainties["FWHMH"] = 2.35482 * fit_uncertainties["sigma"]
-        derived_uncertainties["peak"] = (
-            fit_uncertainties["a"] / (sigma * np.sqrt(2 * np.pi))
-        ) ** 2 + (
-            fit_uncertainties["sigma"] * a / (sigma**2 * np.sqrt(2 * np.pi))
-        ) ** 2
-        derived_uncertainties["w0"] = 4 * fit_uncertainties["sigma"]
+        derived_uncertainties["f"] = fit_uncertainties["omega"] / (2 * np.pi)
+        derived_uncertainties["phi_cosine"] = fit_uncertainties["phi"]
+        derived_uncertainties["contrast"] = 2 * fit_uncertainties["a"]
+        derived_uncertainties["min"] = np.sqrt(
+            fit_uncertainties["y0"] ** 2 + fit_uncertainties["a"] ** 2
+        )
+        derived_uncertainties["max"] = np.sqrt(
+            fit_uncertainties["y0"] ** 2 + fit_uncertainties["a"] ** 2
+        )
+        derived_uncertainties["period"] = (
+            2 * np.pi * fit_uncertainties["omega"] / (fitted_params["omega"] ** 2)
+        )
 
         return derived_params, derived_uncertainties
```

### Comparing `ionics_fits-1.0.4/ionics_fits/models/lorentzian.py` & `ionics_fits-1.0.5/ionics_fits/models/lorentzian.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/models/polynomial.py` & `ionics_fits-1.0.5/ionics_fits/models/polynomial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional, TYPE_CHECKING
 
 import numpy as np
 
-from .utils import MappedModel
+from .containers import MappedModel
 from .. import Model, ModelParameter
 from ..utils import Array
 
 if TYPE_CHECKING:
     num_samples = float
```

### Comparing `ionics_fits-1.0.4/ionics_fits/models/rabi.py` & `ionics_fits-1.0.5/ionics_fits/models/rabi.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/models/rectangle.py` & `ionics_fits-1.0.5/ionics_fits/models/rectangle.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/models/sinc.py` & `ionics_fits-1.0.5/ionics_fits/models/sinc.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/models/sinusoid.py` & `ionics_fits-1.0.5/ionics_fits/models/triangle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,67 @@
 import copy
-import numpy as np
 from typing import Dict, Tuple, TYPE_CHECKING
+import numpy as np
 
 from .. import Model, ModelParameter
 from ..utils import Array
-from . import utils
 
 if TYPE_CHECKING:
     num_samples = float
 
 
-class Sinusoid(Model):
-    """Generalised sinusoid fit according to:
-    y = Gamma * a * sin[omega * (x - x0) + phi] + y0
-    where Gamma = exp(-x / tau).
+class Triangle(Model):
+    """Triangle function according to:
+    y(x>=x0) = k_p*|x-x0| + y0
+    y(x<x0) = k_m*|x-x0| + y0
+    y = max(y, y_min)
+    y = min(y, m_max)
+    k_p = (1 + sym) * k
+    k_m = (1 - sym) * k
 
     Fit parameters (all floated by default unless stated otherwise):
-      - a: initial (x = 0) amplitude of the sinusoid
-      - omega: angular frequency
-      - phi: phase offset (radians)
+      - x0: x-axis offset
       - y0: y-axis offset
-      - x0: x-axis offset (fixed to 0 by default)
-      - tau: decay/growth constant (fixed to np.inf by default)
+      - k: average slope
+      - sym: symmetry parameter (fixed to 0 by default)
+      - y_min: minimum value of y (bound to -inf by default)
+      - y_max: maximum value of y (bound to +inf by default)
 
     Derived parameters:
-      - f: frequency
-      - phi_cosine: cosine phase (phi + pi/2)
-      - contrast: peak-to-peak amplitude of the pure sinusoid
-      - min/max: min / max values of the pure sinusoid
-      - period: period of oscillation
-      - TODO: peak values of the damped sinusoid as well as `x` value that the peak
-          occurs at.
-
-    All phases are in radians, frequencies are in angular units.
-
-    x0 and phi0 are equivalent parametrisations for the phase offset, but in some cases
-    it works out convenient to have access to both (e.g. one as a fixed offset, the
-    other floated). At most one of them should be floated at once. By default, x0 is
-    fixed at 0 and phi0 is floated.
+      - k_m: slope for x < x0
+      - k_p: slope for x >= x0
     """
 
     # pytype: disable=invalid-annotation
     def _func(
         self,
         x: Array[("num_samples",), np.float64],
-        a: ModelParameter(
-            lower_bound=0, scale_func=lambda x_scale, y_scale, _: y_scale
-        ),
-        omega: ModelParameter(
-            lower_bound=0, scale_func=lambda x_scale, y_scale, _: 1 / x_scale
-        ),
-        phi: utils.PeriodicModelParameter(
-            period=2 * np.pi,
-            offset=-np.pi,
-        ),
+        x0: ModelParameter(scale_func=lambda x_scale, y_scale, _: x_scale),
         y0: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale),
-        x0: ModelParameter(fixed_to=0, scale_func=lambda x_scale, y_scale, _: x_scale),
-        tau: ModelParameter(
-            lower_bound=0,
-            fixed_to=np.inf,
-            scale_func=lambda x_scale, y_scale, _: x_scale,
+        k: ModelParameter(scale_func=lambda x_scale, y_scale, _: y_scale / x_scale),
+        sym: ModelParameter(lower_bound=-1, upper_bound=1, fixed_to=0),
+        y_min: ModelParameter(
+            fixed_to=-np.inf, scale_func=lambda x_scale, y_scale, _: y_scale
+        ),
+        y_max: ModelParameter(
+            fixed_to=+np.inf, scale_func=lambda x_scale, y_scale, _: y_scale
         ),
     ) -> Array[("num_samples",), np.float64]:
-        Gamma = np.exp(-x / tau)
-        y = Gamma * a * np.sin(omega * (x - x0) + phi) + y0
+        k_p = k * (1 + sym)
+        k_m = k * (1 - sym)
+
+        y_p = k_p * np.abs(x - x0) + y0
+        y_m = k_m * np.abs(x - x0) + y0
+        y = np.where(x >= x0, y_p, y_m)
+        y = np.where(y > y_min, y, y_min)
+        y = np.where(y < y_max, y, y_max)
+
         return y
 
     # pytype: enable=invalid-annotation
-
     def estimate_parameters(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         model_parameters: Dict[str, ModelParameter],
     ):
         """Set heuristic values for model parameters.
@@ -85,47 +75,95 @@
         rescaling, then `x`, `y` and `model_parameters` will contain rescaled values.
 
         :param x: x-axis data, rescaled if allowed.
         :param y: y-axis data, rescaled if allowed.
         :param model_parameters: dictionary mapping model parameter names to their
             metadata, rescaled if allowed.
         """
-        # We don't have good heuristics for these parameters
-        model_parameters["y0"].heuristic = np.mean(y)
-        model_parameters["tau"].heuristic = np.max(x)
-
-        omega, spectrum = utils.get_spectrum(x, y, density_units=False, trim_dc=True)
-        spectrum = np.abs(spectrum)
-        peak = np.argmax(spectrum)
-
-        model_parameters["a"].heuristic = spectrum[peak] * 2
-        model_parameters["omega"].heuristic = omega[peak]
-
-        phi_params = copy.deepcopy(model_parameters)
-        phi_params["x0"].heuristic = 0.0
-        phi, _ = self.param_min_sqrs(
-            x=x,
-            y=y,
-            parameters=phi_params,
-            scanned_param="phi",
-            scanned_param_values=np.linspace(-np.pi, np.pi, num=20),
+        # Written to be handle the case of data which is only well-modelled by a
+        # triangle function near `x0` but saturates further away
+        model_parameters["y_max"].heuristic = max(y)
+        model_parameters["y_min"].heuristic = min(y)
+
+        min_ind = np.argmin(y)
+        max_ind = np.argmax(y)
+
+        y_min = y[min_ind]
+        y_max = y[max_ind]
+        x_min = x[min_ind]
+        x_max = x[max_ind]
+
+        # Case 1: positive slope with peaks left and right of x_min above y_min
+        x_l = x[x <= x_min]
+        x_r = x[x >= x_min]
+        y_l = y[x <= x_min]
+        y_r = y[x >= x_min]
+
+        left_peak_ind = np.argmax(y_l)
+        right_peak_ind = np.argmax(y_r)
+
+        dx_l = x_min - x_l[left_peak_ind]
+        dx_r = x_r[right_peak_ind] - x_min
+
+        k_m = (y_l[left_peak_ind] - y_min) / dx_l if dx_l != 0 else 0
+        k_p = (y_r[right_peak_ind] - y_min) / dx_r if dx_r != 0 else 0
+        alpha = 0 if k_m == 0 else k_p / k_m
+
+        positive_parameters = copy.deepcopy(model_parameters)
+        positive_parameters["x0"].heuristic = x_min
+        positive_parameters["y0"].heuristic = y_min
+
+        positive_parameters["k"].heuristic = 0.5 * (k_p + k_m)
+        positive_parameters["sym"].heuristic = (alpha - 1) / (1 + alpha)
+
+        positive_parameters = {
+            param: param_data.get_initial_value()
+            for param, param_data in positive_parameters.items()
+        }
+        positive_residuals = np.sum(
+            np.power(y - self._func(x, **positive_parameters), 2)
+        )
+
+        # Case 2: negative slope with peaks left and right of x_max below y_max
+        x_l = x[x <= x_max]
+        x_r = x[x >= x_max]
+        y_l = y[x <= x_max]
+        y_r = y[x >= x_max]
+
+        left_peak_ind = np.argmin(y_l)
+        right_peak_ind = np.argmin(y_r)
+
+        dx_l = x_max - x_l[left_peak_ind]
+        dx_r = x_r[right_peak_ind] - x_max
+
+        k_m = (y_l[left_peak_ind] - y_max) / dx_l if dx_l != 0 else 0
+        k_p = (y_r[right_peak_ind] - y_max) / dx_r if dx_r != 0 else 0
+        alpha = 0 if k_m == 0 else k_p / k_m
+
+        negative_parameters = copy.deepcopy(model_parameters)
+        negative_parameters["x0"].heuristic = x_max
+        negative_parameters["y0"].heuristic = y_max
+        negative_parameters["k"].heuristic = 0.5 * (k_p + k_m)
+        negative_parameters["sym"].heuristic = (alpha - 1) / (1 + alpha)
+
+        negative_parameters = {
+            param: param_data.get_initial_value()
+            for param, param_data in negative_parameters.items()
+        }
+        negative_residuals = np.sum(
+            np.power(y - self._func(x, **negative_parameters), 2)
         )
-        phi = model_parameters["phi"].clip(phi)
 
-        if model_parameters["x0"].fixed_to is None:
-            if model_parameters["phi"].fixed_to is None:
-                raise ValueError("Only one of 'x0' and 'phi' may be floated at once")
-
-            model_parameters["phi"].heuristic = 0
-            model_parameters["x0"].heuristic = (
-                -phi / model_parameters["omega"].get_initial_value()
-            )
+        if positive_residuals < negative_residuals:
+            best_params = positive_parameters
         else:
-            model_parameters["phi"].heuristic = phi
-            model_parameters["x0"].heuristic = 0.0
+            best_params = negative_parameters
+
+        for param, value in best_params.items():
+            model_parameters[param].heuristic = value
 
     def calculate_derived_params(
         self,
         x: Array[("num_samples",), np.float64],
         y: Array[("num_samples",), np.float64],
         fitted_params: Dict[str, float],
         fit_uncertainties: Dict[str, float],
@@ -142,29 +180,25 @@
             fitted values.
         :param fit_uncertainties: dictionary mapping model parameter names to
             their fit uncertainties.
         :returns: tuple of dictionaries mapping derived parameter names to their
             values and uncertainties.
         """
         derived_params = {}
-        derived_params["f"] = fitted_params["omega"] / (2 * np.pi)
-        derived_params["phi_cosine"] = fitted_params["phi"] + np.pi / 2
-        derived_params["contrast"] = 2 * np.abs(fitted_params["a"])
-        derived_params["min"] = fitted_params["y0"] - np.abs(fitted_params["a"])
-        derived_params["max"] = fitted_params["y0"] + np.abs(fitted_params["a"])
-        derived_params["period"] = 2 * np.pi / fitted_params["omega"]
+        k = fitted_params["k"]
+        sym = fitted_params["sym"]
+
+        k_err = fitted_params["k"]
+        sym_err = fitted_params["sym"]
+
+        derived_params["k_p"] = (1 + sym) * k
+        derived_params["k_m"] = (1 - sym) * k
 
         derived_uncertainties = {}
-        derived_uncertainties["f"] = fit_uncertainties["omega"] / (2 * np.pi)
-        derived_uncertainties["phi_cosine"] = fit_uncertainties["phi"]
-        derived_uncertainties["contrast"] = 2 * fit_uncertainties["a"]
-        derived_uncertainties["min"] = np.sqrt(
-            fit_uncertainties["y0"] ** 2 + fit_uncertainties["a"] ** 2
-        )
-        derived_uncertainties["max"] = np.sqrt(
-            fit_uncertainties["y0"] ** 2 + fit_uncertainties["a"] ** 2
+        derived_uncertainties["kp"] = np.sqrt(
+            (k_err * (1 + sym)) ** 2 + (k * sym_err) ** 2
         )
-        derived_uncertainties["period"] = (
-            2 * np.pi * fit_uncertainties["omega"] / (fitted_params["omega"] ** 2)
+        derived_uncertainties["km"] = np.sqrt(
+            (k_err * (1 - sym)) ** 2 + (k * sym_err) ** 2
         )
 
         return derived_params, derived_uncertainties
```

### Comparing `ionics_fits-1.0.4/ionics_fits/normal.py` & `ionics_fits-1.0.5/ionics_fits/normal.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/ionics_fits/utils.py` & `ionics_fits-1.0.5/ionics_fits/utils.py`

 * *Files identical despite different names*

### Comparing `ionics_fits-1.0.4/pyproject.toml` & `ionics_fits-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ionics-fits"
-version = "1.0.4"
+version = "1.0.5"
 description = "Lightweight Python data fitting library with an emphasis on AMO/Quantum Information"
 authors = ["hartytp <thomas.peter.harty@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 numpy = "^1.21.2"
```

### Comparing `ionics_fits-1.0.4/setup.py` & `ionics_fits-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'pyqt5-qt5>=5.15.2,<6.0.0',
  'pyqt5>=5.15.9,<6.0.0',
  'scipy>=1.7.1,<2.0.0',
  'statsmodels>=0.13.2,<0.14.0']
 
 setup_kwargs = {
     'name': 'ionics-fits',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Lightweight Python data fitting library with an emphasis on AMO/Quantum Information',
-    'long_description': 'Lightweight Python library for data fitting with an emphasis on AMO (Atomic Molecular\nand Optical physics) and Quantum Information.\n\n`fits` was inspired by the [Oxford Ion Trap Group fitting library](https://github.com/OxfordIonTrapGroup/oitg/tree/master/oitg/fitting) originally\nauthored by @tballance. It is still in the alpha phase and is likely to be renamed\n(although `fits` is still available on pypi)...please feel free to help bikeshed names.\n\n# Getting started\n\n## Installation\n\nInstall from `pypi` with `pip install ionics_fits` or add to your poetry project with\n`poetry add fits`.\n\n## Example Usage\n\nBasic usage\n```python\nimport numpy as np\nimport ionics_fits as fits\n\na = 3.2\ny0 = -9\n\nx = np.linspace(-10, 10)\ny = a*x + y0\n\nfit = fits.NormalFitter(x, y, model=fits.models.Line())\nprint(f"Fitted: y = {fit.values[\'a\']:.3f} * x + {fit.values[\'y0\']:.3f}")\n```\n\nThe fit can be configured in various ways by modifying the model\'s `parameters`\ndictionary (see the `fits.common.ModelParameter` class for more information). This\nallows one to:\n- change the bounds for parameters\n- change which parameters are fixed to a constant value / floated\n- supply initial values for parameters instead of relying on the heuristics\n\nExample usage:\n```python\nimport numpy as np\nfrom matplotlib import pyplot as plt\nimport ionics_fits as fits\n\n# Example problem: fit the amplitude and phase of a sinusoid whose frequency is known\n# exactly\n\nomega = 2 * np.pi  # we know the frequency\nmodel = fits.models.Sinusoid()\nmodel.parameters["omega"].fixed_to = omega\n\n# generate synthetic data to fit\nparams = {\n    "a": np.random.uniform(low=1, high=5),\n    "omega": omega,\n    "phi": np.random.uniform(-1, 1) * 2 * np.pi,\n    "y0": 0,\n    "x0": 0,\n    "tau": np.inf,\n}\nx = np.linspace(-3, 3, 100)\ny = model.func(x, params)\n\nfit = fits.NormalFitter(x, y, model=model)\nprint(f"Amplitude: dataset = {params[\'a\']:.3f}, fit = {fit.values[\'a\']:.3f}")\nprint(f"Phase: dataset = {params[\'phi\']:.3f}, fit = {fit.values[\'phi\']:.3f}")\n\nplt.plot(x, y, label="data")\nplt.plot(*fit.evaluate(), \'-.o\', label="fit")\nplt.grid()\nplt.legend()\nplt.show()\n```\n\n# Developing\n\nBefore committing:\n- Update formatting: `poe fmt`\n- Lints: `poe flake`\n- Run test suite: `poe test`\n- Optionally: [fuzz](#Fuzzing) any new models\n\n# Design Philosophy\n\n## Good Heuristics\n\nLife is too short for failed fits. We can\'t guarantee to fit every dataset without any\nhelp from the user (e.g. specifying initial parameter values) no matter how noisy or\nincomplete it is...but we do our best!\n\nEvery fit model has a "parameter estimator" which uses heuristics to find good estimates\nof the values of the model\'s free parameters. We expect these heuristics to be good\nenough to allow the optimizer to fit any "reasonable" dataset. Fit failures are viewed\nas a bug and we encourage our users to file issues where they find them (please post an\nexample dataset in the issue).\n\nCurrently this project is a MVP and many of the heuristics need some work. Expect there\nto be cases where we could easily do better. Please report them where you find them!\n\n## Validation\n\nIt\'s not enough to just fit the data, we want to know if we can trust the fit results\nbefore acting on them.  There are two distinct aspects to the validation problem: did\nthe fit find the model parameters which best match the data (as opposed to getting stuck\nin a local minimum in parameter space far from the global optimum)? and, are the fitted\nparameter values consistent with our prior knowledge of the system (e.g. we know that a\nfringe contrast must lie within certain bounds).\n\nFirst, any prior knowledge about the system should be incorporated by specifying fixed\nparameter values and parameter bounds. After that, the fit is validated. At present,\nvalidation is done using the Chi-squared as a test for goodness of fit. It is likely\nthat additional validation tests will be added as the package grows.\n\n## General purpose\n\nThis library is designed to be general purpose; rather than tackling specific problems\nwe try to target sets of problems -- we want to fit sinusoids not *your* sinusoid. This\nis reflected, for example, in the choices of parametrisation, which are intended to be\nextremely flexible, and the effort put into heuristics. If you find you can\'t easily fit\nyour sinusoid with the standard model/heuristics it\'s probably a bug in the model design\nso please open an issue.\n\nWe encourage contributions of new fit models, but please consider generality before\nsubmission. If you want to solve a specific problem in front of you, that\'s fine but\nprobably better suited to your own codebase.\n\n## Extensibility\n\nThe library is designed to be extensible and ergonomic to user. Want to use different\nstatistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some\ncustom post-fit processing? Override the `calculate_derived_parameters` method. Want to\ntweak the parameter estimator for a model? Create a new model class that inherits from\nthe original model and modify away. If you\'re struggling to do what you want, it\'s\nprobably a bug in the library so please report it.\n\n`ionics_fits` provides a number of tools to make it easier to extend models (see, for\nexample in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...\n\n## Rescaling models\n\n...fit some frequency-domain Rabi oscillation data. However, the model works in angular\nunits, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`\ntool.\n\n```python\ndetuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)\n```\n\nOr, suppose you actually want to scan the magnetic field and find the field offset which\nputs the transition at a particular frequency?\n```python\nclass _RabiBField(fits.models.RabiFlopFreq):\n    def __init__(self, dfdB, B_0, f_0, start_excited):\n        super().__init__(start_excited=start_excited)\n        self.dfdB = dfdB\n        self.B_0 = B_0\n        self.f_0 = f_0\n\n    def calculate_derived_params(self, x, y, fitted_params, fit_uncertainties):\n        derived_params, derived_uncertainties = super().calculate_derived_params(\n            x, y, fitted_params, fit_uncertainties\n        )\n\n        df = derived_params["f_0"] - self.f_0\n        dB = df / self.dfdB\n        B_0 = dB + self.B_0\n\n        derived_params["B_0"] = B_0\n        derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB\n\n        return derived_params, derived_uncertainties\n\nRabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)\n```\n\n## Aggregating models\n\n...fit multiple independent models simultaneously and do some post-processing on the\nresults. Use an `AggregateModel`.\n\n```python\nclass LineAndTriange(fits.models.AggregateModel):\n  def __init__(self):\n    line = fits.models.Line()\n    triangle = fits.models.Triangle()\n    super().__init__(models=[("line", line), "triangle", triangle])\n\n  def calculate_derived_params(\n      self,\n      x: Array[("num_samples",), np.float64],\n      y: Array[("num_samples",), np.float64],\n      fitted_params: Dict[str, float],\n      fit_uncertainties: Dict[str, float],\n  ) -> Tuple[Dict[str, float], Dict[str, float]]:\n      derived_params, derived_uncertainties = super().calculate_derived_params()\n      # derive new results from the two fits\n      return derived_params, derived_uncertainties\n```\n\n## And more!\n\nAt present the library is still an MVP. Further work will be driven by use cases, so\nplease open an issue if you find you can\'t easily extend the library in the way you\nwant.\n\n# Ontology\n\nThere are two main kinds of object in the library: `fit`s and `model`s. Models are\ngeneral-purpose functions to be fitted, such as sinusoids or Lorentzians, but are\nagnostic about the statistics. Fits do the fitting (maximum likelihood parameter\nestimation) and validation based on some underlying statistics (normal, binomial, etc). \n\n# Testing methodology\n\nThis package uses both `unit test`s and `fuzzing`.\n\n## Unit Tests\n\n- run using `poe test`\n- to run a subset of tests use the `-k` flag e.g. `poe test -k "rabi"` to run only tests\n  with the word `rabi` in their name. For more information about configuring pytest see\n  the [documentation](https://docs.pytest.org/en/7.1.x/)\n- all tests must pass before a PR can be merged into master\n- PRs to add new models will only be merged once they have reasonable test coverage\n- unit tests aim to provide good coverage over the space of "reasonable datasets". There\n  will always be corner-cases where the fits fail and that\'s fine; the aim here is to\n  cover the main cases users will hit in the wild\n- when a user hits a case in the wild where the fit fails unexpectedly (i.e. we think\n  the fit code should have handled it), a `regression test` based on the failing\n  dataset should be added\n- unit tests should be deterministic. Synthetic datasets should be included in the test\n  rather than randomly generated at run time. Tip: while writing a test it\'s fine to let\n  the test code generate datasets for you. Once you\'re happy, run the test in verbose\n  mode and copy the dataset from the log output\n\n## Fuzzing\n\n- fuzzing is non-deterministic (random parameter values, randomly generated datasets)\n  exploration of the parameter space.\n- used when developing / debugging fits, but not automatically run by CI\n- run with `poe fuzz` (see `--help` for details)\n- fit failures during fuzzing are not automatically considered a bug; unlike unit tests,\n  fuzzing explores the "unreasonable" part of parameter space as well. Indeed, a large\n  part of the point of fuzzing is to help the developer understand what should be\n  considered "reasonable" (this information should end up in the documentation for the\n  fuzzed model).\n',
+    'long_description': 'Lightweight Python library for data fitting with an emphasis on AMO (Atomic Molecular\nand Optical physics) and Quantum Information.\n\n`fits` was inspired by the [Oxford Ion Trap Group fitting library](https://github.com/OxfordIonTrapGroup/oitg/tree/master/oitg/fitting) originally\nauthored by @tballance. It is still in the alpha phase and is likely to be renamed\n(although `fits` is still available on pypi)...please feel free to help bikeshed names.\n\n# Getting started\n\n## Installation\n\nInstall from `pypi` with `pip install ionics_fits` or add to your poetry project with\n`poetry add fits`.\n\n## Example Usage\n\nBasic usage\n```python\nimport numpy as np\nimport ionics_fits as fits\n\na = 3.2\ny0 = -9\n\nx = np.linspace(-10, 10)\ny = a*x + y0\n\nfit = fits.NormalFitter(x, y, model=fits.models.Line())\nprint(f"Fitted: y = {fit.values[\'a\']:.3f} * x + {fit.values[\'y0\']:.3f}")\n```\n\nThe fit can be configured in various ways by modifying the model\'s `parameters`\ndictionary (see the `fits.common.ModelParameter` class for more information). This\nallows one to:\n- change the bounds for parameters\n- change which parameters are fixed to a constant value / floated\n- supply initial values for parameters instead of relying on the heuristics\n\nExample usage:\n```python\nimport numpy as np\nfrom matplotlib import pyplot as plt\nimport ionics_fits as fits\n\n# Example problem: fit the amplitude and phase of a sinusoid whose frequency is known\n# exactly\n\nomega = 2 * np.pi  # we know the frequency\nmodel = fits.models.Sinusoid()\nmodel.parameters["omega"].fixed_to = omega\n\n# generate synthetic data to fit\nparams = {\n    "a": np.random.uniform(low=1, high=5),\n    "omega": omega,\n    "phi": np.random.uniform(-1, 1) * 2 * np.pi,\n    "y0": 0,\n    "x0": 0,\n    "tau": np.inf,\n}\nx = np.linspace(-3, 3, 100)\ny = model.func(x, params)\n\nfit = fits.NormalFitter(x, y, model=model)\nprint(f"Amplitude: dataset = {params[\'a\']:.3f}, fit = {fit.values[\'a\']:.3f}")\nprint(f"Phase: dataset = {params[\'phi\']:.3f}, fit = {fit.values[\'phi\']:.3f}")\n\nplt.plot(x, y, label="data")\nplt.plot(*fit.evaluate(), \'-.o\', label="fit")\nplt.grid()\nplt.legend()\nplt.show()\n```\n\n# Developing\n\nBefore committing:\n- Update formatting: `poe fmt`\n- Lints: `poe flake`\n- Run test suite: `poe test`\n- Optionally: [fuzz](#Fuzzing) any new models\n\n# Design Philosophy\n\n## Good Heuristics\n\nLife is too short for failed fits. We can\'t guarantee to fit every dataset without any\nhelp from the user (e.g. specifying initial parameter values) no matter how noisy or\nincomplete it is...but we do our best!\n\nEvery fit model has a "parameter estimator" which uses heuristics to find good estimates\nof the values of the model\'s free parameters. We expect these heuristics to be good\nenough to allow the optimizer to fit any "reasonable" dataset. Fit failures are viewed\nas a bug and we encourage our users to file issues where they find them (please post an\nexample dataset in the issue).\n\nCurrently this project is a MVP and many of the heuristics need some work. Expect there\nto be cases where we could easily do better. Please report them where you find them!\n\n## Validation\n\nIt\'s not enough to just fit the data, we want to know if we can trust the fit results\nbefore acting on them.  There are two distinct aspects to the validation problem: did\nthe fit find the model parameters which best match the data (as opposed to getting stuck\nin a local minimum in parameter space far from the global optimum)? and, are the fitted\nparameter values consistent with our prior knowledge of the system (e.g. we know that a\nfringe contrast must lie within certain bounds).\n\nFirst, any prior knowledge about the system should be incorporated by specifying fixed\nparameter values and parameter bounds. After that, the fit is validated. At present,\nvalidation is done using the Chi-squared as a test for goodness of fit. It is likely\nthat additional validation tests will be added as the package grows.\n\n## General purpose\n\nThis library is designed to be general purpose; rather than tackling specific problems\nwe try to target sets of problems -- we want to fit sinusoids not *your* sinusoid. This\nis reflected, for example, in the choices of parametrisation, which are intended to be\nextremely flexible, and the effort put into heuristics. If you find you can\'t easily fit\nyour sinusoid with the standard model/heuristics it\'s probably a bug in the model design\nso please open an issue.\n\nWe encourage contributions of new fit models, but please consider generality before\nsubmission. If you want to solve a specific problem in front of you, that\'s fine but\nprobably better suited to your own codebase.\n\n## Extensibility\n\nThe library is designed to be extensible and ergonomic to user. Want to use different\nstatistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some\ncustom post-fit processing? Override the `calculate_derived_parameters` method. Want to\ntweak the parameter estimator for a model? Create a new model class that inherits from\nthe original model and modify away. If you\'re struggling to do what you want, it\'s\nprobably a bug in the library so please report it.\n\n`ionics_fits` provides a number of tools to make it easier to extend models. See, for\nexample [`models.utils`](../master/ionics_fits/models/utils.py) and [`models.containers`](../master/ionics_fits/models/containers.py). Suppose you want to...\n## Rescaling models\n\n...fit some frequency-domain Rabi oscillation data. However, the model works in angular\nunits, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`\ntool.\n\n```python\ndetuning_model = fits.models.utils.rescale_model_x(fits.models.RabiFlopFreq, 2 * np.pi)\n```\n\nOr, suppose you actually want to scan the magnetic field and find the field offset which\nputs the transition at a particular frequency?\n```python\nclass _RabiBField(fits.models.RabiFlopFreq):\n    def __init__(self, dfdB, B_0, f_0, start_excited):\n        super().__init__(start_excited=start_excited)\n        self.dfdB = dfdB\n        self.B_0 = B_0\n        self.f_0 = f_0\n\n    def calculate_derived_params(self, x, y, fitted_params, fit_uncertainties):\n        derived_params, derived_uncertainties = super().calculate_derived_params(\n            x, y, fitted_params, fit_uncertainties\n        )\n\n        df = derived_params["f_0"] - self.f_0\n        dB = df / self.dfdB\n        B_0 = dB + self.B_0\n\n        derived_params["B_0"] = B_0\n        derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB\n\n        return derived_params, derived_uncertainties\n\nRabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)\n```\n\n## Containers\n\n...fit multiple independent models simultaneously and do some post-processing on the\nresults. Use an `AggregateModel`.\n\n```python\nclass LineAndTriange(fits.models.AggregateModel):\n  def __init__(self):\n    line = fits.models.Line()\n    triangle = fits.models.Triangle()\n    super().__init__(models=[("line", line), "triangle", triangle])\n\n  def calculate_derived_params(\n      self,\n      x: Array[("num_samples",), np.float64],\n      y: Array[("num_samples",), np.float64],\n      fitted_params: Dict[str, float],\n      fit_uncertainties: Dict[str, float],\n  ) -> Tuple[Dict[str, float], Dict[str, float]]:\n      derived_params, derived_uncertainties = super().calculate_derived_params()\n      # derive new results from the two fits\n      return derived_params, derived_uncertainties\n```\n\n...use the single-qubit Rabi flop model to fit simultaneous Rabi flopping on multiple\nqubits at once with some parameters shared and some independent.\n\n```python\nclass MultiRabiFreq(fits.models.RepeatedModel):\n    def __init__(self, n_qubits):\n        super().__init__(\n            inner=fits.models.RabiFlopFreq(start_excited=True),\n            common_params=[\n                "P_readout_e",\n                "P_readout_g",\n                "t_pulse",\n                "omega",\n                "tau",\n                "t_dead",\n            ],\n            num_repetitions=n_qubits,\n        )\n\n```\n## And more!\n\nAt present the library is still an MVP. Further work will be driven by use cases, so\nplease open an issue if you find you can\'t easily extend the library in the way you\nwant.\n\n# Ontology\n\nThere are two main kinds of object in the library: `fit`s and `model`s. Models are\ngeneral-purpose functions to be fitted, such as sinusoids or Lorentzians, but are\nagnostic about the statistics. Fits do the fitting (maximum likelihood parameter\nestimation) and validation based on some underlying statistics (normal, binomial, etc). \n\n# Testing methodology\n\nThis package uses both `unit test`s and `fuzzing`.\n\n## Unit Tests\n\n- run using `poe test`\n- to run a subset of tests use the `-k` flag e.g. `poe test -k "rabi"` to run only tests\n  with the word `rabi` in their name. For more information about configuring pytest see\n  the [documentation](https://docs.pytest.org/en/7.1.x/)\n- all tests must pass before a PR can be merged into master\n- PRs to add new models will only be merged once they have reasonable test coverage\n- unit tests aim to provide good coverage over the space of "reasonable datasets". There\n  will always be corner-cases where the fits fail and that\'s fine; the aim here is to\n  cover the main cases users will hit in the wild\n- when a user hits a case in the wild where the fit fails unexpectedly (i.e. we think\n  the fit code should have handled it), a `regression test` based on the failing\n  dataset should be added\n- unit tests should be deterministic. Synthetic datasets should be included in the test\n  rather than randomly generated at run time. Tip: while writing a test it\'s fine to let\n  the test code generate datasets for you. Once you\'re happy, run the test in verbose\n  mode and copy the dataset from the log output\n\n## Fuzzing\n\n- fuzzing is non-deterministic (random parameter values, randomly generated datasets)\n  exploration of the parameter space.\n- used when developing / debugging fits, but not automatically run by CI\n- run with `poe fuzz` (see `--help` for details)\n- fit failures during fuzzing are not automatically considered a bug; unlike unit tests,\n  fuzzing explores the "unreasonable" part of parameter space as well. Indeed, a large\n  part of the point of fuzzing is to help the developer understand what should be\n  considered "reasonable" (this information should end up in the documentation for the\n  fuzzed model).\n',
     'author': 'hartytp',
     'author_email': 'thomas.peter.harty@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ionics_fits-1.0.4/PKG-INFO` & `ionics_fits-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionics-fits
-Version: 1.0.4
+Version: 1.0.5
 Summary: Lightweight Python data fitting library with an emphasis on AMO/Quantum Information
 Author: hartytp
 Author-email: thomas.peter.harty@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -147,17 +147,16 @@
 The library is designed to be extensible and ergonomic to user. Want to use different
 statistics? Easy, just provide a new class that inherits from `FitBase`. Want to do some
 custom post-fit processing? Override the `calculate_derived_parameters` method. Want to
 tweak the parameter estimator for a model? Create a new model class that inherits from
 the original model and modify away. If you're struggling to do what you want, it's
 probably a bug in the library so please report it.
 
-`ionics_fits` provides a number of tools to make it easier to extend models (see, for
-example in [`models.utils`](../master/ionics_fits/models/utils.py)). Say you want to...
-
+`ionics_fits` provides a number of tools to make it easier to extend models. See, for
+example [`models.utils`](../master/ionics_fits/models/utils.py) and [`models.containers`](../master/ionics_fits/models/containers.py). Suppose you want to...
 ## Rescaling models
 
 ...fit some frequency-domain Rabi oscillation data. However, the model works in angular
 units, but your tooling needs linear units. No problem! Simply use the `rescale_model_x`
 tool.
 
 ```python
@@ -187,15 +186,15 @@
         derived_uncertainties["B_0"] = derived_uncertainties["f_0"] * self.dfdB
 
         return derived_params, derived_uncertainties
 
 RabiBField = fits.models.utils.rescale_model_x(_RabiBField, 2 * np.pi * dfdB)
 ```
 
-## Aggregating models
+## Containers
 
 ...fit multiple independent models simultaneously and do some post-processing on the
 results. Use an `AggregateModel`.
 
 ```python
 class LineAndTriange(fits.models.AggregateModel):
   def __init__(self):
@@ -211,14 +210,34 @@
       fit_uncertainties: Dict[str, float],
   ) -> Tuple[Dict[str, float], Dict[str, float]]:
       derived_params, derived_uncertainties = super().calculate_derived_params()
       # derive new results from the two fits
       return derived_params, derived_uncertainties
 ```
 
+...use the single-qubit Rabi flop model to fit simultaneous Rabi flopping on multiple
+qubits at once with some parameters shared and some independent.
+
+```python
+class MultiRabiFreq(fits.models.RepeatedModel):
+    def __init__(self, n_qubits):
+        super().__init__(
+            inner=fits.models.RabiFlopFreq(start_excited=True),
+            common_params=[
+                "P_readout_e",
+                "P_readout_g",
+                "t_pulse",
+                "omega",
+                "tau",
+                "t_dead",
+            ],
+            num_repetitions=n_qubits,
+        )
+
+```
 ## And more!
 
 At present the library is still an MVP. Further work will be driven by use cases, so
 please open an issue if you find you can't easily extend the library in the way you
 want.
 
 # Ontology
```

