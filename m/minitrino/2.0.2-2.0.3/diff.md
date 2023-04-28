# Comparing `tmp/minitrino-2.0.2.tar.gz` & `tmp/minitrino-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minitrino-2.0.2.tar", last modified: Tue Oct 19 16:37:50 2021, max compression
+gzip compressed data, was "minitrino-2.0.3.tar", last modified: Fri Apr 28 21:32:16 2023, max compression
```

## Comparing `minitrino-2.0.2.tar` & `minitrino-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jeffreylester   (501) staff       (20)        0 2021-10-19 16:37:50.184313 minitrino-2.0.2/
--rw-r--r--   0 jeffreylester   (501) staff       (20)    41147 2021-10-19 16:37:50.183621 minitrino-2.0.2/PKG-INFO
-drwxr-xr-x   0 jeffreylester   (501) staff       (20)        0 2021-10-19 16:37:50.177362 minitrino-2.0.2/minitrino/
--rw-r--r--   0 jeffreylester   (501) staff       (20)        0 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/__init__.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     1977 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cli.py
-drwxr-xr-x   0 jeffreylester   (501) staff       (20)        0 2021-10-19 16:37:50.182626 minitrino-2.0.2/minitrino/cmd/
--rw-r--r--   0 jeffreylester   (501) staff       (20)        0 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/__init__.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     2368 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_config.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     2194 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_down.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     2973 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_lib_install.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     2582 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_modules.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)    23541 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_provision.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     4058 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_remove.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)    13033 2021-10-19 16:34:59.000000 minitrino-2.0.2/minitrino/cmd/cmd_snapshot.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)      642 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/cmd/cmd_version.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)    30751 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/components.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)      987 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/errors.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)     2011 2021-10-19 16:34:59.000000 minitrino-2.0.2/minitrino/settings.py
--rw-r--r--   0 jeffreylester   (501) staff       (20)    11299 2021-10-19 15:18:42.000000 minitrino-2.0.2/minitrino/utils.py
-drwxr-xr-x   0 jeffreylester   (501) staff       (20)        0 2021-10-19 16:37:50.179190 minitrino-2.0.2/minitrino.egg-info/
--rw-r--r--   0 jeffreylester   (501) staff       (20)    41147 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/PKG-INFO
--rw-r--r--   0 jeffreylester   (501) staff       (20)      592 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreylester   (501) staff       (20)        1 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreylester   (501) staff       (20)       49 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/entry_points.txt
--rw-r--r--   0 jeffreylester   (501) staff       (20)       43 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/requires.txt
--rw-r--r--   0 jeffreylester   (501) staff       (20)       10 2021-10-19 16:37:50.000000 minitrino-2.0.2/minitrino.egg-info/top_level.txt
--rw-r--r--   0 jeffreylester   (501) staff       (20)       38 2021-10-19 16:37:50.184470 minitrino-2.0.2/setup.cfg
--rw-r--r--   0 jeffreylester   (501) staff       (20)     1110 2021-10-19 16:34:59.000000 minitrino-2.0.2/setup.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.331374 minitrino-2.0.3/
+-rw-r--r--   0 jlester    (503) staff       (20)    31768 2023-04-28 21:32:16.331204 minitrino-2.0.3/PKG-INFO
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.329030 minitrino-2.0.3/minitrino/
+-rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/__init__.py
+-rw-r--r--   0 jlester    (503) staff       (20)     1977 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cli.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.330984 minitrino-2.0.3/minitrino/cmd/
+-rw-r--r--   0 jlester    (503) staff       (20)        0 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/__init__.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2368 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_config.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2194 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_down.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2971 2023-04-17 15:08:13.000000 minitrino-2.0.3/minitrino/cmd/cmd_lib_install.py
+-rw-r--r--   0 jlester    (503) staff       (20)     2291 2023-04-28 18:26:59.000000 minitrino-2.0.3/minitrino/cmd/cmd_modules.py
+-rw-r--r--   0 jlester    (503) staff       (20)    26055 2023-04-28 17:43:50.000000 minitrino-2.0.3/minitrino/cmd/cmd_provision.py
+-rw-r--r--   0 jlester    (503) staff       (20)     4058 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_remove.py
+-rw-r--r--   0 jlester    (503) staff       (20)    13142 2023-04-28 16:41:24.000000 minitrino-2.0.3/minitrino/cmd/cmd_snapshot.py
+-rw-r--r--   0 jlester    (503) staff       (20)      642 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/cmd/cmd_version.py
+-rw-r--r--   0 jlester    (503) staff       (20)    30017 2023-04-28 17:40:12.000000 minitrino-2.0.3/minitrino/components.py
+-rw-r--r--   0 jlester    (503) staff       (20)      987 2023-01-12 16:45:57.000000 minitrino-2.0.3/minitrino/errors.py
+-rw-r--r--   0 jlester    (503) staff       (20)     1656 2023-04-27 23:02:35.000000 minitrino-2.0.3/minitrino/settings.py
+-rw-r--r--   0 jlester    (503) staff       (20)    11306 2023-04-17 15:08:13.000000 minitrino-2.0.3/minitrino/utils.py
+drwxr-xr-x   0 jlester    (503) staff       (20)        0 2023-04-28 21:32:16.329836 minitrino-2.0.3/minitrino.egg-info/
+-rw-r--r--   0 jlester    (503) staff       (20)    31768 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/PKG-INFO
+-rw-r--r--   0 jlester    (503) staff       (20)      592 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/SOURCES.txt
+-rw-r--r--   0 jlester    (503) staff       (20)        1 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/dependency_links.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       49 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/entry_points.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       43 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/requires.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       10 2023-04-28 21:32:16.000000 minitrino-2.0.3/minitrino.egg-info/top_level.txt
+-rw-r--r--   0 jlester    (503) staff       (20)       38 2023-04-28 21:32:16.331430 minitrino-2.0.3/setup.cfg
+-rw-r--r--   0 jlester    (503) staff       (20)     1110 2023-04-28 21:30:48.000000 minitrino-2.0.3/setup.py
```

### Comparing `minitrino-2.0.2/minitrino/cli.py` & `minitrino-2.0.3/minitrino/cli.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_config.py` & `minitrino-2.0.3/minitrino/cmd/cmd_config.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_down.py` & `minitrino-2.0.3/minitrino/cmd/cmd_down.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_lib_install.py` & `minitrino-2.0.3/minitrino/cmd/cmd_lib_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     download_and_extract(version)
     ctx.logger.log("Library installation complete.")
 
 
 @pass_environment
 def download_and_extract(ctx, version=""):
