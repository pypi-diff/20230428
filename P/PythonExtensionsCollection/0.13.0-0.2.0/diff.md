# Comparing `tmp/PythonExtensionsCollection-0.13.0.tar.gz` & `tmp/PythonExtensionsCollection-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonExtensionsCollection-0.13.0.tar", last modified: Fri Apr 28 12:18:33 2023, max compression
+gzip compressed data, was "dist\PythonExtensionsCollection-0.2.0.tar", last modified: Tue Jun 28 13:33:22 2022, max compression
```

## Comparing `PythonExtensionsCollection-0.13.0.tar` & `PythonExtensionsCollection-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.561963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.561963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Comparison/
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Comparison/CComparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Comparison/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.561963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/File/
--rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/File/CFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/File/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Folder/
--rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Folder/CFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   281523 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/PythonExtensionsCollection.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/String/
--rw-r--r--   0 runner    (1001) docker     (123)    37642 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/String/CString.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/String/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Utils/CUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:18:33.561963 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-28 12:18:33.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-28 12:18:33.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:18:33.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:18:33.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 12:18:33.000000 PythonExtensionsCollection-0.13.0/PythonExtensionsCollection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:18:33.565963 PythonExtensionsCollection-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-28 12:16:19.000000 PythonExtensionsCollection-0.13.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.505917 PythonExtensionsCollection-0.2.0/
+-rw-rw-rw-   0        0        0    11357 2022-05-31 17:55:20.000000 PythonExtensionsCollection-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3386 2022-06-28 13:33:22.503963 PythonExtensionsCollection-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.461959 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.486372 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/File/
+-rw-rw-rw-   0        0        0    29590 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/File/CFile.py
+-rw-rw-rw-   0        0        0      611 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/File/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.494207 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/String/
+-rw-rw-rw-   0        0        0    49547 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/String/CString.py
+-rw-rw-rw-   0        0        0      611 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/String/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.501035 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/Utils/
+-rw-rw-rw-   0        0        0    12359 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/Utils/CUtils.py
+-rw-rw-rw-   0        0        0      611 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/Utils/__init__.py
+-rw-rw-rw-   0        0        0      611 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-28 13:33:22.479571 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/
+-rw-rw-rw-   0        0        0     3386 2022-06-28 13:33:21.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2022-06-28 13:33:22.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-28 13:33:21.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2022-06-28 13:33:21.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2022-06-28 13:33:21.000000 PythonExtensionsCollection-0.2.0/PythonExtensionsCollection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2022-06-28 13:33:22.505917 PythonExtensionsCollection-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0    10505 2022-06-24 13:57:03.000000 PythonExtensionsCollection-0.2.0/setup.py
```

### Comparing `PythonExtensionsCollection-0.13.0/LICENSE` & `PythonExtensionsCollection-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Comparison/__init__.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/File/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/File/__init__.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/String/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Folder/__init__.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/Utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/String/CString.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/String/CString.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,84 +16,75 @@
 #
 # **************************************************************************************************************
 #
 # CString.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 14.11.2022
+# 26.01.2022
 #
 # **************************************************************************************************************
 
 # -- import standard Python modules
 import os, ntpath, re
 
 # **************************************************************************************************************
 
 class CString(object):
-   """
-The class ``CString`` contains some string computation methods like e.g. normalizing a path.
-   """
+   """Contains some string computation methods like e.g. normalizing a path."""
 
    # --------------------------------------------------------------------------------------------------------------
    #TM***
 
    def NormalizePath(sPath=None, bWin=False, sReferencePathAbs=None, bConsiderBlanks=False, bExpandEnvVars=True, bMask=True):
       """
-Normalizes local paths, paths to local network resources and internet addresses
+|
 
-**Arguments:**
+**Method:**
 
-* ``sPath``
+**NormalizePath**
 
-  / *Condition*: required / *Type*: str /
+   Normalizes local paths, paths to local network resources and internet addresses
 
-  The path to be normalized
+**Args:**
 
-* ``bWin``
+**sPath** (*string*)
 
-  / *Condition*: optional / *Type*: bool / *Default*: False /
+   The path to be normalized
 
-  If ``True`` then returned path contains masked backslashes as separator, otherwise slashes
+**bWin** (*boolean; optional; default: False*)
 
-* ``sReferencePathAbs``
+   If ``True`` then returned path contains masked backslashes as separator, otherwise slashes
 
-  / *Condition*: optional / *Type*: str / *Default*: None /
+**sReferencePathAbs** (*string, optional*)
 
-  In case of ``sPath`` is relative and ``sReferencePathAbs`` (expected to be absolute) is given, then
-  the returned absolute path is a join of both input paths
+   In case of ``sPath`` is relative and ``sReferencePathAbs`` (expected to be absolute) is given, then
+   the returned absolute path is a join of both input paths
 
-* ``bConsiderBlanks``
+**bConsiderBlanks** (*boolean; optional; default: False*)
 
-  / *Condition*: optional / *Type*: bool / *Default*: False /
+   If ``True`` then the returned path is encapsulated in quotes - in case of the path contains blanks
 
-  If ``True`` then the returned path is encapsulated in quotes - in case of the path contains blanks
-
-* ``bExpandEnvVars``
-
-  / *Condition*: optional / *Type*: bool / *Default*: True /
+**bExpandEnvVars** (*boolean; optional; default: True*)
 
    If ``True`` then in the returned path environment variables are resolved, otherwise not.
 
-* ``bMask``
-
-  / *Condition*: optional / *Type*: bool / *Default*: True (requires ``bWin=True``)/
+**bMask** (*boolean; optional; default: True; requires bWin=True*)
 
-  * If ``bWin`` is ``True`` and ``bMask`` is ``True`` then the returned path contains masked backslashes as separator.
-  * If ``bWin`` is ``True`` and ``bMask`` is ``False`` then the returned path contains single backslashes only - this might be
-    required for applications, that are not able to handle masked backslashes.
-  * In case of ``bWin`` is ``False`` ``bMask`` has no effect.
+   If ``bWin`` is ``True`` and ``bMask`` is ``True`` then the returned path contains masked backslashes as separator.
+   If ``bWin`` is ``True`` and ``bMask`` is ``False`` then the returned path contains single backslashes only - this might be
+   required for applications, that are not able to handle masked backslashes. In case of ``bWin`` is ``False`` ``bMask`` has no effect.
 
 **Returns:**
 
-* ``sPath``
+**sPath** (*string*)
 
-  / *Type*: str /
+   The normalized path (is ``None`` in case of ``sPath`` is ``None``)
 
-  The normalized path (is ``None`` in case of ``sPath`` is ``None``)
+|
       """
 
       if sPath is not None:
 
          # -- expand Windows environment variables
          if bExpandEnvVars is True:
             sPath = os.path.expandvars(sPath)
