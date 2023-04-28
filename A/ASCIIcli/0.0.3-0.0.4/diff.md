# Comparing `tmp/ASCIIcli-0.0.3.tar.gz` & `tmp/ASCIIcli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.3.tar", last modified: Fri Apr 28 07:15:53 2023, max compression
+gzip compressed data, was "ASCIIcli-0.0.4.tar", last modified: Fri Apr 28 07:22:15 2023, max compression
```

## Comparing `ASCIIcli-0.0.3.tar` & `ASCIIcli-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.155571 ASCIIcli-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.132567 ASCIIcli-0.0.3/ASCIIcli.egg-info/
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 07:15:53.000000 ASCIIcli-0.0.3/ASCIIcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:15:53.151570 ASCIIcli-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2031 2023-04-28 06:58:31.000000 ASCIIcli-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.144571 ASCIIcli-0.0.3/asciicli/
--rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.3/asciicli/__init__.py
--rw-rw-rw-   0        0        0     1593 2023-04-28 06:56:39.000000 ASCIIcli-0.0.3/asciicli/__main__.py
--rw-rw-rw-   0        0        0     3280 2023-04-28 06:58:13.000000 ASCIIcli-0.0.3/asciicli/functions.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:15:53.155571 ASCIIcli-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-04-28 07:15:28.000000 ASCIIcli-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:15:53.147570 ASCIIcli-0.0.3/tests/
--rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.3/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.611592 ASCIIcli-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.585593 ASCIIcli-0.0.4/ASCIIcli.egg-info/
+-rw-rw-rw-   0        0        0     2526 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2526 2023-04-28 07:22:15.608597 ASCIIcli-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2031 2023-04-28 06:58:31.000000 ASCIIcli-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.599593 ASCIIcli-0.0.4/asciicli/
+-rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.4/asciicli/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-04-28 07:20:03.000000 ASCIIcli-0.0.4/asciicli/__main__.py
+-rw-rw-rw-   0        0        0     3280 2023-04-28 07:20:33.000000 ASCIIcli-0.0.4/asciicli/functions.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:22:15.611592 ASCIIcli-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-04-28 07:21:20.000000 ASCIIcli-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.601612 ASCIIcli-0.0.4/tests/
+-rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.4/tests/tests.py
```

### Comparing `ASCIIcli-0.0.3/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.0.4/ASCIIcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.3/LICENSE` & `ASCIIcli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.3/PKG-INFO` & `ASCIIcli-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.3/README.md` & `ASCIIcli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.3/asciicli/__main__.py` & `ASCIIcli-0.0.4/asciicli/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import argparse
 from asciicli.functions import convert_to_ascii
 from asciicli.functions import print_cmd
 
 
-def arguments():
+def main():
     """
     Parses the command line arguments for the ASCII art converter program.
     """
 
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
@@ -36,8 +36,8 @@
     # print out the chosen options
     print_cmd(args)
     # call the conversion function from ascii.py
     convert_to_ascii(args)
 
 
 if __name__ == '__main__':
-    arguments()
+    main()
```

### Comparing `ASCIIcli-0.0.3/asciicli/functions.py` & `ASCIIcli-0.0.4/asciicli/functions.py`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.3/setup.py` & `ASCIIcli-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ASCIIcli",
     author="mrq-andras",
-    version="0.0.3",
+    version="0.0.4",
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
-            "asciicli=asciicli.__main__"
+            "asciicli=asciicli.__main__:main"
         ]
     },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/asciicli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
     readme = "README.md"
```

### Comparing `ASCIIcli-0.0.3/tests/tests.py` & `ASCIIcli-0.0.4/tests/tests.py`

 * *Files identical despite different names*

