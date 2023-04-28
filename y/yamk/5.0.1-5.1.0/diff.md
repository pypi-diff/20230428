# Comparing `tmp/yamk-5.0.1.tar.gz` & `tmp/yamk-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamk-5.0.1.tar", max compression
+gzip compressed data, was "yamk-5.1.0.tar", max compression
```

## Comparing `yamk-5.0.1.tar` & `yamk-5.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:46.425974 yamk-5.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2086 2023-03-10 17:25:46.697939 yamk-5.0.1/README.rst
--rw-r--r--   0        0        0     2450 2023-03-15 16:06:56.814108 yamk-5.0.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-03-15 16:06:56.821974 yamk-5.0.1/src/yamk/__init__.py
--rw-r--r--   0        0        0     3118 2023-02-28 15:55:59.735141 yamk-5.0.1/src/yamk/functions.py
--rw-r--r--   0        0        0    13151 2023-03-15 13:49:55.823205 yamk-5.0.1/src/yamk/lib.py
--rw-r--r--   0        0        0     2817 2023-03-15 13:46:25.800131 yamk-5.0.1/src/yamk/main.py
--rw-r--r--   0        0        0    10658 2023-03-15 13:29:18.722813 yamk-5.0.1/src/yamk/make.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:46.427326 yamk-5.0.1/src/yamk/py.typed
--rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 yamk-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:46.425974 yamk-5.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-03-29 13:55:28.435717 yamk-5.1.0/README.rst
+-rw-r--r--   0        0        0     2807 2023-04-28 08:37:33.723617 yamk-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-28 08:37:33.727239 yamk-5.1.0/src/yamk/__init__.py
+-rw-r--r--   0        0        0     3908 2023-04-24 22:20:47.244840 yamk-5.1.0/src/yamk/functions.py
+-rw-r--r--   0        0        0    13526 2023-04-24 21:32:25.497194 yamk-5.1.0/src/yamk/lib.py
+-rw-r--r--   0        0        0     2847 2023-04-24 21:32:10.325884 yamk-5.1.0/src/yamk/main.py
+-rw-r--r--   0        0        0    10738 2023-04-24 22:12:01.439305 yamk-5.1.0/src/yamk/make.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:46.427326 yamk-5.1.0/src/yamk/py.typed
+-rw-r--r--   0        0        0       79 2023-04-24 20:29:05.284987 yamk-5.1.0/src/yamk/types.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 yamk-5.1.0/PKG-INFO
```

### Comparing `yamk-5.0.1/LICENSE.txt` & `yamk-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yamk-5.0.1/README.rst` & `yamk-5.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -30,22 +30,19 @@
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
-The easiest way is to use pip to install ``yam``.
+The easiest way is to use `pipx`_ to install ``yam``.
 
 .. code:: console
 
-   $ pip install --user yamk
-
-Please make sure that the correct directory is added to your path. This
-depends on the OS.
+   $ pipx install yamk
 
 Usage
 ^^^^^
 
 ``yam``'s behaviour is defined in a toml file, called a cookbook. The default name is ``make.toml``,
 but you can specify a different file if you want. Specifying a name ``<name.toml>`` will also parse all the ``.toml``
 files in the directory named ``<name.toml>.d``.
@@ -58,8 +55,9 @@
 -----
 
 - `Documentation`_
 - `Changelog`_
 
 
 .. _Changelog: https://github.com/spapanik/yamk/blob/main/CHANGELOG.rst
-.. _Documentation: https://yamk.readthedocs.io/en/latest/
+.. _Documentation: https://yamk.readthedocs.io/en/stable/
+.. _pipx: https://pypa.github.io/pipx/
```

### Comparing `yamk-5.0.1/pyproject.toml` & `yamk-5.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py38"]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
 no_implicit_reexport = true
 show_error_codes = true
+strict_concatenate = true
+strict_equality = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.ruff]
@@ -58,34 +65,48 @@
     "E501",
     "TRY003",
 ]
 src = ["src"]
 target-version = "py38"
 
 [tool.ruff.per-file-ignores]
-"tests/**" = ["S101"]
+"tests/**" = [
+    "FBT001",
+    "PT011",
+    "S101",
+]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.flake8-tidy-imports.banned-api]
 "mock".msg = "Use unittest.mock"
 "pytz".msg = "Use zoneinfo"
 
