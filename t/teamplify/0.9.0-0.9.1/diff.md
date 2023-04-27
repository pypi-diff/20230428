# Comparing `tmp/teamplify-0.9.0.tar.gz` & `tmp/teamplify-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamplify-0.9.0.tar", last modified: Tue Apr 25 16:02:31 2023, max compression
+gzip compressed data, was "teamplify-0.9.1.tar", last modified: Thu Apr 27 23:26:44 2023, max compression
```

## Comparing `teamplify-0.9.0.tar` & `teamplify-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225680 teamplify-0.9.0/
--rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.9.0/LICENSE
--rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.9.0/MANIFEST.in
--rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 16:02:31.225778 teamplify-0.9.0/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)    23114 2023-04-25 13:03:30.000000 teamplify-0.9.0/README.md
--rw-r--r--   0 ipeterov   (501) staff       (20)       63 2023-04-18 11:09:50.000000 teamplify-0.9.0/requirements-tests.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       79 2023-04-25 13:03:30.000000 teamplify-0.9.0/requirements.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      253 2023-04-25 16:02:31.226109 teamplify-0.9.0/setup.cfg
--rw-r--r--   0 ipeterov   (501) staff       (20)     1276 2023-04-18 11:02:31.000000 teamplify-0.9.0/setup.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.223736 teamplify-0.9.0/teamplify.egg-info/
--rw-r--r--   0 ipeterov   (501) staff       (20)    23437 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/PKG-INFO
--rw-r--r--   0 ipeterov   (501) staff       (20)      589 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/SOURCES.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/dependency_links.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/entry_points.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)      152 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/requires.txt
--rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-25 16:02:31.000000 teamplify-0.9.0/teamplify.egg-info/top_level.txt
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225363 teamplify-0.9.0/teamplify_runner/
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/__init__.py
-drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-25 16:02:31.225530 teamplify-0.9.0/teamplify_runner/backup/
--rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/backup/readme.txt
--rwxr-xr-x   0 ipeterov   (501) staff       (20)    14147 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/cli.py
--rw-r--r--   0 ipeterov   (501) staff       (20)    14340 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/configurator.py
--rw-r--r--   0 ipeterov   (501) staff       (20)     5349 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/docker-compose.yml
--rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/mysql.cnf
--rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/redis.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)     2228 2023-04-25 16:02:21.000000 teamplify-0.9.0/teamplify_runner/utils.py
--rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/uwsgi_params.conf
--rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.9.0/teamplify_runner/vhost.conf
+drwxr-xr-x   0 geyser     (501) staff       (20)        0 2023-04-27 23:26:44.064429 teamplify-0.9.1/
+-rw-r--r--   0 geyser     (501) staff       (20)     1066 2019-02-27 13:59:43.000000 teamplify-0.9.1/LICENSE
+-rw-r--r--   0 geyser     (501) staff       (20)      272 2023-03-24 10:01:20.000000 teamplify-0.9.1/MANIFEST.in
+-rw-r--r--   0 geyser     (501) staff       (20)    23437 2023-04-27 23:26:44.064605 teamplify-0.9.1/PKG-INFO
+-rw-r--r--   0 geyser     (501) staff       (20)    23114 2023-04-25 13:11:46.000000 teamplify-0.9.1/README.md
+-rw-r--r--   0 geyser     (501) staff       (20)       63 2023-04-18 12:07:15.000000 teamplify-0.9.1/requirements-tests.txt
+-rw-r--r--   0 geyser     (501) staff       (20)       79 2023-04-25 13:11:46.000000 teamplify-0.9.1/requirements.txt
+-rw-r--r--   0 geyser     (501) staff       (20)      253 2023-04-27 23:26:44.065275 teamplify-0.9.1/setup.cfg
+-rw-r--r--   0 geyser     (501) staff       (20)     1276 2023-04-18 12:07:15.000000 teamplify-0.9.1/setup.py
+drwxr-xr-x   0 geyser     (501) staff       (20)        0 2023-04-27 23:26:44.053919 teamplify-0.9.1/teamplify.egg-info/
+-rw-r--r--   0 geyser     (501) staff       (20)    23437 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/PKG-INFO
+-rw-r--r--   0 geyser     (501) staff       (20)      638 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/SOURCES.txt
+-rw-r--r--   0 geyser     (501) staff       (20)        1 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/dependency_links.txt
+-rw-r--r--   0 geyser     (501) staff       (20)       56 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/entry_points.txt
+-rw-r--r--   0 geyser     (501) staff       (20)      152 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/requires.txt
+-rw-r--r--   0 geyser     (501) staff       (20)       17 2023-04-27 23:26:43.000000 teamplify-0.9.1/teamplify.egg-info/top_level.txt
+drwxr-xr-x   0 geyser     (501) staff       (20)        0 2023-04-27 23:26:44.061331 teamplify-0.9.1/teamplify_runner/
+-rw-r--r--   0 geyser     (501) staff       (20)       22 2023-04-27 23:09:35.000000 teamplify-0.9.1/teamplify_runner/__init__.py
+drwxr-xr-x   0 geyser     (501) staff       (20)        0 2023-04-27 23:26:44.062086 teamplify-0.9.1/teamplify_runner/backup/
+-rw-r--r--   0 geyser     (501) staff       (20)       51 2023-04-26 09:44:57.000000 teamplify-0.9.1/teamplify_runner/backup/readme.txt
+-rwxr-xr-x   0 geyser     (501) staff       (20)    14195 2023-04-27 22:46:41.000000 teamplify-0.9.1/teamplify_runner/cli.py
+-rw-r--r--   0 geyser     (501) staff       (20)    14340 2023-04-26 16:36:09.000000 teamplify-0.9.1/teamplify_runner/configurator.py
+-rw-r--r--   0 geyser     (501) staff       (20)     5349 2023-04-26 16:36:09.000000 teamplify-0.9.1/teamplify_runner/docker-compose.yml
+-rw-r--r--   0 geyser     (501) staff       (20)      270 2019-02-27 12:37:27.000000 teamplify-0.9.1/teamplify_runner/mysql.cnf
+-rw-r--r--   0 geyser     (501) staff       (20)       22 2022-11-05 06:53:49.000000 teamplify-0.9.1/teamplify_runner/redis.conf
+-rw-r--r--   0 geyser     (501) staff       (20)     2458 2023-04-27 20:59:46.000000 teamplify-0.9.1/teamplify_runner/utils.py
+-rw-r--r--   0 geyser     (501) staff       (20)      766 2023-04-04 09:42:30.000000 teamplify-0.9.1/teamplify_runner/uwsgi_params.conf
+-rw-r--r--   0 geyser     (501) staff       (20)      512 2021-08-03 11:41:01.000000 teamplify-0.9.1/teamplify_runner/vhost.conf
+drwxr-xr-x   0 geyser     (501) staff       (20)        0 2023-04-27 23:26:44.063778 teamplify-0.9.1/tests/
+-rw-r--r--   0 geyser     (501) staff       (20)     2160 2023-04-18 12:07:15.000000 teamplify-0.9.1/tests/test_configurator.py
+-rw-r--r--   0 geyser     (501) staff       (20)      698 2023-04-18 12:07:15.000000 teamplify-0.9.1/tests/test_startup.py
```

### Comparing `teamplify-0.9.0/LICENSE` & `teamplify-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/PKG-INFO` & `teamplify-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.9.0
+Version: 0.9.1
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.9.0/README.md` & `teamplify-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/setup.py` & `teamplify-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/teamplify.egg-info/PKG-INFO` & `teamplify-0.9.1/teamplify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.9.0
+Version: 0.9.1
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.9.0/teamplify_runner/cli.py` & `teamplify-0.9.1/teamplify_runner/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import os
+import re
 import time
 from datetime import datetime
 
 import click
 import requests
 
 from teamplify_runner import __version__