-
     github_uri = f"https://github.com/jefflester/minitrino/archive/{version}.tar.gz"
     tarball = os.path.join(ctx.minitrino_user_dir, f"{version}.tar.gz")
     file_basename = f"minitrino-{version}"  # filename after unpacking
     lib_dir = os.path.join(ctx.minitrino_user_dir, file_basename, "lib")
 
     try:
         # Download the release tarball
@@ -89,12 +88,11 @@
     except Exception as e:
         cleanup(tarball, file_basename, False)
         raise err.MinitrinoError(str(e))
 
 
 @pass_environment
 def cleanup(ctx, tarball="", file_basename="", trigger_error=True):
-
     ctx.cmd_executor.execute_commands(
         f"rm -rf {tarball} {os.path.join(ctx.minitrino_user_dir, file_basename)}",
         trigger_error=trigger_error,
     )
```

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_modules.py` & `minitrino-2.0.3/minitrino/cmd/cmd_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,52 +39,50 @@
     is_flag=True,
     default=False,
     help=("""Print metadata for all running modules."""),
 )
 @utils.exception_handler
 @pass_environment
 def cli(ctx, modules, json_format, running):
-    """Version command for Minitrino."""
+    """Module metadata command for Minitrino."""
 
     utils.check_lib(ctx)
 
     ctx.logger.log("Printing module metadata...")
 
-    if modules and not running:
-        for module in modules:
-            module_dict = ctx.modules.data.get(module, {})
-            if not module_dict:
-                raise err.UserError(
-                    f"Invalid module: {module}",
-                    "Ensure the module you're referencing is in the Minitrino library.",
-                )
+    if not modules and not running:
+        for module, module_dict in ctx.modules.data.items():
             log_info(module, module_dict, json_format)
-    else:
-        if running:
-            for module_key, module_dict in ctx.modules.get_running_modules().items():
-                for i, container in enumerate(module_dict.get("containers", {})):
-                    module_dict["containers"][i] = {
-                        "id": container.short_id,
-                        "name": container.name,
-                        "labels": container.labels,
-                    }
-                log_info(module_key, module_dict, json_format)
-        else:
-            for module_key, module_dict in ctx.modules.data.items():
-                log_info(module_key, module_dict, json_format)
+        return
+
+    if running:
+        modules = ctx.modules.get_running_modules()
+
+    for module in modules:
+        module_dict = ctx.modules.data.get(module, {})
+        if not module_dict:
+            raise err.UserError(
+                f"Invalid module: '{module}'",
+                "Ensure the module you're referencing is in the Minitrino library.",
+            )
+        log_info(module, module_dict, json_format)
 
 
 @pass_environment
 def log_info(ctx, module_name="", module_dict={}, json_format=False):
     """Logs module metadata to the user's terminal."""
 
     if json_format:
         module_dict = {module_name: module_dict}
         ctx.logger.log(json.dumps(module_dict, indent=2))
     else:
         log_msg = [f"Module: {module_name}\n"]
-        keys = ["description", "incompatibleModules", "enterprise"]
-        for k, v in module_dict.items():
-            if k in keys:
-                log_msg.extend(f"{k.title()}: {v}\n")
+        keys = ["description", "incompatibleModules", "dependentModules", "enterprise"]
+        for key in keys:
+            val = module_dict.get(key, None)
+            if val is not None:
+                key = list(key)
+                key[0] = key[0].title()
+                key = "".join(key)
+                log_msg.extend(f"{key}: {val}\n")
 
         ctx.logger.log("".join(log_msg))
```

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_provision.py` & `minitrino-2.0.3/minitrino/cmd/cmd_provision.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 # required because the Docker SDK does not support communication with Compose
 # files, and Minitrino benefits hugely from Docker Compose.
 
 import os
 import stat
 import hashlib
 import time
