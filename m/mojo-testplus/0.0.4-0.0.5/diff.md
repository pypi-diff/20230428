# Comparing `tmp/mojo_testplus-0.0.4.tar.gz` & `tmp/mojo_testplus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_testplus-0.0.4.tar", max compression
+gzip compressed data, was "mojo_testplus-0.0.5.tar", max compression
```

## Comparing `mojo_testplus-0.0.4.tar` & `mojo_testplus-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      195 2023-03-23 07:27:52.484881 mojo_testplus-0.0.4/README.md
--rw-r--r--   0        0        0      696 2023-04-19 06:06:27.030557 mojo_testplus-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      551 2023-03-23 14:26:34.599237 mojo_testplus-0.0.4/source/packages/mojo/factories/testplusfactory.py
--rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.4/source/packages/mojo/testplus/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
--rw-r--r--   0        0        0     6102 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
--rw-r--r--   0        0        0     4130 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
--rw-r--r--   0        0        0    13150 2023-04-19 06:05:41.489797 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
--rw-r--r--   0        0        0     1421 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/testplus_command.py
--rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/constraints.py
--rw-r--r--   0        0        0      556 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/diagnostics.py
--rw-r--r--   0        0        0     5089 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/entrypoints.py
--rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.4/source/packages/mojo/testplus/exceptions.py
--rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/expressions.py
--rw-r--r--   0        0        0      352 2023-03-23 14:25:46.434788 mojo_testplus-0.0.4/source/packages/mojo/testplus/extensionpoints.py
--rw-r--r--   0        0        0     1225 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/initialize.py
--rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/jsos.py
--rw-r--r--   0        0        0     7403 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/markers.py
--rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/parameters.py
--rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/queries.py
--rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/recorders.py
--rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.4/source/packages/mojo/testplus/reflection.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/__init__.py
--rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/integrationsource.py
--rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/parameterorigin.py
--rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourceregistry.py
--rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcescope.py
--rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcesource.py
--rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/scopesource.py
--rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/sourcebase.py
--rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/unknownsource.py
--rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/resourcelifespan.py
--rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/resources.py
--rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.4/source/packages/mojo/testplus/results.py
--rwxr-xr-x   0        0        0      959 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/__init__.py
--rw-r--r--   0        0        0    10399 2023-04-19 05:52:19.472744 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.css
--rw-r--r--   0        0        0    38006 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.js
--rw-r--r--   0        0        0    23424 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/w3.css
--rw-r--r--   0        0        0     3190 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-images.html
--rw-r--r--   0        0        0     3385 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-sounds.html
--rwxr-xr-x   0        0        0     6714 2023-04-19 05:52:19.472744 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/testsummary.html
--rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/testcollector.py
--rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.4/source/packages/mojo/testplus/testgroup.py
--rwxr-xr-x   0        0        0    17780 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/testjob.py
--rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/testref.py
--rw-r--r--   0        0        0    37901 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/testsequencer.py
--rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.4/source/packages/mojo/testplus/utilities.py
--rw-r--r--   0        0        0    17353 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/verification.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 mojo_testplus-0.0.4/setup.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 mojo_testplus-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      195 2023-03-23 07:27:52.484881 mojo_testplus-0.0.5/README.md
+-rw-r--r--   0        0        0      704 2023-04-28 01:18:41.245061 mojo_testplus-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-04-21 02:42:40.372545 mojo_testplus-0.0.5/source/packages/mojo/factories/testplusfactory.py
+-rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.5/source/packages/mojo/testplus/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
+-rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
+-rw-r--r--   0        0        0     6102 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
+-rw-r--r--   0        0        0     4130 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
+-rw-r--r--   0        0        0    13194 2023-04-21 02:42:40.372545 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
+-rw-r--r--   0        0        0     1421 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/testplus_command.py
+-rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/constraints.py
+-rw-r--r--   0        0        0      556 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/diagnostics.py
+-rw-r--r--   0        0        0     5089 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/entrypoints.py
+-rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.5/source/packages/mojo/testplus/exceptions.py
+-rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/expressions.py
+-rw-r--r--   0        0        0      352 2023-03-23 14:25:46.434788 mojo_testplus-0.0.5/source/packages/mojo/testplus/extensionpoints.py
+-rw-r--r--   0        0        0     1532 2023-04-21 02:42:40.368545 mojo_testplus-0.0.5/source/packages/mojo/testplus/initialize.py
+-rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/jsos.py
+-rw-r--r--   0        0        0     7403 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/markers.py
+-rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/parameters.py
+-rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/queries.py
+-rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/recorders.py
+-rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.5/source/packages/mojo/testplus/reflection.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/integrationsource.py
+-rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/parameterorigin.py
+-rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourceregistry.py
+-rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcescope.py
+-rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcesource.py
+-rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/scopesource.py
+-rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/sourcebase.py
+-rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/unknownsource.py
+-rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/resourcelifespan.py
+-rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/resources.py
+-rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.5/source/packages/mojo/testplus/results.py
+-rwxr-xr-x   0        0        0      959 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/__init__.py
+-rw-r--r--   0        0        0    10399 2023-04-19 05:52:19.472744 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.css
+-rw-r--r--   0        0        0    38006 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.js
+-rw-r--r--   0        0        0    23424 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/w3.css
+-rw-r--r--   0        0        0     3190 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     6714 2023-04-19 05:52:19.472744 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/testsummary.html
+-rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/testcollector.py
+-rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.5/source/packages/mojo/testplus/testgroup.py
+-rwxr-xr-x   0        0        0    17780 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/testjob.py
+-rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/testref.py
+-rw-r--r--   0        0        0    37901 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/testsequencer.py
+-rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.5/source/packages/mojo/testplus/utilities.py
+-rw-r--r--   0        0        0    17353 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/verification.py
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 mojo_testplus-0.0.5/setup.py
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 mojo_testplus-0.0.5/PKG-INFO
```

### Comparing `mojo_testplus-0.0.4/LICENSE.txt` & `mojo_testplus-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/pyproject.toml` & `mojo_testplus-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-testplus"
 description = "Automation Mojo TestPlus Test Framework"
