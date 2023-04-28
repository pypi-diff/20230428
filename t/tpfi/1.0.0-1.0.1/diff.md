# Comparing `tmp/tpfi-1.0.0.tar.gz` & `tmp/tpfi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.0.tar", max compression
+gzip compressed data, was "tpfi-1.0.1.tar", max compression
```

## Comparing `tpfi-1.0.0.tar` & `tpfi-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-04-28 03:35:14.040626 tpfi-1.0.0/LICENSE
--rw-r--r--   0        0        0     2211 2023-04-28 03:35:14.040626 tpfi-1.0.0/README.md
--rw-r--r--   0        0        0      417 2023-04-28 03:35:14.048626 tpfi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    13873 2023-04-28 03:35:14.048626 tpfi-1.0.0/tpfi.py
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 tpfi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-28 16:03:14.851920 tpfi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2251 2023-04-28 16:03:14.851920 tpfi-1.0.1/README.md
+-rw-r--r--   0        0        0      417 2023-04-28 16:03:14.859920 tpfi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14657 2023-04-28 16:03:14.859920 tpfi-1.0.1/tpfi.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.1/PKG-INFO
```

### Comparing `tpfi-1.0.0/LICENSE` & `tpfi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.0/README.md` & `tpfi-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 two functions: `plot_identification` and `plot_season`. These functions create 
 plots to help visualize target stars and their surrounding environments.
 
 ---
 
 **Plot identification charts for Kepler, K2 and TESS.**
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/kepler.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/kepler.png)
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/k2.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/k2.png)
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/tess.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tess.png)
 
 The `plot_identification` function creates identification charts, which are useful 
 for determining if a target is contaminated by nearby stars. In each chart, the 
 right panel displays the target (marked by a cross symbol) and nearby stars. The 
 circle size indicates their relative brightness. The left panel displays the same 
 sky coverage but from the [DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
 
 This function is revised based on 
 [_tpfplotter_](https://github.com/jlillo/tpfplotter). 
 
 ---
 
 **Plot season charts for Kepler targets.**
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/season.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/season.png)
 
 The `plot_season` function creates a plot of the TPF for each season of the Kepler 
 mission for a given target star. Note that this function is only applicable for 
 Kepler targets.
 
 ## Installation
```

### Comparing `tpfi-1.0.0/tpfi.py` & `tpfi-1.0.1/tpfi.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,40 +132,43 @@
     add_scalebar(ax=ax_sky, pad=0.15, length=1 / x_pixel, scale='{}"'.format(pixel_scale))
 
 
 def plot_tpf(
     ax_tpf: Axes,
     tpf: Union[TessTargetPixelFile, KeplerTargetPixelFile],
     r: Table,
+    cmap: str,
+    c_star: str,
+    c_mask: str,
+    mag_limit: float,
     ax_cb: Axes = None,
-    cmap: str = "viridis",
-    mag_limit: float = None,
 ):
     """
     Plot the identification charts.
 
     Parameters
     ----------
     ax_tpf: `matplotlib.axes.Axes`
         A matplotlib axes object to plot the tpf into
     tpf: `lightkurve.TessTargetPixelFile` or `lightkurve.KeplerTargetPixelFile`
         Target pixel files read by `lightkurve`
     r: `astropy.table.Table`
         The table of the Gaia objects in the area of TPF
-    ax_cb: `matplotlib.axes.Axes`
-        A matplotlib axes object to plot the color bar into
     cmap: str
         The colormap to use
+    c_star: str
+        The color of the stars
+    c_mask: str
+        The color of the pipeline mask
     mag_limit: float
         The magnitude limit (Gaia G mag) to plot the stars in the TPF
+    ax_cb: `matplotlib.axes.Axes`
+        A matplotlib axes object to plot the color bar into
     """
 
-    if mag_limit is None:
-        mag_limit = 18 if tpf.meta["TELESCOP"] == "TESS" else 19.5
-
     # TPF plot
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", RuntimeWarning)
         median_flux = np.nanmedian(tpf.flux.value, axis=0)
 
     try:
         division = int(np.log10(np.nanmax(median_flux)))
@@ -212,25 +215,25 @@
             [target_gaia_mag < 12, 12 <= target_gaia_mag < mag_limit, target_gaia_mag > mag_limit],
             [70, lambda mag: 190 - mag * 10, 10],
         )
         if tpf.meta["TELESCOP"] != "TESS":
             size_k = size_k * 5
         size = size_k / 1.5 ** (gaia_mags - target_gaia_mag)
 
