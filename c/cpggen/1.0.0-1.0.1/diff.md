# Comparing `tmp/cpggen-1.0.0.tar.gz` & `tmp/cpggen-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.0.tar", max compression
+gzip compressed data, was "cpggen-1.0.1.tar", max compression
```

## Comparing `cpggen-1.0.0.tar` & `cpggen-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-22 22:10:12.484381 cpggen-1.0.0/LICENSE
--rw-r--r--   0        0        0     7673 2023-04-22 22:10:12.484381 cpggen-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/__init__.py
--rw-r--r--   0        0        0    13335 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/cli.py
--rw-r--r--   0        0        0    33224 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/logger.py
--rw-r--r--   0        0        0    11219 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-22 22:10:12.488381 cpggen-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 cpggen-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-28 20:14:32.037230 cpggen-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7673 2023-04-28 20:14:32.037230 cpggen-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/__init__.py
+-rw-r--r--   0        0        0    13913 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/cli.py
+-rw-r--r--   0        0        0    33758 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/logger.py
+-rw-r--r--   0        0        0    11219 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-28 20:14:32.037230 cpggen-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 cpggen-1.0.1/PKG-INFO
```

### Comparing `cpggen-1.0.0/LICENSE` & `cpggen-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.0/README.md` & `cpggen-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.0.0/cpggen/cli.py` & `cpggen-1.0.1/cpggen/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         action="store_true",
         default=False,
         dest="server_mode",
         help="Run cpggen as a server",
     )
     parser.add_argument(
         "--server-host",
-        default=os.getenv("CPGGEN_HOST", "127.0.0.1"),
+        default=os.getenv("CPGGEN_HOST", "0.0.0.0"),
         dest="server_host",
         help="cpggen server host",
     )
     parser.add_argument(
         "--server-port",
         default=os.getenv("CPGGEN_PORT", "7072"),
         dest="server_port",
@@ -127,14 +127,21 @@
     parser.add_argument(
         "--verbose",
         action="store_true",
         default=False,
         dest="verbose_mode",
         help="Run cpggen in verbose mode",
     )
+    parser.add_argument(
+        "--skip-sbom",
+        action="store_true",
+        default=True if not os.getenv("SHIFTLEFT_ACCESS_TOKEN") else False,
+        dest="skip_sbom",
+        help="Do not generate SBoM",
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -152,79 +159,93 @@
 
 @app.route("/cpg", methods=["GET", "POST"])
 async def generate_cpg():
     q = request.args
     params = await request.get_json()
     url = ""
     src = ""
-    languages = "autodetect"
+    languages = ""
     cpg_out_dir = None
     is_temp_dir = False
+    app_manifest_list = []
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
-
     if q.get("lang"):
         languages = q.get("lang")
     if not url and params.get("url"):
         url = params.get("url")
     if not src and params.get("src"):
         src = params.get("src")
     if not languages and params.get("lang"):
         languages = params.get("lang")
     if not cpg_out_dir and params.get("out_dir"):
         cpg_out_dir = params.get("out_dir")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
+    # If src contains url, then reassign
+    if not url and (src.startswith("http") or src.startswith("git")):
+        url = src
     if url.startswith("http") or url.startswith("git"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
         src = utils.clone_repo(url, clone_dir)
         is_temp_dir = True
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     for lang in languages:
-        executor.exec_tool(
+        mlist = executor.exec_tool(
             lang,
             src,
             cpg_out_dir,
             src,
             joern_home=os.getenv(
                 "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
             ),
         )
+        if mlist:
+            app_manifest_list += mlist
     if is_temp_dir:
         try:
             os.remove(src)
         except Exception:
             # Ignore cleanup errors
             pass
     return {
         "success": True,
         "message": f"CPG generated successfully at {cpg_out_dir}",
         "out_dir": cpg_out_dir,
+        "app_manifests": app_manifest_list,
     }
 
 
 def init_worker():
     """
     Handler for worker processes to let their parent handle interruptions
     """
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
 
-def cpg(src, cpg_out_dir, languages, joern_home, use_container=False, auto_build=False):
+def cpg(
+    src,
+    cpg_out_dir,
+    languages,
+    joern_home,
+    use_container=False,
+    auto_build=False,
+    skip_sbom=False,
+):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 for lang in languages:
                     LOG.debug(f"Generating CPG for the language {lang} at {src}")
                     pool.apply_async(
                         executor.exec_tool,
@@ -232,15 +253,15 @@
                             lang,
                             src,
                             cpg_out_dir,
                             src,
                             joern_home,
                             use_container,
                             auto_build,
-                            {},
+                            {"skip_sbom": skip_sbom},
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
@@ -376,14 +397,15 @@
     cpg(
         src,
         cpg_out_dir,
         languages,
         joern_home=joern_home,
         use_container=use_container,
         auto_build=args.auto_build,
+        skip_sbom=args.skip_sbom,
     )
     if args.export:
         export_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
```

### Comparing `cpggen-1.0.0/cpggen/executor.py` & `cpggen-1.0.1/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import tempfile
 import zipfile
 from pathlib import Path
 
 import psutil
 from psutil._common import bytes2human
-from rich.progress import Progress
+from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
 from cpggen.logger import DEBUG, LOG, console
 from cpggen.utils import (
     check_command,
     find_csharp_artifacts,
     find_files,
     find_go_mods,
@@ -121,17 +121,20 @@
             value = default_value
         return value
     except Exception:
         return default_value
 
 
 cpg_tools_map = {
-    "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
-    "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
-    "java": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
+    "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
+    "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
+    "java": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "java-with-deps": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "binary": "%(joern_home)sghidra2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
@@ -201,14 +204,15 @@
     "js": "js",
     "ts": "js",
     "javascript": "js",
     "typescript": "js",
     "go": "go",
     "csharp": "csharp",
     "dotnet": "csharp",
+    "cpp": "c",
 }
 
 
 def qwiet_analysis(app_manifest, src, cwd, env):
     try:
         relative_path = os.path.relpath(cwd, src)
         if relative_path and not relative_path.startswith(".."):
@@ -416,14 +420,15 @@
         transient=True,
         redirect_stderr=False,
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
         lang_build_crashes = {}
+        app_manifest_list = []
         if cwd:
             if os.path.isfile(cwd):
                 cwd = os.path.dirname(cwd)
             else:
                 cwd = os.path.abspath(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
@@ -585,15 +590,15 @@
                             if cp.stdout:
                                 LOG.info(cp.stdout)
                             if cp.stderr:
                                 LOG.info("------------------------------")
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
-                                    "Please report the above error to https://github.com/joernio/joern/issues"
+                                    f"Command used {' '.join(cmd_list_with_args)}\nPlease report the above error to https://github.com/joernio/joern/issues"
                                 )
                         else:
                             if os.path.exists(cpg_out_dir):
                                 LOG.info(
                                     f"CPG {src} successfully exported to {cpg_out_dir}"
                                 )
                                 progress.update(
@@ -618,15 +623,15 @@
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
                     )
                 )
                 cwd = amodule
                 if tool_lang in ("binary",):
                     cwd = os.getcwd()
-                if tool_lang != "binary":
+                if tool_lang != "binary" and not extra_args.get("skip_sbom"):
                     # Generate sbom first since this would even download dependencies for java
                     try:
                         progress.update(
                             task,
                             description="Generating SBoM using cdxgen",
                             completed=10,
                             total=100,
@@ -715,14 +720,15 @@
                             "cpg": cpg_out,
                             "sbom": sbom_out,
                             "language": language,
                             "tool_lang": tool_lang,
                             "cpg_frontend_invocation": " ".join(cmd_list_with_args),
                             "sbom_invocation": " ".join(sbom_cmd_list_with_args),
                         }
+                        app_manifest_list.append(app_manifest)
                         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
                             progress.update(
                                 task,
                                 description="Uploading to Qwiet AI for analysis",
                                 completed=90,
                                 total=100,
                             )
@@ -742,7 +748,8 @@
                 progress.update(task, completed=100, total=100)
         except Exception as e:
             if not os.getenv("AT_DEBUG_MODE"):
                 LOG.info(
                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                 )
             LOG.error(e)
+    return app_manifest_list
```

### Comparing `cpggen-1.0.0/cpggen/logger.py` & `cpggen-1.0.1/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.0/cpggen/utils.py` & `cpggen-1.0.1/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.0/pyproject.toml` & `cpggen-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.0"
+version = "1.0.1"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.0/PKG-INFO` & `cpggen-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -59,23 +59,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

