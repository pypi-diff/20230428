# Comparing `tmp/cryptical-0.3.tar.gz` & `tmp/cryptical-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptical-0.3.tar", last modified: Fri Apr 28 20:55:08 2023, max compression
+gzip compressed data, was "cryptical-0.4.tar", last modified: Fri Apr 28 20:58:11 2023, max compression
```

## Comparing `cryptical-0.3.tar` & `cryptical-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.252367 cryptical-0.3/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:55:08.252367 cryptical-0.3/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.3/README.md
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.249367 cryptical-0.3/cryptical/
--rw-r--r--   0 harshit   (1000) harshit   (1000)     8616 2023-04-28 20:30:40.000000 cryptical-0.3/cryptical/cryptical.py
-drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:55:08.251367 cryptical-0.3/cryptical.egg-info/
--rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/PKG-INFO
--rw-r--r--   0 harshit   (1000) harshit   (1000)      241 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/SOURCES.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/dependency_links.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/entry_points.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       75 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/requires.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       10 2023-04-28 20:55:08.000000 cryptical-0.3/cryptical.egg-info/top_level.txt
--rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-28 20:55:08.252367 cryptical-0.3/setup.cfg
--rw-r--r--   0 harshit   (1000) harshit   (1000)      496 2023-04-28 20:54:58.000000 cryptical-0.3/setup.py
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.746568 cryptical-0.4/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:58:11.746568 cryptical-0.4/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      785 2023-04-28 20:18:30.000000 cryptical-0.4/README.md
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.743568 cryptical-0.4/cryptical/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)     8656 2023-04-28 20:56:55.000000 cryptical-0.4/cryptical/cryptical.py
+drwxr-xr-x   0 harshit   (1000) harshit   (1000)        0 2023-04-28 20:58:11.745568 cryptical-0.4/cryptical.egg-info/
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      150 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/PKG-INFO
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      241 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/SOURCES.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)        1 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/dependency_links.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       55 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/entry_points.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       75 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/requires.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       10 2023-04-28 20:58:11.000000 cryptical-0.4/cryptical.egg-info/top_level.txt
+-rw-r--r--   0 harshit   (1000) harshit   (1000)       38 2023-04-28 20:58:11.746568 cryptical-0.4/setup.cfg
+-rw-r--r--   0 harshit   (1000) harshit   (1000)      496 2023-04-28 20:57:43.000000 cryptical-0.4/setup.py
```

### Comparing `cryptical-0.3/README.md` & `cryptical-0.4/README.md`

 * *Files identical despite different names*

### Comparing `cryptical-0.3/cryptical/cryptical.py` & `cryptical-0.4/cryptical/cryptical.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ░ ░         ░     ░ ░                        ░  ░ ░            ░  ░    ░  ░
 ░                 ░ ░                           ░                          
 """
 
 from PIL.Image import open
 import customtkinter as ctk
 from tkinter import PhotoImage
-from utils.misc import setup_db, get_data
-from utils.add_vault_dialog import AddVaultDialog
-from utils.delete_vault_dialog import DeleteVaultDialog
-from utils.enter_password_dialog import EnterPasswordDialog
+from cryptical.utils.misc import setup_db, get_data
+from cryptical.utils.add_vault_dialog import AddVaultDialog
+from cryptical.utils.delete_vault_dialog import DeleteVaultDialog
+from cryptical.utils.enter_password_dialog import EnterPasswordDialog
 
 DB_FILE = "db.sqlite"
 ICON_PNG = "assets/icon.png"
 VAULT_IMG_PATH = "assets/lock.png"
 DEFAULT_WINDOW_WIDTH = 1100
 DEFAULT_WINDOW_HEIGHT = 580
 ctk.set_appearance_mode("Dark")
```