-        ax_tpf.scatter(x, y, s=size, c="red", alpha=0.5, edgecolor=None, zorder=11)
+        ax_tpf.scatter(x, y, s=size, c=c_star, alpha=0.5, edgecolor=None, zorder=11)
         ax_tpf.scatter(x[this], y[this], marker="x", c="white", s=size_k / 2.5, zorder=12)
 
     # Pipeline aperture
     aperture = tpf.pipeline_mask
     aperture_masks = [(i, j) for i in range(aperture.shape[0]) for j in range(aperture.shape[1]) if aperture[i, j]]
     for i, j in aperture_masks:
         xy = (j - 0.5, i - 0.5)
         if aperture[i, j]:
-            ax_tpf.add_patch(patches.Rectangle(xy, 1, 1, color="tomato", fill=True, alpha=0.4))
-            ax_tpf.add_patch(patches.Rectangle(xy, 1, 1, color="tomato", fill=False, alpha=0.6, lw=1.5, zorder=9))
+            ax_tpf.add_patch(patches.Rectangle(xy, 1, 1, color=c_mask, fill=True, alpha=0.4))
+            ax_tpf.add_patch(patches.Rectangle(xy, 1, 1, color=c_mask, fill=False, alpha=0.6, lw=1.5, zorder=9))
         else:
             ax_tpf.add_patch(patches.Rectangle(xy, 1, 1, color="gray", fill=False, alpha=0.2, lw=0.5, zorder=8))
 
     # Add orientation arrows
     theta, reverse = calculate_theta(tpf.wcs.wcs)
     add_orientation(ax=ax_tpf, theta=theta, pad=0.15, color="k", reverse=reverse)
 
@@ -248,14 +251,17 @@
         cb.set_label(r"Flux {} (e$^-$)".format(exponent), fontsize=13)
 
 
 def plot_identification(
     tpf: Union[TessTargetPixelFile, KeplerTargetPixelFile],
     ax: Axes = None,
     mag_limit: float = None,
+    cmap: str = "viridis",
+    c_star: str = "red",
+    c_mask: str = "tomato",
     verbose: bool = False,
 ):
     """
     Plot the identification chart for a given target pixel file (TPF).
 
     The function creates a combined identification chart, including the sky image and
     the TPF with stars' positions, magnitudes, and pipeline aperture.
@@ -265,52 +271,74 @@
     tpf : `lightkurve.TessTargetPixelFile` or `lightkurve.KeplerTargetPixelFile`
         Target pixel files read by `lightkurve`
     ax : `matplotlib.axes.Axes`, optional
         A matplotlib axes object to plot the identification chart into. If not provided, a new figure will be created.
     mag_limit : float, optional
         The magnitude limit (Gaia G mag) to plot the stars in the TPF. If not provided, the default value will be used.
         (18 for TESS, 19.5 for Kepler/K2)
+    cmap : str, optional
+        The colormap to use for the TPF. Default is 'viridis'.
+    c_star: str, optional
+        The color of the stars in the TPF. Default is 'red'.
+    c_mask: str, optional
+        The color of the pipeline mask in the TPF. Default is 'tomato'.
     verbose : bool, optional
         Whether to print out progress messages. Default is False.
 
     Returns
     -------
     ax : `matplotlib.axes.Axes`
         The matplotlib axes object.
     """
 
     if ax is None:
         _, ax = plt.subplots(figsize=(9, 4))
 
+    if mag_limit is None:
+        mag_limit = 18 if tpf.meta["TELESCOP"] == "TESS" else 19.5
+
     divider = make_axes_locatable(ax)
     ax_tpf = divider.append_axes("right", size="100%", pad=0.1)
     ax_cb = divider.append_axes("right", size="8%", pad=0.35)
 
     plot_sky(ax, tpf, verbose)
 
     r = query_nearby_gaia_objects(tpf, verbose=verbose)
