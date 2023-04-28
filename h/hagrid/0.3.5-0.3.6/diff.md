# Comparing `tmp/hagrid-0.3.5.tar.gz` & `tmp/hagrid-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.5.tar", last modified: Thu Apr 27 05:52:26 2023, max compression
+gzip compressed data, was "hagrid-0.3.6.tar", last modified: Fri Apr 28 03:28:55 2023, max compression
```

## Comparing `hagrid-0.3.5.tar` & `hagrid-0.3.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:52:26.928618 hagrid-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:52:26.928618 hagrid-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-27 05:49:40.000000 hagrid-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:52:26.924618 hagrid-0.3.5/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134776 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-27 05:49:59.000000 hagrid-0.3.5/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-27 05:49:59.000000 hagrid-0.3.5/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-27 05:49:40.000000 hagrid-0.3.5/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:52:26.928618 hagrid-0.3.5/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 05:52:26.000000 hagrid-0.3.5/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:52:26.928618 hagrid-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-27 05:49:59.000000 hagrid-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:52:26.928618 hagrid-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:49:40.000000 hagrid-0.3.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:52:26.928618 hagrid-0.3.5/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:49:40.000000 hagrid-0.3.5/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-27 05:49:40.000000 hagrid-0.3.5/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 03:28:55.537100 hagrid-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-28 03:26:22.000000 hagrid-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.533100 hagrid-0.3.6/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134780 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 03:26:38.000000 hagrid-0.3.6/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 03:26:38.000000 hagrid-0.3.6/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:28:55.537100 hagrid-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 03:26:38.000000 hagrid-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.5/README.md` & `hagrid-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/__init__.py` & `hagrid-0.3.6/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/art.py` & `hagrid-0.3.6/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/auth.py` & `hagrid-0.3.6/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/azure.py` & `hagrid-0.3.6/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/cache.py` & `hagrid-0.3.6/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/cli.py` & `hagrid-0.3.6/hagrid/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         grammar = parse_grammar(args=args, verb=verb)
         verb.load_grammar(grammar=grammar)
     except BadGrammar as e:
         print(e)
         return
 
     try:
-        update_repo(repo=GIT_REPO, branch=str(kwargs["build_src"]))
+        update_repo(repo=GIT_REPO(), branch=str(kwargs["build_src"]))
     except Exception as e:
         print(f"Failed to update repo. {e}")
     try:
         cmds = create_launch_cmd(verb=verb, kwargs=kwargs)
         cmds = [cmds] if isinstance(cmds, str) else cmds
     except Exception as e:
         print(f"Error: {e}\n\n")
@@ -3040,15 +3040,15 @@
         grammar = parse_grammar(args=args, verb=verb)
         verb.load_grammar(grammar=grammar)
     except BadGrammar as e:
         print(e)
         return
 
     try:
-        update_repo(repo=GIT_REPO, branch=str(kwargs["build_src"]))
+        update_repo(repo=GIT_REPO(), branch=str(kwargs["build_src"]))
     except Exception as e:
         print(f"Failed to update repo. {e}")
 
     try:
         cmd = create_land_cmd(verb=verb, kwargs=kwargs)
     except Exception as e:
         print(f"{e}")
```

### Comparing `hagrid-0.3.5/hagrid/deps.py` & `hagrid-0.3.6/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/grammar.py` & `hagrid-0.3.6/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/land.py` & `hagrid-0.3.6/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/launch.py` & `hagrid-0.3.6/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/lib.py` & `hagrid-0.3.6/hagrid/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
     # relative
     from .art import RichEmoji
 
     OK_EMOJI = RichEmoji("white_heavy_check_mark").to_str()
 
     is_git = check_is_git(path=repo_src_path())
     console = rich.get_console()
+
     if not EDITABLE_MODE and not is_git:
         github_repo = "OpenMined/PySyft.git"
         git_url = f"https://github.com/{github_repo}"
 
         print(f"Fetching Syft + Grid Source from {git_url} to {repo_src_path()}")
         try:
             repo_branch = DEFAULT_BRANCH
@@ -459,10 +460,10 @@
             return False
     except Exception as e:
         if not silent:
             print(f"Failed to check jupyter server status {host_ip}. {e}")
         return False
 
 
-GIT_REPO = get_git_repo()
+GIT_REPO = get_git_repo
 GRID_SRC_VERSION = get_version_module()
 GRID_SRC_PATH = grid_src_path()
```

### Comparing `hagrid-0.3.5/hagrid/manifest_template.yml` & `hagrid-0.3.6/hagrid/manifest_template.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.5
+hagrid_version: 0.3.6
 syft_version: 0.8.0
 dockerTag: 0.8.0
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: 062eeb50caf5309d21663e59eb6b345f6815d732
+hash: ed14ea50ece31c8654b229f65e2c598eef1d1a7a
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.5/hagrid/mode.py` & `hagrid-0.3.6/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/names.py` & `hagrid-0.3.6/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/orchestra.py` & `hagrid-0.3.6/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/parse_template.py` & `hagrid-0.3.6/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/quickstart_ui.py` & `hagrid-0.3.6/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/rand_sec.py` & `hagrid-0.3.6/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/style.py` & `hagrid-0.3.6/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/util.py` & `hagrid-0.3.6/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/win_bootstrap.py` & `hagrid-0.3.6/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid/wizard_ui.py` & `hagrid-0.3.6/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.6/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.5/setup.py` & `hagrid-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.5/tests/hagrid/cli_test.py` & `hagrid-0.3.6/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

