# Comparing `tmp/bmi270-0.4.1.tar.gz` & `tmp/bmi270-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmi270-0.4.1.tar", last modified: Thu Apr 20 09:21:00 2023, max compression
+gzip compressed data, was "bmi270-0.4.2.tar", last modified: Fri Apr 28 08:44:37 2023, max compression
```

## Comparing `bmi270-0.4.1.tar` & `bmi270-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/
--rw-rw-r--   0 somml     (1000) somml     (1000)     1073 2023-03-24 10:40:45.000000 bmi270-0.4.1/LICENSE
--rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-20 09:21:00.375079 bmi270-0.4.1/PKG-INFO
--rw-rw-r--   0 somml     (1000) somml     (1000)     2054 2023-04-20 07:49:16.000000 bmi270-0.4.1/README.md
--rw-rw-r--   0 somml     (1000) somml     (1000)      887 2023-04-20 07:49:30.000000 bmi270-0.4.1/pyproject.toml
--rw-rw-r--   0 somml     (1000) somml     (1000)       38 2023-04-20 09:21:00.375079 bmi270-0.4.1/setup.cfg
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/bmi270/
--rw-rw-r--   0 somml     (1000) somml     (1000)    19603 2023-04-20 09:09:13.000000 bmi270-0.4.1/src/bmi270/BMI270.py
--rw-rw-r--   0 somml     (1000) somml     (1000)    51029 2023-04-05 14:15:45.000000 bmi270-0.4.1/src/bmi270/config_file.py
--rw-rw-r--   0 somml     (1000) somml     (1000)     2306 2023-04-05 14:15:45.000000 bmi270-0.4.1/src/bmi270/definitions.py
--rw-rw-r--   0 somml     (1000) somml     (1000)     1003 2023-04-20 07:52:26.000000 bmi270-0.4.1/src/bmi270/registers.py
-drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-20 09:21:00.375079 bmi270-0.4.1/src/bmi270.egg-info/
--rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/PKG-INFO
--rw-rw-r--   0 somml     (1000) somml     (1000)      298 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/SOURCES.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)        1 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/dependency_links.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)       14 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/requires.txt
--rw-rw-r--   0 somml     (1000) somml     (1000)        7 2023-04-20 09:21:00.000000 bmi270-0.4.1/src/bmi270.egg-info/top_level.txt
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-28 08:44:37.718490 bmi270-0.4.2/
+-rw-rw-r--   0 somml     (1000) somml     (1000)     1073 2023-03-24 10:40:45.000000 bmi270-0.4.2/LICENSE
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-28 08:44:37.718490 bmi270-0.4.2/PKG-INFO
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2055 2023-04-20 09:32:41.000000 bmi270-0.4.2/README.md
+-rw-rw-r--   0 somml     (1000) somml     (1000)      887 2023-04-28 08:40:49.000000 bmi270-0.4.2/pyproject.toml
+-rw-rw-r--   0 somml     (1000) somml     (1000)       38 2023-04-28 08:44:37.718490 bmi270-0.4.2/setup.cfg
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-28 08:44:37.714490 bmi270-0.4.2/src/
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-28 08:44:37.714490 bmi270-0.4.2/src/bmi270/
+-rw-rw-r--   0 somml     (1000) somml     (1000)    19603 2023-04-28 08:38:38.000000 bmi270-0.4.2/src/bmi270/BMI270.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)    51029 2023-04-05 14:15:45.000000 bmi270-0.4.2/src/bmi270/config_file.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2306 2023-04-05 14:15:45.000000 bmi270-0.4.2/src/bmi270/definitions.py
+-rw-rw-r--   0 somml     (1000) somml     (1000)     1003 2023-04-20 07:52:26.000000 bmi270-0.4.2/src/bmi270/registers.py
+drwxrwxr-x   0 somml     (1000) somml     (1000)        0 2023-04-28 08:44:37.718490 bmi270-0.4.2/src/bmi270.egg-info/
+-rw-rw-r--   0 somml     (1000) somml     (1000)     2788 2023-04-28 08:44:37.000000 bmi270-0.4.2/src/bmi270.egg-info/PKG-INFO
+-rw-rw-r--   0 somml     (1000) somml     (1000)      298 2023-04-28 08:44:37.000000 bmi270-0.4.2/src/bmi270.egg-info/SOURCES.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)        1 2023-04-28 08:44:37.000000 bmi270-0.4.2/src/bmi270.egg-info/dependency_links.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)       14 2023-04-28 08:44:37.000000 bmi270-0.4.2/src/bmi270.egg-info/requires.txt
+-rw-rw-r--   0 somml     (1000) somml     (1000)        7 2023-04-28 08:44:37.000000 bmi270-0.4.2/src/bmi270.egg-info/top_level.txt
```

### Comparing `bmi270-0.4.1/LICENSE` & `bmi270-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.1/PKG-INFO` & `bmi270-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi270
-Version: 0.4.1
+Version: 0.4.2
 Summary: BMI270 I2C Python library (bare bones)
 Author-email: Kevin Sommler <sommler@live.de>
 License: MIT
 Project-URL: Homepage, https://github.com/CoRoLab-Berlin/bmi270_python
 Project-URL: Bug Tracker, https://github.com/CoRoLab-Berlin/bmi270_python/issues
 Keywords: BMI270,I2C,IMU,sensor,driver,accelerometer,gyroscope,gyro,bosch,sensortech,smbus2,library
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# BMI270 I2C Python Implementation - Version: 0.4.0
+# BMI270 I2C Python Implementation - Version: 0.4.1
 
 Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
