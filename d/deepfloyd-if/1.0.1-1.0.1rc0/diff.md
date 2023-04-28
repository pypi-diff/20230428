# Comparing `tmp/deepfloyd_if-1.0.1.tar.gz` & `tmp/deepfloyd_if-1.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfloyd_if-1.0.1.tar", last modified: Fri Apr 28 12:09:46 2023, max compression
+gzip compressed data, was "deepfloyd_if-1.0.1rc0.tar", last modified: Thu Apr 27 14:48:49 2023, max compression
```

## Comparing `deepfloyd_if-1.0.1.tar` & `deepfloyd_if-1.0.1rc0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.580153 deepfloyd_if-1.0.1/
--rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-1.0.1/LICENSE
--rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/LICENSE-MODEL
--rw-r--r--   0 shonenkov   (501) staff       (20)    14980 2023-04-28 12:09:46.580239 deepfloyd_if-1.0.1/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)    14732 2023-04-28 12:07:04.000000 deepfloyd_if-1.0.1/README.md
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.560388 deepfloyd_if-1.0.1/deepfloyd_if/
--rw-r--r--   0 shonenkov   (501) staff       (20)       48 2023-04-28 12:07:04.000000 deepfloyd_if-1.0.1/deepfloyd_if/__init__.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.575012 deepfloyd_if-1.0.1/deepfloyd_if/model/
--rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/gaussian_diffusion.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/losses.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/nn.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/resample.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/respace.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-1.0.1/deepfloyd_if/model/unet.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.577022 deepfloyd_if-1.0.1/deepfloyd_if/modules/
--rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/base.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-27 14:00:15.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_I.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_II.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_III.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_III_sd_x4.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     9421 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/t5.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1/deepfloyd_if/modules/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.578047 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/
--rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/__init__.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/dream.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/inpainting.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/style_transfer.py
--rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/super_resolution.py
--rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-1.0.1/deepfloyd_if/pipelines/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.578816 deepfloyd_if-1.0.1/deepfloyd_if/resources/
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1/deepfloyd_if/resources/p_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1/deepfloyd_if/resources/w_head_v1.npz
--rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-1.0.1/deepfloyd_if/resources/wm.png
--rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
--rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1/deepfloyd_if/utils.py
-drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-28 12:09:46.573495 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/
--rw-r--r--   0 shonenkov   (501) staff       (20)    14980 2023-04-28 12:09:46.000000 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/PKG-INFO
--rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-28 12:09:46.000000 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/SOURCES.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)        1 2023-04-28 12:09:46.000000 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/dependency_links.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-28 12:09:46.000000 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/requires.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-28 12:09:46.000000 deepfloyd_if-1.0.1/deepfloyd_if.egg-info/top_level.txt
--rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-28 12:09:46.580838 deepfloyd_if-1.0.1/setup.cfg
--rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1/setup.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.164382 deepfloyd_if-1.0.1rc0/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1504 2023-04-26 14:57:02.000000 deepfloyd_if-1.0.1rc0/LICENSE
+-rw-r--r--   0 shonenkov   (501) staff       (20)    11615 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/LICENSE-MODEL
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14255 2023-04-27 14:48:49.164502 deepfloyd_if-1.0.1rc0/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14004 2023-04-27 14:00:43.000000 deepfloyd_if-1.0.1rc0/README.md
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.153882 deepfloyd_if-1.0.1rc0/deepfloyd_if/
+-rw-r--r--   0 shonenkov   (501) staff       (20)       50 2023-04-27 13:01:50.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/__init__.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.157235 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      118 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    35223 2023-03-09 17:58:29.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/gaussian_diffusion.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2587 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/losses.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5965 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/nn.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2001 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/resample.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     6379 2023-01-10 14:02:27.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/respace.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    27952 2023-01-28 11:21:37.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/model/unet.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.159932 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      321 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)    15411 2023-04-26 15:11:36.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/base.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1977 2023-04-27 14:00:15.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_I.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1939 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_II.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1962 2023-04-17 00:13:08.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3126 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III_sd_x4.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     9421 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/t5.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      742 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.161469 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/
+-rw-r--r--   0 shonenkov   (501) staff       (20)      247 2023-03-19 16:24:39.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/__init__.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     5565 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/dream.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4522 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/inpainting.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     4443 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/style_transfer.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1722 2023-04-26 16:50:32.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/super_resolution.py
+-rw-r--r--   0 shonenkov   (501) staff       (20)      709 2023-03-18 20:13:21.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.162582 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/p_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)     3588 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/w_head_v1.npz
+-rw-r--r--   0 shonenkov   (501) staff       (20)      947 2023-01-12 23:07:13.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/wm.png
+-rw-r--r--   0 shonenkov   (501) staff       (20)   630912 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2390 2022-12-21 22:31:58.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if/utils.py
+drwxr-xr-x   0 shonenkov   (501) staff       (20)        0 2023-04-27 14:48:49.154763 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/
+-rw-r--r--   0 shonenkov   (501) staff       (20)    14255 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/PKG-INFO
+-rw-r--r--   0 shonenkov   (501) staff       (20)     1123 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/SOURCES.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)        1 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/dependency_links.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      228 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/requires.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)       99 2023-04-27 14:48:49.000000 deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/top_level.txt
+-rw-r--r--   0 shonenkov   (501) staff       (20)      281 2023-04-27 14:48:49.165027 deepfloyd_if-1.0.1rc0/setup.cfg
+-rw-r--r--   0 shonenkov   (501) staff       (20)     2018 2023-04-06 21:54:11.000000 deepfloyd_if-1.0.1rc0/setup.py
```

### Comparing `deepfloyd_if-1.0.1/LICENSE` & `deepfloyd_if-1.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/LICENSE-MODEL` & `deepfloyd_if-1.0.1rc0/LICENSE-MODEL`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/PKG-INFO` & `deepfloyd_if-1.0.1rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfloyd_if
-Version: 1.0.1
+Version: 1.0.1rc0
 Summary: DeepFloyd-IF (Imagen Free)
 Author: DeepFloyd, StabilityAI
 Author-email: shonenkov@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-MODEL
 
@@ -33,26 +33,22 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1
+pip install deepfloyd_if==1.0.1rc
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebooks
-[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb)
-[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
-
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb).
-
+## Local notebook and UI demo
 
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -135,15 +131,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -322,16 +318,14 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
-**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
-
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
 - [Alex Shonenkov](https://github.com/shonenkov)
@@ -349,8 +343,8 @@
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1/README.md` & `deepfloyd_if-1.0.1rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,22 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1
+pip install deepfloyd_if==1.0.1rc
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebooks
-[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb)
-[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
-
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb).
-
+## Local notebook and UI demo
 
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -125,15 +121,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -312,16 +308,14 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
-**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
-
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
 - [Alex Shonenkov](https://github.com/shonenkov)
@@ -339,8 +333,8 @@
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/gaussian_diffusion.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/losses.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/losses.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/nn.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/nn.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/resample.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/resample.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/respace.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/respace.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/model/unet.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/model/unet.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/base.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/base.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_I.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_I.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_II.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_II.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_III.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/stage_III_sd_x4.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/stage_III_sd_x4.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/t5.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/t5.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/modules/utils.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/modules/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/pipelines/dream.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/dream.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/pipelines/inpainting.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/inpainting.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/pipelines/style_transfer.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/style_transfer.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/pipelines/super_resolution.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/super_resolution.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/pipelines/utils.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/resources/p_head_v1.npz` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/p_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/resources/w_head_v1.npz` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/w_head_v1.npz`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/resources/wm.png` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/wm.png`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/resources/zero_t5-v1_1-xxl_vector.npy`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if/utils.py` & `deepfloyd_if-1.0.1rc0/deepfloyd_if/utils.py`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if.egg-info/PKG-INFO` & `deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfloyd-if
-Version: 1.0.1
+Version: 1.0.1rc0
 Summary: DeepFloyd-IF (Imagen Free)
 Author: DeepFloyd, StabilityAI
 Author-email: shonenkov@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-MODEL
 
