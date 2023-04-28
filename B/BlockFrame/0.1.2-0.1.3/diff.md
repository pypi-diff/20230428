# Comparing `tmp/BlockFrame-0.1.2.tar.gz` & `tmp/BlockFrame-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-0.1.2.tar", last modified: Fri Apr 28 14:39:09 2023, max compression
+gzip compressed data, was "BlockFrame-0.1.3.tar", last modified: Fri Apr 28 14:42:10 2023, max compression
```

## Comparing `BlockFrame-0.1.2.tar` & `BlockFrame-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 14:39:09.090757 BlockFrame-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-28 14:39:09.066170 BlockFrame-0.1.2/BlockFrame/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.2/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0     3747 2023-04-05 06:33:24.000000 BlockFrame-0.1.2/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:39:09.080653 BlockFrame-0.1.2/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.2/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-28 14:30:52.000000 BlockFrame-0.1.2/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0      691 2023-04-28 14:22:04.000000 BlockFrame-0.1.2/BlockFrame/chunking_service/config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:39:09.089245 BlockFrame-0.1.2/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-0.1.2/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0      744 2023-04-28 14:05:46.000000 BlockFrame-0.1.2/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-04-28 14:02:33.000000 BlockFrame-0.1.2/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-28 14:26:18.000000 BlockFrame-0.1.2/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1372 2023-04-28 14:25:42.000000 BlockFrame-0.1.2/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-0.1.2/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:39:09.077640 BlockFrame-0.1.2/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0      218 2023-04-28 14:39:08.000000 BlockFrame-0.1.2/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2023-04-28 14:39:08.000000 BlockFrame-0.1.2/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 14:39:08.000000 BlockFrame-0.1.2/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-28 14:39:08.000000 BlockFrame-0.1.2/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 14:39:08.000000 BlockFrame-0.1.2/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      218 2023-04-28 14:39:09.090757 BlockFrame-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 14:39:09.090757 BlockFrame-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-04-28 14:39:05.000000 BlockFrame-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.582413 BlockFrame-0.1.3/BlockFrame/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.3/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0     3747 2023-04-05 06:33:24.000000 BlockFrame-0.1.3/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.599360 BlockFrame-0.1.3/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-28 14:30:52.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0      691 2023-04-28 14:22:04.000000 BlockFrame-0.1.3/BlockFrame/chunking_service/config.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.605875 BlockFrame-0.1.3/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-0.1.3/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0      744 2023-04-28 14:05:46.000000 BlockFrame-0.1.3/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-04-28 14:02:33.000000 BlockFrame-0.1.3/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 14:26:18.000000 BlockFrame-0.1.3/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     1372 2023-04-28 14:25:42.000000 BlockFrame-0.1.3/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-0.1.3/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:42:10.596369 BlockFrame-0.1.3/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-28 14:42:10.000000 BlockFrame-0.1.3/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      218 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:42:10.607876 BlockFrame-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-04-28 14:42:06.000000 BlockFrame-0.1.3/setup.py
```

### Comparing `BlockFrame-0.1.2/BlockFrame/block_frame.py` & `BlockFrame-0.1.3/BlockFrame/block_frame.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame/chunking_service/chunking.py` & `BlockFrame-0.1.3/BlockFrame/chunking_service/chunking.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame/chunking_service/config.py` & `BlockFrame-0.1.3/BlockFrame/chunking_service/config.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame/database_service/database.py` & `BlockFrame-0.1.3/BlockFrame/database_service/database.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-0.1.3/BlockFrame/database_service/defaultmodel.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame/database_service/initalisation.py` & `BlockFrame-0.1.3/BlockFrame/database_service/initalisation.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.2/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-0.1.3/BlockFrame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

