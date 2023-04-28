# Comparing `tmp/buildapp-1.1.1.tar.gz` & `tmp/buildapp-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildapp-1.1.1.tar", last modified: Thu Apr 27 18:48:41 2023, max compression
+gzip compressed data, was "buildapp-1.1.3.tar", last modified: Fri Apr 28 15:13:19 2023, max compression
```

## Comparing `buildapp-1.1.1.tar` & `buildapp-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.092253 buildapp-1.1.1/
--rw-rw-rw-   0        0        0      153 2023-04-27 18:48:41.092253 buildapp-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2567 2023-04-11 09:31:12.000000 buildapp-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.076629 buildapp-1.1.1/buildapp/
--rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.1.1/buildapp/__init__.py
--rw-rw-rw-   0        0        0     3381 2023-04-27 06:46:32.000000 buildapp-1.1.1/buildapp/buildapp.py
-drwxrwxrwx   0        0        0        0 2023-04-27 18:48:41.092253 buildapp-1.1.1/buildapp.egg-info/
--rw-rw-rw-   0        0        0      153 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 18:48:41.000000 buildapp-1.1.1/buildapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 18:48:41.092253 buildapp-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-04-27 18:46:12.000000 buildapp-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:13:19.632100 buildapp-1.1.3/
+-rw-rw-rw-   0        0        0     3280 2023-04-28 15:13:19.632100 buildapp-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3084 2023-04-28 11:27:51.000000 buildapp-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:13:19.600030 buildapp-1.1.3/buildapp/
+-rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.1.3/buildapp/__init__.py
+-rw-rw-rw-   0        0        0     3380 2023-04-28 11:38:52.000000 buildapp-1.1.3/buildapp/buildapp.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:13:19.627506 buildapp-1.1.3/buildapp.egg-info/
+-rw-rw-rw-   0        0        0     3280 2023-04-28 15:13:19.000000 buildapp-1.1.3/buildapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-28 15:13:19.000000 buildapp-1.1.3/buildapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:13:19.000000 buildapp-1.1.3/buildapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-28 15:13:19.000000 buildapp-1.1.3/buildapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 15:13:19.000000 buildapp-1.1.3/buildapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:13:19.632100 buildapp-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-04-28 15:03:45.000000 buildapp-1.1.3/setup.py
```

### Comparing `buildapp-1.1.1/README.md` & `buildapp-1.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -28,25 +28,29 @@
 For additional flags, ran `buildapp -h` <br/>
 
 - apktool build
     - Use apktool to rebuild the apk from the sources folder
     - > apktool b <sources_folder> -o <output_apk>
 - zip-alignment
     - apk is implemented as a zip file which should have the correct alignment in order to be installed
+    - implemented using [`zipalign`](https://developer.android.com/tools/zipalign)
 - generate / obtain keystore
     - our tool will generate a keystore if you didn't provide any
+    - implemented using [`keytool`](https://docs.oracle.com/javase/8/docs/technotes/tools/unix/keytool.html)
 - apk signing
     - our tool will sign the apk using that keystore
+    - implemented using [`apksigner`](https://developer.android.com/tools/apksigner)
 - apk installation
     - if asked to, buildapp will install the signed apk on connected adb device (if there's only one) <br/>
     *NOTE* that if you won't provide the same keystore as the original app already installed on your device, you may not be able to install the apk you built by this script unless you'll uninstall the original app first.
+    - implemented using [`adb`](https://developer.android.com/tools/adb)
 
 And that's it! Now you have a new apk, waiting to be installed it on your android devices!
 
 ## Requirements
 The project assumes that installer already has the following tools in his path:
-- android SDK tools (installed from android-sdk online)
+- android SDK tools ([download build_tools](https://dl.google.com/android/repository/build-tools_r33-windows.zip), [download platform_tools](https://dl.google.com/android/repository/platform-tools_r34.0.1-windows.zip))
     - adb (default at SDK\platform_tools, only required if `-i` flag is used)
     - zipalign (default at SDK\build_tools)
     - apksigner (default at SDK\build_tools)
 - apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
 - keytool (default at jdk or jre bin folders, only required if `-k` flag is missing)
```

### Comparing `buildapp-1.1.1/buildapp/buildapp.py` & `buildapp-1.1.3/buildapp/buildapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             ObtainKeystore.obtain_default_keystore()
             return
 
         global KEYSTORE_ALIAS, KEYSTORE_PASSWORD, KEYSTORE_PATH
 
         KEYSTORE_PATH = keystore_path
         KEYSTORE_ALIAS = input(f'Enter keystore alias: ')
-        KEYSTORE_PASSWORD = input(f'Enter alias for password: ')
+        KEYSTORE_PASSWORD = input(f'Enter keystore password: ')
 
     @staticmethod
     def obtain_default_keystore():
         if not os.path.isfile(KEYSTORE_PATH):
             run_process(f'keytool -genkey -v -keystore {KEYSTORE_PATH} -alias {KEYSTORE_ALIAS} -keyalg RSA -keysize 2048 -validity 10000', input_string=f'{KEYSTORE_PASSWORD}\n{KEYSTORE_PASSWORD}\n\n\n\n\n\n\nyes', ignore_stderr=True)
 
 class SignApk:
```

