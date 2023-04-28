# Comparing `tmp/ASCIIcli-0.0.7.tar.gz` & `tmp/ASCIIcli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCIIcli-0.0.7.tar", last modified: Fri Apr 28 08:28:14 2023, max compression
+gzip compressed data, was "ASCIIcli-0.0.9.tar", last modified: Fri Apr 28 09:26:49 2023, max compression
```

## Comparing `ASCIIcli-0.0.7.tar` & `ASCIIcli-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.518463 ASCIIcli-0.0.7/ASCIIcli.egg-info/
--rw-rw-rw-   0        0        0     2553 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 08:28:14.000000 ASCIIcli-0.0.7/ASCIIcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-28 06:51:27.000000 ASCIIcli-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2553 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2058 2023-04-28 07:35:43.000000 ASCIIcli-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 08:28:14.570829 ASCIIcli-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-04-28 08:27:50.000000 ASCIIcli-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.565207 ASCIIcli-0.0.7/src/
--rw-rw-rw-   0        0        0      225 2023-04-28 08:20:42.000000 ASCIIcli-0.0.7/src/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-04-28 08:19:56.000000 ASCIIcli-0.0.7/src/__main__.py
--rw-rw-rw-   0        0        0     3289 2023-04-28 08:22:09.000000 ASCIIcli-0.0.7/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-28 08:28:14.565207 ASCIIcli-0.0.7/tests/
--rw-rw-rw-   0        0        0     2635 2023-04-28 08:20:33.000000 ASCIIcli-0.0.7/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.914813 ASCIIcli-0.0.9/ASCIIcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 09:26:49.000000 ASCIIcli-0.0.9/ASCIIcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/src/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:26:49.918814 ASCIIcli-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-28 09:26:34.000000 ASCIIcli-0.0.9/tests/tests.py
```

### Comparing `ASCIIcli-0.0.7/ASCIIcli.egg-info/PKG-INFO` & `ASCIIcli-0.0.9/ASCIIcli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: ASCIIcli
-Version: 0.0.7
-Summary: A command-line tool that converts images to ASCII art.
-Home-page: https://github.com/mrq-andras/asciicli
-Author: mrq-andras
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Command Line ASCII Art Generator
-
-ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
-
----
-
-## Installation & Building
-
-### PIP
-
-The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
-You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
-
-### Releases
-
-If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
-
----
-
-## Usage
-
-`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
-
-Set 1: A -> Z  
-Set 2: 0 -> 9  
-Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
-Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
-Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
-
-**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
-
-If you have downloaded the application through pip input the following command in the terminal:
-`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
-`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
-
-Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
-
----
-[`LICENSE`](./LICENSE)
+Metadata-Version: 2.1
+Name: ASCIIcli
+Version: 0.0.9
+Summary: A command-line tool that converts images to ASCII art.
+Home-page: https://github.com/mrq-andras/asciicli
+Author: mrq-andras
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Command Line ASCII Art Generator
+
+ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
+
+---
+
+## Installation & Building
+
+### PIP
+
+The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
+You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
+
+### Releases
+
+If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
+
+---
+
+## Usage
+
+`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
+
+Set 1: A -> Z  
+Set 2: 0 -> 9  
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
+
+**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
+
+If you have downloaded the application through pip input the following command in the terminal:
+`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
+`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
+
+Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
+
+---
+[`LICENSE`](./LICENSE)
```

### Comparing `ASCIIcli-0.0.7/LICENSE` & `ASCIIcli-0.0.9/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-00000000: 0d0a 2320 4d49 5420 4c69 6365 6e73 650d  ..# MIT License.
-00000010: 0a0d 0a43 6f70 7972 6967 6874 2028 6329  ...Copyright (c)
-00000020: 205b 3230 3233 5d20 5b41 4e44 5241 535d   [2023] [ANDRAS]
-00000030: 0d0a 0d0a 5065 726d 6973 7369 6f6e 2069  ....Permission i
-00000040: 7320 6865 7265 6279 2067 7261 6e74 6564  s hereby granted
-00000050: 2c20 6672 6565 206f 6620 6368 6172 6765  , free of charge
-00000060: 2c20 746f 2061 6e79 2070 6572 736f 6e20  , to any person 
-00000070: 6f62 7461 696e 696e 6720 6120 636f 7079  obtaining a copy
-00000080: 0d0a 6f66 2074 6869 7320 736f 6674 7761  ..of this softwa
-00000090: 7265 2061 6e64 2061 7373 6f63 6961 7465  re and associate
-000000a0: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-000000b0: 6669 6c65 7320 2874 6865 2022 536f 6674  files (the "Soft
-000000c0: 7761 7265 2229 2c20 746f 2064 6561 6c0d  ware"), to deal.
-000000d0: 0a69 6e20 7468 6520 536f 6674 7761 7265  .in the Software
-000000e0: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
-000000f0: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
-00000100: 7769 7468 6f75 7420 6c69 6d69 7461 7469  without limitati
-00000110: 6f6e 2074 6865 2072 6967 6874 730d 0a74  on the rights..t
-00000120: 6f20 7573 652c 2063 6f70 792c 206d 6f64  o use, copy, mod
-00000130: 6966 792c 206d 6572 6765 2c20 7075 626c  ify, merge, publ
-00000140: 6973 682c 2064 6973 7472 6962 7574 652c  ish, distribute,
-00000150: 2073 7562 6c69 6365 6e73 652c 2061 6e64   sublicense, and
-00000160: 2f6f 7220 7365 6c6c 0d0a 636f 7069 6573  /or sell..copies
-00000170: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-00000180: 2c20 616e 6420 746f 2070 6572 6d69 7420  , and to permit 
-00000190: 7065 7273 6f6e 7320 746f 2077 686f 6d20  persons to whom 
-000001a0: 7468 6520 536f 6674 7761 7265 2069 730d  the Software is.
-000001b0: 0a66 7572 6e69 7368 6564 2074 6f20 646f  .furnished to do
-000001c0: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
-000001d0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-000001e0: 6e64 6974 696f 6e73 3a0d 0a0d 0a54 6865  nditions:....The
-000001f0: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
-00000200: 206e 6f74 6963 6520 616e 6420 7468 6973   notice and this
-00000210: 2070 6572 6d69 7373 696f 6e20 6e6f 7469   permission noti
-00000220: 6365 2073 6861 6c6c 2062 6520 696e 636c  ce shall be incl
-00000230: 7564 6564 2069 6e20 616c 6c0d 0a63 6f70  uded in all..cop
-00000240: 6965 7320 6f72 2073 7562 7374 616e 7469  ies or substanti
-00000250: 616c 2070 6f72 7469 6f6e 7320 6f66 2074  al portions of t
-00000260: 6865 2053 6f66 7477 6172 652e 0d0a 0d0a  he Software.....
-00000270: 5448 4520 534f 4654 5741 5245 2049 5320  THE SOFTWARE IS 
-00000280: 5052 4f56 4944 4544 2022 4153 2049 5322  PROVIDED "AS IS"
-00000290: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
-000002a0: 5459 204f 4620 414e 5920 4b49 4e44 2c20  TY OF ANY KIND, 
-000002b0: 4558 5052 4553 5320 4f52 0d0a 494d 504c  EXPRESS OR..IMPL
-000002c0: 4945 442c 2049 4e43 4c55 4449 4e47 2042  IED, INCLUDING B
-000002d0: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
-000002e0: 4f20 5448 4520 5741 5252 414e 5449 4553  O THE WARRANTIES
-000002f0: 204f 4620 4d45 5243 4841 4e54 4142 494c   OF MERCHANTABIL
-00000300: 4954 592c 0d0a 4649 544e 4553 5320 464f  ITY,..FITNESS FO
-00000310: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-00000320: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
-00000330: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
-00000340: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
-00000350: 450d 0a41 5554 484f 5253 204f 5220 434f  E..AUTHORS OR CO
-00000360: 5059 5249 4748 5420 484f 4c44 4552 5320  PYRIGHT HOLDERS 
-00000370: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
-00000380: 5920 434c 4149 4d2c 2044 414d 4147 4553  Y CLAIM, DAMAGES
-00000390: 204f 5220 4f54 4845 520d 0a4c 4941 4249   OR OTHER..LIABI
-000003a0: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-000003b0: 2041 4e20 4143 5449 4f4e 204f 4620 434f   AN ACTION OF CO
-000003c0: 4e54 5241 4354 2c20 544f 5254 204f 5220  NTRACT, TORT OR 
-000003d0: 4f54 4845 5257 4953 452c 2041 5249 5349  OTHERWISE, ARISI
-000003e0: 4e47 2046 524f 4d2c 0d0a 4f55 5420 4f46  NG FROM,..OUT OF
-000003f0: 204f 5220 494e 2043 4f4e 4e45 4354 494f   OR IN CONNECTIO
-00000400: 4e20 5749 5448 2054 4845 2053 4f46 5457  N WITH THE SOFTW
-00000410: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
-00000420: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
-00000430: 2049 4e20 5448 450d 0a53 4f46 5457 4152   IN THE..SOFTWAR
-00000440: 452e 0d0a                                E...
+00000000: 0a23 204d 4954 204c 6963 656e 7365 0a0a  .# MIT License..
+00000010: 436f 7079 7269 6768 7420 2863 2920 5b32  Copyright (c) [2
+00000020: 3032 335d 205b 414e 4452 4153 5d0a 0a50  023] [ANDRAS]..P
+00000030: 6572 6d69 7373 696f 6e20 6973 2068 6572  ermission is her
+00000040: 6562 7920 6772 616e 7465 642c 2066 7265  eby granted, fre
+00000050: 6520 6f66 2063 6861 7267 652c 2074 6f20  e of charge, to 
+00000060: 616e 7920 7065 7273 6f6e 206f 6274 6169  any person obtai
+00000070: 6e69 6e67 2061 2063 6f70 790a 6f66 2074  ning a copy.of t
+00000080: 6869 7320 736f 6674 7761 7265 2061 6e64  his software and
+00000090: 2061 7373 6f63 6961 7465 6420 646f 6375   associated docu
+000000a0: 6d65 6e74 6174 696f 6e20 6669 6c65 7320  mentation files 
+000000b0: 2874 6865 2022 536f 6674 7761 7265 2229  (the "Software")
+000000c0: 2c20 746f 2064 6561 6c0a 696e 2074 6865  , to deal.in the
+000000d0: 2053 6f66 7477 6172 6520 7769 7468 6f75   Software withou
+000000e0: 7420 7265 7374 7269 6374 696f 6e2c 2069  t restriction, i
+000000f0: 6e63 6c75 6469 6e67 2077 6974 686f 7574  ncluding without
+00000100: 206c 696d 6974 6174 696f 6e20 7468 6520   limitation the 
+00000110: 7269 6768 7473 0a74 6f20 7573 652c 2063  rights.to use, c
+00000120: 6f70 792c 206d 6f64 6966 792c 206d 6572  opy, modify, mer
+00000130: 6765 2c20 7075 626c 6973 682c 2064 6973  ge, publish, dis
+00000140: 7472 6962 7574 652c 2073 7562 6c69 6365  tribute, sublice
+00000150: 6e73 652c 2061 6e64 2f6f 7220 7365 6c6c  nse, and/or sell
+00000160: 0a63 6f70 6965 7320 6f66 2074 6865 2053  .copies of the S
+00000170: 6f66 7477 6172 652c 2061 6e64 2074 6f20  oftware, and to 
+00000180: 7065 726d 6974 2070 6572 736f 6e73 2074  permit persons t
+00000190: 6f20 7768 6f6d 2074 6865 2053 6f66 7477  o whom the Softw
+000001a0: 6172 6520 6973 0a66 7572 6e69 7368 6564  are is.furnished
+000001b0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
+000001c0: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
+000001d0: 696e 6720 636f 6e64 6974 696f 6e73 3a0a  ing conditions:.
+000001e0: 0a54 6865 2061 626f 7665 2063 6f70 7972  .The above copyr
+000001f0: 6967 6874 206e 6f74 6963 6520 616e 6420  ight notice and 
+00000200: 7468 6973 2070 6572 6d69 7373 696f 6e20  this permission 
+00000210: 6e6f 7469 6365 2073 6861 6c6c 2062 6520  notice shall be 
+00000220: 696e 636c 7564 6564 2069 6e20 616c 6c0a  included in all.
+00000230: 636f 7069 6573 206f 7220 7375 6273 7461  copies or substa
+00000240: 6e74 6961 6c20 706f 7274 696f 6e73 206f  ntial portions o
+00000250: 6620 7468 6520 536f 6674 7761 7265 2e0a  f the Software..
+00000260: 0a54 4845 2053 4f46 5457 4152 4520 4953  .THE SOFTWARE IS
+00000270: 2050 524f 5649 4445 4420 2241 5320 4953   PROVIDED "AS IS
+00000280: 222c 2057 4954 484f 5554 2057 4152 5241  ", WITHOUT WARRA
+00000290: 4e54 5920 4f46 2041 4e59 204b 494e 442c  NTY OF ANY KIND,
+000002a0: 2045 5850 5245 5353 204f 520a 494d 504c   EXPRESS OR.IMPL
+000002b0: 4945 442c 2049 4e43 4c55 4449 4e47 2042  IED, INCLUDING B
+000002c0: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
+000002d0: 4f20 5448 4520 5741 5252 414e 5449 4553  O THE WARRANTIES
+000002e0: 204f 4620 4d45 5243 4841 4e54 4142 494c   OF MERCHANTABIL
+000002f0: 4954 592c 0a46 4954 4e45 5353 2046 4f52  ITY,.FITNESS FOR
+00000300: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
+00000310: 5250 4f53 4520 414e 4420 4e4f 4e49 4e46  RPOSE AND NONINF
+00000320: 5249 4e47 454d 454e 542e 2049 4e20 4e4f  RINGEMENT. IN NO
+00000330: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
+00000340: 0a41 5554 484f 5253 204f 5220 434f 5059  .AUTHORS OR COPY
+00000350: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
+00000360: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
+00000370: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
+00000380: 5220 4f54 4845 520a 4c49 4142 494c 4954  R OTHER.LIABILIT
+00000390: 592c 2057 4845 5448 4552 2049 4e20 414e  Y, WHETHER IN AN
+000003a0: 2041 4354 494f 4e20 4f46 2043 4f4e 5452   ACTION OF CONTR
+000003b0: 4143 542c 2054 4f52 5420 4f52 204f 5448  ACT, TORT OR OTH
+000003c0: 4552 5749 5345 2c20 4152 4953 494e 4720  ERWISE, ARISING 
+000003d0: 4652 4f4d 2c0a 4f55 5420 4f46 204f 5220  FROM,.OUT OF OR 
+000003e0: 494e 2043 4f4e 4e45 4354 494f 4e20 5749  IN CONNECTION WI
+000003f0: 5448 2054 4845 2053 4f46 5457 4152 4520  TH THE SOFTWARE 
+00000400: 4f52 2054 4845 2055 5345 204f 5220 4f54  OR THE USE OR OT
+00000410: 4845 5220 4445 414c 494e 4753 2049 4e20  HER DEALINGS IN 
+00000420: 5448 450a 534f 4654 5741 5245 2e0a       THE.SOFTWARE..
```

### Comparing `ASCIIcli-0.0.7/PKG-INFO` & `ASCIIcli-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: ASCIIcli
-Version: 0.0.7
-Summary: A command-line tool that converts images to ASCII art.
-Home-page: https://github.com/mrq-andras/asciicli
-Author: mrq-andras
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Command Line ASCII Art Generator
-
-ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
-
----
-
-## Installation & Building
-
-### PIP
-
-The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
-You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
-
-### Releases
-
-If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
-
----
-
-## Usage
-
-`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
-
-Set 1: A -> Z  
-Set 2: 0 -> 9  
-Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
-Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
-Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
-
-**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
-
-If you have downloaded the application through pip input the following command in the terminal:
-`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
-`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
-
-Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
-
----
-[`LICENSE`](./LICENSE)
+Metadata-Version: 2.1
+Name: ASCIIcli
+Version: 0.0.9
+Summary: A command-line tool that converts images to ASCII art.
+Home-page: https://github.com/mrq-andras/asciicli
+Author: mrq-andras
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Command Line ASCII Art Generator
+
+ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
+
+---
+
+## Installation & Building
+
+### PIP
+
+The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
+You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
+
+### Releases
+
+If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
+
+---
+
+## Usage
+
+`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
+
+Set 1: A -> Z  
+Set 2: 0 -> 9  
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
+
+**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
+
+If you have downloaded the application through pip input the following command in the terminal:
+`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
+`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
+
+Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
+
+---
+[`LICENSE`](./LICENSE)
```

### Comparing `ASCIIcli-0.0.7/README.md` & `ASCIIcli-0.0.9/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Command Line ASCII Art Generator
-
-ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
-
----
-
-## Installation & Building
-
-### PIP
-
-The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
-You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
-
-### Releases
-
-If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
-
----
-
-## Usage
-
-`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
-
-Set 1: A -> Z  
-Set 2: 0 -> 9  
-Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
-Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
-Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
-
-**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
-
-If you have downloaded the application through pip input the following command in the terminal:
-`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
-`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
-
-This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
-
-Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
-
----
-[`LICENSE`](./LICENSE)
+# Command Line ASCII Art Generator
+
+ASCIIcli is a command line interface that is powered by Python3. You can generate ASCII art by importing an image and then selecting the character set that you want to generate with.
+
+---
+
+## Installation & Building
+
+### PIP
+
+The easiest way to install ASCIIcli is by using the [PyPI library](https://pypi.org/project/asciicli/).
+You can run `pip install ASCIIcli` on any command-line with Python3 in order to install it.
+
+### Releases
+
+If you are unable to use the PyPI library you can access ASCIIcli by going to our [releases page](https://github.com/mrq-andras/asciicli/releases). There you can download the .exe file and run the CLI by going to the folder that the program is downloaded in and running `.\asciicli`
+
+---
+
+## Usage
+
+`asciicli [-h] [--width] [--height] [--set] [--random] [--invert] [--darkness] C:/full/path/to/your/image`
+
+Set 1: A -> Z  
+Set 2: 0 -> 9  
+Set 3: 0, O, o, 8, 9, 6, @, &, ., ", :  
+Set 4: ▀, ▄, ▌, ▐, ■, ◽, ◆, ►, ●, ░, ▒, ▓, █  
+Set 5: !, @, #, $, %, ^, &, *, (, ), _, +, -, =  
+
+**_NOTE: SET 3 MIGHT NOT DISPLAY CORRECTLY IN CERTAIN FONTS OR EDITORS_**
+
+If you have downloaded the application through pip input the following command in the terminal:
+`asciicli --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+If you are running the .exe package you will need to slightly alter the command by calling the exact folder of ASCIIcli
+`.\path\to\asciicli.exe --width 40 --height 17 --set 1 --random True C:/full/path/to/your/image`
+
+This command will set the width to 40, the height to 17 and the character set to one. The `--set 1` variable is optional as the default character set is one. Random has been set to true and it will take the image from assets/input.jpg and generate a .txt file titled input-ascii.jpg in the same folder as the image.
+
+Random and Invert are boolians and must be set to True/False, whereas Darkness, Set, Height and Width are all integers.
+
+---
+[`LICENSE`](./LICENSE)
```

### Comparing `ASCIIcli-0.0.7/setup.py` & `ASCIIcli-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-"""
-This file is the setup script for the ASCIIcli module.
-This module provides a command line tool for converting images to ASCII art.
-
-To build:
-`py -m build`
-
-To build EXE:
-`pyinstaller --onefile path/to/__main__.py`
-
-To distribute:
-`twine upload dist/*`
-"""
-
-from setuptools import setup
-
-with open("README.md", "r", encoding='utf-8') as fh:
-    long_description = fh.read()
-
-setup(
-    name="ASCIIcli",
-    author="mrq-andras",
-    version="0.0.7",
-    packages=['src'],
-    install_requires=["Pillow"],
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    entry_points={
-        "console_scripts": [
-            "asciicli=src.__main__:main"
-        ]
-    },
-    python_requires=">=3.6",
-    url="https://github.com/mrq-andras/asciicli",
-    license="MIT",
-    description="A command-line tool that converts images to ASCII art.",
-    readme = "README.md"
-)
+"""
+This file is the setup script for the ASCIIcli module.
+This module provides a command line tool for converting images to ASCII art.
+
+To build:
+`py -m build`
+
+To build EXE:
+`pyinstaller --onefile path/to/__main__.py`
+
+To distribute:
+`twine upload dist/*`
+"""
+
+from setuptools import setup
+
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
+
+setup(
+    name="ASCIIcli",
+    author="mrq-andras",
+    version="0.0.9",
+    # needs to be wherever __init__.py is
+    packages=['src'],
+    install_requires=["Pillow"],
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    entry_points={
+        "console_scripts": [
+            # needs to be wherever __init__.py is
+            "asciicli=src.__main__:main"
+        ]
+    },
+    python_requires=">=3.6",
+    url="https://github.com/mrq-andras/asciicli",
+    license="MIT",
+    description="A command-line tool that converts images to ASCII art.",
+    readme = "README.md"
+)
```

### Comparing `ASCIIcli-0.0.7/src/functions.py` & `ASCIIcli-0.0.9/src/functions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-"""
-This file is the functions for the ASCIIcli module.
-This module provides a command line tool for converting images to ASCII art.
-"""
-
-import random
-import os
-import sys
-import string
-from PIL import Image
-
-# define characters used
-char_a = list(string.ascii_uppercase)
-char_b = list(string.digits)
-char_c = ["0", "O", "o", "8", "9", "6", "@", "&", ":", '"', "."]
-char_d = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
-char_e = ['-', '=', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+']
-
-
-def get_char_set(set_choice):
-    """
-    Uses choice for character set by number and then returns the chosen set to.
-    """
-
-    listed_sets = {"1": char_a, "2": char_b, "3": char_c, "4": char_d, "5": char_e}
-
-    if set_choice in listed_sets:
-        return listed_sets[set_choice]
-
-    print("Error: Invalid character set. Please choose 1, 2, 3, 4, or 5.")
-    sys.exit()
-
-
-def randomize(args):
-    """
-    If random is true randomize the character set.
-    """
-
-    char_set = get_char_set(args.set)
-    if args.random:
-        random.shuffle(char_set)
-
-
-def get_gray_value(pixel):
-    """
-    Calculates the gray value of a pixel.
-    """
-
-    return int(sum(pixel) / 2)
-
-
-def convert_to_ascii(args):
-    """
-    Converts the input image into an ASCII string.
-    """
-
-    # input is set
-    brush = int(args.darkness)
-    invert = bool(args.invert)
-    char_set = get_char_set(args.set)
-    full_path = os.path.abspath(args.path)
-
-    # set the current working directory to the one of the input image
-    os.chdir(os.path.dirname(args.path))
-
-    # run other functions
-    randomize(args)
-
-    # resize image
-    with Image.open(full_path) as image:
-        image = image.resize((args.width, args.height))
-
-    # *convert the image to ASCII art
-    ascii_art = ""
-    for y_val in range(args.height):
-        for x_val in range(args.width):
-            pixel = image.getpixel((x_val, y_val))
-            gray_value = get_gray_value(pixel)
-            if invert:
-                gray_value = 255 - gray_value
-            if gray_value >= brush:
-                ascii_char = " "
-            else:
-                index = int(gray_value / 10)
-                ascii_char = char_set[index % len(char_set)]
-            ascii_art += ascii_char
-        ascii_art += "\n"
-
-    # generate output file into text
-    # add -ascii.txt to imagename
-    file_name = args.path.split(".")[0] + "-ascii.txt"
-    output_file = os.path.join(full_path, file_name)
-    with open(output_file, "w", encoding="utf-8") as enc:
-        enc.write(ascii_art)
-
-    # print to output file
-    print(f"ASCII art written to {os.path.abspath(output_file)}")
-
-
-def print_cmd(args):
-    """
-    Prints all of the variables and the character set. (Used for development.)
-    """
-
-    char_set = get_char_set(args.set)
-    invert = bool(args.invert)
-
-    # print chosen options
-    print(f"Set {args.set} chosen.")
-    print(
-        " ".join([f"{i+1}. {char_set[i]}, " for i in range(len(char_set))])[:-2])
-    print(f"{'Randomization is on.' if args.random else 'Randomization is off.'}")
-    print(f"{'Invert is on.' if invert else 'Invert is off.'}")
+"""
+This file is the functions for the ASCIIcli module.
+This module provides a command line tool for converting images to ASCII art.
+"""
+
+import random
+import os
+import sys
+import string
+from PIL import Image
+
+# define characters used
+char_a = list(string.ascii_uppercase)
+char_b = list(string.digits)
+char_c = ["0", "O", "o", "8", "9", "6", "@", "&", ":", '"', "."]
+char_d = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
+char_e = ['-', '=', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+']
+
+
+def get_char_set(set_choice):
+    """
+    Uses choice for character set by number and then returns the chosen set to.
+    """
+
+    listed_sets = {"1": char_a, "2": char_b, "3": char_c, "4": char_d, "5": char_e}
+
+    if set_choice in listed_sets:
+        return listed_sets[set_choice]
+
+    print("Error: Invalid character set. Please choose 1, 2, 3, 4, or 5.")
+    sys.exit()
+
+
+def randomize(args):
+    """
+    If random is true randomize the character set.
+    """
+
+    char_set = get_char_set(args.set)
+    if args.random:
+        random.shuffle(char_set)
+
+
+def get_gray_value(pixel):
+    """
+    Calculates the gray value of a pixel.
+    """
+
+    return int(sum(pixel) / 2)
+
+
+def convert_to_ascii(args):
+    """
+    Converts the input image into an ASCII string.
+    """
+
+    # input is set
+    brush = int(args.darkness)
+    invert = bool(args.invert)
+    char_set = get_char_set(args.set)
+    full_path = os.path.abspath(args.path)
+
+    # set the current working directory to the one of the input image
+    os.chdir(os.path.dirname(args.path))
+
+    # run other functions
+    randomize(args)
+
+    # resize image
+    with Image.open(full_path) as image:
+        image = image.resize((args.width, args.height))
+
+    # *convert the image to ASCII art
+    ascii_art = ""
+    for y_val in range(args.height):
+        for x_val in range(args.width):
+            pixel = image.getpixel((x_val, y_val))
+            gray_value = get_gray_value(pixel)
+            if invert:
+                gray_value = 255 - gray_value
+            if gray_value >= brush:
+                ascii_char = " "
+            else:
+                index = int(gray_value / 10)
+                ascii_char = char_set[index % len(char_set)]
+            ascii_art += ascii_char
+        ascii_art += "\n"
+
+    # generate output file into text
+    # add -ascii.txt to imagename
+    file_name = args.path.split(".")[0] + "-ascii.txt"
+    output_file = os.path.join(full_path, file_name)
+    with open(output_file, "w", encoding="utf-8") as enc:
+        enc.write(ascii_art)
+
+    # print to output file
+    print(f"ASCII art written to {os.path.abspath(output_file)}")
+
+
+def print_cmd(args):
+    """
+    Prints all of the variables and the character set. (Used for development.)
+    """
+
+    char_set = get_char_set(args.set)
+    invert = bool(args.invert)
+
+    # print chosen options
+    print(f"Set {args.set} chosen.")
+    print(
+        " ".join([f"{i+1}. {char_set[i]}, " for i in range(len(char_set))])[:-2])
+    print(f"{'Randomization is on.' if args.random else 'Randomization is off.'}")
+    print(f"{'Invert is on.' if invert else 'Invert is off.'}")
```

### Comparing `ASCIIcli-0.0.7/tests/tests.py` & `ASCIIcli-0.0.9/tests/tests.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""
-This file is the test area for the ASCIIcli module.
-This module provides a command line tool for converting images to ASCII art.
-"""
-
-import unittest
-import argparse
-from unittest.mock import MagicMock
-from src.functions import randomize, get_char_set, char_a, char_b, char_c, char_d, char_e
-
-
-class Testing(unittest.TestCase):
-    """
-    The group of tests for ASCIIcli.
-    """
-
-    def test_randomize(self):
-        """
-        Tests the randomize function to see if it randomizes the sets when the argument is True.
-        """
-
-        args = MagicMock(random=True, set="1")
-        randomize(args)
-        if args.set == "1":
-            self.assertNotEqual(args.set, char_a)
-        elif args.set == "2":
-            self.assertNotEqual(args.set, char_b)
-        elif args.set == "3":
-            self.assertNotEqual(args.set, char_c)
-        elif args.set == "4":
-            self.assertNotEqual(args.set, char_d)
-        elif args.set == "5":
-            self.assertNotEqual(args.set, char_e)
-
-    # see if character sets are operational
-    def test_valid_set_1(self):
-        """
-        Tests whether or not set one is valid.
-        """
-        args = argparse.Namespace(set="1")
-        char_set = get_char_set(args.set)
-        self.assertEqual(char_set, char_a)
-
-    def test_valid_set_2(self):
-        """
-        Tests whether or not set two is valid.
-        """
-        args = argparse.Namespace(set="2")
-        char_set = get_char_set(args.set)
-        self.assertEqual(char_set, char_b)
-
-    def test_valid_set_3(self):
-        """
-        Tests whether or not set five is valid.
-        """
-        args = argparse.Namespace(set="3")
-        char_set = get_char_set(args.set)
-        self.assertEqual(char_set, char_c)
-
-    def test_valid_set_4(self):
-        """
-        Tests whether or not set four is valid.
-        """
-        args = argparse.Namespace(set="4")
-        char_set = get_char_set(args.set)
-        self.assertEqual(char_set, char_d)
-
-    def test_valid_set_5(self):
-        """
-        Tests whether or not set five is valid.
-        """
-        args = argparse.Namespace(set="5")
-        char_set = get_char_set(args.set)
-        self.assertEqual(char_set, char_e)
-
-    def test_invalid_set(self):
-        """
-        Tests whether or not an invalid set will be shown as valid.
-        """
-        args = argparse.Namespace(set="10")
-        char_set = get_char_set(args.set)
-        char_invalid = 0
-        self.assertEqual(char_set, char_invalid)
-
-
-if __name__ == '__main__':
-    unittest.main()
+"""
+This file is the test area for the ASCIIcli module.
+This module provides a command line tool for converting images to ASCII art.
+"""
+
+import unittest
+import argparse
+from unittest.mock import MagicMock
+from src.functions import randomize, get_char_set, char_a, char_b, char_c, char_d, char_e
+
+
+class Testing(unittest.TestCase):
+    """
+    The group of tests for ASCIIcli.
+    """
+
+    def test_randomize(self):
+        """
+        Tests the randomize function to see if it randomizes the sets when the argument is True.
+        """
+
+        args = MagicMock(random=True, set="1")
+        randomize(args)
+        if args.set == "1":
+            self.assertNotEqual(args.set, char_a)
+        elif args.set == "2":
+            self.assertNotEqual(args.set, char_b)
+        elif args.set == "3":
+            self.assertNotEqual(args.set, char_c)
+        elif args.set == "4":
+            self.assertNotEqual(args.set, char_d)
+        elif args.set == "5":
+            self.assertNotEqual(args.set, char_e)
+
+    # see if character sets are operational
+    def test_valid_set_1(self):
+        """
+        Tests whether or not set one is valid.
+        """
+        args = argparse.Namespace(set="1")
+        char_set = get_char_set(args.set)
+        self.assertEqual(char_set, char_a)
+
+    def test_valid_set_2(self):
+        """
+        Tests whether or not set two is valid.
+        """
+        args = argparse.Namespace(set="2")
+        char_set = get_char_set(args.set)
+        self.assertEqual(char_set, char_b)
+
+    def test_valid_set_3(self):
+        """
+        Tests whether or not set five is valid.
+        """
+        args = argparse.Namespace(set="3")
+        char_set = get_char_set(args.set)
+        self.assertEqual(char_set, char_c)
+
+    def test_valid_set_4(self):
+        """
+        Tests whether or not set four is valid.
+        """
+        args = argparse.Namespace(set="4")
+        char_set = get_char_set(args.set)
+        self.assertEqual(char_set, char_d)
+
+    def test_valid_set_5(self):
+        """
+        Tests whether or not set five is valid.
+        """
+        args = argparse.Namespace(set="5")
+        char_set = get_char_set(args.set)
+        self.assertEqual(char_set, char_e)
+
+    def test_invalid_set(self):
+        """
+        Tests whether or not an invalid set will be shown as valid.
+        """
+        args = argparse.Namespace(set="10")
+        char_set = get_char_set(args.set)
+        char_invalid = 0
+        self.assertEqual(char_set, char_invalid)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

