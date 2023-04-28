# Comparing `tmp/generic-path-0.1.tar.gz` & `tmp/generic-path-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-path-0.1.tar", last modified: Fri Apr 28 01:18:32 2023, max compression
+gzip compressed data, was "generic-path-0.2.tar", last modified: Fri Apr 28 04:16:46 2023, max compression
```

## Comparing `generic-path-0.1.tar` & `generic-path-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:18:32.689732 generic-path-0.1/
--rw-rw-rw-   0        0        0    17098 2023-04-27 15:37:26.000000 generic-path-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5362 2023-04-28 01:18:32.688732 generic-path-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3920 2023-04-28 01:17:40.000000 generic-path-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 01:18:32.687733 generic-path-0.1/generic_path.egg-info/
--rw-rw-rw-   0        0        0     5362 2023-04-28 01:18:32.000000 generic-path-0.1/generic_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-28 01:18:32.000000 generic-path-0.1/generic_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:18:32.000000 generic-path-0.1/generic_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-04-28 01:18:32.000000 generic-path-0.1/generic_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 01:18:32.000000 generic-path-0.1/generic_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24579 2023-04-28 01:02:08.000000 generic-path-0.1/gpath.py
--rw-rw-rw-   0        0        0     1811 2023-04-28 01:14:46.000000 generic-path-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 01:18:32.689732 generic-path-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 01:18:32.687733 generic-path-0.1/tests/
--rw-rw-rw-   0        0        0    35176 2023-04-27 23:11:47.000000 generic-path-0.1/tests/test_gpath.py
+drwxrwxrwx   0        0        0        0 2023-04-28 04:16:46.033875 generic-path-0.2/
+-rw-rw-rw-   0        0        0      126 2023-04-28 04:03:00.000000 generic-path-0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    17098 2023-04-27 15:37:26.000000 generic-path-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5654 2023-04-28 04:16:46.032888 generic-path-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3906 2023-04-28 04:15:24.000000 generic-path-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 04:16:46.032356 generic-path-0.2/generic_path.egg-info/
+-rw-rw-rw-   0        0        0     5654 2023-04-28 04:16:46.000000 generic-path-0.2/generic_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-28 04:16:46.000000 generic-path-0.2/generic_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 04:16:46.000000 generic-path-0.2/generic_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2023-04-28 04:16:46.000000 generic-path-0.2/generic_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 04:16:46.000000 generic-path-0.2/generic_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25172 2023-04-28 04:15:49.000000 generic-path-0.2/gpath.py
+-rw-rw-rw-   0        0        0     2132 2023-04-28 04:12:13.000000 generic-path-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 04:16:46.033875 generic-path-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 04:16:46.032888 generic-path-0.2/tests/
+-rw-rw-rw-   0        0        0    35409 2023-04-28 03:55:11.000000 generic-path-0.2/tests/test_gpath.py
```

### Comparing `generic-path-0.1/LICENSE.txt` & `generic-path-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `generic-path-0.1/PKG-INFO` & `generic-path-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: generic-path
-Version: 0.1
+Version: 0.2
 Summary: GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/GPath
 Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
 Keywords: python,filepath,filesystem,cross-platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: config
 Provides-Extra: package
+Provides-Extra: packagetest
+Provides-Extra: ci
 Provides-Extra: publish
 License-File: LICENSE.txt
 
 # GPath
 
 **GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 
@@ -73,21 +78,21 @@
 The `GPath.partition()` method is useful when dealing with paths from various different sources:
 ```python
 partitions = GPath.partition("/usr/bin", "/usr/local/", "../../doc", "C:/Windows", "C:/Program Files")
 
 assert partitions == {
 	GPath("/usr")      : [GPath("/usr/bin"), GPath("/usr/local")],
 	GPath("../../doc") : [GPath("")],
-	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")]
+	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
 }
 ```
 
 ## Issues
 
-Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls)
+Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
 
 ## Development
 
 Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
 
 The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
 
@@ -111,26 +116,37 @@
 
 For unit tests, run `pytest` or `coverage run -m pytest`.
 
 For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`.
 
 ### Packaging
 
