# Comparing `tmp/sagemaker_pytorch_training-2.7.0.tar.gz` & `tmp/sagemaker_pytorch_training-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_pytorch_training-2.7.0.tar", last modified: Thu Oct 20 19:23:51 2022, max compression
+gzip compressed data, was "dist/sagemaker_pytorch_training-2.8.0.tar", last modified: Fri Apr 28 04:21:24 2023, max compression
```

## Comparing `sagemaker_pytorch_training-2.7.0.tar` & `sagemaker_pytorch_training-2.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      178 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      102 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2432 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1411 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/README.rst
--rw-rw-r--   0 root         (0) root         (0)        6 2022-10-20 19:22:24.000000 sagemaker_pytorch_training-2.7.0/VERSION
--rw-rw-r--   0 root         (0) root         (0)      104 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2149 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_container/
--rw-rw-r--   0 root         (0) root         (0)      609 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_container/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6016 2022-10-20 19:20:14.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_container/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2432 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      421 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      161 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-10-20 19:23:51.000000 sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      178 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      102 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1411 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/README.rst
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-04-28 04:19:05.000000 sagemaker_pytorch_training-2.8.0/VERSION
+-rw-rw-r--   0 root         (0) root         (0)      104 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2156 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_container/
+-rw-rw-r--   0 root         (0) root         (0)      609 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_container/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6554 2023-04-27 23:30:14.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_container/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-28 04:21:24.000000 sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/top_level.txt
```

### Comparing `sagemaker_pytorch_training-2.7.0/LICENSE` & `sagemaker_pytorch_training-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_training-2.7.0/PKG-INFO` & `sagemaker_pytorch_training-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_pytorch_training
-Version: 2.7.0
+Version: 2.8.0
 Summary: Open source library for using PyTorch to train models on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-pytorch-training-toolkit
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: 
         ==================================
         SageMaker PyTorch Training Toolkit
```

### Comparing `sagemaker_pytorch_training-2.7.0/README.rst` & `sagemaker_pytorch_training-2.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_training-2.7.0/setup.py` & `sagemaker_pytorch_training-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import find_packages, setup
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-test_dependencies = ['boto3', 'coverage', 'flake8', 'future', 'mock', 'pytest', 'pytest-cov',
+test_dependencies = ['boto3', 'coverage==6.5.0', 'flake8', 'future', 'mock', 'pytest', 'pytest-cov',
                      'pytest-xdist', 'sagemaker[local]<2', 'torch', 'torchvision', 'tox']
 
 setup(
     name='sagemaker_pytorch_training',
     version=read('VERSION').strip(),
     description='Open source library for using PyTorch to train models on Amazon SageMaker.',
```

### Comparing `sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_container/__init__.py` & `sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_container/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_container/training.py` & `sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_container/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 
     # get capture_error from framework parameters
     capture_error = True
     if training_environment.additional_framework_parameters.get("sagemaker_toolkit_native_launcher_enabled"):
         capture_error = False
         logger.info(f'capture_error is {capture_error}. Default is True')
 
+    _set_torch_version_environment()
     try:
         entry_point.run(uri=training_environment.module_dir,
                         user_entry_point=training_environment.user_entry_point,
                         args=training_environment.to_cmd_args(),
                         env_vars=training_environment.to_env_vars(),
                         capture_error=capture_error,
                         runner_type=runner_type)
@@ -145,9 +146,26 @@
     os.environ['NCCL_SOCKET_IFNAME'] = network_interface_name
     # Disable IB transport and force to use IP sockets by default
     os.environ['NCCL_IB_DISABLE'] = '1'
     # Set to INFO for more NCCL debugging information
     os.environ['NCCL_DEBUG'] = 'WARN'
 
 
+def _set_torch_version_environment():
+    """Set PyTorch version environment variable.
+
+    This is the PyTorch version of the DLC.
+    """
+    try:
+        import torch
+
+        os.environ["SM_DLC_TORCH_VERSION"] = torch.__version__
+    except ModuleNotFoundError:
+        logger.warn("PyTorch cannot be found")
+    except ImportError:
+        logger.warn("PyTorch can be found, but cannot be imported")
+    except Exception:
+        logger.warn("Torch version environment variable cannot be set")
+
+
 def main():
     train(environment.Environment())
```

### Comparing `sagemaker_pytorch_training-2.7.0/src/sagemaker_pytorch_training.egg-info/PKG-INFO` & `sagemaker_pytorch_training-2.8.0/src/sagemaker_pytorch_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-pytorch-training
-Version: 2.7.0
+Version: 2.8.0
 Summary: Open source library for using PyTorch to train models on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-pytorch-training-toolkit
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: 
         ==================================
         SageMaker PyTorch Training Toolkit
```

