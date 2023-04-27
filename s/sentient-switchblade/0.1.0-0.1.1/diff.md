# Comparing `tmp/sentient_switchblade-0.1.0.tar.gz` & `tmp/sentient_switchblade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.1.0.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.1.1.tar", max compression
```

## Comparing `sentient_switchblade-0.1.0.tar` & `sentient_switchblade-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.1.0/LICENSE
--rw-r--r--   0        0        0     1359 2023-04-25 19:36:46.615130 sentient_switchblade-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.1.0/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.1.0/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1656 2023-04-26 17:36:40.891577 sentient_switchblade-0.1.0/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    10671 2023-04-25 19:26:37.194064 sentient_switchblade-0.1.0/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.1.0/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:46.529573 sentient_switchblade-0.1.0/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:50.583261 sentient_switchblade-0.1.0/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.1.0/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.1.0/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0     9535 2023-04-26 17:36:59.378665 sentient_switchblade-0.1.0/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.1.0/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.0/setup.py
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6679 2023-04-27 22:35:37.645490 sentient_switchblade-0.1.1/README.md
+-rw-r--r--   0        0        0     1383 2023-04-27 22:46:35.896183 sentient_switchblade-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.1.1/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.1.1/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1656 2023-04-26 17:36:40.891577 sentient_switchblade-0.1.1/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    10671 2023-04-25 19:26:37.194064 sentient_switchblade-0.1.1/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.1.1/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0      820 2023-04-26 17:36:46.529573 sentient_switchblade-0.1.1/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0      820 2023-04-26 17:36:50.583261 sentient_switchblade-0.1.1/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.1.1/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.1.1/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0     9535 2023-04-26 17:36:59.378665 sentient_switchblade-0.1.1/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.1.1/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.1/setup.py
+-rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.1/PKG-INFO
```

### Comparing `sentient_switchblade-0.1.0/LICENSE` & `sentient_switchblade-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/pyproject.toml` & `sentient_switchblade-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.1.0"
+version = "0.1.1"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
-homepage = "https://kegstand.dev/sentient-switchblade"
+homepage = "https://jensroland.com/sentient-switchblade"
+readme = "README.md"
 packages = [
     { include = "switchbladecli", from = "src" },
 ]
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
@@ -29,15 +30,15 @@
 [tool.poetry.scripts]
 swb = "switchbladecli.cli.__main__:switchbladecli"
 
 [tool.poetry.dependencies]
 checksumdir = "^1.2.0"
 click = "^8.0.3"
 PyGithub = "^1.58.1"
-python = "^3.9"
+python = "^3.7"
 tomlkit = "^0.11.7"
 
 [tool.poetry.group.dev.dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.1.1/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.1.1/src/switchbladecli/cli/bundle_cache.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.1.1/src/switchbladecli/cli/lint.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.1.1/src/switchbladecli/cli/test.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/cli/update.py` & `sentient_switchblade-0.1.1/src/switchbladecli/cli/update.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.1.1/src/switchbladecli/modes/python_poetry.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.0/src/switchbladecli/utils.py` & `sentient_switchblade-0.1.1/src/switchbladecli/utils.py`

 * *Files identical despite different names*