@@ -217,77 +208,68 @@
    # eof NormalizePath(sPath=None, bWin=False, sReferencePathAbs=None, bConsiderBlanks=False, bExpandEnvVars=True, bMask=True)
 
    # --------------------------------------------------------------------------------------------------------------
    #TM***
 
    def DetectParentPath(sStartPath=None, sFolderName=None, sFileName=None):
       """
-Computes the path to any parent folder inside a given path. Optionally DetectParentPath is able
-to search for files inside the identified parent folder.
+|
 
-**Arguments:**
+**Method:**
 
-* ``sStartPath``
+**DetectParentPath**
 
-  / *Condition*: required / *Type*: str /
+   Computes the path to any parent folder inside a given path. Optionally DetectParentPath is able
+   to search for files inside the parent folder.
 
-  The path in which to search for a parent folder
+**Args:**
 
-* ``sFolderName``
+**sStartPath** (*string*)
 
-  / *Condition*: required / *Type*: str /
+   The path in which to search for a parent folder
 
-  The name of the folder to search for within ``sStartPath``. It is possible to provide more than one folder name separated by semicolon
+**sFolderName** (*string*)
 
-* ``sFileName``
+   The name of the folder to search for within ``sStartPath``. It is possible to provide more than one folder name separated by semicolon
 
-  / *Condition*: optional / *Type*: str / *Default*: None /
+**sFileName** (*string, optional*)
 
-  The name of a file to search within the detected parent folder
+   The name of a file to search within the detected parent folder
 
 **Returns:**
 
-* ``sDestPath``
-
-  / *Type*: str /
-
-  Path and name of parent folder found inside ``sStartPath``, ``None`` in case of ``sFolderName`` is not found inside ``sStartPath``.
-  In case of more than one parent folder is found ``sDestPath`` contains the first result and ``listDestPaths`` contains all results.
-
-* ``listDestPaths``
+**sDestPath** (*string*)
 
-  / *Type*: list /
+   Path and name of parent folder found inside ``sStartPath``, ``None`` in case of ``sFolderName`` is not found inside ``sStartPath``.
+   In case of more than one parent folder is found ``sDestPath`` contains the first result and ``listDestPaths`` contains all results.
 
-  If ``sFolderName`` contains a single folder name this list contains only one element that is ``sDestPath``.
-  In case of ``FolderName`` contains a semicolon separated list of several folder names this list contains all found paths of the given folder names.
-  ``listDestPaths`` is ``None`` (and not an empty list!) in case of ``sFolderName`` is not found inside ``sStartPath``.
+**listDestPaths** (*list*)
 
-* ``sDestFile``
+   If ``sFolderName`` contains a single folder name this list contains only one element that is ``sDestPath``.
+   In case of ``FolderName`` contains a semicolon separated list of several folder names this list contains all found paths of the given folder names.
+   ``listDestPaths`` is ``None`` (and not an empty list!) in case of ``sFolderName`` is not found inside ``sStartPath``.
 
-  / *Type*: str /
+**sDestFile** (*string*)
 
-  Path and name of ``sFileName``, in case of ``sFileName`` is given and found inside ``listDestPaths``.
-  In case of more than one file is found ``sDestFile`` contains the first result and ``listDestFiles`` contains all results.
-  ``sDestFile`` is ``None`` in case of ``sFileName`` is ``None`` and also in case of ``sFileName`` is not found inside ``listDestPaths``
-  (and therefore also in case of ``sFolderName`` is not found inside ``sStartPath``).
+   Path and name of ``sFileName``, in case of ``sFileName`` is given and found inside ``listDestPaths``.
+   In case of more than one file is found ``sDestFile`` contains the first result and ``listDestFiles`` contains all results.
+   ``sDestFile`` is ``None`` in case of ``sFileName`` is ``None`` and also in case of ``sFileName`` is not found inside ``listDestPaths``
+   (and therefore also in case of ``sFolderName`` is not found inside ``sStartPath``).
 
-* ``listDestFiles``
+**listDestFiles** (*list*)
 
-  / *Type*: list /
+   Contains all positions of ``sFileName`` found inside ``listDestPaths``.
+   ``listDestFiles`` is ``None`` (and not an empty list!) in case of ``sFileName`` is ``None`` and also in case of ``sFileName``
+   is not found inside ``listDestPaths`` (and therefore also in case of ``sFolderName`` is not found inside ``sStartPath``).
 
-  Contains all positions of ``sFileName`` found inside ``listDestPaths``.
+**sDestPathParent** (*string*)
 
-  ``listDestFiles`` is ``None`` (and not an empty list!) in case of ``sFileName`` is ``None`` and also in case of ``sFileName``
-  is not found inside ``listDestPaths`` (and therefore also in case of ``sFolderName`` is not found inside ``sStartPath``).
+   The parent folder of ``sDestPath``, ``None`` in case of ``sFolderName`` is not found inside ``sStartPath`` (``sDestPath`` is ``None``).
 
-* ``sDestPathParent``
-
-  / *Type*: str /
-
-  The parent folder of ``sDestPath``, ``None`` in case of ``sFolderName`` is not found inside ``sStartPath`` (``sDestPath`` is ``None``).
+|
       """
 
       sDestPath       = None
       listDestPaths   = None
       sDestFile       = None
       listDestFiles   = None
       sDestPathParent = None
@@ -338,30 +320,29 @@
       # eof while len(listLevels) > 0:
 
       sDestPath       = None
       sDestPathParent = None
       if len(listDestPaths) > 0:
          # -- returning sDestPath and sDestPathParent related to first entry in list; just to return anything else than None
          sDestPath = listDestPaths[0]
-         sDestPathParent = os.path.dirname(sDestPath)
+         sDestPathParent = CString.NormalizePath(os.path.dirname(sDestPath))
 
       # -- optionally searching also for a single file
       # Input: file name
       # Output: full path of file and list of full paths of files (!!! limited to 'listDestPaths' !!!)
 
       listDestFiles = []
 
       if ( (sFileName is not None) and (len(listDestPaths) > 0) ):
          for sDestPathToWalk in listDestPaths:
             for sLocalRootPath, listFolderNames, listFileNames in os.walk(sDestPathToWalk):
                for sFileNameTmp in listFileNames:
                   if sFileNameTmp == sFileName:
                      sFile = CString.NormalizePath(os.path.join(sLocalRootPath, sFileName))
