# Comparing `tmp/frankAllSkyCam-4.0.tar.gz` & `tmp/frankAllSkyCam-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-4.0.tar", last modified: Thu Apr 27 22:32:22 2023, max compression
+gzip compressed data, was "frankAllSkyCam-4.1.tar", last modified: Thu Apr 27 22:45:55 2023, max compression
```

## Comparing `frankAllSkyCam-4.0.tar` & `frankAllSkyCam-4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:32:22.421929 frankAllSkyCam-4.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-27 22:32:22.421929 frankAllSkyCam-4.0/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:32:22.421929 frankAllSkyCam-4.0/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-27 22:29:12.950926 frankAllSkyCam-4.0/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3145 2023-04-27 20:15:33.286678 frankAllSkyCam-4.0/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)      722 2023-04-27 20:16:14.958227 frankAllSkyCam-4.0/frankAllSkyCam/allskycamdelete.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3026 2023-04-27 20:22:22.766227 frankAllSkyCam-4.0/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-4.0/frankAllSkyCam/drawtext.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-4.0/frankAllSkyCam/fileManager.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:32:22.421929 frankAllSkyCam-4.0/frankAllSkyCam/helper/
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2142 2023-04-26 16:02:38.467378 frankAllSkyCam-4.0/frankAllSkyCam/helper/config.txt
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-16 22:11:11.734516 frankAllSkyCam-4.0/frankAllSkyCam/helper/index.html
--rwxrwxrw-   0 pi        (1000) pi        (1000)    17690 2023-04-27 22:16:28.896526 frankAllSkyCam-4.0/frankAllSkyCam/imageHeader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2818 2023-04-27 20:17:15.505570 frankAllSkyCam-4.0/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-4.0/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.0/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.0/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4172 2023-04-27 20:18:55.748481 frankAllSkyCam-4.0/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1310 2023-04-27 20:16:52.069824 frankAllSkyCam-4.0/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-4.0/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     2470 2023-04-27 22:29:49.155827 frankAllSkyCam-4.0/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:32:22.421929 frankAllSkyCam-4.0/test/
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.0/test/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.0/test/test_suncalc.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:45:55.504885 frankAllSkyCam-4.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-04-27 22:45:55.504885 frankAllSkyCam-4.1/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:45:55.504885 frankAllSkyCam-4.1/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-04-27 22:45:28.885592 frankAllSkyCam-4.1/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3145 2023-04-27 20:15:33.286678 frankAllSkyCam-4.1/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)      722 2023-04-27 20:16:14.958227 frankAllSkyCam-4.1/frankAllSkyCam/allskycamdelete.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3026 2023-04-27 20:22:22.766227 frankAllSkyCam-4.1/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     1313 2023-04-25 21:31:56.286444 frankAllSkyCam-4.1/frankAllSkyCam/drawtext.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2318 2021-07-23 08:29:59.174829 frankAllSkyCam-4.1/frankAllSkyCam/fileManager.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:45:55.504885 frankAllSkyCam-4.1/frankAllSkyCam/helper/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2142 2023-04-26 16:02:38.467378 frankAllSkyCam-4.1/frankAllSkyCam/helper/config.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-04-16 22:11:11.734516 frankAllSkyCam-4.1/frankAllSkyCam/helper/index.html
+-rwxrwxrw-   0 pi        (1000) pi        (1000)    17690 2023-04-27 22:16:28.896526 frankAllSkyCam-4.1/frankAllSkyCam/imageHeader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2818 2023-04-27 20:17:15.505570 frankAllSkyCam-4.1/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-04-26 16:50:47.955578 frankAllSkyCam-4.1/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.1/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.1/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4172 2023-04-27 20:18:55.748481 frankAllSkyCam-4.1/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1310 2023-04-27 20:16:52.069824 frankAllSkyCam-4.1/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-4.1/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     2470 2023-04-27 22:44:54.550598 frankAllSkyCam-4.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 22:45:55.504885 frankAllSkyCam-4.1/test/
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-04-16 16:51:13.326836 frankAllSkyCam-4.1/test/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2263 2023-04-05 15:29:11.227398 frankAllSkyCam-4.1/test/test_suncalc.py
```

### Comparing `frankAllSkyCam-4.0/PKG-INFO` & `frankAllSkyCam-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 4.0
+Version: 4.1
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.0.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.1.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/__main__.py` & `frankAllSkyCam-4.1/frankAllSkyCam/__main__.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-4.1/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/crontab.py` & `frankAllSkyCam-4.1/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-4.1/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-4.1/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/helper/config.txt` & `frankAllSkyCam-4.1/frankAllSkyCam/helper/config.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-4.1/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/startrail.py` & `frankAllSkyCam-4.1/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-4.1/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-4.1/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-4.1/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-4.1/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-4.1/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/setup.py` & `frankAllSkyCam-4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import shutil
 from distutils.core import setup
 
 homepath = os.path.expanduser("~")
 setup(
   name = 'frankAllSkyCam',         # How you named your package folder (MyLib)
   packages = ['frankAllSkyCam'],   # Chose the same as "name"
-  version = '4.0',      # Start with a small number and increase it with every change you make
+  version = '4.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',   # Give a short description about your library
   author = 'Francesco Sferlazza',                   # Type in your name
   author_email = 'sferlazza@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/sferlix/frankAllSkyCam',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.0.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/4.1.tar.gz',    # I explain this later on
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'pytz',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

### Comparing `frankAllSkyCam-4.0/test/test_sqm.py` & `frankAllSkyCam-4.1/test/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-4.0/test/test_suncalc.py` & `frankAllSkyCam-4.1/test/test_suncalc.py`

 * *Files identical despite different names*

