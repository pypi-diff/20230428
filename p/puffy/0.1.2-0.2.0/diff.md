# Comparing `tmp/puffy-0.1.2.tar.gz` & `tmp/puffy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puffy-0.1.2.tar", last modified: Mon Feb 27 03:08:16 2023, max compression
+gzip compressed data, was "puffy-0.2.0.tar", last modified: Fri Apr 28 06:39:40 2023, max compression
```

## Comparing `puffy-0.1.2.tar` & `puffy-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.052859 puffy-0.1.2/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.1.2/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11717 2023-02-27 03:08:16.052937 puffy-0.1.2/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11224 2023-02-27 03:07:35.000000 puffy-0.1.2/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.1.2/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-02-27 03:08:16.053449 puffy-0.1.2/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.050431 puffy-0.1.2/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.051527 puffy-0.1.2/src/puffy/
--rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.1.2/src/puffy/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.052367 puffy-0.1.2/src/puffy/error/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     3985 2023-02-26 14:33:33.000000 puffy-0.1.2/src/puffy/error/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.052645 puffy-0.1.2/src/puffy/object/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.1.2/src/puffy/object/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-02-27 03:08:16.052178 puffy-0.1.2/src/puffy.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)    11717 2023-02-27 03:08:16.000000 puffy-0.1.2/src/puffy.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      285 2023-02-27 03:08:16.000000 puffy-0.1.2/src/puffy.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-02-27 03:08:16.000000 puffy-0.1.2/src/puffy.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-02-27 03:08:16.000000 puffy-0.1.2/src/puffy.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-02-27 03:08:16.000000 puffy-0.1.2/src/puffy.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730876 puffy-0.2.0/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.2.0/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    13398 2023-04-28 06:39:40.731015 puffy-0.2.0/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    12905 2023-04-28 06:38:18.000000 puffy-0.2.0/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.2.0/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-04-28 06:39:40.731751 puffy-0.2.0/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.728752 puffy-0.2.0/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.729892 puffy-0.2.0/src/puffy/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.2.0/src/puffy/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730645 puffy-0.2.0/src/puffy/error/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.2.0/src/puffy/error/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730771 puffy-0.2.0/src/puffy/object/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.2.0/src/puffy/object/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-04-28 06:39:40.730513 puffy-0.2.0/src/puffy.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    13398 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      285 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-04-28 06:39:40.000000 puffy-0.2.0/src/puffy.egg-info/top_level.txt
```

### Comparing `puffy-0.1.2/LICENSE` & `puffy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puffy-0.1.2/PKG-INFO` & `puffy-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-Metadata-Version: 2.1
-Name: puffy
-Version: 0.1.2
-Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
-Home-page: https://github.com/nicolasdao/pypuffy
-Author: Nicolas Dao
-Author-email: nicolas.dao@gmail.com
-License: BSD-3-Clause
-Keywords: util
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PUFFY
 
 A collection of modules with zero-dependencies to help manage common programming tasks.
 
 ```
 pip install puffy
 ```
 
 Usage examples:
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -44,16 +28,17 @@
 obj.s('address.line1', 'Magic street') # Sets obj.address.line1 to 'Magic street' and return 'Magic street'
 ```
 
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
->		- [Basic `error` APIs](#basic-error-apis)
+>		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
+>		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
@@ -67,18 +52,18 @@
 # APIs
 ## `error`
 
 The `error` module exposes the following APIs:
 - `catch_errors`: A higher-order function that returns a function that always return a tuple `(error, response)`. If the `error` is `None`, then the function did not fail. Otherwise, it did and the `error` object can be used to build an error stack.
 - `StackedException`: A class that inherits from `Exception`. Use it to stack errors.
 
-### Basic `error` APIs
+### Basic `error` APIs - Getting in control of your errors
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -140,14 +125,46 @@
 # error: Failed again
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail_again
 #     raise Exception("Failed")
 ```
 
