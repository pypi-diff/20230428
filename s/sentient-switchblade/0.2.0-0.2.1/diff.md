# Comparing `tmp/sentient_switchblade-0.2.0.tar.gz` & `tmp/sentient_switchblade-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.2.0.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.2.1.tar", max compression
```

## Comparing `sentient_switchblade-0.2.0.tar` & `sentient_switchblade-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.2.0/LICENSE
--rw-r--r--   0        0        0     8177 2023-04-28 18:18:01.183570 sentient_switchblade-0.2.0/README.md
--rw-r--r--   0        0        0     1405 2023-04-28 18:11:29.738779 sentient_switchblade-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.2.0/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.2.0/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1656 2023-04-28 12:34:10.275655 sentient_switchblade-0.2.0/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    10660 2023-04-28 17:55:19.000402 sentient_switchblade-0.2.0/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.2.0/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0     1087 2023-04-28 18:13:37.061787 sentient_switchblade-0.2.0/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0     1089 2023-04-28 12:31:21.153690 sentient_switchblade-0.2.0/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.2.0/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.2.0/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0    10948 2023-04-28 18:13:26.743690 sentient_switchblade-0.2.0/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.2.0/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.0/setup.py
--rw-r--r--   0        0        0     9584 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8176 2023-04-28 18:20:25.734064 sentient_switchblade-0.2.1/README.md
+-rw-r--r--   0        0        0     1405 2023-04-28 20:20:39.564699 sentient_switchblade-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.2.1/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.2.1/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1656 2023-04-28 12:34:10.275655 sentient_switchblade-0.2.1/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    11308 2023-04-28 19:56:54.609233 sentient_switchblade-0.2.1/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.2.1/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0     1087 2023-04-28 18:13:37.061787 sentient_switchblade-0.2.1/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0     1089 2023-04-28 12:31:21.153690 sentient_switchblade-0.2.1/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.2.1/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.2.1/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0    11203 2023-04-28 20:16:15.140629 sentient_switchblade-0.2.1/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.2.1/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     9368 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.1/setup.py
+-rw-r--r--   0        0        0     9583 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.1/PKG-INFO
```

### Comparing `sentient_switchblade-0.2.0/LICENSE` & `sentient_switchblade-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/README.md` & `sentient_switchblade-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- markdownlint-disable first-line-h1 line-length no-inline-html -->
 <p align="center">
   <a href="https://github.com/JensRoland/sentient-switchblade">
-    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />
+    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />
   </a>
 </p>
 
 <h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>
 <p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>
 
 <br />