@@ -28,41 +29,40 @@
         root_url += ':' + port
     return root_url
 
 
 def _wait_for_teamplify_start(url, max_minutes=10, check_interval_seconds=1):
     click.echo('\nTeamplify will be available at {0}\n'.format(url))
 
+    status = 'Connecting'
     start_time = time.time()
     while time.time() < start_time + max_minutes * 60:
         seconds_since_launch = int(time.time() - start_time)
         minutes, seconds = divmod(seconds_since_launch, 60)
         # Add two spaces so we always overwrite the previous string
         click.echo(
-            'Startup in progress, {0} min {1} sec ...  \r'.format(minutes, seconds),
+            '{0}, {1} min {2} sec ...  \r'.format(status, minutes, seconds),
             nl=False,
         )
+        time.sleep(check_interval_seconds)
 
         try:
             response = requests.get(url).text
         except (requests.ConnectionError, requests.Timeout):
-            time.sleep(check_interval_seconds)
+            status = 'Connecting'
             continue
 
-        if 'window.BUILD_NUMBER' in response:
+        if re.search(r"window.BUILD_NUMBER = '\d+'", response):
             click.echo('\n\nTeamplify successfully started!')
             return
-        elif any(
-            marker in response
-            for marker in (
-                'Welcome to nginx!',
-                'Teamplify is starting...',
-            )
-        ):
-            time.sleep(check_interval_seconds)
+        elif 'Welcome to nginx!' in response:
+            status = 'Started nginx'
+            continue
+        elif 'Teamplify is starting...' in response:
+            status = 'Teamplify is starting'
             continue
         else:
             raise RuntimeError(
                 '\n\nUnexpected response from Teamplify: {0}\n\n'
                 'Please check the Troubleshooting guide:\n -> '
                 'https://github.com/teamplify/teamplify-runner/#troubleshooting'.format(response)
             )
