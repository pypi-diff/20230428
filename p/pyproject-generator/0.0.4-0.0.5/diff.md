# Comparing `tmp/pyproject-generator-0.0.4.tar.gz` & `tmp/pyproject-generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.4.tar", last modified: Mon Apr 24 15:30:19 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.5.tar", last modified: Fri Apr 28 19:23:36 2023, max compression
```

## Comparing `pyproject-generator-0.0.4.tar` & `pyproject-generator-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.862052 pyproject-generator-0.0.4/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-24 15:30:19.862223 pyproject-generator-0.0.4/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-24 15:30:19.863127 pyproject-generator-0.0.4/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.843238 pyproject-generator-0.0.4/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.848259 pyproject-generator-0.0.4/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.4/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-24 15:30:11.000000 pyproject-generator-0.0.4/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-24 14:59:13.000000 pyproject-generator-0.0.4/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.849579 pyproject-generator-0.0.4/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-19 15:24:27.000000 pyproject-generator-0.0.4/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-24 14:54:50.000000 pyproject-generator-0.0.4/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     7975 2023-04-24 15:28:44.000000 pyproject-generator-0.0.4/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.856940 pyproject-generator-0.0.4/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.4/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.4/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.4/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.4/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.4/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.4/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.860996 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.861671 pyproject-generator-0.0.4/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.015025 pyproject-generator-0.0.5/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:23:36.015286 pyproject-generator-0.0.5/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-28 19:23:36.016563 pyproject-generator-0.0.5/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:35.992215 pyproject-generator-0.0.5/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:35.997430 pyproject-generator-0.0.5/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.5/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-28 19:23:26.000000 pyproject-generator-0.0.5/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-28 19:13:46.000000 pyproject-generator-0.0.5/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.000311 pyproject-generator-0.0.5/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.0.5/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:07.000000 pyproject-generator-0.0.5/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     7486 2023-04-28 19:20:05.000000 pyproject-generator-0.0.5/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.008211 pyproject-generator-0.0.5/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.5/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.5/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.5/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.5/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.5/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.5/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.013286 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-28 19:23:35.000000 pyproject-generator-0.0.5/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-28 19:23:36.014449 pyproject-generator-0.0.5/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.5/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.4/PKG-INFO` & `pyproject-generator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.4/README.md` & `pyproject-generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.4/setup.cfg` & `pyproject-generator-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.4/src/pyproject/cli.py` & `pyproject-generator-0.0.5/src/pyproject/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,13 +73,13 @@
         "email": args.email,
         "set_dependencies": args.set_dependencies,
         "add_dependencies": args.add_dependencies,
         "remove_dependencies": args.remove_dependencies,
         "reset_config": args.reset_config,
     }
 
-    builder = ProjectBuilder(project_name=args.project_name, config=config)
-    builder.dispatch(action=args.action)
+    builder = ProjectBuilder(config=config)
+    builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyproject-generator-0.0.4/src/pyproject/project_builder.py` & `pyproject-generator-0.0.5/src/pyproject/project_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,76 +15,80 @@
 PathLike = Union[Path, str]
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
 CONFIG_PATH = BASE_PATH / "config"
 
 
-class _EnvBuilder(venv.EnvBuilder):
-    def __init__(self, venv_path: PathLike, *args, **kwargs) -> None:
-        self.context: Optional[SimpleNamespace] = None
-        self.venv_path = Path(venv_path)
+class Env(venv.EnvBuilder):
+    def __init__(self, *args, **kwargs) -> None:
+        self.context = self.get_context()
         super().__init__(*args, **kwargs)
 
+    def get_context(self) -> Optional[SimpleNamespace]:
+        if "VIRTUAL_ENV" not in os.environ:
+            self.context = None
+            return None
+
+        env_dir: Path = Path(os.environ["VIRTUAL_ENV"])
+        env_name = env_dir.stem
+
+        namespace = SimpleNamespace(
+            env_dir=env_dir.as_posix(),
+            env_name=env_name,
+            bin_path=env_dir / "bin",
+            env_exe=env_dir / "bin/python",
+        )
+
+        return namespace
+
     def post_setup(self, context: SimpleNamespace):
         self.context = context
 
