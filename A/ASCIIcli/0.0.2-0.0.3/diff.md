# Comparing `tmp/ASCIIcli-0.0.2.tar.gz` & `tmp/ASCIIcli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.2.tar", last modified: Fri Apr 28 07:08:14 2023, max compression
+gzip compressed data, was "ASCIIcli-0.0.3.tar", last modified: Fri Apr 28 07:15:53 2023, max compression
```

## Comparing `ASCIIcli-0.0.2.tar` & `ASCIIcli-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:08:14.440982 ASCIIcli-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-28 07:08:14.419983 ASCIIcli-0.0.2/ASCIIcli.egg-info/
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 07:08:14.000000 ASCIIcli-0.0.2/ASCIIcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:08:14.436985 ASCIIcli-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2031 2023-04-28 06:58:31.000000 ASCIIcli-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:08:14.429983 ASCIIcli-0.0.2/asciicli/
--rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.2/asciicli/__init__.py
--rw-rw-rw-   0        0        0     1593 2023-04-28 06:56:39.000000 ASCIIcli-0.0.2/asciicli/__main__.py
--rw-rw-rw-   0        0        0     3280 2023-04-28 06:58:13.000000 ASCIIcli-0.0.2/asciicli/functions.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:08:14.441981 ASCIIcli-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-04-28 07:07:51.000000 ASCIIcli-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:08:14.431986 ASCIIcli-0.0.2/tests/
--rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.2/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.155571 ASCIIcli-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.132567 ASCIIcli-0.0.3/ASCIIcli.egg-info/
+-rw-rw-rw-   0        0        0     2526 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2526 2023-04-28 07:15:53.151570 ASCIIcli-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2031 2023-04-28 06:58:31.000000 ASCIIcli-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.144571 ASCIIcli-0.0.3/asciicli/
+-rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.3/asciicli/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-04-28 06:56:39.000000 ASCIIcli-0.0.3/asciicli/__main__.py
+-rw-rw-rw-   0        0        0     3280 2023-04-28 06:58:13.000000 ASCIIcli-0.0.3/asciicli/functions.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:15:53.155571 ASCIIcli-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-04-28 07:15:28.000000 ASCIIcli-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.147570 ASCIIcli-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.3/tests/tests.py
```

### Comparing `ASCIIcli-0.0.2/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.0.3/ASCIIcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.2/LICENSE` & `ASCIIcli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.2/PKG-INFO` & `ASCIIcli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.2
+Version: 0.0.3
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.2/README.md` & `ASCIIcli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.2/asciicli/__main__.py` & `ASCIIcli-0.0.3/asciicli/__main__.py`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.2/asciicli/functions.py` & `ASCIIcli-0.0.3/asciicli/functions.py`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.2/setup.py` & `ASCIIcli-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ASCIIcli",
     author="mrq-andras",
-    version="0.0.2",
+    version="0.0.3",
     packages=['asciicli'],
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "asciicli=asciicli.__main__:main"
+            "asciicli=asciicli.__main__"
         ]
     },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/asciicli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
     readme = "README.md"
```

### Comparing `ASCIIcli-0.0.2/tests/tests.py` & `ASCIIcli-0.0.3/tests/tests.py`

 * *Files identical despite different names*

