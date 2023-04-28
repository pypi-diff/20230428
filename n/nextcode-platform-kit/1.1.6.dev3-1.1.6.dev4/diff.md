# Comparing `tmp/nextcode-platform-kit-1.1.6.dev3.tar.gz` & `tmp/nextcode-platform-kit-1.1.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode-platform-kit-1.1.6.dev3.tar", last modified: Fri Apr 28 11:39:25 2023, max compression
+gzip compressed data, was "nextcode-platform-kit-1.1.6.dev4.tar", last modified: Fri Apr 28 14:18:12 2023, max compression
```

## Comparing `nextcode-platform-kit-1.1.6.dev3.tar` & `nextcode-platform-kit-1.1.6.dev4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.782731 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:39:24.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.786399 nextcode-platform-kit-1.1.6.dev3/platkit/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/platkit/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/csautils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.787315 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8609 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/flasksetup.py
--rw-rw-rw-   0 root         (0) root         (0)     2708 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/librarypatches.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/logsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.788232 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/logstash_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/reverse_proxied.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.788232 nextcode-platform-kit-1.1.6.dev3/platkit/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/models/responses.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/testcase.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.053300 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.058301 nextcode-platform-kit-1.1.6.dev4/platkit/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/platkit/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/csautils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.058301 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8609 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/flasksetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/librarypatches.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/logsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.059301 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/logstash_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/reverse_proxied.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.060301 nextcode-platform-kit-1.1.6.dev4/platkit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/models/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/testcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/setup.py
```

### Comparing `nextcode-platform-kit-1.1.6.dev3/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev3
+Version: 1.1.6.dev4
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev3/README.md` & `nextcode-platform-kit-1.1.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev3
+Version: 1.1.6.dev4
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/SOURCES.txt` & `nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/auth.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/cli.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/cli.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/config.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/config.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/csautils.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/csautils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/auth.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/flasksetup.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/flasksetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/librarypatches.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/librarypatches.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # is not swagger into the root. Hopefully this will be solved in flask_restx at some point
 # https://github.com/noirbizarre/flask-restx/issues/247
 class PatchedApi(flask_restx.Api):
     def _register_doc(self, app_or_blueprint):
         if self._add_specs and self._doc:
             app_or_blueprint.add_url_rule(self._doc, "doc", self.render_doc)
 
-    # @property
-    # def base_path(self):
-    #     return ""
+    @property
+    def base_path(self):
+        return ""
 
 
 # Remove Flask restx exception handlers so that we can use our own
 # Otherwise we cannot have custom structured error messages from the Api
 def patched_init_app(self, app):
     if len(self.resources) > 0:
         for resource, namespace, urls, kwargs in self.resources:
```

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/logsetup.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/logsetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/middleware/logstash_formatter.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/middleware/logstash_formatter.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/middleware/reverse_proxied.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/middleware/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/models/responses.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/models/responses.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/testcase.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/testcase.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/platkit/utils.py` & `nextcode-platform-kit-1.1.6.dev4/platkit/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev3/setup.py` & `nextcode-platform-kit-1.1.6.dev4/setup.py`

 * *Files identical despite different names*