+[tool.ruff.isort]
+combine-as-imports = true
+forced-separate = ["tests"]
+split-on-trailing-comma = false
+
 [tool.pytest.ini_options]
-addopts = "-vv --cov --cov-report=term-missing:skip-covered"
+addopts = "-vv"
 testpaths = "tests"
 
 [tool.coverage.run]
 source = ["src/"]
 data_file = ".cov_cache/coverage.dat"
 
+[tool.coverage.report]
+show_missing = true
+skip_covered = true
+skip_empty = true
+
 [tool.poetry]
 name = "yamk"
-version = "5.0.1"
+version = "5.1.0"
 description = "Yet another make"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
@@ -112,22 +133,22 @@
 
 # dependencies
 dj_settings = "^4.2"
 packaging = "^23.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = {version = "^0.13", python = "^3.9"}
-ipython = {version = "^8.11", python = "^3.9"}
-pipdeptree = "^2.5"
+ipython = {version = "^8.12", python = "^3.9"}
+pipdeptree = "^2.7"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.1"
-mypy = "^1.0"
+black = "^23.3"
+mypy = "^1.2"
 ruff = "^0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1"
+pytest = "^7.3"
 pytest-cov = "^4.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1"
+sphinx = "^6.2"
 sphinx-rtd-theme = "^1.2"
```

### Comparing `yamk-5.0.1/src/yamk/lib.py` & `yamk-5.1.0/src/yamk/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import shlex
 import warnings
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from math import ceil, floor
 from pathlib import Path
-from typing import Any, Match, cast
+from typing import Any, Iterator, Literal, Match, cast
 
 from yamk.functions import functions
 
 VAR = re.compile(
     r"(?P<dollars>\$+){(?P<variable>[a-zA-Z0-9_.]+)(?P<sep>:)?(?P<key>[a-zA-Z0-9_.]+)?}"
 )
 OPTIONS = re.compile(r"\[(?P<options>.*?)\](?P<string>.*)")
@@ -37,15 +37,15 @@
     WARNING = "\033[33m"
 
 
 class Recipe:
     def __init__(
         self,
         target: str,
-        raw_recipe,
+        raw_recipe: dict[str, Any],
         base_dir: Path,
         file_vars: dict[str, Any],
         arg_vars: dict[str, Any],
         *,
         specified: bool = False,
     ):
         self._specified = specified
@@ -92,93 +92,93 @@
         else:
             groups = {}
         new_recipe._update_variables(groups)  # noqa: SLF001
         new_recipe._update_requirements()  # noqa: SLF001
         new_recipe._update_commands()  # noqa: SLF001
         return new_recipe
 
-    def _evaluate(self, obj):
+    def _evaluate(self, obj: Any) -> Any:
         parser = Parser(self.vars, self.base_dir)
         return parser.evaluate(obj)
 
-    def _update_variables(self, groups):
+    def _update_variables(self, groups: dict[str, str]) -> None:
         extra_vars = [groups, self.local_vars, {".target": self.target}]
         update_vars(self.vars, extra_vars, self.base_dir)
 
-    def _update_requirements(self):
+    def _update_requirements(self) -> None:
         self.requires = self._evaluate(self.requires)
 
-    def _update_commands(self):
+    def _update_commands(self) -> None:
         extra_vars = [{".requirements": self.requires}]
         update_vars(self.vars, extra_vars, self.base_dir)
         self.commands = self._evaluate(self.commands)
         self.existence_command = self._evaluate(self.existence_command)
 
-    def _alias(self, alias):
+    def _alias(self, alias: str | Literal[False]) -> Any:
         if alias is False:
             return alias
         return self._evaluate(alias)
 
-    def _target(self, target):
+    def _target(self, target: str) -> Any:
         if not self._specified:
             target = self._evaluate(target)
         if not self.phony and not self.alias:
             target = self.base_dir.joinpath(target).as_posix()
         if self.regex and not self._specified:
-            target = re.compile(target)
+            return re.compile(target)
         return target
 
 
 class Parser:
-    def __init__(self, variables, base_dir):
+    def __init__(self, variables: dict[str, Any], base_dir: Path):
         self.vars = variables
         self.base_dir = base_dir
 
     @staticmethod
-    def _stringify(value):
+    def _stringify(value: Any) -> str:
         if isinstance(value, list):
             return " ".join(map(str, value))
         return str(value)
 