@@ -167,17 +167,17 @@
     elif os.path.isdir(filename):
         target_file = os.path.join(filename, default_filename)
     else:
         target_file = filename
     temp_filename = os.path.join('/backup', default_filename)
     cleanup_on_error = not os.path.exists(target_file)
     # check for write access on the host
-    run('touch {0}'.format(temp_filename))
+    run('touch {0}'.format(target_file))
     # check for write access inside docker
-    run('docker exec teamplify_db bash -c "touch {0}"'.format(target_file))
+    run('docker exec teamplify_db bash -c "touch {0}"'.format(temp_filename))
     command = (
         'MYSQL_PWD={password} mysqldump --single-transaction -u{user} '
         '-h {host} {db} | gzip > {filename}'.format(
             user=env['DB_USER'],
             password=env['DB_PASSWORD'],
             host='localhost',
             db=env['DB_NAME'],
```

### Comparing `teamplify-0.9.0/teamplify_runner/configurator.py` & `teamplify-0.9.1/teamplify_runner/configurator.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/teamplify_runner/docker-compose.yml` & `teamplify-0.9.1/teamplify_runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/teamplify_runner/utils.py` & `teamplify-0.9.1/teamplify_runner/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,31 @@
     try:
         yield
     finally:
         os.chdir(cwd)
 
 
 def run(cmd, raise_on_error=True, capture_output=True, suppress_output=False,
-        exit_on_error=True, **kwargs):
+        exit_on_error=True, skip_error_codes=None, **kwargs):
     """
     Wrapper around sarge.run that can raise errors and capture stdout.
     """
     def echo_output(stdout, stderr):
         if stdout:
             click.echo(stdout)
         if stderr:
             click.echo(stderr, err=True)
 
     if capture_output:
         kwargs['stdout'] = sarge.Capture()
         kwargs['stderr'] = sarge.Capture()
     result = sarge.run(cmd, **kwargs)
     code = result.returncode
-    if code and raise_on_error:
+    skip_error_codes = skip_error_codes or []
+    if code and code not in skip_error_codes and raise_on_error:
         if capture_output:
             echo_output(result.stdout.read(), result.stderr.read())
         # print two last traceback records: current line and run caller
         traceback.print_stack(limit=2)
         msg = 'Command failed, exit code {0}'.format(code)
         if exit_on_error:
             click.echo(msg)
@@ -53,16 +54,21 @@
             result.stdout_lines = result.stdout_lines[:-1]
         if not suppress_output:
             echo_output(stdout, result.stderr.read())
     return result
 
 
 def compose(cmd, **kwargs):
-    result = run('docker compose {0}'.format(cmd), **kwargs, raise_on_error=False)
-    if result.returncode == 125:
+    missing_docker_compose_v2_code = 125
+    result = run(
+        'docker compose {0}'.format(cmd),
+        **kwargs,
+        skip_error_codes=[missing_docker_compose_v2_code],
+    )
+    if result.returncode == missing_docker_compose_v2_code:
         result = run('docker-compose {0}'.format(cmd), **kwargs)
         click.echo('WARNING: docker-compose is deprecated, please use Docker Compose V2')
     return result
 
 
 def random_string(length):
     # Use /dev/urandom, see https://stackoverflow.com/a/23728630
```

### Comparing `teamplify-0.9.0/teamplify_runner/uwsgi_params.conf` & `teamplify-0.9.1/teamplify_runner/uwsgi_params.conf`

 * *Files identical despite different names*

### Comparing `teamplify-0.9.0/teamplify_runner/vhost.conf` & `teamplify-0.9.1/teamplify_runner/vhost.conf`

 * *Files identical despite different names*

