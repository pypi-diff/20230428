# Comparing `tmp/pathmatcher-1.8.0.tar.gz` & `tmp/pathmatcher-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathmatcher-1.8.0.tar", last modified: Thu Apr 27 22:31:50 2023, max compression
+gzip compressed data, was "pathmatcher-1.8.0b2.tar", last modified: Thu Apr 27 22:06:41 2023, max compression
```

## Comparing `pathmatcher-1.8.0.tar` & `pathmatcher-1.8.0b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/
--rw-rw-rw-   0        0        0     1093 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/LICENSE
--rw-rw-rw-   0        0        0       69 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    32663 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    29913 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 22:31:50.815819 pathmatcher-1.8.0/pathmatcher/
--rw-rw-rw-   0        0        0      168 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/__init__.py
--rw-rw-rw-   0        0        0       21 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/_version.py
--rw-rw-rw-   0        0        0     1955 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/expandhelper.m
--rw-rw-rw-   0        0        0     8063 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/functionalcoreg.m
-drwxrwxrwx   0        0        0        0 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/pathmatcher/mlabwrap/
--rw-rw-rw-   0        0        0     2123 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/README.rst
--rw-rw-rw-   0        0        0      331 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/__init__.py
--rw-rw-rw-   0        0        0    61177 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/awmstools.py
--rw-rw-rw-   0        0        0     5267 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/matlabcom.py
--rw-rw-rw-   0        0        0    18096 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/matlabpipe.py
--rw-rw-rw-   0        0        0     1069 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/mlabraw.py
--rw-rw-rw-   0        0        0    33031 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/mlabwrap/mlabwrap.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/pathmatcher/pathlib2/
--rw-rw-rw-   0        0        0    54694 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/pathlib2/__init__.py
--rw-rw-rw-   0        0        0    43942 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/pathmatcher.py
--rw-rw-rw-   0        0        0     3066 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/realignhelper.m
--rw-rw-rw-   0        0        0      928 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/regex_files.m
--rw-rw-rw-   0        0        0    62358 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/reorientation_registration_helper.py
--rw-rw-rw-   0        0        0      227 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/reorienthelper.m
--rw-rw-rw-   0        0        0     3297 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pathmatcher/tee.py
-drwxrwxrwx   0        0        0        0 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/pathmatcher.egg-info/
--rw-rw-rw-   0        0        0    32663 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-27 22:31:50.000000 pathmatcher-1.8.0/pathmatcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9954 2023-04-27 22:30:19.000000 pathmatcher-1.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 22:31:50.831443 pathmatcher-1.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/
+-rw-rw-rw-   0        0        0     1093 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0    29868 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/
+-rw-rw-rw-   0        0        0      168 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/_version.py
+-rw-rw-rw-   0        0        0     1955 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/expandhelper.m
+-rw-rw-rw-   0        0        0     8063 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/functionalcoreg.m
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/
+-rw-rw-rw-   0        0        0     2123 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/README.rst
+-rw-rw-rw-   0        0        0      331 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/__init__.py
+-rw-rw-rw-   0        0        0    61177 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py
+-rw-rw-rw-   0        0        0     5267 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py
+-rw-rw-rw-   0        0        0    18096 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py
+-rw-rw-rw-   0        0        0     1069 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py
+-rw-rw-rw-   0        0        0    33031 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher/pathlib2/
+-rw-rw-rw-   0        0        0    54694 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py
+-rw-rw-rw-   0        0        0    43942 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py
+-rw-rw-rw-   0        0        0     3066 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/realignhelper.m
+-rw-rw-rw-   0        0        0      928 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/regex_files.m
+-rw-rw-rw-   0        0        0    62358 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py
+-rw-rw-rw-   0        0        0      227 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/reorienthelper.m
+-rw-rw-rw-   0        0        0     3297 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pathmatcher/tee.py
+drwxrwxrwx   0        0        0        0 2023-04-27 22:06:41.868432 pathmatcher-1.8.0b2/pathmatcher.egg-info/
+-rw-rw-rw-   0        0        0    32620 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-27 22:06:41.000000 pathmatcher-1.8.0b2/pathmatcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9954 2023-04-27 22:04:58.000000 pathmatcher-1.8.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 22:06:41.884031 pathmatcher-1.8.0b2/setup.cfg
```

### Comparing `pathmatcher-1.8.0/LICENSE` & `pathmatcher-1.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/PKG-INFO` & `pathmatcher-1.8.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.8.0
+Version: 1.8.0b2
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
 Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/pathmatcher
