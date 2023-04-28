# Comparing `tmp/pymx2-0.1.1.tar.gz` & `tmp/pymx2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymx2-0.1.1.tar", last modified: Thu Apr 27 14:38:34 2023, max compression
+gzip compressed data, was "pymx2-0.1.2.tar", last modified: Fri Apr 28 12:13:27 2023, max compression
```

## Comparing `pymx2-0.1.1.tar` & `pymx2-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.860597 pymx2-0.1.1/
--rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.1/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.1/LICENSE
--rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-27 14:38:34.860163 pymx2-0.1.1/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2749 2023-04-27 12:33:54.000000 pymx2-0.1.1/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.850240 pymx2-0.1.1/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)   127613 2023-04-27 12:18:08.000000 pymx2-0.1.1/docs/mx2.enums.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-04-27 12:18:16.000000 pymx2-0.1.1/docs/mx2.exceptions.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    21831 2023-04-27 12:17:38.000000 pymx2-0.1.1/docs/mx2.html
--rw-r--r--   0 vpaeder    (501) staff       (20)     9646 2023-04-27 12:18:12.000000 pymx2-0.1.1/docs/mx2.types.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.853314 pymx2-0.1.1/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.1/examples/01_connect.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.1/examples/02_read_write_coil.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.1/examples/03_read_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.1/examples/04_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.1/examples/05_read_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.1/examples/06_data_types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.855119 pymx2-0.1.1/mx2/
--rw-r--r--   0 vpaeder    (501) staff       (20)    31385 2023-04-27 14:23:48.000000 pymx2-0.1.1/mx2/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    48402 2023-04-26 14:06:02.000000 pymx2-0.1.1/mx2/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.1/mx2/exceptions.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    11343 2023-04-27 12:20:33.000000 pymx2-0.1.1/mx2/types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.857271 pymx2-0.1.1/pymx2.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-27 14:38:34.000000 pymx2-0.1.1/pymx2.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-04-27 14:38:34.000000 pymx2-0.1.1/pymx2.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-04-27 14:38:34.000000 pymx2-0.1.1/pymx2.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-04-27 14:38:34.000000 pymx2-0.1.1/pymx2.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-04-27 14:38:34.000000 pymx2-0.1.1/pymx2.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-04-27 14:38:34.860731 pymx2-0.1.1/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-04-27 14:37:54.000000 pymx2-0.1.1/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-27 14:38:34.859575 pymx2-0.1.1/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.1/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    14195 2023-04-27 14:35:49.000000 pymx2-0.1.1/tests/inverter.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     4509 2023-04-25 14:12:46.000000 pymx2-0.1.1/tests/modbus.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.1/tests/ser.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.1/tests/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.231017 pymx2-0.1.2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.2/.gitignore
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.2/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-28 12:13:27.230457 pymx2-0.1.2/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2749 2023-04-27 12:33:54.000000 pymx2-0.1.2/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.215235 pymx2-0.1.2/docs/
+-rw-r--r--   0 vpaeder    (501) staff       (20)   127613 2023-04-27 12:18:08.000000 pymx2-0.1.2/docs/mx2.enums.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-04-27 12:18:16.000000 pymx2-0.1.2/docs/mx2.exceptions.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    21831 2023-04-27 12:17:38.000000 pymx2-0.1.2/docs/mx2.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)     9646 2023-04-27 12:18:12.000000 pymx2-0.1.2/docs/mx2.types.html
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.220393 pymx2-0.1.2/examples/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.2/examples/01_connect.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.2/examples/02_read_write_coil.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.2/examples/03_read_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.2/examples/04_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.2/examples/05_read_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.2/examples/06_data_types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.223231 pymx2-0.1.2/mx2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    31385 2023-04-27 14:23:48.000000 pymx2-0.1.2/mx2/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.2/mx2/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.2/mx2/exceptions.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    11343 2023-04-27 12:20:33.000000 pymx2-0.1.2/mx2/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.226009 pymx2-0.1.2/pymx2.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3501 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-04-28 12:13:27.000000 pymx2-0.1.2/pymx2.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-04-28 12:13:27.231159 pymx2-0.1.2/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-04-28 12:11:32.000000 pymx2-0.1.2/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-04-28 12:13:27.229437 pymx2-0.1.2/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.2/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    14195 2023-04-27 14:35:49.000000 pymx2-0.1.2/tests/inverter.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     4509 2023-04-25 14:12:46.000000 pymx2-0.1.2/tests/modbus.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.2/tests/ser.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.2/tests/types.py
```

### Comparing `pymx2-0.1.1/LICENSE` & `pymx2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/PKG-INFO` & `pymx2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.1/README.md` & `pymx2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/docs/mx2.enums.html` & `pymx2-0.1.2/docs/mx2.enums.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/docs/mx2.exceptions.html` & `pymx2-0.1.2/docs/mx2.exceptions.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/docs/mx2.html` & `pymx2-0.1.2/docs/mx2.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/docs/mx2.types.html` & `pymx2-0.1.2/docs/mx2.types.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/examples/02_read_write_coil.py` & `pymx2-0.1.2/examples/02_read_write_coil.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/examples/03_read_registers.py` & `pymx2-0.1.2/examples/03_read_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/examples/04_write_registers.py` & `pymx2-0.1.2/examples/04_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/examples/05_read_write_registers.py` & `pymx2-0.1.2/examples/05_read_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/examples/06_data_types.py` & `pymx2-0.1.2/examples/06_data_types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/mx2/__init__.py` & `pymx2-0.1.2/mx2/__init__.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/mx2/enums.py` & `pymx2-0.1.2/mx2/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import enum
 
 __all__ = ["FunctionCode", "ExceptionCode", "Coil", "Register", "ModbusRegisters",
            "StandardFunctions", "FineTuningFunctions", "IntelligentTerminalFunctions",
            "MonitoringFunctions", "MainProfileParameters", "MotorConstantsFunctions",
            "OtherParameters", "SecondMotorFunctions", "FaultMonitorData", "TripFactor",
-           "InverterStatus"]
+           "InverterStatus", "GroupA", "GroupB", "GroupC", "GroupD", "GroupF",
+           "GroupH", "GroupP"]
 
 class FunctionCode(enum.IntEnum):
     """Function codes (2nd byte of Modbus message).
     See datasheet section B-3, p. 299."""
     ReadCoilStatus = 0x01
     ReadHoldingRegister = 0x03
     WriteInCoil = 0x05
