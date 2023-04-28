# Comparing `tmp/aihandler-1.9.7.tar.gz` & `tmp/aihandler-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.7.tar", last modified: Fri Apr 21 14:54:17 2023, max compression
+gzip compressed data, was "aihandler-1.9.8.tar", last modified: Fri Apr 28 12:51:06 2023, max compression
```

## Comparing `aihandler-1.9.7.tar` & `aihandler-1.9.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 14:54:05.000000 aihandler-1.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 14:54:17.705761 aihandler-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-21 14:54:05.000000 aihandler-1.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:54:17.705761 aihandler-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 14:54:05.000000 aihandler-1.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.701761 aihandler-1.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    54315 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.171291 aihandler-1.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 12:50:52.000000 aihandler-1.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:51:06.171291 aihandler-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-28 12:50:52.000000 aihandler-1.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:51:06.171291 aihandler-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 12:50:52.000000 aihandler-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.167291 aihandler-1.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.167291 aihandler-1.9.8/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54948 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-04-28 12:50:52.000000 aihandler-1.9.8/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:51:06.171291 aihandler-1.9.8/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 12:51:06.000000 aihandler-1.9.8/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.7/LICENSE` & `aihandler-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/PKG-INFO` & `aihandler-1.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.7
+Version: 1.9.8
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.7/README.md` & `aihandler-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/setup.py` & `aihandler-1.9.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "xformers==0.0.18",
     "omegaconf==2.3.0",
     "accelerate==0.18.0",
     "controlnet_aux==0.0.1",
     "huggingface-hub==0.13.3",
     "numpy==1.23.5",
     "Pillow==9.4.0",
-    "pip==23.1.0",
+    "pip==23.1.2",
     "PyQt6==6.4.2",
     "PyQt6-Qt6==6.4.3",
     "PyQt6-sip==13.4.1",
     "pyqtdarktheme==2.1.0",
     "pyre-extensions==0.0.23",
     "lightning==2.0.0",
     "requests==2.28.2",
@@ -37,25 +37,25 @@
     "tqdm==4.65.0",
     "charset-normalizer==3.1.0",
     "opencv-python==4.7.0.72",
     "setuptools==65.5.1",
     "sympy==1.11.1",
     "typing_extensions==4.5.0",
     "urllib3==1.26.15",
-    "diffusers==0.15.1",
+    "diffusers==0.16.0",
     "transformers==4.28.1",
     "compel==1.1.3",
     "sympy==1.11.1",
     "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.7",
+    version="1.9.8",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.7/src/aihandler/base_runner.py` & `aihandler-1.9.8/src/aihandler/base_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,26 @@
     def is_dev_env(self):
         return AIRUNNER_ENVIRONMENT == "dev"
 
     def __init__(self, *args, **kwargs):
         super().__init__()
         logger.set_level(LOG_LEVEL)
         self.app = kwargs.get("app", None)
-        self.settings_manager = SettingsManager(app=self.app)
+        self.settings_manager = kwargs.get("settings_manager", None)
         self._tqdm_var: TQDMVar = kwargs.get("tqdm_var", None)
         self._tqdm_callback = kwargs.get("tqdm_callback", None)
         self._image_var: ImageVar = kwargs.get("image_var", None)
         self._image_handler = kwargs.get("image_handler", None)
         self._error_handler = kwargs.get("error_handler", None)
         self._error_var = kwargs.get("error_var", None)
         self._message_var = kwargs.get("message_var", None)
         self._message_handler = kwargs.get("message_handler", None)
         self.tqdm_callback_signal = pyqtSignal(int, int, str, object, object)
         self.get_extensions_from_url()
-        #self.initialize_active_extensions()
+        self.initialize_active_extensions()
 
     def get_extensions_from_url(self):
         available_extensions = get_extensions_from_url(self)
         self.settings_manager.settings.available_extensions.set(available_extensions)
 
     def initialize_active_extensions(self):
         """
@@ -45,29 +45,25 @@
         or by browsing for them in the extensions menu and activating them there.
 
         This method initializes active extensions.
         :return:
         """
         extensions = []
         available_extensions = self.settings_manager.settings.available_extensions.get()
