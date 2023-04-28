# Comparing `tmp/pca-2.0.0.tar.gz` & `tmp/pca-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-2.0.0.tar", last modified: Sun Apr 23 10:11:34 2023, max compression
+gzip compressed data, was "pca-2.0.1.tar", last modified: Fri Apr 28 11:38:45 2023, max compression
```

## Comparing `pca-2.0.0.tar` & `pca-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.050449 pca-2.0.0/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9981 2023-04-23 10:11:34.050449 pca-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9457 2023-04-23 08:28:30.000000 pca-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.033471 pca-2.0.0/pca/
--rw-rw-rw-   0        0        0     1272 2023-04-23 09:53:19.000000 pca-2.0.0/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.048432 pca-2.0.0/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.0/pca/data/__init__.py
--rw-rw-rw-   0        0        0    31375 2023-04-23 09:41:51.000000 pca-2.0.0/pca/examples.py
--rw-rw-rw-   0        0        0    73611 2023-04-23 09:40:00.000000 pca-2.0.0/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.049428 pca-2.0.0/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.0/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.0/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:11:34.047433 pca-2.0.0/pca.egg-info/
--rw-rw-rw-   0        0        0     9981 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-23 10:11:33.000000 pca-2.0.0/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:11:34.051423 pca-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.529502 pca-2.0.1/
+-rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9981 2023-04-28 11:38:45.527947 pca-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9457 2023-04-23 08:28:30.000000 pca-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.418075 pca-2.0.1/pca/
+-rw-rw-rw-   0        0        0     1272 2023-04-28 11:38:30.000000 pca-2.0.1/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.518970 pca-2.0.1/pca/data/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.1/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    33412 2023-04-28 11:37:18.000000 pca-2.0.1/pca/examples.py
+-rw-rw-rw-   0        0        0    77776 2023-04-28 11:25:11.000000 pca-2.0.1/pca/pca.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.523957 pca-2.0.1/pca/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.1/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.1/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:38:45.507999 pca-2.0.1/pca.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-04-28 11:38:45.000000 pca-2.0.1/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 11:38:44.000000 pca-2.0.1/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 11:38:45.529941 pca-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.1/setup.py
```

### Comparing `pca-2.0.0/LICENSE` & `pca-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-2.0.0/PKG-INFO` & `pca-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.0
+Version: 2.0.1
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.0 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.1 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.0/README.md` & `pca-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pca-2.0.0/pca/__init__.py` & `pca-2.0.1/pca/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
 Description
```

### Comparing `pca-2.0.0/pca/examples.py` & `pca-2.0.1/pca/examples.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,78 @@
 from pca import pca
 import pandas as pd
 import numpy as np
 import matplotlib as mpl
+from scatterd import scatterd
 
 import numpy as np
 from sklearn.datasets import load_iris
 import pandas as pd
 
-
 # %%
-from sklearn.datasets import make_friedman1
-X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
+# Load pca
+from pca import pca
 
-model = pca()
-model.fit_transform(X)
+# Initialize pca
+model = pca(n_components=3)
 
-# model.scatter(density=True)
-# model.biplot(c=[0,0,0], density=True)
+# Load example data set
+df = model.import_example(data='iris')
 
-# model.scatter3d(fontsize=16, PC=[0,1,3])
-# model.scatter3d(density=True)
+# Fit transform
+results = model.fit_transform(df)
 
