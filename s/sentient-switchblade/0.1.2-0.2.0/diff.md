# Comparing `tmp/sentient_switchblade-0.1.2.tar.gz` & `tmp/sentient_switchblade-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.1.2.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.2.0.tar", max compression
```

## Comparing `sentient_switchblade-0.1.2.tar` & `sentient_switchblade-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.1.2/LICENSE
--rw-r--r--   0        0        0     6679 2023-04-27 22:35:37.645490 sentient_switchblade-0.1.2/README.md
--rw-r--r--   0        0        0     1383 2023-04-27 23:18:39.260211 sentient_switchblade-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.1.2/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.1.2/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1656 2023-04-27 22:56:23.444492 sentient_switchblade-0.1.2/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    10301 2023-04-27 23:17:58.142250 sentient_switchblade-0.1.2/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.1.2/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:46.529573 sentient_switchblade-0.1.2/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:50.583261 sentient_switchblade-0.1.2/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.1.2/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.1.2/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0     9535 2023-04-26 17:36:59.378665 sentient_switchblade-0.1.2/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.1.2/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.2/setup.py
--rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8177 2023-04-28 18:18:01.183570 sentient_switchblade-0.2.0/README.md
+-rw-r--r--   0        0        0     1405 2023-04-28 18:11:29.738779 sentient_switchblade-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.2.0/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.2.0/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1656 2023-04-28 12:34:10.275655 sentient_switchblade-0.2.0/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    10660 2023-04-28 17:55:19.000402 sentient_switchblade-0.2.0/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.2.0/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0     1087 2023-04-28 18:13:37.061787 sentient_switchblade-0.2.0/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0     1089 2023-04-28 12:31:21.153690 sentient_switchblade-0.2.0/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.2.0/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.2.0/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0    10948 2023-04-28 18:13:26.743690 sentient_switchblade-0.2.0/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.2.0/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.0/setup.py
+-rw-r--r--   0        0        0     9584 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.0/PKG-INFO
```

### Comparing `sentient_switchblade-0.1.2/LICENSE` & `sentient_switchblade-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.2/README.md` & `sentient_switchblade-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!-- markdownlint-disable first-line-h1 line-length no-inline-html -->
 <p align="center">
-  <a href="https://jensroland.com/switchblade">
+  <a href="https://github.com/JensRoland/sentient-switchblade">
     <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />
   </a>
 </p>
 
 <h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>
-<p align="center">created by <a href="https://jensroland.com/">Jens Roland</a></p>
+<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>
 
 <br />
 
 ## ⚔️ What is Switchblade?
 
 Switchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.
 
@@ -54,17 +54,14 @@
 
 In an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.
 
 To achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated 'bundles' of dev tools.
 
 Switchblade is that tool.
 
