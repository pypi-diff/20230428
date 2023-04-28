# Comparing `tmp/katalytic-pkg-0.2.6.tar.gz` & `tmp/katalytic-pkg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.2.6.tar", last modified: Fri Apr 14 18:15:14 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.3.0.tar", last modified: Fri Apr 28 10:35:32 2023, max compression
```

## Comparing `katalytic-pkg-0.2.6.tar` & `katalytic-pkg-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
--rw-r--r--   0        0        0       54 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.travis.yml
--rw-r--r--   0        0        0     1726 2023-04-14 18:15:09.736616 katalytic-pkg-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/LICENSE.txt
--rw-r--r--   0        0        0     1542 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/README.md
--rw-r--r--   0        0        0     1399 2023-04-14 18:15:09.232868 katalytic-pkg-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/pytest.sh
--rw-r--r--   0        0        0     2867 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/venv.sh
--rw-r--r--   0        0        0     4107 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2829 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/tests/test_pkg.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-09 20:01:14.425566 katalytic-pkg-0.3.0/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-pkg-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3109 2023-04-27 17:14:43.739675 katalytic-pkg-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1907 2023-04-28 10:27:14.416328 katalytic-pkg-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-07 08:03:04.896413 katalytic-pkg-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1664 2023-04-14 19:07:14.523511 katalytic-pkg-0.3.0/README.md
+-rw-r--r--   0        0        0     1315 2023-04-28 10:33:33.839879 katalytic-pkg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4664 2023-04-28 10:15:23.681535 katalytic-pkg-0.3.0/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2829 2023-04-28 10:02:55.132516 katalytic-pkg-0.3.0/tests/test_pkg.py
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 katalytic-pkg-0.3.0/PKG-INFO
```

### Comparing `katalytic-pkg-0.2.6/.gitignore` & `katalytic-pkg-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.6/CHANGELOG.md` & `katalytic-pkg-0.3.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.3.0 (2023-04-28)
+### feat
+- [[`655bfc7`](https://gitlab.com/katalytic/katalytic-pkg/commit/655bfc7c069f244366fb12c09fe3f06e61fcd7d6)] **get_modules:** find editable installs
+
+
 ## 0.2.6 (2023-04-14)
 ### Fix
 * Merge branch 'main' of gitlab.com:katalytic/katalytic-pkg ([`1710c63`](https://github.com/katalytic/katalytic-pkg/commit/1710c6341d1f367d56ec673afd4bf588067fb484))
 * **get_version:** Return the correct version for katalytic instead of the one of the first plugin found ([`577cc8e`](https://github.com/katalytic/katalytic-pkg/commit/577cc8ebb588fd63172b97b5811b379a3395a531))
 
 
 ## 0.2.5 (2023-04-14)
```

### Comparing `katalytic-pkg-0.2.6/LICENSE.txt` & `katalytic-pkg-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.6/README.md` & `katalytic-pkg-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
 [![Build Status](https://app.travis-ci.com/katalytic/katalytic-pkg.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
 [![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-pkg?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
 [![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-pkg/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-pkg?branch=main)
+[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-pkg
 ```
```

### Comparing `katalytic-pkg-0.2.6/pyproject.toml` & `katalytic-pkg-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.2.6"
+version = "0.3.0"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -46,16 +46,13 @@
 env_list = py36, py37, py38, py39
 isolated_build = True
 
 [testenv]
 extras = dev
 deps = -e .
 
-commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
+commands =
+	pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
 """
 
-[tool.semantic_release]
-version_variable = "pyproject.toml:version"
-branch = "main"
-
 [tool.flit.module]
 name = "katalytic.pkg"
```

### Comparing `katalytic-pkg-0.2.6/src/katalytic/pkg.py` & `katalytic-pkg-0.3.0/src/katalytic/pkg.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,14 +97,29 @@
             module = import_module(module_name)
         except Exception as e:  # pragma: no cover
             warnings.warn(f'Couldn\'t import {module_name!r}\n' + _get_stacktrace(e))
             continue
 
         modules.append(module)
 
+    # find editable installs
+    for item in Path(__file__).parent.parent.iterdir():  # pragma: no cover
+        # no coverage: because I would have to create an editable install,
+        # just to test this functionality
+        if not re.search(__package__ + r'\..*\.pth', item.name):
+            continue
+
+        try:
+            module = import_module(item.stem)
+        except Exception as e:  # pragma: no cover
+            warnings.warn(f'Couldn\'t import {item.stem!r}\n' + _get_stacktrace(e))
+            continue
+
+        modules.append(module)
+
     return sorted(modules, key=lambda m: m.__name__)
 
 
 def get_functions_in_group(group):
     functions = []
     for module in get_modules():
         for func_name in dir(module):
```

### Comparing `katalytic-pkg-0.2.6/tests/test_pkg.py` & `katalytic-pkg-0.3.0/tests/test_pkg.py`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.6/PKG-INFO` & `katalytic-pkg-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.2.6
+Version: 0.3.0
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-pkg)](https://pypi.org/project/katalytic-pkg/)
 [![Build Status](https://app.travis-ci.com/katalytic/katalytic-pkg.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
 [![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-pkg?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-pkg)
 [![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-pkg/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-pkg?branch=main)
+[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-pkg.svg)](https://katalytic-pkg.readthedocs.io/en/latest/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-pkg
 ```
```

