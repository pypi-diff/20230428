# Comparing `tmp/micropython-eduponics-1.0.8.tar.gz` & `tmp/micropython-eduponics-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micropython-eduponics-1.0.8.tar", last modified: Thu Jul 15 06:48:19 2021, max compression
+gzip compressed data, was "micropython-eduponics-2.0.1.tar", last modified: Fri Apr 28 09:46:32 2023, max compression
```

## Comparing `micropython-eduponics-1.0.8.tar` & `micropython-eduponics-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2021-07-15 06:48:19.230128 micropython-eduponics-1.0.8/
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2021-07-15 06:48:19.228643 micropython-eduponics-1.0.8/Eduponics/
--rw-rw-r--   0 roni       (501) staff       (20)       22 2021-07-15 05:57:04.000000 micropython-eduponics-1.0.8/Eduponics/__init__.py
--rw-r--r--   0 roni       (501) staff       (20)     8411 2021-07-15 05:25:10.000000 micropython-eduponics-1.0.8/Eduponics/ads1x15.py
--rw-r--r--   0 roni       (501) staff       (20)     2456 2021-02-23 08:46:25.000000 micropython-eduponics-1.0.8/Eduponics/at24c02.py
--rw-r--r--   0 roni       (501) staff       (20)     2790 2021-02-22 04:21:05.000000 micropython-eduponics-1.0.8/Eduponics/bh1750.py
--rw-r--r--   0 roni       (501) staff       (20)     8818 2021-02-22 04:17:42.000000 micropython-eduponics-1.0.8/Eduponics/bme280.py
--rw-r--r--   0 roni       (501) staff       (20)     3964 2021-02-22 04:20:38.000000 micropython-eduponics-1.0.8/Eduponics/ds1307.py
--rw-r--r--   0 roni       (501) staff       (20)    16517 2021-02-24 08:12:04.000000 micropython-eduponics-1.0.8/Eduponics/mcp23017.py
--rw-r--r--   0 roni       (501) staff       (20)     2450 2021-04-10 10:30:04.000000 micropython-eduponics-1.0.8/Eduponics/pcf8574.py
--rw-r--r--   0 roni       (501) staff       (20)     3893 2021-07-15 05:25:02.000000 micropython-eduponics-1.0.8/Eduponics/tds.py
--rw-r--r--   0 roni       (501) staff       (20)     6481 2021-04-04 08:52:46.000000 micropython-eduponics-1.0.8/Eduponics/umqttsimple.py
--rw-r--r--   0 roni       (501) staff       (20)     8607 2021-07-15 06:48:19.230429 micropython-eduponics-1.0.8/PKG-INFO
--rw-rw-r--   0 roni       (501) staff       (20)     6388 2021-07-15 06:08:05.000000 micropython-eduponics-1.0.8/README.md
-drwxr-xr-x   0 roni       (501) staff       (20)        0 2021-07-15 06:48:19.229802 micropython-eduponics-1.0.8/micropython_eduponics.egg-info/
--rw-r--r--   0 roni       (501) staff       (20)     8607 2021-07-15 06:48:19.000000 micropython-eduponics-1.0.8/micropython_eduponics.egg-info/PKG-INFO
--rw-r--r--   0 roni       (501) staff       (20)      417 2021-07-15 06:48:19.000000 micropython-eduponics-1.0.8/micropython_eduponics.egg-info/SOURCES.txt
--rw-r--r--   0 roni       (501) staff       (20)        1 2021-07-15 06:48:19.000000 micropython-eduponics-1.0.8/micropython_eduponics.egg-info/dependency_links.txt
--rw-r--r--   0 roni       (501) staff       (20)       10 2021-07-15 06:48:19.000000 micropython-eduponics-1.0.8/micropython_eduponics.egg-info/top_level.txt
--rw-rw-r--   0 roni       (501) staff       (20)       79 2021-07-15 06:48:19.230992 micropython-eduponics-1.0.8/setup.cfg
--rwxr-xr-x   0 roni       (501) staff       (20)     1647 2021-07-15 06:47:15.000000 micropython-eduponics-1.0.8/setup.py
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.446922 micropython-eduponics-2.0.1/
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.445736 micropython-eduponics-2.0.1/Eduponics/
+-rw-r--r--   0 roni       (501) staff       (20)       22 2023-04-28 09:43:21.000000 micropython-eduponics-2.0.1/Eduponics/__init__.py
+-rw-r--r--   0 roni       (501) staff       (20)     8620 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/ads1x15.py
+-rw-r--r--   0 roni       (501) staff       (20)     2456 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/at24c02.py
+-rw-r--r--   0 roni       (501) staff       (20)     2790 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/bh1750.py
+-rw-r--r--   0 roni       (501) staff       (20)     8818 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/bme280.py
+-rw-r--r--   0 roni       (501) staff       (20)     3964 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/ds1307.py
+-rw-r--r--   0 roni       (501) staff       (20)    16517 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/mcp23017.py
+-rw-r--r--   0 roni       (501) staff       (20)     4913 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/pca9535.py
+-rw-r--r--   0 roni       (501) staff       (20)    10475 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/pcf8563.py
+-rw-r--r--   0 roni       (501) staff       (20)     2450 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/pcf8574.py
+-rw-r--r--   0 roni       (501) staff       (20)     8532 2023-02-04 21:51:50.000000 micropython-eduponics-2.0.1/Eduponics/qmp6988.py
+-rw-r--r--   0 roni       (501) staff       (20)     6709 2023-04-28 09:39:47.000000 micropython-eduponics-2.0.1/Eduponics/sht30.py
+-rw-r--r--   0 roni       (501) staff       (20)     3893 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/tds.py
+-rw-r--r--   0 roni       (501) staff       (20)     6481 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/Eduponics/umqttsimple.py
+-rw-r--r--   0 roni       (501) staff       (20)     1326 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/LICENSE.md
+-rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 09:46:32.447032 micropython-eduponics-2.0.1/PKG-INFO
+-rw-r--r--   0 roni       (501) staff       (20)     6388 2022-08-15 15:36:05.000000 micropython-eduponics-2.0.1/README.md
+drwxr-xr-x   0 roni       (501) staff       (20)        0 2023-04-28 09:46:32.446725 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/
+-rw-r--r--   0 roni       (501) staff       (20)     7505 2023-04-28 09:46:31.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/PKG-INFO
+-rw-r--r--   0 roni       (501) staff       (20)      510 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/SOURCES.txt
+-rw-r--r--   0 roni       (501) staff       (20)        1 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/dependency_links.txt
+-rw-r--r--   0 roni       (501) staff       (20)       10 2023-04-28 09:46:32.000000 micropython-eduponics-2.0.1/micropython_eduponics.egg-info/top_level.txt
+-rw-r--r--   0 roni       (501) staff       (20)       79 2023-04-28 09:46:32.447464 micropython-eduponics-2.0.1/setup.cfg
+-rwxr-xr-x   0 roni       (501) staff       (20)     1647 2023-04-28 09:43:21.000000 micropython-eduponics-2.0.1/setup.py
```

### Comparing `micropython-eduponics-1.0.8/Eduponics/ads1x15.py` & `micropython-eduponics-2.0.1/Eduponics/ads1x15.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import utime as time
-from Eduponics import mcp23017
+from Eduponics import mcp23017,pca9535
 
 _REGISTER_CONVERT = const(0x00)
 _REGISTER_CONFIG = const(0x01)
 _REGISTER_LOWTHRESH = const(0x02)
 _REGISTER_HITHRESH = const(0x03)
 
 _OS_SINGLE = const(0x8000)  # Write: Set to start a single-conversion
