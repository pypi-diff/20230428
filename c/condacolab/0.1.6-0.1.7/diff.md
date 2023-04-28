# Comparing `tmp/condacolab-0.1.6.tar.gz` & `tmp/condacolab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condacolab-0.1.6.tar", max compression
+gzip compressed data, was "condacolab-0.1.7.tar", max compression
```

## Comparing `condacolab-0.1.6.tar` & `condacolab-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2021-06-30 10:11:56.362416 condacolab-0.1.6/LICENSE
--rw-r--r--   0        0        0     5079 2023-03-14 11:45:08.510576 condacolab-0.1.6/README.md
--rw-r--r--   0        0        0    11041 2023-03-14 11:45:11.889510 condacolab-0.1.6/condacolab.py
--rw-r--r--   0        0        0      471 2023-03-14 11:45:11.889969 condacolab-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5732 2023-03-14 11:46:31.341357 condacolab-0.1.6/setup.py
--rw-r--r--   0        0        0     5719 2023-03-14 11:46:31.341554 condacolab-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-06-30 10:11:56.362416 condacolab-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4969 2023-04-28 15:41:31.296851 condacolab-0.1.7/README.md
+-rw-r--r--   0        0        0    11809 2023-04-28 15:41:31.297352 condacolab-0.1.7/condacolab.py
+-rw-r--r--   0        0        0      472 2023-04-28 15:41:31.297656 condacolab-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5621 2023-04-28 15:42:45.463539 condacolab-0.1.7/setup.py
+-rw-r--r--   0        0        0     5459 2023-04-28 15:42:45.463778 condacolab-0.1.7/PKG-INFO
```

### Comparing `condacolab-0.1.6/LICENSE` & `condacolab-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `condacolab-0.1.6/README.md` & `condacolab-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: condacolab
+Version: 0.1.7
+Summary: Install Conda and friends on Google Colab, easily
+Home-page: https://github.com/jaimergp/condacolab
+License: MIT
+Author: Jaime Rodríguez-Guerra
+Author-email: jaimergp@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Project-URL: Repository, https://github.com/jaimergp/condacolab
+Description-Content-Type: text/markdown
+
 # condacolab
 
 [![Downloads](https://pepy.tech/badge/condacolab/week)](https://pypi.org/project/condacolab)
 [![Downloads](https://pepy.tech/badge/condacolab/month)](https://pypi.org/project/condacolab)
 [![Downloads](https://pepy.tech/badge/condacolab)](https://pypi.org/project/condacolab)
 
 Install Conda and friends on Google Colab, easily.
@@ -27,19 +41,19 @@
 condacolab.check()
 ```
 
 > It is important that you perform the installation first thing in the notebook because it will require a kernel restart, thus resetting the variables set up to that point.
 
 The default `condacolab.install()` provides Mambaforge, but there are other `conda` distributions to choose from:
 
-- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.9. Unlike Anaconda, this distribution only contains `python` and `conda`.
-- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it's built for Python 3.9.
-- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it's built for Python 3.9.
+- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.10. Unlike Anaconda, this distribution only contains `python` and `conda`.
+- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).
+- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).
 
-For advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.9 distribution that fulfills your own needs.
+For advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.10 distribution that fulfills your own needs.
 
 > If you want to build your own `constructor`-based installer, check the FAQ below!
 
 Once the installation is done, you can use `conda` and/or `mamba` to install the needed packages:
 
 ```bash
 !conda install openmm
@@ -57,21 +71,21 @@
 !mamba env update -n base -f environment.yml
 ```
 
 
 ## Shortcomings
 
 - The Python kernel needs to be restarted for changes to be applied. This happens automatically. If you are wondering why you are seeing a message saying _"Your session crashed for an unknown reason"_, this is why. You can safely ignore this message!
-- You can only use the `base` environment, so do not try to create more environments with `conda create`.
+- You can only use the `base` environment, so do not try to create more environments with `conda create`. If you have an environment file, use `conda env update -n base -f <your-file.yml>`.
 
 ## FAQ
 
 ### How does it work?
 