-model.biplot3d(arrowdict={'weight':'bold'},  c=None, n_feat=5)
+# Make plot
+model.biplot(HT2=True,
+             SPE=True,
+             s=np.random.randint(20, 500, size=df.shape[0]),
+             marker=df.index.values,
+             cmap='bwr_r',
+             fontsize=22,
+             legend=2,
+             density=True,
+             arrowdict={'color_strong': 'r', 'color_weak': 'g'},
+             title='Biplot with with the pca library.')
+
+
+# %%
+# from sklearn.datasets import make_friedman1
+# X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
+
+# model = pca()
+# model.fit_transform(X)
+
+# Loading are automatically set based on weak/strong
+model.biplot(s=0)
+# Change strong and weak colors
+model.biplot(s=0, arrowdict={'color_strong': 'r', 'color_weak': 'g'})
+# Set alpha to constant value
+model.biplot(s=0, arrowdict={'alpha': 0.8})
+# Change arrow text color
+model.biplot(s=0, arrowdict={'color_text': 'k'})
+# Change arrow color, which automatically changes the label color too
+model.biplot(s=0, color_arrow='k')
+# Almost Remove arrows but keep the text
+model.biplot(s=0, color_arrow='k', arrowdict={'alpha': 0.9})
+# Set color text
+model.biplot(s=0, arrowdict={'color_text': 'k'})
+# Set color arrow and color text
+model.biplot(s=0, color_arrow='k', arrowdict={'color_text': 'g'})
+# Set color arrow and color text and alpha
+model.biplot(s=0, color_arrow='k', arrowdict={'color_text': 'g', 'alpha': 0.8})
+
+# Change the scale factor of the arrow
+model.biplot(arrowdict={'scale_factor': 2})
+model.biplot3d(arrowdict={'scale_factor': 3})
+
+model.biplot(s=0, arrowdict={'weight':'bold', 'fontsize': 24, 'color_text': 'r'}, color_arrow='k')
+model.biplot3d(density=True, fontsize=0, arrowdict={'weight':'bold', 'fontsize': 14})
+model.biplot3d(density=True, fontsize=0, s=0, arrowdict={'fontsize': 24})
+model.biplot3d(density=True, fontsize=0, s=0, arrowdict={'fontsize': 24, 'scale_factor': 3})
+model.biplot(density=True, fontsize=0, arrowdict={'weight':'bold', 'fontsize': 14})
 
 
 # %%
 from pca import pca
 from sklearn.datasets import load_wine
 import pandas as pd
 
@@ -36,17 +83,17 @@
 labels = data.feature_names
 # Make dataframe
 df = pd.DataFrame(data=X, columns=labels, index=y)
 
 model = pca(normalize=True, n_components=None)
 # Fit transform with dataframe
 results = model.fit_transform(df)
-
-model.biplot(labels=df['flavanoids'].values, legend=False, cmap='seismic', n_feat=3, fontsize=20, arrowdict={'fontsize':28, 'c':'g'}, density=True)
-model.biplot3d(legend=False, n_feat=3, fontcolor='r', arrowdict={'fontsize':22, 'c':'k'}, density=True)
+# Plot
+model.biplot(fontsize=0, labels=df['flavanoids'].values, legend=False, cmap='seismic', n_feat=3, arrowdict={'fontsize':28, 'c':'g'}, density=True)
+# model.biplot3d(legend=None, n_feat=3, fontcolor='r', arrowdict={'fontsize':22, 'c':'k'}, density=True, figsize=(35, 30))
 
 
 # %% Demonstration of specifying colors, markers, alpha, and size per sample
 # Import library
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
@@ -132,31 +179,26 @@
               edgecolor='#FFFFFF',
               gradient='#FFFFFF',
               density=True,
               density_on_top=False,
               visible=True,
               )
 
-
-
-
-
-
 # %%
 # Load pca
 from pca import pca
 
 # Initialize pca
-model = pca()
+model = pca(n_components=3)
 
 # Load example data set
 df = model.import_example(data='iris')
 
 # Fit transform