@@ -110,29 +110,34 @@
     _DR_2400SPS,  # 2400/250 samples per second
     _DR_3300SPS,  # 3300/475 samples per second
     _DR_860SPS    # - /860 samples per Second
 )
 
 
 class ADS1115:
-    def __init__(self, i2c, address=0x48, gain=1, mcp_address=0x20):
+    def __init__(self, i2c, address=0x48, gain=1, mcp_address=0x20,chip=None):
         self.i2c = i2c
         self.address = address
         self.mcp_address = mcp_address
         self.gain = gain
         self.temp2 = bytearray(2)
-        # define MCP for activating MOSFET pins
-        self.mcp = mcp23017.MCP23017(i2c=self.i2c, address=mcp_address)
         # define all the pins for the mosfets
         self.mcp_pins_sheet = {
             0:8,
             1:9,
             2:10,
             3:11
         }
+        # define MCP for activating MOSFET pins
+        if(chip==None):
+            # default is MCP
+            self.mcp = mcp23017.MCP23017(i2c=self.i2c, address=mcp_address)
+        elif(chip == "PCA9535"):
+            # use PCA9535
+            self.mcp = pca9535.PCA9555(i2c=self.i2c, address=mcp_address)
 
     def _write_register(self, register, value):
         self.temp2[0] = value >> 8
         self.temp2[1] = value & 0xff
         self.i2c.writeto_mem(self.address, register, self.temp2)
 
     def _read_register(self, register):