-                     if sFile not in listDestFiles:
-                        listDestFiles.append(sFile)
+                     listDestFiles.append(sFile)
             # eof for sLocalRootPath, listFolderNames, listFileNames in os.walk(sDestPathToWalk):
          # eof for sDestPathToWalk in listDestPaths:
       # eof if ( (sFileName is not None) and (len(listDestPaths) > 0) ):
 
       if len(listDestFiles) > 0:
          listDestFiles.sort()
          sDestFile = listDestFiles[0] # just to return anything else than None
@@ -391,24 +372,73 @@
                     sEndsNotWith      = None,
                     sContains         = None,
                     sContainsNot      = None,
                     sInclRegEx        = None,
                     sExclRegEx        = None,
                     bDebug            = False):
       """
+|
+
+During the computation of strings there might occur the need to get to know if this string fulfils certain criteria or not.
+Such a criterion can e.g. be that the string contains a certain substring. Also an inverse logic might be required:
+In this case the criterion is that the string does **not** contain this substring.
+
+It might also be required to combine several criteria to a final conclusion if in total the criterion for a string is fulfilled or not.
+For example: The string must start with the string *prefix* and must also contain either the string *substring1* or the string *substring2*
+but must also **not** end with the string *suffix*.
+
 This method provides a bunch of predefined filters that can be used singly or combined to come to a final conclusion if the string fulfils all criteria or not.
 
-These filters can be e.g. used to select or exclude lines while reading from a text file. Or they can be used to select or exclude files or folders
-while walking through the file system.
+The filters are divided into three different types:
+
+1. Filters that are interpreted as raw strings (called 'standard filters'; no wild cards supported)
+2. Filters that are interpreted as regular expressions (called 'regular expression based filters'; the syntax of regular expressions has to be considered)
+3. Boolean switches (e.g. indicating if also an empty string is accepted or not)
+
+The input string might contain leading and trailing blanks and tabs. This kind of horizontal space is removed from the input string
+before the standard filters start their work (except the regular expression based filters).
+
+The regular expression based filters consider the original input string (including the leading and trailing space). 
+
+The outcome is that in case of the leading and trailing space shall be part of the criterion, the regular expression based filters can be used only.
+
+It is possible to decide if the standard filters shall work case sensitive or not. This decision has no effect on the regular expression based filters.
+
+The regular expression based filters always work with the original input string that is not modified in any way.
+
+Except the regular expression based filters it is possible to provide more than one string for every standard filter (must be a semikolon separated list in this case).
+A semicolon that shall be part of the search string, has to be masked in this way: ``\;``.
+
+This method returns a boolean value that is ``True`` in case of all criteria are fulfilled, and ``False`` in case of some or all of them are not fulfilled.
+
+The default value for all filters is ``None`` (except ``bSkipBlankStrings``). In case of a filter value is ``None`` this filter has no influence on the result.
+
+In case of all filters are ``None`` (default) the return value is ``True`` (except the string itself is ``None``
+or the string is empty and ``bSkipBlankStrings`` is ``True``).
+
+In case of the string is ``None``, the return value is ``False``, because nothing concrete can be done with ``None`` strings.
 
-**The following filters are available:**
+Internally every filter has his own individual acknowledge that indicates if the criterion of this filter is fulfilled or not.
+
+The meaning of *criterion fulfilled* of a filter is that the filter supports the final return value ``bAck`` of this method with ``True``.
+
+The final return value ``bAck`` of this method is a logical join (``AND``) of all individual acknowledges (except ``bSkipBlankStrings`` and ``sComment``;
+in case of their criteria are **not** fulfilled, immediately ``False`` is returned).
+
+Summarized:
+
+* Filters are used to define *criteria*
+* The return value of this method provides the *conclusion* - indicating if all criteria are fulfilled or not
+
+
+*The following filters are available:*
 
 **bSkipBlankStrings**
 
-   * Leading and trailing spaces are removed from the input string at the beginning
+   * Like already mentioned above leading and trailing spaces are removed from the input string at the beginning
    * In case of the result is an empty string and ``bSkipBlankStrings`` is ``True``, the method immediately returns ``False``
      and all other filters are ignored
 
 **sComment**
 
    * In case of the input string starts with the string ``sComment``, the method immediately returns ``False``
      and all other filters are ignored
@@ -470,43 +500,246 @@
 
    * *Exclude* filter based on regular expressions (consider the syntax of regular expressions!)
    * The criterion of this filter is fulfilled in case of the regular expression ``sExclRegEx`` does **not** match the input string
    * Leading and trailing blanks within the input string are considered
    * ``bCaseSensitive`` has no effect
    * A semicolon separated list of several regular expressions is **not** supported
 
-**Further arguments:**
-
-* ``sString``
+*Further parameter:*
 
-  / *Condition*: required / *Type*: str /
+**sString**
 
   The input string that has to be investigated. 
 
-* ``bCaseSensitive``
-
-  / *Condition*: optional / *Type*: bool / *Default*: True /
+**bCaseSensitive** (*boolean, optional, default*: ``True``)
 
   If ``True``, the standard filters work case sensitive, otherwise not.
 
-* ``bDebug``
-
-  / *Condition*: optional / *Type*: bool / *Default*: False /
+**bDebug** (*boolean, optional, default*: ``False``)
 
   If ``True``, additional output is printed to console (e.g. the decision of every single filter), otherwise not.
 
-**Returns:**
+*Examples:*
 
-* ``bAck``
+Returns ``True``:
 
-  / *Type*: bool /
+.. code::
 
-  Final statement about the input string ``sString`` after filter computation
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = "Sp",
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = "beats",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = "Sp",
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = "minute",
+                               sContains         = "beats",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+Returns ``True``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = None,
+                               sContainsNot      = "Beats",
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+Returns ``True``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = None,
+                               sContainsNot      = None,
+                               sInclRegEx        = r"\d{2}",
+                               sExclRegEx        = None)
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = "Speed",
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = None,
+                               sContainsNot      = None,
+                               sInclRegEx        = r"\d{3}",
+                               sExclRegEx        = None)
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = "Speed",
+                               sEndsWith         = "minute",
+                               sStartsNotWith    = "speed",
+                               sEndsNotWith      = None,
+                               sContains         = "beats",
+                               sContainsNot      = None,
+                               sInclRegEx        = r"\d{2}",
+                               sExclRegEx        = r"\d{2}")
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "     ",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = None,
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "# Speed is 25 beats per minute",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = "#",
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = "beats",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+
+Returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "   Alpha is not beta; and beta is not gamma  ",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = "   Alpha ",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+Because blanks around search strings (here ``"   Alpha "``) are considered, whereas the blanks around the input string are removed before computation.
+Therefore ``"   Alpha "`` cannot be found within the (shortened) input string.
+
+
+This alternative solution returns ``True``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "   Alpha is not beta; and beta is not gamma  ",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = None,
+                               sContainsNot      = None,
+                               sInclRegEx        = r"\s{3}Alpha",
+                               sExclRegEx        = None)
+
+
+Returns ``True``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Alpha is not beta; and beta is not gamma",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = "beta; and",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
+
+The meaning of ``"beta; and"`` is: The criterion is fulfilled in case of either ``"beta"`` or ``" and"`` can be found. That's ``True`` in this example - but this
+has nothing to do with the fact, that also this string ``"beta; and"`` can be found. A semicolon that shall be part of the search, has to be masked!
+
+The meaning of ``"beta\; not"`` in the following example is: The criterion is fulfilled in case of ``"beta; not"`` can be found.
+
+That's **not** ``True``. Therefore the method returns ``False``:
+
+.. code::
+
+   bAck = CString.StringFilter(sString           = "Alpha is not beta; and beta is not gamma",
+                               bCaseSensitive    = True,
+                               bSkipBlankStrings = True,
+                               sComment          = None,
+                               sStartsWith       = None,
+                               sEndsWith         = None,
+                               sStartsNotWith    = None,
+                               sEndsNotWith      = None,
+                               sContains         = r"beta\; not",
+                               sContainsNot      = None,
+                               sInclRegEx        = None,
+                               sExclRegEx        = None)
 
-Further details together with codde examples can be found within chapter **Description**, subsubsection **StringFilter**.
+|
       """
 
       if sString is None:
          return False # hard coded here; no separate filter for that decision
 
       # The original string 'sString' is used by regular expression filters sInclRegEx and sExclRegEx.
       # The stripped string 'sStringStripped' is used by all other filters.
