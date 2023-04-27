# Comparing `tmp/sentient_switchblade-0.1.1.tar.gz` & `tmp/sentient_switchblade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.1.1.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.1.2.tar", max compression
```

## Comparing `sentient_switchblade-0.1.1.tar` & `sentient_switchblade-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.1.1/LICENSE
--rw-r--r--   0        0        0     6679 2023-04-27 22:35:37.645490 sentient_switchblade-0.1.1/README.md
--rw-r--r--   0        0        0     1383 2023-04-27 22:46:35.896183 sentient_switchblade-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.1.1/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.1.1/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1656 2023-04-26 17:36:40.891577 sentient_switchblade-0.1.1/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    10671 2023-04-25 19:26:37.194064 sentient_switchblade-0.1.1/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.1.1/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:46.529573 sentient_switchblade-0.1.1/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0      820 2023-04-26 17:36:50.583261 sentient_switchblade-0.1.1/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.1.1/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.1.1/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0     9535 2023-04-26 17:36:59.378665 sentient_switchblade-0.1.1/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.1.1/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.1/setup.py
--rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6679 2023-04-27 22:35:37.645490 sentient_switchblade-0.1.2/README.md
+-rw-r--r--   0        0        0     1383 2023-04-27 23:18:39.260211 sentient_switchblade-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.1.2/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.1.2/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1656 2023-04-27 22:56:23.444492 sentient_switchblade-0.1.2/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    10301 2023-04-27 23:17:58.142250 sentient_switchblade-0.1.2/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.1.2/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0      820 2023-04-26 17:36:46.529573 sentient_switchblade-0.1.2/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0      820 2023-04-26 17:36:50.583261 sentient_switchblade-0.1.2/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.1.2/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.1.2/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0     9535 2023-04-26 17:36:59.378665 sentient_switchblade-0.1.2/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.1.2/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.2/setup.py
+-rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 sentient_switchblade-0.1.2/PKG-INFO
```

### Comparing `sentient_switchblade-0.1.1/LICENSE` & `sentient_switchblade-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/README.md` & `sentient_switchblade-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/pyproject.toml` & `sentient_switchblade-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.1.1"
+version = "0.1.2"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
```

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.1.2/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.1.2/src/switchbladecli/cli/bundle_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,26 +118,19 @@
         bundle_folder = self._bundle_folder_from_version(remote_version)
         if bundle_source_uri.startswith("gh:"):
             # Create the bundle folder
             bundle_folder.mkdir(parents=True)
             # Get the contents of the repo
             org_name, repo_name, *folder = bundle_source_uri[3:].split("/")
             repo = pygithub.get_repo(f"{org_name}/{repo_name}")
-            repo_contents = repo.get_contents("/".join(folder), ref=remote_version)
-            # If the contents are a folder, download it
-            if repo_contents.type == "dir":
-                for repo_asset in repo_contents:
-                    with open(bundle_folder / repo_asset.name, "wb") as file:
-                        file.write(repo_asset.decoded_content)
-            else:
-                # TODO: Use Click exception/error instead
-                cache.log(f"UPDATING {remote_version} FAILED")
-                raise Exception(
-                    f"Bundle URI {bundle_source_uri} is not a folder. Please use a folder in a Github repo."
-                )
+            repo_contents = repo.get_dir_contents("/".join(folder), ref=remote_version)
+            # Download all the files
+            for repo_asset in repo_contents:
+                with open(bundle_folder / repo_asset.name, "wb") as file:
+                    file.write(repo_asset.decoded_content)
         else:
             # If the source is a local folder, copy it to the cache
             shutil.copytree(bundle_source_uri, bundle_folder)
 
         cache.log(f"UPDATING {remote_version} SUCCEEDED")
 
         # Finally, return the cached bundle
```

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.1.2/src/switchbladecli/cli/lint.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.1.2/src/switchbladecli/cli/test.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/cli/update.py` & `sentient_switchblade-0.1.2/src/switchbladecli/cli/update.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.1.2/src/switchbladecli/modes/python_poetry.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/src/switchbladecli/utils.py` & `sentient_switchblade-0.1.2/src/switchbladecli/utils.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.1.1/setup.py` & `sentient_switchblade-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'tomlkit>=0.11.7,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
 
 setup_kwargs = {
     'name': 'sentient-switchblade',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
     'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://jensroland.com/switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png?" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\nLearn more on the [Switchblade project website](https://jensroland.com/switchblade/).\n\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nAnd in the same repo folder, add any config files you need, e.g. `.pylintrc`:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow when you want to use your custom bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swtichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under the same section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jensroland.com/sentient-switchblade',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['switchbladecli', 'switchbladecli.cli',
 'switchbladecli.modes'] package_data = \ {'': ['*']} install_requires = \
 ['PyGithub>=1.58.1,<2.0.0', 'checksumdir>=1.2.0,<2.0.0', 'click>=8.0.3,<9.0.0',
 'tomlkit>=0.11.7,<0.12.0'] entry_points = \ {'console_scripts': ['swb =
 switchbladecli.cli.__main__:switchbladecli']} setup_kwargs = { 'name':
-'sentient-switchblade', 'version': '0.1.1', 'description': 'Unleash Dev Tool
+'sentient-switchblade', 'version': '0.1.2', 'description': 'Unleash Dev Tool
 Mastery with a Flick of Your Wrist', 'long_description': '\n
                          \n \n_[Switchblade_logo]\n\n
 \n\n
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
 \n
                             created by Jens_Roland
 \n\n
```

### Comparing `sentient_switchblade-0.1.1/PKG-INFO` & `sentient_switchblade-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentient-switchblade
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
 Home-page: https://jensroland.com/sentient-switchblade
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.1.2 Summary:
 Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
 jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
 email: mail@jensroland.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