@@ -459,14 +460,16 @@
     VRInputActiveRangeStartCurrent = 0x12CA
     A163 = 0x12CA
     VRInputActiveRangeEndVoltage = 0x12CB
     A164 = 0x12CB
     VRInputStartFrequencyEnable = 0x12CC
     A165 = 0x12CC
 
+GroupA = StandardFunctions
+
 
 class FineTuningFunctions(Register):
     """Fine tuning function group. See datasheet
     sections 3-6 (pp. 121-153) and B-4 (pp. 328-331)."""
     def contains(value:int):
         return Register.contains(FineTuningFunctions, value)
     # B group
@@ -699,14 +702,16 @@
     ThermalDecrementTime = (0x13C7, 2)
     B911 = (0x13C7, 2)
     ThermalDecrementTimeConstant = (0x13C9, 2)
     B912 = (0x13C9, 2)
     ThermalAccumulatorGain = 0x13CB
     B913 = 0x13CB
 
+GroupB = FineTuningFunctions
+
 
 class IntelligentTerminalFunctions(Register):
     """Intelligent terminal function group. See datasheet
     sections 3-7 (pp. 153-171) and B-4 (pp. 332-336)."""
     def contains(value:int):
         return Register.contains(IntelligentTerminalFunctions, value)
     # C group
