# Comparing `tmp/dreamai-0.2.0.tar.gz` & `tmp/dreamai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.2.0.tar", last modified: Thu Feb  9 00:49:39 2023, max compression
+gzip compressed data, was "dreamai-0.3.0.tar", last modified: Fri Apr 28 13:07:12 2023, max compression
```

## Comparing `dreamai-0.2.0.tar` & `dreamai-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-02-09 00:49:39.553859 dreamai-0.2.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.2.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.2.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-02-09 00:49:39.553859 dreamai-0.2.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-01-18 23:32:17.000000 dreamai-0.2.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-02-09 00:49:39.553859 dreamai-0.2.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-02-09 00:49:32.000000 dreamai-0.2.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8115 2023-02-09 00:47:04.000000 dreamai-0.2.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8603 2023-02-09 00:47:04.000000 dreamai-0.2.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      632 2023-01-27 20:54:39.000000 dreamai-0.2.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8032 2023-02-09 00:47:04.000000 dreamai-0.2.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-02-09 00:49:39.553859 dreamai-0.2.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.2.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      512 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-02-09 00:49:39.000000 dreamai-0.2.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1172 2023-02-09 00:49:32.000000 dreamai-0.2.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-02-09 00:49:39.553859 dreamai-0.2.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.2.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:07:12.265403 dreamai-0.3.0/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.3.0/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.3.0/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-04-28 13:07:12.265403 dreamai-0.3.0/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-01-18 23:32:17.000000 dreamai-0.3.0/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:07:12.265403 dreamai-0.3.0/dreamai/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-04-28 13:07:05.000000 dreamai-0.3.0/dreamai/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8319 2023-04-28 13:07:05.000000 dreamai-0.3.0/dreamai/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8796 2023-04-28 13:07:05.000000 dreamai-0.3.0/dreamai/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      632 2023-01-27 20:54:39.000000 dreamai-0.3.0/dreamai/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8283 2023-04-28 13:07:05.000000 dreamai-0.3.0/dreamai/vision.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-04-28 13:07:12.265403 dreamai-0.3.0/dreamai.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.3.0/dreamai.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      512 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-04-28 13:07:12.000000 dreamai-0.3.0/dreamai.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1172 2023-04-28 13:07:02.000000 dreamai-0.3.0/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-04-28 13:07:12.265403 dreamai-0.3.0/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.3.0/setup.py
```

### Comparing `dreamai-0.2.0/LICENSE` & `dreamai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai-0.2.0/PKG-INFO` & `dreamai-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.2.0/dreamai/_modidx.py` & `dreamai-0.3.0/dreamai/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/dreamai',
                 'doc_host': 'https://HamzaFarhan.github.io',
                 'git_url': 'https://github.com/HamzaFarhan/dreamai',
                 'lib_path': 'dreamai'},
   'syms': { 'dreamai.core': { 'dreamai.core._get_files': ('core.html#_get_files', 'dreamai/core.py'),
-                              'dreamai.core.add_ext_to_path': ('core.html#add_ext_to_path', 'dreamai/core.py'),
                               'dreamai.core.default_device': ('core.html#default_device', 'dreamai/core.py'),
                               'dreamai.core.dict_keys': ('core.html#dict_keys', 'dreamai/core.py'),
                               'dreamai.core.dict_values': ('core.html#dict_values', 'dreamai/core.py'),
                               'dreamai.core.end_of_path': ('core.html#end_of_path', 'dreamai/core.py'),
                               'dreamai.core.extend_path_name': ('core.html#extend_path_name', 'dreamai/core.py'),
                               'dreamai.core.filter_dict': ('core.html#filter_dict', 'dreamai/core.py'),
                               'dreamai.core.flatten_list': ('core.html#flatten_list', 'dreamai/core.py'),
                               'dreamai.core.get_files': ('core.html#get_files', 'dreamai/core.py'),
                               'dreamai.core.is_array': ('core.html#is_array', 'dreamai/core.py'),
                               'dreamai.core.is_clip': ('core.html#is_clip', 'dreamai/core.py'),
                               'dreamai.core.is_df': ('core.html#is_df', 'dreamai/core.py'),
                               'dreamai.core.is_dict': ('core.html#is_dict', 'dreamai/core.py'),
                               'dreamai.core.is_float': ('core.html#is_float', 'dreamai/core.py'),
                               'dreamai.core.is_frozen': ('core.html#is_frozen', 'dreamai/core.py'),
+                              'dreamai.core.is_img': ('core.html#is_img', 'dreamai/core.py'),
                               'dreamai.core.is_int': ('core.html#is_int', 'dreamai/core.py'),
                               'dreamai.core.is_iter': ('core.html#is_iter', 'dreamai/core.py'),
                               'dreamai.core.is_list': ('core.html#is_list', 'dreamai/core.py'),
                               'dreamai.core.is_norm': ('core.html#is_norm', 'dreamai/core.py'),
                               'dreamai.core.is_path': ('core.html#is_path', 'dreamai/core.py'),
                               'dreamai.core.is_pilimage': ('core.html#is_pilimage', 'dreamai/core.py'),
                               'dreamai.core.is_sequential': ('core.html#is_sequential', 'dreamai/core.py'),
@@ -47,14 +47,15 @@
                               'dreamai.core.params': ('core.html#params', 'dreamai/core.py'),
                               'dreamai.core.path_name': ('core.html#path_name', 'dreamai/core.py'),
                               'dreamai.core.path_or_str': ('core.html#path_or_str', 'dreamai/core.py'),
                               'dreamai.core.path_stem': ('core.html#path_stem', 'dreamai/core.py'),
                               'dreamai.core.path_suffix': ('core.html#path_suffix', 'dreamai/core.py'),
                               'dreamai.core.proc_fn': ('core.html#proc_fn', 'dreamai/core.py'),
                               'dreamai.core.replace_dict_key': ('core.html#replace_dict_key', 'dreamai/core.py'),
+                              'dreamai.core.resolve_data_path': ('core.html#resolve_data_path', 'dreamai/core.py'),
                               'dreamai.core.save_obj': ('core.html#save_obj', 'dreamai/core.py'),
                               'dreamai.core.set_pip_req': ('core.html#set_pip_req', 'dreamai/core.py'),
                               'dreamai.core.setify': ('core.html#setify', 'dreamai/core.py'),
                               'dreamai.core.sort_dict': ('core.html#sort_dict', 'dreamai/core.py'),
                               'dreamai.core.yml_to_pip': ('core.html#yml_to_pip', 'dreamai/core.py')},
             'dreamai.imports': {},
             'dreamai.vision': { 'dreamai.vision.add_alpha': ('vision.html#add_alpha', 'dreamai/vision.py'),
@@ -73,11 +74,12 @@
                                 'dreamai.vision.plt_show': ('vision.html#plt_show', 'dreamai/vision.py'),
                                 'dreamai.vision.remove_images': ('vision.html#remove_images', 'dreamai/vision.py'),
                                 'dreamai.vision.rgb2bgr': ('vision.html#rgb2bgr', 'dreamai/vision.py'),
                                 'dreamai.vision.rgb2gray': ('vision.html#rgb2gray', 'dreamai/vision.py'),
                                 'dreamai.vision.rgb2rgba': ('vision.html#rgb2rgba', 'dreamai/vision.py'),
                                 'dreamai.vision.rgb_read': ('vision.html#rgb_read', 'dreamai/vision.py'),
                                 'dreamai.vision.rgba2rgb': ('vision.html#rgba2rgb', 'dreamai/vision.py'),
+                                'dreamai.vision.show_img': ('vision.html#show_img', 'dreamai/vision.py'),
                                 'dreamai.vision.solid_color_img': ('vision.html#solid_color_img', 'dreamai/vision.py'),
                                 'dreamai.vision.solid_color_img_like': ('vision.html#solid_color_img_like', 'dreamai/vision.py'),
                                 'dreamai.vision.tensor_to_img': ('vision.html#tensor_to_img', 'dreamai/vision.py'),
                                 'dreamai.vision.to_pil': ('vision.html#to_pil', 'dreamai/vision.py')}}}
