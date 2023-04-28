# Comparing `tmp/pytest_ruff-0.0.5.tar.gz` & `tmp/pytest_ruff-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ruff-0.0.5.tar", max compression
+gzip compressed data, was "pytest_ruff-0.0.6.tar", max compression
```

## Comparing `pytest_ruff-0.0.5.tar` & `pytest_ruff-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1062 2023-03-22 11:48:45.974373 pytest_ruff-0.0.5/LICENSE
--rw-r--r--   0        0        0      542 2023-03-22 11:48:45.974373 pytest_ruff-0.0.5/README.md
--rw-r--r--   0        0        0      988 2023-03-22 11:49:24.470647 pytest_ruff-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-03-22 11:48:45.974373 pytest_ruff-0.0.5/pytest_ruff.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 pytest_ruff-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/LICENSE
+-rw-r--r--   0        0        0      542 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/README.md
+-rw-r--r--   0        0        0     1012 2023-04-28 11:43:13.781378 pytest_ruff-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/pytest_ruff.py
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 pytest_ruff-0.0.6/PKG-INFO
```

### Comparing `pytest_ruff-0.0.5/LICENSE` & `pytest_ruff-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.0.5/README.md` & `pytest_ruff-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.0.5/pyproject.toml` & `pytest_ruff-0.0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-ruff"
-version = "0.0.5"
+version = "0.0.6"
 description = "pytest plugin to check ruff requirements."
 authors = ["Iuri de Silvio <iurisilvio@gmail.com>"]
 readme = "README.md"
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "Operating System :: OS Independent", "Framework :: Pytest", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 :: Only", "Topic :: Software Development :: Libraries :: Python Modules"]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/buserbrasil/pytest-ruff"
@@ -15,14 +15,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ruff = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
+pytest-mock = "^3.10.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.pytest.ini_options]
 addopts = "--capture=no"
```

### Comparing `pytest_ruff-0.0.5/pytest_ruff.py` & `pytest_ruff-0.0.6/pytest_ruff.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,15 @@
     config = parent.config
     if not config.option.ruff:
         return
 
     if file_path.suffix != ".py":
         return
 
-    item = RuffFile.from_parent(parent, path=file_path)
-    return item
+    return RuffFile.from_parent(parent, path=file_path)
 
 
 def pytest_unconfigure(config):
     if hasattr(config, "_ruffmtimes"):
         cache = config.cache.get(HISTKEY, {})
         cache.update(config._ruffmtimes)
         config.cache.set(HISTKEY, cache)
@@ -59,23 +58,18 @@
             pytest.skip("file previously passed ruff checks")
 
     def runtest(self):
         check_file(self.fspath)
         if hasattr(self.config, "_ruffmtimes"):
             self.config._ruffmtimes[str(self.fspath)] = self._ruffmtime
 
-    def repr_failure(self, excinfo):
-        if excinfo.errisinstance(RuffError):
-            return excinfo.value.args[0].decode()
-        return super().repr_failure(excinfo)
-
     def reportinfo(self):
         return (self.fspath, None, "")
 
 
 def check_file(path):
     ruff = find_ruff_bin()
-    command = f"{ruff} {path} --quiet"
+    command = f"{ruff} {path} --quiet --show-source"
     child = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
-    stdout, stderr = child.communicate()
+    stdout, _ = child.communicate()
     if stdout:
-        raise RuffError(stdout, stderr)
+        raise RuffError(stdout.decode())
```

### Comparing `pytest_ruff-0.0.5/PKG-INFO` & `pytest_ruff-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ruff
-Version: 0.0.5
+Version: 0.0.6
 Summary: pytest plugin to check ruff requirements.
 Author: Iuri de Silvio
 Author-email: iurisilvio@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

