# Comparing `tmp/pythoncolourlibraryV1-1.0.0.tar.gz` & `tmp/pythoncolourlibraryV1-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolourlibraryV1-1.0.0.tar", last modified: Thu Apr 27 08:23:14 2023, max compression
+gzip compressed data, was "pythoncolourlibraryV1-1.0.2.tar", last modified: Fri Apr 28 17:20:29 2023, max compression
```

## Comparing `pythoncolourlibraryV1-1.0.0.tar` & `pythoncolourlibraryV1-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:23:14.078313 pythoncolourlibraryV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-27 08:23:14.078313 pythoncolourlibraryV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:23:14.074313 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1/
--rw-r--r--   0 root         (0) root         (0)    70957 2023-04-27 08:23:13.000000 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 08:23:14.078313 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      406 2023-04-27 08:23:14.000000 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-27 08:23:14.000000 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 08:23:14.000000 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 08:23:14.000000 pythoncolourlibraryV1-1.0.0/pythoncolourlibraryV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 08:23:14.078313 pythoncolourlibraryV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-27 08:23:13.000000 pythoncolourlibraryV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 17:20:29.836470 pythoncolourlibraryV1-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-28 17:20:29.836470 pythoncolourlibraryV1-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 17:20:29.836470 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-28 17:20:29.000000 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 17:20:29.836470 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-28 17:20:29.000000 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-28 17:20:29.000000 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 17:20:29.000000 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 17:20:29.000000 pythoncolourlibraryV1-1.0.2/pythoncolourlibraryV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 17:20:29.836470 pythoncolourlibraryV1-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-28 17:20:28.000000 pythoncolourlibraryV1-1.0.2/setup.py
```

