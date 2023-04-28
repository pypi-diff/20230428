# Comparing `tmp/shift_left_secure-0.1.2.tar.gz` & `tmp/shift_left_secure-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shift_left_secure-0.1.2.tar", max compression
+gzip compressed data, was "shift_left_secure-0.2.0.tar", max compression
```

## Comparing `shift_left_secure-0.1.2.tar` & `shift_left_secure-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      252 2023-03-29 09:04:22.240291 shift_left_secure-0.1.2/README.md
--rw-r--r--   0        0        0      464 2023-03-29 13:07:34.883220 shift_left_secure-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.1.2/shift_left_secure/__init__.py
--rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.1.2/shift_left_secure/__main__.py
--rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.1.2/shift_left_secure/chatgpt_api.py
--rw-r--r--   0        0        0     3773 2023-03-29 13:06:38.175643 shift_left_secure-0.1.2/shift_left_secure/git_handler.py
--rw-r--r--   0        0        0     1608 2023-03-29 12:37:50.265850 shift_left_secure-0.1.2/shift_left_secure/utils.py
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 shift_left_secure-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1601 2023-04-27 17:41:42.013917 shift_left_secure-0.2.0/README.md
+-rw-r--r--   0        0        0      516 2023-04-28 09:39:26.150186 shift_left_secure-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-29 04:11:10.773184 shift_left_secure-0.2.0/shift_left_secure/__init__.py
+-rw-r--r--   0        0        0     1238 2023-03-29 12:35:12.607718 shift_left_secure-0.2.0/shift_left_secure/__main__.py
+-rw-r--r--   0        0        0     2843 2023-03-29 11:50:35.517189 shift_left_secure-0.2.0/shift_left_secure/chatgpt_api.py
+-rw-r--r--   0        0        0     2504 2023-04-28 06:51:55.743407 shift_left_secure-0.2.0/shift_left_secure/gh_action.py
+-rw-r--r--   0        0        0     3773 2023-04-27 18:47:23.586572 shift_left_secure-0.2.0/shift_left_secure/git_handler.py
+-rw-r--r--   0        0        0     2978 2023-04-28 06:51:55.743681 shift_left_secure-0.2.0/shift_left_secure/utils.py
+-rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 shift_left_secure-0.2.0/PKG-INFO
```

### Comparing `shift_left_secure-0.1.2/shift_left_secure/__main__.py` & `shift_left_secure-0.2.0/shift_left_secure/__main__.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.1.2/shift_left_secure/chatgpt_api.py` & `shift_left_secure-0.2.0/shift_left_secure/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `shift_left_secure-0.1.2/shift_left_secure/git_handler.py` & `shift_left_secure-0.2.0/shift_left_secure/git_handler.py`

 * *Files identical despite different names*

