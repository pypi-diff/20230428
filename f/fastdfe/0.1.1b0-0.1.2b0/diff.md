# Comparing `tmp/fastdfe-0.1.1b0.tar.gz` & `tmp/fastdfe-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.1b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.2b0.tar", max compression
```

## Comparing `fastdfe-0.1.1b0.tar` & `fastdfe-0.1.2b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      316 2023-04-24 05:28:36.304713 fastdfe-0.1.1b0/README.md
--rw-r--r--   0        0        0     2596 2023-04-27 17:41:55.145889 fastdfe-0.1.1b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    15352 2023-04-27 17:41:55.136933 fastdfe-0.1.1b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    39982 2023-04-27 17:46:23.094730 fastdfe-0.1.1b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4749 2023-04-25 17:46:33.252414 fastdfe-0.1.1b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0     9521 2023-04-25 17:04:08.653778 fastdfe-0.1.1b0/fastdfe/config.py
--rw-r--r--   0        0        0    14889 2023-04-26 07:24:19.626163 fastdfe-0.1.1b0/fastdfe/discretization.py
--rw-r--r--   0        0        0     3937 2023-04-25 17:46:33.230441 fastdfe-0.1.1b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     1381 2023-04-25 17:46:33.199691 fastdfe-0.1.1b0/fastdfe/mle.py
--rw-r--r--   0        0        0    23624 2023-04-26 07:24:19.643890 fastdfe-0.1.1b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    19959 2023-04-26 07:56:42.720331 fastdfe-0.1.1b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    10734 2023-04-25 17:04:08.646723 fastdfe-0.1.1b0/fastdfe/parser.py
--rw-r--r--   0        0        0    17003 2023-04-25 17:53:02.835980 fastdfe-0.1.1b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0    35424 2023-04-27 17:41:55.093286 fastdfe-0.1.1b0/fastdfe/shared_inference.py
--rw-r--r--   0        0        0    17572 2023-04-25 17:46:33.213791 fastdfe-0.1.1b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0    28388 2023-04-26 06:29:03.499964 fastdfe-0.1.1b0/fastdfe/visualization.py
--rw-r--r--   0        0        0      642 2023-04-28 08:02:22.437093 fastdfe-0.1.1b0/pyproject.toml
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 fastdfe-0.1.1b0/PKG-INFO
+-rw-r--r--   0        0        0      316 2023-04-24 05:28:36.304713 fastdfe-0.1.2b0/README.md
+-rw-r--r--   0        0        0     2649 2023-04-28 15:00:53.726538 fastdfe-0.1.2b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    15675 2023-04-28 15:54:32.817541 fastdfe-0.1.2b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    40231 2023-04-28 16:01:50.252285 fastdfe-0.1.2b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4749 2023-04-25 17:46:33.252414 fastdfe-0.1.2b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0     9520 2023-04-28 15:00:53.695766 fastdfe-0.1.2b0/fastdfe/config.py
+-rw-r--r--   0        0        0    14889 2023-04-26 07:24:19.626163 fastdfe-0.1.2b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0     3937 2023-04-25 17:46:33.230441 fastdfe-0.1.2b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     1381 2023-04-25 17:46:33.199691 fastdfe-0.1.2b0/fastdfe/mle.py
+-rw-r--r--   0        0        0    23671 2023-04-28 15:00:53.721080 fastdfe-0.1.2b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    21128 2023-04-28 15:13:39.927333 fastdfe-0.1.2b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    10986 2023-04-28 15:06:24.181963 fastdfe-0.1.2b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    17094 2023-04-28 15:54:32.832520 fastdfe-0.1.2b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0    35860 2023-04-28 16:01:50.239910 fastdfe-0.1.2b0/fastdfe/shared_inference.py
+-rw-r--r--   0        0        0    17957 2023-04-28 16:01:50.245576 fastdfe-0.1.2b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0    31116 2023-04-28 16:01:50.255162 fastdfe-0.1.2b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0      642 2023-04-28 16:09:12.911964 fastdfe-0.1.2b0/pyproject.toml
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 fastdfe-0.1.2b0/PKG-INFO
```

### Comparing `fastdfe-0.1.1b0/fastdfe/__init__.py` & `fastdfe-0.1.2b0/fastdfe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 # configure logger
 logger = logging.getLogger('fastdfe')
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(logging.Formatter('%(levelname)s:%(name)s:%(message)s'))
 logger.addHandler(handler)
 logger.setLevel(logging.INFO)
 
+# whether to show progress bar
+disable_pbar = False
+
 
 def raise_on_warning(message, category, filename, lineno, file=None, line=None):
     """
     Raise exception on warning.
     """
     raise Exception(warnings.formatwarning(message, category, filename, lineno, line))
```

### Comparing `fastdfe-0.1.1b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.2b0/fastdfe/abstract_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,33 @@
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'discretized DFEs',
             labels: list | np.ndarray = None,
+            ax: plt.Axes = None,
             **kwargs
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize several discretized DFEs given by the list of inference objects.
 
         :param inferences: List of inference objects.
         :param intervals: Intervals to use for discretization.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
         :param kwargs: Additional arguments for the plot.
-        :return: Axis of the plot.
+        :param ax: Axes of the plot.
+        :return: Axes of the plot.
         """
         # get data from inference objects
         values = []
         errors = []
         for i, inference in enumerate(inferences):
             val, errs = inference.get_discretized(
                 intervals=intervals,
@@ -65,15 +67,16 @@
         return Visualization.plot_discretized(
             values=values,
             errors=errors,
             labels=labels,
             file=file,
             show=show,
             intervals=intervals,
-            title=title
+            title=title,
+            ax=ax
         )
 
     @staticmethod
     def plot_continuous(
             inferences: List['AbstractInference'],
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
@@ -81,17 +84,18 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFEs',
             labels: list | np.ndarray = None,
             scale: Literal['lin', 'log'] = 'lin',
             scale_density: bool = False,
+            ax: plt.Axes = None,
             **kwargs
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize several DFEs given by the list of inference objects.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
         disadvantage that the density now changes for x, so that even a constant
@@ -104,16 +108,17 @@
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
         :param scale: y-scale of the plot.
         :param scale_density: Whether to scale the density by the x-axis interval size.
+        :param ax: Axes of the plot.
         :param kwargs: Additional arguments for the plot.
-        :return: Axis of the plot.
+        :return: Axes of the plot.
         """
         # get data from inference objects
         values = []
         errors = []
         for i, inference in enumerate(inferences):
             val, errs = inference.get_discretized(
                 intervals=intervals,
@@ -139,33 +144,35 @@
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             file: str = None,
             show: bool = True,
             title: str = 'parameter estimates',
             labels: list | np.ndarray = None,
             scale: Literal['lin', 'log'] = 'log',
             legend: bool = True,
+            ax: plt.Axes = None,
             **kwargs
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize several discretized DFEs given by the list of inference objects.
         Note that the DFE parametrization needs to be the same for all inference objects.
 
         :param scale: y-scale of the plot.
         :param legend: Whether to show a legend.
         :param inferences: List of inference objects.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param ci_level: Confidence level for confidence intervals.
         :param bootstrap_type: Type of bootstrap to use for confidence intervals.
         :param file: Path to file to save the plot to.
         :param show: Whether to show the plot.
         :param title: Title of the plot.
         :param labels: Labels for the DFEs.
+        :param ax: Axes of the plot.
         :param kwargs: Additional arguments for the plot.
-        :return: Axis of the plot.
+        :return: Axes of the plot.
         """
         return Visualization.plot_inferred_parameters(
             params=[inf.get_bootstrap_params() for inf in inferences],
             bootstraps=[inf.bootstraps for inf in inferences],
             **locals()
         )
 
@@ -173,15 +180,15 @@
     def get_discretized(
             bootstraps: pd.DataFrame,
             params: dict,
             model: Parametrization,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
-            bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
+            bootstrap_type: Literal['percentile', 'bca'] = 'percentile'
 
     ) -> (np.ndarray, np.ndarray):
         """
         Get discretized DFE.
 
         :param bootstraps: Bootstrap samples
         :param params: Parameters of the model
@@ -353,42 +360,45 @@
             ci_level=ci_level,
             bootstrap_type=bootstrap_type
         )
 
     def plot_discretized(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
-            title: str = 'discretized DFE'
-    ) -> plt.axis:
+            title: str = 'discretized DFE',
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Plot discretized DFE.
 
         :param title: Title of the plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence interval level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save the plot to
         :param show: Whether to show the plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
