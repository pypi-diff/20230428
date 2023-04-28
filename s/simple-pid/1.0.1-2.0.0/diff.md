# Comparing `tmp/simple-pid-1.0.1.tar.gz` & `tmp/simple-pid-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-pid-1.0.1.tar", last modified: Sun Apr 11 10:02:21 2021, max compression
+gzip compressed data, was "simple-pid-2.0.0.tar", last modified: Fri Apr 28 21:10:57 2023, max compression
```

## Comparing `simple-pid-1.0.1.tar` & `simple-pid-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.797003 simple-pid-1.0.1/
--rw-r--r--   0 martin    (1000) martin    (1000)     2925 2021-04-11 09:59:23.000000 simple-pid-1.0.1/CHANGELOG.md
--rw-r--r--   0 martin    (1000) martin    (1000)     1077 2021-03-20 15:34:01.000000 simple-pid-1.0.1/LICENSE.md
--rw-r--r--   0 martin    (1000) martin    (1000)      310 2021-03-20 15:28:50.000000 simple-pid-1.0.1/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)     7008 2021-04-11 10:02:21.797003 simple-pid-1.0.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)     5419 2021-03-20 15:33:40.000000 simple-pid-1.0.1/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.750336 simple-pid-1.0.1/docs/
--rw-r--r--   0 martin    (1000) martin    (1000)      611 2018-05-11 09:02:43.000000 simple-pid-1.0.1/docs/Makefile
--rw-r--r--   0 martin    (1000) martin    (1000)       21 2018-05-11 11:39:42.000000 simple-pid-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.777003 simple-pid-1.0.1/docs/source/
--rw-r--r--   0 martin    (1000) martin    (1000)     5148 2018-05-11 10:05:45.000000 simple-pid-1.0.1/docs/source/conf.py
--rw-r--r--   0 martin    (1000) martin    (1000)      477 2018-05-11 10:11:08.000000 simple-pid-1.0.1/docs/source/index.rst
--rw-r--r--   0 martin    (1000) martin    (1000)      177 2018-05-11 09:50:47.000000 simple-pid-1.0.1/docs/source/simple_pid.rst
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.730336 simple-pid-1.0.1/examples/
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.790336 simple-pid-1.0.1/examples/water_boiler/
--rw-r--r--   0 martin    (1000) martin    (1000)     1407 2021-03-20 15:31:52.000000 simple-pid-1.0.1/examples/water_boiler/README.md
--rw-r--r--   0 martin    (1000) martin    (1000)      135 2021-04-11 09:59:59.000000 simple-pid-1.0.1/examples/water_boiler/requirements.txt
--rwxr-xr-x   0 martin    (1000) martin    (1000)     1451 2021-03-20 14:38:51.000000 simple-pid-1.0.1/examples/water_boiler/water_boiler.py
--rw-r--r--   0 martin    (1000) martin    (1000)      137 2021-04-11 10:02:21.797003 simple-pid-1.0.1/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     1174 2021-04-11 09:58:13.000000 simple-pid-1.0.1/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.790336 simple-pid-1.0.1/simple_pid/
--rw-r--r--   0 martin    (1000) martin    (1000)     9275 2021-03-20 14:26:57.000000 simple-pid-1.0.1/simple_pid/PID.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1600 2021-04-11 09:53:16.000000 simple-pid-1.0.1/simple_pid/PID.pyi
--rw-r--r--   0 martin    (1000) martin    (1000)       21 2018-10-08 20:30:43.000000 simple-pid-1.0.1/simple_pid/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)        0 2020-03-05 21:57:13.000000 simple-pid-1.0.1/simple_pid/py.typed
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.797003 simple-pid-1.0.1/simple_pid.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     7008 2021-04-11 10:02:21.000000 simple-pid-1.0.1/simple_pid.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      596 2021-04-11 10:02:21.000000 simple-pid-1.0.1/simple_pid.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2021-04-11 10:02:21.000000 simple-pid-1.0.1/simple_pid.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2021-03-20 15:29:09.000000 simple-pid-1.0.1/simple_pid.egg-info/not-zip-safe
--rw-r--r--   0 martin    (1000) martin    (1000)       29 2021-04-11 10:02:21.000000 simple-pid-1.0.1/simple_pid.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       11 2021-04-11 10:02:21.000000 simple-pid-1.0.1/simple_pid.egg-info/top_level.txt
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2021-04-11 10:02:21.797003 simple-pid-1.0.1/tests/
--rw-r--r--   0 martin    (1000) martin    (1000)        0 2021-03-20 15:27:52.000000 simple-pid-1.0.1/tests/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     5705 2021-03-20 15:11:33.000000 simple-pid-1.0.1/tests/test_pid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.161553 simple-pid-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-28 21:10:46.000000 simple-pid-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 21:10:46.000000 simple-pid-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 21:10:46.000000 simple-pid-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-28 21:10:57.161553 simple-pid-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-28 21:10:46.000000 simple-pid-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.157553 simple-pid-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 21:10:46.000000 simple-pid-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.157553 simple-pid-2.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-28 21:10:46.000000 simple-pid-2.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-28 21:10:46.000000 simple-pid-2.0.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 21:10:46.000000 simple-pid-2.0.0/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-28 21:10:46.000000 simple-pid-2.0.0/docs/source/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.157553 simple-pid-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.161553 simple-pid-2.0.0/examples/water_boiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 21:10:46.000000 simple-pid-2.0.0/examples/water_boiler/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1684 2023-04-28 21:10:46.000000 simple-pid-2.0.0/examples/water_boiler/water_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-28 21:10:46.000000 simple-pid-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 21:10:57.161553 simple-pid-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.161553 simple-pid-2.0.0/simple_pid/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:10:46.000000 simple-pid-2.0.0/simple_pid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-28 21:10:46.000000 simple-pid-2.0.0/simple_pid/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 21:10:46.000000 simple-pid-2.0.0/simple_pid/pid.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:46.000000 simple-pid-2.0.0/simple_pid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.161553 simple-pid-2.0.0/simple_pid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-28 21:10:57.000000 simple-pid-2.0.0/simple_pid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-28 21:10:57.000000 simple-pid-2.0.0/simple_pid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:10:57.000000 simple-pid-2.0.0/simple_pid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-28 21:10:57.000000 simple-pid-2.0.0/simple_pid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 21:10:57.000000 simple-pid-2.0.0/simple_pid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:57.161553 simple-pid-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:10:46.000000 simple-pid-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-28 21:10:46.000000 simple-pid-2.0.0/tests/test_pid.py
```

### Comparing `simple-pid-1.0.1/LICENSE.md` & `simple-pid-2.0.0/LICENSE.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2021 Martin Lundberg
+Copyright (c) 2018-2023 Martin Lundberg
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `simple-pid-1.0.1/README.md` & `simple-pid-2.0.0/docs/source/user_guide.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,139 @@
-# simple-pid
 
-[![Travis](https://travis-ci.com/m-lundberg/simple-pid.svg?branch=master)](https://travis-ci.com/m-lundberg/simple-pid)
-[![PyPI](https://img.shields.io/pypi/v/simple-pid.svg)](https://pypi.org/project/simple-pid/)
-[![Read the Docs](https://img.shields.io/readthedocs/simple-pid.svg)](https://simple-pid.readthedocs.io/)
-[![License](https://img.shields.io/github/license/m-lundberg/simple-pid.svg)](https://github.com/m-lundberg/simple-pid/blob/master/LICENSE.md)
-[![Downloads](https://pepy.tech/badge/simple-pid)](https://pepy.tech/project/simple-pid)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+(user_guide)=
+# User guide
+
+## Installation
+
+To install, run:
+
+```shell
+python -m pip install simple-pid
+```
 
-A simple and easy to use PID controller in Python. If you want a PID controller without external dependencies that just works, this is for you! The PID was designed to be robust with help from [Brett Beauregards guide](http://brettbeauregard.com/blog/2011/04/improving-the-beginners-pid-introduction/).
 
-Usage is very simple:
+## The basics
+
+We already saw a minimal example in {ref}`welcome`:
 
 ```python
 from simple_pid import PID
 pid = PID(1, 0.1, 0.05, setpoint=1)
 
 # Assume we have a system we want to control in controlled_system
 v = controlled_system.update(0)
 
 while True:
     # Compute new output from the PID according to the systems current value
     control = pid(v)