+### Managing errors in `async/await` corountines
+
+```python
+from puffy.error import async_catch_errors
+import asyncio
+
+# This function will never fail. Instead, the error is safely caught.
+@async_catch_errors
+async def fail():
+    await asyncio.sleep(0.01)
+    raise Exception("Failed")
+    return "yes"
+
+loop = asyncio.get_event_loop()
+err, resp = loop.run_until_complete(fail())
+
+print(resp) # None
+print(type(err)) # <class 'src.puffy.error.StackedException'> which inherits from Exception
+print(str(err)) # Failed
+print(len(err.stack)) # 1
+print(str(err.stack[0])) # Failed
+print(err.stack[0].__traceback__) # <traceback object at 0x7fc69066bf00>
+
+# Use the `strinfigy` method to extract the full error stack details.
+print(err.strinfigy()) 
+# error: Failed
+#   File "blablabla.py", line 72, in safe_exec
+#     data = ffn(*args, **named_args)
+#   File "blablabla.py", line 28, in fail
+#     raise Exception("Failed")
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -172,15 +189,16 @@
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
-| `make t` | Formats adnd then lints the project. |
+| `make t` | Formats, lints and then unit tests the project. |
+| `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 
 ## Install dependencies with `easypipinstall`
 
 `easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
@@ -272,15 +290,17 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, `make bp` builds and publishes your package to https://pypi.org.
+> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
+
+__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To build your package, run:
 
 ```
 make b
 ```
 
@@ -301,14 +321,16 @@
 
 Those two steps have been bundled in a single command:
 
 ```
 make bp
 ```
 
+> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
+
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
 ```
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
```

### Comparing `puffy-0.1.2/README.md` & `puffy-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,35 @@
+Metadata-Version: 2.1
+Name: puffy
+Version: 0.2.0
+Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
+Home-page: https://github.com/nicolasdao/pypuffy
+Author: Nicolas Dao
+Author-email: nicolas.dao@gmail.com
+License: BSD-3-Clause
+Keywords: util
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PUFFY
 
 A collection of modules with zero-dependencies to help manage common programming tasks.
 
 ```
 pip install puffy
 ```
 
 Usage examples:
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -28,16 +44,17 @@
 obj.s('address.line1', 'Magic street') # Sets obj.address.line1 to 'Magic street' and return 'Magic street'
 ```
 
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
->		- [Basic `error` APIs](#basic-error-apis)
+>		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
+>		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
@@ -51,18 +68,18 @@
 # APIs
 ## `error`
 
 The `error` module exposes the following APIs:
 - `catch_errors`: A higher-order function that returns a function that always return a tuple `(error, response)`. If the `error` is `None`, then the function did not fail. Otherwise, it did and the `error` object can be used to build an error stack.
 - `StackedException`: A class that inherits from `Exception`. Use it to stack errors.
 
-### Basic `error` APIs
+### Basic `error` APIs - Getting in control of your errors
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -124,14 +141,46 @@
 # error: Failed again
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail_again
 #     raise Exception("Failed")
 ```
 
+### Managing errors in `async/await` corountines
+
+```python
+from puffy.error import async_catch_errors
+import asyncio
+
+# This function will never fail. Instead, the error is safely caught.
+@async_catch_errors
+async def fail():
+    await asyncio.sleep(0.01)
+    raise Exception("Failed")
+    return "yes"
+
+loop = asyncio.get_event_loop()
+err, resp = loop.run_until_complete(fail())
+
+print(resp) # None
+print(type(err)) # <class 'src.puffy.error.StackedException'> which inherits from Exception
+print(str(err)) # Failed
+print(len(err.stack)) # 1
+print(str(err.stack[0])) # Failed
+print(err.stack[0].__traceback__) # <traceback object at 0x7fc69066bf00>
+
+# Use the `strinfigy` method to extract the full error stack details.
+print(err.strinfigy()) 
+# error: Failed
+#   File "blablabla.py", line 72, in safe_exec
+#     data = ffn(*args, **named_args)
+#   File "blablabla.py", line 28, in fail
+#     raise Exception("Failed")
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -156,15 +205,16 @@
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
-| `make t` | Formats adnd then lints the project. |
+| `make t` | Formats, lints and then unit tests the project. |
+| `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 
 ## Install dependencies with `easypipinstall`
 
 `easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
@@ -256,15 +306,17 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, `make bp` builds and publishes your package to https://pypi.org.
+> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
+
+__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To build your package, run:
 
 ```
 make b
 ```
 
@@ -285,14 +337,16 @@
 
 Those two steps have been bundled in a single command:
 
 ```
 make bp
 ```
 
+> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
+
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
 ```
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
```

### Comparing `puffy-0.1.2/setup.cfg` & `puffy-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = puffy
-version = 0.1.2
+version = 0.2.0
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = A collection of modules with zero-dependencies to help manage common programming tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/pypuffy
 readme = README.md