-Learn more on the [Switchblade project website](https://jensroland.com/switchblade/).
-
-
 ## Custom bundles
 
 To create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:
 
 ```toml
 [bundle]
 name = "my-dev-tool-bundle"
@@ -93,30 +90,44 @@
 pylint = "^2.17.2"
 pytest = "^7.3.1"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 ```
 
-And in the same repo folder, add any config files you need, e.g. `.pylintrc`:
+For each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.
+
+The `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.
+
+The same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.
+
+### Tool configuration
+
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project's `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.
+
+If you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:
 
 ```ini
 [MAIN]
 [MESSAGES CONTROL]
 disable=
     C0111,  # missing-docstring
     C0114,  # missing-module-docstring
     C0115,  # missing-class-docstring
     C0116,  # missing-function-docstring
     W0613,  # unused-argument
 ```
 
-Now when you want to use your custom bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swtichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.
+Now, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.
+
+### Per-project overrides
+
+To override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not 'extend' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.
 
-Anything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project's `pyproject.toml` file under the same section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.
+To override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.
 
 ## Prerequisites
 
 - [Python 3.7+](https://www.python.org/downloads/)
 
 Currently, you need Python since you install Switchblade with pip. This may change in the future.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                               [Switchblade_logo]
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
-                            created by Jens_Roland
+                            Created by Jens_Roland
 
 ## âï¸ What is Switchblade? Switchblade is a command line tool that lets you
 install and run dev tools from a central repository, and configure them in a
 standardised way across all your projects. ## Try it To use the included
 `python-poetry-base` bundle for Python, create a `.switchblade` file in your
 project root: ```toml [switchblade] bundle = "gh:jensroland/sentient-
 switchblade/bundles/python-poetry-base" mode = "python-poetry" ``` Then,
@@ -34,33 +34,52 @@
 be checked into version control (*seriously*) but rather **fetched on demand
 from a centrally managed dev tooling repository, and configured and invoked in
 exactly the same way in every repo, every time**. This would allow for a single
 source of truth for all dev tooling, and would make it easy to update
 configurations across all projects. To achieve this however, you would need
 some kind of small helper tool to abstract away the fetching, configuring and
 invoking of your centrally curated 'bundles' of dev tools. Switchblade is that
-tool. Learn more on the [Switchblade project website](https://jensroland.com/
-switchblade/). ## Custom bundles To create your own custom bundle with the dev
-tools and configurations you need, simply create a new Github repo and add a
+tool. ## Custom bundles To create your own custom bundle with the dev tools and
+configurations you need, simply create a new Github repo and add a
 `bundle.toml` file to it: ```toml [bundle] name = "my-dev-tool-bundle" mode =
 "python-poetry" schema_version = "1.0.0" # Linters [linters] all = ["pylint"]
 [linters.pylint] command = "pylint src" # Tests [tests] all = ["pytest"]
 [tests.pytest] command = "pytest -c pyproject.toml tests" # Extensions to
 pyproject.toml [tool.poetry.group.switchblade] optional = true
 [tool.poetry.group.switchblade.dependencies] pylint = "^2.17.2" pytest =
-"^7.3.1" [tool.pytest.ini_options] pythonpath = "src" ``` And in the same repo
-folder, add any config files you need, e.g. `.pylintrc`: ```ini [MAIN]
-[MESSAGES CONTROL] disable= C0111, # missing-docstring C0114, # missing-module-
-docstring C0115, # missing-class-docstring C0116, # missing-function-docstring
-W0613, # unused-argument ``` Now when you want to use your custom bundle in a
-project, simply point to the repo in the project `.switchblade` file as in the
-example above. Swtichblade will then fetch and install the tools you specified
-in the bundle and run them with the configurations you specified. Anything in
-the `bundle.toml` file under a `tool.*` section will be temporarily added to
-the project's `pyproject.toml` file under the same section. This allows you to
-add dependencies and configuration options to all your projects without having
-to manually edit all the individual `pyproject.toml` files. ## Prerequisites -
-[Python 3.7+](https://www.python.org/downloads/) Currently, you need Python
-since you install Switchblade with pip. This may change in the future. ##
-Features - CLI command `swb lint` to run linters - CLI command `swb test` to
-run tests - Project 'modes' supported: Currently only `python-poetry` is
-supported, but more will be added soon.
+"^7.3.1" [tool.pytest.ini_options] pythonpath = "src" ``` For each linter you
+want to add, specify a `[linters.]` section with a `command` key. The `command`
+value will be invoked by Switchblade when you run `swb lint `. The `[linters]`
+section specifies which linters should be invoked (and in which order) when you
+run `swb lint` or `swb lint all`. The same goes for tests: specify a `[tests.]`
+section with a `command` key, and add the tool to the `[tests]` section to have
+it invoked when you run `swb test` or `swb test all`. ### Tool configuration
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily
+added to the project's `pyproject.toml` file under that section. This allows
+you to add dependencies and configuration options to all your projects without
+having to manually edit all the individual `pyproject.toml` files. If you
+prefer having separate config files, or for tools which do not support
+`pyproject.toml` configuration, simply add any config files you need in the
+same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in
+the bundle repo: ```ini [MAIN] [MESSAGES CONTROL] disable= C0111, # missing-
+docstring C0114, # missing-module-docstring C0115, # missing-class-docstring
+C0116, # missing-function-docstring W0613, # unused-argument ``` Now, when you
+want to use your custom dev tool bundle in a project, simply point to the repo
+in the project `.switchblade` file as in the example above. Swichblade will
+then fetch and install the tools you specified in the bundle and run them with
+the configurations you specified. ### Per-project overrides To override the
+bundle configuration for a specific dev tool in one of your project repos,
+simply check in the tool dependencies and configuration files in the project
+repo as you normally would - Switchblade will still invoke the dev tool, but it
+will not overwrite any existing config files or `[tool.*]` sections in your
+`pyproject.toml` file. Be aware that this does not 'extend' the configuration
+from the bundle, but replaces that tool configuration entirely, so this feature
+should be used with caution. To override the command or the list of linters to
+run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in
+the project `.switchblade` file. Switchblade will automatically merge (in this
+case it does extend rather than replace) the bundle config and Switchblade
+config before invoking any of the tools. ## Prerequisites - [Python 3.7+]
+(https://www.python.org/downloads/) Currently, you need Python since you
+install Switchblade with pip. This may change in the future. ## Features - CLI
+command `swb lint` to run linters - CLI command `swb test` to run tests -
+Project 'modes' supported: Currently only `python-poetry` is supported, but
+more will be added soon.
```

### Comparing `sentient_switchblade-0.1.2/pyproject.toml` & `sentient_switchblade-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.1.2"
+version = "0.2.0"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
@@ -29,14 +29,15 @@
 
 [tool.poetry.scripts]
 swb = "switchbladecli.cli.__main__:switchbladecli"
 
 [tool.poetry.dependencies]
 checksumdir = "^1.2.0"
 click = "^8.0.3"
+mergedeep = "^1.3.4"
 PyGithub = "^1.58.1"
 python = "^3.7"
 tomlkit = "^0.11.7"
 
 [tool.poetry.group.dev.dependencies]
 
 [build-system]
```

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.2.0/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.2.0/src/switchbladecli/cli/bundle_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,43 +77,48 @@
         bundle_source_uri = self._switchblade_config["switchblade"]["bundle"]
         click.echo("⚔️ Switchblade checking for updates...")
 
         # Check the remote version to see if we need to update
         remote_version = None
         pygithub = None
         if bundle_source_uri.startswith("gh:"):
-            # Init the Github API
-            pygithub = Github(os.environ.get("GITHUB_TOKEN"))
-            # Get the org name, repo name and folder(s)
-            org_name, repo_name, *folder = bundle_source_uri[3:].split("/")
-            # Get the commit SHA from the repo (default branch)
-            repo = pygithub.get_repo(f"{org_name}/{repo_name}")
-            remote_version = repo.get_branch(repo.default_branch).commit.sha
+            try:
+                # Init the Github API
+                pygithub = Github(os.environ.get("GITHUB_TOKEN"))
+                # Get the org name, repo name and folder(s)
+                org_name, repo_name, *folder = bundle_source_uri[3:].split("/")
+                # Get the commit SHA from the repo (default branch)
+                repo = pygithub.get_repo(f"{org_name}/{repo_name}")
+                remote_version = repo.get_branch(repo.default_branch).commit.sha
+            except Exception as exc:
+                # If something went wrong fetching from Github,
+                # we use the latest cached bundle if it exists
+                latest_cached_version = cache.get_latest_version()
+                if latest_cached_version is not None:
+                    click.echo(f"⚔️ Switchblade failed to fetch remote bundle, using cached version {latest_cached_version} instead.")
+                    cache.log(f"FETCH FAILED_WITH_FALLBACK")
+                    return Bundle(self._switchblade_config, latest_cached_version)
+                else:
+                    # If there is no cached bundle, raise the exception
+                    cache.log(f"FETCH FAILED")
+                    raise click.ClickException(f"Remote bundle repo '{bundle_source_uri}' could not be fetched: {exc}")
         else:
-            # TODO: Hash/Checksum the local folder
             # If the folder doesn't exist, raise an exception
             bundle_source_folder = Path(bundle_source_uri)
             if not bundle_source_folder.exists():
                 raise FileNotFoundError(f"Bundle folder {bundle_source_uri} does not exist.")
             remote_version = hash_dir(bundle_source_uri)
 
         cache.log(f"UPDATING {remote_version}")
-
-        # Check if the latest version from the remote is already in the local cache
-        latest_config = cache.get_latest_config()
-        if latest_config is not None and latest_config["commit_sha"] == remote_version:
-            # If the latest cached bundle is up to date, just return it
-            click.echo(f"⚔️ Switchblade cache already up to date at version {remote_version}")
-            cache.log(f"UPDATING {remote_version} NO_CHANGE")
-            return Bundle(self._switchblade_config, latest_config["commit_sha"])
         
-        # Check if the latest version from the remote is already sitting in an old folder
+        # Check if the latest version from the remote is already cached
+        # (does not necessarily have to be the most recently fetched bundle from 'latest.toml')
         if cache.has_bundle(remote_version):
             # If the latest cached bundle is up to date, just return it
-            click.echo(f"⚔️ Switchblade cache already up to date at version {remote_version}")
+            click.echo(f"⚔️ Switchblade cache already contains version {remote_version}")
             cache.log(f"UPDATING {remote_version} USING_CACHED")
             return Bundle(self._switchblade_config, remote_version)
 
         # If the cache is stale, update it
         click.echo(f"⚔️ Switchblade updating tool bundle to version {remote_version}...")
         bundle_folder = self._bundle_folder_from_version(remote_version)
         if bundle_source_uri.startswith("gh:"):
```

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.2.0/src/switchbladecli/cli/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import click
 
 from switchbladecli.modes.python_poetry import PythonPoetry
 from switchbladecli.cli.config import get_switchblade_config
 
 
 @click.command()
+@click.argument("test", required=False)
 @click.pass_context
-def lint(ctx):
+def test(ctx, test: str):
+    """Run testing tool(s) on project.
+    
+    TEST: Testing tool to run. If not specified, all testing tools will be run.
+    """
     project_dir = ctx.obj["project_dir"]
     config_file = ctx.obj["config"]
     verbose = ctx.obj["verbose"]
-    lint_command(verbose, project_dir, config_file)
+    test_command(verbose, project_dir, config_file, test)
 
 
-def lint_command(verbose: bool, project_dir: str, config_file: str):
+def test_command(verbose: bool, project_dir: str, config_file: str, test_tool: str = "all"):
     config = get_switchblade_config(verbose, project_dir, config_file)
 
+    if test_tool is None:
+        test_tool = "all"
+
     mode = config["switchblade"]["mode"]
 
     tool_runner = None
     if mode == "python-poetry":
         tool_runner = PythonPoetry(config, verbose)
     else:
         raise click.ClickException(
-            f"Project mode {mode} is not supported by Switchblade."
+            f"Invalid project mode {mode} specified."
         )
 
-    tool_runner.lint()
+    tool_runner.test(test_tool)
```

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.2.0/src/switchbladecli/cli/update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 import click
 
-from switchbladecli.modes.python_poetry import PythonPoetry
+from switchbladecli.cli.bundle_cache import Bundle
 from switchbladecli.cli.config import get_switchblade_config
 
 
 @click.command()
 @click.pass_context
-def test(ctx):
+def update(ctx):
     project_dir = ctx.obj["project_dir"]
     config_file = ctx.obj["config"]
     verbose = ctx.obj["verbose"]
-    test_command(verbose, project_dir, config_file)
+    update_command(verbose, project_dir, config_file)
 
 
-def test_command(verbose: bool, project_dir: str, config_file: str):
+def update_command(verbose: bool, project_dir: str, config_file: str):
     config = get_switchblade_config(verbose, project_dir, config_file)
-
-    mode = config["switchblade"]["mode"]
-
-    tool_runner = None
-    if mode == "python-poetry":
-        tool_runner = PythonPoetry(config, verbose)
-    else:
-        raise click.ClickException(
-            f"Project mode {mode} is not supported by Switchblade."
-        )
-
-    tool_runner.test()
+    # Instantiating a Bundle object will fetch the latest bundle from the source or cache
+    latest_bundle = Bundle(config)
```

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.2.0/src/switchbladecli/modes/python_poetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 import click
 import shutil
 import subprocess  # nosec
 
+from mergedeep import merge
 from tomlkit import dumps, loads
 
 from switchbladecli.cli.bundle_cache import Bundle, BundleCache
 
 
 class PythonPoetry:
 
@@ -85,34 +86,14 @@
                     self._project_folder / file
                 )
                 pushed_files.append(file)
                 self._cache.log(f"PUSHED {file}")
         return pushed_files
 
 
-    # TODO: Place this in a superclass
-    def run_linters(self, bundle: Bundle):
-        succeeded = True
-        for linter in bundle.bundle_config["linters"]["all"]:
-            print(f"⚔️ Switchblade running {linter}...")
-            succeeded = succeeded and self.run_linter(bundle, bundle.bundle_config["linters"][linter])
-            self._cache.log(f"RAN {linter}")
-        return succeeded
-
-
-    # TODO: Place this in a superclass
-    def run_tests(self, bundle: Bundle):
-        succeeded = True
-        for test in bundle.bundle_config["tests"]["all"]:
-            print(f"⚔️ Switchblade running {test}...")
-            succeeded = succeeded and self.run_test(bundle, bundle.bundle_config["tests"][test])
-            self._cache.log(f"RAN {test}")
-        return succeeded
-
-
     # TODO: Make this an override (must return False if the linter fails)
     def run_linter(self, bundle: Bundle, linter: dict):
         linter_command_list = linter["command"].split(" ")
         cmd_result = subprocess.run(
             ["poetry", "run", *linter_command_list], cwd=self._project_folder, check=False
         )
         return cmd_result.returncode == 0
@@ -136,15 +117,15 @@
         # Restore the original poetry.lock
         if self.RESET_LOCKFILE_ON_CLEANUP and self._poetry_lockfile_raw_before:
             with open(self._poetry_lockfile, "w") as poetry_lock:
                 poetry_lock.write(self._poetry_lockfile_raw_before)
 
 
     # TODO: Place this in a superclass
-    def lint(self):
+    def lint(self, linter_tool: str):
         # Instantiating a Bundle object will fetch the latest bundle from the source or cache
         latest_bundle = Bundle(self._config)
 
         bundle_config = latest_bundle.bundle_config
         bundle_mode = bundle_config["bundle"]["mode"]
 
         if bundle_mode != self.mode:
@@ -152,28 +133,46 @@
                 f"⚔️ The Switchblade bundle is for a project of mode {bundle_mode}, but this project is of mode {self.mode}.",
                 err=True
             )
             raise click.Abort()
 
         self._cache.log(f"LINTING {latest_bundle.version}")
 
+        # Show error message if the bundle does not contain any linters
+        if "linters" not in bundle_config:
+            self._cache.log(f"LINTING {latest_bundle.version} ABORTED_NO_LINTERS_IN_BUNDLE")
+            click.secho(
+                "⚔️ The Switchblade bundle does not contain any linters.",
+                err=True, fg="red"
+            )
+            raise click.Abort()
+
         pushed_files = []
         success = False
         try:
             print("⚔️ Switchblade installing dev tools...")
             self.install_dev_tools(latest_bundle)
 
             print("⚔️ Switchblade copying configuration...")
             pushed_files = self.copy_config_files(latest_bundle)
 
-            success = self.run_linters(latest_bundle)
+            # Apply local overrides from .switchblade (merging the linter dicts) if any
+            switchblade_linters_config = self._config["linters"] if "linters" in self._config else {}
+            merged_linters_config = merge({}, bundle_config["linters"], switchblade_linters_config)
+
+            success = True
+            linter_names = merged_linters_config[linter_tool] if linter_tool == "all" else [linter_tool]
+            for linter_name in linter_names:
+                print(f"⚔️ Switchblade running {linter_name}...")
+                success = success and self.run_linter(latest_bundle, merged_linters_config[linter_name])
+                self._cache.log(f"RAN {linter_name}")
 
-        except Exception:
+        except Exception as exc:
             self._cache.log(f"LINTING {latest_bundle.version} FAILED_WITH_EXCEPTION")
-            raise click.ClickException("Exception detected while running linters, aborting...")
+            raise click.ClickException(f"Exception detected while running linters, aborting... {exc}")
 
         finally:
             print("⚔️ Switchblade cleaning up...")
             # Remove the files from the project folder that were added in Step 3
             for file in pushed_files:
                 (self._project_folder / file).unlink()
                 self._cache.log(f"POPPED {file}")
@@ -185,15 +184,15 @@
             click.echo("⚔️ Linting finished successfully. 😎")
         else:
             self._cache.log(f"LINTING {latest_bundle.version} FINISHED_WITH_ERRORS")
             click.secho("⚔️ Linting finished with errors. 😭", err=True, fg="red", bold=True)
 
 
     # TODO: Place this in a superclass
-    def test(self):
+    def test(self, test_tool: str):
         # Instantiating a Bundle object will fetch the latest bundle from the source or cache
         latest_bundle = Bundle(self._config)
 
         bundle_config = latest_bundle.bundle_config
         bundle_mode = bundle_config["bundle"]["mode"]
 
         if bundle_mode != self.mode:
@@ -201,28 +200,47 @@
                 f"⚔️ The Switchblade bundle is for a project of mode {bundle_mode}, but this project is of mode {self.mode}.",
                 err=True
             )
             raise click.Abort()
 
         self._cache.log(f"TESTING {latest_bundle.version}")
 
+        # Show error message if the bundle does not contain any linters
+        if "tests" not in bundle_config:
+            self._cache.log(f"TESTING {latest_bundle.version} ABORTED_NO_TESTS_IN_BUNDLE")
+            click.secho(
+                "⚔️ The Switchblade bundle does not contain any tests.",
+                err=True, fg="red"
+            )
+            raise click.Abort()
+
         pushed_files = []
         success = False
         try:
             print("⚔️ Switchblade installing dev tools...")
             self.install_dev_tools(latest_bundle)
 
             print("⚔️ Switchblade copying configuration...")
             pushed_files = self.copy_config_files(latest_bundle)
 
-            success = self.run_tests(latest_bundle)
+            # Apply local overrides from .switchblade (merging the tests dicts) if any
+            bundle_tests_config = bundle_config["tests"]
+            switchblade_tests_config = self._config["tests"] if "tests" in self._config else {}
+            merged_tests_config = merge({}, bundle_tests_config, switchblade_tests_config)
+
+            success = True
+            test_tool_names = merged_tests_config[test_tool] if test_tool == "all" else [test_tool]
+            for test_tool_name in test_tool_names:
+                print(f"⚔️ Switchblade running {test_tool_name}...")
+                success = success and self.run_test(latest_bundle, merged_tests_config[test_tool_name])
+                self._cache.log(f"RAN {test_tool_name}")
 
-        except Exception:
+        except Exception as exc:
             self._cache.log(f"TESTING {latest_bundle.version} FAILED_WITH_EXCEPTION")
-            raise click.ClickException("Exception detected while running tests, aborting...")
+            raise click.ClickException(f"Exception detected while running tests, aborting... {exc}")
 
         finally:
             print("⚔️ Switchblade cleaning up...")
             # Remove the files from the project folder that were added in Step 3
             for file in pushed_files:
                 (self._project_folder / file).unlink()
                 self._cache.log(f"POPPED {file}")
```

### Comparing `sentient_switchblade-0.1.2/src/switchbladecli/utils.py` & `sentient_switchblade-0.2.0/src/switchbladecli/utils.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.2/setup.py` & `sentient_switchblade-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyGithub>=1.58.1,<2.0.0',
  'checksumdir>=1.2.0,<2.0.0',
  'click>=8.0.3,<9.0.0',
+ 'mergedeep>=1.3.4,<2.0.0',
  'tomlkit>=0.11.7,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
 
 setup_kwargs = {
     'name': 'sentient-switchblade',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://jensroland.com/switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\nLearn more on the [Switchblade project website](https://jensroland.com/switchblade/).\n\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nAnd in the same repo folder, add any config files you need, e.g. `.pylintrc`:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow when you want to use your custom bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swtichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under the same section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jensroland.com/sentient-switchblade',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['switchbladecli', 'switchbladecli.cli',
 'switchbladecli.modes'] package_data = \ {'': ['*']} install_requires = \
 ['PyGithub>=1.58.1,<2.0.0', 'checksumdir>=1.2.0,<2.0.0', 'click>=8.0.3,<9.0.0',
-'tomlkit>=0.11.7,<0.12.0'] entry_points = \ {'console_scripts': ['swb =
-switchbladecli.cli.__main__:switchbladecli']} setup_kwargs = { 'name':
-'sentient-switchblade', 'version': '0.1.2', 'description': 'Unleash Dev Tool
-Mastery with a Flick of Your Wrist', 'long_description': '\n
+'mergedeep>=1.3.4,<2.0.0', 'tomlkit>=0.11.7,<0.12.0'] entry_points = \
+{'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
+setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.2.0',
+'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
+'long_description': '\n
                          \n \n_[Switchblade_logo]\n\n
 \n\n
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
 \n
-                            created by Jens_Roland
+                            Created by Jens_Roland
 \n\n
 \n\n## âï¸ What is Switchblade?\n\nSwitchblade is a command line tool that
 lets you install and run dev tools from a central repository, and configure
 them in a standardised way across all your projects.\n\n## Try it\n\nTo use the
 included `python-poetry-base` bundle for Python, create a `.switchblade` file
 in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/
 sentient-switchblade/bundles/python-poetry-base"\nmode = "python-
@@ -45,40 +46,59 @@
 would not be checked into version control (*seriously*) but rather **fetched on
 demand from a centrally managed dev tooling repository, and configured and
 invoked in exactly the same way in every repo, every time**. This would allow
 for a single source of truth for all dev tooling, and would make it easy to
 update configurations across all projects.\n\nTo achieve this however, you
 would need some kind of small helper tool to abstract away the fetching,
 configuring and invoking of your centrally curated \'bundles\' of dev
-tools.\n\nSwitchblade is that tool.\n\nLearn more on the [Switchblade project
-website](https://jensroland.com/switchblade/).\n\n\n## Custom bundles\n\nTo
-create your own custom bundle with the dev tools and configurations you need,
-simply create a new Github repo and add a `bundle.toml` file to it:
-\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-
-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n
-[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall =
-["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n#
-Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional =
-true\n\n[tool.poetry.group.switchblade.dependencies]\npylint =
-"^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath =
-"src"\n```\n\nAnd in the same repo folder, add any config files you need, e.g.
-`.pylintrc`:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n C0111, #
-missing-docstring\n C0114, # missing-module-docstring\n C0115, # missing-class-
-docstring\n C0116, # missing-function-docstring\n W0613, # unused-
-argument\n```\n\nNow when you want to use your custom bundle in a project,
-simply point to the repo in the project `.switchblade` file as in the example
-above. Swtichblade will then fetch and install the tools you specified in the
-bundle and run them with the configurations you specified.\n\nAnything in the
-`bundle.toml` file under a `tool.*` section will be temporarily added to the
-project\'s `pyproject.toml` file under the same section. This allows you to add
-dependencies and configuration options to all your projects without having to
-manually edit all the individual `pyproject.toml` files.\n\n##
-Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/
-)\n\nCurrently, you need Python since you install Switchblade with pip. This
-may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run
-linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported:
-Currently only `python-poetry` is supported, but more will be added soon.\n',
-'author': 'JensRoland', 'author_email': 'mail@jensroland.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://jensroland.com/sentient-
+tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own
+custom bundle with the dev tools and configurations you need, simply create a
+new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname
+= "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n#
+Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint
+src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest
+-c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n
+[tool.poetry.group.switchblade]\noptional = true\n\n
+[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest =
+"^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each
+linter you want to add, specify a `[linters.]` section with a `command` key.
+The `command` value will be invoked by Switchblade when you run `swb lint
+`.\n\nThe `[linters]` section specifies which linters should be invoked (and in
+which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for
+tests: specify a `[tests.]` section with a `command` key, and add the tool to
+the `[tests]` section to have it invoked when you run `swb test` or `swb test
+all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a
+`tool.*` section will be temporarily added to the project\'s `pyproject.toml`
+file under that section. This allows you to add dependencies and configuration
+options to all your projects without having to manually edit all the individual
+`pyproject.toml` files.\n\nIf you prefer having separate config files, or for
+tools which do not support `pyproject.toml` configuration, simply add any
+config files you need in the same folder as the `bundle.toml` file. E.g. you
+might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES
+CONTROL]\ndisable=\n C0111, # missing-docstring\n C0114, # missing-module-
+docstring\n C0115, # missing-class-docstring\n C0116, # missing-function-
+docstring\n W0613, # unused-argument\n```\n\nNow, when you want to use your
+custom dev tool bundle in a project, simply point to the repo in the project
+`.switchblade` file as in the example above. Swichblade will then fetch and
+install the tools you specified in the bundle and run them with the
+configurations you specified.\n\n### Per-project overrides\n\nTo override the
+bundle configuration for a specific dev tool in one of your project repos,
+simply check in the tool dependencies and configuration files in the project
+repo as you normally would - Switchblade will still invoke the dev tool, but it
+will not overwrite any existing config files or `[tool.*]` sections in your
+`pyproject.toml` file. Be aware that this does not \'extend\' the configuration
+from the bundle, but replaces that tool configuration entirely, so this feature
+should be used with caution.\n\nTo override the command or the list of linters
+to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]`
+in the project `.switchblade` file. Switchblade will automatically merge (in
+this case it does extend rather than replace) the bundle config and Switchblade
+config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+]
+(https://www.python.org/downloads/)\n\nCurrently, you need Python since you
+install Switchblade with pip. This may change in the future.\n\n##
+Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test`
+to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is
+supported, but more will be added soon.\n', 'author': 'JensRoland',
+'author_email': 'mail@jensroland.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://jensroland.com/sentient-
 switchblade', 'package_dir': package_dir, 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
 entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `sentient_switchblade-0.1.2/PKG-INFO` & `sentient_switchblade-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentient-switchblade
-Version: 0.1.2
+Version: 0.2.0
 Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
 Home-page: https://jensroland.com/sentient-switchblade
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,27 +22,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyGithub (>=1.58.1,<2.0.0)
 Requires-Dist: checksumdir (>=1.2.0,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
 Project-URL: Repository, https://github.com/jensroland/sentient-switchblade
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable first-line-h1 line-length no-inline-html -->
 <p align="center">
-  <a href="https://jensroland.com/switchblade">
+  <a href="https://github.com/JensRoland/sentient-switchblade">
     <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />
   </a>
 </p>
 
 <h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>
-<p align="center">created by <a href="https://jensroland.com/">Jens Roland</a></p>
+<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>
 
 <br />
 
 ## ⚔️ What is Switchblade?
 
 Switchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.
 
@@ -86,17 +87,14 @@
 
 In an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.
 
 To achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated 'bundles' of dev tools.
 
 Switchblade is that tool.
 
-Learn more on the [Switchblade project website](https://jensroland.com/switchblade/).
-
-
 ## Custom bundles
 
 To create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:
 
 ```toml
 [bundle]
 name = "my-dev-tool-bundle"
@@ -125,30 +123,44 @@
 pylint = "^2.17.2"
 pytest = "^7.3.1"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 ```
 
-And in the same repo folder, add any config files you need, e.g. `.pylintrc`:
+For each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.
+
+The `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.
+
+The same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.
+
+### Tool configuration
+
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project's `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.
+
+If you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:
 
 ```ini
 [MAIN]
 [MESSAGES CONTROL]
 disable=
     C0111,  # missing-docstring
     C0114,  # missing-module-docstring
     C0115,  # missing-class-docstring
     C0116,  # missing-function-docstring
     W0613,  # unused-argument
 ```
 
-Now when you want to use your custom bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swtichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.
+Now, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.
+
+### Per-project overrides
+
+To override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not 'extend' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.
 
-Anything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project's `pyproject.toml` file under the same section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.
+To override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.
 
 ## Prerequisites
 
 - [Python 3.7+](https://www.python.org/downloads/)
 
 Currently, you need Python since you install Switchblade with pip. This may change in the future.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.2.0 Summary:
 Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
 jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
 email: mail@jensroland.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -10,20 +10,20 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Requires-Dist: PyGithub (>=1.58.1,<2.0.0)
 Requires-Dist: checksumdir (>=1.2.0,<2.0.0) Requires-Dist: click
-(>=8.0.3,<9.0.0) Requires-Dist: tomlkit (>=0.11.7,<0.12.0) Project-URL:
-Repository, https://github.com/jensroland/sentient-switchblade Description-
-Content-Type: text/markdown
+(>=8.0.3,<9.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
+tomlkit (>=0.11.7,<0.12.0) Project-URL: Repository, https://github.com/
+jensroland/sentient-switchblade Description-Content-Type: text/markdown
                               [Switchblade_logo]
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
-                            created by Jens_Roland
+                            Created by Jens_Roland
 
 ## âï¸ What is Switchblade? Switchblade is a command line tool that lets you
 install and run dev tools from a central repository, and configure them in a
 standardised way across all your projects. ## Try it To use the included
 `python-poetry-base` bundle for Python, create a `.switchblade` file in your
 project root: ```toml [switchblade] bundle = "gh:jensroland/sentient-
 switchblade/bundles/python-poetry-base" mode = "python-poetry" ``` Then,
@@ -53,33 +53,52 @@
 be checked into version control (*seriously*) but rather **fetched on demand
 from a centrally managed dev tooling repository, and configured and invoked in
 exactly the same way in every repo, every time**. This would allow for a single
 source of truth for all dev tooling, and would make it easy to update
 configurations across all projects. To achieve this however, you would need
 some kind of small helper tool to abstract away the fetching, configuring and
 invoking of your centrally curated 'bundles' of dev tools. Switchblade is that
-tool. Learn more on the [Switchblade project website](https://jensroland.com/
-switchblade/). ## Custom bundles To create your own custom bundle with the dev
-tools and configurations you need, simply create a new Github repo and add a
+tool. ## Custom bundles To create your own custom bundle with the dev tools and
+configurations you need, simply create a new Github repo and add a
 `bundle.toml` file to it: ```toml [bundle] name = "my-dev-tool-bundle" mode =
 "python-poetry" schema_version = "1.0.0" # Linters [linters] all = ["pylint"]
 [linters.pylint] command = "pylint src" # Tests [tests] all = ["pytest"]
 [tests.pytest] command = "pytest -c pyproject.toml tests" # Extensions to
 pyproject.toml [tool.poetry.group.switchblade] optional = true
 [tool.poetry.group.switchblade.dependencies] pylint = "^2.17.2" pytest =
-"^7.3.1" [tool.pytest.ini_options] pythonpath = "src" ``` And in the same repo
-folder, add any config files you need, e.g. `.pylintrc`: ```ini [MAIN]
-[MESSAGES CONTROL] disable= C0111, # missing-docstring C0114, # missing-module-
-docstring C0115, # missing-class-docstring C0116, # missing-function-docstring
-W0613, # unused-argument ``` Now when you want to use your custom bundle in a
-project, simply point to the repo in the project `.switchblade` file as in the
-example above. Swtichblade will then fetch and install the tools you specified
-in the bundle and run them with the configurations you specified. Anything in
-the `bundle.toml` file under a `tool.*` section will be temporarily added to
-the project's `pyproject.toml` file under the same section. This allows you to
-add dependencies and configuration options to all your projects without having
-to manually edit all the individual `pyproject.toml` files. ## Prerequisites -
-[Python 3.7+](https://www.python.org/downloads/) Currently, you need Python
-since you install Switchblade with pip. This may change in the future. ##
-Features - CLI command `swb lint` to run linters - CLI command `swb test` to
-run tests - Project 'modes' supported: Currently only `python-poetry` is
-supported, but more will be added soon.
+"^7.3.1" [tool.pytest.ini_options] pythonpath = "src" ``` For each linter you
+want to add, specify a `[linters.]` section with a `command` key. The `command`
+value will be invoked by Switchblade when you run `swb lint `. The `[linters]`
+section specifies which linters should be invoked (and in which order) when you
+run `swb lint` or `swb lint all`. The same goes for tests: specify a `[tests.]`
+section with a `command` key, and add the tool to the `[tests]` section to have
+it invoked when you run `swb test` or `swb test all`. ### Tool configuration
+Anything in the `bundle.toml` file under a `tool.*` section will be temporarily
+added to the project's `pyproject.toml` file under that section. This allows
+you to add dependencies and configuration options to all your projects without
+having to manually edit all the individual `pyproject.toml` files. If you
+prefer having separate config files, or for tools which do not support
+`pyproject.toml` configuration, simply add any config files you need in the
+same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in
+the bundle repo: ```ini [MAIN] [MESSAGES CONTROL] disable= C0111, # missing-
+docstring C0114, # missing-module-docstring C0115, # missing-class-docstring
+C0116, # missing-function-docstring W0613, # unused-argument ``` Now, when you
+want to use your custom dev tool bundle in a project, simply point to the repo
+in the project `.switchblade` file as in the example above. Swichblade will
+then fetch and install the tools you specified in the bundle and run them with
+the configurations you specified. ### Per-project overrides To override the
+bundle configuration for a specific dev tool in one of your project repos,
+simply check in the tool dependencies and configuration files in the project
+repo as you normally would - Switchblade will still invoke the dev tool, but it
+will not overwrite any existing config files or `[tool.*]` sections in your
+`pyproject.toml` file. Be aware that this does not 'extend' the configuration
+from the bundle, but replaces that tool configuration entirely, so this feature
+should be used with caution. To override the command or the list of linters to
+run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in
+the project `.switchblade` file. Switchblade will automatically merge (in this
+case it does extend rather than replace) the bundle config and Switchblade
+config before invoking any of the tools. ## Prerequisites - [Python 3.7+]
+(https://www.python.org/downloads/) Currently, you need Python since you
+install Switchblade with pip. This may change in the future. ## Features - CLI
+command `swb lint` to run linters - CLI command `swb test` to run tests -
+Project 'modes' supported: Currently only `python-poetry` is supported, but
+more will be added soon.
```

