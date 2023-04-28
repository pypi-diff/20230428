# Comparing `tmp/prepipy-0.6.3.tar.gz` & `tmp/prepipy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepipy-0.6.3.tar", max compression
+gzip compressed data, was "prepipy-0.6.4.tar", max compression
```

## Comparing `prepipy-0.6.3.tar` & `prepipy-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.3/LICENSE
--rw-r--r--   0        0        0     1104 2023-04-23 23:31:54.314610 prepipy-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2049 2023-03-19 20:16:59.384002 prepipy-0.6.3/README.md
--rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.3/src/prepipy/__init__.py
--rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.3/src/prepipy/auxiliaries.py
--rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.3/src/prepipy/config/config_comments.yml
--rw-r--r--   0        0        0      870 2023-04-23 23:31:32.143543 prepipy-0.6.3/src/prepipy/config/logging_config.yml
--rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.3/src/prepipy/config/masking_example.yml
--rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.3/src/prepipy/config_file_examples/bands.yml
--rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.3/src/prepipy/config_file_examples/config_single.yml
--rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.3/src/prepipy/config_file_examples/mask.yml
--rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.3/src/prepipy/configuration.py
--rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.3/src/prepipy/framework.py
--rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.3/src/prepipy/framework_sources.py
--rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.3/src/prepipy/masking.py
--rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.3/src/prepipy/resources/grey_values.yml
--rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.3/src/prepipy/resources/html_templates.yml
--rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.3/src/prepipy/resources/stiff_params.yml
--rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.3/src/prepipy/rgbcombo.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 prepipy-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.4/LICENSE
+-rw-r--r--   0        0        0     1104 2023-04-28 17:17:22.866742 prepipy-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6507 2023-04-28 17:16:37.889028 prepipy-0.6.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.4/src/prepipy/__init__.py
+-rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.4/src/prepipy/auxiliaries.py
+-rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.4/src/prepipy/config/config_comments.yml
+-rw-r--r--   0        0        0      870 2023-04-23 23:31:32.143543 prepipy-0.6.4/src/prepipy/config/logging_config.yml
+-rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.4/src/prepipy/config/masking_example.yml
+-rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/bands.yml
+-rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/config_single.yml
+-rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/mask.yml
+-rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.4/src/prepipy/configuration.py
+-rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.4/src/prepipy/framework.py
+-rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.4/src/prepipy/framework_sources.py
+-rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.4/src/prepipy/masking.py
+-rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.4/src/prepipy/resources/grey_values.yml
+-rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.4/src/prepipy/resources/html_templates.yml
+-rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.4/src/prepipy/resources/stiff_params.yml
+-rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.4/src/prepipy/rgbcombo.py
+-rw-r--r--   0        0        0     7831 1970-01-01 00:00:00.000000 prepipy-0.6.4/PKG-INFO
```

### Comparing `prepipy-0.6.3/LICENSE` & `prepipy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/pyproject.toml` & `prepipy-0.6.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prepipy"
-version = "0.6.3"
+version = "0.6.4"
 description = "Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images."
 authors = ["Fabian Haberhauer <fabian.haberhauer@univie.ac.at>"]
 maintainers = ["teutoburg <ghost@instruct.at>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/teutoburg/prepipy"
 classifiers = [
```

### Comparing `prepipy-0.6.3/src/prepipy/auxiliaries.py` & `prepipy-0.6.4/src/prepipy/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/config/config_comments.yml` & `prepipy-0.6.4/src/prepipy/config/config_comments.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/config/logging_config.yml` & `prepipy-0.6.4/src/prepipy/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/config/masking_example.yml` & `prepipy-0.6.4/src/prepipy/config/masking_example.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/config_file_examples/bands.yml` & `prepipy-0.6.4/src/prepipy/config_file_examples/bands.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/config_file_examples/config_single.yml` & `prepipy-0.6.4/src/prepipy/config_file_examples/config_single.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/configuration.py` & `prepipy-0.6.4/src/prepipy/configuration.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/framework.py` & `prepipy-0.6.4/src/prepipy/framework.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/framework_sources.py` & `prepipy-0.6.4/src/prepipy/framework_sources.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/masking.py` & `prepipy-0.6.4/src/prepipy/masking.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/resources/html_templates.yml` & `prepipy-0.6.4/src/prepipy/resources/html_templates.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.3/src/prepipy/rgbcombo.py` & `prepipy-0.6.4/src/prepipy/rgbcombo.py`

 * *Files identical despite different names*