-version = "0.0.4"
+version = "0.0.5"
 authors = []
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
@@ -15,15 +15,15 @@
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 debugpy = "^1.6.5"
 click = "^8.1.3"
-mojo-runtime = "^0.0.19"
+mojo-runtime = ">=0.0.20 <0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [build-system]
```

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/factories/testplusfactory.py` & `mojo_testplus-0.0.5/source/packages/mojo/factories/testplusfactory.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 class TestPlusExtensionPointsFactory(ExtensionPointsFactory, TestPlusExtensionPoints):
 
     def get_testplus_default_job_type() -> Type[TestJob]:
         """
             Used to lookup and return the most relevant default job type as determined
             by the super factory search path.
         """
-        return DefaultTestJob
+        return DefaultTestJob
```

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/__init__.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/query.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/query.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/run.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 @click.option("--credential", "credential_files", multiple=True, default=None, required=False, help=HELP_CREDENTIAL)
 @click.option("--credential-name", "credential_names", multiple=True, default=None, required=False, help=HELP_CREDENTIAL_NAMES)
 @click.option("--credential-path", "credential_path", default=None, required=False, help=HELP_CREDENTIAL_PATH)
 @click.option("--landscape", "landscape_files", multiple=True, default=None, required=False, help=HELP_LANDSCAPE)
 @click.option("--landscape-name", "landscape_names", multiple=True, default=None, required=False, help=HELP_LANDSCAPE_NAMES)
 @click.option("--landscape-path", "landscape_path", default=None, required=False, help=HELP_LANDSCAPE_PATH)
 @click.option("--runtime", "runtime_files", multiple=True, default=None, required=False, help=HELP_RUNTIME)
-@click.option("--runtime-name", "runtime_names", default=None, required=False, help=HELP_RUNTIME_NAMES)
+@click.option("--runtime-name", "runtime_names", multiple=True, default=None, required=False, help=HELP_RUNTIME_NAMES)
 @click.option("--runtime-path", "runtime_path", default=None, required=False, help=HELP_RUNTIME_PATH)
 @click.option("--topology", "topology_files", multiple=True, default=None, required=False, help=HELP_TOPOLOGY)
 @click.option("--topology-name", "topology_names", multiple=True, default=None, required=False, help=HELP_TOPOLOGY_NAMES)
 @click.option("--topology-path", "topology_path", default=None, required=False, help=HELP_TOPOLOGY_PATH)
 @click.option("--console-level", default=None, required=False, type=click.Choice(LOG_LEVEL_NAMES, case_sensitive=False), help=HELP_CONSOLE_LOG_LEVEL)
 @click.option("--logfile-level", default=None, required=False, type=click.Choice(LOG_LEVEL_NAMES, case_sensitive=False), help=HELP_FILE_LOG_LEVEL)
 @click.option("--debugger", default=None, required=False, type=click.Choice(['pdb', 'debugpy']), help=HELP_DEBUGGER)
@@ -112,15 +112,15 @@
     from mojo.runtime import optionoverrides
 
     # We perform activation a little later in the testrunner.py file so we can
     # handle exceptions in the context of testrunner_main function
     import mojo.runtime.activation.testrun
 
     from mojo.testplus.initialize import initialize_runtime, initialize_testplus_results
