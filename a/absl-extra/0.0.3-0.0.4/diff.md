# Comparing `tmp/absl_extra-0.0.3.tar.gz` & `tmp/absl_extra-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.3.tar", last modified: Thu Apr 27 21:47:47 2023, max compression
+gzip compressed data, was "absl_extra-0.0.4.tar", last modified: Fri Apr 28 18:05:13 2023, max compression
```

## Comparing `absl_extra-0.0.3.tar` & `absl_extra-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1271 2023-04-27 21:47:38.824325 absl_extra-0.0.3/Readme.md
--rw-r--r--   0        0        0     4741 2023-04-27 21:47:38.824325 absl_extra-0.0.3/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-27 21:47:38.824325 absl_extra-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 absl_extra-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1266 2023-04-28 18:05:05.808629 absl_extra-0.0.4/Readme.md
+-rw-r--r--   0        0        0     5463 2023-04-28 18:05:05.808629 absl_extra-0.0.4/absl_extra.py
+-rw-r--r--   0        0        0     6066 2023-04-28 18:05:05.808629 absl_extra-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 absl_extra-0.0.4/PKG-INFO
```

### Comparing `absl_extra-0.0.3/Readme.md` & `absl_extra-0.0.4/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,13 +29,12 @@
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
         slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    pass
+def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
 
 if __name__ == "__main__":
     app.run(main)
 ```
```

### Comparing `absl_extra-0.0.3/absl_extra.py` & `absl_extra-0.0.4/absl_extra.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 from importlib import util
 from typing import Callable, NamedTuple
 from functools import partial, wraps
 from absl import app, flags, logging
+import inspect
 
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
 else:
     logging.warning("pymongo not installed.")
 
@@ -152,7 +153,30 @@
         logging.info("-" * 50)
 
         notifier.notify_job_started(app_name)
         app.run(partial(main, **kwargs))
         notifier.notify_job_finished(app_name)
 
     return wrapper
+
+
+def log_before(func, logger=logging.debug):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
+        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
+        logger(
+            f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
+        )
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def log_after(func, logger=logging.debug):
+    @wraps(func)
+    def wrapper(*func_args, **func_kwargs):
+        retval = func(*func_args, **func_kwargs)
+        logger("Exited " + func.__name__ + "() with value: " + repr(retval))
+        return retval
+
+    return wrapper
```

### Comparing `absl_extra-0.0.3/pyproject.toml` & `absl_extra-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "absl_extra"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.3"  # Required
+version = "0.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A wrapper to run and monitor absl app."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `absl_extra-0.0.3/PKG-INFO` & `absl_extra-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper to run and monitor absl app.
 Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -51,14 +51,13 @@
     mongo_config=MongoConfig(
         uri=os.environ["MONGO_URI"], db_name="my_project", collection="experiment_1"
     ),
     notifier=SlackNotifier(
         slack_token=os.environ["SLACK_TOKEN"], channel_id=os.environ["CHANNEL_ID"]
     ),
 )
-def main(cmd: str, config: ConfigDict, db: Collection) -> None:
-    pass
+def main(cmd: str, config: ConfigDict, db: Collection) -> None: ...
 
 if __name__ == "__main__":
     app.run(main)
 ```
```

