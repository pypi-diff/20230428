# Comparing `tmp/WatchUI-2.0.8.tar.gz` & `tmp/watchui-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WatchUI-2.0.8.tar", max compression
+gzip compressed data, was "watchui-2.0.9.tar", max compression
```

## Comparing `WatchUI-2.0.8.tar` & `watchui-2.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1135 2022-10-04 11:45:19.119792 WatchUI-2.0.8/LICENSE
--rw-r--r--   0        0        0     2691 2022-10-04 11:45:19.123792 WatchUI-2.0.8/README.md
--rw-r--r--   0        0        0     5679 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/Ibasic/IBasic.py
--rw-r--r--   0        0        0       78 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/Ibasic/__init__.py
--rw-r--r--   0        0        0     2229 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/WatchUI.py
--rw-r--r--   0        0        0       36 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/__init__.py
--rw-r--r--   0        0        0    10614 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/keywords/Image.py
--rw-r--r--   0        0        0     3751 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/keywords/PDF.py
--rw-r--r--   0        0        0     4466 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/keywords/Tesseract.py
--rw-r--r--   0        0        0      166 2022-10-04 11:45:19.123792 WatchUI-2.0.8/WatchUI/keywords/__init__.py
--rw-r--r--   0        0        0     1228 2022-10-04 11:45:19.251798 WatchUI-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 WatchUI-2.0.8/setup.py
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 WatchUI-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1139 2022-11-18 05:55:24.473348 watchui-2.0.9/LICENSE
+-rw-r--r--   0        0        0     2691 2022-11-18 05:55:24.473348 watchui-2.0.9/README.md
+-rw-r--r--   0        0        0     5679 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/Ibasic/IBasic.py
+-rw-r--r--   0        0        0       78 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/Ibasic/__init__.py
+-rw-r--r--   0        0        0     2229 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/WatchUI.py
+-rw-r--r--   0        0        0       36 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/__init__.py
+-rw-r--r--   0        0        0    10614 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/keywords/Image.py
+-rw-r--r--   0        0        0     3751 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/keywords/PDF.py
+-rw-r--r--   0        0        0     4466 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/keywords/Tesseract.py
+-rw-r--r--   0        0        0      166 2022-11-18 05:55:24.473348 watchui-2.0.9/WatchUI/keywords/__init__.py
+-rw-r--r--   0        0        0     1228 2022-11-18 05:55:24.597348 watchui-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 watchui-2.0.9/setup.py
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 watchui-2.0.9/PKG-INFO
```

### Comparing `WatchUI-2.0.8/LICENSE` & `watchui-2.0.9/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
+# MIT License
 
-Copyright (c) 2020 Jan Egermaier, Radek Bednarik, Marcel Veselka, Michal Jirka
+Copyright (c) 2022 Jan Egermaier, Radek Bednarik, Marcel Veselka, Michal Jirka
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `WatchUI-2.0.8/README.md` & `watchui-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/WatchUI/Ibasic/IBasic.py` & `watchui-2.0.9/WatchUI/Ibasic/IBasic.py`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/WatchUI/WatchUI.py` & `watchui-2.0.9/WatchUI/WatchUI.py`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/WatchUI/keywords/Image.py` & `watchui-2.0.9/WatchUI/keywords/Image.py`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/WatchUI/keywords/PDF.py` & `watchui-2.0.9/WatchUI/keywords/PDF.py`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/WatchUI/keywords/Tesseract.py` & `watchui-2.0.9/WatchUI/keywords/Tesseract.py`

 * *Files identical despite different names*

### Comparing `WatchUI-2.0.8/pyproject.toml` & `watchui-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WatchUI"
-version = "2.0.8"
+version = "2.0.9"
 description = "RobotFramework library package for automated visual testing."
 readme = "README.md"
 repository = "https://github.com/Tesena-smart-testing/WatchUI"
 documentation = "https://tesena-smart-testing.github.io/WatchUI/"
 authors = ["Jan Egermaier <jan.egermaier@tesena.com>", "Radek Bednarik <radek.bednarik@tesena.com>", "Michal Jirka <michal.jirka@tesena.com>", "Marcel Veselka <marcel.veselka@tesena.com>"]
 license = "MIT"
 classifiers = [
```

### Comparing `WatchUI-2.0.8/setup.py` & `watchui-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn']
 
 entry_points = \
 {'console_scripts': ['docs = tasks:docs', 'test = tasks:test']}
 
 setup_kwargs = {
     'name': 'watchui',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': 'RobotFramework library package for automated visual testing.',
     'long_description': '# WatchUI\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## [Documentation](https://tesena-smart-testing.github.io/WatchUI/) | [Tesena](https://www.tesena.com/) | [Pypi](https://pypi.org/project/WatchUI/)\n\n## Important notice for users\n\nWatchUI 2.0 brings breaking changes. Dev team decided to streamline the library and focus it solely on the image and text comparison. This allows us to remove the implicit dependency on browser automation libraries - namely SeleniumLibrary, which was implicit part of the library via RF `BuiltIn()` import of the SeleniumLibrary instance.\n\nThis is no longer the case - user of the WatchUI therefore **can and have to choose, what UI automation library will use** and provide screenshots to the WatchUI keywords to be compared. It could be now used with SeleniumLibrary, Browser library, Sikuli, Appium or any other UI library where visual validation is required.\n\nVersion 1.x.x is no longer supported, but it is still available on [Pypi](pip install WatchUI==1.0.11).\n\n### Basic Info\n\nCustom library for works with image, pdf and tesseract with RF.\n\n### Folder structure\n\n```\nWatchUI\n└── .github/workflows           # Folder with CI for github actions\n└── assets                      # Folder with images used for documantation as well as test data\n└── test                        # Folder with example how to write rf test.\n│    └── unit_tests             # Pytest unit test cases\n│    └── test.robot             # File with simeple Robot Framework TCs\n└── WatchUI                     # Folder with WatchUI library\n│    └── WatchUI.py             # Main library file\n│    └── IBasics                # Basic utilities and error handling\n│    └── Keywords               # Keywords for working with images, PDFs and text(tesseract)\n└── README.MD                   # Here you are :-)\n└── setup.py                    # File for easy setup use with pip install .\n```\n\n### Install\n\nYou can find detail in [Documentation](https://procesor2017.github.io/WatchUI/) but basically use pip:\n\n```\npip install WatchUI\n```\n\nor some python dependencies management tools, like [pipenv](https://pipenv.pypa.io/en/latest/) or [poetry](https://python-poetry.org/) and their respective methods of libraries installation.\n\n### Sample results\n\n_Image where the differences are stored + You can see two black box in left corner. These black box are ignored during comparison._\n\n<img src="assets/example-ignore-areas.png">\n\n_The red rectangles outlining missing elements on compared screens_\n\n<img src="assets/example-difference.jpg">\n',
     'author': 'Jan Egermaier',
     'author_email': 'jan.egermaier@tesena.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Tesena-smart-testing/WatchUI',
```

### Comparing `WatchUI-2.0.8/PKG-INFO` & `watchui-2.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: watchui
-Version: 2.0.8
+Version: 2.0.9
 Summary: RobotFramework library package for automated visual testing.
 Home-page: https://github.com/Tesena-smart-testing/WatchUI
 License: MIT
 Author: Jan Egermaier
 Author-email: jan.egermaier@tesena.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Pillow
 Requires-Dist: PyMuPDF
 Requires-Dist: imutils
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pandas
```

