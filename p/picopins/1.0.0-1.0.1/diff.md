# Comparing `tmp/picopins-1.0.0.tar.gz` & `tmp/picopins-1.0.1.tar.gz`

## Comparing `picopins-1.0.0.tar` & `picopins-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 picopins-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.0.0/Makefile
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 picopins-1.0.0/README.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.0.0/check.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.0.0/requirements-dev.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picopins-1.0.0/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.0.0/tox.ini
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 picopins-1.0.0/examples/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.0.0/picopins/__init__.py
--rwxr-xr-x   0        0        0     7315 2020-02-02 00:00:00.000000 picopins-1.0.0/picopins/__main__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.0.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.0.0/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 picopins-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 picopins-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 picopins-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 picopins-1.0.1/Makefile
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 picopins-1.0.1/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 picopins-1.0.1/check.sh
+-rw-r--r--   0        0        0    34361 2020-02-02 00:00:00.000000 picopins-1.0.1/example.png
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 picopins-1.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picopins-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 picopins-1.0.1/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picopins-1.0.1/picopins/__init__.py
+-rwxr-xr-x   0        0        0     7315 2020-02-02 00:00:00.000000 picopins-1.0.1/picopins/__main__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 picopins-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 picopins-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 picopins-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 picopins-1.0.1/PKG-INFO
```

### Comparing `picopins-1.0.0/Makefile` & `picopins-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `picopins-1.0.0/check.sh` & `picopins-1.0.1/check.sh`

 * *Files identical despite different names*

### Comparing `picopins-1.0.0/picopins/__main__.py` & `picopins-1.0.1/picopins/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Support me:
 https://ko-fi.com/gadgetoid
 https://github.com/sponsors/Gadgetoid
 https://www.patreon.com/gadgetoid
 """
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 pinout = [[col.strip() for col in line.split("|")] for line in """
       |         |        |        |      |  |     ┏━━━━━┓     |  |          |        |        |         |
       |         |        |        |      |  |┏━━━━┫     ┣━━━━┓|  |          |        |        |         |
 PWM0 A|UART0 TX |I2C0 SDA|SPI0 RX |GP0   |1 |┃◎   ┗━━━━━┛   ◎┃|40|VBUS      |        |        |         |
 PWM0 B|UART0 RX |I2C0 SCL|SPI0 CSn|GP1   |2 |┃◎ ▩           ◎┃|39|VSYS      |        |        |         |
       |         |        |        |Ground|3 |┃▣ └─GP25      ▣┃|38|Ground    |        |        |         |
```

### Comparing `picopins-1.0.0/LICENSE` & `picopins-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picopins-1.0.0/pyproject.toml` & `picopins-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `picopins-1.0.0/PKG-INFO` & `picopins-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopins
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line pinout for the Raspberry Pi Pico W
 Project-URL: GitHub, https://www.github.com/pinout-xyz/picopins
 Project-URL: Homepage, https://pico.pinout.xyz
 Author-email: Philip Howard <pinout@gadgetoid.com>
 Maintainer-email: Philip Howard <pinout@gadgetoid.com>
 License: MIT License
         
@@ -44,24 +44,43 @@
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # Raspberry Pi Pico GPIO Pinout
 
-[![Build Status](https://img.shields.io/github/actions/workflow/status/pinout-xyz/picopins/test.yml?branch=main)](https://github.com/pinout-xyz/picopins/actions/workflows/test.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pinout-xyz/picopins/badge.svg?branch=master)](https://coveralls.io/github/pinout-xyz/picopins?branch=master)
+A beautiful GPIO pinout and pin function guide for the Raspberry Pi Pico.
+
+![Example image](https://raw.githubusercontent.com/pinout-xyz/picopins/main/example.png)
+
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pinout-xyz/picopins/build.yml?branch=main)](https://github.com/pinout-xyz/picopins/actions/workflows/build.yml)
 [![PyPi Package](https://img.shields.io/pypi/v/picopins.svg)](https://pypi.python.org/pypi/picopins)
 [![Python Versions](https://img.shields.io/pypi/pyversions/picopins.svg)](https://pypi.python.org/pypi/picopins)
 
-Generated from [the Pimoroni Python Boilerplate](https://github.com/pimoroni/boilerplate-python).
+# Usage
+
+```
+usage: picopins [--pins] [--all] or {spi,i2c,uart,pwm}
+       --pins - show physical pin numbers
+       --all or {spi,i2c,uart,pwm} - pick list of interfaces to show
+       --hide-gpio - hide GPIO pins
+       --find "<text>" - highlight pins matching <text>
+
+eg:    picopins i2c  - show GPIO and I2C labels
+       picopins      - basic GPIO pinout
+```
 
 # Installing
 
 * Just run `python3 -m pip install picopins`
 # Changelog
 
+1.0.1
+-----
+
+* Tidy up readme
+
 1.0.0
 -----
 
 * Initial Release
 * Ported from https://gist.github.com/Gadgetoid/192af85a3eb05d4a6ac1db076c4ef118
```

