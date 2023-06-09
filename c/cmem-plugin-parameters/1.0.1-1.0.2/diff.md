# Comparing `tmp/cmem_plugin_parameters-1.0.1.tar.gz` & `tmp/cmem_plugin_parameters-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_parameters-1.0.1.tar", max compression
+gzip compressed data, was "cmem_plugin_parameters-1.0.2.tar", max compression
```

## Comparing `cmem_plugin_parameters-1.0.1.tar` & `cmem_plugin_parameters-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11334 2023-02-06 08:03:35.294494 cmem_plugin_parameters-1.0.1/LICENSE
--rw-r--r--   0        0        0      364 2023-02-06 08:03:35.294494 cmem_plugin_parameters-1.0.1/README-public.md
--rw-r--r--   0        0        0     3302 2023-02-06 08:03:35.298495 cmem_plugin_parameters-1.0.1/cmem_plugin_parameters/__init__.py
--rw-r--r--   0        0        0     1682 2023-02-06 08:04:28.481381 cmem_plugin_parameters-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 cmem_plugin_parameters-1.0.1/setup.py
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 cmem_plugin_parameters-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/LICENSE
+-rw-r--r--   0        0        0      364 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/README-public.md
+-rw-r--r--   0        0        0     3301 2023-04-28 10:30:21.343782 cmem_plugin_parameters-1.0.2/cmem_plugin_parameters/__init__.py
+-rw-r--r--   0        0        0     1653 2023-04-28 10:30:55.846243 cmem_plugin_parameters-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 cmem_plugin_parameters-1.0.2/PKG-INFO
```

### Comparing `cmem_plugin_parameters-1.0.1/LICENSE` & `cmem_plugin_parameters-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_parameters-1.0.1/cmem_plugin_parameters/__init__.py` & `cmem_plugin_parameters-1.0.2/cmem_plugin_parameters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
             self.entities, self.total_params = yaml_to_entities(parameters)
         except YAMLError as error:
             raise ValueError(f"Error in parameter input: {str(error)}") from error
 
     def execute(
         self, inputs: Sequence[Entities], context: ExecutionContext
     ) -> Entities:
-
         context.report.update(
             ExecutionReport(
                 entity_count=self.total_params,
                 operation="write",
                 operation_desc="parameters",
             )
         )
```

### Comparing `cmem_plugin_parameters-1.0.1/pyproject.toml` & `cmem_plugin_parameters-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 [tool.poetry]
 name = "cmem-plugin-parameters"
-version = "1.0.1"
+version = "1.0.2"
 license = "Apache-2.0"
 description = "Set or overwrite parameters of a task."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin", "yaml", "parameters"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-parameters"
 
+
 [tool.poetry.dependencies]
 python = "^3.9"
-cmem-plugin-base = "^2.1.0"
+cmem-plugin-base = "^3.1.0"
 PyYAML = "^6.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^4.0.0"
-pytest-memray = "^1.3.0"
-black = "^22.1.0"
-bandit = "^1.7.2"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^0.991"
-coverage = "^6.3.2"
-defusedxml = "^0.7.1"
-wheel = "^0.38.3"
-
-[tool.poetry.group.dev.dependencies]
+typed-ast = "^1.5.4"
+wheel = "^0.38.4"
 types-PyYAML = "^6.0.12"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `cmem_plugin_parameters-1.0.1/PKG-INFO` & `cmem_plugin_parameters-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-parameters
-Version: 1.0.1
+Version: 1.0.2
 Summary: Set or overwrite parameters of a task.
 Home-page: https://github.com/eccenca/cmem-plugin-parameters
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,yaml,parameters
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: cmem-plugin-base (>=2.1.0,<3.0.0)
+Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-parameters
 
 eccenca Corporate Memory Workflow plugin for parameter input
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

