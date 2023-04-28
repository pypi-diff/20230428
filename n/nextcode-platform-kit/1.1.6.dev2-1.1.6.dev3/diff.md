# Comparing `tmp/nextcode-platform-kit-1.1.6.dev2.tar.gz` & `tmp/nextcode-platform-kit-1.1.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode-platform-kit-1.1.6.dev2.tar", last modified: Wed Apr 26 17:11:39 2023, max compression
+gzip compressed data, was "nextcode-platform-kit-1.1.6.dev3.tar", last modified: Fri Apr 28 11:39:25 2023, max compression
```

## Comparing `nextcode-platform-kit-1.1.6.dev2.tar` & `nextcode-platform-kit-1.1.6.dev3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.491736 nextcode-platform-kit-1.1.6.dev2/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 17:11:39.491736 nextcode-platform-kit-1.1.6.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.484735 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 17:11:38.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.488735 nextcode-platform-kit-1.1.6.dev2/platkit/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-26 17:11:39.000000 nextcode-platform-kit-1.1.6.dev2/platkit/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/csautils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.489735 nextcode-platform-kit-1.1.6.dev2/platkit/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/endpoints/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8561 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/flasksetup.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/librarypatches.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/logsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.490735 nextcode-platform-kit-1.1.6.dev2/platkit/middleware/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/middleware/logstash_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/middleware/reverse_proxied.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:11:39.491736 nextcode-platform-kit-1.1.6.dev2/platkit/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/models/responses.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/testcase.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/platkit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 17:11:39.491736 nextcode-platform-kit-1.1.6.dev2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-26 17:11:04.000000 nextcode-platform-kit-1.1.6.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.782731 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:39:24.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.786399 nextcode-platform-kit-1.1.6.dev3/platkit/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-28 11:39:25.000000 nextcode-platform-kit-1.1.6.dev3/platkit/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/csautils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.787315 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8609 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/flasksetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2708 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/librarypatches.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/logsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.788232 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/logstash_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/middleware/reverse_proxied.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:39:25.788232 nextcode-platform-kit-1.1.6.dev3/platkit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/models/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/testcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/platkit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 11:39:25.789149 nextcode-platform-kit-1.1.6.dev3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 11:38:48.000000 nextcode-platform-kit-1.1.6.dev3/setup.py
```

### Comparing `nextcode-platform-kit-1.1.6.dev2/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev2
+Version: 1.1.6.dev3
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev2/README.md` & `nextcode-platform-kit-1.1.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/PKG-INFO` & `nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev2
+Version: 1.1.6.dev3
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev2/nextcode_platform_kit.egg-info/SOURCES.txt` & `nextcode-platform-kit-1.1.6.dev3/nextcode_platform_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/auth.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/cli.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/cli.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/config.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/config.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/csautils.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/csautils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/endpoints/auth.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/flasksetup.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/flasksetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 """
 
 from http import HTTPStatus
 import logging
 import time
 
 from flask import request, current_app, make_response, jsonify, Blueprint
-from flask_restx import abort, Model, Api
+from flask_restx import abort, Model
 from flask_httpauth import HTTPTokenAuth
 from werkzeug.utils import find_modules, import_string
 from werkzeug.exceptions import HTTPException
 from werkzeug.middleware.proxy_fix import ProxyFix
 from flask import Flask
 
 import sentry_sdk
 from sentry_sdk.integrations.flask import FlaskIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 from sentry_sdk.integrations.sqlalchemy import SqlalchemyIntegration
+from platkit.librarypatches import PatchedApi as Api
 from platkit.exceptions import InvalidUsage
 from platkit.utils import CustomJSONProvider
 from platkit import logsetup
 from platkit.config import Config
 from platkit.middleware.reverse_proxied import ReverseProxied
 from platkit.prometheus import metrics
 from platkit.cli import setup_commands
```

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/librarypatches.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/librarypatches.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,63 @@
 #!/usr/bin/env python
 """
 Patching 3rd party libraries
 """
 
 import re
 import os
+import warnings
+
 from flask import make_response
 from flask.json import dumps
 import flask_restx
 
 
+
+# monkeypatch the Api class to remove hard-coded '/' rules so that we can put something that
+# is not swagger into the root. Hopefully this will be solved in flask_restx at some point
+# https://github.com/noirbizarre/flask-restx/issues/247
+class PatchedApi(flask_restx.Api):
+    def _register_doc(self, app_or_blueprint):
+        if self._add_specs and self._doc:
+            app_or_blueprint.add_url_rule(self._doc, "doc", self.render_doc)
+
+    # @property
+    # def base_path(self):
+    #     return ""
+
+
 # Remove Flask restx exception handlers so that we can use our own
 # Otherwise we cannot have custom structured error messages from the Api
 def patched_init_app(self, app):
-    self._register_specs(self.blueprint or app)
-    self._register_doc(self.blueprint or app)
-
     if len(self.resources) > 0:
-        for resource, urls, kwargs in self.resources:
-            self._register_view(app, resource, *urls, **kwargs)
+        for resource, namespace, urls, kwargs in self.resources:
+            self._register_view(app, resource, namespace, *urls, **kwargs)
+
+    for ns in self.namespaces:
+        self._configure_namespace_logger(app, ns)
 
     self._register_apidoc(app)
     self._validate = (
-        self._validate if self._validate is not None else app.config.get("RESTX_VALIDATE", False)
+        self._validate
+        if self._validate is not None
+        else app.config.get("RESTX_VALIDATE", False)
     )
     app.config.setdefault("RESTX_MASK_HEADER", "X-Fields")
     app.config.setdefault("RESTX_MASK_SWAGGER", True)
     app.config.setdefault("RESTX_INCLUDE_ALL_MODELS", False)
 
+    # check for deprecated config variable names
+    if "ERROR_404_HELP" in app.config:
+        app.config["RESTX_ERROR_404_HELP"] = app.config["ERROR_404_HELP"]
+        warnings.warn(
+            "'ERROR_404_HELP' config setting is deprecated and will be "
+            "removed in the future. Use 'RESTX_ERROR_404_HELP' instead.",
+            DeprecationWarning,
+        )
 
 flask_restx.Api._init_app = patched_init_app
 
 
 # Install proper json dumper for Flask restx library.
 # This is needed because we need to use Flask's JSON converter which can
 # handle more variety of Python types than the standard converter.
```

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/logsetup.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/logsetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/middleware/logstash_formatter.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/middleware/logstash_formatter.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/middleware/reverse_proxied.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/middleware/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/models/responses.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/models/responses.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/testcase.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/testcase.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/platkit/utils.py` & `nextcode-platform-kit-1.1.6.dev3/platkit/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev2/setup.py` & `nextcode-platform-kit-1.1.6.dev3/setup.py`

 * *Files identical despite different names*