```

### Comparing `puffy-0.1.2/src/puffy/error/__init__.py` & `puffy-0.2.0/src/puffy/error/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,18 +72,25 @@
             return ""
 
 
 def catch_errors(arg):
     if not arg:
         raise Exception("Missing required argument.")
 
+    isAsyncFunction = inspect.iscoroutinefunction(arg)
+    isSyncFunction = callable(arg)
+    if isAsyncFunction:
+        raise Exception(
+            "Invalid argument exception. 'catch_errors' does not accept coroutines (i.e., async/await functions). Use 'async_catch_errors' instead."
+        )
+
     fn = None
     wrappingError = None
 
-    if callable(arg):
+    if isSyncFunction:
         fn = arg
     elif isinstance(arg, str):
         wrappingError = Exception(arg)
     else:
         raise Exception(
             f'Wrong argument exception. "catch_errors"\'s argument must be a function or a string. Found {type(arg).__name__} instead.'
         )
@@ -112,7 +119,59 @@
                     else StackedException(name, error),
                     None,
                 ]
 
         return safe_exec
 
     return safe_fn_exec(fn) if fn else safe_fn_exec
+
+
+def async_catch_errors(arg):
+    if not arg:
+        raise Exception("Missing required argument.")
+    isAsyncFunction = inspect.iscoroutinefunction(arg)
+    isSyncFunction = callable(arg) and not isAsyncFunction
+    if isSyncFunction:
+        raise Exception(
+            "Invalid argument exception. 'async_catch_errors' does not accept synchronous functions. Use 'catch_errors' instead."
+        )
+
+    afn = None
+    wrappingError = None
+
+    if isAsyncFunction:
+        afn = arg
+    elif isinstance(arg, str):
+        wrappingError = Exception(arg)
+    else:
+        raise Exception(
+            f'Wrong argument exception. "catch_errors"\'s argument must be a function or a string. Found {type(arg).__name__} instead.'
+        )
+
+    def safe_fn_exec(ffn):
+        async def async_safe_exec(*args, **named_args):
+            fn_name = fn_file = fn_line = None
+            try:
+                try:
+                    fn_name = ffn.__name__
+                    fn_file = inspect.getfile(ffn)
+                    try:
+                        lines = inspect.getsourcelines(ffn)
+                        fn_line = lines[1] if lines and len(lines) >= 2 else 0
+                    except:
+                        fn_line = ""
+                except:
+                    fn_name = fn_file = fn_line = ""
+                data = await ffn(*args, **named_args)
+                return [None, data]
+            except BaseException as error:
+                name = _WrappedFunction(fn_name, fn_file, fn_line)
+                return [
+                    StackedException(name, wrappingError, error)
+                    if wrappingError
+                    else StackedException(name, error),
+                    None,
+                ]
+
+        return async_safe_exec
+
+    return safe_fn_exec(afn) if afn else safe_fn_exec
```

### Comparing `puffy-0.1.2/src/puffy/object/__init__.py` & `puffy-0.2.0/src/puffy/object/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.1.2/src/puffy.egg-info/PKG-INFO` & `puffy-0.2.0/src/puffy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 ```
 pip install puffy
 ```
 
 Usage examples:
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -44,16 +44,17 @@
 obj.s('address.line1', 'Magic street') # Sets obj.address.line1 to 'Magic street' and return 'Magic street'
 ```
 
 # Table of contents
 
 > * [APIs](#apis)
 >	- [`error`](#error)
->		- [Basic `error` APIs](#basic-error-apis)
+>		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
+>		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
 >		- [Ignoring `flake8` errors](#ignoring-flake8-errors)
@@ -67,18 +68,18 @@
 # APIs
 ## `error`
 
 The `error` module exposes the following APIs:
 - `catch_errors`: A higher-order function that returns a function that always return a tuple `(error, response)`. If the `error` is `None`, then the function did not fail. Otherwise, it did and the `error` object can be used to build an error stack.
 - `StackedException`: A class that inherits from `Exception`. Use it to stack errors.
 
-### Basic `error` APIs
+### Basic `error` APIs - Getting in control of your errors
 
 ```python