@@ -33,26 +33,22 @@
 
 
 ## Quick Start
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/deepfloyd_if_free_tier_google_colab.ipynb)
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/DeepFloyd/IF)
 
 ```shell
-pip install deepfloyd_if==1.0.1
+pip install deepfloyd_if==1.0.1rc
 pip install xformers==0.0.16
 pip install git+https://github.com/openai/CLIP.git --no-deps
 ```
 
-## Local notebooks
-[![Jupyter Notebook](https://img.shields.io/badge/jupyter_notebook-%23FF7A01.svg?logo=jupyter&logoColor=white)](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb)
-[![Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/shonenkov/deepfloyd-if-4-3b-generator-of-pictures)
-
-The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable in a Jupyter Notebook [here](https://huggingface.co/DeepFloyd/IF-I-XL-v1.0/blob/main/notebooks/pipes-DeepFloyd-IF-v1.0.ipynb).
-
+## Local notebook and UI demo
 
+The Dream, Style Transfer, Super Resolution or Inpainting modes are avaliable as in a Jupyter Notebook at `IF/notebooks/pipes-DeepFloyd-IF.ipynb`.
 
 ## Integration with 🤗 Diffusers
 
 IF is also integrated with the 🤗 Hugging Face [Diffusers library](https://github.com/huggingface/diffusers/).
 
 Diffusers runs each stage individually allowing the user to customize the image generation process as well as allowing to inspect intermediate results easily.
 
@@ -135,15 +131,15 @@
 ```
 
  There are multiple ways to speed up the inference time and lower the memory consumption even more with `diffusers`. To do so, please have a look at the Diffusers docs:
 
 - 🚀 [Optimizing for inference time](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-speed)
 - ⚙️ [Optimizing for low memory during inference](https://huggingface.co/docs/diffusers/api/pipelines/if#optimizing-for-memory)
 
-For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) and [the documentation](https://huggingface.co/docs/diffusers/main/en/api/pipelines/if) 📖.
+For more in-detail information about how to use IF, please have a look at [the IF blog post](https://huggingface.co/blog/if) 📖.
 
 ## Run the code locally
 
 ### Loading the models into VRAM
 
 ```python
 from deepfloyd_if.modules import IFStageI, IFStageII, StableStageIII
@@ -322,16 +318,14 @@
 
 ## License
 
 The code in this repository is released under the bespoke license (see added [point two](https://github.com/deep-floyd/IF/blob/main/LICENSE#L13)).
 
 The weights will be available soon via [the DeepFloyd organization at Hugging Face](https://huggingface.co/DeepFloyd) and have their own LICENSE.
 
-**Disclaimer:** *The initial release of the IF model is under a restricted research-purposes-only license temporarily to gather feedback, and after that we intend to release a fully open-source model in line with other Stability AI models.*
-
 ## Limitations and Biases
 
 The models available in this codebase have known limitations and biases. Please refer to [the model card](https://huggingface.co/DeepFloyd/IF-I-L-v1.0) for more information.
 
 
 ## 🎓 DeepFloyd IF creators:
 - [Alex Shonenkov](https://github.com/shonenkov)
@@ -349,8 +343,8 @@
 
 ## 🚀 External Contributors 🚀
 - The Biggest Thanks [@Apolinário](https://github.com/apolinario), for ideas, consultations, help and support on all stages to make IF available in open-source; for writing a lot of documentation and instructions; for creating a friendly atmosphere in difficult moments 🦉;
 - Thanks, [@patrickvonplaten](https://github.com/patrickvonplaten), for improving loading time of unet models by 80%;
 for integration Stable-Diffusion-x4 as native pipeline 💪;
 - Thanks, [@williamberman](https://github.com/williamberman) and [@patrickvonplaten](https://github.com/patrickvonplaten) for diffusers integration 🙌;
 - Thanks, [@hysts](https://github.com/hysts) and [@Apolinário](https://github.com/apolinario) for creating [the best gradio demo with IF](https://huggingface.co/spaces/DeepFloyd/IF) 🚀;
-- Thanks, [@Dango233](https://github.com/Dango233), for adapting IF with xformers memory efficient attention 💪;
+- Thanks, [@Dango233](https://github.com/Dango233), for adaptation IF with xformers memory efficient attention 💪;
```

### Comparing `deepfloyd_if-1.0.1/deepfloyd_if.egg-info/SOURCES.txt` & `deepfloyd_if-1.0.1rc0/deepfloyd_if.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepfloyd_if-1.0.1/setup.py` & `deepfloyd_if-1.0.1rc0/setup.py`

 * *Files identical despite different names*