-results = model.fit_transform(X)
+results = model.fit_transform(df)
 
 # Make plot
 model.biplot(HT2=True,
              SPE=True,
              s=np.random.randint(20, 500, size=df.shape[0]),
              marker=y,
              cmap='bwr_r',
@@ -388,19 +430,19 @@
 # Remove scatterpoints by setting cmap=None
 model.biplot(cmap=None)
 
 
 # Color on classlabel (Unchanged)
 model.biplot()
 # Use cmap colors for classlabels (unchanged)
-model.biplot(labels=y, cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
+model.biplot(labels=y, cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']), density=True)
 # Do not show points when cmap=None (unchanged)
-model.biplot(labels=load_iris().target, cmap=None)
+model.biplot(labels=load_iris().target, cmap=None, density=True)
 # Plot all points as unique entity (unchanged)
-model.biplot(labels=y, gradient='#ffffff', cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']))
+model.biplot(labels=y, gradient='#ffffff', cmap=mpl.colors.ListedColormap(['green', 'red', 'blue']), density=True)
 
 
 # %%
 import numpy as np
 from sklearn.datasets import load_iris
 
 # Load dataset
@@ -455,14 +497,15 @@
 X_unseen = np.array(np.random.uniform(5, 10, 25)).reshape(5, 5)
 
 # map the new "unseen" data in the existing space
 PCnew = model.transform(X_unseen)
 
 # Plot image
 model.biplot(SPE=True, HT2=True, density=True)
+model.biplot3d(SPE=True, HT2=True, density=True, arrowdict={'scale_factor': 1})
 
 # %% Detect unseen outliers
 # Import libraries
 from pca import pca
 import pandas as pd
 import numpy as np
 
@@ -470,29 +513,29 @@
 X = np.array(np.random.normal(0, 1, 500)).reshape(100, 5)
 
 # Initialize model. Alpha is the threshold for the hotellings T2 test to determine outliers in the data.
 model = pca(alpha=0.05, detect_outliers=['HT2', 'SPE'])
 # model = pca(alpha=0.05, detect_outliers=None)
 
 # Fit transform
-model.fit_transform(X)
+model.fit_transform(X, row_labels=np.zeros(X.shape[0]))
 
 model.scatter(SPE=True, HT2=True)
 
 for i in range(0, 10):
     # Create 5 outliers
     X_unseen = np.array(np.random.uniform(5, 10, 25)).reshape(5, 5)
 
     # Transform new "unseen" data.
     PCnew = model.transform(X_unseen, row_labels=np.repeat('mapped_' + str(i), X_unseen.shape[0]), update_outlier_params=True)
 
     # Scatterplot
-    model.scatter(SPE=True, HT2=True)
+    # model.scatter(SPE=True, HT2=True)
     # Biplot
-    # Model.biplot(SPE=True, HT2=True)
+    model.biplot(SPE=True, HT2=True, density=True)
 
 
 # %%
 from sklearn.datasets import make_friedman1
 X, _ = make_friedman1(n_samples=200, n_features=30, random_state=0)
 
 model = pca(method='sparse_pca')
```

### Comparing `pca-2.0.0/pca/pca.py` & `pca-2.0.1/pca/pca.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import scipy.sparse as sp
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 from adjustText import adjust_text
 import statsmodels.stats.multitest as multitest
+from typing import List, Union, Tuple
 
 
 # %% Association learning across all variables
 class pca:
     """pca module.
 
     Parameters
@@ -693,28 +694,28 @@
                alpha=0.8,
                gradient=None,
                density=False,
                density_on_top=False,
                fontcolor=[0,0,0],
                fontsize=18,
                fontweight='normal',
-               color_arrow='#000000',
-               arrowdict={'fontsize': None, 'c': None, 'weight': None, 'ha': 'center', 'va': 'center'},
+               color_arrow=None,
+               arrowdict={'fontsize': None, 'color_text': None, 'weight': None, 'alpha': None, 'color_strong': '#880808', 'color_weak': '#002a77', 'scale_factor': None},
                cmap='tab20c',
                title=None,
                legend=None,
                figsize=(25, 15),
                visible=True,
                fig=None,
                ax=None,
                dpi=100,
                y=None,  # deprecated
                label=None,  # deprecated
                verbose=None):
-        """Create the Biplot.
+        """Create Biplot.
 
         Plots the Principal components with the samples, and the best performing features.
         Per PC, The feature with absolute highest loading is gathered. This can result into features that are seen over multiple PCs, and some features may never be detected.
         For vizualization purposes we will keep only the unique feature-names and plot them with red arrows and green labels.
         The feature-names that were never discovered (described as weak) are colored yellow.
 
         Parameters
@@ -762,27 +763,38 @@
             Hex (ending) color for the gradient of the scatterplot colors.
             '#FFFFFF'
         density : Bool (default: False)
             Include the kernel density in the scatter plot.
         density_on_top : bool, (default: False)
             True : The density is the highest layer.
             False : The density is the lowest layer.
-        color_arrow : String, (default: '#000000')
-            color for the arrow.
-            * '#000000'
-            * 'r'
-        arrowdict : dict.
-            dictionary containing properties for the arrow font-text.
-            Note that the [c]olor: None inherits the color used in color_arrow.
-            {'fontsize': None, 'c': None, 'weight': None, 'ha': 'center', 'va': 'center'}
-        fontsize : String, optional
-            The fontsize of the y labels that are plotted in the graph. The default is 16.
+        fontsize : String (default: 16)
+            The fontsize of the labels.
         fontcolor: list/array of RGB colors with same size as X (default : None)
             None : Use same colorscheme as for c
             '#000000' : If the input is a single color, all fonts will get this color.
+        fontweight : String, (default: 'normal')
+            The fontweight of the labels.
+                * 'normal'
+                * 'bold'
+        color_arrow : String, (default: None)
+            color for the arrow.
+                * None: Color arrows based on strength using 'color_strong' and 'color_weak'.
+                * '#000000'
+                * 'r'
+        arrowdict : dict.
+            Dictionary containing properties for the arrow font-text.
+            {'fontsize': None, 'color_text': None, 'weight': None, 'alpha': None, 'color_strong': '#880808', 'color_weak': '#002a77', 'ha': 'center', 'va': 'center'}
+                * fontsize: None automatically adjust based on the fontsize. Specify otherwise.
+                * 'color_text': None automatically adjust color based color_strong and color_weak. Specify hex color otherwise.
+                * 'weight': None automatically adjust based on fontweight. Specify otherwise: 'normal', 'bold'
+                * 'alpha': None automatically adjust based on loading value.
+                * 'color_strong': Hex color for strong loadings (color_arrow needs to be set to None).
+                * 'color_weak': Hex color for weak loadings (color_arrow needs to be set to None).
+                * 'scale_factor': The scale factor for the arrow length. None automatically sets changes between 2d and 3d plots.
         cmap : String, optional, default: 'Set1'
             Colormap. If set to None, no points are shown.
         title : str, default: None
             Title of the figure.
             None: Automatically create title text based on results.
             '' : Remove all title text.
             'title text' : Add custom title text.
@@ -825,15 +837,15 @@
         # Input checks
         arrowdict, cmap, PC, d3, s = _biplot_input_checks(self.results, PC, cmap, arrowdict, color_arrow, fontsize, fontweight, c, s, verbose)
         # Pre-processing
         labels, topfeat, n_feat = self._fig_preprocessing(labels, n_feat, d3)
         # Scatterplot
         fig, ax = self.scatter(labels=labels, legend=legend, PC=PC, SPE=SPE, HT2=HT2, cmap=cmap, visible=visible, figsize=figsize, alpha=alpha, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, fontcolor=fontcolor, fontweight=fontweight, fontsize=fontsize, edgecolor=edgecolor, density=density, density_on_top=density_on_top, dpi=dpi, verbose=verbose)
         # Add the loadings with arrow to the plot
-        fig, ax = _plot_loadings(self, topfeat, n_feat, PC, d3, color_arrow, arrowdict, fig, ax, verbose)
+        fig, ax = _plot_loadings(self, topfeat, n_feat, PC, d3, arrowdict, fig, ax, verbose)
         # Plot
         if visible: plt.show()
         # Return
         return fig, ax
 
     def scatter3d(self, PC=[0, 1, 2], **args):
         """Scatter 3d plot.
@@ -841,23 +853,23 @@
         Parameters
         ----------
         Input parameters are described under <scatter>.
         """
         fig, ax = self.scatter(PC=PC, **args)
         return fig, ax
 
-    def biplot3d(self, PC=[0, 1, 2], alpha=0.8, **args):
+    def biplot3d(self, PC=[0, 1, 2], alpha=0.8, figsize=(30, 25), **args):
         """Biplot 3d plot.
 
         Parameters
         ----------
         Input parameters are described under <scatter>.
         """
         if not isinstance(alpha, (int, float)): alpha=0.8
-        fig, ax = self.biplot(PC=PC, alpha=alpha, **args)
+        fig, ax = self.biplot(PC=PC, alpha=alpha, figsize=figsize, **args)
         return fig, ax
 
     # Show explained variance plot
     def plot(self, n_components=None, xsteps=None, title=None, visible=True, figsize=(15, 10), fig=None, ax=None, verbose=None):
         """Scree-plot together with explained variance.
 
         Parameters
@@ -1463,18 +1475,18 @@
     # Set defaults in arrowdict
     arrowdict =_set_arrowdict(arrowdict, color_arrow=color_arrow, fontsize=fontsize, fontweight=fontweight)
     # Return
     return arrowdict, cmap, PC, d3, s
 
 
 def _set_arrowdict(arrowdict, color_arrow=None, fontsize=18, fontweight='normal'):
-    color_arrow = 'black' if (color_arrow is None) else color_arrow
-    arrowdict = {**{'fontsize': 18 if fontsize==0 else fontsize, 'c': color_arrow, 'weight': fontweight, 'ha': 'center', 'va': 'center'}, **arrowdict}
-    if arrowdict.get('c') is None and (color_arrow is not None):
-        arrowdict['c'] = color_arrow
+    # color_arrow = None if (color_arrow is None) else color_arrow
+    arrowdict = {**{'color_arrow': color_arrow, 'color_text': None, 'fontsize': 18 if fontsize==0 else fontsize, 'weight': fontweight, 'alpha': None, 'ha': 'center', 'va': 'center', 'color_strong': '#880808', 'color_weak': '#002a77', 'scale_factor': None}, **arrowdict}
+    # if arrowdict.get('color_text') is None and (color_arrow is not None):
+        # arrowdict['color_text'] = color_arrow
     if arrowdict.get('fontsize') is None:
         arrowdict['fontsize'] = 18 if fontsize==0 else fontsize
     if arrowdict.get('weight') is None:
         arrowdict['weight'] = fontweight
     return arrowdict
 
 
@@ -1524,56 +1536,72 @@
 
     if fig is not None:
         fig.set_visible(visible)
 
     return fig, ax
 
 
-def _plot_loadings(self, topfeat, n_feat, PC, d3, color_arrow, arrowdict, fig, ax, verbose):
+def _plot_loadings(self, topfeat, n_feat, PC, d3, arrowdict, fig, ax, verbose):
     topfeat = pd.concat([topfeat.iloc[PC, :], topfeat.loc[~topfeat.index.isin(PC), :]])
     topfeat.reset_index(inplace=True)
     # Collect coefficients
     coeff = self.results['loadings'].iloc[PC, :]
 
     # Use the PCs only for scaling purposes
     mean_x = np.mean(self.results['PC'].iloc[:, PC[0]].values)
     mean_y = np.mean(self.results['PC'].iloc[:, PC[1]].values)
     if d3: mean_z = np.mean(self.results['PC'].iloc[:, PC[2]].values)
 
     # Plot and scale values for arrows and text by taking the absolute minimum range of the x-axis and y-axis.
     max_axis = np.max(np.abs(self.results['PC'].iloc[:, PC]).min(axis=1))
     max_arrow = np.abs(coeff).max().max()
-    scale = (np.max([1, np.round(max_axis / max_arrow, 2)])) * 0.93
+    if arrowdict['scale_factor'] is None: 
+        scale_factor = 1.8 if d3 else 1.1
+    else:
+        scale_factor = arrowdict['scale_factor']
+    # Scale the arrows using the scale factor
+    scale = (np.max([1, np.round(max_axis / max_arrow, 2)])) * scale_factor
 
     # For vizualization purposes we will keep only the unique feature-names
     topfeat = topfeat.drop_duplicates(subset=['feature'])
     if topfeat.shape[0]<n_feat:
         n_feat = topfeat.shape[0]
         if verbose>=2: print('[pca] >[WARNING]: n_feat can not be reached because of the limitation of n_components (=%d). n_feat is reduced to %d.' %(self.n_components, n_feat))
 
     # Plot arrows and text
+    arrow_line_color = arrowdict['color_arrow']
+    arrow_text_color = arrowdict['color_text']
+    arrow_alpha = arrowdict['alpha']
+    alpha_scaled = normalize_size(topfeat['loading'].abs().values.reshape(-1,1), minscale=0.35, maxscale=0.95, scaler='minmax')
     texts = []
     for i in range(0, n_feat):
         getfeat = topfeat['feature'].iloc[i]
         label = getfeat + ' (' + ('%.3g' %topfeat['loading'].iloc[i]) + ')'
         getcoef = coeff[getfeat].values
         # Set first PC vs second PC direction. Note that these are not neccarily the best loading.
         xarrow = getcoef[0] * scale  # First PC in the x-axis direction
         yarrow = getcoef[1] * scale  # Second PC in the y-axis direction
-        txtcolor = 'y' if topfeat['type'].iloc[i] == 'weak' else 'g'
+        # Set the arrow and arrow-text colors
+        # Update arrow color if None
+        loading_color = arrowdict['color_weak'] if topfeat['type'].iloc[i] == 'weak' else arrowdict['color_strong']
+        # Update colors if None
+        if arrowdict['color_arrow'] is None: arrow_line_color = loading_color
+        if arrowdict['color_text'] is None: arrow_text_color = loading_color
+        if arrowdict['alpha'] is None: arrow_alpha =  alpha_scaled[i]
 
         if d3:
             zarrow = getcoef[2] * scale
-            ax.quiver(mean_x, mean_y, mean_z, xarrow - mean_x, yarrow - mean_y, zarrow - mean_z, color=color_arrow, alpha=0.8, lw=2)
-            texts.append(ax.text(xarrow, yarrow, zarrow, label, color=arrowdict['c'], ha='center', va='center', fontsize=arrowdict['fontsize'], zorder=25))
+            ax.quiver(mean_x, mean_y, mean_z, xarrow - mean_x, yarrow - mean_y, zarrow - mean_z, color=arrow_line_color, alpha=arrow_alpha, lw=2)
+            texts.append(ax.text(xarrow, yarrow, zarrow, label, fontsize=arrowdict['fontsize'], c=arrow_text_color, weight=arrowdict['weight'], ha=arrowdict['ha'], va=arrowdict['va'], zorder=25))
         else:
-            ax.arrow(mean_x, mean_y, xarrow - mean_x, yarrow - mean_y, color=color_arrow, alpha=0.8, width=0.002, head_width=0.1, head_length=0.1 * 1.1, length_includes_head=True, zorder=10)
-            texts.append(ax.text(xarrow, yarrow, label, fontdict=arrowdict, zorder=10))
+            head_width = 0.1
+            ax.arrow(mean_x, mean_y, xarrow - mean_x, yarrow - mean_y, color=arrow_line_color, alpha=arrow_alpha, width=0.002, head_width=head_width, head_length=head_width * 1.1, length_includes_head=True, zorder=10)
+            texts.append(ax.text(xarrow, yarrow, label, fontsize=arrowdict['fontsize'], c=arrow_text_color, weight=arrowdict['weight'], ha=arrowdict['ha'], va=arrowdict['va'], zorder=10))
 
-    # Plot the adjusted text labels to prevent overlap
+    # Plot the adjusted text labels to prevent overlap. Do not adjust text in 3d plots as it will mess up the locations.
     if len(texts)>0 and not d3: adjust_text(texts)
 
     # Return
     return fig, ax
 
 
 def _add_plot_SPE(self, xs, ys, zs, SPE, d3, alpha, s, fig, ax):
@@ -1591,17 +1619,17 @@
 
     # Plot outliers for hotelling T2 test.
     if isinstance(s, (int, float)): s = 150 if s>0 else 0
     if not isinstance(s, (int, float)): s=150
     if SPE and ('y_bool_spe' in self.results['outliers'].columns):
         label_spe = str(sum(Ioutlier2)) + ' outlier(s) (SPE/DmodX)'
         if d3:
-            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], zs[Ioutlier2], marker='x', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha)
+            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], zs[Ioutlier2], marker='x', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha, zorder=15)
         else:
-            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], marker='d', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha)
+            ax.scatter(xs[Ioutlier2], ys[Ioutlier2], marker='d', color=[0.5, 0.5, 0.5], s=s, label=label_spe, alpha=alpha, zorder=15)
 
     return fig, ax
 
 
 def _add_plot_HT2(self, xs, ys, zs, HT2, d3, alpha, s, fig, ax):
     # Plot outliers for hotelling T2 test.
     if isinstance(s, (int, float)): s = 150 if s>0 else 0
@@ -1609,17 +1637,17 @@
     # Plot outliers for hotelling T2 test.
     if HT2 and ('y_bool' in self.results['outliers'].columns):
         Ioutlier1 = self.results['outliers']['y_bool'].values
 
     if HT2 and ('y_bool' in self.results['outliers'].columns):
         label_t2 = str(sum(Ioutlier1)) + ' outlier(s) (hotelling t2)'
         if d3:
-            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], zs[Ioutlier1], marker='d', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha)
+            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], zs[Ioutlier1], marker='d', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha, zorder=15)
         else:
-            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], marker='x', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha)
+            ax.scatter(xs[Ioutlier1], ys[Ioutlier1], marker='x', color=[0, 0, 0], s=s, label=label_t2, alpha=alpha, zorder=15)
 
     return fig, ax
 
 
 def _add_plot_properties(self, PC, d3, title, legend, labels, fig, ax, fontsize, verbose):
     # Set labels
     ax.set_xlabel('PC' + str(PC[0] + 1) + ' (' + str(self.results['model'].explained_variance_ratio_[PC[0]] * 100)[0:4] + '% expl.var)')