-        if available_extensions:
-            for extension in available_extensions:
-                if extension.enabled:
-                    repo = extension.repo.get()
-                    name = repo.split("/")[-1]
-                    base_path = self.settings_manager.settings.model_base_path.get()
-                    path = os.path.join(base_path, "extensions", name)
-                    ExtensionClass = import_extension_class(repo, path, "stablediffusion.py", "RunnerExtension")
-                    if ExtensionClass:
-                        extensions.append(ExtensionClass(self.settings_manager))
-
+        enabled_extensions = self.settings_manager.settings.enabled_extensions.get()
+        for extension in available_extensions:
+            if extension.name.get() in enabled_extensions:
+                repo = extension.repo.get()
+                name = repo.split("/")[-1]
+                base_path = self.settings_manager.settings.model_base_path.get()
+                path = os.path.join(base_path, "extensions", name)
+                ExtensionClass = import_extension_class(repo, path, "main.py", "Extension")
+                if ExtensionClass:
+                    extensions.append(ExtensionClass(self.settings_manager))
         self.active_extensions = extensions
-        print("*" * 100)
-        print("EXTENSIONS LOADED: ", extensions)
-        print("*" * 100)
 
     def set_message(self, message):
         if self._message_handler:
             self._message_handler(message)
         elif self._message_var:
             self._message_var.set(message)
```

### Comparing `aihandler-1.9.7/src/aihandler/controlnet_utils.py` & `aihandler-1.9.8/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/database.py` & `aihandler-1.9.8/src/aihandler/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
             else:
                 name_spaced = f"{self.namespace}_{name}"
                 if hasattr(self, name_spaced):
                     return getattr(self, name_spaced)
             raise e
 
     def initialize(self, settings=None):
-        self.settings = settings
         app = self.app
 
         # general settings
         self.nsfw_filter = BooleanVar(app)
         self.nsfw_filter._default = True
         self.allow_hf_downloads = BooleanVar(app)
         self.pixel_mode = BooleanVar(app)
@@ -250,14 +249,15 @@
         self.txt2vid_random_seed = BooleanVar(app)
         self.txt2vid_model_var = StringVar(app, DEFAULT_MODEL)
         self.txt2vid_scheduler_var = StringVar(app, DEFAULT_SCHEDULER)
         self.txt2vid_prompt_triggers = StringVar(app, "")
         self.txt2vid_n_samples = IntVar(app, 1)
 
         self.available_extensions = ListVar(app, [])
+        self.enabled_extensions = ListVar(app, [])
+        self.active_extensions = ListVar(app, [])
 
     def set_namespace(self, namespace):
         self.namespace = namespace
 
     def reset_settings_to_default(self):
         self.initialize()
-
```

### Comparing `aihandler-1.9.7/src/aihandler/llmrunner.py` & `aihandler-1.9.8/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/logger.py` & `aihandler-1.9.8/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/offline_client.py` & `aihandler-1.9.8/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.8/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/qtvar.py` & `aihandler-1.9.8/src/aihandler/qtvar.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,14 +111,22 @@
 class StringVar(Var):
     my_signal = pyqtSignal(str)
 
 
 class ListVar(Var):
     my_signal = pyqtSignal(list)
 
+    def append(self, item):
+        self._my_variable.append(item)
+        self.emit()
+
+    def remove(self, item):
+        self._my_variable.remove(item)
+        self.emit()
+
 
 class DictVar(Var):
     my_signal = pyqtSignal(dict)
 
 
 class DoubleVar(Var):
     my_signal = pyqtSignal(float)
@@ -150,11 +158,11 @@
         self.name.set(name, skip_save=True)
         self.description.set(description, skip_save=True)
         self.repo.set(repo, skip_save=True)
         self.version.set(version, skip_save=True)
         self.reviewed.set(reviewed, skip_save=True)
         self.official.set(official, skip_save=True)
         self.enabled.set(enabled, skip_save=True)
-        self.name.my_signal.connect(self.emit)
+        self.enabled.my_signal.connect(self.emit)
 
     def emit(self):
         self.my_signal.emit(self.name.get(), self.enabled.get() == True)
```

### Comparing `aihandler-1.9.7/src/aihandler/runner.py` & `aihandler-1.9.8/src/aihandler/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -391,29 +391,39 @@
     @property
     def device(self):
         return "cuda" if self.cuda_is_available else "cpu"
 
     @property
     def controlnet_model(self):
         if self.controlnet_type == "canny":
