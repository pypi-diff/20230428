# Comparing `tmp/zoomaker-0.1.1.tar.gz` & `tmp/zoomaker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.1.1.tar", max compression
+gzip compressed data, was "zoomaker-0.2.0.tar", max compression
```

## Comparing `zoomaker-0.1.1.tar` & `zoomaker-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2516 2023-04-25 10:26:51.821798 zoomaker-0.1.1/README.md
--rw-r--r--   0        0        0      346 2023-04-25 12:37:05.238936 zoomaker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5410 2023-04-25 12:36:59.947188 zoomaker-0.1.1/zoomaker.py
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 zoomaker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2542 2023-04-28 06:30:40.762242 zoomaker-0.2.0/README.md
+-rw-r--r--   0        0        0      346 2023-04-28 07:23:20.531604 zoomaker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5392 2023-04-28 07:23:35.499196 zoomaker-0.2.0/zoomaker.py
+-rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 zoomaker-0.2.0/PKG-INFO
```

### Comparing `zoomaker-0.1.1/README.md` & `zoomaker-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Work in progress. Please ignore.
 
+?? huggingface-cli login
+
 zoomaker
 ========
 
 Zoomaker is a command-line tool that helps install models, git repositories and run scripts. The information about the resources and scripts to be installed is specified in the `zoo.yaml` file.
 
 ## zoo.yaml example
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4xgfe_4x_/tmppxvdgvqe_TarContainer/0/0.md", line 101, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_4xgfe_4x_/tmppxvdgvqe_TarContainer/0/0.md", line 101, column 0: CDATA terminal not found*

```diff
@@ -1,18 +1,18 @@
-# Work in progress. Please ignore. zoomaker ======== Zoomaker is a command-line
-tool that helps install models, git repositories and run scripts. The
-information about the resources and scripts to be installed is specified in the
-`zoo.yaml` file. ## zoo.yaml example ```yaml name: my-automatic1111-model-zoo
-version: 1.0 description: Lorem ipsum author: your name aliases:
-image_generator: ℑ_generator ./ models: &models ./stable-diffusion-webui/
-models/Stable-diffusion/ controlnet: &controlnet ./stable-diffusion-webui/
-models/ControlNet/ embeddings: &embeddings ./stable-diffusion-webui/embeddings/
-extensions: &extensions ./stable-diffusion-webui/extensions/ resources:
-image_generator: - name: automatic1111 src: https://github.com/AUTOMATIC1111/
-stable-diffusion-webui.git type: git revision:
+# Work in progress. Please ignore. ?? huggingface-cli login zoomaker ========
+Zoomaker is a command-line tool that helps install models, git repositories and
+run scripts. The information about the resources and scripts to be installed is
+specified in the `zoo.yaml` file. ## zoo.yaml example ```yaml name: my-
+automatic1111-model-zoo version: 1.0 description: Lorem ipsum author: your name
+aliases: image_generator: ℑ_generator ./ models: &models ./stable-diffusion-
+webui/models/Stable-diffusion/ controlnet: &controlnet ./stable-diffusion-
+webui/models/ControlNet/ embeddings: &embeddings ./stable-diffusion-webui/
+embeddings/ extensions: &extensions ./stable-diffusion-webui/extensions/
+resources: image_generator: - name: automatic1111 src: https://github.com/
+AUTOMATIC1111/stable-diffusion-webui.git type: git revision:
 22bcc7be428c94e9408f589966c2040187245d81 install_to: *image_generator models: -
 name: v1-5-pruned-emaonly src: runwayml/stable-diffusion-v1-5/v1-5-pruned-
 emaonly.safetensors type: huggingface install_to: *models - name: analog-
 diffusion-v1 src: https://civitai.com/api/download/models/1344 type: donwload
 install_to: *models rename_to: analog-diffusion-v1.safetensors controlnet: -
 name: control_sd15_canny src: lllyasviel/ControlNet/models/
 control_sd15_canny.pth type: huggingface install_to: *controlnet embeddings: -
```

### Comparing `zoomaker-0.1.1/zoomaker.py` & `zoomaker-0.2.0/zoomaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                             repo.git.checkout(revision)
                             print(f"\tgit checkout revision: {repo.head.object.hexsha}")
                         else:
                             repo.remotes.origin.pull()
                             print(f"\tgit pull: {repo.head.object.hexsha}")
                     # new repo
                     else:
-                        repo = git.Repo.clone_from(src, repo_path, no_checkout=True, allow_unsafe_protocols=True, allow_unsafe_options=True)
+                        repo = git.Repo.clone_from(src, repo_path, allow_unsafe_protocols=True, allow_unsafe_options=True)
                         if revision:
                             repo.git.checkout(revision)
                             print(f"\tgit checkout revision: {repo.head.object.hexsha}")
                         else:
                             repo.remotes.origin.pull()
                             print(f"\tgit pull latest: {repo.head.object.hexsha}")
                 # Download
@@ -104,15 +104,15 @@
             return None
         return filename
 
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file")
     parser.add_argument("command", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.1.1")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.2.0")
     args = parser.parse_args()
 
     zoomaker = Zoomaker("zoo.yaml")
     if args.command == "install":
         zoomaker.install()
     elif args.command == "run":
         zoomaker.run(args.script)