-    plot_tpf(ax_tpf, tpf, r, ax_cb=ax_cb, mag_limit=mag_limit)
+    plot_tpf(ax_tpf, tpf, r, cmap, c_star, c_mask, ax_cb=ax_cb, mag_limit=mag_limit)
 
 
-def plot_season(label: str, ax: Axes = None, mag_limit: float = None, verbose: bool = False):
+def plot_season(
+    label: str,
+    ax: Axes = None,
+    mag_limit: float = 19.5,
+    cmap: str = "gray_r",
+    c_star: str = "red",
+    c_mask: str = "tomato",
+    verbose: bool = False,
+):
     """
     Plot identification charts for different seasons of an astronomical object using data from the Kepler mission.
 
     The function searches for the target pixel files (TPFs) from the Kepler mission for different seasons
     and creates identification charts for each season, showing the sky image and TPFs.
 
     Parameters
     ----------
     label : str
         The label of the astronomical object to be searched for in the Kepler mission.
     ax : `matplotlib.axes.Axes`, optional
         A matplotlib axes object to plot the identification charts into. If not provided, a new figure will be created.
     mag_limit : float, optional
-        The magnitude limit (Gaia G mag) to plot the stars in the TPF. If not provided, the default value will be used.
-        (18 for TESS, 19.5 for Kepler/K2)
+        The magnitude limit (Gaia G mag) to plot the stars in the TPF. Default is 19.5.
+    c_star: str, optional
+        The color of the stars in the TPFs. Default is 'red'.
+    c_mask: str, optional
+        The color of the pipeline mask in the TPFs. Default is 'tomato'.
+    cmap : str, optional
+        The colormap to use for the TPF. Default is 'gray_r'.
     verbose : bool, optional
         Whether to print out progress messages. Default is False.
 
     Returns
     -------
     ax : `matplotlib.axes.Axes`
         The matplotlib axes object.
@@ -367,12 +395,12 @@
         ax_list.append(divider.append_axes("right", size=f"{percent}%", pad=0.1))
 
     plot_sky(ax, tpf_list[max_index], verbose)
 
     r = query_nearby_gaia_objects(tpf_list[max_index], verbose=verbose)
     for i, tpf in enumerate(tpf_list):
         if tpf is not None:
-            plot_tpf(ax_list[i], tpf_list[i], r, cmap="gray_r", mag_limit=mag_limit)
+            plot_tpf(ax_list[i], tpf_list[i], r, cmap, c_star, c_mask, mag_limit)
             at = AnchoredText(f"Season {i + 1}", frameon=False, loc="upper left", prop=dict(size=13), zorder=100)
             ax_list[i].add_artist(at)
         ax_list[i].set_xticks([])
         ax_list[i].set_yticks([])
```

### Comparing `tpfi-1.0.0/PKG-INFO` & `tpfi-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -26,34 +26,34 @@
 two functions: `plot_identification` and `plot_season`. These functions create 
 plots to help visualize target stars and their surrounding environments.
 
 ---
 
 **Plot identification charts for Kepler, K2 and TESS.**
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/kepler.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/kepler.png)
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/k2.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/k2.png)
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/tess.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tess.png)
 
 The `plot_identification` function creates identification charts, which are useful 
 for determining if a target is contaminated by nearby stars. In each chart, the 
 right panel displays the target (marked by a cross symbol) and nearby stars. The 
 circle size indicates their relative brightness. The left panel displays the same 
 sky coverage but from the [DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
 
 This function is revised based on 
 [_tpfplotter_](https://github.com/jlillo/tpfplotter). 
 
 ---
 
 **Plot season charts for Kepler targets.**
 
-![alt text](https://github.com/keyuxing/tpfi/blob/main/examples/season.png)
+![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/season.png)
 
 The `plot_season` function creates a plot of the TPF for each season of the Kepler 
 mission for a given target star. Note that this function is only applicable for 
 Kepler targets.
 
 ## Installation
```