-            return "lllyasviel/sd-controlnet-canny"
+            return "lllyasviel/control_v11p_sd15_canny"
         elif self.controlnet_type == "depth":
-            return "fusing/stable-diffusion-v1-5-controlnet-depth"
-        elif self.controlnet_type == "hed":
-            return "fusing/stable-diffusion-v1-5-controlnet-hed"
+            return "lllyasviel/control_v11f1p_sd15_depth"
         elif self.controlnet_type == "mlsd":
-            return "fusing/stable-diffusion-v1-5-controlnet-mlsd"
+            return "lllyasviel/control_v11p_sd15_mlsd"
         elif self.controlnet_type == "normal":
-            return "fusing/stable-diffusion-v1-5-controlnet-normal"
+            return "lllyasviel/control_v11p_sd15_normalbae"
         elif self.controlnet_type == "scribble":
-            return "fusing/stable-diffusion-v1-5-controlnet-scribble"
+            return "lllyasviel/control_v11p_sd15_scribble"
         elif self.controlnet_type == "segmentation":
-            return "fusing/stable-diffusion-v1-5-controlnet-seg"
+            return "lllyasviel/control_v11p_sd15_seg"
+        elif self.controlnet_type == "lineart":
+            return "lllyasviel/control_v11p_sd15_lineart"
         elif self.controlnet_type == "openpose":
-            return "fusing/stable-diffusion-v1-5-controlnet-openpose"
+            return "lllyasviel/control_v11p_sd15_openpose"
+        elif self.controlnet_type == "softedge":
+            return "lllyasviel/control_v11p_sd15_softedge"
+        elif self.controlnet_type == "pixel2pixel":
+            return "lllyasviel/control_v11e_sd15_ip2p"
+        elif self.controlnet_type == "inpaint":
+            return "lllyasviel/control_v11p_sd15_inpaint"
+        elif self.controlnet_type == "shuffle":
+            return "lllyasviel/control_v11e_sd15_shuffle"
+        elif self.controlnet_type == "anime":
+            return "lllyasviel/control_v11p_sd15s2_lineart_anime"
 
     @property
     def has_internet_connection(self):
         try:
             response = requests.get('https://huggingface.co/')
             return True
         except requests.ConnectionError:
@@ -942,16 +952,16 @@
     def call_pipe_extension(self, **kwargs):
         """
         This calls the call_pipe method on all active extensions
         :param kwargs:
         :return:
         """
         for extension in self.active_extensions:
-            kwargs = extension.call_pipe(self.options, self.model_base_path, self.pipe, **kwargs)
-        return kwargs
+            self.pipe = extension.call_pipe(self.options, self.model_base_path, self.pipe, **kwargs)
+        return self.pipe
 
     def call_pipe(self, **kwargs):
         """
         Generate an image using the pipe
         :param kwargs:
         :return:
         """
@@ -970,22 +980,23 @@
                 negative_prompt_embeds=negative_prompt_embeds,
                 guidance_scale=self.guidance_scale,
                 num_inference_steps=self.num_inference_steps,
                 num_frames=self.batch_size,
                 callback=self.callback,
             )
         else:
-            kwargs = self.call_pipe_extension(**kwargs)
+            self.pipe = self.call_pipe_extension(**kwargs)
             return self.pipe(
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
                 guidance_scale=self.guidance_scale,
                 num_inference_steps=self.num_inference_steps,
                 num_images_per_prompt=1,
                 callback=self.callback,
+                # cross_attention_kwargs={"scale": 0.5},
                 **kwargs
             )
 
     def _preprocess_canny(self, image):
         image = np.array(image)
         low_threshold = 100
         high_threshold = 200
@@ -1135,78 +1146,77 @@
             mask = data["options"]["mask"]
             extra_args["image"] = image
             extra_args["mask_image"] = mask
             extra_args["width"] = self.width
             extra_args["height"] = self.height
 
         # do the sample
