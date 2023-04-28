# Comparing `tmp/mpose-1.0.8.tar.gz` & `tmp/mpose-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpose-1.0.8.tar", last modified: Tue Dec 21 09:39:02 2021, max compression
+gzip compressed data, was "dist/mpose-1.0.9.tar", last modified: Tue Dec 21 11:20:33 2021, max compression
```

## Comparing `mpose-1.0.8.tar` & `mpose-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 09:39:02.000000 mpose-1.0.8/
--rw-rw-r--   0 simone    (1005) simone    (1005)     5140 2021-12-21 09:18:40.000000 mpose-1.0.8/README.md
--rwxrwxrwx   0 simone    (1005) simone    (1005)      594 2021-12-21 09:37:42.000000 mpose-1.0.8/setup.py
--rw-rw-r--   0 simone    (1005) simone    (1005)       38 2021-12-21 09:39:02.000000 mpose-1.0.8/setup.cfg
-drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/
--rwxrwxrwx   0 simone    (1005) simone    (1005)      248 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/SOURCES.txt
--rwxrwxrwx   0 simone    (1005) simone    (1005)        1 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/dependency_links.txt
--rwxrwxrwx   0 simone    (1005) simone    (1005)       38 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/requires.txt
--rwxrwxrwx   0 simone    (1005) simone    (1005)        6 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/top_level.txt
--rwxrwxrwx   0 simone    (1005) simone    (1005)     6078 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose.egg-info/PKG-INFO
-drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 09:39:02.000000 mpose-1.0.8/mpose/
--rwxrwxrwx   0 simone    (1005) simone    (1005)     9408 2021-12-21 09:24:48.000000 mpose-1.0.8/mpose/mpose.py
--rwxrwxrwx   0 simone    (1005) simone    (1005)       21 2021-09-15 09:41:23.000000 mpose-1.0.8/mpose/transforms.py
--rwxrwxrwx   0 simone    (1005) simone    (1005)     1626 2021-12-20 17:10:19.000000 mpose-1.0.8/mpose/config.yaml
--rwxrwxrwx   0 simone    (1005) simone    (1005)       57 2021-09-16 17:27:41.000000 mpose-1.0.8/mpose/__init__.py
--rwxrwxrwx   0 simone    (1005) simone    (1005)     2047 2021-12-21 09:25:52.000000 mpose-1.0.8/mpose/utils.py
--rw-rw-r--   0 simone    (1005) simone    (1005)     6078 2021-12-21 09:39:02.000000 mpose-1.0.8/PKG-INFO
+drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 11:20:33.000000 mpose-1.0.9/
+-rw-rw-r--   0 simone    (1005) simone    (1005)     5402 2021-12-21 11:16:52.000000 mpose-1.0.9/README.md
+-rwxrwxrwx   0 simone    (1005) simone    (1005)      594 2021-12-21 11:16:58.000000 mpose-1.0.9/setup.py
+-rw-rw-r--   0 simone    (1005) simone    (1005)       38 2021-12-21 11:20:33.000000 mpose-1.0.9/setup.cfg
+drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/
+-rwxrwxrwx   0 simone    (1005) simone    (1005)      248 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/SOURCES.txt
+-rwxrwxrwx   0 simone    (1005) simone    (1005)        1 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/dependency_links.txt
+-rwxrwxrwx   0 simone    (1005) simone    (1005)       38 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/requires.txt
+-rwxrwxrwx   0 simone    (1005) simone    (1005)        6 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/top_level.txt
+-rwxrwxrwx   0 simone    (1005) simone    (1005)     6364 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose.egg-info/PKG-INFO
+drwxrwxr-x   0 simone    (1005) simone    (1005)        0 2021-12-21 11:20:33.000000 mpose-1.0.9/mpose/
+-rwxrwxrwx   0 simone    (1005) simone    (1005)     9408 2021-12-21 09:24:48.000000 mpose-1.0.9/mpose/mpose.py
+-rwxrwxrwx   0 simone    (1005) simone    (1005)       21 2021-09-15 09:41:23.000000 mpose-1.0.9/mpose/transforms.py
+-rwxrwxrwx   0 simone    (1005) simone    (1005)     1626 2021-12-20 17:10:19.000000 mpose-1.0.9/mpose/config.yaml
+-rwxrwxrwx   0 simone    (1005) simone    (1005)       57 2021-09-16 17:27:41.000000 mpose-1.0.9/mpose/__init__.py
+-rwxrwxrwx   0 simone    (1005) simone    (1005)     2047 2021-12-21 09:25:52.000000 mpose-1.0.9/mpose/utils.py
+-rw-rw-r--   0 simone    (1005) simone    (1005)     6364 2021-12-21 11:20:33.000000 mpose-1.0.9/PKG-INFO
```

### Comparing `mpose-1.0.8/README.md` & `mpose-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 Since these datasets have heterogenous action labels, each dataset labels are remapped to a common and homogeneous list of actions.
 
 This repository allows users to generate pose data for MPOSE2021 in a python-friendly format. 
 Generated sequences have a number of frames between 20 and 30. 
 Sequences are obtained by cutting the so-called Precursor VIDEOS (videos from the above-mentioned datasets), with non-overlapping sliding windows.
 Frames where OpenPose cannot detect any subject are automatically discarded. Resulting samples contain one subject at the time, performing a fraction of a single action. Overall, MPOSE2021 contains 15429 samples, divided into 20 actions, performed by 100 subjects. 
 
