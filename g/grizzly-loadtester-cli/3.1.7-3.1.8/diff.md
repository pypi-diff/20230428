# Comparing `tmp/grizzly-loadtester-cli-3.1.7.tar.gz` & `tmp/grizzly-loadtester-cli-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-cli-3.1.7.tar", last modified: Fri Apr 28 09:16:56 2023, max compression
+gzip compressed data, was "grizzly-loadtester-cli-3.1.8.tar", last modified: Fri Apr 28 10:25:04 2023, max compression
```

## Comparing `grizzly-loadtester-cli-3.1.7.tar` & `grizzly-loadtester-cli-3.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27696 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/script/docs-generate-licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.971810 grizzly-loadtester-cli-3.1.8/grizzly_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.971810 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.971810 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/grizzly_cli/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/static/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/static/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    28194 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/grizzly_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 10:25:04.000000 grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-28 10:24:43.000000 grizzly-loadtester-cli-3.1.8/script/docs-generate-licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:25:04.975810 grizzly-loadtester-cli-3.1.8/setup.cfg
```

### Comparing `grizzly-loadtester-cli-3.1.7/LICENSE.md` & `grizzly-loadtester-cli-3.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/PKG-INFO` & `grizzly-loadtester-cli-3.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.7
+Version: 3.1.8
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/__init__.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/__main__.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/__init__.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/__init__.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/bashcompletion.bash` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/bashcompletion.bash`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/types.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/bashcompletion/types.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/markdown.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/argparse/markdown.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/__init__.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/build.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/build.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/clean.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/distributed/clean.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/init.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/init.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/local.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/local.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/run.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/run.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/static/Containerfile` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/static/Containerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/static/compose.yaml` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/static/compose.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_cli/utils.py` & `grizzly-loadtester-cli-3.1.8/grizzly_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,20 +141,29 @@
         return (None, None,), None
 
     if grizzly_requirement is None:
         print(f'!! unable to find grizzly dependency in {project_requirements}', file=sys.stderr)
         return ('(unknown)', None, ), '(unknown)'
 
     # check if it's a repo or not
-    if grizzly_requirement.startswith('git+'):
-        suffix = sha1(grizzly_requirement.encode('utf-8')).hexdigest()
-        url, egg_part = grizzly_requirement.rsplit('#', 1)
+    if 'git+' in grizzly_requirement:
+        if grizzly_requirement.startswith('git+'):
+            url, egg_part = grizzly_requirement.rsplit('#', 1)
+            _, grizzly_requirement_egg = egg_part.split('=', 1)
+        elif grizzly_requirement.index('@') < grizzly_requirement.index('git+'):
+            grizzly_requirement_egg, url = grizzly_requirement.split('@', 1)
+            grizzly_requirement_egg = grizzly_requirement_egg.strip()
+            url = url.strip()
+        else:
+            print(f'!! unable to find properly formatted grizzly dependency in {project_requirements}', file=sys.stderr)
+            return ('(unknown)', None, ), '(unknown)'
+
         url, branch = url.rsplit('@', 1)
         url = url[4:]  # remove git+
-        _, grizzly_requirement_egg = egg_part.split('=', 1)
+        suffix = sha1(grizzly_requirement.encode('utf-8')).hexdigest()
 
         # extras_requirement normalization
         egg = grizzly_requirement_egg.replace('[', '__').replace(']', '__').replace(',', '_')
 
         tmp_workspace = mkdtemp(prefix='grizzly-cli-')
         repo_destination = path.join(tmp_workspace, f'{egg}_{suffix}')
```

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/PKG-INFO` & `grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.7
+Version: 3.1.8
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/SOURCES.txt` & `grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/requires.txt` & `grizzly-loadtester-cli-3.1.8/grizzly_loadtester_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/pyproject.toml` & `grizzly-loadtester-cli-3.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.7/script/docs-generate-licenses.py` & `grizzly-loadtester-cli-3.1.8/script/docs-generate-licenses.py`

 * *Files identical despite different names*