+import platform
 import click
 import yaml
 
 from minitrino.cli import pass_environment
 from minitrino import utils
 from minitrino import errors as err
 from minitrino.settings import RESOURCE_LABEL
-from minitrino.settings import MODULE_ROOT
-from minitrino.settings import MODULE_CATALOG
-from minitrino.settings import MODULE_SECURITY
 from minitrino.settings import ETC_TRINO
+from minitrino.settings import SEP_VOLUME_MOUNT
 from minitrino.settings import TRINO_CONFIG
 from minitrino.settings import TRINO_JVM_CONFIG
 
 from docker.errors import NotFound
 
 
 @click.command(
@@ -75,21 +74,22 @@
     """Provision command for Minitrino. If the resulting docker-compose command
     is unsuccessful, the function exits with a non-zero status code."""
 
     utils.check_daemon(ctx.docker_client)
     utils.check_lib(ctx)
     utils.check_starburst_ver(ctx)
     modules = append_running_modules(modules)
+    modules = check_dependent_modules(modules)
     check_compatibility(modules)
     check_enterprise(modules)
+    check_volumes(modules)
 
     if not modules:
         ctx.logger.log(
-            f"No catalog or security options received. Provisioning "
-            f"standalone Trino container..."
+            f"No modules specified. Provisioning standalone Trino container..."
         )
     else:
         for module in modules:
             if not ctx.modules.data.get(module, False):
                 raise err.UserError(
                     f"Invalid module: '{module}'. It was not found "
                     f"in the Minitrino library at {ctx.minitrino_lib_dir}"
@@ -100,21 +100,23 @@
 
         # Module env variables shared with compose should be from the modules
         # section of environment variables and any extra variables provided by the
         # user that didn't fit into any other section
 
         compose_env = ctx.env.get_section("MODULES")
         compose_env.update(ctx.env.get_section("EXTRA"))
+        if is_apple_m1():
+            compose_env.update({"MODULE_PLATFORM": "linux/amd64"})
         compose_cmd = build_command(docker_native, compose_env, cmd_chunk)
 
         ctx.cmd_executor.execute_commands(compose_cmd, environment=compose_env)
         initialize_containers()
 
         containers_to_restart = execute_bootstraps(modules)
-        containers_to_restart = append_user_config(containers_to_restart)
+        containers_to_restart = write_trino_configs(containers_to_restart, modules)
         check_dup_configs()
         restart_containers(containers_to_restart)
         ctx.logger.log(f"Environment provisioning complete.")
 
     except Exception as e:
         rollback_provision(no_rollback)
         utils.handle_exception(e)
@@ -122,30 +124,44 @@
 
 @pass_environment
 def append_running_modules(ctx, modules=[]):
     """Checks if any modules are already running. If they are, they are appended
     to the provided modules list and the updated list is returned."""
 
     ctx.logger.log("Checking for running modules...", level=ctx.logger.verbose)
-    running_modules_dict = ctx.modules.get_running_modules()
-    running_modules_list = []
+    running_modules = ctx.modules.get_running_modules()
 
-    for module in running_modules_dict:
-        running_modules_list.append(module)
-
-    if running_modules_list:
+    if running_modules:
         ctx.logger.log(
-            f"Identified the following running modules: {running_modules_list}. "
-            f"Appending the running module list to the list of modules to provsion.",
+            f"Identified the following running modules: {running_modules}. "
+            f"Appending the running module list to the list of modules to provision.",
             level=ctx.logger.verbose,
         )
 
     modules = list(modules)
-    modules.extend(running_modules_list)
-    return list(set(modules))
+    modules.extend(running_modules)
+    return modules
+
+
+@pass_environment
+def check_dependent_modules(ctx, modules=[]):
+    """Checks if any of the provided modules have module dependencies."""
+
+    for module in modules:
+        dependent_modules = ctx.modules.data.get(module, {}).get("dependentModules", [])
+        if not dependent_modules:
+            continue
+        for dependent_module in dependent_modules:
+            if not dependent_module in modules:
+                modules.append(dependent_module)
+                ctx.logger.log(
+                    f"Module dependency for module '{module}' will be included: '{dependent_module}'",
+                    level=ctx.logger.verbose,
+                )
+    return modules
 
 
 @pass_environment
 def check_compatibility(ctx, modules=[]):
     """Checks if any of the provided modules are mutually exclusive of each
     other. If they are, a user error is raised."""
 
@@ -179,40 +195,77 @@
 
     for module in modules:
         enterprise = ctx.modules.data.get(module, {}).get("enterprise", False)
         if enterprise:
             yaml_path = os.path.join(ctx.minitrino_lib_dir, "docker-compose.yml")
             with open(yaml_path) as f:
                 yaml_file = yaml.load(f, Loader=yaml.FullLoader)
-            if (
-                not yaml_file.get("services", False)
-                .get("trino", False)
-                .get("volumes", False)
-            ):
+            volumes = yaml_file.get("services", {}).get("trino", {}).get("volumes", [])
+            if SEP_VOLUME_MOUNT not in volumes:
                 raise err.UserError(
                     f"Module {module} requires a Starburst license. "
                     f"The license volume in the library's docker-compose.yml "
-                    f"file must be uncommented at: {yaml_path}"
+                    f"file must be uncommented at: {yaml_path}."
+                    f"For reference, the proper volume mount is: '{SEP_VOLUME_MOUNT}'"
                 )
             if not ctx.env.get_var("STARBURST_LIC_PATH", False):
                 raise err.UserError(
                     f"Module {module} requires a Starburst license. "
                     f"You must provide a path to a Starburst license via the "
                     f"STARBURST_LIC_PATH environment variable"
                 )
 
 
 @pass_environment
+def check_volumes(ctx, modules=[]):
+    """Checks if any of the modules have persistent volumes and issues a warning
+    to the user if so."""
+
+    ctx.logger.log(
+        "Checking modules for persisent volumes...",
+        level=ctx.logger.verbose,
+    )
+
+    for module in modules:
+        if ctx.modules.data.get(module, {}).get("yaml_dict", {}).get("volumes", {}):
+            ctx.logger.log(
+                f"Module '{module}' has persistent volumes associated with it. "
+                f"To delete these volumes, remember to run `minitrino remove --volumes`.",
+                level=ctx.logger.warn,
+            )
+
+
+@pass_environment
+def is_apple_m1(ctx):
+    """Checks the host platform to determine if MODULE_PLATFORM needs to
+    be set."""
+
+    ctx.logger.log(
+        "Checking host platform...",
+        level=ctx.logger.verbose,
+    )
+
+    if "arm64" == os.uname().machine.lower() and platform.processor().lower() == "arm":
+        ctx.logger.log(
+            f"Host machine running on Apple M1 architecture. "
+            f"Images will pull in a best-effort fashion.",
+            level=ctx.logger.verbose,
+        )
+        return True
+    return False
+
+
+@pass_environment
 def chunk(ctx, modules=[]):
     """Builds docker-compose command chunk for the chosen modules. Returns a
     command chunk string."""
 
     chunk = []
-    for mod in modules:
-        yaml_file = ctx.modules.data.get(mod, "").get("yaml_file", "")
+    for module in modules:
+        yaml_file = ctx.modules.data.get(module, {}).get("yaml_file", "")
         chunk.extend(f"-f {yaml_file} \\\n")
     return "".join(chunk)
 
 
 @pass_environment
 def build_command(ctx, docker_native="", compose_env={}, chunk=""):
     """Builds a formatted docker-compose command for shell execution. Returns a
@@ -434,29 +487,43 @@
                         f"{check_file} file:\n{duplicates_string}",
                         level=ctx.logger.warn,
                     )
                     duplicates = []
 
 
 @pass_environment
-def append_user_config(ctx, containers_to_restart=[]):
-    """Appends Trino config from minitrino.cfg file. If the config is not
-    present, it is added. If it exists, it is replaced. If anything changes in
-    the Trino config, the Trino container is added to the restart list if it's
-    not already in the list."""
-
-    user_trino_config = ctx.env.get_var("CONFIG", "")
-    if user_trino_config:
-        user_trino_config = user_trino_config.strip().split("\n")
-
-    user_jvm_config = ctx.env.get_var("JVM_CONFIG", "")
-    if user_jvm_config:
-        user_jvm_config = user_jvm_config.strip().split("\n")
+def write_trino_configs(ctx, containers_to_restart=[], modules=[]):
+    """Appends Trino config from various modules if specified in the module YAML
+    file. The Trino container is added to the restart list if any configs are
+    written to files in the container."""
+
+    config_properties = []
+    jvm_config = []
+
+    for module in modules:
+        yaml = ctx.modules.data.get(module, {}).get("yaml_dict")
+        conf = (
+            yaml.get("services", {})
+            .get("trino", {})
+            .get("environment", {})
+            .get("CONFIG_PROPERTIES", {})
+        )
+        jvm = (
+            yaml.get("services", {})
+            .get("trino", {})
+            .get("environment", {})
+            .get("JVM_CONFIG", {})
+        )
+
+        if conf:
+            config_properties.extend(conf.strip().split("\n"))
+        if jvm:
+            jvm_config.extend(jvm.strip().split("\n"))
 
-    if not user_trino_config and not user_jvm_config:
+    if not config_properties and not jvm_config:
         return containers_to_restart
 
     ctx.logger.log(
         "Appending user-defined Trino config to Trino container config...",
         level=ctx.logger.verbose,
     )
 
@@ -497,19 +564,22 @@
         suppress_output=True,
     )
 
     current_trino_config = current_configs[0].get("output", "").strip().split("\n")
     current_jvm_config = current_configs[1].get("output", "").strip().split("\n")
 
     def append_configs(user_configs, current_configs, filename):
-
         # If there is an overlapping config key, replace it with the user
         # config. If there is not overlapping config key, append it to the
         # current config list.
 
+        # No additional configs, leave the file in the container alone
+        if not user_configs:
+            return
+
         if filename == TRINO_CONFIG:
             for user_config in user_configs:
                 user_config = utils.parse_key_value_pair(
                     user_config, err_type=err.UserError, key_to_upper=False
                 )
                 if user_config is None:
                     continue
@@ -545,27 +615,36 @@
                         break
                     if (
                         i + 1 == len(current_configs)
                         and not user_config in current_configs
                     ):
                         current_configs.append(user_config)
 
-        # Replace existing file with new values
+        ctx.logger.log(
+            f"Removing existing {filename} file...",
+            level=ctx.logger.verbose,
+        )
         ctx.cmd_executor.execute_commands(
             f"rm {ETC_TRINO}/{filename}", container=trino_container
         )
 
+        ctx.logger.log(
+            f"Writing new config to {filename}...",
+            level=ctx.logger.verbose,
+        )
         for current_config in current_configs:
             append_config = (
                 f'bash -c "cat <<EOT >> {ETC_TRINO}/{filename}\n{current_config}\nEOT"'
             )
-            ctx.cmd_executor.execute_commands(append_config, container=trino_container)
+            ctx.cmd_executor.execute_commands(
+                append_config, container=trino_container, suppress_output=True
+            )
 
-    append_configs(user_trino_config, current_trino_config, TRINO_CONFIG)
-    append_configs(user_jvm_config, current_jvm_config, TRINO_JVM_CONFIG)
+    append_configs(config_properties, current_trino_config, TRINO_CONFIG)
+    append_configs(jvm_config, current_jvm_config, TRINO_JVM_CONFIG)
 
     if not "trino" in containers_to_restart:
         containers_to_restart.append("trino")
 
     return containers_to_restart
```

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_remove.py` & `minitrino-2.0.3/minitrino/cmd/cmd_remove.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_snapshot.py` & `minitrino-2.0.3/minitrino/cmd/cmd_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from minitrino.cli import pass_environment
 from minitrino import utils
 from minitrino import errors as err
 from minitrino.settings import SNAPSHOT_ROOT_FILES
 from minitrino.settings import PROVISION_SNAPSHOT_TEMPLATE
 from minitrino.settings import LIB
 from minitrino.settings import MODULE_ROOT
+from minitrino.settings import MODULE_ADMIN
 from minitrino.settings import MODULE_CATALOG
 from minitrino.settings import MODULE_SECURITY
 from minitrino.settings import MODULE_RESOURCES
 from minitrino.settings import SCRUB_KEYS
 
 
 @click.command(
@@ -114,15 +115,15 @@
             ctx.logger.log(
                 f"No running Minitrino modules to snapshot. Snapshotting "
                 f"Trino resources only.",
                 level=ctx.logger.verbose,
             )
         else:
             ctx.logger.log(f"Creating snapshot of active environment...")
-        snapshot_runner(name, no_scrub, True, list(modules.keys()), directory)
+        snapshot_runner(name, no_scrub, True, modules, directory)
 
     check_complete(name, directory)
     ctx.logger.log(
         f"Snapshot complete and saved at path: {os.path.join(directory, name)}.tar.gz"
     )
 
 
@@ -249,15 +250,16 @@
 def clone_lib_dir(ctx, name):
     """Clones the library directory structure and necessary top-level files in
     preparation for copying over module directories.
 
     Returns the absolute path of the named snapshot directory."""
 
     snapshot_name_dir = os.path.join(ctx.snapshot_dir, name)
-    os.makedirs(os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, MODULE_CATALOG))
+    os.makedirs(os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, MODULE_ADMIN))
+    os.mkdir(os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, MODULE_CATALOG))
     os.mkdir(os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, MODULE_SECURITY))
     os.mkdir(os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, MODULE_RESOURCES))
 
     # Copy root lib files to snapshot
     for filename in os.listdir(ctx.minitrino_lib_dir):
         if filename in SNAPSHOT_ROOT_FILES:
             file_path = os.path.join(ctx.minitrino_lib_dir, filename)
@@ -347,16 +349,16 @@
 
 
 @pass_environment
 def copy_module_dirs(ctx, snapshot_name_dir, modules=[]):
     """Copies module directories into the named snapshot directory."""
 
     for module in modules:
-        module_dir = ctx.modules.data.get(module, "").get("module_dir", "")
-        module_type = ctx.modules.data.get(module, "").get("type", "")
+        module_dir = ctx.modules.data.get(module, {}).get("module_dir", "")
+        module_type = ctx.modules.data.get(module, {}).get("type", "")
         dest_dir = os.path.join(
             os.path.join(snapshot_name_dir, LIB, MODULE_ROOT, module_type),
             os.path.basename(module_dir),
         )
         shutil.copytree(module_dir, dest_dir)
```

### Comparing `minitrino-2.0.2/minitrino/cmd/cmd_version.py` & `minitrino-2.0.3/minitrino/cmd/cmd_version.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/components.py` & `minitrino-2.0.3/minitrino/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from configparser import ConfigParser
 
 from minitrino import utils
 from minitrino import errors as err
 from minitrino.settings import RESOURCE_LABEL
 from minitrino.settings import MODULE_LABEL_KEY_ROOT
 from minitrino.settings import MODULE_ROOT
+from minitrino.settings import MODULE_ADMIN
 from minitrino.settings import MODULE_SECURITY
 from minitrino.settings import MODULE_CATALOG
 
 
 class Environment:
     """Provides context and core controls that are globally accessible in
     command scripts. This class should not be instantiated from anywhere but the
@@ -45,15 +46,14 @@
     - `snapshot_dir`: The location of the user's snapshot directory (this is
         essentially a temporary directory, as 'permanent' snapshot tarballs are
         written to the library or user-specified directory).
     - `minitrino_lib_dir`: The location of the Minitrino library."""
 
     @utils.exception_handler
     def __init__(self):
-
         # Attributes that depend on user input prior to being set
         self.verbose = False
         self._user_env = []
 
         self.logger = utils.Logger()
         self.env = EnvironmentVariables
         self.modules = Modules
@@ -180,27 +180,25 @@
                 f"No minitrino.cfg file found at {config_file}. "
                 f"Run 'minitrino config' to reconfigure this file and directory.",
                 level=self.logger.warn,
             )
         return config_file
 
     def _get_docker_clients(self):
-        """Gets DockerClient and APIClient objects. References the DOCKER_HOST
-        variable in `minitrino.cfg` and uses for clients if present. Returns a
-        tuple of DockerClient and APIClient objects, respectiveley.
+        """Gets DockerClient and APIClient objects. Returns a tuple of DockerClient
+        and APIClient objects, respectively.
 
         If there is an error fetching the clients, None types will be returned
         for each client. The lack of clients should be caught by check_daemon()
         calls that execute in each command that requires an accessible Docker
         service."""
 
         try:
-            docker_host = self.env.get_var("DOCKER_HOST", "")
-            docker_client = docker.DockerClient(base_url=docker_host)
-            api_client = docker.APIClient(base_url=docker_host)
+            docker_client = docker.DockerClient(base_url="")
+            api_client = docker.APIClient(base_url="")
             self.docker_client, self.api_client = docker_client, api_client
         except:
             return None, None
 
 
 class EnvironmentVariables:
     """Gathers all Minitrino variables into a single source of truth.
@@ -215,21 +213,20 @@
     ### Public Methods
     - `get_var()`: Gets an environment variable from a specific section and key.
     - `get_section()`: Gets a a section from the environment variable dict.
 
     ### Usage
     ```python
     # ctx object has an instantiated EnvironmentVariables object
-    env_variable = ctx.env.get_var("STARBURST_VER", "354-e")
+    env_variable = ctx.env.get_var("STARBURST_VER", "370-e")
     env_section = ctx.env.get_section("MODULES")
     ```"""
 
     @utils.exception_handler
     def __init__(self, ctx=None):
-
         if not ctx:
             raise utils.handle_missing_param(list(locals().keys()))
 
         self.env = {}
         self._ctx = ctx
 
         self._parse_minitrino_config()
@@ -388,21 +385,18 @@
     - `ctx`: Instantiated Environment object (with user input already accounted
       for).
 
     ### Public Attributes
     - `data`: A dictionary of module information.
 
     ### Public Methods
-    - `get_running_modules()`: Returns a dictionary with the same information as
-      the `modules` attribute, but includes Docker labels and container objects
-      tied to the module."""
+    - `get_running_modules()`: Returns a list of running modules."""
 
     @utils.exception_handler
     def __init__(self, ctx=None):
-
         if not ctx:
             raise utils.handle_missing_param(list(locals().keys()))
 
         self.data = {}
         self._ctx = ctx
         self._load_modules()
 
@@ -412,74 +406,59 @@
 
         utils.check_daemon(self._ctx.docker_client)
         containers = self._ctx.docker_client.containers.list(
             filters={"label": RESOURCE_LABEL}
         )
 
         if not containers:
-            return {}
+            return []
 
-        # Remove Trino container since it isn't a module
-        for i, container in enumerate(containers):
-            if container.name == "trino":
-                del containers[i]
-
-        names = []
-        label_sets = []
-        for i, container in enumerate(containers):
+        modules = []
+        for container in containers:
             label_set = {}
+            ids = ["admin-", "catalog-", "security-"]
             for k, v in container.labels.items():
-                if "catalog-" in v:
-                    names.append(v.lower().strip().replace("catalog-", ""))
-                elif "security-" in v:
-                    names.append(v.lower().strip().replace("security-", ""))
-                else:
-                    continue
-                label_set[k] = v
+                for _id in ids:
+                    if "com.starburst.tests" in k and _id in v:
+                        modules.append(v.lower().strip().replace(_id, ""))
+                        label_set[k] = v
+            # All containers except the trino container must have
+            # module-specific labels. The trino container only has module labels
+            # if a module applies labels to it
             if not label_set and container.name != "trino":
                 raise err.UserError(
                     f"Missing Minitrino labels for container '{container.name}'.",
                     f"Check this module's 'docker-compose.yml' file and ensure you are "
                     f"following the documentation on labels.",
                 )
-            label_sets.append(label_set)
 
-        running = {}
-        for name, label_set, container in zip(names, label_sets, containers):
-            if not isinstance(self.data.get(name), dict):
+        for module in modules:
+            if not isinstance(self.data.get(module), dict):
                 raise err.UserError(
-                    f"Module '{name}' is running, but it is not found "
+                    f"Module '{module}' is running, but it is not found "
                     f"in the library. Was it deleted, or are you pointing "
                     f"Minitrino to the wrong location?"
                 )
-            if not running.get(name, False):
-                running[name] = self.data[name]
-            if not running.get("labels", False):
-                running[name]["labels"] = label_set
-            if not running.get(name).get("containers", False):
-                running[name]["containers"] = [container]
-            else:
-                running[name]["containers"].append(container)
-
-        return running
+        return modules
 
     def _load_modules(self):
         """Loads module data during instantiation."""
 
         self._ctx.logger.log("Loading modules...", level=self._ctx.logger.verbose)
 
         modules_dir = os.path.join(self._ctx.minitrino_lib_dir, MODULE_ROOT)
         if not os.path.isdir(modules_dir):
             raise err.MinitrinoError(
                 f"Path is not a directory: {modules_dir}. "
                 f"Are you pointing to a compatible Minitrino library?"
             )
 
-        # Loop through both catalog and security modules
+        # Loop through all module types
         sections = [
+            os.path.join(modules_dir, MODULE_ADMIN),
             os.path.join(modules_dir, MODULE_CATALOG),
             os.path.join(modules_dir, MODULE_SECURITY),
         ]
 
         for section_dir in sections:
             for _dir in os.listdir(section_dir):
                 module_dir = os.path.join(section_dir, _dir)
@@ -546,15 +525,14 @@
 
     ### Public Methods
     - `execute_commands()`: Executes commands in the user's shell or inside of a
         container."""
 
     @utils.exception_handler
     def __init__(self, ctx=None):
-
         if not ctx:
             raise utils.handle_missing_param(list(locals().keys()))
 
         self._ctx = ctx
 
     def execute_commands(self, *args, **kwargs):
         """Executes commands in the user's shell or inside of a container.
@@ -656,18 +634,19 @@
         container = kwargs.get("container", None)
         if container is None:
             raise err.MinitrinoError(
                 f"Attempted to execute a command inside of a "
                 f"container, but a container object was not provided."
             )
 
-        self._ctx.logger.log(
-            f"Executing command in container '{container.name}':\n{command}",
-            level=self._ctx.logger.verbose,
-        )
+        if not kwargs.get("suppress_output"):
+            self._ctx.logger.log(
+                f"Executing command in container '{container.name}':\n{command}",
+                level=self._ctx.logger.verbose,
+            )
 
         # Create exec handler and execute the command
         exec_handler = self._ctx.api_client.exec_create(
             container.name,
             cmd=command,
             environment=kwargs.get("environment", {}),
             privileged=True,
```

### Comparing `minitrino-2.0.2/minitrino/errors.py` & `minitrino-2.0.3/minitrino/errors.py`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/minitrino/settings.py` & `minitrino-2.0.3/minitrino/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 
 # Generic Constants
 CONTAINER = "container"
 IMAGE = "image"
 VOLUME = "volume"
 LIB = "lib"
 MODULE_ROOT = "modules"
+MODULE_ADMIN = "admin"
 MODULE_CATALOG = "catalog"
 MODULE_SECURITY = "security"
 MODULE_RESOURCES = "resources"
 ETC_TRINO = "/etc/starburst"
+SEP_VOLUME_MOUNT = "${STARBURST_LIC_PATH}:/etc/starburst/starburstdata.license:ro"
 TRINO_CONFIG = "config.properties"
 TRINO_JVM_CONFIG = "jvm.config"
 LIB_INDEPENDENT_CMDS = ["lib_install"]
 
 # Snapshots
 SNAPSHOT_ROOT_FILES = [
     "docker-compose.yml",
@@ -43,42 +45,16 @@
 
 # Templates
 CONFIG_TEMPLATE = """
 [CLI]
 LIB_PATH=
 TEXT_EDITOR=
 
-[DOCKER]
-DOCKER_HOST=
-
-[TRINO]
-CONFIG=
-JVM_CONFIG=
-
 [MODULES]
 STARBURST_LIC_PATH=
-
-S3_ENDPOINT=s3.region.amazonaws.com
-S3_ACCESS_KEY=
-S3_SECRET_KEY=
-AWS_REGION=
-
-SNOWFLAKE_DIST_CONNECT_URL=
-SNOWFLAKE_DIST_CONNECT_USER=
-SNOWFLAKE_DIST_CONNECT_PASSWORD=
-SNOWFLAKE_DIST_WAREHOUSE=
-SNOWFLAKE_DIST_DB=
-SNOWFLAKE_DIST_STAGE_SCHEMA=
-
-SNOWFLAKE_JDBC_CONNECT_URL=
-SNOWFLAKE_JDBC_CONNECT_USER=
-SNOWFLAKE_JDBC_CONNECT_PASSWORD=
-SNOWFLAKE_JDBC_WAREHOUSE=
-SNOWFLAKE_JDBC_DB=
-SNOWFLAKE_JDBC_STAGE_SCHEMA=
 """
 
 PROVISION_SNAPSHOT_TEMPLATE = """
 #!/usr/bin/env bash
 
 # ------------------------------------------------------------------------------------
 # Below is the exact command used to provision the snapshotted environment. Run this
```

### Comparing `minitrino-2.0.2/minitrino/utils.py` & `minitrino-2.0.3/minitrino/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     - `verbose`: Verbose log level.
 
     ### Public Methods
     - `log()`: Logs a message to the user's terminal.
     - `prompt_msg()`: Logs a prompt message and returns the user's input."""
 
     def __init__(self, log_verbose=False):
-
         self.info = {"prefix": "[i]  ", "prefix_color": "cyan"}
         self.warn = {"prefix": "[w]  ", "prefix_color": "yellow"}
         self.error = {"prefix": "[e]  ", "prefix_color": "red"}
         self.verbose = {"prefix": "[i]  ", "prefix_color": "cyan", "verbose": True}
 
         self._log_verbose = log_verbose
 
@@ -242,20 +241,20 @@
 
 def check_starburst_ver(ctx):
     """Checks if a proper Starburst version is provided."""
 
     starburst_ver = ctx.env.get_var("STARBURST_VER", "")
     error_msg = (
         f"Provided Starburst version '{starburst_ver}' is invalid. "
-        f"The provided version must be 354-e or higher."
+        f"The provided version must be 370-e or higher."
     )
 
     try:
         starburst_ver_int = int(starburst_ver[0:3])
-        if starburst_ver_int < 354 or "-e" not in starburst_ver:
+        if starburst_ver_int < 370 or "-e" not in starburst_ver:
             raise err.UserError(error_msg)
     except:
         raise err.UserError(error_msg)
 
 
 def generate_identifier(identifiers=None):
     """Returns an 'object identifier' string used for creating log messages,
@@ -285,15 +284,15 @@
 ):
     """Parses a key-value pair in string form and returns the resulting pair as
     both a 2-element list. If the string cannot be split by "=", a
     MinitrinoError is raised.
 
     ### Parameters
     - `key_value_pair`: A string formatted as a key-value pair, i.e.
-      `"TRINO=354-e"`.
+      `"STARBURST_VER=370-e"`.
     - `err_type`: The exception to raise if an "=" delimiter is not in the
       key-value pair. Defaults to `MinitrinoError`.
     - `key_to_upper`: If `True`, the key will be forced to uppercase.
 
     ### Return Values
     - A list `[k, v]`, but will return `None` if the stripped input is an empty
       string."""
```

### Comparing `minitrino-2.0.2/minitrino.egg-info/SOURCES.txt` & `minitrino-2.0.3/minitrino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minitrino-2.0.2/setup.py` & `minitrino-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 HERE = Path(os.path.abspath(__file__)).resolve().parents[1]
 README = (HERE / "readme.md").read_text()
 
 setup(
     name="minitrino",
-    version="2.0.2",
+    version="2.0.3",
     description="A command line tool that makes it easy to run modular Trino environments locally.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jefflester/minitrino",
     author="Jeff Lester",
     author_email="jeff.lester.dev@gmail.com",
     license="Apache-2.0",
@@ -24,14 +24,14 @@
         "Operating System :: OS Independent",
     ],
     keyword="trino, docker, minitrino",
     python_requires=">=3.8",
     packages=["minitrino", "minitrino.cmd"],
     include_package_data=True,
     install_requires=[
-        "click==7.1.2",
+        "click==8.1.3",
         "colorama",
         "docker==5.0.0",
         "PyYAML",
     ],
     entry_points={"console_scripts": ["minitrino=minitrino.cli:cli"]},
 )
```

