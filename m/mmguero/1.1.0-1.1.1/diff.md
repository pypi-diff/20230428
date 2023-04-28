# Comparing `tmp/mmguero-1.1.0.tar.gz` & `tmp/mmguero-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmguero-1.1.0.tar", last modified: Tue Apr 18 18:37:48 2023, max compression
+gzip compressed data, was "mmguero-1.1.1.tar", last modified: Fri Apr 28 13:54:09 2023, max compression
```

## Comparing `mmguero-1.1.0.tar` & `mmguero-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 18:37:40.000000 mmguero-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-18 18:37:48.947974 mmguero-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-18 18:37:40.000000 mmguero-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 18:37:40.000000 mmguero-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 18:37:48.947974 mmguero-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.943974 mmguero-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.943974 mmguero-1.1.0/src/mmguero/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/caselessdictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    34925 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/mmguero.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/src/mmguero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 18:37:40.000000 mmguero-1.1.0/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:09.360211 mmguero-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 13:54:00.000000 mmguero-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-28 13:54:09.360211 mmguero-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-28 13:54:00.000000 mmguero-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 13:54:00.000000 mmguero-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-28 13:54:09.360211 mmguero-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:09.360211 mmguero-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:09.360211 mmguero-1.1.1/src/mmguero/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 13:54:00.000000 mmguero-1.1.1/src/mmguero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-28 13:54:00.000000 mmguero-1.1.1/src/mmguero/caselessdictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34910 2023-04-28 13:54:00.000000 mmguero-1.1.1/src/mmguero/mmguero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:09.360211 mmguero-1.1.1/src/mmguero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-28 13:54:09.000000 mmguero-1.1.1/src/mmguero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-28 13:54:09.000000 mmguero-1.1.1/src/mmguero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:54:09.000000 mmguero-1.1.1/src/mmguero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:54:09.000000 mmguero-1.1.1/src/mmguero.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 13:54:09.000000 mmguero-1.1.1/src/mmguero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:54:09.360211 mmguero-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 13:54:00.000000 mmguero-1.1.1/tests/test_sample.py
```

### Comparing `mmguero-1.1.0/LICENSE` & `mmguero-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmguero-1.1.0/PKG-INFO` & `mmguero-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmguero
-Version: 1.1.0
+Version: 1.1.1
 Summary: Useful helpers by me, for me.
 Home-page: https://github.com/mmguero/python-mmguero
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mmguero/python-mmguero/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mmguero-1.1.0/README.md` & `mmguero-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mmguero-1.1.0/setup.cfg` & `mmguero-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mmguero
-version = 1.1.0
+version = 1.1.1
 author = Seth Grover
 author_email = mero.mero.guero@gmail.com
 description = Useful helpers by me, for me.
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mmguero/python-mmguero
```

### Comparing `mmguero-1.1.0/src/mmguero/caselessdictionary.py` & `mmguero-1.1.1/src/mmguero/caselessdictionary.py`

 * *Files identical despite different names*

### Comparing `mmguero-1.1.0/src/mmguero/mmguero.py` & `mmguero-1.1.1/src/mmguero/mmguero.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 from enum import IntFlag, auto
 from multiprocessing import RawValue
 from subprocess import PIPE, Popen, CalledProcessError
 from threading import Lock
 
 try:
     from pwd import getpwuid
-except ImportError:
+except Exception:
     getpwuid = None
 
 try:
     from shutil import which
 
     HasWhich = True
-except ImportError:
+except Exception:
     HasWhich = False
 
 try:
     from dialog import Dialog
 
     MainDialog = Dialog(dialog='dialog', autowidgetsize=True)
-except ImportError:
+except Exception:
     Dialog = None
     MainDialog = None
 
 ###################################################################################################
 PLATFORM_WINDOWS = "Windows"
 PLATFORM_MAC = "Darwin"
 PLATFORM_LINUX = "Linux"
@@ -908,15 +908,15 @@
     if not DynImports[importName]:
         # if not, attempt the import
         try:
             tmpImport = importlib.import_module(importName)
             if tmpImport:
                 DynImports[importName] = tmpImport
                 return DynImports[importName]
-        except ImportError:
+        except Exception:
             pass
 
         # see if we can help out by installing the module
 
         pyPlatform = platform.system()
         pyExec = sys.executable
         pipCmd = "pip3"
@@ -944,15 +944,15 @@
                 err, out = RunProcess(installCmd, debug=debug)
                 if err == 0:
                     eprint(f"Installation of {pipPkgName} module apparently succeeded")
                     try:
                         tmpImport = importlib.import_module(importName)
                         if tmpImport:
                             DynImports[importName] = tmpImport
-                    except ImportError as e:
+                    except Exception:
                         eprint(f"Importing the {importName} module still failed: {e}")
                 else:
                     eprint(f"Installation of {importName} module failed: {out}")
 
     if not DynImports[importName]:
         eprint(
             "System-wide installation varies by platform and Python configuration. Please consult platform-specific documentation for installing Python modules."
```

### Comparing `mmguero-1.1.0/src/mmguero.egg-info/PKG-INFO` & `mmguero-1.1.1/src/mmguero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmguero
-Version: 1.1.0
+Version: 1.1.1
 Summary: Useful helpers by me, for me.
 Home-page: https://github.com/mmguero/python-mmguero
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mmguero/python-mmguero/issues
 Classifier: License :: OSI Approved :: MIT License
```

