# Comparing `tmp/grizzly-loadtester-cli-3.1.6.tar.gz` & `tmp/grizzly-loadtester-cli-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-cli-3.1.6.tar", last modified: Mon Apr 17 05:45:01 2023, max compression
+gzip compressed data, was "grizzly-loadtester-cli-3.1.7.tar", last modified: Fri Apr 28 09:16:56 2023, max compression
```

## Comparing `grizzly-loadtester-cli-3.1.6.tar` & `grizzly-loadtester-cli-3.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.378837 grizzly-loadtester-cli-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/static/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/grizzly_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 05:45:01.000000 grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:45:01.374837 grizzly-loadtester-cli-3.1.6/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/script/docs-generate-licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:45:01.378837 grizzly-loadtester-cli-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 05:44:36.000000 grizzly-loadtester-cli-3.1.6/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.223992 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/bashcompletion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/static/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27696 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/grizzly_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 09:16:56.000000 grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-28 09:16:32.000000 grizzly-loadtester-cli-3.1.7/script/docs-generate-licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:16:56.227992 grizzly-loadtester-cli-3.1.7/setup.cfg
```

### Comparing `grizzly-loadtester-cli-3.1.6/LICENSE.md` & `grizzly-loadtester-cli-3.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/PKG-INFO` & `grizzly-loadtester-cli-3.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.6
+Version: 3.1.7
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
@@ -19,8 +19,10 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ci
 License-File: LICENSE.md
 
 # Grizzly Command Line Interface
 
-Documentation in [`biometria-se/grizzly`](https://biometria-se.github.io/grizzly/command-line-interface/usage/).
+Documentation can be found [here](https://biometria-se.github.io/grizzly/command-line-interface/usage/).
+
+Issues should be reported in [`biometria-se/grizzly/issues`](https://github.com/Biometria-se/grizzly/issues).
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/__init__.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/__main__.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/__init__.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/__init__.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/bashcompletion.bash` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/bashcompletion.bash`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/bashcompletion/types.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/bashcompletion/types.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/argparse/markdown.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/argparse/markdown.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/__init__.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     if mtu is None and os.environ.get('GRIZZLY_MTU', None) is None:
         print('!! unable to determine MTU, try manually setting GRIZZLY_MTU environment variable if anything other than 1500 is needed')
         mtu = '1500'
 
     columns, lines = get_terminal_size()
 
-    # set environment variables needed by compose files, when *-compose executes
+    # set environment variables needed by compose files, when * compose executes
     os.environ['GRIZZLY_MTU'] = cast(str, mtu)
     os.environ['GRIZZLY_EXECUTION_CONTEXT'] = EXECUTION_CONTEXT
     os.environ['GRIZZLY_STATIC_CONTEXT'] = STATIC_CONTEXT
     os.environ['GRIZZLY_MOUNT_CONTEXT'] = MOUNT_CONTEXT
     os.environ['GRIZZLY_PROJECT_NAME'] = project_name
     os.environ['GRIZZLY_USER_TAG'] = tag
     os.environ['GRIZZLY_EXPECTED_WORKERS'] = str(args.workers)
@@ -253,15 +253,15 @@
         fd.flush()
 
         os.environ['GRIZZLY_ENVIRONMENT_FILE'] = fd.name
 
         validate_config = getattr(args, 'validate_config', False)
 
         compose_command = [
-            f'{args.container_system}-compose',
+            args.container_system, 'compose',
             *compose_args,
             'config',
         ]
 
         rc = run_command(compose_command, silent=not validate_config)
 
         if validate_config or rc != 0:
@@ -279,15 +279,15 @@
                 print(f'!! failed to build {project_name}, rc={rc}')
                 return rc
 
         compose_scale_argument = ['--scale', f'worker={args.workers}']
 
         # bring up containers
         compose_command = [
-            f'{args.container_system}-compose',
+            args.container_system, 'compose',
             *compose_args,
             'up',
             *compose_scale_argument,
             '--remove-orphans',
         ]
 
         rc = run_command(compose_command, verbose=args.verbose)
@@ -311,15 +311,15 @@
             )
             rc = int(output.strip())
         except:
             rc = 1
 
         # stop containers
         compose_command = [
-            f'{args.container_system}-compose',
+            args.container_system, 'compose',
             *compose_args,
             'stop',
         ]
 
         run_command(compose_command)
 
         if rc != 0:
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/build.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/build.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/distributed/clean.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/distributed/clean.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             'GRIZZLY_LIMIT_NOFILE': '1024',
             'GRIZZLY_ENVIRONMENT_FILE': fd.name,
             'COLUMNS': str(columns),
             'LINES': str(lines),
         })
 
         compose_command = [
-            f'{args.container_system}-compose',
+            args.container_system, 'compose',
             '-f', f'{STATIC_CONTEXT}/compose.yaml',
             '-p', f'{project_name}{suffix}-{tag}',
             'rm', '-f', '-s', '-v',
         ]
 
         rc = run_command(compose_command, env=env)
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/init.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/init.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/local.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/local.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/run.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/run.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/static/Containerfile` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/static/Containerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/static/compose.yaml` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/static/compose.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_cli/utils.py` & `grizzly-loadtester-cli-3.1.7/grizzly_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     process.wait()
 
     return returncode or process.returncode
 
 
 def get_docker_compose_version() -> Tuple[int, int, int]:
-    output = subprocess.getoutput('docker-compose version')
+    output = subprocess.getoutput('docker compose version')
 
     version_line = output.splitlines()[0]
 
     match = re.match(r'.*version [v]?([1-2]\.[0-9]+\.[0-9]+).*$', version_line)
 
     if match:
         version = cast(Tuple[int, int, int], tuple([int(part) for part in match.group(1).split('.')]))
@@ -477,22 +477,14 @@
         return None
 
 
 def requirements(execution_context: str) -> Callable[[Callable[..., int]], Callable[..., int]]:
     def wrapper(func: Callable[..., int]) -> Callable[..., int]:
         @wraps(func)
         def _wrapper(*args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> int:
-            requirements_file = path.join(getattr(func, '__value__'), 'requirements.txt')
-            if not path.exists(requirements_file):
-                with open(requirements_file, 'w+') as fd:
-                    fd.write('grizzly-loadtester\n')
-
-                print('!! created a default requirements.txt with one dependency:')
-                print('grizzly-loadtester\n')
-
             return func(*args, **kwargs)
 
         # a bit ugly, but needed for testability
         setattr(func, '__value__', execution_context)
         setattr(_wrapper, '__wrapped__', func)
 
         return _wrapper
@@ -506,16 +498,18 @@
     elif which('podman') is not None:
         container_system = 'podman'
         print('!! podman might not work due to buildah missing support for `RUN --mount=type=ssh`: https://github.com/containers/buildah/issues/2835')
     else:
         print('neither "podman" nor "docker" found in PATH')
         return None
 
-    if which(f'{container_system}-compose') is None:
-        print(f'"{container_system}-compose" not found in PATH')
+    rc, _ = subprocess.getstatusoutput(f'{container_system} compose version')
+
+    if rc != 0:
+        print(f'"{container_system} compose" not found in PATH')
         return None
 
     return container_system
 
 
 def get_input(text: str) -> str:  # pragma: no cover
     return input(text).strip()
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/PKG-INFO` & `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester-cli
-Version: 3.1.6
+Version: 3.1.7
 Summary: Command line interface for grizzly-loadtester
 Author-email: biometria <opensource@biometria.se>
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/command-line-interface/usage/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: grizzly,grizzly-loadtester,cli,command line interface,locust,behave,load,loadtest,performance,traffic generator
 Classifier: Development Status :: 4 - Beta
@@ -19,8 +19,10 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ci
 License-File: LICENSE.md
 
 # Grizzly Command Line Interface
 
-Documentation in [`biometria-se/grizzly`](https://biometria-se.github.io/grizzly/command-line-interface/usage/).
+Documentation can be found [here](https://biometria-se.github.io/grizzly/command-line-interface/usage/).
+
+Issues should be reported in [`biometria-se/grizzly/issues`](https://github.com/Biometria-se/grizzly/issues).
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/SOURCES.txt` & `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+.dockerignore
 .editorconfig
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
-test.py
 grizzly_cli/__init__.py
 grizzly_cli/__main__.py
 grizzly_cli/__version__.py
 grizzly_cli/init.py
 grizzly_cli/local.py
 grizzly_cli/py.typed
 grizzly_cli/run.py
```

### Comparing `grizzly-loadtester-cli-3.1.6/grizzly_loadtester_cli.egg-info/requires.txt` & `grizzly-loadtester-cli-3.1.7/grizzly_loadtester_cli.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 gevent<22.0.0,>=21.12.0
 flask==2.0.3
 pyyaml<7.0.0,>=6.0.0
 types-requests<3.0.0,>=2.27.13
 types-pyyaml
 setuptools-scm>=7.0.3
 wheel>=0.37.0
+snakeviz
```

### Comparing `grizzly-loadtester-cli-3.1.6/pyproject.toml` & `grizzly-loadtester-cli-3.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,17 @@
     "pytablewriter >=0.64.1",
     "line-profiler >=3.5.1",
     "gevent >=21.12.0,<22.0.0",
     "flask ==2.0.3",
     "pyyaml >=6.0.0,<7.0.0",
     "types-requests >=2.27.13,<3.0.0",
     "types-pyyaml",
-    "setuptools-scm>=7.0.3",
-    "wheel>=0.37.0"
+    "setuptools-scm >= 7.0.3",
+    "wheel >= 0.37.0",
+    "snakeviz"
 ]
 ci = [
     "build >=0.7.0",
     "twine >=3.8.0"
 ]
 
 [tool.setuptools_scm]
```

### Comparing `grizzly-loadtester-cli-3.1.6/script/docs-generate-licenses.py` & `grizzly-loadtester-cli-3.1.7/script/docs-generate-licenses.py`

 * *Files identical despite different names*