-        # try:
-        if self.do_mega_scale:
-            # first we will downscale the original image using the PIL algorithm
-            # called "bicubic" which is a high quality algorithm
-            # then we will upscale the image using the super resolution model
-            # then we will upscale the image using the PIL algorithm called "bicubic"
-            # to the desired size
-            # the new dimensions of scaled_w and scaled_h should be the width and height
-            # of the image that current image but aspect ratio scaled to 128
-            # so if the image is 256x256 then the scaled_w and scaled_h should be 128x128 but
-            # if the image is 512x256 then the scaled_w and scaled_h should be 128x64
-
-            max_in_width = 512
-            scale_size = 256
-            in_width = self.width
-            in_height = self.height
-            original_image_width = data["options"]["original_image_width"]
-            original_image_height = data["options"]["original_image_height"]
-
-            if original_image_width > max_in_width:
-                scale_factor = max_in_width / original_image_width
-                in_width = int(original_image_width * scale_factor)
-                in_height = int(original_image_height * scale_factor)
-                scale_size = int(scale_size * scale_factor)
-
-            if in_width > max_in_width:
-                # scale down in_width and in_height by scale_size
-                # but keep the aspect ratio
-                in_width = scale_size
-                in_height = int((scale_size / original_image_width) * original_image_height)
-
-            # now we will scale the image to the new dimensions
-            # and then upscale it using the super resolution model
-            # and then downscale it using the PIL bicubic algorithm
-            # to the original dimensions
-            # this will give us a high quality image
-            scaled_w = int(in_width * (scale_size / in_height))
-            scaled_h = scale_size
-            downscaled_image = image.resize((scaled_w, scaled_h), Image.BILINEAR)
-            extra_args["image"] = downscaled_image
-            upscaled_image, nsfw_content_detected = self.do_sample(**extra_args)
-            # upscale back to self.width and self.height
-            image = upscaled_image.resize((original_image_width, original_image_height), Image.BILINEAR)
-
-            return image
-        else:
-            image, nsfw_content_detected = self.do_sample(**extra_args)
-        # except Exception as e:
-        #     if "PYTORCH_CUDA_ALLOC_CONF" in str(e):
-        #         raise Exception(self.cuda_error_message)
-        #     elif "`flshattF` is not supported because" in str(e):
-        #         # try again
-        #         logger.info("Disabling xformers and trying again")
-        #         self.pipe.enable_xformers_memory_efficient_attention(
-        #             attention_op=None)
-        #         self.pipe.vae.enable_xformers_memory_efficient_attention(
-        #             attention_op=None)
-        #         # redo the sample with xformers enabled
-        #         return self._sample_diffusers_model(data)
-        #     else:
-        #         if self.is_dev_env:
-        #             traceback.print_exc()
-        #         logger.error("Something went wrong while generating image")
-        #         logger.error(e)
+        try:
+            if self.do_mega_scale:
+                # first we will downscale the original image using the PIL algorithm
+                # called "bicubic" which is a high quality algorithm
+                # then we will upscale the image using the super resolution model
+                # then we will upscale the image using the PIL algorithm called "bicubic"
+                # to the desired size
+                # the new dimensions of scaled_w and scaled_h should be the width and height
+                # of the image that current image but aspect ratio scaled to 128
+                # so if the image is 256x256 then the scaled_w and scaled_h should be 128x128 but
+                # if the image is 512x256 then the scaled_w and scaled_h should be 128x64
+
+                max_in_width = 512
+                scale_size = 256
+                in_width = self.width
+                in_height = self.height
+                original_image_width = data["options"]["original_image_width"]
+                original_image_height = data["options"]["original_image_height"]
+
+                if original_image_width > max_in_width:
+                    scale_factor = max_in_width / original_image_width
+                    in_width = int(original_image_width * scale_factor)
+                    in_height = int(original_image_height * scale_factor)
+                    scale_size = int(scale_size * scale_factor)
+
+                if in_width > max_in_width:
+                    # scale down in_width and in_height by scale_size
+                    # but keep the aspect ratio
+                    in_width = scale_size
+                    in_height = int((scale_size / original_image_width) * original_image_height)
+
+                # now we will scale the image to the new dimensions
+                # and then upscale it using the super resolution model
+                # and then downscale it using the PIL bicubic algorithm
+                # to the original dimensions
+                # this will give us a high quality image
+                scaled_w = int(in_width * (scale_size / in_height))
+                scaled_h = scale_size
+                downscaled_image = image.resize((scaled_w, scaled_h), Image.BILINEAR)
+                extra_args["image"] = downscaled_image
+                upscaled_image, nsfw_content_detected = self.do_sample(**extra_args)
+                # upscale back to self.width and self.height
+                image = upscaled_image.resize((original_image_width, original_image_height), Image.BILINEAR)
+
+                return image
+            else:
+                image, nsfw_content_detected = self.do_sample(**extra_args)
+        except Exception as e:
+            if "PYTORCH_CUDA_ALLOC_CONF" in str(e):
+                raise Exception(self.cuda_error_message)
+            elif "`flshattF` is not supported because" in str(e):
+                # try again
+                logger.info("Disabling xformers and trying again")
+                self.pipe.enable_xformers_memory_efficient_attention(
+                    attention_op=None)
+                self.pipe.vae.enable_xformers_memory_efficient_attention(
+                    attention_op=None)
+                # redo the sample with xformers enabled
+                return self._sample_diffusers_model(data)
+            else:
+                traceback.print_exc()
+                logger.error("Something went wrong while generating image")
+                logger.error(e)
 
         self.final_callback()
 
         return image, nsfw_content_detected
 
     def _blend_images_by_average(self, composite, original):
         # upscale the original image