-    initialize_runtime()
+    initialize_runtime(name="mjr", logger_name="MJR")
 
     ctx = Context()
     env = ctx.lookup("/environment")
 
     # We need to set the job type before we trigger activation.
     env["jobtype"] = JobType.TestRun
```

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/testplus_command.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/testplus_command.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/constraints.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/constraints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/diagnostics.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/diagnostics.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/entrypoints.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/entrypoints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/exceptions.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/expressions.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/expressions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/initialize.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/initialize.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 
+
 import os
 
 from mojo.xmods.xcollections.context import Context, ContextPaths
 
-from mojo.runtime.initialize import initialize_runtime
+from mojo.runtime.initialize import initialize_runtime, MOJO_RUNTIME_STATE
 from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 
 TESTPLUS_DIR = os.path.dirname(__file__)
 TEMPLATES_DIR = os.path.join(TESTPLUS_DIR, "templates")
 STATIC_DIR = os.path.join(TEMPLATES_DIR, "static")
 
 def initialize_testplus_runtime():
-    initialize_runtime(name="testplus", logger_name="TP")
+    if not MOJO_RUNTIME_STATE.INITIALIZED:
+        initialize_runtime(name="testplus", logger_name="TP")
     return
 
 def initialize_testplus_results():
     dest_static_dir = os.path.join(MOJO_RUNTIME_VARIABLES.MJR_HOME_DIRECTORY, "results", "static")
 
-    MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR = STATIC_DIR
-    MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR = dest_static_dir
-    MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE = os.path.join(TEMPLATES_DIR, "testsummary.html")
+    if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR is None:
+        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR = STATIC_DIR
+    if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR is None:
+        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR = dest_static_dir
+    if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE is None:
+        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE = os.path.join(TEMPLATES_DIR, "testsummary.html")
 
     ctx = Context()
     ctx.insert(ContextPaths.DIR_RESULTS_RESOURCE_SRC, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR)
     ctx.insert(ContextPaths.DIR_RESULTS_RESOURCE_DEST, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR)
     ctx.insert(ContextPaths.FILE_RESULTS_TEMPLATE, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE)
-    return
+    return
```

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/jsos.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/jsos.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/markers.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/markers.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/parameters.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/parameters.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/queries.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/queries.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/recorders.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/recorders.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/reflection.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/reflection.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/integrationsource.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/integrationsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/parameterorigin.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/parameterorigin.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourceregistry.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourceregistry.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcescope.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcescope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcesource.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/scopesource.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/scopesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/sourcebase.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/sourcebase.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/unknownsource.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/unknownsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/resources.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/resources.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/results.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/results.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/__init__.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.css` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.js` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/w3.css` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/w3.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-images.html` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-images.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-sounds.html` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-sounds.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/testsummary.html` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/testsummary.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/testcollector.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/testcollector.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/testgroup.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/testgroup.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/testjob.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/testjob.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/testref.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/testref.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/testsequencer.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/testsequencer.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/utilities.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/source/packages/mojo/testplus/verification.py` & `mojo_testplus-0.0.5/source/packages/mojo/testplus/verification.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.4/setup.py` & `mojo_testplus-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  'mojo.testplus.registration',
  'mojo.testplus.templates']
 
 package_data = \
 {'': ['*'], 'mojo.testplus.templates': ['static/v0/*', 'tabs/*']}
 
 install_requires = \
-['click>=8.1.3,<9.0.0', 'debugpy>=1.6.5,<2.0.0', 'mojo-runtime>=0.0.19,<0.0.20']
+['click>=8.1.3,<9.0.0', 'debugpy>=1.6.5,<2.0.0', 'mojo-runtime>=0.0.20,<0.1.0']
 
 setup_kwargs = {
     'name': 'mojo-testplus',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Automation Mojo TestPlus Test Framework',
     'long_description': "# Automation Mojo - Testplus \nThis is preliminary release of the 'testplus' automation framework in a separate package from\nthe AutomationKit.  This release is not ready for public consumption.\n\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_testplus-0.0.4/PKG-INFO` & `mojo_testplus-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-testplus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automation Mojo TestPlus Test Framework
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: debugpy (>=1.6.5,<2.0.0)
-Requires-Dist: mojo-runtime (>=0.0.19,<0.0.20)
+Requires-Dist: mojo-runtime (>=0.0.20,<0.1.0)
 Description-Content-Type: text/markdown
 
 # Automation Mojo - Testplus 
 This is preliminary release of the 'testplus' automation framework in a separate package from
 the AutomationKit.  This release is not ready for public consumption.
```

