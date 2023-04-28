# Comparing `tmp/tamp-0.0.0.tar.gz` & `tmp/tamp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-0.0.0.tar", max compression
+gzip compressed data, was "tamp-1.0.0.tar", max compression
```

## Comparing `tamp-0.0.0.tar` & `tamp-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 17:14:59.421766 tamp-0.0.0/LICENSE
--rw-r--r--   0        0        0     1151 2023-04-14 17:15:27.741585 tamp-0.0.0/README.rst
--rw-r--r--   0        0        0     3280 2023-04-14 17:15:33.138091 tamp-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      109 2023-04-14 17:15:33.138182 tamp-0.0.0/tamp/__init__.py
--rw-r--r--   0        0        0       57 2023-04-14 17:15:27.739653 tamp-0.0.0/tamp/__main__.py
--rw-r--r--   0        0        0        0 2023-04-14 17:15:27.739729 tamp-0.0.0/tamp/cli/__init__.py
--rw-r--r--   0        0        0      621 2023-04-14 17:15:27.739977 tamp-0.0.0/tamp/cli/main.py
--rw-r--r--   0        0        0     1770 1970-01-01 00:00:00.000000 tamp-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 19:18:02.269358 tamp-1.0.0/LICENSE
+-rw-r--r--   0        0        0    14269 2023-04-28 19:18:02.273358 tamp-1.0.0/README.rst
+-rw-r--r--   0        0        0     4998 2023-04-28 19:18:19.405580 tamp-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2497 2023-04-28 19:18:19.405580 tamp-1.0.0/tamp/__init__.py
+-rw-r--r--   0        0        0     1523 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2665 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/cli/main.py
+-rw-r--r--   0        0        0     8237 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/compressor.py
+-rw-r--r--   0        0        0     7136 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     6530 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/decompressor.py
+-rw-r--r--   0        0        0     9951 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-04-28 19:18:02.277358 tamp-1.0.0/tamp/py.typed
+-rw-r--r--   0        0        0    14888 1970-01-01 00:00:00.000000 tamp-1.0.0/PKG-INFO
```

### Comparing `tamp-0.0.0/LICENSE` & `tamp-1.0.0/LICENSE`

 * *Files identical despite different names*

