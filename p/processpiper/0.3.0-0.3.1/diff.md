# Comparing `tmp/processpiper-0.3.0.tar.gz` & `tmp/processpiper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.3.0.tar", last modified: Fri Apr 21 09:16:03 2023, max compression
+gzip compressed data, was "processpiper-0.3.1.tar", last modified: Fri Apr 28 09:04:09 2023, max compression
```

## Comparing `processpiper-0.3.0.tar` & `processpiper-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.038380 processpiper-0.3.0/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6245 2023-04-21 09:16:03.037380 processpiper-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-04-21 09:15:30.000000 processpiper-0.3.0/README.md
--rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 09:16:03.038380 processpiper-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.007374 processpiper-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.022377 processpiper-0.3.0/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.3.0/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.3.0/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.3.0/src/processpiper/constants.py
--rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.3.0/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.3.0/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.3.0/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.3.0/src/processpiper/helper.py
--rw-rw-rw-   0        0        0    10689 2023-04-21 08:45:10.000000 processpiper-0.3.0/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    35665 2023-04-21 04:25:43.000000 processpiper-0.3.0/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    18855 2023-04-21 08:59:35.000000 processpiper-0.3.0/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    19242 2023-04-21 08:51:52.000000 processpiper-0.3.0/src/processpiper/shape.py
--rw-rw-rw-   0        0        0     9016 2023-04-21 09:05:31.000000 processpiper-0.3.0/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.3.0/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-04-21 06:29:34.000000 processpiper-0.3.0/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.035380 processpiper-0.3.0/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6245 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-21 09:16:03.000000 processpiper-0.3.0/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-21 09:16:02.000000 processpiper-0.3.0/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:03.036380 processpiper-0.3.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.3.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.3.0/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.940065 processpiper-0.3.1/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6365 2023-04-28 09:04:09.940065 processpiper-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5810 2023-04-28 09:03:44.000000 processpiper-0.3.1/README.md
+-rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 09:04:09.941065 processpiper-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.905741 processpiper-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.922059 processpiper-0.3.1/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.3.1/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.3.1/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.3.1/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.3.1/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.3.1/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.3.1/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.3.1/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0    10689 2023-04-21 08:45:10.000000 processpiper-0.3.1/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    35665 2023-04-21 04:25:43.000000 processpiper-0.3.1/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    18885 2023-04-28 08:53:46.000000 processpiper-0.3.1/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    19242 2023-04-21 08:51:52.000000 processpiper-0.3.1/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0     9395 2023-04-28 08:56:59.000000 processpiper-0.3.1/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.3.1/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-04-28 08:23:04.000000 processpiper-0.3.1/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.937064 processpiper-0.3.1/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6365 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.939064 processpiper-0.3.1/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.3.1/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/tests/github_action_test.py
```

### Comparing `processpiper-0.3.0/LICENSE` & `processpiper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/PKG-INFO` & `processpiper-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.3.0
+Version: 0.3.1
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 ![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+![CI](https://github.com/csgoh/processpiper/actions/workflows/python-package.yml/badge.svg)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
@@ -75,14 +76,15 @@
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
+colourtheme: BLUEMOUNTAIN
     lane: End User
         (start) as start
         [Enter Keyword] as enter_keyword
         (end) as end
 pool: System Search
     lane: Database System
         [Login] as login
```

### Comparing `processpiper-0.3.0/README.md` & `processpiper-0.3.1/src/processpiper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+Metadata-Version: 2.1
+Name: processpiper
+Version: 0.3.1
+Summary: Processpiper. An open source python library to generate business process diagram using code.
+Author: CS Goh
+Project-URL: Homepage, https://github.com/csgoh/processpiper
+Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
 ![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+![CI](https://github.com/csgoh/processpiper/actions/workflows/python-package.yml/badge.svg)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
@@ -61,14 +76,15 @@
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
+colourtheme: BLUEMOUNTAIN
     lane: End User
         (start) as start
         [Enter Keyword] as enter_keyword
         (end) as end
 pool: System Search
     lane: Database System
         [Login] as login
```

### Comparing `processpiper-0.3.0/pyproject.toml` & `processpiper-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/activity.py` & `processpiper-0.3.1/src/processpiper/activity.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/colourtheme.py` & `processpiper-0.3.1/src/processpiper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/constants.py` & `processpiper-0.3.1/src/processpiper/constants.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/event.py` & `processpiper-0.3.1/src/processpiper/event.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/footer.py` & `processpiper-0.3.1/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/gateway.py` & `processpiper-0.3.1/src/processpiper/gateway.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/helper.py` & `processpiper-0.3.1/src/processpiper/helper.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/lane.py` & `processpiper-0.3.1/src/processpiper/lane.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/painter.py` & `processpiper-0.3.1/src/processpiper/painter.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/pool.py` & `processpiper-0.3.1/src/processpiper/pool.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/processmap.py` & `processpiper-0.3.1/src/processpiper/processmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .title import Title
 from .footer import Footer
 from .constants import Configs
 from .helper import Helper
 from PIL import Image
 import time
 import logging
+import PIL
 
 
 class UnconnectedElementException(Exception):
     pass
 
 
 class EmptyProcessMapException(Exception):
@@ -483,17 +484,18 @@
     def save(self, filename: str) -> None:
         """This method saves the process map to a file"""
         self.__painter.save_surface(filename)
 
         elapsed_time = (time.time() - self.start_time) * 1000
         Helper.info_log(f"Took [{elapsed_time:.2f}ms] to generate '{filename}' diagram")
 
-    # def get_image(self) -> Image:
-    #     """This method returns the process map image"""
-    #     return self.__painter.get_image()
+    def getImage(self) -> PIL.Image:
+        """This method returns the process map image"""
+        image = self.__painter.__surface
+        return image
 
     def __enter__(self):
         """This method is called when the 'with' statement is used"""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """This method is called when the 'with' statement is used"""
```

### Comparing `processpiper-0.3.0/src/processpiper/shape.py` & `processpiper-0.3.1/src/processpiper/shape.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/text2diagram.py` & `processpiper-0.3.1/src/processpiper/text2diagram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import datetime
 import re
+import os
 from processpiper.helper import Helper
 from PIL import Image
 
 
 def parse_and_generate_code(input_str, png_output_file):
     """
     Parse input string and generate code to create a diagram
     """
 
-    lines = input_str.strip().split("\n")
+    # lines = input_str.strip().split("\n")
+    lines = [
+        line.strip()
+        for line in input_str.strip().split("\n")
+        if not line.startswith("#") and line.strip()
+    ]
+
     process_map_title = parse_title(lines)
 
     if len(lines) == 0:
         raise ValueError(
             "No business process definition found. Please add pool(s), lane(s) and element(s)."
         )
 
@@ -233,21 +240,27 @@
     ### If a multiline code does not contain add_element, raise error
     if "add_element" not in code:
         raise ValueError("There is no element defined. Please add elements to lane.")
 
 
 def render(text: str, png_output_file: str = ""):
     """Render text to diagram"""
+    output_file_provided = True
     if png_output_file.strip() == "":
+        output_file_provided = False
         # add datetime to the file name
         png_output_file = (
             f"piper_{datetime.datetime.now().strftime('%Y%m%d_%H%M%S')}.png"
         )
 
     generated_code = parse_and_generate_code(text, png_output_file)
     validate_generated_code(generated_code)
     # show_code_with_line_number(generated_code)
     # print(generated_code)
     exec(generated_code)
     generated_image = Image.open(png_output_file)
+    generated_image.load()
+    # Clean up the generated image file
+    if output_file_provided == False:
+        os.remove(png_output_file)
 
     return generated_code, generated_image
```

### Comparing `processpiper-0.3.0/src/processpiper/title.py` & `processpiper-0.3.1/src/processpiper/title.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/processpiper/version.py` & `processpiper-0.3.1/src/processpiper/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Version information for processpiper."""
-__version__ = "v0.3.0"
+__version__ = "v0.3.1"
```

### Comparing `processpiper-0.3.0/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.3.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-Metadata-Version: 2.1
-Name: processpiper
-Version: 0.3.0
-Summary: Processpiper. An open source python library to generate business process diagram using code.
-Author: CS Goh
-Project-URL: Homepage, https://github.com/csgoh/processpiper
-Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
 ![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
 ![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
 ![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+![CI](https://github.com/csgoh/processpiper/actions/workflows/python-package.yml/badge.svg)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
@@ -75,14 +62,15 @@
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
+colourtheme: BLUEMOUNTAIN
     lane: End User
         (start) as start
         [Enter Keyword] as enter_keyword
         (end) as end
 pool: System Search
     lane: Database System
         [Login] as login
```

### Comparing `processpiper-0.3.0/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.3.1/src/processpiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.0/src/tests/github_action_test.py` & `processpiper-0.3.1/src/tests/github_action_test.py`

 * *Files identical despite different names*

