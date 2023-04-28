# Comparing `tmp/monplugin-0.6.0.tar.gz` & `tmp/monplugin-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monplugin-0.6.0.tar", last modified: Fri Apr 21 12:19:40 2023, max compression
+gzip compressed data, was "monplugin-0.6.1.tar", last modified: Fri Apr 28 12:40:21 2023, max compression
```

## Comparing `monplugin-0.6.0.tar` & `monplugin-0.6.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      188 2023-04-05 12:16:51.767308 monplugin-0.6.0/README.md
--rw-r--r--   0        0        0     8542 2023-04-21 12:10:43.505809 monplugin-0.6.0/monplugin/__init__.py
--rw-r--r--   0        0        0      542 2023-04-21 12:18:36.449379 monplugin-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 monplugin-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      188 2023-04-05 12:16:51.767308 monplugin-0.6.1/README.md
+-rw-r--r--   0        0        0     8547 2023-04-28 12:24:24.191457 monplugin-0.6.1/monplugin/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-28 12:29:50.545610 monplugin-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 monplugin-0.6.1/PKG-INFO
```

### Comparing `monplugin-0.6.0/monplugin/__init__.py` & `monplugin-0.6.1/monplugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.range_spec = range_spec
         self.start = None
         self.end = None
         self.outside = True
         self._parse_range()
 
     def __str__(self):
-        return self.range_spec or ""
+        return str(self.range_spec or "")
 
     def __repr__(self):
         return f'Range({self.range_spec})'
 
     def is_set(self):
         return self.range_spec is not None
```

### Comparing `monplugin-0.6.0/pyproject.toml` & `monplugin-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "monplugin"
 readme = "README.md"
 description = "Partial python port of perls Monitoring::Plugin"
-version = "0.6.0"
+version = "0.6.1"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
```

### Comparing `monplugin-0.6.0/PKG-INFO` & `monplugin-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monplugin
-Version: 0.6.0
+Version: 0.6.1
 Summary: Partial python port of perls Monitoring::Plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

