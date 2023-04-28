# Comparing `tmp/utilki-0.1.3.tar.gz` & `tmp/utilki-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.1.3.tar", max compression
+gzip compressed data, was "utilki-0.1.7.tar", max compression
```

## Comparing `utilki-0.1.3.tar` & `utilki-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      921 2023-04-07 09:39:03.009675 utilki-0.1.3/README.md
--rw-r--r--   0        0        0      511 2023-04-07 13:49:12.445773 utilki-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.1.3/utilki/__init__.py
--rw-r--r--   0        0        0     2168 2023-04-07 09:37:49.369962 utilki-0.1.3/utilki/cli.py
--rw-r--r--   0        0        0     2853 2023-04-07 13:46:41.063717 utilki-0.1.3/utilki/task_mixin.py
--rw-r--r--   0        0        0     1676 2023-04-07 13:49:41.962742 utilki-0.1.3/setup.py
--rw-r--r--   0        0        0     1325 2023-04-07 13:49:41.963016 utilki-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.1.7/README.md
+-rw-r--r--   0        0        0      532 2023-04-28 13:26:59.815475 utilki-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.1.7/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.1.7/utilki/cli.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:28:34.414115 utilki-0.1.7/utilki/nomad.py
+-rw-r--r--   0        0        0     3992 2023-04-28 13:26:04.137420 utilki-0.1.7/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1848 2023-04-28 13:27:35.066547 utilki-0.1.7/setup.py
+-rw-r--r--   0        0        0     1510 2023-04-28 13:27:35.066721 utilki-0.1.7/PKG-INFO
```

### Comparing `utilki-0.1.3/README.md` & `utilki-0.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # utilki
 
+[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)
+
 utils that are frequently used by me and might be useful for others
 
 ## installation
 
 ```bash
 pip install utilki
 ```
```

### Comparing `utilki-0.1.3/utilki/cli.py` & `utilki-0.1.7/utilki/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             if response == "y":
                 process = subprocess.Popen(
                     ["pyenv", "install", python_version],
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     text=True,
                 )
-                for line in iter(process.stdout.readline, ""):
+                for line in iter(process.stdout.readline, ""):  # type: ignore
                     click.echo(line.strip())
                 return_code = process.wait()
                 if return_code != 0:
                     click.echo("Installation failed")
                     return
                 click.echo("Installation successful")
```

### Comparing `utilki-0.1.3/setup.py` & `utilki-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['utilki']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.1.3,<9.0.0']
+['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.1.3',
+    'version': '0.1.7',
     'description': 'A collection of useful utilities',
-    'long_description': '# utilki\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
+    'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `utilki-0.1.3/PKG-INFO` & `utilki-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.1.3
+Version: 0.1.7
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
 # utilki
 
+[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)
+
 utils that are frequently used by me and might be useful for others
 
 ## installation
 
 ```bash
 pip install utilki
 ```
```