-Google Colab runs on Python 3.9. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.9 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.
+Google Colab runs on Python 3.10. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.10 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.
 
 ### How can I cache my installation? I don't want to wait every time I start Colab.
 
 The recommended approach is to build your own `constructor`-based installer. We have provided an example in `constructor-example/construct.yaml`.
 
 > You can generate a `constructor` installer on Colab too! Follow [this tutorial](https://colab.research.google.com/github/jaimergp/condacolab/blob/main/constructor-example/condacolab_constructor_tutorial.ipynb).
 
@@ -100,7 +114,8 @@
 condacolab.install_from_url(URL_TO_YOUR_CUSTOM_CONSTRUCTOR_INSTALLER)
 ```
 
 ## Can I install R packages?
 
 Yes, as long as you make sure you also install `rpy2` to overwrite Colab's installation.
 See [issue #26](https://github.com/conda-incubator/condacolab/issues/26) for more details.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `condacolab-0.1.6/condacolab.py` & `condacolab-0.1.7/condacolab.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 >>> import condacolab
 >>> condacolab.install()
 
 For more details, check the docstrings for ``install_from_url()``.
 """
 
+import hashlib
 import os
 import sys
 import shutil
 from datetime import datetime, timedelta
 from pathlib import Path
 from subprocess import run, PIPE, STDOUT
 from typing import Dict, AnyStr
@@ -24,26 +25,35 @@
 
 try:
     import google.colab
 except ImportError:
     raise RuntimeError("This module must ONLY run as part of a Colab notebook!")
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __author__ = "Jaime Rodríguez-Guerra <jaimergp@users.noreply.github.com>"
 
 
 PREFIX = "/usr/local"
 
 
+def _chunked_sha256(path, chunksize=1_048_576):
+    hasher = hashlib.sha256()
+    with open(path, "rb") as f:
+        while (chunk := f.read(chunksize)):
+            hasher.update(chunk)
+    return hasher.hexdigest()
+
+
 def install_from_url(
     installer_url: AnyStr,
     prefix: os.PathLike = PREFIX,
     env: Dict[AnyStr, AnyStr] = None,
     run_checks: bool = True,
+    sha256: AnyStr = None,
 ):
     """
     Download and run a constructor-like installer, patching
     the necessary bits so it works on Colab right away.
 
     This will restart your kernel as a result!
 
@@ -64,27 +74,33 @@
         For example, a value with spaces should be passed as::
 
             env={"VAR": '"a value with spaces"'}
     run_checks
         Run checks to see if installation was run previously.
         Change to False to ignore checks and always attempt
         to run the installation.
+    sha256
+        Expected SHA256 checksum of the installer. Optional.
     """
     if run_checks:
         try:  # run checks to see if it this was run already
             return check(prefix)
         except AssertionError:
             pass  # just install
 
     t0 = datetime.now()
     print(f"⏬ Downloading {installer_url}...")
     installer_fn = "__installer__.sh"
     with urlopen(installer_url) as response, open(installer_fn, "wb") as out:
         shutil.copyfileobj(response, out)
 
+    if sha256 is not None:
+        digest = _chunked_sha256(installer_fn)
+        assert digest == sha256, f"💥💔💥 Checksum failed! Expected {sha256}, got {digest}"
+
     print("📦 Installing...")
     task = run(
         ["bash", installer_fn, "-bfp", str(prefix)],
         check=False,
         stdout=PIPE,
         stderr=STDOUT,
         text=True,
@@ -146,22 +162,20 @@
     get_ipython().kernel.do_shutdown(True)
 
 
 def install_mambaforge(
     prefix: os.PathLike = PREFIX, env: Dict[AnyStr, AnyStr] = None, run_checks: bool = True
 ):
     """
-    Install Mambaforge, built for Python 3.9.
+    Install Mambaforge, built for Python 3.10.
 
     Mambaforge consists of a Miniconda-like distribution optimized
     and preconfigured for conda-forge packages, and includes ``mamba``,
     a faster ``conda`` implementation.
 
-    Unlike the official Miniconda, this is built with the latest ``conda``.
-
     Parameters
     ----------
     prefix
         Target location for the installation
     env
         Environment variables to inject in the kernel restart.
         We *need* to inject ``LD_LIBRARY_PATH`` so ``{PREFIX}/lib``
@@ -173,33 +187,32 @@
 
             env={"VAR": '"a value with spaces"'}
     run_checks
         Run checks to see if installation was run previously.
         Change to False to ignore checks and always attempt
         to run the installation.
     """
-    installer_url = r"https://github.com/jaimergp/miniforge/releases/latest/download/Mambaforge-colab-Linux-x86_64.sh"
-    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks)
+    installer_url = "https://github.com/conda-forge/miniforge/releases/download/23.1.0-1/Mambaforge-23.1.0-1-Linux-x86_64.sh"
+    checksum = "cfb16c47dc2d115c8b114280aa605e322173f029fdb847a45348bf4bd23c62ab"
+    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks, sha256=checksum)
 
 
 # Make mambaforge the default
 install = install_mambaforge
 
 
 def install_miniforge(
     prefix: os.PathLike = PREFIX, env: Dict[AnyStr, AnyStr] = None, run_checks: bool = True
 ):
     """
-    Install Miniforge, built for Python 3.9.
+    Install Miniforge, built for Python 3.10.
 
     Miniforge consists of a Miniconda-like distribution optimized
     and preconfigured for conda-forge packages.
 
-    Unlike the official Miniconda, this is built with the latest ``conda``.
-
     Parameters
     ----------
     prefix
         Target location for the installation
     env
         Environment variables to inject in the kernel restart.
         We *need* to inject ``LD_LIBRARY_PATH`` so ``{PREFIX}/lib``
@@ -211,23 +224,24 @@
 
             env={"VAR": '"a value with spaces"'}
     run_checks
         Run checks to see if installation was run previously.
         Change to False to ignore checks and always attempt
         to run the installation.
     """
-    installer_url = r"https://github.com/jaimergp/miniforge/releases/latest/download/Miniforge-colab-Linux-x86_64.sh"
-    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks)
+    installer_url = "https://github.com/conda-forge/miniforge/releases/download/23.1.0-1/Miniforge3-23.1.0-1-Linux-x86_64.sh"
+    checksum = "7a5859e873ed36fc9a141fff0ac60e133b971b3413aed49a4c82693d4f4a2ad2"
+    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks, sha256=checksum)
 
 
 def install_miniconda(
     prefix: os.PathLike = PREFIX, env: Dict[AnyStr, AnyStr] = None, run_checks: bool = True
 ):
     """
-    Install Miniconda 23.1.0 for Python 3.9.
+    Install Miniconda 23.1.0 for Python 3.10.
 
     Parameters
     ----------
     prefix
         Target location for the installation
     env
         Environment variables to inject in the kernel restart.
@@ -240,24 +254,25 @@
 
             env={"VAR": '"a value with spaces"'}
     run_checks
         Run checks to see if installation was run previously.
         Change to False to ignore checks and always attempt
         to run the installation.
     """
-    installer_url = r"https://repo.anaconda.com/miniconda/Miniconda3-py39_23.1.0-1-Linux-x86_64.sh"
-    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks)
+    installer_url = "https://repo.anaconda.com/miniconda/Miniconda3-py310_23.3.1-0-Linux-x86_64.sh"
+    checksum = "aef279d6baea7f67940f16aad17ebe5f6aac97487c7c03466ff01f4819e5a651"
+    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks, sha256=checksum)
 
 
 def install_anaconda(
     prefix: os.PathLike = PREFIX, env: Dict[AnyStr, AnyStr] = None, run_checks: bool = True
 ):
     """
-    Install Anaconda 2022.10, the latest version built
-    for Python 3.9 at the time of update.
+    Install Anaconda 2023.03, the latest version built
+    for Python 3.10 at the time of update.
 
     Parameters
     ----------
     prefix
         Target location for the installation
     env
         Environment variables to inject in the kernel restart.
@@ -270,16 +285,17 @@
 
             env={"VAR": '"a value with spaces"'}
     run_checks
         Run checks to see if installation was run previously.
         Change to False to ignore checks and always attempt
         to run the installation.
     """
-    installer_url = r"https://repo.anaconda.com/archive/Anaconda3-2022.10-Linux-x86_64.sh"
-    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks)
+    installer_url = "https://repo.anaconda.com/archive/Anaconda3-2023.03-1-Linux-x86_64.sh"
+    checksum = "95102d7c732411f1458a20bdf47e4c1b0b6c8a21a2edfe4052ca370aaae57bab"
+    install_from_url(installer_url, prefix=prefix, env=env, run_checks=run_checks, sha256=checksum)
 
 
 def check(prefix: os.PathLike = PREFIX, verbose: bool = True):
     """
     Run some basic checks to ensure that ``conda`` has been installed
     correctly
```

### Comparing `condacolab-0.1.6/setup.py` & `condacolab-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['condacolab']
 setup_kwargs = {
     'name': 'condacolab',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Install Conda and friends on Google Colab, easily',
-    'long_description': '# condacolab\n\n[![Downloads](https://pepy.tech/badge/condacolab/week)](https://pypi.org/project/condacolab)\n[![Downloads](https://pepy.tech/badge/condacolab/month)](https://pypi.org/project/condacolab)\n[![Downloads](https://pepy.tech/badge/condacolab)](https://pypi.org/project/condacolab)\n\nInstall Conda and friends on Google Colab, easily.\n\n![CondaColab](https://github.com/jaimergp/condacolab/raw/main/condacolab.png)\n\n## Usage\n\n> **TLDR**: Check the [example notebook here](https://colab.research.google.com/drive/1c_RGCgQeLHVXlF44LyOFjfUW32CmG6BP)!\n\nOn your Colab notebook, run the following code as the _first executable cell_:\n\n```python\n!pip install -q condacolab\nimport condacolab\ncondacolab.install()\n```\n\nAfter the kernel restart, you can optionally add a new cell to check that everything is in place:\n\n```python\nimport condacolab\ncondacolab.check()\n```\n\n> It is important that you perform the installation first thing in the notebook because it will require a kernel restart, thus resetting the variables set up to that point.\n\nThe default `condacolab.install()` provides Mambaforge, but there are other `conda` distributions to choose from:\n\n- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.9. Unlike Anaconda, this distribution only contains `python` and `conda`.\n- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it\'s built for Python 3.9.\n- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it\'s built for Python 3.9.\n\nFor advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.9 distribution that fulfills your own needs.\n\n> If you want to build your own `constructor`-based installer, check the FAQ below!\n\nOnce the installation is done, you can use `conda` and/or `mamba` to install the needed packages:\n\n```bash\n!conda install openmm\n\n# or, faster:\n!mamba install openmm\n```\n\nIf you have a environment file (e.g. `environment.yml`), you can use it like this:\n\n```bash\n!conda env update -n base -f environment.yml\n\n# or, faster:\n!mamba env update -n base -f environment.yml\n```\n\n\n## Shortcomings\n\n- The Python kernel needs to be restarted for changes to be applied. This happens automatically. If you are wondering why you are seeing a message saying _"Your session crashed for an unknown reason"_, this is why. You can safely ignore this message!\n- You can only use the `base` environment, so do not try to create more environments with `conda create`.\n\n## FAQ\n\n### How does it work?\n\nGoogle Colab runs on Python 3.9. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.9 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.\n\n### How can I cache my installation? I don\'t want to wait every time I start Colab.\n\nThe recommended approach is to build your own `constructor`-based installer. We have provided an example in `constructor-example/construct.yaml`.\n\n> You can generate a `constructor` installer on Colab too! Follow [this tutorial](https://colab.research.google.com/github/jaimergp/condacolab/blob/main/constructor-example/condacolab_constructor_tutorial.ipynb).\n\nLocally, follow these steps:\n\n1. In your local computer:\n\n```bash\nconda create -n constructor -c conda-forge constructor\nconda activate constructor\nmkdir my-installer\ncd my-installer\ncurl -sLO https://raw.githubusercontent.com/jaimergp/condacolab/main/constructor-example/construct.yaml\ncurl -sLO https://raw.githubusercontent.com/jaimergp/condacolab/main/constructor-example/pip-dependencies.sh\n```\n\n2. Add your `conda` packages to `construct.yaml` in the `specs` section. Read the comments to respect the constrains already present! You can also adapt the metadata to your liking.\n3. If you _do_ need to install `pip` requirements, uncomment the `post_install` line and edit `pip-dependencies.sh`.\n4. Run `constructor --platform linux-64 .`\n5. Upload the resulting `.sh` to an online location with a permanent URL. GitHub Releases is great for this!\n6. In Colab, run:\n\n```python\n!pip install -q condacolab\nimport condacolab\ncondacolab.install_from_url(URL_TO_YOUR_CUSTOM_CONSTRUCTOR_INSTALLER)\n```\n\n## Can I install R packages?\n\nYes, as long as you make sure you also install `rpy2` to overwrite Colab\'s installation.\nSee [issue #26](https://github.com/conda-incubator/condacolab/issues/26) for more details.\n',
+    'long_description': '# condacolab\n\n[![Downloads](https://pepy.tech/badge/condacolab/week)](https://pypi.org/project/condacolab)\n[![Downloads](https://pepy.tech/badge/condacolab/month)](https://pypi.org/project/condacolab)\n[![Downloads](https://pepy.tech/badge/condacolab)](https://pypi.org/project/condacolab)\n\nInstall Conda and friends on Google Colab, easily.\n\n![CondaColab](https://github.com/jaimergp/condacolab/raw/main/condacolab.png)\n\n## Usage\n\n> **TLDR**: Check the [example notebook here](https://colab.research.google.com/drive/1c_RGCgQeLHVXlF44LyOFjfUW32CmG6BP)!\n\nOn your Colab notebook, run the following code as the _first executable cell_:\n\n```python\n!pip install -q condacolab\nimport condacolab\ncondacolab.install()\n```\n\nAfter the kernel restart, you can optionally add a new cell to check that everything is in place:\n\n```python\nimport condacolab\ncondacolab.check()\n```\n\n> It is important that you perform the installation first thing in the notebook because it will require a kernel restart, thus resetting the variables set up to that point.\n\nThe default `condacolab.install()` provides Mambaforge, but there are other `conda` distributions to choose from:\n\n- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.10. Unlike Anaconda, this distribution only contains `python` and `conda`.\n- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).\n- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).\n\nFor advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.10 distribution that fulfills your own needs.\n\n> If you want to build your own `constructor`-based installer, check the FAQ below!\n\nOnce the installation is done, you can use `conda` and/or `mamba` to install the needed packages:\n\n```bash\n!conda install openmm\n\n# or, faster:\n!mamba install openmm\n```\n\nIf you have a environment file (e.g. `environment.yml`), you can use it like this:\n\n```bash\n!conda env update -n base -f environment.yml\n\n# or, faster:\n!mamba env update -n base -f environment.yml\n```\n\n\n## Shortcomings\n\n- The Python kernel needs to be restarted for changes to be applied. This happens automatically. If you are wondering why you are seeing a message saying _"Your session crashed for an unknown reason"_, this is why. You can safely ignore this message!\n- You can only use the `base` environment, so do not try to create more environments with `conda create`. If you have an environment file, use `conda env update -n base -f <your-file.yml>`.\n\n## FAQ\n\n### How does it work?\n\nGoogle Colab runs on Python 3.10. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.10 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.\n\n### How can I cache my installation? I don\'t want to wait every time I start Colab.\n\nThe recommended approach is to build your own `constructor`-based installer. We have provided an example in `constructor-example/construct.yaml`.\n\n> You can generate a `constructor` installer on Colab too! Follow [this tutorial](https://colab.research.google.com/github/jaimergp/condacolab/blob/main/constructor-example/condacolab_constructor_tutorial.ipynb).\n\nLocally, follow these steps:\n\n1. In your local computer:\n\n```bash\nconda create -n constructor -c conda-forge constructor\nconda activate constructor\nmkdir my-installer\ncd my-installer\ncurl -sLO https://raw.githubusercontent.com/jaimergp/condacolab/main/constructor-example/construct.yaml\ncurl -sLO https://raw.githubusercontent.com/jaimergp/condacolab/main/constructor-example/pip-dependencies.sh\n```\n\n2. Add your `conda` packages to `construct.yaml` in the `specs` section. Read the comments to respect the constrains already present! You can also adapt the metadata to your liking.\n3. If you _do_ need to install `pip` requirements, uncomment the `post_install` line and edit `pip-dependencies.sh`.\n4. Run `constructor --platform linux-64 .`\n5. Upload the resulting `.sh` to an online location with a permanent URL. GitHub Releases is great for this!\n6. In Colab, run:\n\n```python\n!pip install -q condacolab\nimport condacolab\ncondacolab.install_from_url(URL_TO_YOUR_CUSTOM_CONSTRUCTOR_INSTALLER)\n```\n\n## Can I install R packages?\n\nYes, as long as you make sure you also install `rpy2` to overwrite Colab\'s installation.\nSee [issue #26](https://github.com/conda-incubator/condacolab/issues/26) for more details.\n',
     'author': 'Jaime Rodríguez-Guerra',
     'author_email': 'jaimergp@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/jaimergp/condacolab',
     'py_modules': modules,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `condacolab-0.1.6/PKG-INFO` & `condacolab-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: condacolab
-Version: 0.1.6
-Summary: Install Conda and friends on Google Colab, easily
-Home-page: https://github.com/jaimergp/condacolab
-License: MIT
-Author: Jaime Rodríguez-Guerra
-Author-email: jaimergp@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Project-URL: Repository, https://github.com/jaimergp/condacolab
-Description-Content-Type: text/markdown
-
 # condacolab
 
 [![Downloads](https://pepy.tech/badge/condacolab/week)](https://pypi.org/project/condacolab)
 [![Downloads](https://pepy.tech/badge/condacolab/month)](https://pypi.org/project/condacolab)
 [![Downloads](https://pepy.tech/badge/condacolab)](https://pypi.org/project/condacolab)
 
 Install Conda and friends on Google Colab, easily.
@@ -44,19 +27,19 @@
 condacolab.check()
 ```
 
 > It is important that you perform the installation first thing in the notebook because it will require a kernel restart, thus resetting the variables set up to that point.
 
 The default `condacolab.install()` provides Mambaforge, but there are other `conda` distributions to choose from:
 
-- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.9. Unlike Anaconda, this distribution only contains `python` and `conda`.
-- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it's built for Python 3.9.
-- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge) but we [forked and patched it](https://github.com/jaimergp/miniforge) so it's built for Python 3.9.
+- `install_miniconda()`: This will install the Miniconda distribution, using a version built for Python 3.10. Unlike Anaconda, this distribution only contains `python` and `conda`.
+- `install_miniforge()`: Like Miniconda, but built off `conda-forge` packages. The Miniforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).
+- `install_mambaforge()`: Like Miniforge, but with `mamba` included. The Mambaforge distribution is officially provided by [conda-forge](https://github.com/conda-forge/miniforge).
 
-For advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.9 distribution that fulfills your own needs.
+For advanced users, `install_from_url()` is also available. It expects a URL pointing to a [`constructor`-like installer](https://github.com/conda/constructor), so you can prebuild a Python 3.10 distribution that fulfills your own needs.
 
 > If you want to build your own `constructor`-based installer, check the FAQ below!
 
 Once the installation is done, you can use `conda` and/or `mamba` to install the needed packages:
 
 ```bash
 !conda install openmm
@@ -74,21 +57,21 @@
 !mamba env update -n base -f environment.yml
 ```
 
 
 ## Shortcomings
 
 - The Python kernel needs to be restarted for changes to be applied. This happens automatically. If you are wondering why you are seeing a message saying _"Your session crashed for an unknown reason"_, this is why. You can safely ignore this message!
-- You can only use the `base` environment, so do not try to create more environments with `conda create`.
+- You can only use the `base` environment, so do not try to create more environments with `conda create`. If you have an environment file, use `conda env update -n base -f <your-file.yml>`.
 
 ## FAQ
 
 ### How does it work?
 
-Google Colab runs on Python 3.9. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.9 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.
+Google Colab runs on Python 3.10. We install the Miniconda distribution on top of the existing one at `/usr/local`, add a few configuration files so we stay with Python 3.10 and the newly installed packages are available. Finally, we wrap the Python executable to redirect and inject some environment variables needed to load the new libraries. Since we need to re-read `LD_LIBRARY_PATH`, a kernel restart is needed.
 
 ### How can I cache my installation? I don't want to wait every time I start Colab.
 
 The recommended approach is to build your own `constructor`-based installer. We have provided an example in `constructor-example/construct.yaml`.
 
 > You can generate a `constructor` installer on Colab too! Follow [this tutorial](https://colab.research.google.com/github/jaimergp/condacolab/blob/main/constructor-example/condacolab_constructor_tutorial.ipynb).
 
@@ -117,8 +100,7 @@
 condacolab.install_from_url(URL_TO_YOUR_CUSTOM_CONSTRUCTOR_INSTALLER)
 ```
 
 ## Can I install R packages?
 
 Yes, as long as you make sure you also install `rpy2` to overwrite Colab's installation.
 See [issue #26](https://github.com/conda-incubator/condacolab/issues/26) for more details.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

