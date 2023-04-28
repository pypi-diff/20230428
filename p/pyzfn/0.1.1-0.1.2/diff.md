# Comparing `tmp/pyzfn-0.1.1.tar.gz` & `tmp/pyzfn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzfn-0.1.1.tar", last modified: Wed Mar 22 16:06:06 2023, max compression
+gzip compressed data, was "pyzfn-0.1.2.tar", last modified: Fri Apr 28 13:03:44 2023, max compression
```

## Comparing `pyzfn-0.1.1.tar` & `pyzfn-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-03-22 16:06:06.506210 pyzfn-0.1.1/
--rw-r--r--   0 mat       (1000) mat       (1000)    35149 2022-11-21 13:47:16.000000 pyzfn-0.1.1/LICENSE
--rw-r--r--   0 mat       (1000) mat       (1000)      538 2023-03-22 16:06:06.506210 pyzfn-0.1.1/PKG-INFO
--rw-r--r--   0 mat       (1000) mat       (1000)     1597 2023-03-15 11:37:32.000000 pyzfn-0.1.1/README.md
--rw-r--r--   0 mat       (1000) mat       (1000)      631 2022-12-07 14:31:13.000000 pyzfn-0.1.1/pyproject.toml
-drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-03-22 16:06:06.506210 pyzfn-0.1.1/pyzfn/
--rw-r--r--   0 mat       (1000) mat       (1000)      112 2023-01-31 23:02:37.000000 pyzfn-0.1.1/pyzfn/__init__.py
--rw-r--r--   0 mat       (1000) mat       (1000)     3757 2023-03-07 09:22:31.000000 pyzfn-0.1.1/pyzfn/equations.py
--rw-r--r--   0 mat       (1000) mat       (1000)        0 2022-12-05 13:22:21.000000 pyzfn-0.1.1/pyzfn/py.typed
--rw-r--r--   0 mat       (1000) mat       (1000)    16922 2023-03-21 16:21:45.000000 pyzfn-0.1.1/pyzfn/pyzfn.py
--rw-r--r--   0 mat       (1000) mat       (1000)     9454 2023-03-21 15:56:44.000000 pyzfn-0.1.1/pyzfn/utils.py
-drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-03-22 16:06:06.506210 pyzfn-0.1.1/pyzfn.egg-info/
--rw-r--r--   0 mat       (1000) mat       (1000)      538 2023-03-22 16:06:06.000000 pyzfn-0.1.1/pyzfn.egg-info/PKG-INFO
--rw-r--r--   0 mat       (1000) mat       (1000)      345 2023-03-22 16:06:06.000000 pyzfn-0.1.1/pyzfn.egg-info/SOURCES.txt
--rw-r--r--   0 mat       (1000) mat       (1000)        1 2023-03-22 16:06:06.000000 pyzfn-0.1.1/pyzfn.egg-info/dependency_links.txt
--rw-r--r--   0 mat       (1000) mat       (1000)        1 2022-12-06 07:55:22.000000 pyzfn-0.1.1/pyzfn.egg-info/not-zip-safe
--rw-r--r--   0 mat       (1000) mat       (1000)      218 2023-03-22 16:06:06.000000 pyzfn-0.1.1/pyzfn.egg-info/requires.txt
--rw-r--r--   0 mat       (1000) mat       (1000)        6 2023-03-22 16:06:06.000000 pyzfn-0.1.1/pyzfn.egg-info/top_level.txt
--rw-r--r--   0 mat       (1000) mat       (1000)      916 2023-03-22 16:06:06.506210 pyzfn-0.1.1/setup.cfg
--rw-r--r--   0 mat       (1000) mat       (1000)       69 2022-12-05 12:05:38.000000 pyzfn-0.1.1/setup.py
-drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-03-22 16:06:06.506210 pyzfn-0.1.1/tests/
--rw-r--r--   0 mat       (1000) mat       (1000)      919 2022-12-09 10:48:57.000000 pyzfn-0.1.1/tests/test_pyzfn.py
--rw-r--r--   0 mat       (1000) mat       (1000)     2341 2022-12-09 08:30:03.000000 pyzfn-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-04-28 13:03:44.705908 pyzfn-0.1.2/
+-rw-r--r--   0 mat       (1000) mat       (1000)    35149 2022-11-21 13:47:16.000000 pyzfn-0.1.2/LICENSE
+-rw-r--r--   0 mat       (1000) mat       (1000)      538 2023-04-28 13:03:44.705908 pyzfn-0.1.2/PKG-INFO
+-rw-r--r--   0 mat       (1000) mat       (1000)     1597 2023-03-15 11:37:32.000000 pyzfn-0.1.2/README.md
+-rw-r--r--   0 mat       (1000) mat       (1000)      631 2022-12-07 14:31:13.000000 pyzfn-0.1.2/pyproject.toml
+drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-04-28 13:03:44.705908 pyzfn-0.1.2/pyzfn/
+-rw-r--r--   0 mat       (1000) mat       (1000)      112 2023-01-31 23:02:37.000000 pyzfn-0.1.2/pyzfn/__init__.py
+-rw-r--r--   0 mat       (1000) mat       (1000)     3757 2023-03-07 09:22:31.000000 pyzfn-0.1.2/pyzfn/equations.py
+-rw-r--r--   0 mat       (1000) mat       (1000)        0 2022-12-05 13:22:21.000000 pyzfn-0.1.2/pyzfn/py.typed
+-rw-r--r--   0 mat       (1000) mat       (1000)    17346 2023-04-28 13:01:28.000000 pyzfn-0.1.2/pyzfn/pyzfn.py
+-rw-r--r--   0 mat       (1000) mat       (1000)     9620 2023-04-28 12:59:33.000000 pyzfn-0.1.2/pyzfn/utils.py
+drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-04-28 13:03:44.705908 pyzfn-0.1.2/pyzfn.egg-info/
+-rw-r--r--   0 mat       (1000) mat       (1000)      538 2023-04-28 13:03:44.000000 pyzfn-0.1.2/pyzfn.egg-info/PKG-INFO
+-rw-r--r--   0 mat       (1000) mat       (1000)      345 2023-04-28 13:03:44.000000 pyzfn-0.1.2/pyzfn.egg-info/SOURCES.txt
+-rw-r--r--   0 mat       (1000) mat       (1000)        1 2023-04-28 13:03:44.000000 pyzfn-0.1.2/pyzfn.egg-info/dependency_links.txt
+-rw-r--r--   0 mat       (1000) mat       (1000)        1 2022-12-06 07:55:22.000000 pyzfn-0.1.2/pyzfn.egg-info/not-zip-safe
+-rw-r--r--   0 mat       (1000) mat       (1000)      218 2023-04-28 13:03:44.000000 pyzfn-0.1.2/pyzfn.egg-info/requires.txt
+-rw-r--r--   0 mat       (1000) mat       (1000)        6 2023-04-28 13:03:44.000000 pyzfn-0.1.2/pyzfn.egg-info/top_level.txt
+-rw-r--r--   0 mat       (1000) mat       (1000)      916 2023-04-28 13:03:44.705908 pyzfn-0.1.2/setup.cfg
+-rw-r--r--   0 mat       (1000) mat       (1000)       69 2022-12-05 12:05:38.000000 pyzfn-0.1.2/setup.py
+drwxr-xr-x   0 mat       (1000) mat       (1000)        0 2023-04-28 13:03:44.705908 pyzfn-0.1.2/tests/
+-rw-r--r--   0 mat       (1000) mat       (1000)      919 2023-04-28 12:56:46.000000 pyzfn-0.1.2/tests/test_pyzfn.py
+-rw-r--r--   0 mat       (1000) mat       (1000)     2341 2023-04-28 12:56:46.000000 pyzfn-0.1.2/tests/test_utils.py
```

### Comparing `pyzfn-0.1.1/LICENSE` & `pyzfn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.1/PKG-INFO` & `pyzfn-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzfn
-Version: 0.1.1
+Version: 0.1.2
 Summary: micromagnetic post processing library
 Author: Mathieu Moalic
 License: GPL-3.0
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pyzfn-0.1.1/README.md` & `pyzfn-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.1/pyproject.toml` & `pyzfn-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.1/pyzfn/equations.py` & `pyzfn-0.1.2/pyzfn/equations.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.1/pyzfn/pyzfn.py` & `pyzfn-0.1.2/pyzfn/pyzfn.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,25 @@
         if not os.path.exists(path):
             raise FileNotFoundError(f"Path Not Found : '{path}'")
         self.z: zarr.Group = zarr.open(path)
         self.path: Path = Path(path).absolute()
         self.name: str = self.path.name.replace(self.path.suffix, "")
 
     def __getitem__(self, item: str) -> Union[zarr.Array, zarr.Group]:
-        return self.z[item]
+        if item in dir(self):
+            return getattr(self, item)
+        if item in dir(self.z):
+            return getattr(self.z, item)
+        if item in self.z.attrs:
+            return self.z.attrs[item]
+        else:
+            raise NameError
+
+    def __setitem__(self, key: str, value: str) -> None:
+        self.z[key] = value
 
     def __getattr__(self, name: str) -> Union[zarr.Array, zarr.Group, int, float, str]:
         if name in dir(self):
             return getattr(self, name)
         if name in dir(self.z):
             return getattr(self.z, name)
         if name in self.z.attrs:
@@ -117,20 +127,23 @@
             arr,
             axes=(1, 0),
             threads=mp.cpu_count() // 2,
             planner_effort="FFTW_ESTIMATE",
             avoid_copy=True,
         )
         save_wisdom(arr)
+        ychuncks = dset_in.chunks[2]
         for iy in trange(
-            dset_in.shape[2] // dset_in.chunks[2],
+            dset_in.shape[2] // ychuncks - 1,
             leave=False,
             desc=f"Calculating the dispersion for `{self.name}`",
         ):
-            arr[:] = dset_in[1:, 0, iy, 1:, :]
+            arr[:] = np.sum(
+                dset_in[1:, 0, iy * ychuncks : (iy + 1) * ychuncks, 1:, :], axis=2
+            )
             arr *= hann2d
             out = fft()
             out -= np.average(out, axis=(0, 1))[None, None, :]
             out = out[: out.shape[0] // 2]
             out = np.fft.fftshift(out, axes=(1, 2))
             arr_out[:] += np.abs(out[: arr_out.shape[0]])
             if single_y:
```

### Comparing `pyzfn-0.1.1/pyzfn/utils.py` & `pyzfn-0.1.2/pyzfn/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,20 +179,27 @@
             tmp_list[chunk_nb].append(pt)
         for sublist in tmp_list:
             out[i].append(slice(min(sublist), max(sublist) + 1, sl.step))
     return out
 
 
 def load_mpl_style(skip_style: bool = False) -> None:
-    ipy = IPython.get_ipython()  # type: ignore
+    ipy = IPython.get_ipython()
     if ipy is not None:
         ipy.run_cell_magic(
             "html",
             "",
-            "<style> .cell-output-ipywidget-background {background-color: transparent !important;}</style>",
+            """<style>
+                .cell-output-ipywidget-background {
+                    background-color: transparent !important;
+                }
+                .jupyter-matplotlib-footer {
+                    color: white !important;
+                }
+               </style>""",
         )
         ipy.run_line_magic("matplotlib", "widget")
         ipy.run_line_magic("load_ext", "autoreload")
         ipy.run_line_magic("autoreload", "2")
 
         plt.rcParams["figure.max_open_warning"] = 1000
```

### Comparing `pyzfn-0.1.1/pyzfn.egg-info/PKG-INFO` & `pyzfn-0.1.2/pyzfn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzfn
-Version: 0.1.1
+Version: 0.1.2
 Summary: micromagnetic post processing library
 Author: Mathieu Moalic
 License: GPL-3.0
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pyzfn-0.1.1/setup.cfg` & `pyzfn-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyzfn
-version = 0.1.1
+version = 0.1.2
 description = micromagnetic post processing library
 author = Mathieu Moalic
 license = GPL-3.0
 license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `pyzfn-0.1.1/tests/test_pyzfn.py` & `pyzfn-0.1.2/tests/test_pyzfn.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.1/tests/test_utils.py` & `pyzfn-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

