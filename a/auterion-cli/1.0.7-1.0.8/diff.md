# Comparing `tmp/auterion-cli-1.0.7.tar.gz` & `tmp/auterion-cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.7.tar", last modified: Thu Apr 27 11:42:00 2023, max compression
+gzip compressed data, was "auterion-cli-1.0.8.tar", last modified: Fri Apr 28 08:44:58 2023, max compression
```

## Comparing `auterion-cli-1.0.7.tar` & `auterion-cli-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.956484 auterion-cli-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 11:41:59.000000 auterion-cli-1.0.7/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.948484 auterion-cli-1.0.7/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 11:42:00.000000 auterion-cli-1.0.7/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:42:00.952484 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-27 11:41:50.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-27 11:41:50.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 11:42:00.956484 auterion-cli-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-27 11:41:49.000000 auterion-cli-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/setup.py
```

### Comparing `auterion-cli-1.0.7/README.md` & `auterion-cli-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.0.8/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_command.py` & `auterion-cli-1.0.8/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     server_version = 'N/A'
     if 'Server' in res:
         server_version = res['Server']['Version']
     client_version = res['Client']['Version']
     print(f'.. Found docker client {client_version}, server {server_version}')
 
     client_version_components = client_version.split('.')
-    if len(client_version_components) <= 0 or int(client_version_components[0]) < 23:
-        error('auterion-cli needs at least docker client 23.\nMake sure to update the docker version on your system'
+    if len(client_version_components) <= 0 or int(client_version_components[0]) < 20:
+        error('auterion-cli needs at least docker client 20.\nMake sure to update the docker version on your system'
               'using your package manager. \n'
               'For ubuntu, find more information on https://docs.docker.com/engine/install/ubuntu/ ')
 
     # Try podman-compose, fall back to docker compose
     compose_cmd = ['podman-compose']
 
     code, _ = try_command(compose_cmd + ['version'])
```

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/slimify.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,38 +48,28 @@
     if cache_dir is not None:
         cache_file = os.path.join(cache_dir, cache_key)
         if os.path.exists(os.path.join(cache_dir, cache_key)):
             print(f'.. Found cached base layer information for {base_image}')
             with open(cache_file, 'r') as f:
                 return json.load(f)
 
-    print(f'> Fetching manifest for {base_image}')
-    ret = {}
     try:
-        ret = run_docker_command(['docker', 'manifest', 'inspect', base_image])
+        run_docker_command(['docker', 'pull', '--platform=linux/arm64', base_image], json_out=False)
     except:
-        error(f'Could not fetch manifest for image {base_image}. Aborting...')
+        error(f'Failed to pull arm64 image for {base_image}. Aborting...')
 
-    manifests = ret['manifests']
-    arm64_digest = next(d['digest'] for d in manifests if 'arm64' in d['platform']['architecture'])
-    print(f'.. arm64 image digest for {base_image} is {arm64_digest}')
-    print(f'> Pulling arm64 image for {base_image}')
-    pull_name = base_image.split(':')[0] + '@' + arm64_digest
-    try:
-        run_docker_command(['docker', 'pull', pull_name], json_out=False)
-    except:
-        error(f'Failed to pull {pull_name}. Aborting...')
-
-    print(f'.. Pulled {pull_name}')
+    print(f'.. Pulled {base_image}')
     print('> Inspecting image')
     try:
-        ret = run_docker_command(['docker', 'inspect', pull_name])
+        ret = run_docker_command(['docker', 'inspect', base_image])
     except:
-        error(f'Failed to inspect image {pull_name}. Aborting..')
+        error(f'Failed to inspect image {base_image}. Aborting..')
 
+    assert(ret[0]['Architecture'] == 'arm64')
+    assert(ret[0]['Os'] == 'linux')
     layers = ret[0]['RootFS']['Layers']
     print(f'.. Base image has {len(layers)} layers')
 
     if cache_dir is not None:
         cache_file = os.path.join(cache_dir, cache_key)
         with open(cache_file, 'w') as f:
             json.dump(layers, f)
```

### Comparing `auterion-cli-1.0.7/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.0.8/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/container_command.py` & `auterion-cli-1.0.8/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/device_command.py` & `auterion-cli-1.0.8/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/info_command.py` & `auterion-cli-1.0.8/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/report_command.py` & `auterion-cli-1.0.8/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/commands/utils.py` & `auterion-cli-1.0.8/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/main.py` & `auterion-cli-1.0.8/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/auterioncli/meta_util.py` & `auterion-cli-1.0.8/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.7/setup.py` & `auterion-cli-1.0.8/setup.py`

 * *Files identical despite different names*