-    def expand_function(self, name, args):
-        args = shlex.split(args)
-        for i, arg in enumerate(args):
-            args[i] = self.evaluate(arg)
+    def expand_function(self, name: str, args: str) -> Any:
+        split_args = shlex.split(args)
+        for i, arg in enumerate(split_args):
+            split_args[i] = self.evaluate(arg)
         function = functions[name](self.base_dir)
-        return function(*args)
+        return function(*split_args)
 
-    def repl(self, matchobj):
+    def repl(self, matchobj: re.Match[str]) -> str:
         dollars = matchobj.group("dollars")
         variable = matchobj.group("variable")
         key = matchobj.group("key")
         if len(dollars) % 2:
             value = self.vars.get(variable, "")
             if key is None:
                 return self._stringify(value)
             if isinstance(value, list):
                 key = int(key)
             return self._stringify(value[key])
         return f"{'$'*(len(dollars)//2)}{{{variable}}}"
 
-    def substitute(self, string):
+    def substitute(self, string: str) -> Any:
         function = re.fullmatch(FUNCTION, string)
         if function is not None:
             return self.expand_function(**function.groupdict())
 
         if (
             string.startswith("$")
             and not string.startswith("$$")
             and re.fullmatch(VAR, string)
         ):
             match = cast(Match[str], re.fullmatch(VAR, string))
             if match["sep"] is None:
                 return self.vars[match["variable"]]
         return re.sub(VAR, self.repl, string)
 
-    def evaluate(self, obj):
+    def evaluate(self, obj: str | list[Any] | dict[str, Any]) -> Any:
         if isinstance(obj, str):
             return self.substitute(obj)
         if isinstance(obj, list):
             out = []
             for string in obj:
                 evaluated = self.evaluate(string)
                 if isinstance(evaluated, list):
@@ -209,23 +209,23 @@
 
     def __str__(self) -> str:
         return self.target
 
     def __repr__(self) -> str:
         return f"Node <{self}>"
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
         return self.target == other.target
 
     def __hash__(self) -> int:
         return hash(self.target)
 
-    def add_requirement(self, other):
+    def add_requirement(self, other: Node) -> None:
         if other in self.requires:
             warnings.warn(
                 f"`{other}` is included twice in `{self}` requirements, "
                 "only the first will be considered",
                 RuntimeWarning,
                 stacklevel=3,
             )
@@ -243,30 +243,30 @@
 
     def __getitem__(self, item: str) -> Node:
         return self._mapping[item]
 
     def __contains__(self, item: str) -> bool:
         return item in self._mapping
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Node]:
         if hasattr(self, "ordered"):
             return iter(self.ordered)
         return iter(self._mapping.values())
 
-    def sort(self):
+    def sort(self) -> None:
         try:
             self.c3_sort()
         except ValueError:
             self.topological_sort()
 
-    def c3_sort(self):
+    def c3_sort(self) -> None:
         self.ordered = self._node_s3_sort(self.root)
         self.ordered.reverse()
 
-    def topological_sort(self):
+    def topological_sort(self) -> None:
         self.ordered = []
         unordered_nodes = self._mapping.copy()
         while unordered_nodes:
             for target, node in unordered_nodes.items():
                 if all((parent in self.ordered) for parent in node.requires):
                     del unordered_nodes[target]
                     self.ordered.append(node)
@@ -276,15 +276,15 @@
         warnings.warn(
             "The requirements order didn't allow the deterministic order; "
             "fell back to old-style dependency resolution",
             RuntimeWarning,
             stacklevel=3,
         )
 
-    def add_node(self, node):
+    def add_node(self, node: Node) -> None:
         self._mapping[node.target] = node
 
     def _node_s3_sort(self, node: Node) -> list[Node]:
         out = [node]
         requirements = node.requires
         if requirements:
             try:
@@ -383,15 +383,15 @@
             key, options = extract_options(key)
             if "weak" in options and key in old_keys:
                 continue
             value = parser.evaluate(raw_value)
             variables[key] = value
 
 
-def extract_options(string: str):
+def extract_options(string: str) -> tuple[str, set[str]]:
     match = re.fullmatch(OPTIONS, string)
     if match is None:
         return string.strip(), set()
 
     options = match["options"]
     string = match["string"]
     return string, {s.strip() for s in options.split(",")}
```

### Comparing `yamk-5.0.1/src/yamk/main.py` & `yamk-5.1.0/src/yamk/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from yamk import __version__
 from yamk.lib import SUPPORTED_FILE_EXTENSIONS
 from yamk.make import MakeCommand
 
 sys.tracebacklimit = 0
 
 