```

### Comparing `sentient_switchblade-0.2.0/pyproject.toml` & `sentient_switchblade-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.2.0"
+version = "0.2.1"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
```

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.2.1/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.2.1/src/switchbladecli/cli/bundle_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 import os
 import shutil
 
 from datetime import datetime, timezone
 from github import Github
+from mergedeep import merge
 from pathlib import Path
 from tomlkit import dumps, loads
 
 from switchbladecli.utils import hash_dir
 
 BUNDLE_CONFIG_FILES = ["bundle.toml"]
 CACHE_FOLDERNAME = ".switchblade-cache"
@@ -35,15 +36,14 @@
         self._switchblade_config = switchblade_config
         if version is None:
             cache = BundleCache(self._switchblade_config)
             bundle = self._fetch_latest(cache)
             self.version = bundle.version
             self.bundle_folder = bundle.bundle_folder
             self.bundle_config = bundle.bundle_config
-            cache.set_latest_config(bundle)
 
         else:
             self.version = version
             self.bundle_folder = self._bundle_folder_from_version(version)
             self.bundle_config = self._load_bundle_config()
     
 
@@ -111,15 +111,15 @@
         cache.log(f"UPDATING {remote_version}")
         
         # Check if the latest version from the remote is already cached
         # (does not necessarily have to be the most recently fetched bundle from 'latest.toml')
         if cache.has_bundle(remote_version):
             # If the latest cached bundle is up to date, just return it
             click.echo(f"⚔️ Switchblade cache already contains version {remote_version}")
-            cache.log(f"UPDATING {remote_version} USING_CACHED")
+            cache.log(f"UPDATING {remote_version} SKIPPED_ALREADY_CACHED")
             return Bundle(self._switchblade_config, remote_version)
 
         # If the cache is stale, update it
         click.echo(f"⚔️ Switchblade updating tool bundle to version {remote_version}...")
         bundle_folder = self._bundle_folder_from_version(remote_version)
         if bundle_source_uri.startswith("gh:"):
             # Create the bundle folder
@@ -134,16 +134,19 @@
                     file.write(repo_asset.decoded_content)
         else:
             # If the source is a local folder, copy it to the cache
             shutil.copytree(bundle_source_uri, bundle_folder)
 
         cache.log(f"UPDATING {remote_version} SUCCEEDED")
 
-        # Finally, return the cached bundle
-        return Bundle(self._switchblade_config, remote_version)
+        new_bundle = Bundle(self._switchblade_config, remote_version)
+        cache.set_latest_config(new_bundle)
+
+        # Finally, return the fetched bundle
+        return new_bundle
 
 
 class BundleCache:
 
     def __init__(self, switchblade_config: dict):
         self._switchblade_config = switchblade_config
         self._project_folder = Path(self._switchblade_config.get("project_dir"))
@@ -214,22 +217,38 @@
         latest_config_file = self._get_latest_config_file(False)
         with open(latest_config_file, "w") as latest_toml:
             latest_toml.write(
                 dumps(
                     {
                         "latest": {
                             "commit_sha": bundle.version,
-                            "timestamp": datetime.now(tz=timezone.utc).strftime("%Y-%m-%d %H:%M:%S"),
+                            "fetched_on": datetime.now(tz=timezone.utc).strftime("%Y-%m-%d %H:%M:%S"),
                             "files": bundle.get_files(),
+                            "last_installed_on": ""
                         }
                     }
                 )
             )
 
 
+    def update_latest_config(self, updated_latest: dict):
+        """Update the latest config, merging with updated dict."""
+        latest_config_file = self._get_latest_config_file(False)
+        latest_config = self.get_latest_config()
+        merge(latest_config, updated_latest)
+        with open(latest_config_file, "w") as latest_toml:
+            latest_toml.write(
+                dumps(
+                    {
+                        "latest": latest_config
+                    }
+                )
+            )
+
+
     def get_latest_version(self) -> str:
         """Get the latest version."""
         latest_config = self.get_latest_config()
         if latest_config is None:
             return None
         return latest_config["commit_sha"]
```

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.2.1/src/switchbladecli/cli/lint.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.2.1/src/switchbladecli/cli/test.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/cli/update.py` & `sentient_switchblade-0.2.1/src/switchbladecli/cli/update.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.2.1/src/switchbladecli/modes/python_poetry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from pathlib import Path
 import click
 import shutil
 import subprocess  # nosec
 
+from datetime import datetime, timezone
 from mergedeep import merge
 from tomlkit import dumps, loads
 
 from switchbladecli.cli.bundle_cache import Bundle, BundleCache
 
 
 class PythonPoetry:
 
-    RESET_LOCKFILE_ON_CLEANUP = False
+    SKIP_UPDATE_IF_INSTALLED_WITHIN = 60*60*24  # 24 hours
     mode = "python-poetry"
 
     def __init__(self, config: dict, verbose: bool):
         self._config = config
         self._project_folder = Path(config["project_dir"])
         self._verbose = verbose
         self._cache = BundleCache(self._config)
@@ -31,48 +32,47 @@
 
         self._pyproject_file_raw_before = self._pyproject_file.read_text(encoding="utf-8")
         self._poetry_lockfile_raw_before = self._poetry_lockfile.read_text(encoding="utf-8")  # TODO: handle missing file
         pyproject_config = loads(self._pyproject_file_raw_before)
         pyproject_config["tool"]["poetry"]["group"][
             "switchblade"
         ] = bundle.bundle_config["tool"]["poetry"]["group"]["switchblade"]
-        # pyproject_config["tool"]["poetry"]["group"]["switchblade"][
-        #     "dependencies"
-        # ] = bundle.bundle_config["tool"]["poetry"]["group"]["switchblade"][
-        #     "dependencies"
-        # ]
+
         # Also take all other sections beginning with 'tool.' and add them to the pyproject.toml
         # unless there is already a section with the same name in the pyproject.toml
         for section in bundle.bundle_config["tool"]:
             if not section.startswith("poetry") and section not in pyproject_config["tool"]:
                 pyproject_config["tool"][section] = bundle.bundle_config["tool"][
                     section
                 ]
         with open(self._pyproject_file, "w") as pyproject_toml:
             pyproject_toml.write(dumps(pyproject_config))
 