@@ -672,14 +905,15 @@
          if sContains != "":
             sContainsModified = sContains.replace(r"\;", sSeparatorSubstitute) # replace the masked separator by a substitute separator
             listContains = []
             if sContainsModified.find(";") >= 0:
                listParts = sContainsModified.split(";")
                for sPart in listParts:
                   sPart = sPart.replace(sSeparatorSubstitute , ";") # recover the original version
+                  print(f"- Part: '{sPart}'")
                   listContains.append(sPart)
             else:
                sContainsModified = sContains.replace(r"\;", ";") # convert to unmasked version
                listContains.append(sContainsModified)
 
             bContains = False
             for sContains in listContains:
@@ -817,50 +1051,32 @@
    # eof def StringFilter(...)
 
    # --------------------------------------------------------------------------------------------------------------
    #TM***
 
    def FormatResult(sMethod="", bSuccess=True, sResult=""):
       """
-Formats the result string ``sResult`` depending on ``bSuccess``:
+|
 
-* ``bSuccess`` is ``True`` indicates *success*
-* ``bSuccess`` is ``False`` indicates an *error*
-* ``bSuccess`` is ``None`` indicates an *exception*
+**Method:**
 
-Additionally the name of the method that causes the result, can be provided (*optional*).
-This is useful for debugging.
+**FormatResult**
 
-**Arguments:**
+   Formats the result string ``sResult`` depending on ``bSuccess``:
 
-* ``sMethod``
-
-  / *Condition*: optional / *Type*: str / *Default*: (empty string) /
-
-  Name of the method that causes the result.
-
-* ``bSuccess``
-
-  / *Condition*: optional / *Type*: bool / *Default*: True /
-
-  Indicates if the computation of the method ``sMethod`` was successful or not.
-
-* ``sResult``
-
-  / *Condition*: optional / *Type*: str / *Default*: (empty string) /
-
-  The result of the computation of the method ``sMethod``.
-
-**Returns:**
+   * ``bSuccess`` is ``True`` indicates *success*
+   * ``bSuccess`` is ``False`` indicates an *error*
+   * ``bSuccess`` is ``None`` indicates an *exception*
 
-* ``sResult``
+   Additionally the name of the method that causes the result, can be provided (*optional*).
+   This is useful for debugging.
 
-  / *Type*: str /
+   Returns the formatted result string.
 
-  The formatted result string.
+|
       """
 
       if sMethod is None:
          sMethod = str(sMethod)
       if sResult is None:
          sResult = str(sResult)
       if bSuccess is True:
```

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/String/__init__.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `PythonExtensionsCollection-0.13.0/PythonExtensionsCollection/Utils/CUtils.py` & `PythonExtensionsCollection-0.2.0/PythonExtensionsCollection/Utils/CUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,84 +16,116 @@
 #
 # **************************************************************************************************************
 #
 # CUtils.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# 29.03.2023
