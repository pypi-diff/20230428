# Comparing `tmp/ASCIIcli-0.0.4.tar.gz` & `tmp/ASCIIcli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.4.tar", last modified: Fri Apr 28 07:22:15 2023, max compression
+gzip compressed data, was "ASCIIcli-0.0.5.tar", last modified: Fri Apr 28 07:32:39 2023, max compression
```

## Comparing `ASCIIcli-0.0.4.tar` & `ASCIIcli-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.611592 ASCIIcli-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.585593 ASCIIcli-0.0.4/ASCIIcli.egg-info/
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 07:22:15.000000 ASCIIcli-0.0.4/ASCIIcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2526 2023-04-28 07:22:15.608597 ASCIIcli-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2031 2023-04-28 06:58:31.000000 ASCIIcli-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.599593 ASCIIcli-0.0.4/asciicli/
--rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.4/asciicli/__init__.py
--rw-rw-rw-   0        0        0     1583 2023-04-28 07:20:03.000000 ASCIIcli-0.0.4/asciicli/__main__.py
--rw-rw-rw-   0        0        0     3280 2023-04-28 07:20:33.000000 ASCIIcli-0.0.4/asciicli/functions.py
--rw-rw-rw-   0        0        0       42 2023-04-28 07:22:15.611592 ASCIIcli-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-04-28 07:21:20.000000 ASCIIcli-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:22:15.601612 ASCIIcli-0.0.4/tests/
--rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.4/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:32:39.188849 ASCIIcli-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-04-28 07:32:39.151849 ASCIIcli-0.0.5/ASCIIcli.egg-info/
+-rw-rw-rw-   0        0        0     2543 2023-04-28 07:32:38.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 07:32:39.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 07:32:38.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-28 07:32:38.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 07:32:38.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 07:32:38.000000 ASCIIcli-0.0.5/ASCIIcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2543 2023-04-28 07:32:39.185845 ASCIIcli-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2048 2023-04-28 07:32:04.000000 ASCIIcli-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 07:32:39.171847 ASCIIcli-0.0.5/asciicli/
+-rw-rw-rw-   0        0        0      230 2023-04-28 06:56:27.000000 ASCIIcli-0.0.5/asciicli/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-04-28 07:20:03.000000 ASCIIcli-0.0.5/asciicli/__main__.py
+-rw-rw-rw-   0        0        0     3289 2023-04-28 07:32:01.000000 ASCIIcli-0.0.5/asciicli/functions.py
+-rw-rw-rw-   0        0        0       42 2023-04-28 07:32:39.188849 ASCIIcli-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-04-28 07:25:50.000000 ASCIIcli-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 07:32:39.183849 ASCIIcli-0.0.5/tests/
+-rw-rw-rw-   0        0        0     2640 2023-04-28 06:56:13.000000 ASCIIcli-0.0.5/tests/tests.py
```

### Comparing `ASCIIcli-0.0.4/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.0.5/ASCIIcli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -32,17 +32,19 @@
 
 ---
 
 ## Usage
 
 `asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
-Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
-Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
-Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
+Set 1: A -> Z
+Set 2: 0 -> 9
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
 If you have downloaded the application through pip input the following command in the terminal:
 `asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
 
 If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
```

### Comparing `ASCIIcli-0.0.4/LICENSE` & `ASCIIcli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.4/PKG-INFO` & `ASCIIcli-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCIIcli
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/asciicli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -32,17 +32,19 @@
 
 ---
 
 ## Usage
 
 `asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
-Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
-Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
-Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
+Set 1: A -> Z
+Set 2: 0 -> 9
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
 If you have downloaded the application through pip input the following command in the terminal:
 `asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
 
 If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
```

### Comparing `ASCIIcli-0.0.4/README.md` & `ASCIIcli-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 
 ---
 
 ## Usage
 
 `asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
 
-Set 1: /, !, =, +, |, #, %,@, 0-9, ?, [, ], {, }, A-Z.  
-Set 2: 0, O, o, 8, 9, 6, @, &, ., ", :.  
-Set 3: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █.
+Set 1: A -> Z
+Set 2: 0 -> 9
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =
 
 **_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
 
 If you have downloaded the application through pip input the following command in the terminal:
 `asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
 
 If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
```

### Comparing `ASCIIcli-0.0.4/asciicli/__main__.py` & `ASCIIcli-0.0.5/asciicli/__main__.py`

 * *Files identical despite different names*

### Comparing `ASCIIcli-0.0.4/asciicli/functions.py` & `ASCIIcli-0.0.5/asciicli/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PIL import Image
 
 # define characters used
 char_a = list(string.ascii_uppercase)
 char_b = list(string.digits)
 char_c = ["0", "O", "o", "8", "9", "6", "@", "&", ":", '"', "."]
 char_d = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
-char_e = ['/', '!', '=', '+', '|', '#', '%', '@', '=', '?', '[', ']',]
+char_e = ['!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+', '-', '+']
 
 
 def get_char_set(set_choice):
     """
     Uses choice for character set by number and then returns the chosen set to.
     """
```

### Comparing `ASCIIcli-0.0.4/setup.py` & `ASCIIcli-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ASCIIcli",
     author="mrq-andras",
-    version="0.0.4",
+    version="0.0.5",
     packages=['asciicli'],
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
```

### Comparing `ASCIIcli-0.0.4/tests/tests.py` & `ASCIIcli-0.0.5/tests/tests.py`

 * *Files identical despite different names*

