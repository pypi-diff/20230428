# Comparing `tmp/hagrid-0.3.6.tar.gz` & `tmp/hagrid-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.6.tar", last modified: Fri Apr 28 03:28:55 2023, max compression
+gzip compressed data, was "hagrid-0.3.7.tar", last modified: Fri Apr 28 06:16:02 2023, max compression
```

## Comparing `hagrid-0.3.6.tar` & `hagrid-0.3.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 03:28:55.537100 hagrid-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-28 03:26:22.000000 hagrid-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.533100 hagrid-0.3.6/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134780 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 03:26:38.000000 hagrid-0.3.6/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 03:26:38.000000 hagrid-0.3.6/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 03:26:22.000000 hagrid-0.3.6/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 03:28:55.000000 hagrid-0.3.6/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:28:55.537100 hagrid-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 03:26:38.000000 hagrid-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:55.537100 hagrid-0.3.6/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 03:26:22.000000 hagrid-0.3.6/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.879761 hagrid-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 06:16:02.875761 hagrid-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-28 06:13:50.000000 hagrid-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134867 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 06:14:05.000000 hagrid-0.3.7/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 06:14:05.000000 hagrid-0.3.7/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 06:16:02.879761 hagrid-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 06:14:05.000000 hagrid-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.6/README.md` & `hagrid-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/__init__.py` & `hagrid-0.3.7/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/art.py` & `hagrid-0.3.7/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/auth.py` & `hagrid-0.3.7/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/azure.py` & `hagrid-0.3.7/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/cache.py` & `hagrid-0.3.7/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/cli.py` & `hagrid-0.3.7/hagrid/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,23 +550,19 @@
     dry_run: bool,
     silent: bool,
     from_rendered_dir: bool,
     progress_bar: Union[Progress, None] = None,
     cmd_name: str = "",
 ) -> None:
     process_list: TypeList = []
-
+    grid_path = GRID_SRC_PATH()
     if node_type == "enclave":
-        cwd = GRID_SRC_PATH + "/worker"
+        cwd = grid_path + "/worker"
     else:
-        cwd = (
-            os.path.join(GRID_SRC_PATH, RENDERED_DIR)
-            if from_rendered_dir
-            else GRID_SRC_PATH
-        )
+        cwd = os.path.join(grid_path, RENDERED_DIR) if from_rendered_dir else grid_path
 
     username, password = (
         extract_username_and_pass(cmds[0]) if len(cmds) > 0 else ("-", "-")
     )
     # display VM credentials
     console = rich.get_console()
     credentials = generate_user_table(username=username, password=password)
@@ -1864,32 +1860,33 @@
     version_string = kwargs["tag"]
     version_hash = "dockerhub"
     build = kwargs["build"]
     from_template = kwargs["from_template"]
 
     # if in development mode, generate a version_string which is either
     # the one you inputed concatenated with -dev or the contents of the VERSION file
+    version = GRID_SRC_VERSION()
     if "release" in kwargs and kwargs["release"] == "development":
         # force version to have -dev at the end in dev mode
         # during development we can use the latest beta version
         if version_string is None:
-            version_string = GRID_SRC_VERSION[0]
+            version_string = version[0]
         version_string += "-dev"
-        version_hash = GRID_SRC_VERSION[1]
+        version_hash = version[1]
         build = True
     else:
         # whereas if in production mode and tag == "local" use the local VERSION file
         # or if its not set somehow, which should never happen, use stable
         # otherwise use the kwargs["tag"] from above
 
         # during production the default would be stable
         if version_string == "local":
             # this can be used in VMs in production to auto update from src
-            version_string = GRID_SRC_VERSION[0]
-            version_hash = GRID_SRC_VERSION[1]
+            version_string = version[0]
+            version_hash = version[1]
             build = True
         elif version_string is None:
             version_string = "latest"
 
     if platform.uname().machine.lower() in ["x86_64", "amd64"]:
         docker_platform = "linux/amd64"
     else:
@@ -1995,42 +1992,43 @@
     else:
         cmd += " ".join(args)
 
     cmd += " docker compose -p " + snake_name
 
     # new docker compose regression work around
     # default_env = os.path.expanduser("~/.hagrid/app/.env")
