# Comparing `tmp/FuncsForSPO-4.40.3.tar.gz` & `tmp/FuncsForSPO-4.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.40.3.tar", last modified: Fri Mar 31 19:29:55 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.41.0.tar", last modified: Fri Apr 28 12:42:54 2023, max compression
```

## Comparing `FuncsForSPO-4.40.3.tar` & `FuncsForSPO-4.41.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.513397 FuncsForSPO-4.40.3/
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.237913 FuncsForSPO-4.40.3/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.293739 FuncsForSPO-4.40.3/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.40.3/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.40.3/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.302738 FuncsForSPO-4.40.3/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.40.3/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.313302 FuncsForSPO-4.40.3/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.40.3/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.321313 FuncsForSPO-4.40.3/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.40.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.231427 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.337081 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.351987 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.356974 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.372357 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     2979 2023-01-20 12:06:28.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.382354 FuncsForSPO-4.40.3/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.392362 FuncsForSPO-4.40.3/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.40.3/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.401560 FuncsForSPO-4.40.3/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.40.3/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.413015 FuncsForSPO-4.40.3/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.40.3/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.421227 FuncsForSPO-4.40.3/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.40.3/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.40.3/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.430648 FuncsForSPO-4.40.3/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.40.3/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.40.3/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.435646 FuncsForSPO-4.40.3/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.40.3/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:29:55.282245 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-03-31 19:29:55.000000 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-03-31 19:29:55.000000 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 19:29:55.000000 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-03-31 19:29:55.000000 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-03-31 19:29:55.000000 FuncsForSPO-4.40.3/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.40.3/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-03-31 19:29:55.509393 FuncsForSPO-4.40.3/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.40.3/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 19:29:55.513397 FuncsForSPO-4.40.3/setup.cfg
--rw-rw-rw-   0        0        0     2150 2023-03-31 19:29:50.000000 FuncsForSPO-4.40.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:54.115944 FuncsForSPO-4.41.0/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.550721 FuncsForSPO-4.41.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.673833 FuncsForSPO-4.41.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.41.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.41.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.696332 FuncsForSPO-4.41.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.41.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.720212 FuncsForSPO-4.41.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.41.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.740232 FuncsForSPO-4.41.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.41.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.536564 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.765998 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.791074 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.801639 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.844028 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     4844 2023-04-28 12:40:26.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.869041 FuncsForSPO-4.41.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.887366 FuncsForSPO-4.41.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    69597 2023-03-17 17:54:18.000000 FuncsForSPO-4.41.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.907278 FuncsForSPO-4.41.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.41.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.927621 FuncsForSPO-4.41.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38180 2023-03-31 19:28:24.000000 FuncsForSPO-4.41.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.953185 FuncsForSPO-4.41.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.41.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.41.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.968786 FuncsForSPO-4.41.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.41.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.41.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.980348 FuncsForSPO-4.41.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.41.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 12:42:53.658577 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-04-28 12:42:53.000000 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-04-28 12:42:53.000000 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 12:42:53.000000 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-04-28 12:42:53.000000 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-04-28 12:42:53.000000 FuncsForSPO-4.41.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.41.0/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-04-28 12:42:54.109543 FuncsForSPO-4.41.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.41.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 12:42:54.117452 FuncsForSPO-4.41.0/setup.cfg
+-rw-rw-rw-   0        0        0     2150 2023-04-28 12:42:41.000000 FuncsForSPO-4.41.0/setup.py
```

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.41.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.41.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.41.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.41.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.40.3
+Version: 4.41.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.40.3/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.41.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/LICENSE` & `FuncsForSPO-4.41.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/PKG-INFO` & `FuncsForSPO-4.41.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.40.3
+Version: 4.41.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.40.3/README.md` & `FuncsForSPO-4.41.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.40.3/setup.py` & `FuncsForSPO-4.41.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.40.3'
+version = '4.41.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

