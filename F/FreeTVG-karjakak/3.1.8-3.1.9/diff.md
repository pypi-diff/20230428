# Comparing `tmp/FreeTVG-karjakak-3.1.8.tar.gz` & `tmp/FreeTVG-karjakak-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.1.8.tar", last modified: Fri Jan  6 16:37:16 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.1.9.tar", last modified: Tue Jan 10 15:44:45 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.1.8.tar` & `FreeTVG-karjakak-3.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-06 16:37:16.719422 FreeTVG-karjakak-3.1.8/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-06 16:37:16.715541 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      426 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      118 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-01-06 16:37:16.000000 FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.1.8/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-06 16:37:16.719512 FreeTVG-karjakak-3.1.8/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.1.8/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-06 16:37:16.717437 FreeTVG-karjakak-3.1.8/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   158552 2023-01-06 16:19:56.000000 FreeTVG-karjakak-3.1.8/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   521169 2022-12-20 04:59:38.000000 FreeTVG-karjakak-3.1.8/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.1.8/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-06 16:37:16.719293 FreeTVG-karjakak-3.1.8/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.1.8/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.1.8/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     5322 2023-01-06 05:51:32.000000 FreeTVG-karjakak-3.1.8/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.1.8/TVG/utility/term.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.1.8/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      941 2023-01-06 16:37:16.719801 FreeTVG-karjakak-3.1.8/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.535956 FreeTVG-karjakak-3.1.9/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.534245 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      426 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      118 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-01-10 15:44:45.000000 FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.1.9/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-01-10 15:44:45.536033 FreeTVG-karjakak-3.1.9/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.1.9/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.534966 FreeTVG-karjakak-3.1.9/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   158552 2023-01-06 16:19:56.000000 FreeTVG-karjakak-3.1.9/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   521169 2022-12-20 04:59:38.000000 FreeTVG-karjakak-3.1.9/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.1.9/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-01-10 15:44:45.535687 FreeTVG-karjakak-3.1.9/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)     1091 2022-12-04 14:36:50.000000 FreeTVG-karjakak-3.1.9/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)      110 2022-11-22 15:56:19.000000 FreeTVG-karjakak-3.1.9/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5637 2023-01-10 15:40:05.000000 FreeTVG-karjakak-3.1.9/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)     1174 2022-11-23 15:06:38.000000 FreeTVG-karjakak-3.1.9/TVG/utility/term.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.1.9/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      941 2023-01-10 15:44:45.536316 FreeTVG-karjakak-3.1.9/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.1.8/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.1.9/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.1.8
+Version: 3.1.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.1.8/LICENSE.txt` & `FreeTVG-karjakak-3.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/PKG-INFO` & `FreeTVG-karjakak-3.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.1.8
+Version: 3.1.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.1.8/README.md` & `FreeTVG-karjakak-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.1.9/TVG/FreeTVG.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.1.9/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.1.9/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.1.9/TVG/utility/mdh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2020, KarjaKAK
 # All rights reserved.
 
 import os
 import re
+from pathlib import Path
+from subprocess import run
 from sys import platform
 
 import markdown
 
 __all__ = [""]
 
 
@@ -170,18 +172,26 @@
                     fcs.append(f"{i}\n")
 
         if fcs:
             cssstyle = "".join(fcs)
         del fcs
         with open(f"{filename}.html", "w") as whtm:
             whtm.write(cssstyle)
+        pro = None
         if platform.startswith("win"):
-            os.startfile(f"{filename}.html")
+            pro = [
+                "powershell.exe",
+                "start",
+                "msedge",
+                f"'\"{Path(f'{filename}.html').absolute()}\"'",
+            ]
+            run(pro)
         else:
-            os.system(f'open "{filename}.html"')
+            pro = ["open", "-a", "Safari", f"{Path(f'{filename}.html').absolute()}"]
+            run(pro)
         del (
             text,
             filename,
             font,
             bg,
             fg,
             gettext,
@@ -190,10 +200,11 @@
             foreground,
             kbfg,
             chg,
             setfont,
             cssstyle,
             printed,
             nxt,
+            pro,
         )
     except Exception as e:
         raise e
```

### Comparing `FreeTVG-karjakak-3.1.8/TVG/utility/term.py` & `FreeTVG-karjakak-3.1.9/TVG/utility/term.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.1.8/setup.cfg` & `FreeTVG-karjakak-3.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.1.8
+version = 3.1.9
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

