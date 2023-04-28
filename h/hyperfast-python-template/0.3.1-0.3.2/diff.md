# Comparing `tmp/hyperfast_python_template-0.3.1.tar.gz` & `tmp/hyperfast_python_template-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.3.1.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.3.2.tar", max compression
```

## Comparing `hyperfast_python_template-0.3.1.tar` & `hyperfast_python_template-0.3.2.tar`

### file list

```diff
@@ -1,4 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-04-27 07:17:54.819143 hyperfast_python_template-0.3.1/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-27 07:17:48.690796 hyperfast_python_template-0.3.1/README.md
--rw-r--r--   0        0        0     3112 2023-04-27 07:18:14.036223 hyperfast_python_template-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/README.md
+-rw-r--r--   0        0        0     2968 2023-04-28 04:17:24.384385 hyperfast_python_template-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-28 04:17:24.336387 hyperfast_python_template-0.3.2/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-04-28 04:17:24.336387 hyperfast_python_template-0.3.2/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-04-28 04:17:06.772614 hyperfast_python_template-0.3.2/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     6364 1970-01-01 00:00:00.000000 hyperfast_python_template-0.3.2/PKG-INFO
```

### Comparing `hyperfast_python_template-0.3.1/LICENSE` & `hyperfast_python_template-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.3.1/README.md` & `hyperfast_python_template-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.3.1/pyproject.toml` & `hyperfast_python_template-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.3.1"
+version = "0.3.2"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
+repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
 hyperfastpy = 'hyperfastpy.__cli__:main'
 
 [tool.poetry.dependencies]
@@ -27,64 +28,28 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe]
 include = ".tasks.toml"
 
 [tool.black]
-exclude = [
-    '_version.py',
-    'node_modules',
-    '_build',
-    'docs',
-    'tests',
-    'venv',
-    '.copier-template',
-    '.refs',
-]
+exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
-skip = [
-    '_version.py',
-    'node_modules',
-    '_build',
-    'docs',
-    'tests',
-    'venv',
-    '.copier-template',
-    '.refs',
-]
+skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.flake8]
 ignore = ['F401', 'E501', 'W503']
-exclude = [
-    "node_modules",
-    "_build",
-    "docs",
-    "tests",
-    "venv",
-    ".copier-template",
-    ".refs",
-]
+exclude = ["node_modules", "_build", "docs", "tests", "venv", ".copier-template", ".refs"]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
-exclude = [
-    "node_modules",
-    "build",
-    "_build",
-    "dist",
-    "docs",
-    "tests",
-    "venv",
-    ".copier-template",
-    ".refs",
-]
+exclude = ["node_modules", "build", "_build", "dist", "docs", "tests", "venv", ".copier-template", ".refs"]
 # 3rd party import
 ignore_missing_imports = true
 # dynamic typing
 disallow_any_unimported = true
 disallow_any_expr = false
 disallow_any_decorated = false
 disallow_any_explicit = true
@@ -112,29 +77,27 @@
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 
-[tool.setuptools_scm]
-write_to_template = '__version__ = "{version}"'
-tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
-
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
+version_variable = "src/hyperfastpy/_version.py:__version__"
+version_pattern = 'src/hyperfastpy/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
-commit_version_number = true                                    # required for version_source = "tag"
+commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
-hvcs = "github"                                                 # hosting version control system, gitlab is also supported
+hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hyperfast_python_template-0.3.1/PKG-INFO` & `hyperfast_python_template-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/entelecheia/hyperfast-python-template
 Description-Content-Type: text/markdown
 
 # Hyperfast Python Template
 
 [![license-image]][license-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
```

