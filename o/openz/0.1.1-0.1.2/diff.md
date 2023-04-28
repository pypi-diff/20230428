# Comparing `tmp/openz-0.1.1.tar.gz` & `tmp/openz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openz-0.1.1.tar", max compression
+gzip compressed data, was "openz-0.1.2.tar", max compression
```

## Comparing `openz-0.1.1.tar` & `openz-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-04-27 13:14:20.771065 openz-0.1.1/LICENSE
--rw-r--r--   0        0        0      231 2023-04-27 14:47:34.718102 openz-0.1.1/openz/__init__.py
--rw-r--r--   0        0        0     3980 2023-04-27 15:45:33.710543 openz-0.1.1/openz/_core.py
--rw-r--r--   0        0        0      606 2023-04-27 15:55:36.060885 openz-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      714 2023-04-27 15:50:55.554663 openz-0.1.1/README.md
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 openz-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-27 13:14:20.771065 openz-0.1.2/LICENSE
+-rw-r--r--   0        0        0      231 2023-04-27 14:47:34.718102 openz-0.1.2/openz/__init__.py
+-rw-r--r--   0        0        0     3989 2023-04-28 08:27:44.098554 openz-0.1.2/openz/_core.py
+-rw-r--r--   0        0        0      606 2023-04-28 08:51:50.324834 openz-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      891 2023-04-28 08:51:30.010552 openz-0.1.2/README.md
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 openz-0.1.2/PKG-INFO
```

### Comparing `openz-0.1.1/LICENSE` & `openz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openz-0.1.1/openz/_core.py` & `openz-0.1.2/openz/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     backup_path: Optional[Path] = None
 
     with ExitStack() as open_stack:
 
         parent = Path(path).parent
 
         if with_lockfile:
-            lockfile_path = lockfile_format.format_map(path_dict)
+            lockfile_path = parent / lockfile_format.format_map(path_dict)
             open_stack.enter_context(filelock.FileLock(lockfile_path))
 
         if with_backup and os.path.exists(path):
             backup_path = parent / backup_format.format_map(path_dict)
             with open(path, 'rb') as fp_src:
                 with _atomic_open_for_write(backup_path, parent) as fp_dst:
                     shutil.copyfileobj(fp_src, fp_dst)
```

### Comparing `openz-0.1.1/pyproject.toml` & `openz-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openz"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Cologler <skyoflw@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openz"}]
 homepage = "https://github.com/Cologler/openz-python"
```

### Comparing `openz-0.1.1/README.md` & `openz-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # openz
 
+[![Python Testing](https://github.com/Cologler/openz-python/actions/workflows/testing.yml/badge.svg)](https://github.com/Cologler/openz-python/actions/workflows/testing.yml)
+
 A strange file opener.
 
 ## Usage
 
 ``` python
 from openz import open_for_write, try_rollback
```

### Comparing `openz-0.1.1/PKG-INFO` & `openz-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openz
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/Cologler/openz-python
 License: MIT
 Author: Cologler
 Author-email: skyoflw@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Requires-Dist: filelock (>=3.12.0,<4.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # openz
 
+[![Python Testing](https://github.com/Cologler/openz-python/actions/workflows/testing.yml/badge.svg)](https://github.com/Cologler/openz-python/actions/workflows/testing.yml)
+
 A strange file opener.
 
 ## Usage
 
 ``` python
 from openz import open_for_write, try_rollback
```