+# 26.01.2022
 #
 # **************************************************************************************************************
 
 # -- import standard Python modules
 from dotdict import dotdict
 
 # **************************************************************************************************************
 # wrapper
 # **************************************************************************************************************
 
 def PrettyPrint(oData=None, hOutputFile=None, bToConsole=True, nIndent=0, sPrefix=None, bHexFormat=False):
    """
-Wrapper function to create and use a ``CTypePrint`` object. This wrapper function is responsible for
-printing out the content to console and to a file (depending on input parameter).
+|
 
-The content itself is prepared by the method ``TypePrint`` of class ``CTypePrint``. This happens ``PrettyPrint`` internally.
+**Function:**
 
-The idea behind the ``PrettyPrint`` function is to resolve also the content of composite data types and provide for every parameter inside:
+**PrettyPrint**
 
-* the type
-* the total number of elements inside (e.g. the number of keys inside a dictionary)
-* the counter number of the current element
-* the value
+   Wrapper function to create and use a ``CTypePrint`` object. This wrapper function is responsible for
+   printing out the content to console and to a file (depending on input parameter).
 
-**Arguments:**
+   The content itself is prepared by the method ``TypePrint`` of class ``CTypePrint``. This happens ``PrettyPrint`` internally.
 
-* ``oData``
+   The idea behind the ``PrettyPrint`` function is to resolve also the content of composite data types and provide for every parameter inside:
 
-  / *Condition*: required / *Type*: (*any Python data type*) /
+   * the type
+   * the total number of elements inside (e.g. the number of keys inside a dictionary)
+   * the counter number of the current element
+   * the value
 
-  A variable of any Python data type.
+   Example call:
 
-* ``hOutputFile``
+   ``PrettyPrint(oData)`` (*with oData is a Python variable of any type*)
 
-  / *Condition*: optional / *Type*: file handle / *Default*: None /
+   The output can e.g. look like this:
 
-  If handle is not ``None`` the content is written to this file, otherwise not.
+   .. code:: python
 
-* ``bToConsole``
+      [DICT] (3/1) > {K1} [STR]  :  'Val1'
+      [DICT] (3/2) > {K2} [LIST] (4/1) > [INT]  :  1
+      [DICT] (3/2) > {K2} [LIST] (4/2) > [STR]  :  'A'
+      [DICT] (3/2) > {K2} [LIST] (4/3) > [INT]  :  2
+      [DICT] (3/2) > {K2} [LIST] (4/4) > [TUPLE] (2/1) > [INT]  :  9
+      [DICT] (3/2) > {K2} [LIST] (4/4) > [TUPLE] (2/2) > [STR]  :  'Z'
+      [DICT] (3/3) > {K3} [INT]  :  5
 
-  / *Condition*: optional / *Type*: bool / *Default*: True /
+   Every line of output has to be interpreted strictly from left to right.
 
-  If ``True`` the content is written to console, otherwise not.
+   For example the meaning of the fifth line of output
 
-* ``nIndent``
+   ``[DICT] (3/2) > {K2} [LIST] (4/4) > [TUPLE] (2/1) > [INT]  :  9``
 
-  / *Condition*: optional / *Type*: int / *Default*: 0 /
+   is:
 
-  Sets the number of additional blanks at the beginning of every line of output (indentation).
+   * The type of input parameter (``oData``) is ``dict``
+   * The dictionary contains 3 keys
+   * The current line gives information about the second key of the dictionary
+   * The name of the second key is 'K2'
+   * The value of the second key is of type ``list``
+   * The list contains 4 elements
+   * The current line gives information about the fourth element of the list
+   * The fourth element of the list is of type ``tuple``
+   * The tuple contains 2 elements
+   * The current line gives information about the first element of the tuple
+   * The first element of the tuple is of type ``int`` and has the value 9
 
-* ``sPrefix``
+   Types are encapsulated in square brackets, counter in round brackets and key names are encapsulated in curly brackets.
 
-  / *Condition*: optional / *Type*: str / *Default*: None /
+**Args:**
 
-  Sets a prefix string that is added at the beginning of every line of output.
+**oData** (*any Python data type*)
 
-* ``bHexFormat``
+   A variable of any Python data type.
 
-  / *Condition*: optional / *Type*: bool / *Default*: False /
+**hOutputFile** (*handle to a file opened for writing or appending; optional; default None*)
 
-  If ``True`` the output is printed in hexadecimal format (but valid for strings only).
+   If handle is not ``None`` the content is written to this file, otherwise not.
+
+**bToConsole** (*bool; optional; default: True*)
+
+   If ``True`` the content is written to console, otherwise not.
+
+**nIndent** (*int; optional; default: 0*)
+
+   Sets the number of additional blanks at the beginning of every line of output (indentation).
+
+**sPrefix** (*str; optional; default: None*)
+
+   Sets a prefix string that is added at the beginning of every line of output.
+
+**bHexFormat** (*bool; optional; default: False*)
+
+   If ``True`` the output is printed in hexadecimal format (but strings only).
 
 **Returns:**
 
-* ``listOutLines`` (*list*)
+**listOutLines** (*list*)
 
-  / *Type*: list /
+   List of lines containing the prepared output
 
-  List of lines containing the prepared output
+|
    """
 
    oTypePrint   = CTypePrint()
    listOutLines = oTypePrint.TypePrint(oData, bHexFormat)
 
    listReturned = []
    for sLine in listOutLines:
@@ -113,27 +145,16 @@
    return listReturned
 
 # eof def PrettyPrint(oData=None, hOutputFile=None, bToConsole=True, nIndent=0, sPrefix=None, bHexFormat=False):
 
 # --------------------------------------------------------------------------------------------------------------
 # TM***
 
-class CTypePrint(object):
-   """
-The class ``CTypePrint`` provides a method (``TypePrint``) to compute the following data:
-
-* the type
-* the total number of elements inside (e.g. the number of keys inside a dictionary)
-* the counter number of the current element
-* the value
-
-of simple and composite data types.
+class CTypePrint():
 
-The call of this method is encapsulated within the function ``PrettyPrint`` inside this module.
-   """
    def __init__(self):
       self.listGlobalPrefixes = []
       self.listOutLines       = []
 
    def __del__(self):
       pass
 
@@ -143,74 +164,49 @@
       listHex = []
       for sChar in sString:
          listHex.append(hex(ord(sChar)))
       sStringHex = " ".join(listHex)
       return sStringHex
 
    def TypePrint(self, oData=None, bHexFormat=False):
-      """
-The method ``TypePrint`` computes details about the input variable ``oData``.
-
-**Arguments:**
-
-* ``oData``
-
-  / *Condition*: required / *Type*: any Python data type /
-
-  Python variable of any data type.
-
-* ``bHexFormat``
-
-  / *Condition*: optional / *Type*: bool / *Default*: False /
-
-  If ``True`` the output is provide in hexadecimal format.
-
-**Returns:**
-
-* ``listOutLines``
-
-  / *Type*: list /
-
-  List of lines containing the resolved content of ``oData``.
-      """
 
       if oData is None:
          sLocalPrefix = "[NONE]"
          sGlobalPrefix = " ".join(self.listGlobalPrefixes)
          sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  " + str(oData)
          self.listOutLines.append(sOut.strip())
 
-      elif type(oData) is int:
+      elif type(oData) == int:
          sLocalPrefix = "[INT]"
          sGlobalPrefix = " ".join(self.listGlobalPrefixes)
          sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  " + str(oData)
          self.listOutLines.append(sOut.strip())
 
-      elif type(oData) is float:
+      elif type(oData) == float:
          sLocalPrefix = "[FLOAT]"
          sGlobalPrefix = " ".join(self.listGlobalPrefixes)
          sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  " + str(oData)
          self.listOutLines.append(sOut.strip())
 