@@ -64,29 +64,29 @@
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher --use-pep517
+pip install --upgrade pathmatcher
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre --use-pep517
+pip install --upgrade pathmatcher --pre
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
```

### Comparing `pathmatcher-1.8.0/README.md` & `pathmatcher-1.8.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher --use-pep517
+pip install --upgrade pathmatcher
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre --use-pep517
+pip install --upgrade pathmatcher --pre
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
```

### Comparing `pathmatcher-1.8.0/pathmatcher/expandhelper.m` & `pathmatcher-1.8.0b2/pathmatcher/expandhelper.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/functionalcoreg.m` & `pathmatcher-1.8.0b2/pathmatcher/functionalcoreg.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/README.rst` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/README.rst`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/awmstools.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/awmstools.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/matlabcom.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabcom.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/matlabpipe.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/matlabpipe.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/mlabraw.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabraw.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/mlabwrap/mlabwrap.py` & `pathmatcher-1.8.0b2/pathmatcher/mlabwrap/mlabwrap.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/pathlib2/__init__.py` & `pathmatcher-1.8.0b2/pathmatcher/pathlib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/pathmatcher.py` & `pathmatcher-1.8.0b2/pathmatcher/pathmatcher.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/realignhelper.m` & `pathmatcher-1.8.0b2/pathmatcher/realignhelper.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/regex_files.m` & `pathmatcher-1.8.0b2/pathmatcher/regex_files.m`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/reorientation_registration_helper.py` & `pathmatcher-1.8.0b2/pathmatcher/reorientation_registration_helper.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher/tee.py` & `pathmatcher-1.8.0b2/pathmatcher/tee.py`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pathmatcher.egg-info/PKG-INFO` & `pathmatcher-1.8.0b2/pathmatcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathmatcher
-Version: 1.8.0
+Version: 1.8.0b2
 Summary: Regular Expression Path Matcher - Easily batch manipulate folders and files trees with regular expression!
 Author-email: Stephen Karl Larroque <lrq3000@gmail.com>
 Maintainer-email: Stephen Karl Larroque <lrq3000@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/pathmatcher
 Project-URL: Documentation, https://github.com/lrq3000/pathmatcher/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/pathmatcher
@@ -64,29 +64,29 @@
 If you are not familliar with [regular expressions](http://regexone.com/), you can use online tools such as [Pythex](http://pythex.org/) to instantly test your regexp, and [this easy tutorial](https://github.com/ziishaned/learn-regex) to learn how this works.
 
 ## Install
 
 For Python 3.7+:
 
 ```
-pip install --upgrade pathmatcher --use-pep517
+pip install --upgrade pathmatcher
 ```
 
 Or on Windows you can use the prebuilt binaries in the [GitHub Releases](https://github.com/lrq3000/pathmatcher/releases).
 
 For the latest development release, use:
 
 ```
-pip install --upgrade pathmatcher --pre --use-pep517
+pip install --upgrade pathmatcher --pre
 ```
 
 For the cutting-edge code (likely unstable, do not use in production!), use:
 
 ```
-pip install --upgrade git+https://github.com/lrq3000/pathmatcher --pre --use-pep517
+pip install --upgrade git+https://github.com/lrq3000/pathmatcher
 ```
 
 For Python 2.7 to 3.6, the last compatible version is v1.7.6:
 
 ```
 pip install --upgrade pathmatcher==1.7.6
 ```
```

### Comparing `pathmatcher-1.8.0/pathmatcher.egg-info/SOURCES.txt` & `pathmatcher-1.8.0b2/pathmatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathmatcher-1.8.0/pyproject.toml` & `pathmatcher-1.8.0b2/pyproject.toml`

 * *Files identical despite different names*