-        :return: Axis
+        :param ax: Axes to plot to
+        :return: Axes
         """
         return Inference.plot_discretized(
             inferences=[self],
             file=file,
             show=show,
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
-            title=title
+            title=title,
+            ax=ax
         )
 
     def to_json(self) -> str:
         """
         Serialize object.
 
         :return: JSON string
```

### Comparing `fastdfe-0.1.1b0/fastdfe/base_inference.py` & `fastdfe-0.1.2b0/fastdfe/base_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import logging
 import time
 from typing import List, Optional, Dict, Literal, cast
 
 import multiprocess as mp
 import numpy as np
 import pandas as pd
-import seaborn as sns
 from matplotlib import pyplot as plt
 from numpy.linalg import norm
 from scipy.optimize._optimize import OptimizeResult
 from scipy.stats import chi2
 from typing_extensions import Self
 
 from . import parametrization, optimization
@@ -627,23 +626,25 @@
         # adjust for demography and polarization error
         return r * counts_sel_adjusted
 
     @run_if_required_wrapper
     def plot_continuous(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             intervals: np.ndarray = None,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             scale_density: bool = False,
             scale: Literal['lin', 'log'] = 'lin',
-            title: str = 'DFE'
-    ) -> plt.axis:
+            title: str = 'DFE',
+            ax: plt.Axes = None
+
+    ) -> plt.Axes:
         """
         Plot continuous DFE.
         The special constants np.inf and -np.inf are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
@@ -655,128 +656,117 @@
         :param ci_level: Confidence level for confidence intervals.
         :param confidence_intervals: Whether to plot confidence intervals.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param scale: y-scale
         :param scale_density: Whether to scale the density by the x-axis interval size
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         if intervals is None:
             intervals = self.discretization.bins
 
         return Inference.plot_continuous(
             inferences=[self],
             file=file,
             show=show,
             intervals=intervals,
             confidence_intervals=confidence_intervals,
             ci_level=ci_level,
             bootstrap_type=bootstrap_type,
             title=title,
             scale=scale,
-            scale_density=scale_density
+            scale_density=scale_density,
+            ax=ax
         )
 
     @run_if_required_wrapper
     def plot_bucket_sizes(
             self,
             file: str = None,
             show: bool = True,
-            title: str = 'bucket sizes'
+            title: str = 'bucket sizes',
+            ax: plt.Axes = None
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot mass in each bucket for the MLE DFE.
         This can be used to check if the interval bounds and spacing
         are chosen appropriately.
 
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param title: Plot title.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         # evaluate at fixed parameters
         sizes = self.model.discretize(self.params_mle, self.discretization.bins)
 
-        Visualization.plot_buckets_sizes(
+        return Visualization.plot_buckets_sizes(
             n_intervals=self.discretization.n_intervals,
             bins=self.discretization.bins,
             sizes=sizes,
             title=title,
             file=file,
-            show=show
+            show=show,
+            ax=ax
         )
 
     @run_if_required_wrapper
-    @Visualization.clear_show_save
     def plot_interval_density(
             self,
             file: str = None,
             show: bool = True,
             intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             interval_labels: List[str] = None,
-            color: str = 'C0'
+            color: str = 'C0',
+            ax: plt.Axes = None
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
-        Plot density of the discretization intervals chosen.
+        Plot density of the discretization intervals chosen. Note that although this plot looks similar, this is
+        not the DFE!
 
         :param color: Color of the bars.
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param interval_labels: Labels for the intervals.
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         # issue warning
         if not self.discretization.linearized:
             logger.warning('Note that the interval density is not important if the DFE was not linearized.')
 
-        # number of intervals
-        n_intervals = len(intervals)
-
-        # plot interval density
-        y = self.discretization.get_interval_density(intervals)
-        x = np.arange(n_intervals - 1)
-        ax = sns.barplot(x=x, y=y / y.sum(), color=color)
-        ax.set(xlabel='S', ylabel='fraction')
-
-        # determine x-labels
-        if interval_labels is None:
-            xlabels = [Visualization.interval_to_string(intervals[i - 1], intervals[i]) for i in range(1, n_intervals)]
-        else:
-            xlabels = interval_labels
-
-        # adjust x-ticks
-        ax.set_xticks(x)
-        ax.set_xticklabels(xlabels)
-
-        # set title
-        ax.set_title('interval density')
-
-        # remove x-margins
-        ax.autoscale(tight=True, axis='x')
+        return Visualization.plot_interval_density(
+            density=self.discretization.get_interval_density(intervals),
+            **locals()
+        )
 
     def plot_sfs_comparison(
             self,
             types: List[Literal['modelled', 'observed', 'modelled', 'neutral']] = ['modelled', 'observed'],
             labels: List[str] = None,
             file: str = None,
-            show=True
+            show: bool = True,
+            ax: plt.Axes = None
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
         :param types: Types of SFS to plot.
         :param show: Whether to show plot.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         if 'modelled' in types:
             self.run_if_required()
 
         mapping = dict(
             observed=self.sfs_sel,
             selected=self.sfs_sel,
@@ -784,33 +774,42 @@
             neutral=self.sfs_neut
         )
 
         return Visualization.plot_sfs_comparison(
             spectra=[mapping[t] for t in types],
             labels=types if labels is None else labels,
             file=file,
-            show=show
+            show=show,
+            ax=ax
         )
 
-    def plot_input_sfs(
+    def plot_observed_sfs(
             self,
             labels: List[str] = None,
             file: str = None,
-            show=True
+            show: bool = True,
+            ax: plt.Axes = None
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
-        Plot SFS comparison.
+        Plot neutral and selected SFS.
 
         :param file: File to save plot to.
         :param labels: Labels for the SFS.
         :param show: Whether to show plot.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
-        return self.plot_sfs_comparison(['neutral', 'selected'], labels=labels, file=file, show=show)
+        return self.plot_sfs_comparison(
+            types=['neutral', 'selected'],
+            labels=labels,
+            file=file,
+            show=show,
+            ax=ax
+        )
 
     @run_if_required_wrapper
     def plot_all(self, show: bool = True):
         """
         Plot everything.
         """
         self.plot_inferred_parameters(show=show)
@@ -823,67 +822,73 @@
     @run_if_required_wrapper
     def plot_inferred_parameters(
             self,
             file: str = None,
             confidence_intervals: bool = True,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
-            show=True,
+            show: bool = True,
             title: str = 'inferred parameters',
             scale: Literal['lin', 'log'] = 'log',
+            ax: plt.Axes = None,
             **kwargs
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param confidence_intervals: Whether to show confidence intervals.
         :param bootstrap_type: Type of bootstrap to use.
         :param ci_level: Confidence level for the confidence intervals.
         :param file: File to save plot to.
         :param show: Whether to show plot.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         return Visualization.plot_inferred_parameters(
             params=[self.get_bootstrap_params()],
             bootstraps=[self.bootstraps],
             file=file,
             show=show,
             title=title,
             ci_level=ci_level,
             confidence_intervals=confidence_intervals,
             bootstrap_type=bootstrap_type,
-            scale=scale
+            scale=scale,
+            ax=ax
         )
 
     @run_if_required_wrapper
     def plot_likelihoods(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             title: str = 'likelihoods',
             scale: Literal['lin', 'log'] = 'lin',
+            ax: plt.Axes = None,
             **kwargs
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize the likelihoods of the optimization runs.
 
         :param scale: y-scale of the plot.
         :param title: Plot title.
         :param file: File to save plot to.
         :param show: Whether to show plot.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         return Visualization.plot_likelihoods(
             likelihoods=self.optimization.likelihoods,
             file=file,
             show=show,
             title=title,
-            scale=scale
+            scale=scale,
+            ax=ax
         )
 
     @staticmethod
     def lrt(ll_simple: float, ll_complex: float, df: int = 1) -> float:
         """
         Perform the likelihood ratio test (LRT).
 
