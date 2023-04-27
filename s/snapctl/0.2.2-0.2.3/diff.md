# Comparing `tmp/snapctl-0.2.2.tar.gz` & `tmp/snapctl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.2.2.tar", max compression
+gzip compressed data, was "snapctl-0.2.3.tar", max compression
```

## Comparing `snapctl-0.2.2.tar` & `snapctl-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.2/README.md
--rw-r--r--   0        0        0      399 2023-04-27 23:51:21.069010 snapctl-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.2/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.2/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.2/snapctl/commands/__init__.py
--rw-r--r--   0        0        0     8130 2023-04-27 23:51:15.912586 snapctl-0.2.2/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.2/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.2/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.2/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.2/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.2/snapctl/utils/echo.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.3/README.md
+-rw-r--r--   0        0        0      399 2023-04-27 23:55:39.164939 snapctl-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.3/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.3/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.3/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     8348 2023-04-27 23:55:33.316516 snapctl-0.2.3/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.3/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.3/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.3/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.3/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.3/snapctl/utils/echo.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.3/PKG-INFO
```

### Comparing `snapctl-0.2.2/snapctl/commands/byosnap.py` & `snapctl-0.2.3/snapctl/commands/byosnap.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,17 @@
         transient=True,
       ) as progress:
         progress.add_task(description=f'Logging into Snapser Image Registry...', total=None)
         if platform == 'win32':
           response = subprocess.run([
             f'echo({ecr_repo_token}| docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+          response = subprocess.run([
+            f'docker login --username {ecr_repo_username} --password {ecr_repo_token} {ecr_repo_url}'
+          ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         else:
           response = subprocess.run([
             f'echo "{ecr_repo_token}" | docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to connect to the Snapser Container Repository. Please get the latest token from the Web app.')
           error(f'echo({ecr_repo_token}| docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}')
```

### Comparing `snapctl-0.2.2/snapctl/main.py` & `snapctl-0.2.3/snapctl/main.py`

 * *Files identical despite different names*

### Comparing `snapctl-0.2.2/PKG-INFO` & `snapctl-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapctl
-Version: 0.2.2
+Version: 0.2.3
 Summary: Snapser CLI Tool
 Author: Ajinkya Apte
 Author-email: aj@snapser.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