```

### Comparing `dreamai-0.2.0/dreamai/core.py` & `dreamai-0.3.0/dreamai/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['default_device', 'flatten_list', 'noop', 'is_list', 'is_tuple', 'list_or_tuple', 'is_iter', 'is_dict', 'is_df',
-           'is_str', 'is_int', 'is_float', 'is_array', 'is_pilimage', 'is_tensor', 'is_set', 'is_path', 'path_or_str',
-           'is_norm', 'params', 'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_sequential', 'is_clip', 'path_name',
-           'path_stem', 'path_suffix', 'extend_path_name', 'end_of_path', 'add_ext_to_path', 'last_modified',
-           'load_yaml', 'save_obj', 'load_obj', 'yml_to_pip', 'set_pip_req', 'merge_dicts', 'dict_values', 'dict_keys',
-           'sort_dict', 'locals_to_params', 'list_map', 'next_batch', 'model_children', 'replace_dict_key', 'proc_fn',
-           'filter_dict', 'setify', 'get_files']
+           'is_str', 'is_int', 'is_float', 'is_array', 'is_pilimage', 'is_img', 'is_tensor', 'is_set', 'is_path',
+           'path_or_str', 'is_norm', 'params', 'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_sequential',
+           'is_clip', 'path_name', 'path_stem', 'path_suffix', 'extend_path_name', 'end_of_path', 'last_modified',
+           'load_yaml', 'save_obj', 'load_obj', 'resolve_data_path', 'yml_to_pip', 'set_pip_req', 'merge_dicts',
+           'dict_values', 'dict_keys', 'sort_dict', 'locals_to_params', 'list_map', 'next_batch', 'model_children',
+           'replace_dict_key', 'proc_fn', 'filter_dict', 'setify', 'get_files']
 
 # %% ../nbs/00_core.ipynb 3
 from .imports import *
 
 # %% ../nbs/00_core.ipynb 4
 def default_device(device=None):
     if device is None:
@@ -63,14 +63,17 @@
 
 def is_array(x):
     return isinstance(x, np.ndarray)
 
 def is_pilimage(x):
     return 'PIL' in str(type(x))
 
+def is_img(x):
+    return is_array(x) or is_pilimage(x)
+
 def is_tensor(x):
     return isinstance(x, torch.Tensor)
 
 def is_set(x):
     return isinstance(x, set)
 
 def is_path(x):
@@ -119,26 +122,14 @@
     "Get the last `n` parts of a path `p`."
     parts = p.parts
     p = Path(parts[-n])
     for i in range(-(n-1), 0):
         p/=parts[i]
     return p
 
-def add_ext_to_path(p, ext='pkl'):
-    "Add an extension to a path `p` if it doesn't have one."
-    if ext[0] != '.':
-        ext = '.'+ext
-    if len(Path(p).suffix) == 0:
-        p = str(p)
-        if p[-1] != '.':
-            p+=ext
-        else:
-            p+=ext[1:]
-    return p
-
 def last_modified(x):
     "Get the last modified time of a file."
     return x.stat().st_ctime
 
 def load_yaml(file):
     with open(file) as f:
         env = load(f, Loader=Loader)
@@ -147,14 +138,28 @@
 def save_obj(path, obj):
     with open(path, 'wb') as f:
         pickle.dump(obj, f, pickle.HIGHEST_PROTOCOL)
 
 def load_obj(path):
     with open(path, 'rb') as f:
         return pickle.load(f)
+
+def resolve_data_path(data_path):
+    if not is_list(data_path): data_path = [data_path]
+    data_path = flatten_list(data_path)
+    paths = []
+    for dp in data_path:
+        dp = Path(dp)
+        if not dp.exists():
+            raise Exception(f'Path {dp} does not exist.')
+        if dp.is_dir():
+            paths.append(dp.iterdir())
+        else:
+            paths.append([dp])
+    return chain(*paths)
     
 def yml_to_pip(yml, remove_eq=True):
     "Get pip packages from a conda environment `yml` file."
     env = load_yaml(yml)
     env_pip = env['dependencies'][-1]['pip']
     pip_list = []
     for x in env_pip:
```

### Comparing `dreamai-0.2.0/dreamai/imports.py` & `dreamai-0.3.0/dreamai/imports.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.2.0/dreamai/vision.py` & `dreamai-0.3.0/dreamai/vision.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_vision.ipynb.
 
 # %% auto 0
 __all__ = ['image_extensions', 'remove_images', 'bgr2rgb', 'rgb2bgr', 'gray2rgb', 'rgb2gray', 'rgb2rgba', 'bgra2rgb', 'rgba2rgb',
-           'rgb_read', 'c1_read', 'tensor_to_img', 'plt_show', 'get_hw', 'get_image_files', 'to_pil', 'add_alpha',
-           'has_alpha', 'color_to_rgb', 'solid_color_img', 'solid_color_img_like', 'get_pos_factors', 'get_pos_',
-           'get_pos', 'paste_img']
+           'rgb_read', 'c1_read', 'tensor_to_img', 'plt_show', 'show_img', 'get_hw', 'get_image_files', 'to_pil',
+           'add_alpha', 'has_alpha', 'color_to_rgb', 'solid_color_img', 'solid_color_img_like', 'get_pos_factors',
+           'get_pos_', 'get_pos', 'paste_img']
 
 # %% ../nbs/01_vision.ipynb 3
 from .imports import *
 from .core import *
 
 # %% ../nbs/01_vision.ipynb 4
 image_extensions = {'.art','.bmp','.cdr','.cdt','.cpt','.cr2','.crw','.djv','.djvu','.erf','.gif','.ico',
@@ -74,14 +74,21 @@
         im = tensor_to_img(im)
         if is_list(im): im = im[0]
     fig=plt.figure(figsize=figsize)
     plt.imshow(im, cmap=cmap)
     plt.title(title)
     plt.show()
 
+def show_img(img, cmap=None, title='', figsize=(7,7)):
+    if path_or_str(img):
+        imgs = resolve_data_path(img)
+    elif is_img(img):
+        imgs = [img]
+    [plt_show(img, cmap=cmap, title=title, figsize=figsize) for img in imgs]
+
 def get_hw(x):
     "Return the height and width of `x`."
     if is_clip(x):
         return x.size[1], x.size[0]
     return np.array(x).shape[:2]
 
 def get_image_files(path, recurse=True, folders=None,
```

### Comparing `dreamai-0.2.0/dreamai.egg-info/PKG-INFO` & `dreamai-0.3.0/dreamai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.2.0/dreamai.egg-info/requires.txt` & `dreamai-0.3.0/dreamai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dreamai-0.2.0/settings.ini` & `dreamai-0.3.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai
 lib_name = %(repo)s
-version = 0.2.0
+version = 0.3.0
 min_python = 3.8
 license = apache2
 doc_path = _docs
 lib_path = dreamai
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `dreamai-0.2.0/setup.py` & `dreamai-0.3.0/setup.py`

 * *Files identical despite different names*