-    default_env = f"{GRID_SRC_PATH}/.env"
+    grid_path = GRID_SRC_PATH()
+    default_env = f"{grid_path}/.env"
     default_envs = {}
     with open(default_env, "r") as f:
         for line in f.readlines():
             if "=" in line:
                 parts = line.strip().split("=")
                 key = parts[0]
                 value = ""
                 if len(parts) > 1:
                     value = parts[1]
                 default_envs[key] = value
     default_envs.update(envs)
 
     # env file path
-    env_file_path = os.path.join(GRID_SRC_PATH, ".envfile")
+    env_file_path = os.path.join(grid_path, ".envfile")
 
     # Render templates if creating stack from the manifest_template.yml
     if from_template and host_term.host is not None:
         # If release is development, update relative path
         if EDITABLE_MODE:
             default_envs["RELATIVE_PATH"] = "../"
 
         render_templates(
             env_vars=default_envs,
             host_type=host_term.host,
         )
 
-        env_file_path = os.path.join(GRID_SRC_PATH, RENDERED_DIR, ".envfile")
+        env_file_path = os.path.join(grid_path, RENDERED_DIR, ".envfile")
 
     try:
         env_file = ""
         for k, v in default_envs.items():
             env_file += f"{k}={v}\n"
 
         with open(env_file_path, "w") as f:
@@ -2127,15 +2125,15 @@
 
     cmd = ""
     cmd += 'ANSIBLE_ARGS="'
     cmd += f"-e 'node_name={snake_name}'"
     cmd += f"-e 'node_type={node_type.input}'"
     cmd += '" '
     cmd += "vagrant up --provision"
-    cmd = "cd " + GRID_SRC_PATH + ";" + cmd
+    cmd = "cd " + GRID_SRC_PATH() + ";" + cmd
     return cmd
 
 
 def get_or_make_resource_group(resource_group: str, location: str = "westus") -> None:
     cmd = f"az group show --resource-group {resource_group}"
     exists = True
     try:
@@ -2731,16 +2729,17 @@
     try:
         host_term = verb.get_named_term_hostgrammar(name="host")
         print("Landing PyGrid node on port " + str(host_term.port) + "!\n")
 
         print("  - PORT: " + str(host_term.port))
         print("\n")
 
-        playbook_path = GRID_SRC_PATH + "/ansible/site.yml"
-        ansible_cfg_path = GRID_SRC_PATH + "/ansible.cfg"
+        grid_path = GRID_SRC_PATH()
+        playbook_path = grid_path + "/ansible/site.yml"
+        ansible_cfg_path = grid_path + "/ansible.cfg"
         auth = cast(AuthCredentials, auth)
 
         if not os.path.exists(playbook_path):
             print(f"Can't find playbook site.yml at: {playbook_path}")
         cmd = f"ANSIBLE_CONFIG={ansible_cfg_path} ansible-playbook "
         if host_term.host == "localhost":
             cmd += "--connection=local "
@@ -2764,15 +2763,15 @@
                 parts = option.strip().split("=")
                 if len(parts) == 2:
                     ANSIBLE_ARGS[parts[0]] = parts[1]
 
         for k, v in ANSIBLE_ARGS.items():
             cmd += f" -e \"{k}='{v}'\""
 
-        cmd = "cd " + GRID_SRC_PATH + ";" + cmd
+        cmd = "cd " + grid_path + ";" + cmd
         return cmd
     except Exception as e:
         print(f"Failed to construct custom deployment cmd: {cmd}. {e}")
         raise e
 
 
 def create_launch_custom_cmd(
@@ -2798,16 +2797,17 @@
         )
 
         print("  - TYPE: " + str(node_type.input))
         print("  - NAME: " + str(snake_name))
         print("  - PORT: " + str(host_term.port))
         print("\n")
 
-        playbook_path = GRID_SRC_PATH + "/ansible/site.yml"
-        ansible_cfg_path = GRID_SRC_PATH + "/ansible.cfg"
+        grid_path = GRID_SRC_PATH()
+        playbook_path = grid_path + "/ansible/site.yml"
+        ansible_cfg_path = grid_path + "/ansible.cfg"
         auth = cast(AuthCredentials, auth)
 
         if not os.path.exists(playbook_path):
             print(f"Can't find playbook site.yml at: {playbook_path}")
         cmd = f"ANSIBLE_CONFIG={ansible_cfg_path} ansible-playbook "
         if host_term.host == "localhost":
             cmd += "--connection=local "
@@ -2877,15 +2877,15 @@
 
         # if mode == "deploy":
         #     ANSIBLE_ARGS["deploy"] = "true"
 
         for k, v in ANSIBLE_ARGS.items():
             cmd += f" -e \"{k}='{v}'\""
 
