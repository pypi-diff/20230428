# Comparing `tmp/mell-2.0.3.tar.gz` & `tmp/mell-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.3.tar", last modified: Wed Apr 26 22:11:15 2023, max compression
+gzip compressed data, was "mell-2.0.4.tar", last modified: Fri Apr 28 18:16:49 2023, max compression
```

## Comparing `mell-2.0.3.tar` & `mell-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.371753 mell-2.0.3/
--rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-26 22:11:15.371753 mell-2.0.3/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)    15314 2023-04-26 21:22:17.000000 mell-2.0.3/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.367753 mell-2.0.3/mell/
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.3/mell/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-04-26 15:39:46.000000 mell-2.0.3/mell/consts.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    25505 2023-04-26 22:09:09.000000 mell-2.0.3/mell/main.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-26 22:11:15.367753 mell-2.0.3/mell.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      233 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-26 22:11:15.000000 mell-2.0.3/mell.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-26 22:11:15.371753 mell-2.0.3/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.3/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-28 18:16:49.607933 mell-2.0.4/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-28 18:16:49.607933 mell-2.0.4/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15314 2023-04-26 21:22:17.000000 mell-2.0.4/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-28 18:16:49.603933 mell-2.0.4/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.4/mell/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-04-28 18:16:20.000000 mell-2.0.4/mell/consts.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    25557 2023-04-27 15:32:46.000000 mell-2.0.4/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-28 18:16:49.607933 mell-2.0.4/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)    15743 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      275 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-04-28 18:16:49.000000 mell-2.0.4/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-04-28 18:16:49.607933 mell-2.0.4/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.4/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-04-28 18:16:49.607933 mell-2.0.4/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1516 2023-04-27 18:13:19.000000 mell-2.0.4/tests/test_metadata.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1784 2023-04-27 17:50:36.000000 mell-2.0.4/tests/test_news.py
```

### Comparing `mell-2.0.3/PKG-INFO` & `mell-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.3
+Version: 2.0.4
 Summary: Generate anything from template files and metadata files!
 Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mell-2.0.3/README.md` & `mell-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mell-2.0.3/mell/main.py` & `mell-2.0.4/mell/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,21 +48,23 @@
         info(f"  {path}")
         os.makedirs(path)
     
     sys.exit(0)
 
 def run_new_style(args):
 
-    info("Creating a new style structure at", args.new_style)
+    folderpath = os.path.join(args.root, args.new_style)
+
+    info("Creating a new style structure at", folderpath)
     
-    if os.path.exists(args.new_style):
-        error(f"Can't create a style structure, a folder with this name already exists: {args.new_style}")
+    if os.path.exists(folderpath):
+        error(f"Can't create a style structure, a folder with this name already exists: {folderpath}")
         
-    for foldernames in ["asset", "template", "plugin", "static"]:
-        path = os.path.join(args.new_style, foldernames)
+    for foldernames in ["asset", "template", "plugin", "static", "logic"]:
+        path = os.path.join(folderpath, foldernames)
         info(f"  {path}")
         os.makedirs(path)
     
     sys.exit(0)
 
 def run_new_plugin(args):
 
@@ -141,15 +143,15 @@
                         dest='do',
                         help="define one or more action to be executed [nothing, clean, static, template, plugin]",
                         action='append')
 
     parser.add_argument('--root',
                         type=str,
                         metavar='PATH',
-                        default='.',
+                        default=None,
                         dest='root',
                         help="root folder that contains the folders style, meta, and generate [.]",
                         action='store')
     
     parser.add_argument('--style',
                         type=str,
                         metavar='PATH',
```

### Comparing `mell-2.0.3/mell.egg-info/PKG-INFO` & `mell-2.0.4/mell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mell
-Version: 2.0.3
+Version: 2.0.4
 Summary: Generate anything from template files and metadata files!
 Home-page: https://github.com/diegofps/mell
 Author: Diego Souza
 Author-email: diegofpsouza+mell@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mell-2.0.3/setup.py` & `mell-2.0.4/setup.py`

 * *Files identical despite different names*

