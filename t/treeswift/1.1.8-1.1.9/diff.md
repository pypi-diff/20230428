# Comparing `tmp/treeswift-1.1.8.tar.gz` & `tmp/treeswift-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treeswift-1.1.8.tar", last modified: Tue Mar  3 16:47:06 2020, max compression
+gzip compressed data, was "dist/treeswift-1.1.9.tar", last modified: Wed Mar  4 06:42:04 2020, max compression
```

## Comparing `treeswift-1.1.8.tar` & `treeswift-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-03 16:47:06.000000 treeswift-1.1.8/
--rwxrwxrwx   0 niema     (1000) niema     (1000)     3219 2020-03-03 16:28:02.000000 treeswift-1.1.8/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 niema     (1000) niema     (1000)    35147 2020-03-03 16:28:02.000000 treeswift-1.1.8/LICENSE
--rwxrwxrwx   0 niema     (1000) niema     (1000)      130 2020-03-03 16:28:02.000000 treeswift-1.1.8/MANIFEST.in
--rwxrwxrwx   0 niema     (1000) niema     (1000)     1152 2020-03-03 16:47:06.000000 treeswift-1.1.8/PKG-INFO
--rwxrwxrwx   0 niema     (1000) niema     (1000)     1116 2020-03-03 16:28:02.000000 treeswift-1.1.8/README.md
--rwxrwxrwx   0 niema     (1000) niema     (1000)      102 2020-03-03 16:47:06.000000 treeswift-1.1.8/setup.cfg
--rwxrwxrwx   0 niema     (1000) niema     (1000)     2219 2020-03-03 16:47:04.000000 treeswift-1.1.8/setup.py
-drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift/
--rwxrwxrwx   0 niema     (1000) niema     (1000)    13427 2020-03-03 16:28:02.000000 treeswift-1.1.8/treeswift/Node.py
--rwxrwxrwx   0 niema     (1000) niema     (1000)    71443 2020-03-03 16:43:46.000000 treeswift-1.1.8/treeswift/Tree.py
--rwxrwxrwx   0 niema     (1000) niema     (1000)      265 2020-03-03 16:28:02.000000 treeswift-1.1.8/treeswift/__init__.py
-drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/
--rwxrwxrwx   0 niema     (1000) niema     (1000)        1 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/dependency_links.txt
--rwxrwxrwx   0 niema     (1000) niema     (1000)     1152 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/PKG-INFO
--rwxrwxrwx   0 niema     (1000) niema     (1000)       22 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/requires.txt
--rwxrwxrwx   0 niema     (1000) niema     (1000)      289 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/SOURCES.txt
--rwxrwxrwx   0 niema     (1000) niema     (1000)       10 2020-03-03 16:47:06.000000 treeswift-1.1.8/treeswift.egg-info/top_level.txt
+drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-04 06:42:04.000000 treeswift-1.1.9/
+-rwxrwxrwx   0 niema     (1000) niema     (1000)     3219 2020-03-04 06:39:23.000000 treeswift-1.1.9/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 niema     (1000) niema     (1000)    35147 2020-03-04 06:39:23.000000 treeswift-1.1.9/LICENSE
+-rwxrwxrwx   0 niema     (1000) niema     (1000)      130 2020-03-04 06:39:23.000000 treeswift-1.1.9/MANIFEST.in
+-rwxrwxrwx   0 niema     (1000) niema     (1000)     1152 2020-03-04 06:42:04.000000 treeswift-1.1.9/PKG-INFO
+-rwxrwxrwx   0 niema     (1000) niema     (1000)     1116 2020-03-04 06:39:23.000000 treeswift-1.1.9/README.md
+-rwxrwxrwx   0 niema     (1000) niema     (1000)      102 2020-03-04 06:42:04.000000 treeswift-1.1.9/setup.cfg
+-rwxrwxrwx   0 niema     (1000) niema     (1000)     2219 2020-03-04 06:42:02.000000 treeswift-1.1.9/setup.py
+drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift/
+-rwxrwxrwx   0 niema     (1000) niema     (1000)    13427 2020-03-04 06:39:23.000000 treeswift-1.1.9/treeswift/Node.py
+-rwxrwxrwx   0 niema     (1000) niema     (1000)    71513 2020-03-04 06:41:26.000000 treeswift-1.1.9/treeswift/Tree.py
+-rwxrwxrwx   0 niema     (1000) niema     (1000)      265 2020-03-04 06:39:23.000000 treeswift-1.1.9/treeswift/__init__.py
+drwxrwxrwx   0 niema     (1000) niema     (1000)        0 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/
+-rwxrwxrwx   0 niema     (1000) niema     (1000)        1 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/dependency_links.txt
+-rwxrwxrwx   0 niema     (1000) niema     (1000)     1152 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/PKG-INFO
+-rwxrwxrwx   0 niema     (1000) niema     (1000)       22 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/requires.txt
+-rwxrwxrwx   0 niema     (1000) niema     (1000)      289 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/SOURCES.txt
+-rwxrwxrwx   0 niema     (1000) niema     (1000)       10 2020-03-04 06:42:04.000000 treeswift-1.1.9/treeswift.egg-info/top_level.txt
```

### Comparing `treeswift-1.1.8/CODE_OF_CONDUCT.md` & `treeswift-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `treeswift-1.1.8/LICENSE` & `treeswift-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `treeswift-1.1.8/PKG-INFO` & `treeswift-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treeswift
-Version: 1.1.8
+Version: 1.1.9
 Summary: TreeSwift: Fast tree module for Python 2 and 3
 Home-page: https://github.com/niemasd/TreeSwift
 Author: Niema Moshiri
 Author-email: niemamoshiri@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/niemasd/TreeSwift
 Project-URL: Bug Reports, https://github.com/niemasd/TreeSwift/issues
