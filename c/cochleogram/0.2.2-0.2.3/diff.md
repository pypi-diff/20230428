# Comparing `tmp/cochleogram-0.2.2.tar.gz` & `tmp/cochleogram-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.2.2.tar", last modified: Thu Apr 27 15:12:08 2023, max compression
+gzip compressed data, was "cochleogram-0.2.3.tar", last modified: Thu Apr 27 22:30:52 2023, max compression
```

## Comparing `cochleogram-0.2.2.tar` & `cochleogram-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.539695 cochleogram-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.531695 cochleogram-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.531695 cochleogram-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-27 15:11:51.000000 cochleogram-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-27 15:11:51.000000 cochleogram-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 15:12:08.539695 cochleogram-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.535695 cochleogram-0.2.2/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.539695 cochleogram-0.2.2/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26607 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-27 15:11:51.000000 cochleogram-0.2.2/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:12:08.535695 cochleogram-0.2.2/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:12:08.000000 cochleogram-0.2.2/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 15:11:51.000000 cochleogram-0.2.2/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 15:11:51.000000 cochleogram-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-27 15:11:51.000000 cochleogram-0.2.2/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:12:08.539695 cochleogram-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.510623 cochleogram-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.502623 cochleogram-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-27 22:30:41.000000 cochleogram-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-27 22:30:41.000000 cochleogram-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 22:30:52.510623 cochleogram-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.510623 cochleogram-0.2.3/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26607 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-27 22:30:41.000000 cochleogram-0.2.3/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:30:52.506623 cochleogram-0.2.3/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 22:30:52.000000 cochleogram-0.2.3/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 22:30:41.000000 cochleogram-0.2.3/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-27 22:30:41.000000 cochleogram-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-27 22:30:41.000000 cochleogram-0.2.3/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:30:52.510623 cochleogram-0.2.3/setup.cfg
```

### Comparing `cochleogram-0.2.2/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/.gitignore` & `cochleogram-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/PKG-INFO` & `cochleogram-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.2
+Version: 0.2.3
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.2/cochleogram/gui.enaml` & `cochleogram-0.2.3/cochleogram/gui.enaml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/cells.png` & `cochleogram-0.2.3/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/exclude.png` & `cochleogram-0.2.3/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/main-icon.png` & `cochleogram-0.2.3/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/make_icons.py` & `cochleogram-0.2.3/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/spiral.png` & `cochleogram-0.2.3/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/icons/tile.png` & `cochleogram-0.2.3/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/instructions.html` & `cochleogram-0.2.3/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/main.py` & `cochleogram-0.2.3/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/model.py` & `cochleogram-0.2.3/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/plot.py` & `cochleogram-0.2.3/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/presenter.py` & `cochleogram-0.2.3/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram/reader.py` & `cochleogram-0.2.3/cochleogram/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def __init__(self, path):
         from readlif.reader import LifFile
         super().__init__(path)
         self.fh = LifFile(path)
 
     def list_pieces(self):
-        p_piece = re.compile('.*piece_(\d+)\w?')
+        p_piece = re.compile('^(?!_)piece_(\d+)\w?')
         pieces = {}
         for img in self.fh.get_iter_image():
             try:
                 piece = int(p_piece.match(img.name).group(1))
                 pieces.setdefault(piece, []).append(img.name)
             except Exception as e:
                 pass
```

### Comparing `cochleogram-0.2.2/cochleogram/util.py` & `cochleogram-0.2.3/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.2.3/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.2.2
+Version: 0.2.3
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.2.2/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.2.3/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/pyproject.toml` & `cochleogram-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.2.2/readme.rst` & `cochleogram-0.2.3/readme.rst`

 * *Files identical despite different names*

