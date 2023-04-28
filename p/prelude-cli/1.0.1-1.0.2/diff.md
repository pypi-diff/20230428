# Comparing `tmp/prelude-cli-1.0.1.tar.gz` & `tmp/prelude-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.0.1.tar", last modified: Fri Apr 21 19:57:04 2023, max compression
+gzip compressed data, was "prelude-cli-1.0.2.tar", last modified: Fri Apr 28 19:05:44 2023, max compression
```

## Comparing `prelude-cli-1.0.1.tar` & `prelude-cli-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.978189 prelude-cli-1.0.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-21 19:57:04.978257 prelude-cli-1.0.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.974379 prelude-cli-1.0.1/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1243 2023-04-18 14:03:55.000000 prelude-cli-1.0.1/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.975671 prelude-cli-1.0.1/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.977982 prelude-cli-1.0.1/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.1/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.1/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3757 2023-04-21 19:52:17.000000 prelude-cli-1.0.1/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.1/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.1/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.975461 prelude-cli-1.0.1/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       59 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      690 2023-04-21 19:57:04.978511 prelude-cli-1.0.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.161214 prelude-cli-1.0.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-28 19:05:44.161278 prelude-cli-1.0.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.157199 prelude-cli-1.0.2/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1078 2023-04-28 18:41:33.000000 prelude-cli-1.0.2/prelude_cli/cli.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.158362 prelude-cli-1.0.2/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.160987 prelude-cli-1.0.2/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.2/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.2/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3757 2023-04-21 20:11:38.000000 prelude-cli-1.0.2/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.2/prelude_cli/views/interactive.py
+-rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.2/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.158167 prelude-cli-1.0.2/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       61 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      694 2023-04-28 19:05:44.161532 prelude-cli-1.0.2/setup.cfg
```

### Comparing `prelude-cli-1.0.1/LICENSE` & `prelude-cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/PKG-INFO` & `prelude-cli-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.0.1/prelude_cli/cli.py` & `prelude-cli-1.0.2/prelude_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 from prelude_cli.views.detect import detect
 from prelude_cli.views.partner import partner
 from prelude_sdk.models.account import Account
 from prelude_cli.views.configure import configure
 from prelude_cli.views.interactive import interactive as interactive_command
 
 
-def complete_profile(ctx, param, incomplete):
-    return [x for x in Account().read_keychain_config() if x.startswith(incomplete)]
-
 @click.group(invoke_without_command=True)
 @click.version_option()
 @click.pass_context
-@click.option('--profile', default='default', help='The prelude keychain profile to use', show_default=True, shell_complete=complete_profile)
+@click.option('--profile', default='default', help='The prelude keychain profile to use', show_default=True)
 @click.option('--interactive', help='Open interactive wizard (cannot be used with a subcommand)', default=False, is_flag=True)
 def cli(ctx, profile, interactive):
     ctx.obj = Account(profile=profile)
     if ctx.invoked_subcommand is None:
         if interactive:
             ctx.invoke(interactive_command)
         else:
```

### Comparing `prelude-cli-1.0.1/prelude_cli/views/build.py` & `prelude-cli-1.0.2/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli/views/configure.py` & `prelude-cli-1.0.2/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli/views/detect.py` & `prelude-cli-1.0.2/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli/views/iam.py` & `prelude-cli-1.0.2/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli/views/interactive.py` & `prelude-cli-1.0.2/prelude_cli/views/interactive.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli/views/partner.py` & `prelude-cli-1.0.2/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.0.2/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.0.1/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.0.2/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.1/setup.cfg` & `prelude-cli-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.0.1
+version = 1.0.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -14,15 +14,15 @@
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	prelude-sdk == 1.0.1
-	click
+	click > 8
 	rich
 	simple-term-menu
 	gnureadline
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