```

### Comparing `zoomaker-0.1.1/PKG-INFO` & `zoomaker-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: huggingface-hub (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Work in progress. Please ignore.
 
+?? huggingface-cli login
+
 zoomaker
 ========
 
 Zoomaker is a command-line tool that helps install models, git repositories and run scripts. The information about the resources and scripts to be installed is specified in the `zoo.yaml` file.
 
 ## zoo.yaml example
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4xgfe_4x_/tmppxvdgvqe_TarContainer/0/3", line 116, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_4xgfe_4x_/tmppxvdgvqe_TarContainer/0/3", line 116, column 0: CDATA terminal not found*

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: zoomaker Version: 0.1.1 Summary: Author: Benedikt
+Metadata-Version: 2.1 Name: zoomaker Version: 0.2.0 Summary: Author: Benedikt
 GroÃ Requires-Python: >=3.9,<4.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0) Requires-Dist: huggingface-hub
 (>=0.14.0,<0.15.0) Description-Content-Type: text/markdown # Work in progress.
-Please ignore. zoomaker ======== Zoomaker is a command-line tool that helps
-install models, git repositories and run scripts. The information about the
-resources and scripts to be installed is specified in the `zoo.yaml` file. ##
-zoo.yaml example ```yaml name: my-automatic1111-model-zoo version: 1.0
-description: Lorem ipsum author: your name aliases: image_generator:
-ℑ_generator ./ models: &models ./stable-diffusion-webui/models/Stable-
-diffusion/ controlnet: &controlnet ./stable-diffusion-webui/models/ControlNet/
-embeddings: &embeddings ./stable-diffusion-webui/embeddings/ extensions:
-&extensions ./stable-diffusion-webui/extensions/ resources: image_generator: -
-name: automatic1111 src: https://github.com/AUTOMATIC1111/stable-diffusion-
-webui.git type: git revision: 22bcc7be428c94e9408f589966c2040187245d81
-install_to: *image_generator models: - name: v1-5-pruned-emaonly src: runwayml/
-stable-diffusion-v1-5/v1-5-pruned-emaonly.safetensors type: huggingface
-install_to: *models - name: analog-diffusion-v1 src: https://civitai.com/api/
-download/models/1344 type: donwload install_to: *models rename_to: analog-
-diffusion-v1.safetensors controlnet: - name: control_sd15_canny src:
-lllyasviel/ControlNet/models/control_sd15_canny.pth type: huggingface
-install_to: *controlnet embeddings: - name: midjourney-style src: sd-concepts-
-library/midjourney-style/learned_embeds.bin type: huggingface install_to:
-*embeddings rename_to: midjourney-style.bin - name: moebius src: sd-concepts-
-library/moebius/learned_embeds.bin type: huggingface install_to: *embeddings
-rename_to: moebius.bin extensions: - name: sd-webui-tunnels src: https://
-github.com/Bing-su/sd-webui-tunnels.git type: git install_to: *extensions
-scripts: start: | conda init bash source ~/.bashrc conda activate automatic1111
-cd /home/$(whoami)/stable-diffusion-webui/ ./webui.sh --no-half --listen ``` ##
+Please ignore. ?? huggingface-cli login zoomaker ======== Zoomaker is a
+command-line tool that helps install models, git repositories and run scripts.
+The information about the resources and scripts to be installed is specified in
+the `zoo.yaml` file. ## zoo.yaml example ```yaml name: my-automatic1111-model-
+zoo version: 1.0 description: Lorem ipsum author: your name aliases:
+image_generator: ℑ_generator ./ models: &models ./stable-diffusion-webui/
+models/Stable-diffusion/ controlnet: &controlnet ./stable-diffusion-webui/
+models/ControlNet/ embeddings: &embeddings ./stable-diffusion-webui/embeddings/
+extensions: &extensions ./stable-diffusion-webui/extensions/ resources:
+image_generator: - name: automatic1111 src: https://github.com/AUTOMATIC1111/
+stable-diffusion-webui.git type: git revision:
+22bcc7be428c94e9408f589966c2040187245d81 install_to: *image_generator models: -
+name: v1-5-pruned-emaonly src: runwayml/stable-diffusion-v1-5/v1-5-pruned-
+emaonly.safetensors type: huggingface install_to: *models - name: analog-
+diffusion-v1 src: https://civitai.com/api/download/models/1344 type: donwload
+install_to: *models rename_to: analog-diffusion-v1.safetensors controlnet: -
+name: control_sd15_canny src: lllyasviel/ControlNet/models/
+control_sd15_canny.pth type: huggingface install_to: *controlnet embeddings: -
+name: midjourney-style src: sd-concepts-library/midjourney-style/
+learned_embeds.bin type: huggingface install_to: *embeddings rename_to:
+midjourney-style.bin - name: moebius src: sd-concepts-library/moebius/
+learned_embeds.bin type: huggingface install_to: *embeddings rename_to:
+moebius.bin extensions: - name: sd-webui-tunnels src: https://github.com/Bing-
+su/sd-webui-tunnels.git type: git install_to: *extensions scripts: start: |
+conda init bash source ~/.bashrc conda activate automatic1111 cd /home/$
+(whoami)/stable-diffusion-webui/ ./webui.sh --no-half --listen ``` ##
 Installation ``` pip install zoomaker ``` ## Usage ``` zoomaker
```