-    
+
     # Feed the PID output to the system and get its current value
     v = controlled_system.update(control)
 ```
 
-Complete API documentation can be found [here](https://simple-pid.readthedocs.io/en/latest/simple_pid.html#module-simple_pid.PID).
+This shows the basic structure of a PID loop. You construct a PID object and then in each loop iteration you feed it the current value of whatever system you want to control. The PID takes the error from the setpoint you want to achieve and outputs the value to feed back into the controlled system.
 
-## Installation
-To install, run:
-```
-pip install simple-pid
-```
-
-## Usage
 The `PID` class implements `__call__()`, which means that to compute a new output value, you simply call the object like this:
+
 ```python
 output = pid(current_value)
 ```
 
-### The basics
 The PID works best when it is updated at regular intervals. To achieve this, set `sample_time` to the amount of time there should be between each update and then call the PID every time in the program loop. A new output will only be calculated when `sample_time` seconds has passed:
+
 ```python
 pid.sample_time = 0.01  # Update every 0.01 seconds
 
 while True:
     output = pid(current_value)
 ```
 
 To set the setpoint, ie. the value that the PID is trying to achieve, simply set it like this:
+
 ```python
 pid.setpoint = 10
 ```
 
 The tunings can be changed any time when the PID is running. They can either be set individually or all at once:
+
 ```python
 pid.Ki = 1.0
 pid.tunings = (1.0, 0.2, 0.4)
 ```
 
+In order to get output values in a certain range, and also to avoid [integral windup](https://en.wikipedia.org/wiki/Integral_windup) (since the integral term will never be allowed to grow outside of these limits), the output can be limited to a range:
+
+```python
+pid.output_limits = (0, 10)    # Output value will be between 0 and 10
+pid.output_limits = (0, None)  # Output will always be above 0, but with no upper bound
+```
+
+
+### Reverse mode
+
 To use the PID in [reverse mode](http://brettbeauregard.com/blog/2011/04/improving-the-beginners-pid-direction/), meaning that an increase in the input leads to a decrease in the output (like when cooling for example), you can set the tunings to negative values:
 
 ```python
 pid.tunings = (-1.0, -0.1, 0)
 ```
 
 Note that all the tunings should have the same sign.
 
-In order to get output values in a certain range, and also to avoid [integral windup](https://en.wikipedia.org/wiki/Integral_windup) (since the integral term will never be allowed to grow outside of these limits), the output can be limited to a range:
-```python
-pid.output_limits = (0, 10)    # Output value will be between 0 and 10
-pid.output_limits = (0, None)  # Output will always be above 0, but with no upper bound
-```
 
-### Other features
-#### Auto mode
-To disable the PID so that no new values are computed, set auto mode to False:
+## Other features
+
+### Auto mode
+
+To disable the PID so that no new values are computed, set auto mode to `False`:
+
 ```python
 pid.auto_mode = False  # No new values will be computed when pid is called
 pid.auto_mode = True   # pid is enabled again
 ```
+
 When disabling the PID and controlling a system manually, it might be useful to tell the PID controller where to start from when giving back control to it. This can be done by enabling auto mode like this:
+
 ```python
 pid.set_auto_mode(True, last_output=8.0)
 ```
+
 This will set the I-term to the value given to `last_output`, meaning that if the system that is being controlled was stable at that output value the PID will keep the system stable if started from that point, without any big bumps in the output when turning the PID back on.
 
-#### Observing separate components
+
+### Observing separate components
+
 When tuning the PID, it can be useful to see how each of the components contribute to the output. They can be seen like this:
+
 ```python
 p, i, d = pid.components  # The separate terms are now in p, i, d
 ```
 
-#### Proportional on measurement
+
+### Proportional on measurement
+
 To eliminate overshoot in certain types of systems, you can calculate the [proportional term directly on the measurement](http://brettbeauregard.com/blog/2017/06/introducing-proportional-on-measurement/) instead of the error. This can be enabled like this:
+
 ```python
 pid.proportional_on_measurement = True
 ```
 
-#### Error mapping
-To transform the error value to another domain before doing any computations on it, you can supply an `error_map` callback function to the PID. The callback function should take one argument which is the error from the setpoint. This can be used e.g. to get a degree value error in a yaw angle control with values between [-pi, pi):
+
+### Differential on measurement
+
+By default the [differential term is calculated on the measurement](http://brettbeauregard.com/blog/2011/04/improving-the-beginner%e2%80%99s-pid-derivative-kick/) instead of the error. This can be disabled like this:
+
+```python
+pid.differential_on_measurement = False
+```
+
+
+### Error mapping
+
+To transform the error value to another domain before doing any computations on it, you can supply an `error_map` callback function to the PID. The callback function should take one argument which is the error from the setpoint. This can be used e.g. to get a degree value error in a yaw angle control with values between `[-pi, pi)`:
+
 ```python
 import math
 
 def pi_clip(angle):
     if angle > 0:
         if angle > math.pi:
             return angle - 2*math.pi