-      elif type(oData) is bool:
+      elif type(oData) == bool:
          sLocalPrefix = "[BOOL]"
          sGlobalPrefix = " ".join(self.listGlobalPrefixes)
          sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  " + str(oData)
          self.listOutLines.append(sOut.strip())
 
-      elif type(oData) is str:
+      elif type(oData) == str:
          sLocalPrefix = "[STR]"
          sGlobalPrefix = " ".join(self.listGlobalPrefixes)
          sData = str(oData)
          if bHexFormat is True:
             sData = self._ToHex(sData)
          sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  '" + sData + "'"
          self.listOutLines.append(sOut.strip())
 
-      elif type(oData) is list:
+      elif type(oData) == list:
          nNrOfElements = len(oData)
          if nNrOfElements == 0:
             # -- indicate empty list
             sLocalPrefix = "[LIST]"
             sGlobalPrefix = " ".join(self.listGlobalPrefixes)
             sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  []"
             self.listOutLines.append(sOut.strip())
@@ -222,15 +218,15 @@
                nCnt = nCnt + 1
                sCnt = "(" + str(nNrOfElements) + "/" + str(nCnt) + ") >"
                self.listGlobalPrefixes.append(sCnt)
                self.TypePrint(oElement, bHexFormat) # >>>> recursion
                del self.listGlobalPrefixes[-1]      # remove prefix count
             del self.listGlobalPrefixes[-1]         # remove prefix name
 
-      elif type(oData) is tuple:
+      elif type(oData) == tuple:
          nNrOfElements = len(oData)
          if nNrOfElements == 0:
             # -- indicate empty tuple
             sLocalPrefix = "[TUPLE]"
             sGlobalPrefix = " ".join(self.listGlobalPrefixes)
             sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  ()"
             self.listOutLines.append(sOut.strip())
@@ -242,15 +238,15 @@
                nCnt = nCnt + 1
                sCnt = "(" + str(nNrOfElements) + "/" + str(nCnt) + ") >"
                self.listGlobalPrefixes.append(sCnt)
                self.TypePrint(oElement, bHexFormat) # >>>> recursion
                del self.listGlobalPrefixes[-1]      # remove prefix count
             del self.listGlobalPrefixes[-1]         # remove prefix name
 
-      elif type(oData) is set:
+      elif type(oData) == set:
          nNrOfElements = len(oData)
          if nNrOfElements == 0:
             # -- indicate empty set
             sLocalPrefix = "[SET]"
             sGlobalPrefix = " ".join(self.listGlobalPrefixes)
             sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  ()"
             self.listOutLines.append(sOut.strip())
@@ -262,15 +258,15 @@
                nCnt = nCnt + 1
                sCnt = "(" + str(nNrOfElements) + "/" + str(nCnt) + ") >"
                self.listGlobalPrefixes.append(sCnt)
                self.TypePrint(oElement, bHexFormat) # >>>> recursion
                del self.listGlobalPrefixes[-1]      # remove prefix count
             del self.listGlobalPrefixes[-1]         # remove prefix name
 
-      elif type(oData) is dict:
+      elif type(oData) == dict:
          nNrOfElements = len(oData)
          if nNrOfElements == 0:
             # -- indicate empty dictionary
             sLocalPrefix = "[DICT]"
             sGlobalPrefix = " ".join(self.listGlobalPrefixes)
             sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  {}"
             self.listOutLines.append(sOut.strip())
@@ -284,15 +280,16 @@
                oValue = oData[sKey]
                sCntAndKey = "(" + str(nNrOfElements) + "/" + str(nCnt) + ") > {" + str(sKey) + "}"
                self.listGlobalPrefixes.append(sCntAndKey)
                self.TypePrint(oValue, bHexFormat) # >>>> recursion
                del self.listGlobalPrefixes[-1]    # remove prefix count
             del self.listGlobalPrefixes[-1]       # remove prefix name
 
-      elif ( (type(oData) is dotdict) or (str(type(oData)) == "<class 'robot.utils.dotdict.DotDict'>") or (str(type(oData)) == "<class 'RobotFramework_TestsuitesManagement.Config.CConfig.dotdict'>") ):
+      # elif type(oData) == dotdict:
+      elif ( (type(oData) == dotdict) or (str(type(oData)) == "<class 'robot.utils.dotdict.DotDict'>") ):
          nNrOfElements = len(oData)
          if nNrOfElements == 0:
             # -- indicate empty dot dictionary
             sLocalPrefix = "[DOTDICT]"
             sGlobalPrefix = " ".join(self.listGlobalPrefixes)
             sOut = sGlobalPrefix + " " + sLocalPrefix + "  :  {}"
             self.listOutLines.append(sOut.strip())
```

### Comparing `PythonExtensionsCollection-0.13.0/README.rst` & `PythonExtensionsCollection-0.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,71 @@
-.. Copyright 2020-2022 Robert Bosch GmbH
+.. Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
 
-.. Licensed under the Apache License, Version 2.0 (the "License");
+   Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
-.. http://www.apache.org/licenses/LICENSE-2.0
+   http://www.apache.org/licenses/LICENSE-2.0
 
-.. Unless required by applicable law or agreed to in writing, software
+   Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 Package Description
 ===================
 
-The **PythonExtensionsCollection** package extends the functionality of Python by some useful functions
+Getting Started
+---------------
+
+The Python Extensions Collection package extends the functionality of Python by some useful functions
 that are not available in Python immediately.
 
 How to install
 --------------
 
-The **PythonExtensionsCollection** can be installed in two different ways.
-
-1. Installation via PyPi (recommended for users)
-
-   .. code::
-
-      pip install PythonExtensionsCollection
-
-   `PythonExtensionsCollection in PyPi <https://pypi.org/project/PythonExtensionsCollection/>`_
-
-2. Installation via GitHub (recommended for developers)
-
-   Clone the **python-extensions-collection** repository to your machine.
+Firstly clone the **python-extensions-collection** repository to your machine.
 
-   .. code::
+`Python Extensions Collection <https://github.com/test-fullautomation/python-extensions-collection>`_
 
-      git clone https://github.com/test-fullautomation/python-extensions-collection.git
+Use the following two common commands to build or install this package:
 
-   `PythonExtensionsCollection in GitHub <https://github.com/test-fullautomation/python-extensions-collection>`_
+.. code-block::
 
