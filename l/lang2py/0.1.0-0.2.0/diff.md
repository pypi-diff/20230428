# Comparing `tmp/lang2py-0.1.0.tar.gz` & `tmp/lang2py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lang2py-0.1.0.tar", max compression
+gzip compressed data, was "lang2py-0.2.0.tar", max compression
```

## Comparing `lang2py-0.1.0.tar` & `lang2py-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       42 2023-04-27 20:52:25.963880 lang2py-0.1.0/README.md
--rw-r--r--   0        0        0     5933 2023-04-27 20:52:25.963880 lang2py-0.1.0/lang2py/__init__.py
--rw-r--r--   0        0        0      439 2023-04-27 20:52:25.963880 lang2py-0.1.0/lang2py/_utils.py
--rw-r--r--   0        0        0      289 2023-04-27 20:52:25.963880 lang2py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 lang2py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-04-27 22:29:44.996968 lang2py-0.2.0/README.md
+-rw-r--r--   0        0        0     3161 2023-04-27 22:29:44.996968 lang2py-0.2.0/lang2py/__init__.py
+-rw-r--r--   0        0        0      643 2023-04-27 22:29:44.996968 lang2py-0.2.0/lang2py/__main__.py
+-rw-r--r--   0        0        0      667 2023-04-27 22:29:44.996968 lang2py-0.2.0/lang2py/_utils.py
+-rw-r--r--   0        0        0      289 2023-04-27 22:29:44.996968 lang2py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 lang2py-0.2.0/PKG-INFO
```

