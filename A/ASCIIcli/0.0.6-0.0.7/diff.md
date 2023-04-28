# Comparing `tmp/ASCIIcli-0.0.6.tar.gz` & `tmp/ASCIIcli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.6.tar", last modified: Fri Apr 28 07:37:09 2023, max compression
+gzip compressed data, was "ASCIIcli-0.0.7.tar", last modified: Fri Apr 28 08:28:14 2023, max compression
```

## Comparing `ASCIIcli-0.0.6.tar` & `ASCIIcli-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:37:09.809683 ASCIIcli-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-04-28 07:37:09.763745 ASCIIcli-0.0.6/ASCIIcli.egg-info/
--rw-rw-rw-   0        0        0     2553 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 07:37:09.000000 ASCIIcli-0.0.6/ASCIIcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2553 2023-04-28 07:37:09.807642 ASCIIcli-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2058 2023-04-28 07:35:43.000000 ASCIIcli-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:37:09.794542 ASCIIcli-0.0.6/asciicli/
--rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.6/asciicli/__init__.py
--rw-rw-rw-   0        0        0     1583 2023-04-28 07:20:03.000000 ASCIIcli-0.0.6/asciicli/__main__.py
--rw-rw-rw-   0        0        0     3289 2023-04-28 07:37:08.000000 ASCIIcli-0.0.6/asciicli/functions.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:37:09.809683 ASCIIcli-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-04-28 07:36:53.000000 ASCIIcli-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:37:09.804870 ASCIIcli-0.0.6/tests/
--rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.6/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.518463 ASCIIcli-0.0.7/ASCIIcli.egg-info/
+-rw-rw-rw-   0        0        0     2553 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2553 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2058 2023-04-28 07:35:43.000000 ASCIIcli-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-04-28 08:27:50.000000 ASCIIcli-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.565207 ASCIIcli-0.0.7/src/
+-rw-rw-rw-   0        0        0      225 2023-04-28 08:20:42.000000 ASCIIcli-0.0.7/src/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-04-28 08:19:56.000000 ASCIIcli-0.0.7/src/__main__.py
+-rw-rw-rw-   0        0        0     3289 2023-04-28 08:22:09.000000 ASCIIcli-0.0.7/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.565207 ASCIIcli-0.0.7/tests/
+-rw-rw-rw-   0        0        0     2635 2023-04-28 08:20:33.000000 ASCIIcli-0.0.7/tests/tests.py
```

### Comparing `ASCIIcli-0.0.6/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.0.7/ASCIIcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.6/LICENSE` & `ASCIIcli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.6/PKG-INFO` & `ASCIIcli-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ASCIIcli-0.0.6/README.md` & `ASCIIcli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.6/asciicli/__main__.py` & `ASCIIcli-0.0.7/src/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This file is the command line parser for the ASCIIcli module.
 This module provides a command line tool for converting images to ASCII art.
 """
 
 import argparse
-from asciicli.functions import convert_to_ascii
-from asciicli.functions import print_cmd
+from src.functions import convert_to_ascii
+from src.functions import print_cmd
 
 
 def main():
     """
     Parses the command line arguments for the ASCII art converter program.
     """
```

### Comparing `ASCIIcli-0.0.6/asciicli/functions.py` & `ASCIIcli-0.0.7/src/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PIL import Image
 
 # define characters used
 char_a = list(string.ascii_uppercase)
 char_b = list(string.digits)
 char_c = ["0", "O", "o", "8", "9", "6", "@", "&", ":", '"', "."]
 char_d = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
-char_e = ['!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+', '-', '+']
+char_e = ['-', '=', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+']
 
 
 def get_char_set(set_choice):
     """
     Uses choice for character set by number and then returns the chosen set to.
     """
```

### Comparing `ASCIIcli-0.0.6/setup.py` & `ASCIIcli-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """
 This file is the setup script for the ASCIIcli module.
 This module provides a command line tool for converting images to ASCII art.
 
 To build:
 `py -m build`
 
+To build EXE:
+`pyinstaller --onefile path/to/__main__.py`
+
 To distribute:
 `twine upload dist/*`
 """
 
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ASCIIcli",
     author="mrq-andras",
-    version="0.0.6",
-    packages=['asciicli'],
+    version="0.0.7",
+    packages=['src'],
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
+            "asciicli=src.__main__:main"
         ]
     },
     python_requires=">=3.6",
     url="https://github.com/mrq-andras/asciicli",
     license="MIT",
     description="A command-line tool that converts images to ASCII art.",
     readme = "README.md"
```

### Comparing `ASCIIcli-0.0.6/tests/tests.py` & `ASCIIcli-0.0.7/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This file is the test area for the ASCIIcli module.
 This module provides a command line tool for converting images to ASCII art.
 """
 
 import unittest
 import argparse
 from unittest.mock import MagicMock
-from asciicli.functions import randomize, get_char_set, char_a, char_b, char_c, char_d, char_e
+from src.functions import randomize, get_char_set, char_a, char_b, char_c, char_d, char_e
 
 
 class Testing(unittest.TestCase):
     """
     The group of tests for ASCIIcli.
     """
```