-   Use the following command to install the **PythonExtensionsCollection**:
+    setup.py build      will build the package underneath 'build/'
+    setup.py install    will install the package
 
-   .. code::
-
-      setup.py install
+After the build processes is completed, the package is located in 'build/', and the generated 
+package documentation is located in 'doc/_build/'.
 
 Package Documentation
 ---------------------
 
-A detailed documentation of the **PythonExtensionsCollection** can be found here:
-`PythonExtensionsCollection.pdf <https://github.com/test-fullautomation/python-extensions-collection/blob/develop/PythonExtensionsCollection/PythonExtensionsCollection.pdf>`_
-
+A detailed documentation of the Python Extensions Collection package can be found here:
+`Python-Extensions-Collection.pdf <https://github.com/test-fullautomation/python-extensions-collection/blob/develop/doc/_build/latex/Python-Extensions-Collection.pdf>`_
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to `Thomas Pollerspöck <mailto:Thomas.Pollerspoeck@de.bosch.com>`_ 
 
-In case you want to report a bug or request any interesting feature, please don't hesitate to raise a ticket.
+In case you want to report a bug or request any interesting feature, please don't 
+hesitate to raise a ticket.
 
 Maintainers
 -----------
 
-`Holger Queckenstedt <mailto:Holger.Queckenstedt@de.bosch.com>`_
-
 `Thomas Pollerspöck <mailto:Thomas.Pollerspoeck@de.bosch.com>`_
 
 Contributors
 ------------
 
 `Holger Queckenstedt <mailto:Holger.Queckenstedt@de.bosch.com>`_
 
-`Thomas Pollerspöck <mailto:Thomas.Pollerspoeck@de.bosch.com>`_
-
 License
 -------
 
 Copyright 2020-2022 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

### Comparing `PythonExtensionsCollection-0.13.0/setup.py` & `PythonExtensionsCollection-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 # **************************************************************************************************************
 #
 # setup.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# Extends the standard setuptools installation by adding the documentation in PDF format
+# Extends the standard setuptools installation by adding the documentation in HTML format
 # (requires installation mode) and tidying up some folders.
 #
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #
-# This script deletes folders (as defined in config.CRepositoryConfig, depending on the position of this script):
+# This script deletes folders (as defined in config.CConfig, depending on the position of this script):
 # - previous builds within this repository
 # - previous installations within
 #   * <Python installation>\Lib\site-packages (Windows)
 #   * <Python installation>/../lib/python3.9/site-packages (Linux)
 #
 # before the build and the installation start again!
 #
@@ -40,40 +40,59 @@
 # --------------------------------------------------------------------------------------------------------------
 #
 # * Hints:
 #
 # The usual
 #    packages = setuptools.find_packages(),
 # is replaced by
-#    packages = [str(oRepositoryConfig.Get('PACKAGENAME')), ],
-# to avoid that also config.CRepositoryConfig() and additions.CExtendedSetup() are part of the distribution.
-# CRepositoryConfig and CExtendedSetup() are only repository internal helper.
+#    packages = [str(oRepositoryConfig.Get('sPackageName')), ],
+# to avoid that also config.CConfig() and config.CExtendedSetup() are part of the distribution.
+# CConfig and CExtendedSetup() are only repository internal helper.
 #
 # * Known issues:
 #
 #   - setuptools do not properly update an existing package installation under <Python installation>\Lib\site-packages\<package name>!
 #     > Files modified manually within installation folder, are still modified after repeated execution of setuptools.
 #     > Files added manually within installation folder, are still present there after repeated execution of setuptools.
 #     > Only files deleted manually within installation folder, are are restored there after repeated execution of setuptools.
 #   - No such issues with <Python installation>\Lib\site-packages\<package name>-<versions>.egg-info.
 #   - Solution: explicit deletion of all previous output (all documentation-, build- and installation-folder, except the egg-info folder)
 #     (see 'delete_previous_build()' and 'delete_previous_installation()')
 #
 # --------------------------------------------------------------------------------------------------------------
 #
-# 25.10.2022
+# 22.02.2022 / XC-CT/ECA3-Queckenstedt
+# "sdist bdist_wheel" maintenance: some steps moved from inside 'ExtendedInstallCommand' to outside
+#
+# 16.12.2021 / XC-CI1/ECA3-Queckenstedt
+# Bugfix: Added missing module folder 'Utils'
+#
+# 15.12.2021 / XC-CI1/ECA3-Queckenstedt
+# Suppressed generation of documents and installations in case of command line
+# parameter is not 'install' and not 'build' (this enables printing the help only).
+#
+# 03.11.2021 / XC-CI1/ECA3-Queckenstedt
+# Adapted to computation of 'python_extensions_collection' package
+# 
+# 11.10.2021 / XC-CI1/ECA3-Queckenstedt
+# Fixed computation order of readme files together with long_description
+# 
+# 30.09.2021 / XC-CI1/ECA3-Queckenstedt
+# Added wrapper for error messages
+# 
+# Initial version 08/2021
 #
 # --------------------------------------------------------------------------------------------------------------
 
 import os, sys, platform, shlex, subprocess
 import setuptools
 from setuptools.command.install import install
 
-from config.CRepositoryConfig import CRepositoryConfig # providing repository and environment specific information
-from additions.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
+from config.CConfig import CConfig # providing repository and environment specific information
+from config.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
 
 import colorama as col
 
 col.init(autoreset=True)
 
 COLBR = col.Style.BRIGHT + col.Fore.RED
 COLBY = col.Style.BRIGHT + col.Fore.YELLOW
@@ -95,28 +114,50 @@
 class ExtendedInstallCommand(install):
     """Extended setup for installation mode."""
 
     def run(self):
 
         listCmdArgs = sys.argv
         if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
-            install.run(self)
+            print()
+            print(COLBY + "Extended setup step 4/5: install.run(self)") # creates the build folder .\build
+            print()
+            install.run(self) # TODO: What does install.run(self) return? How to realize error handling?
+            print()
+            if 'bdist_wheel' in listCmdArgs:
+                print(COLBY + "Extended setup step 5/5: Add html documentation to local wheel folder inside build")
+                print()
+                nReturn = oExtendedSetup.add_htmldoc_to_wheel()
+                if nReturn != SUCCESS:
+                    return nReturn
+                print()
+            else:
+                print(COLBY + "Extended setup step 5/5: Add html documentation to package installation folder") # (./doc/_build/html to <Python installation>\Lib\site-packages\<package name>_doc)
+                print()
+                nReturn = oExtendedSetup.add_htmldoc_to_installation()
+                if nReturn != SUCCESS:
+                    return nReturn
+                print()
+            print(COLBG + "Extended installation done")
+            print()
+
         return SUCCESS
 
 # eof class ExtendedInstallCommand(install):
 
 # --------------------------------------------------------------------------------------------------------------
 
 # -- Even in case of other command line parameters than 'install' or 'build' are used we need the following objects.
 #    (Without repository configuration commands like '--author-email' would not be possible)
 
 # -- setting up the repository configuration
 oRepositoryConfig = None