@@ -200,7 +205,8 @@
         time.sleep(0.1)
         # read the data
         raw = self.read_raw(channel1=pin)
         voltage = self.raw_to_v(raw)
         # deactivate mosfet after use
         self.mcp.pin(self.mcp_pins_sheet[pin], mode=0, value=0)
         return {"raw":raw,"voltage":voltage}
+
```

### Comparing `micropython-eduponics-1.0.8/Eduponics/at24c02.py` & `micropython-eduponics-2.0.1/Eduponics/at24c02.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/bh1750.py` & `micropython-eduponics-2.0.1/Eduponics/bh1750.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/bme280.py` & `micropython-eduponics-2.0.1/Eduponics/bme280.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/ds1307.py` & `micropython-eduponics-2.0.1/Eduponics/ds1307.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/mcp23017.py` & `micropython-eduponics-2.0.1/Eduponics/mcp23017.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/pcf8574.py` & `micropython-eduponics-2.0.1/Eduponics/pcf8574.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/tds.py` & `micropython-eduponics-2.0.1/Eduponics/tds.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/Eduponics/umqttsimple.py` & `micropython-eduponics-2.0.1/Eduponics/umqttsimple.py`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/PKG-INFO` & `micropython-eduponics-2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,162 +1,162 @@
 Metadata-Version: 2.1
 Name: micropython-eduponics
-Version: 1.0.8
+Version: 2.0.1
 Summary: STEMinds Eduponics Mini MicroPython library
 Home-page: https://github.com/STEMinds/micropython-eduponics
+Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz
 Author: STEMinds
 Author-email: contact@steminds.com
 License: MIT
-Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/1.0.8.tar.gz
-Description: [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=bugs)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=ncloc)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=security_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        
-        # MicroPython-Eduponics
-        
-        The official MicroPython Eduponics library for Eduponics Mini ESP32 dev board.
-        
-        ## What can this library do
-        
-        This library allows you to control all the functionalities of the ESP32 Eduponics mini dev board from one place.
-        The classes that are currently supported are:
-        
-        - umqttsimple.py - implementation of simple MQTT protocol for MicroPython.
-        - ads1x15.py - ADS1x15 precide Analog-to-digital chip (available on extension board).
-        - mcp23017.py - MCP23017 16-bit IO Expander (available on extension board).
-        - at24c02.py - AT24C02 EEPROM module.
-        - bh1750.py - BH1750 photodiode (light sensor).
-        - bme280.py - 3 in 1: temperature, humidity and barometric sensor.
-        - ds1307.py - DS1307 RTC module.
-        - pcf8574.py - PCF8574 8-bit IO Expander (available on valve extension board).
-        - tds.py - To control TDS sensor through extension board.
-        
-        The ADS1x15 class is integrated with MCP23017 in order to control the on-board MOSFET's and allow super low power consumption.
-        When the program ask for data form the ADC the MOSFET will open allowing current to flow (which will activate the sensor) once probing is done, the MOSFET will be deactivated.
-        
-        This approach also allows to control multiple sensors such as: pH, EC, TDS etc .. without conflict! also extending the sensors lifespan.
-        
-        The MCP23017 class also contains code to control the valve which can be found on the Eduponics Mini extension board.
-        
-        ## How to install
-        
-        First, connect the ESP32 board to the WiFi by creating boot.py file and writing the following:
-        
-        ```python
-        import network
-        import esp
-        import time
-        esp.osdebug(None)
-        import gc
-        gc.collect()
-        
-        # set WiFi credentials
-        ssid = ''
-        password = ''
-        
-        # check if there is username and password for wifi
-        if(ssid != '' and password != ''):
-        
-            station = network.WLAN(network.STA_IF)
-        
-            station.active(True)
-            station.connect(ssid, password)
-        
-            timeout_interval = 10
-        
-            # try to connect with timeout interval
-            for i in range(0,timeout_interval):
-                if(station.isconnected() == False):
-                    time.sleep(1)
-                    pass
-                else:
-                    break;
-        
-            if(station.isconnected()):
-                print('Connected to WiFi successfully, IP: %s' % station.ifconfig()[0])
-            else:
-                print("Something went wrong, connection timeout, try again!")
-        else:
-            print("Please add WiFi credentials properly")
-        ```
-        
-        Make sure to change WiFi ESSID and Password. Once the ESP32 is connected to the Wifi, run the following commands:
-        
-        ```python
-        import upip
-        upip.install("micropython-eduponics")
-        ```
-        
-        This will install the latest version of micropython-eduponics package through upip.
-        
-        Examples are available in the examples/ directory.
-        
-        ## Using firmwares
-        
-        Alternatively, you can burn a ready made firmware which located under the repository firmwares directory
-        currently 2 firmware available:
-        
-        1. 4M-eduponics-micropython.bin - firmware includes micropython-eduponics library pre-installed (without the MQTT client).
-        2. 4M-eduponics-MQTT.bin - firmware includes the MQTT library and everything you need to get started with the Eduponics mobile app.
-        
-        To flash the firmware, run the following command using esptool.py
-        ```
-        esptool.py --baud 115200 --port <port_name> write_flash 0x0 <firmware_name>.bin
-        ```
-        Where <firmware_name> is the file name (the bin file you want to flash) and <port_name> is the port name to flash through.
-        
-        Current firmware version: MicroPython v1.13 on 2020-09-02; ESP32 module with ESP32
-        
-        ## Changing MQTT broker
-        
-        In order to change the MQTT broker, change the umqttsimple.py file inside the [/Eduponics/](/Eduponics/umqttsimple.py) directory
-        Make sure to properly mark whenever you use SSL or not.
-        
-        ## License
-        
-        MIT License
-        
-        Copyright (c) 2014 Adafruit Industries,
-                      2016 Radomir Dopieralski (@deshipu),
-                      2016 Paul Cunnane 2016,
-                      2016 Peter Dahlebrg,
-                      2017 Robert Hammelrath (@robert-hh),
-                      2019 Mike Causer (@mcauser),
-                      2021 STEMinds (@STEMinds),
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Keywords: STEMinds,MicroPython,uPython,Eduponics-Mini,Eduponics,ESP32,ADS1x15,MCP23017,TDS,pH,bh1750,BME280,DS1307,AT24C02
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=bugs)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=ncloc)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=security_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+
+# MicroPython-Eduponics
+
+The official MicroPython Eduponics library for Eduponics Mini ESP32 dev board.
+
+## What can this library do
+
+This library allows you to control all the functionalities of the ESP32 Eduponics mini dev board from one place.
+The classes that are currently supported are:
+
+- umqttsimple.py - implementation of simple MQTT protocol for MicroPython.
+- ads1x15.py - ADS1x15 precide Analog-to-digital chip (available on extension board).
+- mcp23017.py - MCP23017 16-bit IO Expander (available on extension board).
+- at24c02.py - AT24C02 EEPROM module.
+- bh1750.py - BH1750 photodiode (light sensor).
+- bme280.py - 3 in 1: temperature, humidity and barometric sensor.
+- ds1307.py - DS1307 RTC module.
+- pcf8574.py - PCF8574 8-bit IO Expander (available on valve extension board).
+- tds.py - To control TDS sensor through extension board.
+
+The ADS1x15 class is integrated with MCP23017 in order to control the on-board MOSFET's and allow super low power consumption.
+When the program ask for data form the ADC the MOSFET will open allowing current to flow (which will activate the sensor) once probing is done, the MOSFET will be deactivated.
+
+This approach also allows to control multiple sensors such as: pH, EC, TDS etc .. without conflict! also extending the sensors lifespan.
+
+The MCP23017 class also contains code to control the valve which can be found on the Eduponics Mini extension board.
+
+## How to install
+
+First, connect the ESP32 board to the WiFi by creating boot.py file and writing the following:
+
+```python
+import network
+import esp
+import time
+esp.osdebug(None)
+import gc
+gc.collect()
+
+# set WiFi credentials
+ssid = ''
+password = ''
+
+# check if there is username and password for wifi
+if(ssid != '' and password != ''):
+
+    station = network.WLAN(network.STA_IF)
+
+    station.active(True)
+    station.connect(ssid, password)
+
+    timeout_interval = 10
+
+    # try to connect with timeout interval
+    for i in range(0,timeout_interval):
+        if(station.isconnected() == False):
+            time.sleep(1)
+            pass
+        else:
+            break;
+
+    if(station.isconnected()):
+        print('Connected to WiFi successfully, IP: %s' % station.ifconfig()[0])
+    else:
+        print("Something went wrong, connection timeout, try again!")
+else:
+    print("Please add WiFi credentials properly")
+```
+
+Make sure to change WiFi ESSID and Password. Once the ESP32 is connected to the Wifi, run the following commands:
+
+```python
+import upip
+upip.install("micropython-eduponics")
+```
+
+This will install the latest version of micropython-eduponics package through upip.
+
+Examples are available in the examples/ directory.
+
+## Using firmwares
+
+Alternatively, you can burn a ready made firmware which located under the repository firmwares directory
+currently 2 firmware available:
+
+1. 4M-eduponics-micropython.bin - firmware includes micropython-eduponics library pre-installed (without the MQTT client).
+2. 4M-eduponics-MQTT.bin - firmware includes the MQTT library and everything you need to get started with the Eduponics mobile app.
+
+To flash the firmware, run the following command using esptool.py
+```
+esptool.py --baud 115200 --port <port_name> write_flash 0x0 <firmware_name>.bin
+```
+Where <firmware_name> is the file name (the bin file you want to flash) and <port_name> is the port name to flash through.
+
+Current firmware version: MicroPython v1.13 on 2020-09-02; ESP32 module with ESP32
+
+## Changing MQTT broker
+
+In order to change the MQTT broker, change the umqttsimple.py file inside the [/Eduponics/](/Eduponics/umqttsimple.py) directory
+Make sure to properly mark whenever you use SSL or not.
+
+## License
+
+MIT License
+
+Copyright (c) 2014 Adafruit Industries,
+              2016 Radomir Dopieralski (@deshipu),
+              2016 Paul Cunnane 2016,
+              2016 Peter Dahlebrg,
+              2017 Robert Hammelrath (@robert-hh),
+              2019 Mike Causer (@mcauser),
+              2021 STEMinds (@STEMinds),
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `micropython-eduponics-1.0.8/README.md` & `micropython-eduponics-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `micropython-eduponics-1.0.8/micropython_eduponics.egg-info/PKG-INFO` & `micropython-eduponics-2.0.1/micropython_eduponics.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,162 +1,162 @@
 Metadata-Version: 2.1
 Name: micropython-eduponics
-Version: 1.0.8
+Version: 2.0.1
 Summary: STEMinds Eduponics Mini MicroPython library
 Home-page: https://github.com/STEMinds/micropython-eduponics
+Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz
 Author: STEMinds
 Author-email: contact@steminds.com
 License: MIT
-Download-URL: https://github.com/STEMinds/micropython-eduponics/archive/1.0.8.tar.gz
-Description: [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=bugs)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=ncloc)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=security_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
-        
-        # MicroPython-Eduponics
-        
-        The official MicroPython Eduponics library for Eduponics Mini ESP32 dev board.
-        
-        ## What can this library do
-        
-        This library allows you to control all the functionalities of the ESP32 Eduponics mini dev board from one place.
-        The classes that are currently supported are:
-        
-        - umqttsimple.py - implementation of simple MQTT protocol for MicroPython.
-        - ads1x15.py - ADS1x15 precide Analog-to-digital chip (available on extension board).
-        - mcp23017.py - MCP23017 16-bit IO Expander (available on extension board).
-        - at24c02.py - AT24C02 EEPROM module.
-        - bh1750.py - BH1750 photodiode (light sensor).
-        - bme280.py - 3 in 1: temperature, humidity and barometric sensor.
-        - ds1307.py - DS1307 RTC module.
-        - pcf8574.py - PCF8574 8-bit IO Expander (available on valve extension board).
-        - tds.py - To control TDS sensor through extension board.
-        
-        The ADS1x15 class is integrated with MCP23017 in order to control the on-board MOSFET's and allow super low power consumption.
-        When the program ask for data form the ADC the MOSFET will open allowing current to flow (which will activate the sensor) once probing is done, the MOSFET will be deactivated.
-        
-        This approach also allows to control multiple sensors such as: pH, EC, TDS etc .. without conflict! also extending the sensors lifespan.
-        
-        The MCP23017 class also contains code to control the valve which can be found on the Eduponics Mini extension board.
-        
-        ## How to install
-        
-        First, connect the ESP32 board to the WiFi by creating boot.py file and writing the following:
-        
-        ```python
-        import network
-        import esp
-        import time
-        esp.osdebug(None)
-        import gc
-        gc.collect()
-        
-        # set WiFi credentials
-        ssid = ''
-        password = ''
-        
-        # check if there is username and password for wifi
-        if(ssid != '' and password != ''):
-        
-            station = network.WLAN(network.STA_IF)
-        
-            station.active(True)
-            station.connect(ssid, password)
-        
-            timeout_interval = 10
-        
-            # try to connect with timeout interval
-            for i in range(0,timeout_interval):
-                if(station.isconnected() == False):
-                    time.sleep(1)
-                    pass
-                else:
-                    break;
-        
-            if(station.isconnected()):
-                print('Connected to WiFi successfully, IP: %s' % station.ifconfig()[0])
-            else:
-                print("Something went wrong, connection timeout, try again!")
-        else:
-            print("Please add WiFi credentials properly")
-        ```
-        
-        Make sure to change WiFi ESSID and Password. Once the ESP32 is connected to the Wifi, run the following commands:
-        
-        ```python
-        import upip
-        upip.install("micropython-eduponics")
-        ```
-        
-        This will install the latest version of micropython-eduponics package through upip.
-        
-        Examples are available in the examples/ directory.
-        
-        ## Using firmwares
-        
-        Alternatively, you can burn a ready made firmware which located under the repository firmwares directory
-        currently 2 firmware available:
-        
-        1. 4M-eduponics-micropython.bin - firmware includes micropython-eduponics library pre-installed (without the MQTT client).
-        2. 4M-eduponics-MQTT.bin - firmware includes the MQTT library and everything you need to get started with the Eduponics mobile app.
-        
-        To flash the firmware, run the following command using esptool.py
-        ```
-        esptool.py --baud 115200 --port <port_name> write_flash 0x0 <firmware_name>.bin
-        ```
-        Where <firmware_name> is the file name (the bin file you want to flash) and <port_name> is the port name to flash through.
-        
-        Current firmware version: MicroPython v1.13 on 2020-09-02; ESP32 module with ESP32
-        
-        ## Changing MQTT broker
-        
-        In order to change the MQTT broker, change the umqttsimple.py file inside the [/Eduponics/](/Eduponics/umqttsimple.py) directory
-        Make sure to properly mark whenever you use SSL or not.
-        
-        ## License
-        
-        MIT License
-        
-        Copyright (c) 2014 Adafruit Industries,
-                      2016 Radomir Dopieralski (@deshipu),
-                      2016 Paul Cunnane 2016,
-                      2016 Peter Dahlebrg,
-                      2017 Robert Hammelrath (@robert-hh),
-                      2019 Mike Causer (@mcauser),
-                      2021 STEMinds (@STEMinds),
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Keywords: STEMinds,MicroPython,uPython,Eduponics-Mini,Eduponics,ESP32,ADS1x15,MCP23017,TDS,pH,bh1750,BME280,DS1307,AT24C02
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=bugs)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=duplicated_lines_density)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=ncloc)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=security_rating)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=STEMinds_micropython-eduponics&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=STEMinds_micropython-eduponics)
+
+# MicroPython-Eduponics
+
+The official MicroPython Eduponics library for Eduponics Mini ESP32 dev board.
+
+## What can this library do
+
+This library allows you to control all the functionalities of the ESP32 Eduponics mini dev board from one place.
+The classes that are currently supported are:
+
+- umqttsimple.py - implementation of simple MQTT protocol for MicroPython.
+- ads1x15.py - ADS1x15 precide Analog-to-digital chip (available on extension board).
+- mcp23017.py - MCP23017 16-bit IO Expander (available on extension board).
+- at24c02.py - AT24C02 EEPROM module.
+- bh1750.py - BH1750 photodiode (light sensor).
+- bme280.py - 3 in 1: temperature, humidity and barometric sensor.
+- ds1307.py - DS1307 RTC module.
+- pcf8574.py - PCF8574 8-bit IO Expander (available on valve extension board).
+- tds.py - To control TDS sensor through extension board.
+
+The ADS1x15 class is integrated with MCP23017 in order to control the on-board MOSFET's and allow super low power consumption.
+When the program ask for data form the ADC the MOSFET will open allowing current to flow (which will activate the sensor) once probing is done, the MOSFET will be deactivated.
+
+This approach also allows to control multiple sensors such as: pH, EC, TDS etc .. without conflict! also extending the sensors lifespan.
+
+The MCP23017 class also contains code to control the valve which can be found on the Eduponics Mini extension board.
+
+## How to install
+
+First, connect the ESP32 board to the WiFi by creating boot.py file and writing the following:
+
+```python
+import network
+import esp
+import time
+esp.osdebug(None)
+import gc
+gc.collect()
+
+# set WiFi credentials
+ssid = ''
+password = ''
+
+# check if there is username and password for wifi
+if(ssid != '' and password != ''):
+
+    station = network.WLAN(network.STA_IF)
+
+    station.active(True)
+    station.connect(ssid, password)
+
+    timeout_interval = 10
+
+    # try to connect with timeout interval
+    for i in range(0,timeout_interval):
+        if(station.isconnected() == False):
+            time.sleep(1)
+            pass
+        else:
+            break;
+
+    if(station.isconnected()):
+        print('Connected to WiFi successfully, IP: %s' % station.ifconfig()[0])
+    else:
+        print("Something went wrong, connection timeout, try again!")
+else:
+    print("Please add WiFi credentials properly")
+```
+
+Make sure to change WiFi ESSID and Password. Once the ESP32 is connected to the Wifi, run the following commands:
+
+```python
+import upip
+upip.install("micropython-eduponics")
+```
+
+This will install the latest version of micropython-eduponics package through upip.
+
+Examples are available in the examples/ directory.
+
+## Using firmwares
+
+Alternatively, you can burn a ready made firmware which located under the repository firmwares directory
+currently 2 firmware available:
+
+1. 4M-eduponics-micropython.bin - firmware includes micropython-eduponics library pre-installed (without the MQTT client).
+2. 4M-eduponics-MQTT.bin - firmware includes the MQTT library and everything you need to get started with the Eduponics mobile app.
+
+To flash the firmware, run the following command using esptool.py
+```
+esptool.py --baud 115200 --port <port_name> write_flash 0x0 <firmware_name>.bin
+```
+Where <firmware_name> is the file name (the bin file you want to flash) and <port_name> is the port name to flash through.
+
+Current firmware version: MicroPython v1.13 on 2020-09-02; ESP32 module with ESP32
+
+## Changing MQTT broker
+
+In order to change the MQTT broker, change the umqttsimple.py file inside the [/Eduponics/](/Eduponics/umqttsimple.py) directory
+Make sure to properly mark whenever you use SSL or not.
+
+## License
+
+MIT License
+
+Copyright (c) 2014 Adafruit Industries,
+              2016 Radomir Dopieralski (@deshipu),
+              2016 Paul Cunnane 2016,
+              2016 Peter Dahlebrg,
+              2017 Robert Hammelrath (@robert-hh),
+              2019 Mike Causer (@mcauser),
+              2021 STEMinds (@STEMinds),
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `micropython-eduponics-1.0.8/setup.py` & `micropython-eduponics-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = f.read()
 
 setup(
     name='micropython-eduponics',
     packages=find_packages(),
     include_package_data=True,
     version=__version__,
-    download_url = 'https://github.com/STEMinds/micropython-eduponics/archive/1.0.8.tar.gz',
+    download_url = 'https://github.com/STEMinds/micropython-eduponics/archive/2.0.1.tar.gz',
     keywords = ["STEMinds",'MicroPython','uPython', 'Eduponics-Mini', 'Eduponics', 'ESP32', 'ADS1x15', 'MCP23017', 'TDS', 'pH', 'bh1750', 'BME280', 'DS1307', 'AT24C02'],
     description='STEMinds Eduponics Mini MicroPython library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     classifiers=[
         'Development Status :: 4 - Beta',
```