@@ -112,15 +141,16 @@
         if angle < -math.pi:
             return angle + 2*math.pi
     return angle
 
 pid.error_map = pi_clip
 ```
 
-## Tests
-Use the following to run tests:
-```
-tox
-```
 
-## License
-Licensed under the [MIT License](https://github.com/m-lundberg/simple-pid/blob/master/LICENSE.md).
+### Overriding time function
+
+By default, the PID uses `time.monotonic()` (or if not available, `time.time()` as fallback) to get the current time on each invocation. The time function can be overridden by setting `PID.time_fn` to whichever function you want to use. For example, to use the [MicroPython `time.ticks_us()`](https://docs.micropython.org/en/latest/library/time.html#time.ticks_us):
+
+```python
+import time
+pid.time_fn = time.ticks_us
+```
```

### Comparing `simple-pid-1.0.1/examples/water_boiler/README.md` & `simple-pid-2.0.0/examples/water_boiler/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # Water Boiler Example
 
 Simple simulation of a water boiler which can heat up water and where the heat dissipates slowly over time. Running the example will run the water boiler simulation for 10 seconds and use the PID controller to make the boiler reach a setpoint temperature. The results will also be plotted using [Matplotlib](https://matplotlib.org).
 
 ## Installation
 
-Optionally, create a virtual environment for this example and activate it.
+It's recommended to install the dependencies (numpy and matplotlib, in addition to the simple-pid library itself) in a virtual environment.
 
 ```bash
-python -m venv water_boiler_venv  # Assuming Python 3
-. water_boiler_venv/bin/activate
+# Linux:
+python -m venv venv
+. venv/bin/activate
+
+# Windows:
+python -m venv venv
+venv/Scripts/activate
 ```
 
 Then install the example dependencies:
 
 ```bash
-pip install -r requirements.txt
+python -m pip install ../..[examples]
 ```
 
 ## Usage
 
 ```bash
 # Activate the virtual environment if you use one:
-. water_boiler_venv/bin/activate
+. venv/bin/activate
 
 # Run the example:
 python water_boiler.py
 
 # Once you're done deactivate the virtual environment if you use one:
 deactivate
 ```
```

### Comparing `simple-pid-1.0.1/examples/water_boiler/water_boiler.py` & `simple-pid-2.0.0/examples/water_boiler/water_boiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python
 
+import os
+import sys
 import time
 import matplotlib.pyplot as plt
 from simple_pid import PID
 
 
 class WaterBoiler:
     """
@@ -54,8 +56,12 @@
         last_time = current_time
 
     plt.plot(x, y, label='measured')
     plt.plot(x, setpoint, label='target')
     plt.xlabel('time')
     plt.ylabel('temperature')
     plt.legend()
-    plt.show()
+    if os.getenv('NO_DISPLAY'):
+        # If run in CI the plot is saved to file instead of shown to the user
+        plt.savefig(f"result-py{'.'.join([str(x) for x in sys.version_info[:2]])}.png")
+    else:
+        plt.show()
```

### Comparing `simple-pid-1.0.1/simple_pid/PID.py` & `simple-pid-2.0.0/simple_pid/pid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-import time
-import warnings
-
-
 def _clamp(value, limits):
     lower, upper = limits
     if value is None:
         return None
     elif (upper is not None) and (value > upper):
         return upper
     elif (lower is not None) and (value < lower):
         return lower
     return value
 
 
-try:
-    # Get monotonic time to ensure that time deltas are always positive
-    _current_time = time.monotonic
-except AttributeError:
-    # time.monotonic() not available (using python < 3.3), fallback to time.time()
-    _current_time = time.time
-    warnings.warn('time.monotonic() not available in python < 3.3, using time.time() as fallback')
-
-
 class PID(object):
     """A simple PID controller."""
 
     def __init__(
         self,
         Kp=1.0,
         Ki=0.0,
         Kd=0.0,
         setpoint=0,
         sample_time=0.01,
         output_limits=(None, None),
         auto_mode=True,
         proportional_on_measurement=False,
+        differential_on_measurement=True,
         error_map=None,
+        time_fn=None,
+        starting_output=0.0,
     ):
         """
         Initialize a new PID controller.
 
         :param Kp: The value for the proportional gain Kp
         :param Ki: The value for the integral gain Ki
         :param Kd: The value for the derivative gain Kd
@@ -54,63 +44,92 @@
             or above the upper limit. Either of the limits can also be set to None to have no limit
             in that direction. Setting output limits also avoids integral windup, since the
             integral term will never be allowed to grow outside of the limits.
         :param auto_mode: Whether the controller should be enabled (auto mode) or not (manual mode)
         :param proportional_on_measurement: Whether the proportional term should be calculated on
             the input directly rather than on the error (which is the traditional way). Using
             proportional-on-measurement avoids overshoot for some types of systems.
+        :param differential_on_measurement: Whether the differential term should be calculated on
+            the input directly rather than on the error (which is the traditional way).
         :param error_map: Function to transform the error value in another constrained value.
+        :param time_fn: The function to use for getting the current time, or None to use the
+            default. This should be a function taking no arguments and returning a number
+            representing the current time. The default is to use time.monotonic() if available,
+            otherwise time.time().
+        :param starting_output: The starting point for the PID's output. If you start controlling
+            a system that is already at the setpoint, you can set this to your best guess at what
+            output the PID should give when first calling it to avoid the PID outputting zero and
+            moving the system away from the setpoint.
         """
         self.Kp, self.Ki, self.Kd = Kp, Ki, Kd
         self.setpoint = setpoint
         self.sample_time = sample_time
 
         self._min_output, self._max_output = None, None
         self._auto_mode = auto_mode
         self.proportional_on_measurement = proportional_on_measurement
+        self.differential_on_measurement = differential_on_measurement
         self.error_map = error_map
 
         self._proportional = 0
         self._integral = 0
         self._derivative = 0
 
         self._last_time = None
         self._last_output = None
+        self._last_error = None
         self._last_input = None
 
+        if time_fn is not None:
+            # Use the user supplied time function
+            self.time_fn = time_fn
+        else:
+            import time
+
+            try:
+                # Get monotonic time to ensure that time deltas are always positive
+                self.time_fn = time.monotonic
+            except AttributeError:
+                # time.monotonic() not available (using python < 3.3), fallback to time.time()
+                self.time_fn = time.time
+
         self.output_limits = output_limits
         self.reset()
 
+        # Set initial state of the controller
+        self._integral = _clamp(starting_output, output_limits)
+
     def __call__(self, input_, dt=None):
         """
         Update the PID controller.
 
         Call the PID controller with *input_* and calculate and return a control output if
         sample_time seconds has passed since the last update. If no new output is calculated,
         return the previous output instead (or None if no value has been calculated yet).
 
         :param dt: If set, uses this value for timestep instead of real time. This can be used in
             simulations when simulation time is different from real time.
         """
         if not self.auto_mode:
             return self._last_output
 
-        now = _current_time()
+        now = self.time_fn()
         if dt is None:
             dt = now - self._last_time if (now - self._last_time) else 1e-16
         elif dt <= 0:
             raise ValueError('dt has negative value {}, must be positive'.format(dt))
 
         if self.sample_time is not None and dt < self.sample_time and self._last_output is not None:
             # Only update every sample_time seconds
             return self._last_output
 
         # Compute error terms
         error = self.setpoint - input_
         d_input = input_ - (self._last_input if (self._last_input is not None) else input_)
+        d_error = error - (self._last_error if (self._last_error is not None) else error)
 
         # Check if must map the error
         if self.error_map is not None:
             error = self.error_map(error)
 
         # Compute the proportional term
         if not self.proportional_on_measurement:
@@ -120,34 +139,39 @@
             # Add the proportional error on measurement to error_sum
             self._proportional -= self.Kp * d_input
 
         # Compute integral and derivative terms
         self._integral += self.Ki * error * dt
         self._integral = _clamp(self._integral, self.output_limits)  # Avoid integral windup
 
-        self._derivative = -self.Kd * d_input / dt
+        if self.differential_on_measurement:
+            self._derivative = -self.Kd * d_input / dt
+        else:
+            self._derivative = self.Kd * d_error / dt
 
         # Compute final output
         output = self._proportional + self._integral + self._derivative
         output = _clamp(output, self.output_limits)
 
         # Keep track of state
         self._last_output = output
         self._last_input = input_
+        self._last_error = error
         self._last_time = now
 
         return output
 
     def __repr__(self):
         return (
             '{self.__class__.__name__}('
             'Kp={self.Kp!r}, Ki={self.Ki!r}, Kd={self.Kd!r}, '
             'setpoint={self.setpoint!r}, sample_time={self.sample_time!r}, '
             'output_limits={self.output_limits!r}, auto_mode={self.auto_mode!r}, '
-            'proportional_on_measurement={self.proportional_on_measurement!r},'
+            'proportional_on_measurement={self.proportional_on_measurement!r}, '
+            'differential_on_measurement={self.differential_on_measurement!r}, '
             'error_map={self.error_map!r}'
             ')'
         ).format(self=self)
 
     @property
     def components(self):
         """
@@ -235,10 +259,10 @@
         """
         self._proportional = 0
         self._integral = 0
         self._derivative = 0
 
         self._integral = _clamp(self._integral, self.output_limits)
 
-        self._last_time = _current_time()
+        self._last_time = self.time_fn()
         self._last_output = None
         self._last_input = None
```

### Comparing `simple-pid-1.0.1/simple_pid/PID.pyi` & `simple-pid-2.0.0/simple_pid/pid.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 _Limits = Tuple[Optional[float], Optional[float]]
 _Components = Tuple[float, float, float]
 _Tunings = Tuple[float, float, float]
 
 def _clamp(value: Optional[float], limits: _Limits) -> Optional[float]: ...
 
-_current_time: Callable[[], float]
-
 class PID(object):
     Kp: float
     Ki: float
     Kd: float
     setpoint: float
     sample_time: Optional[float]
-    output_limits: _Limits
     proportional_on_measurement: bool
+    differential_on_measurement: bool
     error_map: Optional[Callable[[float], float]]
+    time_fn: Callable[[], float]
     def __init__(
         self,
         Kp: float = ...,
         Ki: float = ...,
         Kd: float = ...,
         setpoint: float = ...,
         sample_time: Optional[float] = ...,
         output_limits: _Limits = ...,
         auto_mode: bool = ...,
         proportional_on_measurement: bool = ...,
+        differential_on_measurement: bool = ...,
         error_map: Optional[Callable[[float], float]] = ...,
+        time_fn: Optional[Callable[[], float]] = ...,
+        starting_output: float = ...,
     ) -> None: ...
     def __call__(self, input_: float, dt: Optional[float] = ...) -> Optional[float]: ...
     def __repr__(self) -> str: ...
     @property
     def components(self) -> _Components: ...
     @property
     def tunings(self) -> _Tunings: ...
```