@@ -887,14 +892,16 @@
     InputTerminalResponseTime6 = 0x14A9
     C165 = 0x14A9
     InputTerminalResponseTime7 = 0x14AA
     C166 = 0x14AA
     MultiStepSpeedPositionDeterminationTime = 0x14AD
     C169 = 0x14AD
 
+GroupC = IntelligentTerminalFunctions
+
 
 class MonitoringFunctions(Register):
     """Intelligent terminal function group. See datasheet
     sections 3-3 (pp. 74-88) and B-4 (pp. 319-320 and 322-323)."""
     def contains(value:int):
         return Register.contains(MonitoringFunctions, value)
     # D group
@@ -1025,14 +1032,16 @@
     PulseTrainInput = 0x10A4
     D133 = 0x10A4
     PIDDeviation = 0x10A6
     D153 = 0x10A6
     PIDOutput = 0x10A8
     D155 = 0x10A8
 
+GroupD = MonitoringFunctions
+
 
 class MainProfileParameters(Register):
     """Main profile parameters group. See datasheet
     sections 3-4 (p. 89) and B-4 (pp. 319-320, 322-323 and 344)."""
     def contains(value:int):
         return Register.contains(MainProfileParameters, value)
     # F group
@@ -1045,14 +1054,16 @@
     OperatorRotationDirection = 0x1107
     F004 = 0x1107
     SecondAccelerationTime1 = (0x2103, 2)
     F202 = (0x2103, 2)
     SecondDecelerationTime1 = (0x2105, 2)
     F203 = (0x2105, 2)
 
+GroupF = MainProfileParameters
+
 
 class MotorConstantsFunctions(Register):
     """Motor constants function group. See datasheet
     sections 3-8 (pp. 172-178) and B-4 (pp. 337-338)."""
     def contains(value:int):
         return Register.contains(MotorConstantsFunctions, value)
     # H group
@@ -1133,14 +1144,16 @@
     PMIMPEDetectWait = 0x158B
     H132 = 0x158B
     PMIMPEDetect = 0x158C
     H133 = 0x158C
     PMIMPEVoltageGain = 0x158D
     H134 = 0x158D
 
+GroupH = MotorConstantsFunctions
+
 
 class OtherParameters(Register):
     """Other parameters group. See datasheet
     sections 3-9 (pp. 179-190) and B-4 (pp. 339-343)."""
     def contains(value:int):
         return Register.contains(OtherParameters, value)
     # P group
@@ -1471,14 +1484,16 @@
     ModbusInternalRegister9 = 0x16EF
     P309 = 0x16EF
     ModbusInternalRegister10 = 0x16F0
     P310 = 0x16F0
     Endianness = 0x16F1
     P400 = 0x16F1
 
+GroupP = OtherParameters
+
 
 class SecondMotorFunctions(Register):
     """Second motor function group. See datasheet
     sections 3-x and B-4 (pp. 344-346)."""
     def contains(value:int):
         return Register.contains(SecondMotorFunctions, value)
     # A group
```

### Comparing `pymx2-0.1.1/mx2/exceptions.py` & `pymx2-0.1.2/mx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/mx2/types.py` & `pymx2-0.1.2/mx2/types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/pymx2.egg-info/PKG-INFO` & `pymx2-0.1.2/pymx2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.1/pymx2.egg-info/SOURCES.txt` & `pymx2-0.1.2/pymx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/setup.py` & `pymx2-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymx2",
-    version="0.1.1",
+    version="0.1.2",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="A Python driver to communicate with an Omron MX2 inverter through Modbus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['omron', 'mx2', 'inverter'],
     url="https://github.com/vpaeder/pymx2",
```

### Comparing `pymx2-0.1.1/tests/inverter.py` & `pymx2-0.1.2/tests/inverter.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/tests/modbus.py` & `pymx2-0.1.2/tests/modbus.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/tests/ser.py` & `pymx2-0.1.2/tests/ser.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.1/tests/types.py` & `pymx2-0.1.2/tests/types.py`

 * *Files identical despite different names*