-    def venv_create(self) -> Optional[SimpleNamespace]:
-        self.create(self.venv_path)
+    def venv_create(self, venv_path: PathLike) -> Optional[SimpleNamespace]:
+        # This sets self.context because `create()` calls `post_setup()`
+        self.create(venv_path)
 
         return self.context
 
-    def run_python_in_venv(
-        self, command: list[str]
-    ) -> subprocess.CompletedProcess[bytes]:
-        assert self.context is not None
-        command = [self.context.env_exe] + command
-
-        return subprocess.run(command, check=True)
-
-    def run_bin_in_venv(
+    def run_bin(
         self, command: list[str], **kwargs
     ) -> subprocess.CompletedProcess[bytes]:
-        assert self.context is not None
-        command[0] = Path(self.context.bin_path).joinpath(command[0]).as_posix()
+        if self.context is not None:
+            command[0] = Path(self.context.bin_path).joinpath(command[0]).as_posix()
 
         return subprocess.run(command, check=True, **kwargs)
 
 
 class ProjectBuilder:
     def __init__(
         self,
-        project_name: Optional[str],
         template_path: PathLike = TEMPLATE_PATH,
         config_path: PathLike = CONFIG_PATH,
         config: Optional[dict[str, str]] = None,
     ) -> None:
-        if project_name is not None:
-            self._validate_project_name(project_name)
-            self._project_name = project_name
-
-        self._project_path = Path().cwd()
+        self.proj_path = Path().cwd()
 
         self._template_path = Path(template_path)
         self._config_path = Path(config_path)
         self._config = self._set_config(config)
 
     @staticmethod
     def _validate_project_name(project_name: str) -> None:
         regex = "^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$"
         if not bool(re.match(regex, project_name, re.IGNORECASE)):
             raise ValueError(
                 "A valid project name may only contain ASCII letters, numbers, ., -,"
                 " and/or _, and they must begin and end with a letter or number."
             )
 
-    def _fill_in_templates(self) -> dict[str, str]:
+    def _fill_in_templates(self, project_name: str) -> dict[str, str]:
         config = self._config
         d = {
-            "PACKAGE": self._project_name,
+            "PACKAGE": project_name,
             "PYPI_USERNAME": config["pypi_username"],
             "PYPI_PASSWORD": config["pypi_password"],
             "GITHUB_URL": config["github_url"],
             "AUTHOR": config["author"],
             "EMAIL": config["email"],
         }
 
@@ -94,65 +98,68 @@
                 src = string.Template(f.read())
                 result = src.substitute(d)
 
                 filled_in_templates[file.stem] = result
 
         return filled_in_templates
 
-    def init_project(self):
+    def init_project(self, project_name: str):
         # Create the project directory
-        self._project_path.mkdir()
+        self._validate_project_name(project_name)
+
+        proj_path = self.proj_path / project_name
+        proj_path.mkdir()
 
         # src
-        src_path = self._project_path / "src"
+        src_path = proj_path / "src"
         src_path.mkdir()
 
-        src_proj_path = src_path / self._project_name
+        src_proj_path = src_path / project_name
         src_proj_path.mkdir()
         (src_proj_path / "__init__.py").touch()
         (src_proj_path / "py.typed").touch()
 
         # Fill in templates
-        templates = self._fill_in_templates()
+        templates = self._fill_in_templates(project_name)
 
         # tests
-        tests_path = self._project_path / "tests"
+        tests_path = proj_path / "tests"
         tests_path.mkdir()
-        (tests_path / f"test_{self._project_name}.py").touch()
+        (tests_path / f"test_{project_name}.py").touch()
 
         # benchmarks
-        benchmarks_path = self._project_path / "benchmarks"
+        benchmarks_path = proj_path / "benchmarks"
         benchmarks_path.mkdir()
         (benchmarks_path / "benchmark.py").touch()
 
         # github actions
-        workflows_path = self._project_path / ".github/workflows"
+        workflows_path = proj_path / ".github/workflows"
         workflows_path.mkdir(parents=True)
         (workflows_path / "tests.yml").write_text(templates["tests"])
 
         # misc setup
-        (self._project_path / "tox.ini").write_text(templates["tox"])
-        (self._project_path / "pyproject.toml").write_text(templates["pyproject"])
-        (self._project_path / "setup.cfg").write_text(templates["setup"])
-        (self._project_path / ".gitignore").write_text(templates["gitignore"])
-        (self._project_path / "README.md").write_text(templates["readme"])
+        (proj_path / "tox.ini").write_text(templates["tox"])
+        (proj_path / "pyproject.toml").write_text(templates["pyproject"])
+        (proj_path / "setup.cfg").write_text(templates["setup"])
+        (proj_path / ".gitignore").write_text(templates["gitignore"])
+        (proj_path / "README.md").write_text(templates["readme"])
 
         # Setup the virtual environment
 
-        venv_builder = _EnvBuilder(self._project_path / "venv", with_pip=True)
-        venv_builder.venv_create()
-        venv_builder.run_python_in_venv(["-m", "pip", "install", "-U", "pip"])
+        venv_builder = Env(with_pip=True)
+        venv_builder.venv_create(proj_path / "venv")
+        venv_builder.run_bin(["python", "-m", "pip", "install", "-U", "pip"])
 
         # Install developer dependencies
         for dep in ("black", "mypy", "build", "tox", "pytest"):
-            venv_builder.run_bin_in_venv(["pip", "install", dep])
+            venv_builder.run_bin(["pip", "install", dep])
 
         # Create requirements_dev file
-        reqs = venv_builder.run_bin_in_venv(["pip", "freeze"], capture_output=True)
-        (self._project_path / "requirements_dev.txt").write_bytes(reqs.stdout)
+        reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
+        (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
     def _parse_config_file(self, filename: PathLike) -> dict:
         with open(self._config_path / filename) as f:
             config: dict = json.load(f)
 
         return config
 
@@ -201,40 +208,26 @@
         with open(self._config_path, "w") as f:
             json.dump(config, f, indent=4)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
 
-        try:
-            venv_path = Path(os.environ["VIRTUAL_ENV"]) / "bin"
-        except KeyError:
-            venv_path = ""
-
-        # TODO: Make EnvBuilder class capable of handling existing venvs, removing
-        # the need for this duplicate function
-        def run_bin_in_venv(
-            command: list[str], **kwargs
-        ) -> subprocess.CompletedProcess[bytes]:
-            command[0] = Path(venv_path).joinpath(command[0]).as_posix()
+        env = Env()
 
-            return subprocess.run(command, check=True, **kwargs)
+        shutil.rmtree(self.proj_path / "dist", ignore_errors=True)
 
-        shutil.rmtree(self._project_path / "dist", ignore_errors=True)
-
-        run_bin_in_venv(["python", "-m", "build"])
-        run_bin_in_venv(["twine", "check", "dist/*"])
+        env.run_bin(["python", "-m", "build"])
+        env.run_bin(["twine", "check", "dist/*"])
 
         if "" in (username, password):
-            run_bin_in_venv(["twine", "upload", "dist/*"])
+            env.run_bin(["twine", "upload", "dist/*"])
         else:
-            run_bin_in_venv(
-                ["twine", "upload", "dist/*", "-u", username, "-p", password]
-            )
+            env.run_bin(["twine", "upload", "dist/*", "-u", username, "-p", password])
 
-    def dispatch(self, action: Action):
+    def dispatch(self, action: Action, **kwargs):
         if action == "init":
-            self.init_project()
+            self.init_project(**kwargs)
         elif action == "upload":
             self.upload()
         elif action == "config":
             self.config()
```

### Comparing `pyproject-generator-0.0.4/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.5/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.4/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.5/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.4/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.5/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.4/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.0.5/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.0.4/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.5/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

