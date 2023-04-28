# Comparing `tmp/zoomaker-0.2.0.tar.gz` & `tmp/zoomaker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.2.0.tar", max compression
+gzip compressed data, was "zoomaker-0.3.0.tar", max compression
```

## Comparing `zoomaker-0.2.0.tar` & `zoomaker-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2542 2023-04-28 06:30:40.762242 zoomaker-0.2.0/README.md
--rw-r--r--   0        0        0      346 2023-04-28 07:23:20.531604 zoomaker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5392 2023-04-28 07:23:35.499196 zoomaker-0.2.0/zoomaker.py
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 zoomaker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5252 2023-04-28 12:07:13.807392 zoomaker-0.3.0/README.md
+-rw-r--r--   0        0        0      416 2023-04-28 13:00:06.190371 zoomaker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6645 2023-04-28 13:00:02.284666 zoomaker-0.3.0/zoomaker.py
+-rw-r--r--   0        0        0     5700 1970-01-01 00:00:00.000000 zoomaker-0.3.0/PKG-INFO
```

### Comparing `zoomaker-0.2.0/zoomaker.py` & `zoomaker-0.3.0/zoomaker.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,34 @@
 from tqdm import tqdm
 
 class Zoomaker:
     def __init__(self, yaml_file: str):
         self.yaml_file = yaml_file
         with open(yaml_file, "r") as f:
             self.data = yaml.safe_load(f)
+        self._check_yaml()
+
+    def _check_yaml(self):
+        if "name" not in self.data:
+            raise Exception("👊 'name' is missing in zoo.yaml")
+        if "resources" not in self.data:
+            raise Exception("👊 'resources' is missing in zoo.yaml")
+        for group, resources in self.data["resources"].items():
+            for resource in resources:
+                if "name" not in resource:
+                    raise Exception("👊 Resource must have 'name' attribute")
+                if "src" not in resource:
+                    raise Exception("👊 Resource must have 'src' attribute")
+                if "type" not in resource:
+                    raise Exception("👊 Resource must have 'type' attribute")
+                if "install_to" not in resource:
+                    raise Exception("👊 Resource must have 'install_to' attribute")
+                type = resource["type"]
+                if type not in ["huggingface", "git", "download"]:
+                    raise Exception(f"👊 Unknown resource type: {type}")
 
     def install(self):
         print(f"👋 -- {self.yaml_file} --")
         print(f"name: {self.data.get('name', 'N/A')}")
         print(f"version: {self.data.get('version', 'N/A')}\n")
         print(f"👇 installing resources ...")
         counter = 0;
@@ -60,29 +80,30 @@
                         if revision:
                             repo.git.checkout(revision)
                             print(f"\tgit checkout revision: {repo.head.object.hexsha}")
                         else:
                             repo.remotes.origin.pull()
                             print(f"\tgit pull latest: {repo.head.object.hexsha}")
                 # Download
-                elif type == "donwload":
+                else:
                     downloaded = self._download_file(src, os.path.join(install_to, os.path.basename(src)))
                     if rename_to:
                         os.rename(downloaded, os.path.join(install_to, rename_to))
                     if revision:
                         print(f"\trevision is not supported for download. Ignoring revision: {revision}")
-                # Unknown
-                else:
-                    print(f"\tUnknown resource type: {type}")
 
-        print(f"\n✅ Installation of {counter} resources completed.")
+        print(f"\n✅ {counter} resources installed.")
 
     def run(self, script_name: str):
         if script_name not in self.data["scripts"]:
-            print(f"No script found with name: {script_name}")
+            print(f"No script found with name: '{script_name}'")
+            if self.data["scripts"]:
+                print(f"\nAvailable scripts:")
+                for script_name in self.data["scripts"]:
+                    print(f"zoomaker run {script_name}")
             return
         script_string = self.data["scripts"][script_name]
         subprocess.check_call(script_string, shell=True)
 
     def _get_repo_name(self, src: str):
         if src.endswith(".git"):
             return os.path.basename(src).replace(".git", "")
@@ -102,18 +123,24 @@
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             print("Error: Failed to download the complete file.")
             return None
         return filename
 
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file")
-    parser.add_argument("command", choices=["install", "run"], help="The command to execute.")
+    parser.add_argument("command", nargs="?", default="help", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.2.0")
-    args = parser.parse_args()
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.3.0")
+
+    # print help if no arguments are provided
+    try:
+        args = parser.parse_args()
+    except:
+        parser.print_help()
+        return
 
     zoomaker = Zoomaker("zoo.yaml")
     if args.command == "install":
         zoomaker.install()
     elif args.command == "run":
         zoomaker.run(args.script)
```

