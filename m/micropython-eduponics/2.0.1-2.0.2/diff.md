# Comparing `tmp/micropython-eduponics-2.0.1.tar.gz` & `tmp/micropython-eduponics-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-eduponics-2.0.1.tar", last modified: Fri Apr 28 09:46:32 2023, max compression
+gzip compressed data, was "micropython-eduponics-2.0.2.tar", last modified: Fri Apr 28 10:31:29 2023, max compression
```

## Comparing `micropython-eduponics-2.0.1.tar` & `micropython-eduponics-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.446922 micropython-eduponics-2.0.1/
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.445736 micropython-eduponics-2.0.1/Eduponics/
--rw-r--r--   0 roni       (501) staff       (20)       22 2023-04-28 09:43:21.000000 micropython-eduponics-2.0.1/Eduponics/__init__.py
--rw-r--r--   0 roni       (501) staff       (20)     8620 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/ads1x15.py
--rw-r--r--   0 roni       (501) staff       (20)     2456 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/at24c02.py
--rw-r--r--   0 roni       (501) staff       (20)     2790 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/bh1750.py
--rw-r--r--   0 roni       (501) staff       (20)     8818 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/bme280.py
--rw-r--r--   0 roni       (501) staff       (20)     3964 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/ds1307.py
--rw-r--r--   0 roni       (501) staff       (20)    16517 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/mcp23017.py
--rw-r--r--   0 roni       (501) staff       (20)     4913 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/pca9535.py
--rw-r--r--   0 roni       (501) staff       (20)    10475 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/pcf8563.py
--rw-r--r--   0 roni       (501) staff       (20)     2450 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/pcf8574.py
--rw-r--r--   0 roni       (501) staff       (20)     8532 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/qmp6988.py
--rw-r--r--   0 roni       (501) staff       (20)     6709 2023-04-28 09:39:47.000000 micropython-eduponics-2.0.1/Eduponics/sht30.py
--rw-r--r--   0 roni       (501) staff       (20)     3893 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/tds.py
--rw-r--r--   0 roni       (501) staff       (20)     6481 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/umqttsimple.py
--rw-r--r--   0 roni       (501) staff       (20)     1326 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/LICENSE.md
--rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 09:46:32.447032 micropython-eduponics-2.0.1/PKG-INFO
--rw-r--r--   0 roni       (501) staff       (20)     6388 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/README.md
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.446725 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/
--rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 09:46:31.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/PKG-INFO
--rw-r--r--   0 roni       (501) staff       (20)      510 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/SOURCES.txt
--rw-r--r--   0 roni       (501) staff       (20)        1 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/dependency_links.txt
--rw-r--r--   0 roni       (501) staff       (20)       10 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/top_level.txt
--rw-r--r--   0 roni       (501) staff       (20)       79 2023-04-28 09:46:32.447464 micropython-eduponics-2.0.1/setup.cfg
--rwxr-xr-x   0 roni       (501) staff       (20)     1647 2023-04-28 09:43:21.000000 micropython-eduponics-2.0.1/setup.py
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 10:31:29.970870 micropython-eduponics-2.0.2/
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 10:31:29.969638 micropython-eduponics-2.0.2/Eduponics/
+-rw-r--r--   0 roni       (501) staff       (20)       22 2023-04-28 10:30:42.000000 micropython-eduponics-2.0.2/Eduponics/__init__.py
+-rw-r--r--   0 roni       (501) staff       (20)     8620 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.2/Eduponics/ads1x15.py
+-rw-r--r--   0 roni       (501) staff       (20)     2456 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/at24c02.py
+-rw-r--r--   0 roni       (501) staff       (20)     2790 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/bh1750.py
+-rw-r--r--   0 roni       (501) staff       (20)     8818 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/bme280.py
+-rw-r--r--   0 roni       (501) staff       (20)     3964 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/ds1307.py
+-rw-r--r--   0 roni       (501) staff       (20)    16517 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/mcp23017.py
+-rw-r--r--   0 roni       (501) staff       (20)     4913 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.2/Eduponics/pca9535.py
+-rw-r--r--   0 roni       (501) staff       (20)    10475 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.2/Eduponics/pcf8563.py
+-rw-r--r--   0 roni       (501) staff       (20)     2450 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/pcf8574.py
+-rw-r--r--   0 roni       (501) staff       (20)     8532 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.2/Eduponics/qmp6988.py
+-rw-r--r--   0 roni       (501) staff       (20)     6709 2023-04-28 10:27:58.000000 micropython-eduponics-2.0.2/Eduponics/sht30.py
+-rw-r--r--   0 roni       (501) staff       (20)     3893 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/tds.py
+-rw-r--r--   0 roni       (501) staff       (20)     6481 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/Eduponics/umqttsimple.py
+-rw-r--r--   0 roni       (501) staff       (20)     1326 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/LICENSE.md
+-rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 10:31:29.970988 micropython-eduponics-2.0.2/PKG-INFO
+-rw-r--r--   0 roni       (501) staff       (20)     6388 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.2/README.md
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 10:31:29.970649 micropython-eduponics-2.0.2/micropython_eduponics.egg-info/
+-rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 10:31:29.000000 micropython-eduponics-2.0.2/micropython_eduponics.egg-info/PKG-INFO
+-rw-r--r--   0 roni       (501) staff       (20)      510 2023-04-28 10:31:29.000000 micropython-eduponics-2.0.2/micropython_eduponics.egg-info/SOURCES.txt
+-rw-r--r--   0 roni       (501) staff       (20)        1 2023-04-28 10:31:29.000000 micropython-eduponics-2.0.2/micropython_eduponics.egg-info/dependency_links.txt
+-rw-r--r--   0 roni       (501) staff       (20)       10 2023-04-28 10:31:29.000000 micropython-eduponics-2.0.2/micropython_eduponics.egg-info/top_level.txt
+-rw-r--r--   0 roni       (501) staff       (20)       79 2023-04-28 10:31:29.971411 micropython-eduponics-2.0.2/setup.cfg
+-rwxr-xr-x   0 roni       (501) staff       (20)     1647 2023-04-28 10:30:42.000000 micropython-eduponics-2.0.2/setup.py
```

### Comparing `micropython-eduponics-2.0.1/Eduponics/ads1x15.py` & `micropython-eduponics-2.0.2/Eduponics/ads1x15.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/at24c02.py` & `micropython-eduponics-2.0.2/Eduponics/at24c02.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/bh1750.py` & `micropython-eduponics-2.0.2/Eduponics/bh1750.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/bme280.py` & `micropython-eduponics-2.0.2/Eduponics/bme280.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/ds1307.py` & `micropython-eduponics-2.0.2/Eduponics/ds1307.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/mcp23017.py` & `micropython-eduponics-2.0.2/Eduponics/mcp23017.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/pca9535.py` & `micropython-eduponics-2.0.2/Eduponics/pca9535.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/pcf8563.py` & `micropython-eduponics-2.0.2/Eduponics/pcf8563.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/pcf8574.py` & `micropython-eduponics-2.0.2/Eduponics/pcf8574.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/qmp6988.py` & `micropython-eduponics-2.0.2/Eduponics/qmp6988.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/sht30.py` & `micropython-eduponics-2.0.2/Eduponics/sht30.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from machine import I2C, Pin
 import time
 
 __version__ = '0.2.1'
 __author__ = 'Roberto Sánchez'
 __license__ = "Apache License 2.0. https://www.apache.org/licenses/LICENSE-2.0"
 