```

### Comparing `aihandler-1.9.7/src/aihandler/settings.py` & `aihandler-1.9.8/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/socket_server.py` & `aihandler-1.9.8/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler/util.py` & `aihandler-1.9.8/src/aihandler/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,18 +36,16 @@
         print("Unable to load extensions")
     return available_extensions
 
 
 def get_extensions_from_path(path):
     # check for extensions via subfolders under path
     available_extensions = []
-    print("directories", os.listdir(path))
     for f in os.listdir(path):
         if os.path.isdir(os.path.join(path, f)):
-            print("its a dir")
             # build extension details from {path}/setup.py
             try:
                 # read setup.py from the extensions folder
                 with open(os.path.join(path, f, "setup.py"), "r") as setup_file:
                     setup = setup_file.read()
                 # get the name
                 name = setup.split("name=")[1].split(",")[0].replace('"', "").replace("'", "")
@@ -82,29 +80,23 @@
     """
     try:
         # download the extension
         # download the latest release zip and extract it into the extensions folder
         # get the latest release
         repo_name = github_url.split("/")[-1]
         url = f"{github_url}/releases/latest"
-        print("Downloading", url)
         response = requests.get(url)
-        print("Response", response.status_code)
         if response.status_code == 200:
             # get the latest release zip
             latest_release_url = response.url
             # replace "tag" with "tags" in latest_release_url
             latest_release_url = latest_release_url.replace("/releases/tag/", "/archive/refs/tags/")
-            print(response.links)
-            print(response.url)
-            print("Downloading", f"{latest_release_url}.zip")
             response = requests.get(f"{latest_release_url}.zip")
             if response.status_code == 200:
                 # extract the zip into the extensions folder
-                print("Extracting to ", extension_path)
                 with zipfile.ZipFile(io.BytesIO(response.content)) as zip_ref:
                     # extract the contents of zip folder into extension_path + repo_name
                     zip_ref.extractall(extension_path)
                     # the above extracts into extension_path/<repo_name>-<version> but we want
                     # extension_path/<repo_name> so we need to move the contents of the extracted
                     # folder into extension_path/<repo_name>
                     # get the name of the extracted folder
```

### Comparing `aihandler-1.9.7/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.8/src/aihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.7
+Version: 1.9.8
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.7/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.8/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.7/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.8/src/aihandler.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 xformers==0.0.18
 omegaconf==2.3.0
 accelerate==0.18.0
 controlnet_aux==0.0.1
 huggingface-hub==0.13.3
 numpy==1.23.5
 Pillow==9.4.0
-pip==23.1.0
+pip==23.1.2
 PyQt6==6.4.2
 PyQt6-Qt6==6.4.3
 PyQt6-sip==13.4.1
 pyqtdarktheme==2.1.0
 pyre-extensions==0.0.23
 lightning==2.0.0
 requests==2.28.2
@@ -25,12 +25,12 @@
 tqdm==4.65.0
 charset-normalizer==3.1.0
 opencv-python==4.7.0.72
 setuptools==65.5.1
 sympy==1.11.1
 typing_extensions==4.5.0
 urllib3==1.26.15
-diffusers==0.15.1
+diffusers==0.16.0
 transformers==4.28.1
 compel==1.1.3
 sympy==1.11.1
 regex
```

