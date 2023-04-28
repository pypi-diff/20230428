# Comparing `tmp/python-observer-0.2.0.tar.gz` & `tmp/python-observer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-observer-0.2.0.tar", max compression
+gzip compressed data, was "python-observer-0.3.0.tar", max compression
```

## Comparing `python-observer-0.2.0.tar` & `python-observer-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.2.0/LICENSE
--rw-r--r--   0        0        0      541 2023-04-25 13:32:03.887748 python-observer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.2.0/python_observer/__init__.py
--rw-r--r--   0        0        0     2259 2023-04-25 13:30:23.403543 python-observer-0.2.0/python_observer/cli.py
--rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.2.0/python_observer/constants.py
--rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.2.0/python_observer/date.py
--rw-r--r--   0        0        0      595 2023-04-24 10:43:39.568229 python-observer-0.2.0/python_observer/display.py
--rw-r--r--   0        0        0      437 2023-04-25 13:30:23.404545 python-observer-0.2.0/python_observer/misc.py
--rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.2.0/python_observer/watch.py
--rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.2.0/README.md
--rw-r--r--   0        0        0      923 2023-04-25 13:33:03.025319 python-observer-0.2.0/setup.py
--rw-r--r--   0        0        0      717 2023-04-25 13:33:03.026775 python-observer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-24 10:28:29.010276 python-observer-0.3.0/LICENSE
+-rw-r--r--   0        0        0      580 2023-04-28 10:32:48.923265 python-observer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 09:24:48.929131 python-observer-0.3.0/python_observer/__init__.py
+-rw-r--r--   0        0        0     4446 2023-04-28 10:31:08.927636 python-observer-0.3.0/python_observer/cli.py
+-rw-r--r--   0        0        0       48 2023-04-23 10:25:03.851281 python-observer-0.3.0/python_observer/constants.py
+-rw-r--r--   0        0        0      529 2023-04-24 10:10:37.131958 python-observer-0.3.0/python_observer/date.py
+-rw-r--r--   0        0        0      992 2023-04-28 10:31:06.738394 python-observer-0.3.0/python_observer/display.py
+-rw-r--r--   0        0        0      972 2023-04-28 10:24:47.359182 python-observer-0.3.0/python_observer/misc.py
+-rw-r--r--   0        0        0     2855 2023-04-25 13:30:23.405542 python-observer-0.3.0/python_observer/watch.py
+-rw-r--r--   0        0        0      149 2023-04-24 10:36:02.903294 python-observer-0.3.0/README.md
+-rw-r--r--   0        0        0      966 2023-04-28 10:33:03.968515 python-observer-0.3.0/setup.py
+-rw-r--r--   0        0        0      787 2023-04-28 10:33:03.968515 python-observer-0.3.0/PKG-INFO
```

### Comparing `python-observer-0.2.0/LICENSE` & `python-observer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-observer-0.2.0/pyproject.toml` & `python-observer-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "python-observer"
-version = "0.2.0"
+version = "0.3.0"
 description = "Live reload for Python apps"
 authors = ["Skyascii <savioxavier112@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "python_observer/**/*.py" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rich = "^13.3.4"
+rich = ">=12.5.1"
 humanfriendly = "^10.0"
+pyboxen = "^1.2.0"
+tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python-observer-0.2.0/python_observer/date.py` & `python-observer-0.3.0/python_observer/date.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.2.0/python_observer/display.py` & `python-observer-0.3.0/python_observer/display.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import sys
+
 from rich.console import Console
 from rich.table import Table
+
 from .constants import DOT_CHAR
 
 console = Console()
-rich_print = console.print
+rich_print = console.print  # Rich variant
+pyprint = print  # Python variant
 
 
 def newline():
     print("\n", end="")
 
 
 def print_both_sides(left, right):
@@ -15,13 +19,27 @@
     grid.add_column()
     grid.add_column(justify="right")
     grid.add_row(left, right)
 
     rich_print(grid)
 
 
+def render_rich_text(text, highlight=False):
+    with console.capture() as capture:
+        rich_print(text, highlight=highlight)
+
+    return capture.get()
+
+
 def print_line(rule_style="dim green", char="─"):
     console.rule(style=rule_style, characters=char)
 
 
 def observer_message(message, style="yellow"):
     return f"[{style}]observer[/{style}] [dim]{DOT_CHAR}[/dim] {message}"
+
+
+def print_observer_error(message, style="red"):
+    rich_print(
+        f"[{style}]observer error[/{style}] [dim]{DOT_CHAR}[/dim] [red]{message}[/red]"
+    )
+    sys.exit(1)
```

### Comparing `python-observer-0.2.0/python_observer/watch.py` & `python-observer-0.3.0/python_observer/watch.py`

 * *Files identical despite different names*

### Comparing `python-observer-0.2.0/setup.py` & `python-observer-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 packages = \
 ['python_observer']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['humanfriendly>=10.0,<11.0', 'rich>=13.3.4,<14.0.0']
+['humanfriendly>=10.0,<11.0',
+ 'pyboxen>=1.2.0,<2.0.0',
+ 'rich>=12.5.1',
+ 'tomli>=2.0.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['observer = python_observer.cli:main']}
 
 setup_kwargs = {
     'name': 'python-observer',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Live reload for Python apps',
     'long_description': "# observer\n\n![observer image](https://i.imgur.com/ZoafdEY.png)\n\n> Live reload for Python apps\n\nDocs coming soon - I've ordered them via Amazon Prime\n",
     'author': 'Skyascii',
     'author_email': 'savioxavier112@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `python-observer-0.2.0/PKG-INFO` & `python-observer-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: python-observer
-Version: 0.2.0
+Version: 0.3.0
 Summary: Live reload for Python apps
 License: MIT
 Author: Skyascii
 Author-email: savioxavier112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: humanfriendly (>=10.0,<11.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: pyboxen (>=1.2.0,<2.0.0)
+Requires-Dist: rich (>=12.5.1)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # observer
 
 ![observer image](https://i.imgur.com/ZoafdEY.png)
 
 > Live reload for Python apps
```

