# Comparing `tmp/stirpy-1.2.0.tar.gz` & `tmp/stirpy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stirpy-1.2.0.tar", last modified: Fri Apr 28 17:24:27 2023, max compression
+gzip compressed data, was "dist\stirpy-1.2.5.tar", last modified: Fri Apr 28 17:50:23 2023, max compression
```

## Comparing `stirpy-1.2.0.tar` & `stirpy-1.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 17:24:27.871580 stirpy-1.2.0/
--rw-rw-rw-   0        0        0      413 2023-04-28 17:24:27.869580 stirpy-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-28 17:24:27.872580 stirpy-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-04-28 17:24:18.000000 stirpy-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 17:24:27.866580 stirpy-1.2.0/stirpy.egg-info/
--rw-rw-rw-   0        0        0      413 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 17:24:27.000000 stirpy-1.2.0/stirpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 17:50:23.198789 stirpy-1.2.5/
+-rw-rw-rw-   0        0        0      413 2023-04-28 17:50:23.198789 stirpy-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:50:23.198789 stirpy-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      493 2023-04-28 17:50:16.000000 stirpy-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:50:23.198789 stirpy-1.2.5/stirpy.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-04-28 17:50:22.000000 stirpy-1.2.5/stirpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-28 17:50:22.000000 stirpy-1.2.5/stirpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:50:22.000000 stirpy-1.2.5/stirpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-28 17:50:22.000000 stirpy-1.2.5/stirpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:50:22.000000 stirpy-1.2.5/stirpy.egg-info/top_level.txt
```