```

### Comparing `treeswift-1.1.8/README.md` & `treeswift-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `treeswift-1.1.8/setup.py` & `treeswift-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 setup(
     name='treeswift',  # Required
-    version='1.1.8',  # Required
+    version='1.1.9',  # Required
     description='TreeSwift: Fast tree module for Python 2 and 3',  # Required
     long_description='TreeSwift is a Python library for parsing, manipulating, and iterating over (rooted) tree structures. TreeSwift places an emphasis on speed.',  # Optional
     long_description_content_type='text/plain',  # Optional (see note above)
     url='https://github.com/niemasd/TreeSwift',  # Optional
     author='Niema Moshiri',  # Optional
     author_email='niemamoshiri@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `treeswift-1.1.8/treeswift/Node.py` & `treeswift-1.1.9/treeswift/Node.py`

 * *Files identical despite different names*

### Comparing `treeswift-1.1.8/treeswift/Tree.py` & `treeswift-1.1.9/treeswift/Tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,20 +412,20 @@
             ``label_fontsize`` (``int``): Font size of the leaf labels (in points). 8pt = 1/9in --> 1in = 72pt
 
             ``color`` (``str``): The color of the resulting plot
 
             ``xlabel`` (``str``): The label of the horizontal axis in the resulting plot
         '''
         import matplotlib.pyplot as plt
-        import matplotlib as mpl
         from matplotlib.ticker import MaxNLocator
-        rcParams_orig = mpl.rcParams.copy()
-        mpl.rcParams['axes.spines.left'] = False # hide left spine
-        mpl.rcParams['axes.spines.right'] = False # hide right spine
-        mpl.rcParams['axes.spines.top'] = False # hide top spine
+        from matplotlib import rcParams
+        orig = {k:rcParams[k] for k in ['axes.spines.left','axes.spines.right','axes.spines.top']}
+        rcParams['axes.spines.left'] = False # hide left spine
+        rcParams['axes.spines.right'] = False # hide right spine
+        rcParams['axes.spines.top'] = False # hide top spine
 
         # compute total height needed at each node
         dy = dict()
         for node in self.traverse_postorder():
             if node.is_leaf():
                 dy[node] = 1
             else:
@@ -481,15 +481,16 @@
             plt.xlabel(xlabel)
         plt.tight_layout()
         if show_plot:
             plt.show()
         if export_filename is not None:
             plt.savefig(export_filename)
         plt.close()
-        mpl.rcParams = rcParams_orig
+        for k in orig:
+            rcParams[k] = orig[k]
 
     def edge_length_sum(self, terminal=True, internal=True):
         '''Compute the sum of all selected edge lengths in this ``Tree``
 
         Args:
             ``terminal`` (``bool``): ``True`` to include terminal branches, otherwise ``False``
```

### Comparing `treeswift-1.1.8/treeswift.egg-info/PKG-INFO` & `treeswift-1.1.9/treeswift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treeswift
-Version: 1.1.8
+Version: 1.1.9
 Summary: TreeSwift: Fast tree module for Python 2 and 3
 Home-page: https://github.com/niemasd/TreeSwift
 Author: Niema Moshiri
 Author-email: niemamoshiri@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/niemasd/TreeSwift
 Project-URL: Bug Reports, https://github.com/niemasd/TreeSwift/issues
```