-        lock_check = subprocess.run(
-            ["poetry", "lock", "--check"],
-            cwd=self._project_folder,
-            check=False,
-            capture_output=True,
-        )
-
-        # If the lock file is up to date, we can optimistically skip the update
-        if lock_check.returncode == 0:
-            print("🔒 poetry.lock is up to date, install skipped")
-            return
+        # If the bundle was recently installed, we can optimistically skip the update
+        latest_config = self._cache.get_latest_config()
+        last_installed_on = latest_config["last_installed_on"]
+        print(f"last_installed_on: {last_installed_on}")
+        if last_installed_on:
+            last_installed_on = datetime.strptime(last_installed_on, "%Y-%m-%d %H:%M:%S").replace(tzinfo=timezone.utc)
+            current_datetime = datetime.now(tz=timezone.utc)
+            if (current_datetime - last_installed_on).total_seconds() < self.SKIP_UPDATE_IF_INSTALLED_WITHIN:
+                print("🔒 bundle dependencies were recently installed, skipping...")
+                return
 
         subprocess.run(
             ["poetry", "update", "--only", "switchblade"],
             cwd=self._project_folder,
             check=True,
             capture_output=False,
         )
 
+        self._cache.update_latest_config({
+            "last_installed_on": datetime.now(tz=timezone.utc).strftime("%Y-%m-%d %H:%M:%S")
+        })
+
 
     # TODO: Place this in a superclass
     def copy_config_files(self, bundle: Bundle):
         # For each file in the bundle, check if the file exists in the project folder
         pushed_files = []
         for file in bundle.get_files():
             if (self._project_folder / file).exists():
@@ -111,15 +111,15 @@
     # TODO: Make this an override
     def post_cleanup(self, bundle: Bundle, pushed_files: list):
         # Restore the original pyproject.toml
         if self._pyproject_file_raw_before:
             with open(self._pyproject_file, "w") as pyproject_toml:
                 pyproject_toml.write(self._pyproject_file_raw_before)
         # Restore the original poetry.lock
-        if self.RESET_LOCKFILE_ON_CLEANUP and self._poetry_lockfile_raw_before:
+        if self._poetry_lockfile_raw_before:
             with open(self._poetry_lockfile, "w") as poetry_lock:
                 poetry_lock.write(self._poetry_lockfile_raw_before)
 
 
     # TODO: Place this in a superclass
     def lint(self, linter_tool: str):
         # Instantiating a Bundle object will fetch the latest bundle from the source or cache
```

### Comparing `sentient_switchblade-0.2.0/src/switchbladecli/utils.py` & `sentient_switchblade-0.2.1/src/switchbladecli/utils.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.0/setup.py` & `sentient_switchblade-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'tomlkit>=0.11.7,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
 
 setup_kwargs = {
     'name': 'sentient-switchblade',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
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
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['switchbladecli', 'switchbladecli.cli',
 'switchbladecli.modes'] package_data = \ {'': ['*']} install_requires = \
 ['PyGithub>=1.58.1,<2.0.0', 'checksumdir>=1.2.0,<2.0.0', 'click>=8.0.3,<9.0.0',
 'mergedeep>=1.3.4,<2.0.0', 'tomlkit>=0.11.7,<0.12.0'] entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
-setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.2.0',
+setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.2.1',
 'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
 'long_description': '\n
                          \n \n_[Switchblade_logo]\n\n
 \n\n
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
 \n
                             Created by Jens_Roland
```

### Comparing `sentient_switchblade-0.2.0/PKG-INFO` & `sentient_switchblade-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentient-switchblade
-Version: 0.2.0
+Version: 0.2.1
 Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
 Home-page: https://jensroland.com/sentient-switchblade
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 Requires-Dist: tomlkit (>=0.11.7,<0.12.0)
 Project-URL: Repository, https://github.com/jensroland/sentient-switchblade
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable first-line-h1 line-length no-inline-html -->
 <p align="center">
   <a href="https://github.com/JensRoland/sentient-switchblade">
-    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />
+    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />
   </a>
 </p>
 
 <h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>
 <p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>
 
 <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.2.1 Summary:
 Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
 jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
 email: mail@jensroland.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

