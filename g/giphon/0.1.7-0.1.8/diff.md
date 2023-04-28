# Comparing `tmp/giphon-0.1.7.tar.gz` & `tmp/giphon-0.1.8.tar.gz`

## Comparing `giphon-0.1.7.tar` & `giphon-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__about__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/__main__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/git.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/gitlab.py
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 giphon-0.1.7/src/giphon/siphon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_git.py
--rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_gitlab.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/test_siphon.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 giphon-0.1.7/tests/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.1.7/.gitignore
--rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.1.7/LICENSE
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 giphon-0.1.7/README.md
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 giphon-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__about__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/__main__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/git.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/gitlab.py
+-rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 giphon-0.1.8/src/giphon/siphon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_git.py
+-rw-r--r--   0        0        0    10343 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_gitlab.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/test_siphon.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 giphon-0.1.8/tests/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 giphon-0.1.8/.gitignore
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 giphon-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 giphon-0.1.8/README.md
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 giphon-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 giphon-0.1.8/PKG-INFO
```

### Comparing `giphon-0.1.7/src/giphon/git.py` & `giphon-0.1.8/src/giphon/git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/src/giphon/gitlab.py` & `giphon-0.1.8/src/giphon/gitlab.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/src/giphon/siphon.py` & `giphon-0.1.8/src/giphon/siphon.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                 clone_task_id,
                 description=(f"Handling {element_type} {element_full_path}"),
             )
 
             if isinstance(element, Project):
                 if clone_through_ssh:
                     url_to_repo = element.ssh_url_to_repo
-                if not clone_through_ssh and gitlab_username:
+                elif not clone_through_ssh and gitlab_username:
                     parsed_url_to_repo = urlparse(element.http_url_to_repo)
 
                     unauthenticated_domain = parsed_url_to_repo.netloc.split(
                         "@"
                     )[-1]
 
                     authenticated_domain = (
```

### Comparing `giphon-0.1.7/tests/test_git.py` & `giphon-0.1.8/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/tests/test_gitlab.py` & `giphon-0.1.8/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/tests/test_siphon.py` & `giphon-0.1.8/tests/test_siphon.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/tests/utils.py` & `giphon-0.1.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/.gitignore` & `giphon-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/LICENSE` & `giphon-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `giphon-0.1.7/README.md` & `giphon-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -13,24 +13,31 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
-```shq
+```sh
 pip install --user giphon
 ```
 
+And if you wish to use giphon by simply calling `giphon`, you can set-up an 
+alias in your `.bashrc` (or other, if you have another shell):
+
+```sh
+echo 'alias giphon="/usr/bin/env python3 -m giphon"' >> ~/.bashrc
+```
+
 ## Parameters
 
 The `giphon` tool allows for the following parameters:
 
 - **namespace** (CLI: `--namespace`): The Gitlab namespace to be cloned. `/`
   defaults to the whole instance.
 - **output** (CLI: `--output`): The target path to clone the repositories to.
```

### Comparing `giphon-0.1.7/pyproject.toml` & `giphon-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "typer>=0.7",
   "python-gitlab>=3,<4",
   "GitPython>=3,<4",
-  "rich>=12,<13",
+  "rich>=12,<14",
 ]
 description = "Copy locally a Gitlab group or instance"
 dynamic = ["version"]
 keywords = [
   "gitlab",
   "clone",
   "copy",
```

### Comparing `giphon-0.1.7/PKG-INFO` & `giphon-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giphon
-Version: 0.1.7
+Version: 0.1.8
 Summary: Copy locally a Gitlab group or instance
 Project-URL: Bug Reports, https://github.com/kabooboo/giphon/issues
 Project-URL: Documentation, https://github.com/kabooboo/giphon
 Project-URL: Homepage, https://github.com/kabooboo/giphon
 Project-URL: Source Code, https://github.com/kabooboo/giphon
 Author-email: Gabriel Creti <gabrielcreti@gmail.com>
 License-File: LICENSE
@@ -20,21 +20,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Requires-Dist: gitpython<4,>=3
 Requires-Dist: python-gitlab<4,>=3
-Requires-Dist: rich<13,>=12
+Requires-Dist: rich<14,>=12
 Requires-Dist: typer>=0.7
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/logo.png)
+![Logo](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/logo.png)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/giphon) [![Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://pypi.org/project/black/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kabooboo/giphon/test.yml?label=tests)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) ![PyPI](https://img.shields.io/pypi/v/giphon) ![PyPI - License](https://img.shields.io/pypi/l/giphon) ![GitHub Repo stars](https://img.shields.io/github/stars/kabooboo/giphon?style=social)
 
 ---
 
 ✨ Giphon is the contraction of 🦊 _Gitlab_ and 🫗 _siphon_. This CLI tools allows users
 to recursively clone all projects in a given Gitlab group or instance.
@@ -45,24 +45,31 @@
 structure into a directory structure.
 
 Locally cloned projects enable users to use familiar CLI tools such as `grep`
 and `sed` directly into the projects' tree structure.
 
 ## Demo
 
-![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.7/docs/assets/usage.gif)
+![Usage GIF](https://raw.githubusercontent.com/kabooboo/giphon/0.1.8/docs/assets/usage.gif)
 
 ## Installation
 
 To install `giphon`, simply run:
 
-```shq
+```sh
 pip install --user giphon
 ```
 
+And if you wish to use giphon by simply calling `giphon`, you can set-up an 
+alias in your `.bashrc` (or other, if you have another shell):
+
+```sh
+echo 'alias giphon="/usr/bin/env python3 -m giphon"' >> ~/.bashrc
+```
+
 ## Parameters
 
 The `giphon` tool allows for the following parameters:
 
 - **namespace** (CLI: `--namespace`): The Gitlab namespace to be cloned. `/`
   defaults to the whole instance.
 - **output** (CLI: `--output`): The target path to clone the repositories to.
```

