# Comparing `tmp/stirpy-1.1.5.tar.gz` & `tmp/stirpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stirpy-1.1.5.tar", last modified: Fri Apr 28 16:43:39 2023, max compression
+gzip compressed data, was "dist\stirpy-1.2.0.tar", last modified: Fri Apr 28 17:24:27 2023, max compression
```

## Comparing `stirpy-1.1.5.tar` & `stirpy-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 16:43:39.837275 stirpy-1.1.5/
--rw-rw-rw-   0        0        0      821 2023-04-28 16:43:39.835275 stirpy-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 16:43:39.838276 stirpy-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1019 2023-04-28 16:43:25.000000 stirpy-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 16:43:39.832275 stirpy-1.1.5/stirpy.egg-info/
--rw-rw-rw-   0        0        0      821 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 16:43:39.000000 stirpy-1.1.5/stirpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 17:24:27.871580 stirpy-1.2.0/
+-rw-rw-rw-   0        0        0      413 2023-04-28 17:24:27.869580 stirpy-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:24:27.872580 stirpy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-04-28 17:24:18.000000 stirpy-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:24:27.866580 stirpy-1.2.0/stirpy.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/top_level.txt
```

