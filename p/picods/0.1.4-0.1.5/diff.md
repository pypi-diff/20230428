# Comparing `tmp/picods-0.1.4.tar.gz` & `tmp/picods-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picods-0.1.4.tar", max compression
+gzip compressed data, was "picods-0.1.5.tar", max compression
```

## Comparing `picods-0.1.4.tar` & `picods-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        6 2022-11-24 16:50:58.416987 picods-0.1.4/README.md
--rw-r--r--   0        0        0       93 2023-02-22 01:08:29.782750 picods-0.1.4/picods/__init__.py
--rw-r--r--   0        0        0       51 2023-02-22 01:08:58.862993 picods-0.1.4/picods/plot/__init__.py
--rw-r--r--   0        0        0      988 2023-02-22 02:24:49.590115 picods-0.1.4/picods/plot/plot.py
--rw-r--r--   0        0        0       54 2023-02-22 01:09:09.969753 picods-0.1.4/picods/table/__init__.py
--rw-r--r--   0        0        0      856 2023-02-22 02:22:54.999163 picods-0.1.4/picods/table/table.py
--rw-r--r--   0        0        0      418 2023-02-22 02:23:50.739626 picods-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 picods-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3157 2023-04-28 12:58:26.332181 picods-0.1.5/README.md
+-rw-r--r--   0        0        0       93 2023-04-28 12:58:26.332181 picods-0.1.5/picods/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-28 12:58:26.332181 picods-0.1.5/picods/plot/__init__.py
+-rw-r--r--   0        0        0      988 2023-04-28 12:58:26.332181 picods-0.1.5/picods/plot/plot.py
+-rw-r--r--   0        0        0       54 2023-04-28 12:58:26.332181 picods-0.1.5/picods/table/__init__.py
+-rw-r--r--   0        0        0      856 2023-04-28 12:58:26.332181 picods-0.1.5/picods/table/table.py
+-rw-r--r--   0        0        0      418 2023-04-28 12:58:55.528330 picods-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 picods-0.1.5/PKG-INFO
```

### Comparing `picods-0.1.4/picods/plot/plot.py` & `picods-0.1.5/picods/plot/plot.py`

 * *Files identical despite different names*

### Comparing `picods-0.1.4/picods/table/table.py` & `picods-0.1.5/picods/table/table.py`

 * *Files identical despite different names*