-Before packaging, check the package configuration by running `pyroma .`
+Before packaging, check the package config by running `pyroma .`
 
 To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`.
 
+### Automated tests
+
+To test for different supported environments, run `tox -p` or <code>tox -p <var>num_workers</var></code>. This will run unit tests, check for test coverage, and also generate packages.
+
 ### Config files
 
-- `pyproject.toml` Package metadata, as well as configs for pytest and setuptools
+- `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
+- `tox.ini` Config file for tox
 
 ### Troubleshooting
 
 #### Unable to uninstall the local package
 
 Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
 <pre><code>Found existing installation: gpath <var>version</var>
 Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
 
-In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, as well as `Lib/site-packages/gpath.py` and <code>Lib/site-packages/generic_path-<var>version</var>.dist-info/</code>, then verify that pip no longer sees the package by running `pip list`. If the package was installed outside of a local venv, the latter two items would instead be found at the same location where the other pip packages are installed.
+In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
+
+## Changelog
+
+### 0.2
+
+- Added support for Python versions 3.7 through 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `generic-path-0.1/README.md` & `generic-path-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 The `GPath.partition()` method is useful when dealing with paths from various different sources:
 ```python
 partitions = GPath.partition("/usr/bin", "/usr/local/", "../../doc", "C:/Windows", "C:/Program Files")
 
 assert partitions == {
 	GPath("/usr")      : [GPath("/usr/bin"), GPath("/usr/local")],
 	GPath("../../doc") : [GPath("")],
-	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")]
+	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
 }
 ```
 
 ## Issues
 
-Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls)
+Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
 
 ## Development
 
 Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
 
 The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
 
@@ -81,26 +81,31 @@
 
 For unit tests, run `pytest` or `coverage run -m pytest`.
 
 For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`.
 
 ### Packaging
 
-Before packaging, check the package configuration by running `pyroma .`
+Before packaging, check the package config by running `pyroma .`
 
 To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`.
 
+### Automated tests
+
+To test for different supported environments, run `tox -p` or <code>tox -p <var>num_workers</var></code>. This will run unit tests, check for test coverage, and also generate packages.
+
 ### Config files
 
-- `pyproject.toml` Package metadata, as well as configs for pytest and setuptools
+- `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
+- `tox.ini` Config file for tox
 
 ### Troubleshooting
 
 #### Unable to uninstall the local package
 
 Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
 <pre><code>Found existing installation: gpath <var>version</var>
 Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
 
-In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, as well as `Lib/site-packages/gpath.py` and <code>Lib/site-packages/generic_path-<var>version</var>.dist-info/</code>, then verify that pip no longer sees the package by running `pip list`. If the package was installed outside of a local venv, the latter two items would instead be found at the same location where the other pip packages are installed.
+In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
```

### Comparing `generic-path-0.1/generic_path.egg-info/PKG-INFO` & `generic-path-0.2/generic_path.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: generic-path
-Version: 0.1
+Version: 0.2
 Summary: GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 Author-email: Yu Shiyang <yu.shiyang@gnayihs.uy>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/yushiyangk/GPath
 Project-URL: Issues, https://github.com/yushiyangk/GPath/issues
 Keywords: python,filepath,filesystem,cross-platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: config
 Provides-Extra: package
+Provides-Extra: packagetest
+Provides-Extra: ci
 Provides-Extra: publish
 License-File: LICENSE.txt
 
 # GPath
 
 **GPath** is a Python package that provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 
@@ -73,21 +78,21 @@
 The `GPath.partition()` method is useful when dealing with paths from various different sources:
 ```python
 partitions = GPath.partition("/usr/bin", "/usr/local/", "../../doc", "C:/Windows", "C:/Program Files")
 
 assert partitions == {
 	GPath("/usr")      : [GPath("/usr/bin"), GPath("/usr/local")],
 	GPath("../../doc") : [GPath("")],
-	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")]
+	GPath("C:/")       : [GPath("Windows"), GPath("Program Files")],
 }
 ```
 
 ## Issues
 
-Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls)
+Found a bug? Please [file an issue](https://github.com/yushiyangk/GPath/issues), or, better yet, [submit a pull request](https://github.com/yushiyangk/GPath/pulls).
 
 ## Development
 
 Clone the repository with `git clone https://github.com/yushiyangk/GPath.git`.
 
 The source for the package is entirely contained in `gpath.py`, with tests in `tests/`.
 
@@ -111,26 +116,37 @@
 
 For unit tests, run `pytest` or `coverage run -m pytest`.
 
 For coverage report, first run `coverage run -m pytest`, then either `coverage report -m` to print to stdout or `coverage html` to generate an HTML report in `htmlcov/`.
 
 ### Packaging
 
-Before packaging, check the package configuration by running `pyroma .`
+Before packaging, check the package config by running `pyroma .`
 
 To generate sdist and wheel packages, delete `dist/` and `generic_path.egg-info/` if they exist, then run `python -m build`.
 
+### Automated tests
+
+To test for different supported environments, run `tox -p` or <code>tox -p <var>num_workers</var></code>. This will run unit tests, check for test coverage, and also generate packages.
+
 ### Config files
 
-- `pyproject.toml` Package metadata, as well as configs for pytest and setuptools
+- `pyproject.toml` Package metadata, as well as configs for test and build tools
 - `requirements.dev.txt` Package dependencies for development, in pip format
 - `requirements.publish.txt` Package dependencies for publishing, in pip format
+- `tox.ini` Config file for tox
 
 ### Troubleshooting
 
 #### Unable to uninstall the local package
 
 Sometimes, if gpath was installed using `pip install .`, pip might have difficulty uninstalling the package, giving the contradictory message
 <pre><code>Found existing installation: gpath <var>version</var>
 Can't uninstall 'gpath'. No files were found to uninstall.</code></pre>
 
-In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, as well as `Lib/site-packages/gpath.py` and <code>Lib/site-packages/generic_path-<var>version</var>.dist-info/</code>, then verify that pip no longer sees the package by running `pip list`. If the package was installed outside of a local venv, the latter two items would instead be found at the same location where the other pip packages are installed.
+In this case, manually delete `build/` and `generic_path.egg-info/` if they exist, then run `pip uninstall generic-path` again. This should allow pip to successfully uninstall the package.
+
+## Changelog
+
+### 0.2
+
+- Added support for Python versions 3.7 through 3.9; previously only 3.10 and 3.11 were supported
```

### Comparing `generic-path-0.1/gpath.py` & `generic-path-0.2/gpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,42 @@
 	GPath is a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system.
 """
 
 from __future__ import annotations
 
 import functools
 import os
+import sys
 from collections.abc import Collection, Iterator, Sequence
-from typing import Any, Final, ClassVar
+#from typing import Any, ClassVar, Final
+
+
+# Type hinting prior to 3.10
+# Using generics in built-in collections, e.g. list[int], is supported from 3.7 by __future__.annotations
+from typing import Any, ClassVar, Optional, Union
+if sys.version_info >= (3, 8):
+	from typing import Final
+else:
+	Final = Any
+def is_gpathlike(obj: Any) -> bool:
+	if sys.version_info >= (3, 10):
+		return isinstance(obj, GPathLike)
+	else:
+		return isinstance(obj, GPath) or isinstance(obj, str) or isinstance(obj, os.PathLike)
+
+
+__version__ = '0.2'
 
-__version__ = '0.1'
 
 PATH_SEPARATOR: Final = "/" if os.sep == '/' or os.altsep == '/' else os.sep
 PATH_CURRENT: Final = os.curdir
 PATH_PARENT: Final = os.pardir
 
-PathLike = str | os.PathLike
+PathLike = Union[str, os.PathLike]
+
 
 @functools.total_ordering
 class GPath():
 	"""
 		A normalised and generalised abstract file path that has no dependency on the layout of any real filesystem. This allows us to manipulate file paths that were generated on a different system, particularly one with a different operating environment as compared to the local system.
 
 		The path can be manipulated before being rendered in a format that is meaningful to the local operating system.
@@ -34,15 +52,16 @@
 
 	__slots__ = ('_parts', '_device', '_root', '_dotdot')
 
 	separator: ClassVar = PATH_SEPARATOR
 	current: ClassVar = PATH_CURRENT
 	parent: ClassVar = PATH_PARENT
 
-	def __init__(self, path: PathLike | GPath | None="") -> None:
+
+	def __init__(self, path: Union[PathLike, GPath, None]="") -> None:
 		"""
 			Initialise a normalised and generalised abstract file path, possibly by copying an existing GPath object.
 
 			Evoked by `GPath(path)`
 
 			Parameters
 			----------
@@ -82,25 +101,27 @@
 
 				dotdot = 0
 				while dotdot < len(parts) and parts[dotdot] == GPath.parent:  # GPath.parent == '..' usually
 					dotdot += 1
 				self._parts = tuple(parts[dotdot:])
 				self._dotdot = dotdot
 
+
 	@staticmethod
 	def from_parts(parts: Sequence[str]) -> GPath:
 		"""
 			Static method. Create a GPath object from a sequence of path components, such as that generated by `get_parts()`.
 
 			Note that unlike `GPath.join()`, this method expects each item in the sequence to be a single string without any file separators. Absolute paths are represented in the same manner as returned by `get_parts()`.
 		"""
 		return GPath(GPath.separator.join(parts))
 
+
 	@staticmethod
-	def find_common(path1: GPathLike, path2: GPathLike, common_current: bool=True, common_parent: bool=False) -> GPath | None:
+	def find_common(path1: GPathLike, path2: GPathLike, common_current: bool=True, common_parent: bool=False) -> Optional[GPath]:
 		"""
 			Static method. Find the longest common base path shared by the two paths. Return None if the two paths do not share any base components, such as if they are not both relative paths or both absolute paths, or if they are rooted on different device names.
 
 			By default, two non-parent relative paths that do not share any named components are still considered to share a common base path, namely the imaginary current working directory (e.g. `GPath("some/rel/path")` and `GPath("another/rel/path")` will give `GPath("")` by default). To prevent this, set `common_current` to False, and None will be returned instead.
 
 			By default, two relative paths that are relative to different levels of parent directories are considered to not have a common base path, and will return None. To prevent this, set `common_parent` to True in order to return the highest level parent directory between the two paths (e.g. `("../relative/to/parent")` and `GPath("../../relative/to/grandparent")` will give `GPath("../..")` if `common_parent` is True). Note that `common_parent` implies `common_current`.
 
@@ -168,16 +189,17 @@
 		common_path._parts = tuple(parts)
 
 		if not common_current and not bool(common_path):
 			if common_path != path1 or common_path != path2:
 				return None
 		return common_path
 
+
 	@staticmethod
-	def partition(*paths: Collection[GPathLike] | GPathLike, **find_common_kwargs: bool) -> dict[GPath, list[GPath]]:
+	def partition(*paths: Union[Collection[GPathLike], GPathLike], **find_common_kwargs: bool) -> dict[GPath, list[GPath]]:
 		"""
 			Static method. Partition a collection of paths based on the common base paths shared between members of the collection, such that each path can only belong to one partition. Return a list of relative paths from the common base path in each partition.
 
 			The partitioning logic is similar to that of `GPath.common()`; by default, non-parent relative paths are always placed in the same partition, while paths that are relative to different levels of parent directories will be placed in separate partitions.
 
 			Note that `common_parent` should only be set to True if the members of each partition are not of interest. When `common_parent` is True, the output lists will all be explicitly empty, because it is not possible to obtain a relative path from a parent directory of a higher level to one of a lower level. In most cases, this option should not be used.
 
@@ -200,15 +222,15 @@
 			Raises
 			------
 			  `ValueError`
 			  if any of the GPaths are invalid
 		"""
 		flattened_paths: list[GPathLike] = []
 		for path_or_list in paths:
-			if isinstance(path_or_list, GPathLike):
+			if is_gpathlike(path_or_list):
 				flattened_paths.append(path_or_list)
 			else:
 				flattened_paths.extend(path_or_list)
 		gpaths = [path if isinstance(path, GPath) else GPath(path) for path in flattened_paths]
 
 		partition_map = {}
 		if len(gpaths) > 0:
@@ -236,16 +258,17 @@
 					partition_map[path] = [path]
 
 		for partition, path_list in partition_map.items():
 			partition_map[partition] = [path.subpath_from(partition) for path in path_list]
 
 		return partition_map
 
+
 	@staticmethod
-	def join(*paths: Collection[GPathLike]) -> GPath:
+	def join(*paths: Union[Collection[GPathLike], GPathLike]) -> GPath:
 		"""
 			Join a sequence of paths into a single path. Apart from the first item in the sequence, all subsequent paths should be relative paths and any absolute paths will be ignored.
 
 			Evoked by either `GPath.join([gpath1, gpath2, ...])` or `GPath.join(gpath1, gpath2, ...)`
 
 			Parameters
 			----------
@@ -260,15 +283,15 @@
 			Raises
 			------
 			  `ValueError`
 			  if any of the GPaths are invalid
 		"""
 		flattened_paths: list[GPathLike] = []
 		for path_or_list in paths:
-			if isinstance(path_or_list, GPathLike):
+			if is_gpathlike(path_or_list):
 				flattened_paths.append(path_or_list)
 			else:
 				flattened_paths.extend(path_or_list)
 
 		if len(flattened_paths) == 0:
 			return GPath()
 
@@ -276,14 +299,15 @@
 		if not isinstance(combined_path, GPath):
 			combined_path = GPath(combined_path)
 		for path in flattened_paths[1:]:
 			combined_path = combined_path + path
 
 		return combined_path
 
+
 	def get_parts(self, root: bool=True, parent: bool=True) -> list[str]:
 		"""
 			Get a list of strings representing each component of the path.
 
 			By default, components representing the full path is returned in such a way that it can be reconstructed as a string using `GPath.separator.join(mygpath.get_parts())`. If it is an absolute path, the first item of the returned list will contain the device name if it exists, or be an empty string otherwise. If the path is exactly the filesystem root, the returned list will contain exactly two items, with the second being an empty string.
 
 			If the path is relative to an parent directory (e.g. '../..'), each parent level will be given as a separate item in the returned list.
@@ -318,41 +342,43 @@
 				# bool(self) == False
 				return [GPath.current]
 
 			base_parts = []
 
 		return base_parts + list(self._parts)
 
+
 	def get_parent_parts(self) -> list[str]:
 		"""
 			Get a list of strings representing the parent directory that the path is relative to, if any.
 
 			The returned list will contain a copy of `GPath.parent` for each parent level. If the path is not relative to a parent directory, the returned list will be empty.
 		"""
 		return [GPath.parent for i in range(self._dotdot)]
 
 	def get_parent_level(self) -> int:
 		"""
 			Get the number of levels of parent directories that the path is relative to, if any.
 		"""
 		return self._dotdot
 
-	def get_device(self) -> str | None:
+	def get_device(self) -> Optional[str]:
 		"""
 			Get the device name of the path.
 		"""
 		return self._device
 
 	def is_root(self) -> bool:
 		"""
 			Check if the path is relative to filesystem root
 		"""
 		return self._root
 
-	def subpath_from(self, base: GPathLike) -> GPath | None:
+
+	def subpath_from(self, base: GPathLike) -> Optional[GPath]:
 		"""
 			Find the relative subpath from `base` to `self` if possible and if `base` contains `self`, or return None otherwise.
 
 			None will be returned if there are components with names that cannot be known in the subpath, for instance when `self` and `base` base are relative paths with `base` being relative to a parent directory of a higher level than `self`.
 
 			Parameters
 			----------
@@ -379,15 +405,16 @@
 			base_length = len(base._parts)
 			new_path = GPath()
 			new_path._parts = self._parts[base_length:]  # () when self == base
 			return new_path
 		else:
 			return None
 
-	def relpath_from(self, origin: GPathLike) -> GPath | None:
+
+	def relpath_from(self, origin: GPathLike) -> Optional[GPath]:
 		"""
 			Find the relative path from `origin` to `self` if possible, or return None otherwise.
 
 			None will be returned if there are components with names that cannot be known in the relative path, for instance when `self` is a relative path while `origin` is an absolute path or a path that is relative to a parent directory of a higher level than `self`.
 
 			Parameters
 			----------
@@ -439,111 +466,122 @@
 				new_path._parts = self._parts
 			else:
 				new_path._dotdot = len(origin) - len(common)
 				new_path._parts = self._parts[len(common):]
 
 			return new_path
 
+
 	def __hash__(self) -> int:
 		"""
 			Calculate hash of the GPath object.
 
 			Evoked by `hash(mygpath)`
 		"""
 		return hash((tuple(self._parts), self._device, self._root, self._dotdot))
 
+
 	def __eq__(self, other: Any) -> bool:
 		"""
 			Check if two GPaths are completely identical. Always return False if `other` is not a GPath object, even if it is a GPath-like object.
 
 			Evoked by `gpath1 == gpath2`
 		"""
 		if isinstance(other, GPath):
 			return ((self._root, self._device, self._dotdot) + self._parts) == ((other._root, other._device, other._dotdot) + other._parts)
 		else:
 			return False
 
+
 	def __gt__(self, other: GPathLike) -> bool:
 		"""
 			Check if `self` should be collated after `other` by comparing their component-wise lexicographical order. Absolute paths come before (is less than) parent relative paths, which come before (is less than) non-parent relative paths. Between two parent relative paths, the path with the higher parent level is considered greater (comes later).
 
 			Evoked by `gpath1 < gpath2`
 		"""
 		if not isinstance(other, GPath):
 			other = GPath(other)
 		return ((not self._root, self._device, -1 * self._dotdot) + self._parts) > ((not other._root, other._device, -1 * other._dotdot) + other._parts)
 
+
 	def __bool__(self) -> bool:
 		"""
 			Return True if `self` is an absolute path, if `self` is relative to a parent directory, or if `self` has at least one named component; return False otherwise.
 
 			Evoked by `bool(mygpath)`
 		"""
 		return self._root or self._dotdot != 0 or len(self._parts) > 0
 
+
 	def __str__(self) -> str:
 		"""
 			Return a string representation of the path that is meaningful to the local operating system.
 
 			Evoked by `str(mygpath)`
 		"""
 		return GPath.separator.join(self.get_parts())
 
+
 	def __repr__(self) -> str:
 		"""
 			Return a string that can be printed as a source code representation of the GPath object.
 
 			Evoked by `repr(mygpath)`
 		"""
 		if bool(self):
 			return f"GPath({repr(str(self))})"
 		else:
 			return f"GPath({repr('')})"
 
+
 	def __len__(self) -> int:
 		"""
 			Get the number of relative path components, excluding any device name or parent directories.
 
 			Evoked by `len(mygpath)`
 		"""
 		return len(self._parts)
 
-	def __getitem__(self, index: int | slice) -> str | list[str]:
+
+	def __getitem__(self, index: Union[int, slice]) -> Union[str, list[str]]:
 		"""
 			Get a 0-indexed relative path component, or a slice of path components, excluding any device name or parent directories.
 
 			Evoked by `mygpath[n]`, `mygpath[start:end]`, `mygpath[start:end:step]`, etc.
 		"""
 		if isinstance(index, int):
 			return self._parts[index]
 		elif isinstance(index, slice):
 			return list(self._parts[index])
 
+
 	def __iter__(self) -> Iterator[str]:
 		"""
 			Get an iterator through the relative path components, excluding any device name or parent directories.
 
 			Evoked by `iter(mygpath)`
 		"""
 		return iter(self._parts)
 
+
 	def __contains__(self, other: GPathLike) -> bool:
 		"""
 			Check if the path represented by `self` contains the path represented by `other`; i.e. check if `self` is a parent directory of `other`.
 
 			Evoked by `other in mygpath`
 
 			Raises `ValueError` if either GPath is invalid
 		"""
 		if not isinstance(other, GPath):
 			other = GPath(other)
 
 		common_path = GPath.find_common(self, other, common_current=True, common_parent=True)
 		return common_path is not None and common_path == self
 
+
 	def __add__(self, other: GPathLike) -> GPath:
 		"""
 			Add (append) `other` to the end of `self` if `other` is a relative path, and return a new copy. If `other` is an absolute path, or if `other` has a different device name, add nothing and return a copy of `self`.
 
 			Evoked by `gpath1 + gpath2`
 
 			Raises `ValueError` if either GPath is invalid
@@ -568,14 +606,15 @@
 				else:
 					pass  # parent of directory of root is still root
 
 			new_parts.extend(other._parts)
 			new_path._parts = tuple(new_parts)
 			return new_path
 
+
 	def __sub__(self, n: int) -> GPath:
 		"""
 			Remove `n` components from the end of the path and return a new copy.
 
 			Evoked by `mygpath - n`
 
 			Raises `ValueError` if `self` is an invalid GPath or if `n` is negative
@@ -591,14 +630,15 @@
 			elif not new_path._root:
 				new_path._dotdot += 1
 			else:
 				pass  # removing components from root should still give root
 		new_path._parts = tuple(new_parts)
 		return new_path
 
+
 	def __mul__(self, n: int) -> GPath:
 		"""
 			Duplicate the relative components of `self` `n` times and return a new path with the duplicated components instead. Named components will be duplicated separately from the components representing a parent directory. If it is an absolute path, only the relative components will be duplicated.
 
 			If `n` is 0, the result should be an empty path (relative or absolute).
 
 			Evoked by `mygpath * n`
@@ -608,14 +648,15 @@
 		if n < 0:
 			raise ValueError("cannot multiply path by a negative integer")
 		new_path = GPath(self)
 		new_path._dotdot = self._dotdot * n
 		new_path._parts = self._parts * n
 		return new_path
 
+
 	def __lshift__(self, n: int) -> GPath:
 		"""
 			Move the imaginary current working directory `n` steps up the filesystem tree. If it is a relative path, remove up to `n` levels of parent directories from the start of the path and return a copy. If it is an absolute path, return a copy of `self` unchanged.
 
 			If `n` is negative, the behaviour of `__rshift__(-n)` will be used instead.
 
 			Evoked by `mygpath << n`
@@ -625,14 +666,15 @@
 		if n < 0:
 			return self.__rshift__(-1 * n)
 		new_path = GPath(self)
 		if not new_path._root:
 			new_path._dotdot = max(new_path._dotdot - n, 0)
 		return new_path
 
+
 	def __rshift__(self, n: int) -> GPath:
 		"""
 			Move the imaginary current working directory `n` steps down the filesystem tree. If it is a relative path, add `n` levels of parent directories to the start of the path and return a copy. If it is an absolute path, return a copy of `self` unchanged.
 
 			If `n` is negative, the behaviour of `__lshift__(-n)` will be used instead.
 
 			Evoked by `mygpath >> n`
@@ -651,8 +693,9 @@
 		if self._dotdot < 0:
 			raise ValueError(f"invalid GPath, dotdot cannot be negative: {repr(self)}")
 		if self._root:
 			if self._dotdot != 0:
 				raise ValueError(f"invalid GPath, dotdot must be 0 when root is True: {repr(self)}")
 		return True
 
-GPathLike = GPath | PathLike
+
+GPathLike = Union[GPath, PathLike]
```

### Comparing `generic-path-0.1/pyproject.toml` & `generic-path-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "generic-path"  # "gpath" is taken on PyPI, and "g-path" is too similar
-dynamic = ["version"]
+dynamic = ["version", "readme"]
 authors = [
 	{name = "Yu Shiyang", email = "yu.shiyang@gnayihs.uy"}
 ]
 description = "GPath provides a robust, generalised abstract file path that provides functions for common path manipulations independent from the local operating system."
-readme = "README.md"
 license = {text = "MPL-2.0"}
 classifiers = [
 	"Development Status :: 3 - Alpha",
 	"Intended Audience :: Developers",
 	"Intended Audience :: System Administrators",
 	"License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3 :: Only",
+	"Programming Language :: Python :: 3.7",
+	"Programming Language :: Python :: 3.8",
+	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
-	"Programming Language :: Python :: 3.12",
+	#"Programming Language :: Python :: 3.12",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 	"Topic :: System :: Filesystems",
 	"Typing :: Typed",
 ]
 keywords = ["python", "filepath", "filesystem", "cross-platform"]
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 dependencies = []
 
 [project.optional-dependencies]
-dev = ["pytest ~= 7.3.1", "coverage ~= 7.2.3", "pyroma ~= 4.2", "build ~= 0.10.0"]
+dev = ["pytest ~= 7.3.1", "coverage ~= 7.2.3", "pyroma ~= 4.2", "build ~= 0.10.0", "tox~=4.5.1"]
 test = ["pytest ~= 7.3.1", "coverage ~= 7.2.3"]
-package = ["pyroma ~= 4.2", "build ~= 0.10.0"]
+config = ["pyroma ~= 4.2"]
+package = ["build ~= 0.10.0"]
+packagetest = ["twine ~= 4.0.2"]
+ci = ["tox~=4.5.1"]
 publish = ["twine ~= 4.0.2"]
 
 [project.urls]
 # key is used verbatim on PyPI
 Homepage = "https://github.com/yushiyangk/GPath"
 Issues = "https://github.com/yushiyangk/GPath/issues"
 
 [tool.pytest.ini_options]
-addopts = "--ignore=Lib"
+addopts = "tests"
+
+[tool.coverage.report]
+include = ["gpath.py"]
 
 [tool.setuptools]
 packages = []
 py-modules = ["gpath"]
 
 [tool.setuptools.dynamic]
 version = {attr = "gpath.__version__"}
+readme = {file = ["README.md", "CHANGELOG.md"], content-type = "text/markdown"}
```

### Comparing `generic-path-0.1/tests/test_gpath.py` & `generic-path-0.2/tests/test_gpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+from __future__ import annotations
+
 import pytest
 
 from gpath import GPath
 
 
+# Type hinting prior to 3.10
+# Using generics in built-in collections, e.g. list[int], is supported from 3.7 by __future__.annotations
+from typing import Optional, Union
+
+
 class TestGPath:
 
 	@pytest.fixture
 	def gpath1(self, request: pytest.FixtureRequest) -> GPath:
 		return GPath(request.param)
 
 	@pytest.fixture
 	def gpath2(self, request: pytest.FixtureRequest) -> GPath:
 		return GPath(request.param)
 
 	@pytest.fixture
-	def expected_gpath(self, request: pytest.FixtureRequest) -> GPath | None:
+	def expected_gpath(self, request: pytest.FixtureRequest) -> Optional[GPath]:
 		if request.param is None:
 			return None
 		else:
 			return GPath(request.param)
 
 
 	@pytest.mark.parametrize(
@@ -39,15 +46,15 @@
 			("/./..", tuple(), "", True, 0),
 			("C:/", tuple(), "C:", True, 0),
 			("C:/.", tuple(), "C:", True, 0),
 			("c:/", tuple(), "c:", True, 0),
 		]
 	)
 	def test_constructor_root(self,
-		path: str | None,
+		path: Optional[str],
 		expected_parts: tuple[str, ...],
 		expected_device: str,
 		expected_root: bool,
 		expected_dotdot: int,
 	):
 		"""
 			Test constructor `__init__()` as well as getters `is_root()`, `get_device()`, `get_parent_parts()`, `get_parent_level()`, but not `get_parts()`, for paths requiring special treatment.
@@ -463,15 +470,15 @@
 			slice(0), slice(1), slice(-1),
 			slice(None, 0), slice(None, 1), slice(None, -1),
 			slice(1, 1), slice(1, 2), slice(1, -1),
 			slice(-2, 1), slice(-2, 2), slice(-2, -1),
 			slice(0, 1, 2), slice(0, 2, 2), slice(0, -1, 2),
 		]
 	)
-	def test_getitem_iter(self, gpath1: GPath, index: int | slice, expected_list: list[str]):
+	def test_getitem_iter(self, gpath1: GPath, index: Union[int, slice], expected_list: list[str]):
 		"""
 			Test `__getitem__()`, for both indexing and slicing, and `__iter__()`.
 		"""
 		try:
 			expected = expected_list[index]
 			result = gpath1[index]
 			assert result == expected
@@ -617,15 +624,15 @@
 			("C:/a/b", "C:/", "a/b", "a/b"),
 			("C:/a/b", "C:/a", "b", "b"),
 			("C:/a/b", "D:/a", None, None),
 			("C:/a/b", "C:/b", None, "../a/b"),
 		],
 		indirect=['gpath1', 'gpath2']
 	)
-	def test_subpath_relpath(self, gpath1: GPath, gpath2: GPath, subpath_expected: str, relpath_expected: str | GPath):
+	def test_subpath_relpath(self, gpath1: GPath, gpath2: GPath, subpath_expected: str, relpath_expected: Union[str, GPath]):
 		"""
 			Test `subpath_from()` and `relpath_from()`.
 		"""
 		if subpath_expected is not None:
 			subpath_expected_gpath = GPath(subpath_expected)
 		else:
 			subpath_expected_gpath = None
```