-# I2C address B 0x45 ADDR (pin 2) connected to VDD
-DEFAULT_I2C_ADDRESS = 0x45
+# I2C address B 0x44 ADDR (pin 2) connected to VDD
+DEFAULT_I2C_ADDRESS = 0x44
 
 class SHT30():
     """
     SHT30 sensor driver in pure python based on I2C bus
     
     References: 
     * https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/2_Humidity_Sensors/Sensirion_Humidity_Sensors_SHT3x_Datasheet_digital.pdf
```

### Comparing `micropython-eduponics-2.0.1/Eduponics/tds.py` & `micropython-eduponics-2.0.2/Eduponics/tds.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/Eduponics/umqttsimple.py` & `micropython-eduponics-2.0.2/Eduponics/umqttsimple.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/LICENSE.md` & `micropython-eduponics-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/PKG-INFO` & `micropython-eduponics-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: micropython-eduponics
-Version: 2.0.1
+Version: 2.0.2
 Summary: STEMinds Eduponics Mini MicroPython library
 Home-page: https://github.com/STEMinds/micropython-eduponics
-Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz
+Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.2.tar.gz
 Author: STEMinds
 Author-email: contact@steminds.com
 License: MIT
 Keywords: STEMinds,MicroPython,uPython,Eduponics-Mini,Eduponics,ESP32,ADS1x15,MCP23017,TDS,pH,bh1750,BME280,DS1307,AT24C02
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `micropython-eduponics-2.0.1/README.md` & `micropython-eduponics-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-2.0.1/micropython_eduponics.egg-info/PKG-INFO` & `micropython-eduponics-2.0.2/micropython_eduponics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: micropython-eduponics
-Version: 2.0.1
+Version: 2.0.2
 Summary: STEMinds Eduponics Mini MicroPython library
 Home-page: https://github.com/STEMinds/micropython-eduponics
-Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz
+Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.2.tar.gz
 Author: STEMinds
 Author-email: contact@steminds.com
 License: MIT
 Keywords: STEMinds,MicroPython,uPython,Eduponics-Mini,Eduponics,ESP32,ADS1x15,MCP23017,TDS,pH,bh1750,BME280,DS1307,AT24C02
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `micropython-eduponics-2.0.1/setup.py` & `micropython-eduponics-2.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = f.read()
 
 setup(
     name='micropython-eduponics',
     packages=find_packages(),
     include_package_data=True,
     version=__version__,
-    download_url = 'https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz',
+    download_url = 'https://github.com/STEMinds/micropython-eduponics/archive/2.0.2.tar.gz',
     keywords = ["STEMinds",'MicroPython','uPython', 'Eduponics-Mini', 'Eduponics', 'ESP32', 'ADS1x15', 'MCP23017', 'TDS', 'pH', 'bh1750', 'BME280', 'DS1307', 'AT24C02'],
     description='STEMinds Eduponics Mini MicroPython library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     classifiers=[
         'Development Status :: 4 - Beta',
```