```

### Comparing `bmi270-0.4.1/README.md` & `bmi270-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BMI270 I2C Python Implementation - Version: 0.4.0
+# BMI270 I2C Python Implementation - Version: 0.4.1
 
 Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
@@ -59,8 +59,8 @@
 - [BMI270 Datasheet](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bmi270-ds000.pdf)
 - [smbus2 docs](https://smbus2.readthedocs.io/en/latest/)
 
 ## Troubleshooting
 
 -bash: pip3: command not found
 
-`sudo apt install python3-pip`
+`sudo apt install python3-pip`
```

### Comparing `bmi270-0.4.1/pyproject.toml` & `bmi270-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bmi270"
-version = "0.4.1"
+version = "0.4.2"
 authors = [{name = "Kevin Sommler", email = "sommler@live.de"}]
 description = "BMI270 I2C Python library (bare bones)"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["BMI270", "I2C", "IMU", "sensor", "driver", "accelerometer", "gyroscope", "gyro", "bosch", "sensortech", "smbus2", "library"]
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `bmi270-0.4.1/src/bmi270/BMI270.py` & `bmi270-0.4.2/src/bmi270/BMI270.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.1/src/bmi270/config_file.py` & `bmi270-0.4.2/src/bmi270/config_file.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.1/src/bmi270/definitions.py` & `bmi270-0.4.2/src/bmi270/definitions.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.1/src/bmi270/registers.py` & `bmi270-0.4.2/src/bmi270/registers.py`

 * *Files identical despite different names*

### Comparing `bmi270-0.4.1/src/bmi270.egg-info/PKG-INFO` & `bmi270-0.4.2/src/bmi270.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmi270
-Version: 0.4.1
+Version: 0.4.2
 Summary: BMI270 I2C Python library (bare bones)
 Author-email: Kevin Sommler <sommler@live.de>
 License: MIT
 Project-URL: Homepage, https://github.com/CoRoLab-Berlin/bmi270_python
 Project-URL: Bug Tracker, https://github.com/CoRoLab-Berlin/bmi270_python/issues
 Keywords: BMI270,I2C,IMU,sensor,driver,accelerometer,gyroscope,gyro,bosch,sensortech,smbus2,library
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# BMI270 I2C Python Implementation - Version: 0.4.0
+# BMI270 I2C Python Implementation - Version: 0.4.1
 
 Bare bones BMI270 I2C Python implementation. This was a project for my practical phase at my University and my first time working hands on with IMUs.
 
 ## Installation
 The package is [available on pypi.org](https://pypi.org/project/bmi270).
 
 You can install this package using this command:
```