-        cmd = "cd " + GRID_SRC_PATH + ";" + cmd
+        cmd = "cd " + grid_path + ";" + cmd
         return cmd
     except Exception as e:
         print(f"Failed to construct custom deployment cmd: {cmd}. {e}")
         raise e
 
 
 def create_land_cmd(verb: GrammarVerb, kwargs: TypeDict[str, Any]) -> str:
@@ -2979,19 +2979,20 @@
 
 def create_land_docker_cmd(verb: GrammarVerb) -> str:
     node_name = verb.get_named_term_type(name="node_name")
     snake_name = str(node_name.snake_input)
     containers = shell("docker ps --format '{{.Names}}' | " + f"grep {snake_name}")
 
     # Check if the container name belongs to worker container
+    grid_path = GRID_SRC_PATH()
     if "proxy" in containers:
-        path = GRID_SRC_PATH
+        path = grid_path
         env_var = ";export $(cat .env | sed 's/#.*//g' | xargs);"
     else:
-        path = GRID_SRC_PATH + "/worker"
+        path = grid_path + "/worker"
         env_var = ";export $(cat ../.env | sed 's/#.*//g' | xargs);"
 
     cmd = ""
     cmd += "docker compose"
     cmd += ' --file "docker-compose.yml"'
     cmd += ' --project-name "' + snake_name + '"'
     cmd += " down"
@@ -3062,32 +3063,34 @@
                 var_name="_land_domain",
                 question=f"Are you sure you want to land {target} (y/n)",
                 kind="yesno",
             ),
             kwargs={},
         )
 
+    grid_path = GRID_SRC_PATH()
+
     if force or _land_domain == "y":
         if not bool(kwargs["cmd"]):
             if not silent:
                 print("Running: \n", cmd)
             try:
                 if silent:
                     process = subprocess.Popen(  # nosec
                         cmd,
                         stdout=subprocess.PIPE,
                         stderr=subprocess.PIPE,
-                        cwd=GRID_SRC_PATH,
+                        cwd=grid_path,
                         shell=True,
                     )
                     process.communicate()
 
                     print(f"HAGrid land {target} complete!")
                 else:
-                    subprocess.call(cmd, shell=True, cwd=GRID_SRC_PATH)  # nosec
+                    subprocess.call(cmd, shell=True, cwd=grid_path)  # nosec
             except Exception as e:
                 print(f"Failed to run cmd: {cmd}. {e}")
     else:
         print("Hagrid land aborted.")
 
 
 cli.add_command(launch)
```

### Comparing `hagrid-0.3.6/hagrid/deps.py` & `hagrid-0.3.7/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/grammar.py` & `hagrid-0.3.7/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/land.py` & `hagrid-0.3.7/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/launch.py` & `hagrid-0.3.7/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/lib.py` & `hagrid-0.3.7/hagrid/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,9 +461,9 @@
     except Exception as e:
         if not silent:
             print(f"Failed to check jupyter server status {host_ip}. {e}")
         return False
 
 
 GIT_REPO = get_git_repo
-GRID_SRC_VERSION = get_version_module()
-GRID_SRC_PATH = grid_src_path()
+GRID_SRC_VERSION = get_version_module
+GRID_SRC_PATH = grid_src_path
```

### Comparing `hagrid-0.3.6/hagrid/manifest_template.yml` & `hagrid-0.3.7/hagrid/manifest_template.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.6
+hagrid_version: 0.3.7
 syft_version: 0.8.0
 dockerTag: 0.8.0
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: ed14ea50ece31c8654b229f65e2c598eef1d1a7a
+hash: 65a6ec9eb935fc0f190ff16ea04edecfbdba9e49
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.6/hagrid/mode.py` & `hagrid-0.3.7/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/names.py` & `hagrid-0.3.7/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/orchestra.py` & `hagrid-0.3.7/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/parse_template.py` & `hagrid-0.3.7/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/quickstart_ui.py` & `hagrid-0.3.7/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/rand_sec.py` & `hagrid-0.3.7/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/style.py` & `hagrid-0.3.7/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/util.py` & `hagrid-0.3.7/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/win_bootstrap.py` & `hagrid-0.3.7/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid/wizard_ui.py` & `hagrid-0.3.7/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.7/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.6/setup.py` & `hagrid-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.6/tests/hagrid/cli_test.py` & `hagrid-0.3.7/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