@@ -1641,12 +1669,60 @@
 
     ax.set_title(title, fontsize=18)
     ax.grid(True)
     # Return
     return fig, ax
 
 
+def normalize_size(getsizes, minscale: Union[int, float] = 0.5, maxscale: Union[int, float] = 4, scaler: str = 'zscore'):
+    """Normalize values between minimum and maximum value.
+
+    Parameters
+    ----------
+    getsizes : input array
+        Array of values that needs to be scaled.
+    minscale : Union[int, float], optional
+        Minimum value. The default is 0.5.
+    maxscale : Union[int, float], optional
+        Maximum value. The default is 4.
+    scaler : str, optional
+        Type of scaler. The default is 'zscore'.
+            * 'zscore'
+            * 'minmax'
+
+    Returns
+    -------
+    getsizes : array-like
+        scaled values between min-max.
+
+    """
+    # Instead of Min-Max scaling, that shrinks any distribution in the [0, 1] interval, scaling the variables to
+    # Z-scores is better. Min-Max Scaling is too sensitive to outlier observations and generates unseen problems,
+    
+    # Set sizes to 0 if not available
+    getsizes[np.isinf(getsizes)]=0
+    getsizes[np.isnan(getsizes)]=0
+
+    # out-of-scale datapoints.
+    if scaler == 'zscore' and len(np.unique(getsizes)) > 3:
+        getsizes = (getsizes.flatten() - np.mean(getsizes)) / np.std(getsizes)
+        getsizes = getsizes + (minscale - np.min(getsizes))
+    elif scaler == 'minmax':
+        try:
+            from sklearn.preprocessing import MinMaxScaler
+        except:
+            raise Exception('sklearn needs to be pip installed first. Try: pip install scikit-learn')
+        # scaling
+        getsizes = MinMaxScaler(feature_range=(minscale, maxscale)).fit_transform(getsizes).flatten()
+    else:
+        getsizes = getsizes.ravel()
+    # Max digits is 4
+    getsizes = np.array(list(map(lambda x: round(x, 4), getsizes)))
+
+    return getsizes
+
+
 def _show_deprecated_warning(label, y, verbose):
     if label is not None:
         if verbose>=2: print('[pca]> [WARNING]: De parameter <label> is deprecated and will not be supported in future version.')
     if y is not None:
         if verbose>=2: print('[pca]> [WARNING]: De parameter <y> is deprecated and will not be supported in future version. Use <labels> instead.')
```

### Comparing `pca-2.0.0/pca/tests/test_pca.py` & `pca-2.0.1/pca/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.0/pca.egg-info/PKG-INFO` & `pca-2.0.1/pca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.0
+Version: 2.0.1
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.0 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.1 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.0.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.1.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.0/setup.py` & `pca-2.0.1/setup.py`

 * *Files identical despite different names*