-from puffy.error import catch_errors, StackedException
+from puffy.error import catch_errors
 
 # This function will never fail. Instead, the error is safely caught.
 @catch_errors
 def fail():
     raise Exception("Failed")
     return "yes"
 
@@ -140,14 +141,46 @@
 # error: Failed again
 #   File "blablabla.py", line 72, in safe_exec
 #     data = ffn(*args, **named_args)
 #   File "blablabla.py", line 28, in fail_again
 #     raise Exception("Failed")
 ```
 
+### Managing errors in `async/await` corountines
+
+```python
+from puffy.error import async_catch_errors
+import asyncio
+
+# This function will never fail. Instead, the error is safely caught.
+@async_catch_errors
+async def fail():
+    await asyncio.sleep(0.01)
+    raise Exception("Failed")
+    return "yes"
+
+loop = asyncio.get_event_loop()
+err, resp = loop.run_until_complete(fail())
+
+print(resp) # None
+print(type(err)) # <class 'src.puffy.error.StackedException'> which inherits from Exception
+print(str(err)) # Failed
+print(len(err.stack)) # 1
+print(str(err.stack[0])) # Failed
+print(err.stack[0].__traceback__) # <traceback object at 0x7fc69066bf00>
+
+# Use the `strinfigy` method to extract the full error stack details.
+print(err.strinfigy()) 
+# error: Failed
+#   File "blablabla.py", line 72, in safe_exec
+#     data = ffn(*args, **named_args)
+#   File "blablabla.py", line 28, in fail
+#     raise Exception("Failed")
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
@@ -172,15 +205,16 @@
 | `make b` | Builds the package. |
 | `make p` | Publish the package to https://pypi.org. |
 | `make bp` | Builds the package and then publish it to https://pypi.org. |
 | `make bi` | Builds the package and install it locally (`pip install -e .`). |
 | `make install` | Install the dependencies defined in the `requirements.txt`. This file contains all the dependencies (i.e., both prod and dev). |
 | `make install-prod` | Install the dependencies defined in the `prod-requirements.txt`. This file only contains the production dependencies. |
 | `make n` | Starts a Jupyter notebook for this project. |
-| `make t` | Formats adnd then lints the project. |
+| `make t` | Formats, lints and then unit tests the project. |
+| `make t testpath=<FULLY QUALIFIED TEST PATH>` | Foccuses the unit test on a specific test. For a concrete example, please refer to the [Executing a specific test only](#executing-a-specific-test-only) section. |
 | `easyi numpy` | Instals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 | `easyi flake8 -D` | Instals `flake8` and update `setup.cfg` and `requirements.txt`. |
 | `easyu numpy` | Uninstals `numpy` and update `setup.cfg`, `prod-requirements.txt` and `requirements.txt`. |
 
 ## Install dependencies with `easypipinstall`
 
 `easypipinstall` adds two new CLI utilities: `easyi` (install) and `easyu` (uninstall).
@@ -272,15 +306,17 @@
 
 ```
 make t testpath=tests/error/test_catch_errors.py::test_catch_errors_StackedException_arbitrary_inputs
 ```
 
 ## Building and distributing this package
 
-> Tl;dr, `make bp` builds and publishes your package to https://pypi.org.
+> Tl;dr, Update the version in the `setup.cfg` file, and then run `make bp` to build and publish your package to https://pypi.org.
+
+__IMPORTANT:__ First, make sure you've updated the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
 
 To build your package, run:
 
 ```
 make b
 ```
 
@@ -301,14 +337,16 @@
 
 Those two steps have been bundled in a single command:
 
 ```
 make bp
 ```
 
+> __IMPORTANT:__ Don't forget to update the version in the the `setup.cfg` file. Ideally, you should also tag your git repository `git tag vx.x.x`.
+
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
 
 ```
 make bi
 ```
 
 This command buils the package and follows with `pip install -e .`.
```