+sReferencePath = os.path.dirname(os.path.abspath(sys.argv[0]))
 try:
-    oRepositoryConfig = CRepositoryConfig(os.path.abspath(sys.argv[0]))
+    oRepositoryConfig = CConfig(sReferencePath)
 except Exception as ex:
     print()
     printexception(str(ex))
     print()
     sys.exit(ERROR)
 
 # -- setting up the extended setup
@@ -136,90 +177,67 @@
 listCmdArgs = sys.argv
 if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
     print()
     print(COLBY + "Entering extended installation")
     print()
 
     print(COLBY + "Extended setup step 1/5: Calling the documentation builder")
+    # (previously called inside ExtendedInstallCommand - but this is too late, because the content of the initially
+    # generated or updated README file is already needed for the long_description below.)
     print()
-
-    nReturn = oExtendedSetup.genpackagedoc()
-    if nReturn != SUCCESS:
-        sys.exit(nReturn)
-
-    print(COLBY + "Extended setup step 2/5: Converting the repository README")
-    print()
-
-    nReturn = oExtendedSetup.convert_repo_readme()
+    nReturn = oExtendedSetup.gen_doc()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    print(COLBY + "Extended setup step 3/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
+    print(COLBY + "Extended setup step 2/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
     print()
-
     nReturn = oExtendedSetup.delete_previous_build()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    if ( ('bdist_wheel' in listCmdArgs) or ('build' in listCmdArgs) ):
+    if not 'bdist_wheel' in listCmdArgs:
         print()
-        print(COLBY + "Skipping extended setup step 4/5: Deleting previous package installation folder within site-packages")
-        print()
-    else:
-        print()
-        print(COLBY + "Extended setup step 4/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
+        print(COLBY + "Extended setup step 3/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
         print()
         nReturn = oExtendedSetup.delete_previous_installation()
         if nReturn != SUCCESS:
             sys.exit(nReturn)
 
-    README_MD = str(oRepositoryConfig.Get('README_MD'))
-    with open(README_MD, "r", encoding="utf-8") as fh:
+    with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
-    fh.close()
-
-# --------------------------------------------------------------------------------------------------------------
+    print()
 
-# -- the 'setup' itself
 
-print(COLBY + "Extended setup step 5/5: install.run(self)")
-print()
+# --------------------------------------------------------------------------------------------------------------
 
+# This also handles the printing of help to console and therefore must be called in every case.
+# And therefore all variables and objects must exist (even in case of the values are not used).
 setuptools.setup(
-    name         = str(oRepositoryConfig.Get('PACKAGENAME')),
-    version      = str(oRepositoryConfig.Get('PACKAGEVERSION')),
-    author       = str(oRepositoryConfig.Get('AUTHOR')),
-    author_email = str(oRepositoryConfig.Get('AUTHOREMAIL')),
-    description  = str(oRepositoryConfig.Get('DESCRIPTION')),
+    name         = str(oRepositoryConfig.Get('sPackageName')),
+    version      = str(oRepositoryConfig.Get('sVersion')),
+    author       = str(oRepositoryConfig.Get('sAuthor')),
+    author_email = str(oRepositoryConfig.Get('sAuthorEMail')),
+    description  = str(oRepositoryConfig.Get('sDescription')),
     long_description = long_description,
-    long_description_content_type = str(oRepositoryConfig.Get('LONGDESCRIPTIONCONTENTTYPE')),
-    url = str(oRepositoryConfig.Get('URL')),
-    packages = [str(oRepositoryConfig.Get('PACKAGENAME')),
-                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Comparison",
-                str(oRepositoryConfig.Get('PACKAGENAME')) + ".String",
-                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Utils",
-                str(oRepositoryConfig.Get('PACKAGENAME')) + ".File",
-                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Folder"],
+    long_description_content_type = str(oRepositoryConfig.Get('sLongDescriptionContentType')),
+    url = str(oRepositoryConfig.Get('sURL')),
+    packages = [str(oRepositoryConfig.Get('sPackageName')),
+                str(oRepositoryConfig.Get('sPackageName')) + ".String",
+                str(oRepositoryConfig.Get('sPackageName')) + ".Utils",
+                str(oRepositoryConfig.Get('sPackageName')) + ".File"],
     classifiers = [
-        str(oRepositoryConfig.Get('PROGRAMMINGLANGUAGE')),
-        str(oRepositoryConfig.Get('LICENCE')),
-        str(oRepositoryConfig.Get('OPERATINGSYSTEM')),
-        str(oRepositoryConfig.Get('DEVELOPMENTSTATUS')),
-        str(oRepositoryConfig.Get('INTENDEDAUDIENCE')),
-        str(oRepositoryConfig.Get('TOPIC')),
+        str(oRepositoryConfig.Get('sProgrammingLanguage')),
+        str(oRepositoryConfig.Get('sLicence')),
+        str(oRepositoryConfig.Get('sOperatingSystem')),
+        str(oRepositoryConfig.Get('sDevelopmentStatus')),
+        str(oRepositoryConfig.Get('sIntendedAudience')),
+        str(oRepositoryConfig.Get('sTopic')),
     ],
-    python_requires = str(oRepositoryConfig.Get('PYTHONREQUIRES')),
+    python_requires = str(oRepositoryConfig.Get('sPythonRequires')),
     cmdclass={
         'install': ExtendedInstallCommand,
     },
-    install_requires = oRepositoryConfig.Get('INSTALLREQUIRES'),
-    package_data={f"{oRepositoryConfig.Get('PACKAGENAME')}" : oRepositoryConfig.Get('PACKAGEDATA')},
+    install_requires = oRepositoryConfig.Get('arInstallRequires'),
 )
 
 # --------------------------------------------------------------------------------------------------------------
 
-print()
-print(COLBG + "Extended installation done")
-print()
-
-# --------------------------------------------------------------------------------------------------------------
-
```

