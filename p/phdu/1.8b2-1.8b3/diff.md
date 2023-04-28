# Comparing `tmp/phdu-1.8b2.tar.gz` & `tmp/phdu-1.8b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-1.8b2.tar", last modified: Tue Apr 25 11:09:02 2023, max compression
+gzip compressed data, was "phdu-1.8b3.tar", last modified: Fri Apr 28 14:31:31 2023, max compression
```

## Comparing `phdu-1.8b2.tar` & `phdu-1.8b3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.918442 phdu-1.8b2/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-1.8b2/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-25 11:09:02.918442 phdu-1.8b2/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-1.8b2/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.846439 phdu-1.8b2/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-1.8b2/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-1.8b2/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-1.8b2/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-1.8b2/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-1.8b2/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-1.8b2/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.878440 phdu-1.8b2/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-1.8b2/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-1.8b2/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-1.8b2/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    13684 2023-04-25 09:22:33.000000 phdu-1.8b2/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-1.8b2/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.898441 phdu-1.8b2/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-1.8b2/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-1.8b2/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-1.8b2/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-1.8b2/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    27792 2023-04-25 08:51:16.000000 phdu-1.8b2/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-1.8b2/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-1.8b2/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.906442 phdu-1.8b2/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-1.8b2/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-1.8b2/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-1.8b2/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.914442 phdu-1.8b2/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-1.8b2/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-1.8b2/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-1.8b2/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-1.8b2/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 11:09:02.866440 phdu-1.8b2/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-04-25 11:09:02.000000 phdu-1.8b2/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-04-25 11:09:02.000000 phdu-1.8b2/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-25 11:09:02.000000 phdu-1.8b2/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-04-25 11:09:02.000000 phdu-1.8b2/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-04-25 11:09:02.000000 phdu-1.8b2/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-25 11:09:02.926442 phdu-1.8b2/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-04-25 11:08:53.000000 phdu-1.8b2/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-01-19 11:17:18.000000 phdu-1.8b3/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-04-28 14:31:31.040145 phdu-1.8b3/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-03-22 15:47:48.000000 phdu-1.8b3/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      486 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      608 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2828 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2628 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5912 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3359 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    14203 2023-04-28 14:30:33.000000 phdu-1.8b3/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-04-28 14:15:26.000000 phdu-1.8b3/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    27792 2023-04-19 09:32:30.000000 phdu-1.8b3/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.040145 phdu-1.8b3/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-01-19 11:17:18.000000 phdu-1.8b3/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-03-22 15:47:48.000000 phdu-1.8b3/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4179 2023-04-28 14:15:26.000000 phdu-1.8b3/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-28 14:31:31.036811 phdu-1.8b3/phdu.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      752 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        5 2023-04-28 14:31:30.000000 phdu-1.8b3/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-28 14:31:31.040145 phdu-1.8b3/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1660 2023-04-28 14:30:59.000000 phdu-1.8b3/setup.py
```

### Comparing `phdu-1.8b2/LICENSE.md` & `phdu-1.8b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/PKG-INFO` & `phdu-1.8b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.8b2
+Version: 1.8b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.8b2/README.md` & `phdu-1.8b3/README.md`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/_helper.py` & `phdu-1.8b3/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/clustering.py` & `phdu-1.8b3/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/decomposition.py` & `phdu-1.8b3/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/np_utils.py` & `phdu-1.8b3/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/pd_utils.py` & `phdu-1.8b3/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/plots/base.py` & `phdu-1.8b3/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/plots/plotly_utils.py` & `phdu-1.8b3/phdu/plots/plotly_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,24 +74,45 @@
 mod_expfmt           = get_mod_layout("exponentformat", "power")
 mod_range            = get_mod_layout("range")
 mod_logaxes_expfmt   = lambda fig, axes=["x", "y"]: {**mod_logaxes(fig, axes=axes), **mod_expfmt(fig, axes=axes)}
 
 def mod_common_range(fig, axes=["x", "y"], **kwargs):
     return mod_range(fig, val=get_common_range(fig, axes=axes, **kwargs), axes=axes)
 
+def fig_base_layout(**kwargs):
+    base = dict(margin=dict(l=100, r=20, b=80, t=20, pad=1),
+                height=800, width=1000, yaxis=dict(tickfont_size=32),
+                xaxis=dict(tickfont_size=32), font_size=40, legend_font_size=40,
+                font_family="sans-serif", hovermode=False
+                )
+    base.update(kwargs)
+    return base
+
 def get_figure(height=800, width=1000, ticksize=32, font_size=40, margin=None, font_family="sans-serif", hovermode=False, delete_axes=False, **kwargs):
-    fig = go.Figure(layout=dict(margin=dict(l=100, r=20, b=80, t=20, pad=1) if margin is None else margin,
-                                height=height, width=width, yaxis=dict(tickfont_size=ticksize),
-                                xaxis=dict(tickfont_size=ticksize), font_size=font_size, legend_font_size=font_size,
-                                font_family=font_family, hovermode=hovermode,
-                                **kwargs))
+    args = locals()
+    del args['kwargs']
+    del args['delete_axes']
+    args.update(kwargs)
+
+    fig = go.Figure(layout=fig_base_layout(**args))
     if delete_axes:
         fig.update_layout(**mod_delete_axes(fig), margin=dict(l=0, t=0, b=0, r=0), paper_bgcolor="rgba(0,0,0,0)", plot_bgcolor="rgba(0,0,0,0)")
     return fig
 
+def subplots_base_layout(cols, rows=1, make_subplots_kwargs={}, **layout_kwargs):
+    layout = dict(margin=dict(l=100, r=20, b=80, t=60, pad=1), height=800*rows, width=2500)
+    layout.update(layout_kwargs)
+
+    base = dict(layout=layout,
+                shared_yaxes=True, shared_xaxes=True,
+                horizontal_spacing=0.03, vertical_spacing=0.03, rows=rows, cols=cols,
+                )
+    base.update(make_subplots_kwargs)
+    return base
+
 def get_subplots(cols, rows=1, horizontal_spacing=0.03, vertical_spacing=0.03, height=None, width=2500, ticksize=32, font_size=40, font_family="sans-serif",
                  hovermode=False, delete_axes=False, shared_xaxes=True, shared_yaxes=True, layout_kwargs={},
                  **make_subplots_kwargs):
     height = 800*rows if height is None else height
     fig = make_subplots(figure=go.Figure(layout=dict(margin=dict(l=100, r=20, b=80, t=60, pad=1), height=height, width=width)),
                         shared_yaxes=shared_yaxes, shared_xaxes=shared_xaxes,
                         horizontal_spacing=horizontal_spacing, vertical_spacing=vertical_spacing, rows=rows, cols=cols,
```

### Comparing `phdu-1.8b2/phdu/script_fmt.py` & `phdu-1.8b3/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/_integration.py` & `phdu-1.8b3/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/_plots.py` & `phdu-1.8b3/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/bootstrap.py` & `phdu-1.8b3/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/conf_interval.py` & `phdu-1.8b3/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/corr.py` & `phdu-1.8b3/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/rtopy/_helper.py` & `phdu-1.8b3/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/rtopy/resample.py` & `phdu-1.8b3/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/stats/test/permutation.py` & `phdu-1.8b3/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu/storage.py` & `phdu-1.8b3/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/phdu.egg-info/PKG-INFO` & `phdu-1.8b3/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 1.8b2
+Version: 1.8b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-1.8b2/phdu.egg-info/SOURCES.txt` & `phdu-1.8b3/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-1.8b2/setup.py` & `phdu-1.8b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='1.8.b2',
+    version='1.8.b3',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

