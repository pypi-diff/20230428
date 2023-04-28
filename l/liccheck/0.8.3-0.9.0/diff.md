# Comparing `tmp/liccheck-0.8.3.tar.gz` & `tmp/liccheck-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liccheck-0.8.3.tar", last modified: Thu Jan  5 07:50:45 2023, max compression
+gzip compressed data, was "liccheck-0.9.0.tar", last modified: Fri Apr 28 14:38:48 2023, max compression
```

## Comparing `liccheck-0.8.3.tar` & `liccheck-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:50:45.035164 liccheck-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-05 07:50:42.000000 liccheck-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-05 07:50:45.035164 liccheck-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-01-05 07:50:42.000000 liccheck-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:50:45.035164 liccheck-0.8.3/liccheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:50:42.000000 liccheck-0.8.3/liccheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-05 07:50:42.000000 liccheck-0.8.3/liccheck/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-01-05 07:50:42.000000 liccheck-0.8.3/liccheck/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-05 07:50:42.000000 liccheck-0.8.3/liccheck/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:50:45.035164 liccheck-0.8.3/liccheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-05 07:50:45.000000 liccheck-0.8.3/liccheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-05 07:50:45.035164 liccheck-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-01-05 07:50:42.000000 liccheck-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 14:38:46.000000 liccheck-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 14:38:48.173187 liccheck-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-04-28 14:38:46.000000 liccheck-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/liccheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-28 14:38:46.000000 liccheck-0.9.0/liccheck/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:38:48.173187 liccheck-0.9.0/liccheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 14:38:48.000000 liccheck-0.9.0/liccheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 14:38:48.173187 liccheck-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-28 14:38:46.000000 liccheck-0.9.0/setup.py
```

### Comparing `liccheck-0.8.3/LICENSE` & `liccheck-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liccheck-0.8.3/PKG-INFO` & `liccheck-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liccheck
-Version: 0.8.3
+Version: 0.9.0
 Summary: Check python packages from requirement.txt and report issues
 Home-page: https://github.com/dhatim/python-license-check
 Author: Dhatim
 Author-email: contact@dhatim.com
 License: Apache Software License
 Keywords: license check build tool
 Platform: UNKNOWN
```

### Comparing `liccheck-0.8.3/README.rst` & `liccheck-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `liccheck-0.8.3/liccheck/command_line.py` & `liccheck-0.9.0/liccheck/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,29 +451,37 @@
         "optional_dependencies": config.get(
             "optional_dependencies", args["optional_dependencies"]
         ),
         "as_regex": config.get("as_regex", args["as_regex"]),
     }
 
 
-def generate_requirements_file_from_pyproject(include_dependencies, extra_dependencies):
+def generate_requirements_file_from_pyproject(include_dependencies, optional_dependencies):
     import tempfile
 
     directory = tempfile.mkdtemp(prefix="liccheck_")
     requirements_txt_file = directory + "/requirements.txt"
     with open(requirements_txt_file, "w") as f:
-        project = toml.load("pyproject.toml").get("project", {})
-        dependencies = project.get("dependencies", []) if include_dependencies else []
-        optional_dependencies = (
-            project.get("optional-dependencies", {}) if extra_dependencies else {}
-        )
-        for extra_dependency in extra_dependencies:
-            if extra_dependency in optional_dependencies:
-                dependencies += optional_dependencies[extra_dependency]
-        f.write(os.linesep.join(dependencies))
+        ptoml = toml.load("pyproject.toml")
+        project = ptoml.get("project", {})
+        poetry = ptoml.get("tool", {}).get('poetry', {})
+        dependencies = set()
+        if include_dependencies:
+            dependencies |= set(project.get("dependencies", []))
+            dependencies |= set(d for d, v in poetry.get("dependencies", {}).items() 
+                                if d != 'python' and (not isinstance(v, dict) or not v.get('optional')))
+        if optional_dependencies:
+            extra_dependency = project.get("optional-dependencies", {})
+            extra_dependency.update(poetry.get("extras", {}))
+            if '*' in optional_dependencies:
+                optional_dependencies = extra_dependency.keys()
+            for opt in optional_dependencies:
+                extralist = extra_dependency.get(opt, [])
+                dependencies |= set(extralist)
+        f.write(os.linesep.join(sorted(dependencies)))
     return requirements_txt_file
 
 
 def run(args):
     args = merge_args(
         {
             "strategy_ini_file": args.strategy_ini_file,
```

### Comparing `liccheck-0.8.3/liccheck/requirements.py` & `liccheck-0.9.0/liccheck/requirements.py`

 * *Files identical despite different names*

### Comparing `liccheck-0.8.3/liccheck.egg-info/PKG-INFO` & `liccheck-0.9.0/liccheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liccheck
-Version: 0.8.3
+Version: 0.9.0
 Summary: Check python packages from requirement.txt and report issues
 Home-page: https://github.com/dhatim/python-license-check
 Author: Dhatim
 Author-email: contact@dhatim.com
 License: Apache Software License
 Keywords: license check build tool
 Platform: UNKNOWN
```

### Comparing `liccheck-0.8.3/setup.py` & `liccheck-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name='liccheck',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.8.3',
+    version='0.9.0',
 
     description='Check python packages from requirement.txt and report issues',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/dhatim/python-license-check',
```