@@ -977,35 +982,36 @@
         P = np.reshape(
             [cast(BaseInference, i[0][1]).compare_nested_likelihoods(cast(BaseInference, i[1][1])) for i in inputs],
             (n, n)
         )
 
         return P, inferences
 
-    @Visualization.clear_show_save
     def plot_nested_likelihoods(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             remove_empty: bool = False,
             transpose: bool = False,
             cmap: str = None,
-            title: str = 'nested model comparison'
+            title: str = 'nested model comparison',
+            ax: plt.Axes = None,
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot the p-values of nested likelihoods.
 
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param remove_empty: Whether to remove empty rows and columns.
         :param transpose: Whether to transpose the matrix.
         :param cmap: Colormap to use.
         :param title: Plot title.
-        :return: Axis object
+        :param ax: Axes object to plot on.
+        :return: Axes object
         """
         # get p-values and names
         P, inferences = self.compare_nested_models()
 
         # define labels
         labels_x = np.array(list(inferences.keys()))
         labels_y = np.array(list(inferences.keys()))
@@ -1029,15 +1035,16 @@
         return Visualization.plot_nested_likelihoods(
             P=P,
             labels_x=labels_x,
             labels_y=labels_y,
             file=file,
             show=show,
             cmap=cmap,
-            title=title
+            title=title,
+            ax=ax
         )
 
     def get_alpha(self, params: dict = None) -> float:
         """
         Get alpha, the proportion of beneficial non-synonymous substitutions.
 
         :param params: Parameters to use for calculation.
```

### Comparing `fastdfe-0.1.1b0/fastdfe/bootstrap.py` & `fastdfe-0.1.2b0/fastdfe/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.1b0/fastdfe/config.py` & `fastdfe-0.1.2b0/fastdfe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .optimization import SharedParams, merge_dicts
 from .parametrization import Parametrization, from_string, to_string
 from .polydfe import parse_init_file, models, create_sfs_config, create_init_file
 from .spectrum import Spectra, parse_polydfe_sfs_config
 
 logger = logging.getLogger('fastdfe')
 
-
 class Config:
     """
     Configuration class to be used for Inference and polyDFE.
     """
 
     def __init__(
             self,
```

### Comparing `fastdfe-0.1.1b0/fastdfe/discretization.py` & `fastdfe-0.1.2b0/fastdfe/discretization.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.1b0/fastdfe/json_handlers.py` & `fastdfe-0.1.2b0/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.1b0/fastdfe/mle.py` & `fastdfe-0.1.2b0/fastdfe/mle.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.1b0/fastdfe/optimization.py` & `fastdfe-0.1.2b0/fastdfe/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import multiprocess as mp
 import numpy as np
 from numpy.linalg import norm
 from scipy.optimize import minimize, OptimizeResult
 from scipy.stats import loguniform, uniform
 from tqdm import tqdm
 
-from fastdfe.mle import MLE
+from .mle import MLE
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 def parallelize(
         func: Callable,
@@ -28,26 +28,28 @@
 
     :param pbar: Whether to show a progress bar
     :param parallelize: Whether to parallelize
     :param data: Data to iterate over
     :param func: Function to apply to each element of data
     :return: List of results
     """
+    from . import disable_pbar
+
     n = len(data)
 
     if parallelize and n > 1:
         # parallelize
         iterator = mp.Pool().imap(func, data)
     else:
         # sequentialize
         iterator = map(func, data)
 
     # whether to show a progress bar
     if pbar is True or (pbar is None and not parallelize and n > 1) or pbar is None and n > mp.cpu_count():
-        iterator = tqdm(iterator, total=n)
+        iterator = tqdm(iterator, total=n, disable=disable_pbar)
 
     return np.array(list(iterator), dtype=object)
 
 
 def flatten_dict(d: dict, separator='.', prefix=''):
     """
     Flatten dictionary.
```

### Comparing `fastdfe-0.1.1b0/fastdfe/parametrization.py` & `fastdfe-0.1.2b0/fastdfe/parametrization.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,17 @@
         return model.__class__.__name__
 
     return model
 
 
 class Parametrization:
     """
-    A DFE parametrized by a set of parameters which are determined
-    using MLE.
+    Base class for parametrizing a DFE by a set of parameters.
+    Note that :func:`get_pdf` is not required to be implemented, provided that the
+    linearized mode of fastDFE is used (which is highly recommended).
     """
     #: Default initial parameters
     x0 = {}
 
     #: Default parameter bounds
     bounds = {}
 
@@ -153,21 +154,24 @@
     .. math::
         \phi(S; S_d, b, p_b, S_b) = (1 - p_b) f_\Gamma(-S; S_d, b) \cdot \mathbf{1}_{\{S < 0\}} +
         p_b f_e(S; S_b) \cdot \mathbf{1}_{\{S \geq 0\}}
 
     where:
 
     * :math:`S_d` is the mean of the DFE for :math:`S < 0`
-    * :math:`b` is the shape of the Gamma distribution
+    * :math:`b` is the shape of the gamma distribution
     * :math:`p_b` is the probability that :math:`S \geq 0`
     * :math:`S_b` is the mean of the DFE for :math:`S \geq 0`
-    * :math:`f_\Gamma(x; m, b)` is the density of the Gamma distribution with mean :math:`m` and shape :math:`b`
+    * :math:`f_\Gamma(x; m, b)` is the density of the gamma distribution with mean :math:`m` and shape :math:`b`
     * :math:`f_e(x; m)` is the density of the Exponential distribution with mean :math:`m`
     * :math:`\mathbf{1}_{\{A\}}` denotes the indicator function, which is 1 if :math:`A` is true, and 0 otherwise.
 
+    The DFE has often been observed to be multi-modal for negative selection coefficients. A gamma distribution
+    provides a good amount of flexibility to accommodate this.
+
     """
 
     #: Default initial parameters
     x0 = dict(
         S_d=-1000,
         b=0.4,
         p_b=0.05,
@@ -290,19 +294,23 @@
 
     .. math::
         \phi(S; \hat{S}, b, S_{max}) = f_\Gamma(S_{max} - S; S_{max} - \hat{S}, b) \cdot \mathbf{1}_{\{S \leq S_{max}\}}
 
     where:
 
     * :math:`\hat{S}` is the mean of the DFE
-    * :math:`b` is the shape of the Gamma distribution
+    * :math:`b` is the shape of the gamma distribution
     * :math:`S_{max}` is the maximum value that :math:`S` can take
-    * :math:`f_\Gamma(x; m, b)` is the density of the Gamma distribution with mean :math:`m` and shape :math:`b`
+    * :math:`f_\Gamma(x; m, b)` is the density of the gamma distribution with mean :math:`m` and shape :math:`b`
     * :math:`\mathbf{1}_{\{A\}}` denotes the indicator function, which is 1 if :math:`A` is true, and 0 otherwise.
 
+    This parametrization uses a single gamma distribution for both positive and negative selection coefficients.
+    This is a less flexible parametrization, which may produce results similar to the other models while requiring
+    fewer parameters.
+
     """
 
     #: Default initial parameters
     x0 = dict(
         S_mean=-100,
         b=1,
         S_max=1
@@ -387,19 +395,21 @@
     .. math::
         \phi(S; S_d, b, p_b, S_b) = (1 - p_b) f_{\Gamma}(S; S_d, b) \cdot \mathbf{1}_{\{S < 0\}} +
         p_b \cdot S_b \cdot \mathbf{1}_{\{0 \leq S \leq 1 / S_b\}}
 
     where:
 
     * :math:`S_d` is the mean of the DFE for :math:`S < 0`
-    * :math:`b` is the shape of the Gamma distribution
+    * :math:`b` is the shape of the gamma distribution
     * :math:`p_b` is the probability that :math:`S \geq 0`
     * :math:`S_b` is the shared selection coefficient of all positively selected mutations up to :math:`1/S_b`
-    * :math:`f_\Gamma(x; m, b)` is the density of the Gamma distribution with mean :math:`m` and shape :math:`b`
+    * :math:`f_\Gamma(x; m, b)` is the density of the gamma distribution with mean :math:`m` and shape :math:`b`
 
+    This parametrization is similar to :class:`GammaExpParametrization`, but uses a constant mass for positive
+    selection coefficients. The results should be rather similar in most cases.
     """
 
     #: Default initial parameters
     x0 = dict(
         S_d=-1000,
         b=0.4,
         p_b=0.05,
@@ -424,15 +434,15 @@
 
     @staticmethod
     def get_pdf(S_d: float, b: float, p_b: float, S_b: float, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
         """
         Get PDF.
 
         :param S_d: Mean of the DFE for S >= 0
-        :param b: Shape of the Gamma distribution
+        :param b: Shape of the gamma distribution
         :param p_b: Probability that S > 0
         :param S_b: Shared selection coefficient of all positively selected mutations up to S_b
         :return: Function that accepts an array of selection coefficients and returns their probability density
         """
 
         @Parametrization.accepts_scalars
         def pdf(S: np.ndarray) -> np.ndarray:
@@ -458,15 +468,15 @@
 
     @staticmethod
     def get_cdf(S_d: float, b: float, p_b: float, S_b: float, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
         """
         Get CDF.
 
         :param S_d: Mean of the DFE for S >= 0
-        :param b: Shape of the Gamma distribution
+        :param b: Shape of the gamma distribution
         :param p_b: Probability that S > 0
         :param S_b: Shared selection coefficient of all positively selected mutations up to S_b
         :return: Function that accepts an array of selection coefficients and returns their cumulative probability
         """
 
         @Parametrization.accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
@@ -500,14 +510,19 @@
 
     That is, the probability density function is given by:
 
     :math:`\phi(S; S_1, S_2, \dots, S_k) = \sum_{i=1}^{k} S_i/c_i \cdot \mathbf{1}_{\{S \in B_i\}}`
     such that :math:`\sum_{i=1}^{k} S_i = 1,`
 
     where :math:`B_i` and :math:`c_i` are interval :math:`i` and the width of interval :math:`i`, respectively.
+
+    This parametrization has the advantage of not imposing a shape on the DFE. For a reasonably fine parametrization,
+    the number of parameters is larger than those of the other models, however. We generally also observe larger
+    confidence intervals for this parametrization, and the optimization procedure may well be less efficient as
+    we have to renormalize the parameters to make sure they sum up to 1.
     """
 
     def __init__(
             self,
             intervals: np.ndarray = np.array([-100000, -100, -10, -1, 0, 1, 1000])
     ):
         """
```

### Comparing `fastdfe-0.1.1b0/fastdfe/parser.py` & `fastdfe-0.1.2b0/fastdfe/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Callable, Literal, Optional
 
 import numpy as np
 from cyvcf2 import VCF, Variant
 from pyfaidx import Fasta
 from tqdm import tqdm
 
-from fastdfe import Spectra
+from .spectrum import Spectra
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class NoTypeException(BaseException):
     """
@@ -32,15 +32,15 @@
     a site's type based on its properties.
     """
 
     @abstractmethod
     def get_type(self, variant: Variant) -> Optional[str]:
         """
         Get type of given Variant. Only the types
-        given by :meth:`get_types()` are valid, or ``None` if
+        given by :meth:`get_types()` are valid, or ``None`` if
         no type could be determined.
 
         :param variant: The vcf site
         :return: Type of the variant
         """
         pass
 
@@ -264,20 +264,23 @@
     def open_file(file: str):
         if file.endswith('.gz'):
             return gzip.open(file, "rt")
 
         return open(file, 'r')
 
     def count_lines_vcf(self):
+        from . import disable_pbar
+
         i = 0
 
         logger.info('Counting number of sites.')
 
         with self.open_file(self.vcf_file) as f:
-            with tqdm() as pbar:
+
+            with tqdm(disable=disable_pbar) as pbar:
                 for line in f:
                     if not line.startswith('#'):
                         i += 1
                         pbar.update()
 
                     # stop counting if max_sites was reached
                     if i >= self.max_sites:
@@ -299,28 +302,34 @@
         sfs = {}
         for context in contexts:
             sfs[context] = np.zeros(self.n + 1)
 
         return sfs
 
     def parse(self) -> Spectra:
+        """
+        Parse the VCF file and return the SFS.
+        :return: the spectra for the different stratifications
+        """
+
+        from . import disable_pbar
 
         sfs = self.create_sfs_dictionary()
 
         representation = '.'.join(['[' + ','.join(s.get_types()) + ']' for s in self.stratifications])
         logger.info(f'Using stratification: {representation}.')
 
         n_sites = self.count_lines_vcf()
 
         # parse VCF file
         vcf = VCF(self.vcf_file)
 
         logger.info(f'Starting to parse.')
 
-        with tqdm(total=n_sites) as pbar:
+        with tqdm(total=n_sites, disable=disable_pbar) as pbar:
             for i, variant in enumerate(vcf):
 
                 # stop if max_sites was reached
                 if i >= self.max_sites:
                     break
 
                 # just update beforehand
```

### Comparing `fastdfe-0.1.1b0/fastdfe/polydfe.py` & `fastdfe-0.1.2b0/fastdfe/polydfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,33 +506,36 @@
         """
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
 
     def plot_inferred_parameters(
             self,
             file: str = None,
-            show=True,
-            scale: Literal['lin', 'log'] = 'log'
-    ) -> plt.axis:
+            show: bool = True,
+            scale: Literal['lin', 'log'] = 'log',
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
 
         :param scale: Scale of the y-axis
         :param file: File to save the plot to
         :param show: Show the plot
-        :return: Axis object
+        :param ax: Axes object
+        :return: Axes object
         """
         param_names = self.get_bootstrap_param_names()
 
         return Visualization.plot_inferred_parameters(
             params=[self.get_bootstrap_params()],
             bootstraps=[self.bootstraps[param_names]] if self.bootstraps is not None else [None],
             scale=scale,
             file=file,
-            show=show
+            show=show,
+            ax=ax
         )
 
     def get_bootstrap_param_names(self) -> List[str]:
         """
         Parameter names for parameters included in bootstraps.
 
         :return: List of parameter names
```

### Comparing `fastdfe-0.1.1b0/fastdfe/shared_inference.py` & `fastdfe-0.1.2b0/fastdfe/shared_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -727,61 +727,65 @@
 
         return inferences
 
     @BaseInference.run_if_required_wrapper
     def plot_discretized(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
             intervals_ben: (float, float, int) = (1.0e-5, 1.0e4, 1000),
             title: str = 'discretized DFE comparison',
-            labels: List[str] = None
-    ) -> plt.axis:
+            labels: List[str] = None,
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Plot discretized DFE comparing the different types.
 
         :param labels: Labels for types
         :param title: Title of plot
         :param intervals_ben: Interval boundaries for beneficial DFE
         :param intervals_del: Interval boundaries for deleterious DFE
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
-        :return: Axis object
+        :param ax: Axes object
+        :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_discretized(**locals())
 
     def plot_sfs_comparison(
             self,
             sfs_types: List[Literal['modelled', 'observed', 'modelled', 'neutral']] = ['modelled', 'observed'],
             types: List[str] = None,
             labels: List[str] = None,
             file: str = None,
-            show=True
+            show: bool = True,
+            ax: plt.Axes = None
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param types: Types to plot
         :param file: File to save plot to
         :param labels: Labels for types
         :param sfs_types: Types of SFS to plot
         :param show: Whether to show plot
-        :return: Axis object
+        :param ax: Axes object
+        :return: Axes object
         """
         from fastdfe import Visualization
 
         if 'modelled' in sfs_types:
             self.run_if_required()
 
         mapping = dict(
@@ -809,31 +813,33 @@
         # get spectra
         spectra = {get_label(t, sfs): getattr(inf, mapping[sfs]) for t, inf in inferences for sfs in sfs_types}
 
         return Visualization.plot_sfs_comparison(
             spectra=list(spectra.values()),
             labels=list(spectra.keys()) if labels is None else labels,
             file=file,
-            show=show
+            show=show,
+            ax=ax
         )
 
     @BaseInference.run_if_required_wrapper
     def plot_continuous(
             self,
             file: str = None,
-            show=True,
+            show: bool = True,
             intervals: np.ndarray = None,
             confidence_intervals: bool = True,
             ci_level: float = 0.05,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             title: str = 'DFE comparison',
             labels: List[str] = None,
             scale_density: bool = False,
-            scale: Literal['lin', 'log'] = 'lin'
-    ) -> plt.axis:
+            scale: Literal['lin', 'log'] = 'lin',
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Plot discretized DFE. The special constants ``np.inf`` and ``-np.inf`` are also valid interval bounds.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
         disadvantage that the density now changes for x, so that even a constant
@@ -845,15 +851,16 @@
         :param title: Title of plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
-        :return: Axis object
+        :param ax: Axes object
+        :return: Axes object
         """
         if intervals is None:
             intervals = self.discretization.bins
 
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_continuous(**locals())
@@ -865,55 +872,60 @@
             confidence_intervals: bool = True,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
             show: bool = True,
             title: str = 'inferred parameters',
             labels: List[str] = None,
             legend: bool = True,
+            ax: plt.Axes = None,
             **kwargs: List[str]
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot discretized DFE comparing the different types.
 
         :param legend: Whether to show legend
         :param labels: Labels for types
         :param title: Title of plot
         :param bootstrap_type: Type of bootstrap
         :param ci_level: Confidence level
         :param confidence_intervals: Whether to plot confidence intervals
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis object
+        :param ax: Axes object
+        :return: Axes object
         """
         labels, inferences = zip(*self.get_inferences(labels=labels).items())
 
         return Inference.plot_inferred_parameters(**locals())
 
     @BaseInference.run_if_required_wrapper
     def plot_covariates(
             self,
             file: str = None,
             show: bool = True,
-    ) -> plt.axis:
+            axs: List[plt.Axes] = None
+    ) -> List[plt.Axes]:
         """
         Plot inferred parameters of joint inference vs inferred
         parameters of marginal inferences side by side.
 
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis object
+        :param axs: List of axes object, one for each covariate
+        :return: Axes object
         """
         from . import Visualization
 
-        Visualization.plot_covariates(
+        return Visualization.plot_covariates(
             covariates=self.covariates,
             params_marginal=dict((t, inf.params_mle) for t, inf in self.marginal_inferences.items()),
             params_joint=self.params_mle,
             file=file,
-            show=show
+            show=show,
+            axs=axs
         )
 
     def to_json(self) -> str:
         """
         Serialize object. Note that the deserialized inference objects no
         longer share the same optimization instance among other things.
```

### Comparing `fastdfe-0.1.1b0/fastdfe/spectrum.py` & `fastdfe-0.1.2b0/fastdfe/spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,28 +197,37 @@
         return Spectrum.from_list(self.data / other)
 
     def plot(
             self,
             show: bool = True,
             file: str = None,
             title: str = None,
-            show_monomorphic: bool = False
-    ) -> plt.axis:
+            show_monomorphic: bool = False,
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Plot spectrum.
+
+        :param show: Whether to show plot
+        :param file: File to save plot to
+        :param title: Title of plot
+        :param show_monomorphic: Whether to show monomorphic counts
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # import locally to avoid circular dependencies
         from fastdfe import Visualization
 
         return Visualization.plot_sfs_comparison(
             spectra=[self],
             file=file,
             show=show,
             title=title,
-            show_monomorphic=show_monomorphic
+            show_monomorphic=show_monomorphic,
+            ax=ax
         )
 
     @staticmethod
     def standard_kingman(n: int) -> 'Spectrum':
         """
         Get standard Kingman SFS.
 
@@ -534,37 +543,40 @@
 
     def plot(
             self,
             show: bool = True,
             file: str = None,
             title: str = None,
             use_subplots: bool = False,
-            show_monomorphic: bool = False
-    ) -> plt.axis:
+            show_monomorphic: bool = False,
+            ax: plt.Axes = None
+    ) -> plt.Axes:
         """
         Visualize spectra.
 
         :param show: Whether to show the plot
         :param file: File name to save the plot to
         :param title: Plot title
         :param use_subplots: Whether to use subplots
         :param show_monomorphic: Whether to show monomorphic sites
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # import locally to avoid circular dependencies
         from fastdfe import Visualization
 
         return Visualization.plot_sfs_comparison(
             spectra=list(self.to_spectra().values()),
             labels=self.types,
             file=file,
             show=show,
             title=title,
             use_subplots=use_subplots,
-            show_monomorphic=show_monomorphic
+            show_monomorphic=show_monomorphic,
+            ax=ax
         )
 
     def remove_empty(self) -> 'Spectra':
         """
         Remove types whose spectra have no counts.
         """
         return Spectra.from_dataframe(self.data.loc[:, self.data.any()])
```

### Comparing `fastdfe-0.1.1b0/fastdfe/visualization.py` & `fastdfe-0.1.2b0/fastdfe/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import pandas as pd
 import seaborn as sns
 from matplotlib import colors
 from matplotlib.colors import LogNorm
 from matplotlib.container import BarContainer
 from matplotlib.ticker import MaxNLocator
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-from tqdm import tqdm
 
 from . import Parametrization
 from .bootstrap import Bootstrap
 from .spectrum import Spectrum
 
 # get logger
 logger = logging.getLogger('fastdfe')
@@ -54,56 +53,64 @@
         and showing or saving produced plot subsequently.
 
         :param func: Function to decorate
         :return: Wrapper function
         """
 
         @functools.wraps(func)
-        def wrapper(*args, **kwargs) -> plt.axis:
+        def wrapper(*args, **kwargs) -> plt.Axes:
             """
             Wrapper function.
 
             :param args: Positional arguments
             :param kwargs: Keyword arguments
-            :return: Axis
+            :return: Axes
             """
-            # clear current figure
-            plt.clf()
+
+            # add axes if not given
+            if 'ax' not in kwargs or ('ax' in kwargs and kwargs['ax'] is None):
+                # clear current figure
+                plt.clf()
+
+                kwargs['ax'] = plt.gca()
 
             # execute function
             func(*args, **kwargs)
 
+            # make layout tight
+            plt.tight_layout()
+
             # show or save
             # show by default here
             return Visualization.show_and_save(
                 file=kwargs['file'] if 'file' in kwargs else None,
                 show=kwargs['show'] if 'show' in kwargs else True
             )
 
         return wrapper
 
     @staticmethod
-    def show_and_save(file: str = None, show=True) -> plt.axis:
+    def show_and_save(file: str = None, show: bool = True) -> plt.Axes:
         """
         Show and save plot.
 
         :param file: File path to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :return: Axes
 
         """
         # save figure if file path given
         if file is not None:
             plt.savefig(file, dpi=200, bbox_inches='tight', pad_inches=0.1)
 
         # show figure if specified and if not in interactive mode
         if show and not plt.isinteractive():
             plt.show()
 
-        # return axis
+        # return current axes
         return plt.gca()
 
     @staticmethod
     def interval_to_string(left: float, right: float) -> str:
         """
         Get string representation for given interval.
 
@@ -129,49 +136,51 @@
             return str(np.inf)
 
         return bracket_left + format_number(left) + ', ' + format_number(right) + bracket_right
 
     @staticmethod
     @clear_show_save
     def plot_discretized(
+            ax: plt.Axes,
             values: list | np.ndarray,
             errors: list | np.ndarray = None,
             labels: list | np.ndarray = None,
             file: str = None,
             show: bool = True,
             intervals: np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
             title: str = 'discretized DFE',
-            interval_labels: List[str] = None
+            interval_labels: List[str] = None,
 
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot discretized DFEs using a bar plot.
 
         :param interval_labels: Labels for the intervals
         :param labels: Labels for the DFEs
         :param title: Title of the plot
         :param values: Array of values of size ``intervals.shape[0] - 1``
         :param errors: Array of errors of size ``intervals.shape[0] - 1``
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bars.
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # number of intervals
         n_intervals = len(intervals) - 1
         n_dfes = len(values)
 
         width_total = 0.9
         width = width_total / n_dfes
 
         for i in range(n_dfes):
             x = np.arange(n_intervals) + i * width
 
             # plot discretized DFE
-            bars = plt.bar(
+            bars = ax.bar(
                 x=x,
                 height=values[i],
                 width=width,
                 yerr=errors[i],
                 error_kw=dict(
                     capsize=width * 7
                 ),
@@ -179,15 +188,14 @@
                 linewidth=0,
                 hatch=Visualization.get_hatch(i, labels),
                 color=Visualization.get_color(labels[i], labels) if labels is not None else None
             )
 
             Visualization.darken_edge_colors(bars)
 
-        ax = plt.gca()
         ax.set(xlabel='S', ylabel='fraction')
 
         # determine x-labels
         if interval_labels is None:
             xlabels = [Visualization.interval_to_string(intervals[i - 1], intervals[i]) for
                        i in range(1, n_intervals + 1)]
         else:
@@ -204,29 +212,32 @@
         # show legend if labels were given
         if labels is not None:
             plt.legend(prop=dict(size=8))
 
         # remove x-margins
         ax.autoscale(tight=True, axis='x')
 
+        return ax
+
     @staticmethod
     @clear_show_save
     def plot_continuous(
+            ax: plt.Axes,
             bins: np.ndarray,
             values: list | np.ndarray,
             errors: list | np.ndarray = None,
             labels: list | np.ndarray = None,
             file: str = None,
             show: bool = True,
             title: str = 'continuous DFE',
             scale: Literal['log', 'linear'] = 'lin',
             ylim: float = 1e-2,
             scale_density: bool = False,
             **kwargs
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot DFEs using a line plot.
         By default, the PDF is plotted as is. Due to the logarithmic scale on
         the x-axis, we may get a wrong intuition on how the mass is distributed,
         however. To get a better intuition, we can optionally scale the density
         by the x-axis interval size using ``scale_density = True``. This has the
         disadvantage that the density now changes for x, so that even a constant
@@ -238,26 +249,25 @@
         :param title: Title of the plot
         :param labels: Labels for the DFEs
         :param errors: Array of errors
         :param values: Array of values
         :param file: File path to save plot to
         :param show: Whether to show plot
         :param scale_density: Whether to scale the density by the bin size
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         from fastdfe.discretization import get_midpoints_and_spacing
 
         n_bins = len(bins) - 1
         n_dfes = len(values)
 
         # get interval sizes
         _, interval_sizes = get_midpoints_and_spacing(bins)
 
-        fig, ax = plt.subplots()
-
         for i in range(n_dfes):
             x = np.arange(n_bins)
 
             # plot DFE
             ax.plot(x,
                     values[i] if scale_density else values[i] / interval_sizes,
                     label=labels[i] if labels is not None else None)
@@ -284,14 +294,16 @@
             plt.legend(prop=dict(size=8))
 
         # remove x-margins
         ax.set_xmargin(0)
 
         ax.set_title(title)
 
+        return ax
+
     @staticmethod
     def adjust_ticks_show_s(s: np.ndarray):
         """
         Adjust x-ticks to show bin values.
 
         :return: Array of selection coefficients
         """
@@ -304,79 +316,83 @@
 
         ax.set_xticks(ticks)
         ax.set_xticklabels(ticks_new)
 
     @staticmethod
     @clear_show_save
     def plot_sfs_comparison(
+            ax: plt.Axes,
             spectra: List[Spectrum] | np.ndarray,
             labels: List[str] = [],
             file: str = None,
             show: bool = True,
             title: str = 'SFS comparison',
             use_subplots: bool = False,
             show_monomorphic: bool = False,
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot SFS comparison.
 
         :param use_subplots: Whether to use subplots
         :param show_monomorphic: Whether to show monomorphic counts
         :param title: Title of the plot
         :param labels: Labels for the SFSs
         :param spectra: List of spectrum objects in the same order as the labels or a 2D array
         :param file: File path to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # plot modelled vs observed non-neutral SFS
-        Visualization.plot_spectra(
+        ax = Visualization.plot_spectra(
             spectra=spectra,
             labels=labels,
             use_subplots=use_subplots,
-            show_monomorphic=show_monomorphic
+            show_monomorphic=show_monomorphic,
+            ax=ax
         )
 
         # set title
-        plt.title(title)
+        ax.set_title(title)
+
+        return ax
 
     @staticmethod
     @clear_show_save
     def plot_inferred_parameters(
             params: List[dict],
             bootstraps: List[pd.DataFrame],
+            ax: plt.Axes,
             file: str = None,
             show: bool = True,
             confidence_intervals: bool = True,
             bootstrap_type: Literal['percentile', 'bca'] = 'percentile',
             ci_level: float = 0.05,
             title: str = 'parameter estimates',
             scale: Literal['lin', 'log'] = 'log',
             labels: List[str] = None,
             **kwargs
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Visualize the inferred parameters and their confidence intervals.
         using a bar plot.
 
         :param labels: Labels for the parameters
         :param scale: Whether to use a linear or log scale
         :param title: Title of the plot
         :param ci_level: Confidence level
         :param bootstrap_type: Type of bootstrap to use
         :param confidence_intervals: Whether to show confidence intervals
         :param params: List of parameter dictionaries in the same order as the labels
         :param bootstraps: List of dataframes containing bootstrapped parameter values in the same order as the labels
         :param file: File path to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
-        # get current axes
-        fig, ax = plt.subplots()
-
         n_types = len(params)
 
         width_total = 0.9
         width = width_total / n_types
 
         # get keys of first element which we use to order the rest
         keys = sorted(list(params[0].keys()))
@@ -425,15 +441,15 @@
                     return '$' + label + '$'
 
                 return '$-' + key + '$'
 
             # append a minus sign to negative parameters values
             xlabels = np.array([name_to_label(key) for key in keys])
 
-            bars = plt.bar(
+            bars = ax.bar(
                 x=x,
                 height=y,
                 yerr=errors,
                 error_kw=dict(
                     capsize=width * 7
                 ),
                 label=labels[i] if labels is not None else None,
@@ -460,14 +476,16 @@
         # change to log-scale if specified
         if scale == 'log':
             ax.set_yscale('symlog', linthresh=1e-3)
 
         # remove x-margins
         ax.autoscale(tight=True, axis='x')
 
+        return ax
+
     @staticmethod
     def get_color(
             label: str,
             labels: List[str],
             get_group: Callable = lambda x: x.split('.')[-1]
     ) -> str:
         """
@@ -512,69 +530,70 @@
         prefix_index = list(prefixes).index(prefix)
 
         return hatch_styles[prefix_index % len(hatch_styles)]
 
     @staticmethod
     def plot_spectra(
             spectra: List[Spectrum],
+            ax: plt.Axes,
             labels: List[str] = [],
             log_scale: bool = False,
             use_subplots: bool = False,
             show_monomorphic: bool = False,
-            ax=None,
-            n_ticks=10
-    ) -> plt.axis:
+            n_ticks=10,
+            file: str = None,
+            show: bool = True
+    ) -> plt.Axes:
         """
         Plot the given 1D spectra.
 
         :param show_monomorphic: Whether to show monomorphic site counts
         :param n_ticks: Number of x-ticks to use
-        :param ax: Axis to plot on
+        :param ax: Axes to plot on
         :param use_subplots: Whether to use subplots
         :param spectra: List of spectra to plot
         :param labels: List of labels for each spectrum
         :param log_scale: Whether to use logarithmic y-scale
-        :return: Axis
+        :param file: File to save plot to
+        :param show: Whether to show the plot
+        :return: Axes
         """
         if use_subplots:
             n_plots = len(spectra)
             n_rows = int(np.ceil(np.sqrt(n_plots)))
             n_cols = int(np.ceil(np.sqrt(n_plots)))
             fig = plt.figure(figsize=(6.4 * n_cols ** (1 / 3), 4.8 * n_rows ** (1 / 3)))
             axes = fig.subplots(ncols=n_cols, nrows=n_rows, squeeze=False).flatten()
 
             # plot spectra individually
-            for i in tqdm(range(n_plots)):
+            for i in range(n_plots):
                 Visualization.plot_spectra(
                     spectra=[spectra[i]],
                     labels=[labels[i]] if len(labels) else [],
                     ax=axes[i],
                     n_ticks=15 // min(2, n_cols),
                     log_scale=log_scale,
                     show_monomorphic=show_monomorphic
                 )
 
             # make empty plots invisible
             [ax.set_visible(False) for ax in axes[n_plots:]]
 
-            plt.tight_layout()
+            # show and save plot
+            Visualization.show_and_save(file, show)
 
-            return
+            return plt.gca()
 
         # determine sample size and width
         n = spectra[0].n
         width_total = 0.9
         width = width_total / len(spectra)
 
         x = np.arange(n + 1) if show_monomorphic else np.arange(1, n)
 
-        # create axis if not specified
-        if ax is None:
-            _, ax = plt.subplots()
-
         # iterator over spectra and draw bars
         for i, sfs in enumerate(spectra):
             indices = x + i * width
             heights = sfs.to_list() if show_monomorphic else sfs.to_list()[1:-1]
 
             bars = ax.bar(
                 x=indices,
@@ -606,14 +625,17 @@
             ax.set_yscale('log')
 
         if len(labels) == 1:
             ax.set_title(labels[0])
         elif len(labels) > 1:
             plt.legend(prop=dict(size=8))
 
+        # show and save plot
+        Visualization.show_and_save(file, show)
+
         return ax
 
     @staticmethod
     def darken_edge_colors(bars: BarContainer):
         """
         Darken the edge color of the given bars.
 
@@ -639,157 +661,170 @@
 
     @staticmethod
     @clear_show_save
     def plot_pdf(
             model: Parametrization,
             params: dict,
             s: np.array,
+            ax: plt.Axes,
             file: str = None,
             show: bool = True
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot PDF of given parametrization.
 
         :param model: DFE parametrization
         :param params: Parameters to be used for parametrization
         :param s: Selection coefficients
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
-        plt.plot(np.arange(len(s)), model.get_pdf(**params)(s))
+        ax.plot(np.arange(len(s)), model.get_pdf(**params)(s))
 
         # customize x-ticks
         Visualization.adjust_ticks_show_s(s)
 
         # remove x-margins
-        plt.margins(x=0)
+        ax.margins(x=0)
+
+        return ax
 
     @staticmethod
     @clear_show_save
     def plot_cdf(
             model: Parametrization,
             params: dict,
             s: np.array,
+            ax: plt.Axes,
             file: str = None,
             show: bool = True
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot CDF of given parametrization.
 
         :param model: DFE parametrization
         :param params: Parameters to be used for parametrization
         :param s: Selection coefficients
+        :param ax: Axes to plot on
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :return: Axes
         """
-        plt.plot(np.arange(len(s)), model.get_cdf(**params)(s))
+        ax.plot(np.arange(len(s)), model.get_cdf(**params)(s))
 
         # customize x-ticks
         Visualization.adjust_ticks_show_s(s)
 
         # remove x-margins
-        plt.margins(x=0)
+        ax.margins(x=0)
+
+        return ax
 
     @staticmethod
     @clear_show_save
     def plot_likelihoods(
             likelihoods: list | np.ndarray,
             file: str, show: bool,
             title: str,
+            ax: plt.Axes,
             scale: Literal['lin', 'log'] = 'lin'
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         A scatter plot of the likelihoods specified.
 
         :param scale: Scale of y-axis
         :param likelihoods: Likelihoods to plot
         :param file: File to save plot to
         :param show: Whether to show plot
         :param title: Title of plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # plot
-        plt.scatter(np.arange(len(likelihoods)), likelihoods)
-
-        # get axis
-        ax = plt.gca()
+        ax.scatter(np.arange(len(likelihoods)), likelihoods)
 
         # set title
         ax.set_title(title)
 
         # use integer ticks
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
 
         # set labels
         ax.set_xlabel('iteration')
         ax.set_ylabel('lnl')
 
         if scale == 'log':
             ax.set_yscale('symlog')
 
+        return ax
+
     @staticmethod
     @clear_show_save
     def plot_buckets_sizes(
             n_intervals: int,
             bins: list | np.ndarray,
             sizes: list | np.ndarray,
             title: str,
             file: str,
-            show: bool
-    ) -> plt.axis:
+            show: bool,
+            ax: plt.Axes
+    ) -> plt.Axes:
         """
         A line plot of the bucket sizes.
 
         :param bins: Bins of the histogram
         :param n_intervals: Number of intervals
         :param sizes: Sizes of the buckets
         :param title: Title of plot
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
         # plot line
-        plt.plot(np.arange(n_intervals), sizes)
-
-        ax = plt.gca()
+        ax.plot(np.arange(n_intervals), sizes)
 
         # use log scale
         ax.set_yscale('log')
         ax.set_title(title)
 
         # customize x-ticks
         Visualization.adjust_ticks_show_s(bins)
 
         # remove x-margins
         ax.set_xmargin(0)
 
+        return ax
+
     @staticmethod
     @clear_show_save
     def plot_nested_likelihoods(
             P: np.ndarray,
             labels_x: list,
             labels_y: list,
+            ax: plt.Axes,
             file: str = None,
             show: bool = True,
             cmap: str = None,
             title: str = None
-    ) -> plt.axis:
+    ) -> plt.Axes:
         """
         Plot p-values of nested likelihoods.
 
         :param P: Matrix of p-values
         :param labels_x: Labels for x-axis
         :param labels_y: Labels for y-axis
         :param file: File to save plot to
         :param show: Whether to show plot
         :param cmap: Colormap to use
         :param title: Title of plot
-        :return: Axis
+        :param ax: Axes to plot on
+        :return: Axes
         """
 
         def format_number(x: float | int | None) -> float | int | str:
             """
             Format number to be displayed.
             """
             if x == 0 or x is None:
@@ -803,19 +838,17 @@
         # determine values to display
         annot = np.vectorize(lambda x: str(format_number(x)))(P)
         annot[np.equal(P, None)] = '-'
 
         # change to 1 to get a nicer color
         P[np.equal(P, None)] = 1
 
-        fig, ax = plt.subplots()
-
         # make the cbar have the same height as the heatmap
         cbar_ax = make_axes_locatable(ax).new_horizontal(size="4%", pad=0.15)
-        fig.add_axes(cbar_ax)
+        plt.gcf().add_axes(cbar_ax)
 
         # default color map
         if cmap is None:
             cmap = colors.LinearSegmentedColormap.from_list('_', plt.get_cmap('inferno')(np.linspace(0.3, 1, 100)))
 
         # plot heatmap
         sns.heatmap(
@@ -840,45 +873,54 @@
         # adjust tick labels
         ax.set_xticklabels([l.replace('_', ' ') for l in labels_x], rotation=45)
         ax.set_yticklabels([l.replace('_', ' ') for l in labels_y], rotation=0)
 
         # set title
         ax.set_title(title)
 
+        return ax
+
     @staticmethod
     @clear_show_save
     def plot_covariates(
             covariates: Dict[str, 'Covariate'],
             params_marginal: Dict[str, Dict[str, float]],
             params_joint: Dict[str, Dict[str, float]],
+            axs: List[plt.Axes],
             scale: Literal['lin', 'log'] = 'log',
             file: str = None,
-            show: bool = True
-    ) -> plt.axis:
+            show: bool = True,
+            **kwargs
+    ) -> List[plt.Axes]:
         """
         Plot covariates.
 
-        :param params_joint: Unpacked joint parameters indexed by type
+        :param covariates: Covariates to plot
         :param params_marginal: Marginal parameters indexed by type
+        :param params_joint: Unpacked joint parameters indexed by type
+        :param axs: List of axes, one for each covariate
         :param scale: Scale of y-axis
-        :param covariates: Covariates to plot
         :param file: File to save plot to
         :param show: Whether to show plot
-        :return: Axis
+        :return: Axes
         """
         if len(covariates) == 0:
-            return logger.info("There are no covariates to be plotted.")
+            logger.info("There are no covariates to be plotted.")
+
+            return axs
 
         types = list(params_joint.keys())
 
         num_covariates = len(covariates)
 
         n_cols = min(3, num_covariates)
         n_rows = int(np.ceil(num_covariates / n_cols))
-        fig, axs = plt.subplots(n_rows, n_cols, figsize=(6.4 * n_cols, 4.8 * n_rows), squeeze=False)
+
+        if not isinstance(axs, np.ndarray | list):
+            _, axs = plt.subplots(n_rows, n_cols, figsize=(6.4 * n_cols, 4.8 * n_rows), squeeze=False)
 
         n_intervals = len(types)
         width_total = 0.9
         width = width_total / 2
 
         for i, (p, cov) in enumerate(covariates.items()):
             ax = axs[i // n_cols, i % n_cols]
@@ -917,8 +959,62 @@
             # set legend
             ax.legend()
 
             # set y-scale
             if scale == 'log':
                 ax.set_yscale('log')
 
-        fig.tight_layout()
+        return axs
+
+    @clear_show_save
+    def plot_interval_density(
+            self,
+            ax: plt.Axes,
+            density: np.ndarray,
+            intervals: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf]),
+            interval_labels: List[str] = None,
+            file: str = None,
+            show: bool = True,
+            color: str = 'C0',
+
+    ) -> plt.Axes:
+        """
+        Plot density of the discretization intervals chosen.
+
+        :param density:
+        :param color: Color of the bars.
+        :param file: File to save plot to.
+        :param show: Whether to show plot.
+        :param interval_labels: Labels for the intervals.
+        :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
+        :param ax: Axes to plot on.
+        :return: Axes object
+        """
+        # number of intervals
+        n_intervals = len(intervals)
+
+        # x-values
+        x = np.arange(n_intervals - 1)
+
+        # plot plot
+        sns.barplot(x=x, y=density / density.sum(), color=color, ax=ax)
+
+        # set labels
+        ax.set(xlabel='S', ylabel='fraction')
+
+        # determine x-labels
+        if interval_labels is None:
+            xlabels = [Visualization.interval_to_string(intervals[i - 1], intervals[i]) for i in range(1, n_intervals)]
+        else:
+            xlabels = interval_labels
+
+        # adjust x-ticks
+        ax.set_xticks(x)
+        ax.set_xticklabels(xlabels)
+
+        # set title
+        ax.set_title('interval density')
+
+        # remove x-margins
+        ax.autoscale(tight=True, axis='x')
+
+        return ax
```

### Comparing `fastdfe-0.1.1b0/pyproject.toml` & `fastdfe-0.1.2b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastdfe"
-version = "0.1.1-beta"
+version = "0.1.2-beta"
 description = "Fast, flexible, and hierarchical inference of the distribution of fitness effects"
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `fastdfe-0.1.1b0/PKG-INFO` & `fastdfe-0.1.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 0.1.1b0
+Version: 0.1.2b0
 Summary: Fast, flexible, and hierarchical inference of the distribution of fitness effects
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

