# Comparing `tmp/apkmod-1.0.0.tar.gz` & `tmp/apkmod-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkmod-1.0.0.tar", last modified: Thu Apr 27 18:29:47 2023, max compression
+gzip compressed data, was "apkmod-1.0.1.tar", last modified: Fri Apr 28 15:01:48 2023, max compression
```

## Comparing `apkmod-1.0.0.tar` & `apkmod-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 18:29:47.752046 apkmod-1.0.0/
--rw-rw-rw-   0        0        0    18385 2023-04-09 07:03:40.000000 apkmod-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      190 2023-04-27 18:29:47.751044 apkmod-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1356 2023-04-27 10:54:15.000000 apkmod-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 18:29:47.691042 apkmod-1.0.0/apkmod/
--rw-rw-rw-   0        0        0       24 2023-04-27 10:37:18.000000 apkmod-1.0.0/apkmod/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-04-27 18:17:43.000000 apkmod-1.0.0/apkmod/android_manifest_util.py
--rw-rw-rw-   0        0        0     4023 2023-04-27 08:47:56.000000 apkmod-1.0.0/apkmod/frida_gadget_util.py
--rw-rw-rw-   0        0        0     2582 2023-04-27 18:27:19.000000 apkmod-1.0.0/apkmod/main.py
--rw-rw-rw-   0        0        0     5529 2023-04-27 10:40:53.000000 apkmod-1.0.0/apkmod/smali_injector_util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 18:29:47.748042 apkmod-1.0.0/apkmod.egg-info/
--rw-rw-rw-   0        0        0      190 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 18:29:47.000000 apkmod-1.0.0/apkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 18:29:47.752046 apkmod-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-04-27 18:29:28.000000 apkmod-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.749643 apkmod-1.0.1/
+-rw-rw-rw-   0        0        0    18385 2023-04-09 07:03:40.000000 apkmod-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1561 2023-04-28 15:01:48.749643 apkmod-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1328 2023-04-27 18:34:29.000000 apkmod-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.694615 apkmod-1.0.1/apkmod/
+-rw-rw-rw-   0        0        0       24 2023-04-27 10:37:18.000000 apkmod-1.0.1/apkmod/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-04-27 18:17:43.000000 apkmod-1.0.1/apkmod/android_manifest_util.py
+-rw-rw-rw-   0        0        0     4023 2023-04-27 08:47:56.000000 apkmod-1.0.1/apkmod/frida_gadget_util.py
+-rw-rw-rw-   0        0        0     2582 2023-04-27 18:27:19.000000 apkmod-1.0.1/apkmod/main.py
+-rw-rw-rw-   0        0        0     5529 2023-04-27 10:40:53.000000 apkmod-1.0.1/apkmod/smali_injector_util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.746566 apkmod-1.0.1/apkmod.egg-info/
+-rw-rw-rw-   0        0        0     1561 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:01:48.749643 apkmod-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-04-28 15:01:02.000000 apkmod-1.0.1/setup.py
```

### Comparing `apkmod-1.0.0/LICENSE` & `apkmod-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.0/README.md` & `apkmod-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Corss-Platform script used to inject frida scripts and gadget to an APK <br />
 This project started as a fork of [apkpatcher](https://github.com/badadaf/apkpatcher) <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only!
 
 ## Installation
 After you made sure that all of the requirements are met, <br />
-You may install the package and use the cmdline tool `apkmod` <br />
+You may install the package and use the cmdline tool `apkmod`, which comes with the cmdline tool [`buildapp`](https://github.com/mon231/buildapp) <br />
 
-package isn't yet on py-pi, so you'll have to install it from github: <br />
-> pip install git+https://github.com/mon231/apkpatcher
+> pip install apkmod
 
 ## Patching process
 This tool gets an android app installation file (`.apk`) and a [frida js-script](https://frida.re/docs/javascript-api/) <br />
 Then builds a new apk with frida-gadget & script runner ready to be installed on non-rooted android devices!
 
 ## Requirements
 The project assumes that installer already has the following tools in his path:
```

### Comparing `apkmod-1.0.0/apkmod/android_manifest_util.py` & `apkmod-1.0.1/apkmod/android_manifest_util.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.0/apkmod/frida_gadget_util.py` & `apkmod-1.0.1/apkmod/frida_gadget_util.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.0/apkmod/main.py` & `apkmod-1.0.1/apkmod/main.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.0/apkmod/smali_injector_util.py` & `apkmod-1.0.1/apkmod/smali_injector_util.py`

 * *Files identical despite different names*