-The overview of the action composition of MPOSE2021 is provided [here](https://github.com/FedericoAngelini/MPOSE2021_Dataset/blob/master/docs/mpose2021_summary.pdf?raw=true).
+The overview of the action composition of MPOSE2021 is provided in the following image:
 
-Below, the steps to install the ```mpose``` library and obtain sequences are explained.
+<p align="center">
+  <img src="https://github.com/PIC4SeR/MPOSE2021_Dataset/docs/mpose2021_summary.png" alt="MPOSE2021 Summary" width="600">
+</p>
 
-Check our [Colab Notebook Tutorial](link) for quick hands-on examples.
+Below, the steps to install the ```mpose``` library and obtain sequences are explained. Source code can be found in the [MPOSE2021 repository](https://github.com/PIC4SeRCentre/MPOSE2021_Dataset).
 
 ### Installation
 
 Install MPOSE2021 as python package from [PyPi](https://pypi.org/project/mpose)
 ```
 pip install mpose
 ```
 
 ### Getting Started
 
-This minimal working example
 ```python
 # import package
 import mpose
 
 # initialize and download data
 dataset = mpose.MPOSE(pose_extractor='openpose', 
                       split=1, 
@@ -43,15 +44,17 @@
 # print data info 
 dataset.get_info()
 
 # get data samples (as numpy arrays)
 X_train, y_train, X_test, y_test = dataset.get_dataset()
 ```
 
-[![asciicast](https://asciinema.org/a/455413.svg)](https://asciinema.org/a/455413)
+[![asciicast](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7.svg)](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7)
+
+Check out our [Colab Notebook Tutorial](https://colab.research.google.com/drive/1_v3DYwgZPMCiELtgiwMRYxQzcYGdSWFH?usp=sharing) for quick hands-on examples.
 
 ### References
 
 MPOSE2021 is part of a paper published by the [Pattern Recognition Journal](https://authors.elsevier.com/a/1eH6s77nKcvmg) (Elsevier), and is intended for scientific research purposes.
 If you want to use MPOSE2021 for your research work, please also cite [1-10].
 
 ```
```

### Comparing `mpose-1.0.8/setup.py` & `mpose-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         long_description = f.read()
 except:
     long_description = ''
     
 setup(
     name='mpose',
     packages=find_packages(),
-    version='1.0.8',
+    version='1.0.9',
     description='MPOSE2021: a Dataset for Short-time Pose-based Human Action Recognition',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='Simone Angarano',
     license='MIT',
     install_requires=['numpy', 'tqdm', 'pyyaml', 'importlib_resources'],
     package_data={'': ["*.yaml"]}
```

### Comparing `mpose-1.0.8/mpose.egg-info/PKG-INFO` & `mpose-1.0.9/mpose.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpose
-Version: 1.0.8
+Version: 1.0.9
 Summary: MPOSE2021: a Dataset for Short-time Pose-based Human Action Recognition
 Home-page: UNKNOWN
 Author: Simone Angarano
 License: MIT
 Description: # MPOSE2021:
         #### A Dataset for Real-Time Short-Time HAR
         
@@ -17,30 +17,31 @@
         Since these datasets have heterogenous action labels, each dataset labels are remapped to a common and homogeneous list of actions.
         
         This repository allows users to generate pose data for MPOSE2021 in a python-friendly format. 
         Generated sequences have a number of frames between 20 and 30. 
         Sequences are obtained by cutting the so-called Precursor VIDEOS (videos from the above-mentioned datasets), with non-overlapping sliding windows.
         Frames where OpenPose cannot detect any subject are automatically discarded. Resulting samples contain one subject at the time, performing a fraction of a single action. Overall, MPOSE2021 contains 15429 samples, divided into 20 actions, performed by 100 subjects. 
         
-        The overview of the action composition of MPOSE2021 is provided [here](https://github.com/FedericoAngelini/MPOSE2021_Dataset/blob/master/docs/mpose2021_summary.pdf?raw=true).
+        The overview of the action composition of MPOSE2021 is provided in the following image:
         
-        Below, the steps to install the ```mpose``` library and obtain sequences are explained.
+        <p align="center">
+          <img src="https://github.com/PIC4SeR/MPOSE2021_Dataset/docs/mpose2021_summary.png" alt="MPOSE2021 Summary" width="600">
+        </p>
         
-        Check our [Colab Notebook Tutorial](link) for quick hands-on examples.
+        Below, the steps to install the ```mpose``` library and obtain sequences are explained. Source code can be found in the [MPOSE2021 repository](https://github.com/PIC4SeRCentre/MPOSE2021_Dataset).
         
         ### Installation
         
         Install MPOSE2021 as python package from [PyPi](https://pypi.org/project/mpose)
         ```
         pip install mpose
         ```
         
         ### Getting Started
         
-        This minimal working example
         ```python
         # import package
         import mpose
         
         # initialize and download data
         dataset = mpose.MPOSE(pose_extractor='openpose', 
                               split=1, 
@@ -50,15 +51,17 @@
         # print data info 
         dataset.get_info()
         
         # get data samples (as numpy arrays)
         X_train, y_train, X_test, y_test = dataset.get_dataset()
         ```
         
-        [![asciicast](https://asciinema.org/a/455413.svg)](https://asciinema.org/a/455413)
+        [![asciicast](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7.svg)](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7)
+        
+        Check out our [Colab Notebook Tutorial](https://colab.research.google.com/drive/1_v3DYwgZPMCiELtgiwMRYxQzcYGdSWFH?usp=sharing) for quick hands-on examples.
         
         ### References
         
         MPOSE2021 is part of a paper published by the [Pattern Recognition Journal](https://authors.elsevier.com/a/1eH6s77nKcvmg) (Elsevier), and is intended for scientific research purposes.
         If you want to use MPOSE2021 for your research work, please also cite [1-10].
         
         ```
```

### Comparing `mpose-1.0.8/mpose/mpose.py` & `mpose-1.0.9/mpose/mpose.py`

 * *Files identical despite different names*

### Comparing `mpose-1.0.8/mpose/config.yaml` & `mpose-1.0.9/mpose/config.yaml`

 * *Files identical despite different names*

### Comparing `mpose-1.0.8/mpose/utils.py` & `mpose-1.0.9/mpose/utils.py`

 * *Files identical despite different names*

### Comparing `mpose-1.0.8/PKG-INFO` & `mpose-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpose
-Version: 1.0.8
+Version: 1.0.9
 Summary: MPOSE2021: a Dataset for Short-time Pose-based Human Action Recognition
 Home-page: UNKNOWN
 Author: Simone Angarano
 License: MIT
 Description: # MPOSE2021:
         #### A Dataset for Real-Time Short-Time HAR
         
@@ -17,30 +17,31 @@
         Since these datasets have heterogenous action labels, each dataset labels are remapped to a common and homogeneous list of actions.
         
         This repository allows users to generate pose data for MPOSE2021 in a python-friendly format. 
         Generated sequences have a number of frames between 20 and 30. 
         Sequences are obtained by cutting the so-called Precursor VIDEOS (videos from the above-mentioned datasets), with non-overlapping sliding windows.
         Frames where OpenPose cannot detect any subject are automatically discarded. Resulting samples contain one subject at the time, performing a fraction of a single action. Overall, MPOSE2021 contains 15429 samples, divided into 20 actions, performed by 100 subjects. 
         
-        The overview of the action composition of MPOSE2021 is provided [here](https://github.com/FedericoAngelini/MPOSE2021_Dataset/blob/master/docs/mpose2021_summary.pdf?raw=true).
+        The overview of the action composition of MPOSE2021 is provided in the following image:
         
-        Below, the steps to install the ```mpose``` library and obtain sequences are explained.
+        <p align="center">
+          <img src="https://github.com/PIC4SeR/MPOSE2021_Dataset/docs/mpose2021_summary.png" alt="MPOSE2021 Summary" width="600">
+        </p>
         
-        Check our [Colab Notebook Tutorial](link) for quick hands-on examples.
+        Below, the steps to install the ```mpose``` library and obtain sequences are explained. Source code can be found in the [MPOSE2021 repository](https://github.com/PIC4SeRCentre/MPOSE2021_Dataset).
         
         ### Installation
         
         Install MPOSE2021 as python package from [PyPi](https://pypi.org/project/mpose)
         ```
         pip install mpose
         ```
         
         ### Getting Started
         
-        This minimal working example
         ```python
         # import package
         import mpose
         
         # initialize and download data
         dataset = mpose.MPOSE(pose_extractor='openpose', 
                               split=1, 
@@ -50,15 +51,17 @@
         # print data info 
         dataset.get_info()
         
         # get data samples (as numpy arrays)
         X_train, y_train, X_test, y_test = dataset.get_dataset()
         ```
         
-        [![asciicast](https://asciinema.org/a/455413.svg)](https://asciinema.org/a/455413)
+        [![asciicast](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7.svg)](https://asciinema.org/a/4dXzjbZUoxXM6d3o0aNumGLr7)
+        
+        Check out our [Colab Notebook Tutorial](https://colab.research.google.com/drive/1_v3DYwgZPMCiELtgiwMRYxQzcYGdSWFH?usp=sharing) for quick hands-on examples.
         
         ### References
         
         MPOSE2021 is part of a paper published by the [Pattern Recognition Journal](https://authors.elsevier.com/a/1eH6s77nKcvmg) (Elsevier), and is intended for scientific research purposes.
         If you want to use MPOSE2021 for your research work, please also cite [1-10].
         
         ```
```