-def parse_args():
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="yamk", description="Yet another make command"
     )
 
     # positional arguments
     parser.add_argument("target", help="the target for yamk")
 
@@ -106,10 +106,10 @@
         help="a list of variables to override the ones set in the cookbook, "
         "which should be in the form <variable>=<value>",
     )
 
     return parser.parse_args()
 
 
-def main():
+def main() -> None:
     args = parse_args()
     MakeCommand(args).make()
```

### Comparing `yamk-5.0.1/src/yamk/make.py` & `yamk-5.1.0/src/yamk/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import subprocess
 import sys
 from time import perf_counter_ns, sleep
 from typing import Any, cast
 
 from dj_settings import SettingsParser
+from packaging.version import Version
 
 from yamk import __version__, lib
 
 
 class MakeCommand:
     def __init__(self, args: argparse.Namespace):
         self.verbosity = args.verbose
@@ -31,17 +32,17 @@
         self.dry_run = args.dry_run
         cookbook = self.find_cookbook(args)
         self.base_dir = cookbook.parent
         self.phony_dir = self.base_dir.joinpath(".yamk")
         self.arg_vars = dict(var.split("=", maxsplit=1) for var in args.variables)
         parsed_cookbook = SettingsParser(cookbook, force_type=args.cookbook_type).data
         self.globals = parsed_cookbook.pop("$globals", {})
-        self.version = self.globals.get("version", 4)
-        if self.version > __version__.major:
-            raise RuntimeError(f"This cookbook requires an yamk >= v{self.version}.0.0")
+        self.version = Version(str(self.globals.get("version", "4.0.0")))
+        if self.version > __version__:
+            raise RuntimeError(f"This cookbook requires an yamk >= v{self.version}")
         self.up_to_date = args.assume
         self._parse_recipes(parsed_cookbook)
         self.subprocess_kwargs = {
             "shell": True,
             "cwd": self.base_dir,
             "executable": self.globals.get("shell") or args.shell,
         }
@@ -62,29 +63,29 @@
             if cookbook.exists():
                 return cookbook
         raise FileNotFoundError(f"No candidate cookbook found in {args.directory}")
 
     def make(self) -> None:
         dag = self._preprocess_target()
         for node in filter(lambda x: x.should_build, dag):
-            self._make_target(node.recipe)
+            self._make_target(cast(lib.Recipe, node.recipe))
         if self.print_timing_report:
             lib.print_reports(self.reports)
 
     def _run_command(self, command: str) -> int:
         status = 0
         if self.dry_run:
             print(command)
             return status
 
         a, b = 1, 1
         total = 0
         for i in range(self.retries + 1):
             start = perf_counter_ns()
-            result = subprocess.run(command, **self.subprocess_kwargs)
+            result = subprocess.run(command, **self.subprocess_kwargs)  # noqa: S603
             end = perf_counter_ns()
             total += end - start
             status = result.returncode
             if status == 0:
                 report = lib.CommandReport(
                     command=command, timing_ns=total, retries=i, success=True
                 )
```

### Comparing `yamk-5.0.1/PKG-INFO` & `yamk-5.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamk
-Version: 5.0.1
+Version: 5.1.0
 Summary: Yet another make
 Home-page: https://yamk.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: make,build,cli
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
@@ -56,22 +56,19 @@
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
-The easiest way is to use pip to install ``yam``.
+The easiest way is to use `pipx`_ to install ``yam``.
 
 .. code:: console
 
-   $ pip install --user yamk
-
-Please make sure that the correct directory is added to your path. This
-depends on the OS.
+   $ pipx install yamk
 
 Usage
 ^^^^^
 
 ``yam``'s behaviour is defined in a toml file, called a cookbook. The default name is ``make.toml``,
 but you can specify a different file if you want. Specifying a name ``<name.toml>`` will also parse all the ``.toml``
 files in the directory named ``<name.toml>.d``.
@@ -84,9 +81,10 @@
 -----
 
 - `Documentation`_
 - `Changelog`_
 
 
 .. _Changelog: https://github.com/spapanik/yamk/blob/main/CHANGELOG.rst
-.. _Documentation: https://yamk.readthedocs.io/en/latest/
+.. _Documentation: https://yamk.readthedocs.io/en/stable/
+.. _pipx: https://pypa.github.io/pipx/
```

