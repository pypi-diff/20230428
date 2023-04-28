# Comparing `tmp/tello_asyncio-2.1.2.tar.gz` & `tmp/tello_asyncio-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_asyncio-2.1.2.tar", last modified: Sat Jul 31 14:38:23 2021, max compression
+gzip compressed data, was "tello_asyncio-2.1.3.tar", last modified: Fri Apr 28 08:31:22 2023, max compression
```

## Comparing `tello_asyncio-2.1.2.tar` & `tello_asyncio-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rob        (502) staff       (20)        0 2021-07-31 14:38:23.629201 tello_asyncio-2.1.2/
--rw-r--r--   0 rob        (502) staff       (20)    26526 2021-04-26 20:49:10.000000 tello_asyncio-2.1.2/LICENSE
--rw-r--r--   0 rob        (502) staff       (20)     4342 2021-07-31 14:38:23.628603 tello_asyncio-2.1.2/PKG-INFO
--rw-r--r--   0 rob        (502) staff       (20)     3920 2021-06-18 17:58:40.000000 tello_asyncio-2.1.2/README.md
--rw-r--r--   0 rob        (502) staff       (20)       38 2021-07-31 14:38:23.629380 tello_asyncio-2.1.2/setup.cfg
--rw-r--r--   0 rob        (502) staff       (20)      678 2021-07-31 14:35:26.000000 tello_asyncio-2.1.2/setup.py
-drwxr-xr-x   0 rob        (502) staff       (20)        0 2021-07-31 14:38:23.604313 tello_asyncio-2.1.2/tello_asyncio/
--rw-r--r--   0 rob        (502) staff       (20)    29050 2021-07-31 12:16:31.000000 tello_asyncio-2.1.2/tello_asyncio/Tello.py
--rw-r--r--   0 rob        (502) staff       (20)      226 2021-06-04 10:14:48.000000 tello_asyncio-2.1.2/tello_asyncio/__init__.py
--rw-r--r--   0 rob        (502) staff       (20)     2724 2021-05-23 11:00:07.000000 tello_asyncio-2.1.2/tello_asyncio/state.py
--rw-r--r--   0 rob        (502) staff       (20)     1998 2021-06-04 10:14:48.000000 tello_asyncio-2.1.2/tello_asyncio/types.py
--rw-r--r--   0 rob        (502) staff       (20)     1464 2021-06-13 16:56:10.000000 tello_asyncio-2.1.2/tello_asyncio/video.py
--rw-r--r--   0 rob        (502) staff       (20)     2016 2021-06-18 17:41:03.000000 tello_asyncio-2.1.2/tello_asyncio/wifi.py
-drwxr-xr-x   0 rob        (502) staff       (20)        0 2021-07-31 14:38:23.627630 tello_asyncio-2.1.2/tello_asyncio.egg-info/
--rw-r--r--   0 rob        (502) staff       (20)     4342 2021-07-31 14:38:23.000000 tello_asyncio-2.1.2/tello_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 rob        (502) staff       (20)      373 2021-07-31 14:38:23.000000 tello_asyncio-2.1.2/tello_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (502) staff       (20)        1 2021-07-31 14:38:23.000000 tello_asyncio-2.1.2/tello_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (502) staff       (20)        1 2021-04-26 21:26:12.000000 tello_asyncio-2.1.2/tello_asyncio.egg-info/not-zip-safe
--rw-r--r--   0 rob        (502) staff       (20)       14 2021-07-31 14:38:23.000000 tello_asyncio-2.1.2/tello_asyncio.egg-info/top_level.txt
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-04-28 08:31:22.745751 tello_asyncio-2.1.3/
+-rw-r--r--   0 rob        (501) staff       (20)    26526 2022-06-02 06:34:42.000000 tello_asyncio-2.1.3/LICENSE
+-rw-r--r--   0 rob        (501) staff       (20)     4658 2023-04-28 08:31:22.745614 tello_asyncio-2.1.3/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     4256 2023-04-27 06:41:35.000000 tello_asyncio-2.1.3/README.md
+-rw-r--r--   0 rob        (501) staff       (20)       38 2023-04-28 08:31:22.745792 tello_asyncio-2.1.3/setup.cfg
+-rw-r--r--   0 rob        (501) staff       (20)      678 2023-04-27 06:36:29.000000 tello_asyncio-2.1.3/setup.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-04-28 08:31:22.744744 tello_asyncio-2.1.3/tello_asyncio/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2023-04-27 06:33:02.000000 tello_asyncio-2.1.3/tello_asyncio/__init__.py
+-rw-r--r--   0 rob        (501) staff       (20)     2910 2023-04-27 06:33:02.000000 tello_asyncio-2.1.3/tello_asyncio/state.py
+-rw-r--r--   0 rob        (501) staff       (20)    29388 2023-04-27 06:34:22.000000 tello_asyncio-2.1.3/tello_asyncio/tello.py
+-rw-r--r--   0 rob        (501) staff       (20)     2029 2023-04-27 06:33:02.000000 tello_asyncio-2.1.3/tello_asyncio/types.py
+-rw-r--r--   0 rob        (501) staff       (20)     1464 2023-04-27 06:33:02.000000 tello_asyncio-2.1.3/tello_asyncio/video.py
+-rw-r--r--   0 rob        (501) staff       (20)     2006 2023-04-27 06:33:02.000000 tello_asyncio-2.1.3/tello_asyncio/wifi.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2023-04-28 08:31:22.745450 tello_asyncio-2.1.3/tello_asyncio.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)     4658 2023-04-28 08:31:22.000000 tello_asyncio-2.1.3/tello_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)      350 2023-04-28 08:31:22.000000 tello_asyncio-2.1.3/tello_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-04-28 08:31:22.000000 tello_asyncio-2.1.3/tello_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2022-06-25 08:24:17.000000 tello_asyncio-2.1.3/tello_asyncio.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       14 2023-04-28 08:31:22.000000 tello_asyncio-2.1.3/tello_asyncio.egg-info/top_level.txt
```

### Comparing `tello_asyncio-2.1.2/LICENSE` & `tello_asyncio-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tello_asyncio-2.1.2/PKG-INFO` & `tello_asyncio-2.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tello_asyncio
-Version: 2.1.2
+Version: 2.1.3
 Summary: Asyncio-based control library for the Tello drone
 Home-page: https://github.com/robagar/tello-asyncio
 Author: Rob Agar
 Author-email: tello_asyncio@fastmail.net
 License: LGPL
 Project-URL: Documentation, https://tello-asyncio.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tello-asyncio
 
 A library for controlling and interacting with the [Tello EDU](https://www.ryzerobotics.com/tello-edu) drone using [modern asynchronous Python](https://docs.python.org/3/library/asyncio.html).  All operations are implemented as awaitable coroutines, completed when the drone sends acknowledgment of the command message.
@@ -41,14 +40,16 @@
 
 See the [examples](examples) directory for more usage example scripts.
 
 Requires Python 3.6+. Developed and tested with Python 3.9.4 in Mac OS and 3.6.9 in Ubuntu 18.04 on a [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano-developer-kit).  The *tello_asyncio* package has no other dependencies (and never will have any), but some examples need other things to be installed to work.
 
 Full documentation is available on [Read the docs](https://tello-asyncio.readthedocs.io/en/latest/)
 
+(If Rust is more your thing, there is also an equivalent aynchronous Rust library [tello-edu](https://crates.io/crates/tello-edu)) 
+
 ## Tello SDK Support
 
 * [Tello SDK 2.0](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20SDK%202.0%20User%20Guide.pdf) (Tello EDU) - complete support
 * [Tello SDK 3.0](https://dl.djicdn.com/downloads/RoboMaster+TT/Tello_SDK_3.0_User_Guide_en.pdf) (RoboMaster TT) - complete support, but `EXT` commands for controlling LEDs etc must be formatted by the user
 
 ## A Note on Awaiting
 
@@ -148,10 +149,18 @@
 - Wait for Wifi network implemented for macOS as well as Linux
 - Mission pad fixes & example improvement (thanks @jsolderitsch!)
 
 **2.1.1**
 
 - Examples ask the user for the WiFi name prefix
 
+**2.1.2**
+
+- Don't wait for a response from remote control (`rc x x x x`) commands
+
+**2.1.3**
 
+- Various SDK 3.0 fixes (thanks @jdelfino!)
+- Handle "forced stop" message which arrives out of sequence
 
+
```

### Comparing `tello_asyncio-2.1.2/README.md` & `tello_asyncio-2.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 See the [examples](examples) directory for more usage example scripts.
 
 Requires Python 3.6+. Developed and tested with Python 3.9.4 in Mac OS and 3.6.9 in Ubuntu 18.04 on a [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano-developer-kit).  The *tello_asyncio* package has no other dependencies (and never will have any), but some examples need other things to be installed to work.
 
 Full documentation is available on [Read the docs](https://tello-asyncio.readthedocs.io/en/latest/)
 
+(If Rust is more your thing, there is also an equivalent aynchronous Rust library [tello-edu](https://crates.io/crates/tello-edu)) 
+
 ## Tello SDK Support
 
 * [Tello SDK 2.0](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20SDK%202.0%20User%20Guide.pdf) (Tello EDU) - complete support
 * [Tello SDK 3.0](https://dl.djicdn.com/downloads/RoboMaster+TT/Tello_SDK_3.0_User_Guide_en.pdf) (RoboMaster TT) - complete support, but `EXT` commands for controlling LEDs etc must be formatted by the user
 
 ## A Note on Awaiting
 
@@ -134,8 +136,18 @@
 - Wait for Wifi network implemented for macOS as well as Linux
 - Mission pad fixes & example improvement (thanks @jsolderitsch!)
 
 **2.1.1**
 
 - Examples ask the user for the WiFi name prefix
 
+**2.1.2**
+
+- Don't wait for a response from remote control (`rc x x x x`) commands
+
+**2.1.3**
+
+- Various SDK 3.0 fixes (thanks @jdelfino!)
+- Handle "forced stop" message which arrives out of sequence
+
+
```

### Comparing `tello_asyncio-2.1.2/setup.py` & `tello_asyncio-2.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='tello_asyncio',
-      version='2.1.2',
+      version='2.1.3',
       description='Asyncio-based control library for the Tello drone',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/robagar/tello-asyncio',
       project_urls={
             'Documentation': 'https://tello-asyncio.readthedocs.io/en/latest/'
       },
```

### Comparing `tello_asyncio-2.1.2/tello_asyncio/Tello.py` & `tello_asyncio-2.1.3/tello_asyncio/tello.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,889 +3,924 @@
 from inspect import iscoroutinefunction
 
 from .types import Direction, MissionPadDetection, ControllerHardware
 from .state import TelloStateListener, STATE_FIELDS
 from .video import TelloVideoListener, VIDEO_URL
 from .wifi import wait_for_wifi
 
-DEFAULT_DRONE_HOST = '192.168.10.1'
+DEFAULT_DRONE_HOST = "192.168.10.1"
 
 CONTROL_UDP_PORT = 8889
 STATE_UDP_PORT = 8890
 
 DEFAULT_RESPONSE_TIMEOUT = 10
 LONG_RESPONSE_TIMEOUT = 60
 
+
 class Tello:
-    '''
+    """
     For ayncio-based interaction with the Tello EDU drone.
 
     :param drone_host: Drone IP address, defaults to '192.168.10.1'
     :param on_state: Callback called when state data is received from the drone, taking :class:`tello_asyncio.tello.Tello` drone and :class:`tello_asyncio.types.TelloState` state arguments.
     :type on_state: Callable, optional
     :param on_video_frame: Called when video frame data is received from the drone, taking :class:`tello_asyncio.tello.Tello` drone and `bytes` frame argument containing the raw data from the drone.
     :type on_video_frame: Callable, optional
     :param on_error: Called when a command fails for any reason, taking :class:`tello_asyncio.tello.Tello` drone and :class:`tello_asyncio.tello.Tello.Error` frame arguments.
     :type on_video_frame: Callable or awaitable function, optional
-    '''
+    """
 
     _protocol = None
     _transport = None
 
     _state = None
     _video = None
     _flying = False
     _wifi_ssid_prefix = None
     _sdk_version = None
     _controller_hardware = None
 
     class Error(Exception):
-        '''
+        """
         Exception thrown if anything goes wrong controlling the drone.
-        '''
+        """
+
         pass
 
     class Protocol:
-        '''
+        """
         UDP protocol for drone control using the Tello SDK.
         The basic flow from the user's point of view is
 
            SEND command → drone does something → RECEIVE response when it's finished
 
         Messages are plain ASCII text, eg command `forward 10` → response `ok`
-        '''
+        """
+
         def connection_made(self, transport):
             self.pending = deque()
 
         def datagram_received(self, data, addr):
             try:
-                message = data.decode('ascii')
+                message = data.decode("ascii")
             except UnicodeDecodeError as e:
-                raise Tello.Error(f'DECODE ERROR {e} (data: {data})')
-                
-            print('RECEIVED', message)
+                raise Tello.Error(f"DECODE ERROR {e} (data: {data})")
+
+            print("RECEIVED", message)
+
+            if message == "forced stop":
+                print("FORCED STOP")
+                return
+
             try:
                 sent_message, response, response_parser = self.pending.popleft()
                 if response_parser:
                     result = response_parser(message)
-                else:    
-                    if message == 'ok':
+                else:
+                    if message == "ok" or message == "matrix ok":
                         result = None
                     else:
                         response.set_exception(Tello.Error(message))
                         return
                 response.set_result((sent_message, result))
 
             except IndexError:
-                raise Tello.Error('NOT WAITING FOR RESPONSE')
+                raise Tello.Error("NOT WAITING FOR RESPONSE")
             except asyncio.InvalidStateError:
                 pass
 
         def error_received(self, error):
-            raise Tello.Error(f'PROTOCOL ERROR {error}')
+            raise Tello.Error(f"PROTOCOL ERROR {error}")
 
         def connection_lost(self, error):
             # print('CONNECTION LOST', error)
             for m, response, rp in self.pending:
                 response.cancel()
             self.pending.clear()
 
-    def __init__(self, drone_host=DEFAULT_DRONE_HOST, on_state=None, on_video_frame=None, on_error=None):
-        '''
+    def __init__(
+        self,
+        drone_host=DEFAULT_DRONE_HOST,
+        on_state=None,
+        on_video_frame=None,
+        on_error=None,
+    ):
+        """
         Constructor
-        '''
+        """
         self._drone_host = drone_host
         self._on_state_callback = on_state
         self._on_video_frame_callback = on_video_frame
         self._on_error = on_error
         self._loop = asyncio.get_event_loop()
 
     async def connect(self):
-        '''
+        """
         Opens the UDP connection to the drone and puts it in SDK mode.
 
         :return: The response from the drone
-        '''
-        print(f'CONNECT {self._drone_host}')
+        """
+        print(f"CONNECT {self._drone_host}")
 
         transport, protocol = await self._loop.create_datagram_endpoint(
-            Tello.Protocol, 
+            Tello.Protocol,
             local_addr=("0.0.0.0", CONTROL_UDP_PORT),
-            remote_addr=(self._drone_host, CONTROL_UDP_PORT)
+            remote_addr=(self._drone_host, CONTROL_UDP_PORT),
         )
 
         self._transport = transport
         self._protocol = protocol
 
         self._state_listener = TelloStateListener(local_port=STATE_UDP_PORT)
         await self._state_listener.connect(self._loop, self._on_state_received)
         self._state_event = asyncio.Event()
 
         # tell drone to be in SDK mode
-        response = await self.send('command')
+        response = await self.send("command")
 
         # check battery
         b = await self.query_battery()
         if b < 10:
-            print(f'WARNING low battery: {b}%')
+            print(f"WARNING low battery: {b}%")
         else:
-            print(f'battery: {b}%')
+            print(f"battery: {b}%")
 
         return response
 
     async def disconnect(self):
-        '''
+        """
         Closes all UDP connections to this drone.
-        '''
+        """
         if self._transport and not self._transport.is_closing():
-            print(f'DISCONNECT {self._drone_host}')
+            print(f"DISCONNECT {self._drone_host}")
 
             self._transport.close()
             await self._state_listener.disconnect()
             if self._video:
                 await self._video.disconnect()
 
     @property
     async def serial_number(self):
-        '''
+        """
         The unique drone serial number.
-        '''
-        return await self.send('sn?', response_parser=lambda m: m)
+        """
+        return await self.send("sn?", response_parser=lambda m: m)
 
     @property
     async def sdk_version(self):
-        '''
+        """
         The Tello SDK version.
-        '''
+        """
         if not self._sdk_version:
-            self._sdk_version = await self.send('sdk?', response_parser=lambda m: m)
+            self._sdk_version = await self.send("sdk?", response_parser=lambda m: m)
         return self._sdk_version
 
     async def query_battery(self):
-        '''
+        """
         The battery level as a percentage, requested directly from the drone.
-        '''
-        return await self.send('battery?', response_parser=lambda m: int(m))
+        """
+        return await self.send("battery?", response_parser=lambda m: int(m))
 
     async def query_motor_time(self):
-        '''
+        """
         The active motor time in seconds, requested directly from the drone.
-        '''
-        return await self.send('time?', response_parser=lambda m: int(m))
+        """
+        return await self.send("time?", response_parser=lambda m: int(m))
 
     async def emergency_stop(self):
-        '''
-        Stop all motors immediately.  Warning - this will make the drone drop like a brick.        
-        '''
-        await self.send('emergency')
+        """
+        Stop all motors immediately.  Warning - this will make the drone drop like a brick.
+        """
+        await self.send("emergency")
 
     async def takeoff(self):
-        '''
+        """
         Take off and hover.
 
         :return: The response from the drone
-        '''
+        """
         self._flying = True
-        return await self.send('takeoff')
+        return await self.send("takeoff")
 
     async def land(self):
-        '''
+        """
         Land and stop motors.
 
         :return: The response from the drone
-        '''
-        return await self.send('land')
+        """
+        return await self.send("land")
         self._flying = False
 
     @property
     def flying(self):
-        '''
+        """
         True if `takeoff` has been called but `land` has not.
-        '''
+        """
         return self._flying
 
     @property
     async def speed(self):
-        '''
+        """
         The drone speed in cm/s, requested directly from the drone.
-        '''
-        return await self.send('speed?', response_parser=lambda m: float(m))
+        """
+        return await self.send("speed?", response_parser=lambda m: float(m))
 
     async def set_speed(self, speed):
-        '''
+        """
         Set the forward speed.
 
         :param speed: Desired speed, 10-100 cm/s
         :return: The response from the drone
-        '''
-        return await self.send(f'speed {speed}')
+        """
+        return await self.send(f"speed {speed}")
 
     async def stop(self):
-        '''
+        """
         Stop and hover in place.
 
         :return: The response from the drone
-        '''
-        return await self.send('stop')
+        """
+        return await self.send("stop")
 
     async def turn_clockwise(self, degrees):
-        '''
+        """
         Turn clockwise.
 
         :param degrees: int, Angle in degrees 1-360°
         :return: The response from the drone
-        '''
-        return await self.send(f'cw {round(degrees)}')    
+        """
+        return await self.send(f"cw {round(degrees)}")
 
     async def turn_counterclockwise(self, degrees):
-        '''
+        """
         Turn anticlockwise.
 
         :param degrees: Angle in degrees 1-360°
         :return: The response from the drone
-        '''
-        return await self.send(f'ccw {round(degrees)}')
+        """
+        return await self.send(f"ccw {round(degrees)}")
 
     async def move(self, direction, distance):
-        '''
+        """
         Move in a straight line in the given direction.
 
         :param direction: Direction of movement
         :type direction: :class:`tello_asyncio.types.Direction`
         :param distance: The distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
+        """
         if direction == Direction.UP:
-            return await self.move_up(distance)    
+            return await self.move_up(distance)
         if direction == Direction.DOWN:
-            return await self.move_down(distance)    
+            return await self.move_down(distance)
         if direction == Direction.LEFT:
-            return await self.move_left(distance)    
+            return await self.move_left(distance)
         if direction == Direction.RIGHT:
-            return await self.move_right(distance)    
+            return await self.move_right(distance)
         if direction == Direction.FORWARD:
-            return await self.move_forward(distance)    
+            return await self.move_forward(distance)
         if direction == Direction.BACK:
             return await self.move_back(distance)
-        raise ValueError('invalid move direction')    
+        raise ValueError("invalid move direction")
 
     async def move_up(self, distance):
-        '''
+        """
         Move straight up.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'up {distance}')
+        """
+        return await self.send(f"up {distance}")
 
     async def move_down(self, distance):
-        '''
+        """
         Move straight down.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'down {distance}')
+        """
+        return await self.send(f"down {distance}")
 
     async def move_left(self, distance):
-        '''
+        """
         Move straight left.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'left {distance}')
+        """
+        return await self.send(f"left {distance}")
 
     async def move_right(self, distance):
-        '''
+        """
         Move straight right.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'right {distance}')
+        """
+        return await self.send(f"right {distance}")
 
     async def move_forward(self, distance):
-        '''
+        """
         Move straight forwards.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'forward {distance}')
+        """
+        return await self.send(f"forward {distance}")
 
     async def move_back(self, distance):
-        '''
+        """
         Move straight backwards.
 
         :param distance: Distance to travel, 20-500 cm
         :return: The response from the drone
-        '''
-        return await self.send(f'back {distance}')
+        """
+        return await self.send(f"back {distance}")
 
     async def flip(self, direction):
-        '''
+        """
         Do a flip in the given direction.
 
         :param direction: The direction to flip in.
-        :type direction: :class:`tello_asyncio.types.Direction` 
+        :type direction: :class:`tello_asyncio.types.Direction`
         :return: The response from the drone
-        '''
+        """
         if direction == Direction.LEFT:
-            return await self.flip_left()    
+            return await self.flip_left()
         if direction == Direction.RIGHT:
-            return await self.flip_right()    
+            return await self.flip_right()
         if direction == Direction.FORWARD:
-            return await self.flip_forward()    
+            return await self.flip_forward()
         if direction == Direction.BACK:
             return await self.flip_back()
-        raise ValueError('invalid flip direction')    
+        raise ValueError("invalid flip direction")
 
     async def flip_left(self):
-        '''
+        """
         Flip left.
 
         :return: The response from the drone
-        '''
-        return await self.send('flip l')
+        """
+        return await self.send("flip l")
 
     async def flip_right(self):
-        '''
+        """
         Flip right.
 
         :return: The response from the drone
-        '''
-        return await self.send('flip r')
+        """
+        return await self.send("flip r")
 
     async def flip_forward(self):
-        '''
+        """
         Flip forwards.
 
         :return: The response from the drone
-        '''
-        return await self.send('flip f')
+        """
+        return await self.send("flip f")
 
     async def flip_back(self):
-        '''
+        """
         Flip backwards.
 
         :return: The response from the drone
-        '''
-        await self.send('flip b')
+        """
+        await self.send("flip b")
 
     async def go_to(self, relative_position, speed, mission_pad=None):
-        '''
-        Go to the given position, either relative to a mission pad if given, 
+        """
+        Go to the given position, either relative to a mission pad if given,
         otherwise relative to the current position.
 
         :param relative_position: Position relative to drone or mission pad
         :type relative_position: :class:`tello_asyncio.types.Vector`
         :param mission_pad: The mission pad ID, 1-8
-        :type mission_pad: int, optional 
+        :type mission_pad: int, optional
         :return: The response from the drone
-        '''
+        """
         p = relative_position
-        command = f'go {p.x} {p.y} {p.z} {speed}'
+        command = f"go {p.x} {p.y} {p.z} {speed}"
         if mission_pad:
-            command += f' m{mission_pad}'
+            command += f" m{mission_pad}"
         return await self.send(command, timeout=LONG_RESPONSE_TIMEOUT)
 
-    async def curve_to(self, via_relative_position, relative_position, speed, mission_pad=None):
-        '''
-        Fly in a curve defined by the two positions, which must lie on a circle with a radius of 50cm - 10m. 
+    async def curve_to(
+        self, via_relative_position, relative_position, speed, mission_pad=None
+    ):
+        """
+        Fly in a curve defined by the two positions, which must lie on a circle with a radius of 50cm - 10m.
 
         :param via_relative_position: First position relative to drone or mission pad
         :type via_relative_position: :class:`tello_asyncio.types.Vector`
         :param relative_position: Destination relative to drone or mission pad
         :type relative_position: :class:`tello_asyncio.types.Vector`
         :param speed: The speed to travel at 10-60cm/s
         :type speed: int
         :param mission_pad: The mission pad ID, 1-8
-        :type mission_pad: int, optional 
+        :type mission_pad: int, optional
         :return: The response from the drone
-        '''
+        """
         p = relative_position
         v = via_relative_position
-        command = f'curve {v.x} {v.y} {v.z} {p.x} {p.y} {p.z} {speed}'
+        command = f"curve {v.x} {v.y} {v.z} {p.x} {p.y} {p.z} {speed}"
         if mission_pad:
-            command += f' m{mission_pad}'
+            command += f" m{mission_pad}"
         return await self.send(command, timeout=LONG_RESPONSE_TIMEOUT)
 
     async def enable_mission_pads(self):
-        '''
+        """
         Start attempting to detect mission pads.
 
         :return: The response from the drone
-        '''
-        return await self.send('mon')
+        """
+        return await self.send("mon")
 
     async def disable_mission_pads(self):
-        '''
+        """
         Stop detecting mission pads.
 
         :return: The response from the drone
-        '''
-        return await self.send('moff')
+        """
+        return await self.send("moff")
 
     async def set_mission_pad_detection(self, mission_pad_detection):
-        '''
+        """
         Sets the directions to look for mission pads in - forwards, down or both.
-        
+
         :param mission_pad_detection: Forwards, down or both.
         :param mission_pad_detection: :class:`tello_asyncio.types.MissionPadDetection`
         :return: The response from the drone
-        '''
-        return await self.send(f'mdirection {mission_pad_detection.value}')
+        """
+        return await self.send(f"mdirection {mission_pad_detection.value}")
 
-    async def jump(self, relative_position, speed, yaw, from_mission_pad, to_mission_pad):
-        '''
+    async def jump(
+        self, relative_position, speed, yaw, from_mission_pad, to_mission_pad
+    ):
+        """
         Travel from one mission pad to another.
-        
+
         :param relative_position: Final position relative to the mission pad.
         :type relative_position: :class:`tello_asyncio.types.Vector`
         :param speed: Speed of travel, 10-100 cm/s
         :param yaw: Angle to turn on arrival 0-360°
         :return: The response from the drone
-        '''
+        """
         p = relative_position
-        command = f'jump {p.x} {p.y} {p.z} {speed} {yaw} m{from_mission_pad} m{to_mission_pad}'
+        command = f"jump {p.x} {p.y} {p.z} {speed} {yaw} m{from_mission_pad} m{to_mission_pad}"
         return await self.send(command)
 
     async def remote_control(self, left_right, forward_back, up_down, yaw):
-        '''
+        """
         Send remote control commands.
 
         :param left_right: Desired speed to the left, -100-100 cm/s
         :param forward_back: Desired speed forwards, -100-100 cm/s
         :param up_down: Desired speed up, -100-100 cm/s
         :param yaw: Desired yaw -100-100°/s
         :return: The response from the drone
-        '''
-        return await self.send(f'rc {left_right} {forward_back} {up_down} {yaw}')
+        """
+        return await self.send(f"rc {left_right} {forward_back} {up_down} {yaw}")
 
     async def set_wifi_credentials(self, ssid, password):
-        '''
+        """
         Set credentials for the drone's own WiFi network
 
         :param ssid: Network name
         :param password: Password
         :return: The response from the drone
-        '''
+        """
         self._wifi_ssid_prefix = ssid
-        return await self.send(f'wifi {ssid} {password}')
+        return await self.send(f"wifi {ssid} {password}")
 
     async def connect_to_wifi(self, ssid, password):
-        '''
+        """
         Connect to another WiFi network and reboot.
 
         NB this also sets the Wifi network prefix used by `wifi_wait_for_network`
- 
+
         :param ssid: Network name
         :param password: Password
         :return: The response from the drone
-        '''
+        """
         self._wifi_ssid_prefix = ssid
-        return await self.send(f'ap {ssid} {password}')
+        return await self.send(f"ap {ssid} {password}")
 
     @property
     async def wifi_signal_to_noise_ratio(self):
-        '''
+        """
         The signal-to-noise ratio of the WiFi connection.
-        '''
-        return await self.send('wifi?', response_parser=lambda m: int(m))
+        """
+        return await self.send("wifi?", response_parser=lambda m: int(m))
 
     async def wifi_wait_for_network(self, prefix=None, prompt=False):
-        '''
+        """
         Waits until the WiFi network is established.
-        
-        NB: 
+
+        NB:
         - This does not actually connect to the WiFi network
         - Only works on Linux and macOS
 
         :param prefix: The WiFi network SSID name prefix, defaults to the hardware string "RMTT" or "TELLO" (if known, otherwise "TELLO")
         :param prompt: If true, ask the user for the prefix
-        '''
+        """
         if prompt:
-            prefix = input('Please enter the WiFi network name prefix to look for, eg "RMTT". Defaults to "TELLO"> ')
+            prefix = input(
+                'Please enter the WiFi network name prefix to look for, eg "RMTT". Defaults to "TELLO"> '
+            )
         if prefix:
             self._wifi_ssid_prefix = prefix
         if not prefix:
-            prefix = self._controller_hardware or 'TELLO'
+            prefix = self._controller_hardware or "TELLO"
 
-        print(f'waiting for WiFi ({prefix})...')
+        print(f"waiting for WiFi ({prefix})...")
         try:
             await wait_for_wifi(prefix)
         except Exception as e:
-            print(f'...wait for WiFi failed, error: {e}')
-            print('assuming WiFi network is connected and continuing')
+            print(f"...wait for WiFi failed, error: {e}")
+            print("assuming WiFi network is connected and continuing")
 
-    async def send(self, message, timeout=DEFAULT_RESPONSE_TIMEOUT, response_parser=None):
-        '''
+    async def send(
+        self, message, timeout=DEFAULT_RESPONSE_TIMEOUT, response_parser=None
+    ):
+        """
         Send a command message and wait for response.
 
         :param message: The command string
         :param timeout: Time to wait in seconds for a response
-        :param response_parser: A function that converts the response into a return value. 
+        :param response_parser: A function that converts the response into a return value.
         :return: The response from the drone
         :rtype: str, unless `response_parser` is used.
-        '''
+        """
         if not self._transport.is_closing():
-            print(f'SEND {message}')
-            
+            print(f"SEND {message}")
+
             self._transport.sendto(message.encode())
             if not self._expect_response(message):
                 return
 
             response = self._loop.create_future()
             self._protocol.pending.append((message, response, response_parser))
             error = None
             try:
-                response_message, result = await asyncio.wait_for(response, timeout=timeout)
+                response_message, result = await asyncio.wait_for(
+                    response, timeout=timeout
+                )
                 if response_message == message:
                     return result
                 else:
-                    error = Tello.Error('RESPONSE WRONG MESSAGE "{response_message}", expected "{message}" (UDP packet loss detected)')
+                    error = Tello.Error(
+                        'RESPONSE WRONG MESSAGE "{response_message}", expected "{message}" (UDP packet loss detected)'
+                    )
             except asyncio.TimeoutError:
-                error = Tello.Error(f'[{message}] TIMEOUT')
+                error = Tello.Error(f"[{message}] TIMEOUT")
             except Tello.Error as e:
-                error = Tello.Error(f'[{message}] ERROR {e}')
-    
+                error = Tello.Error(f"[{message}] ERROR {e}")
+
             if self._on_error:
                 # user callback
                 if iscoroutinefunction(self._on_error):
                     await self._on_error(self, error)
                 else:
                     self._on_error(self, error)
             else:
                 # default behaviour
                 await self._abort()
                 raise error
 
     def _expect_response(self, message):
         # drone responds to everything except remote control commands
-        return not message.startswith('rc ')
+        return not message.startswith("rc ")
 
     _aborted = False
+
     async def _abort(self):
         if not self._aborted:
             self._aborted = True
             if self._flying:
                 await self.land()
             await self.disconnect()
 
     @property
     def state(self):
-        '''
+        """
         The current state of the drone, if any.
 
         :rtype: :class:`tello_asyncio.types.TelloState`
-        '''
+        """
         return self._state
 
     @property
     async def state_stream(self):
-        '''
+        """
         In infinite stream of drone state objects.
-        
+
         :rtype: :class:`tello_asyncio.types.TelloState`
-        '''
+        """
         while True:
             await self._state_event.wait()
             yield self._state
 
     def _on_state_received(self, state):
         if self._on_state_callback:
             self._on_state_callback(self, state)
 
         self._state = state
         self._state_event.set()
         self._state_event.clear()
 
     def __getattr__(self, name):
-        '''
+        """
         Shortcut to the drone state :class:`tello_asyncio.types.TelloState` properties.
-        '''
+        """
         if name in STATE_FIELDS:
             if self._state:
                 return getattr(self._state, name)
             else:
                 return None
-        raise AttributeError(f"'Tello' object has no attribute {name}") 
+        raise AttributeError(f"'Tello' object has no attribute {name}")
 
     @property
     def video_url(self):
-        '''
+        """
         The URL for video data, if `start_video` has been called.
-        '''
+        """
         return VIDEO_URL
 
     async def start_video(self, on_frame=None, connect=True):
-        '''
+        """
         Start streaming video data.  Only works in AP mode using the drone's own WiFi.
 
         :param on_frame: Callback called when a new frame arrives, taking :class:`tello_asyncio.tello.Tello` drone and `bytes` frame raw data arguments
         :type on_frame: Callable, optional
         :param connect: Whether to start receiving frame data, default `True`
         :type connect: Boolean, optional
         :return: The response from the drone
-        '''
+        """
         if connect:
             await self.connect_video(on_frame)
-        return await self.send('streamon')
- 
+        return await self.send("streamon")
+
     async def stop_video(self):
-        '''
+        """
         Stop streaming video.
 
         :return: The response from the drone
-        '''
-        return await self.send('streamoff')
+        """
+        return await self.send("streamoff")
 
     async def connect_video(self, on_frame=None):
-        '''
-        Opens a connection to the `video_url` and listens for the video frame 
+        """
+        Opens a connection to the `video_url` and listens for the video frame
         data streamed after `start_video` is called.
 
         :param on_frame: Callback called when a new frame arrives, taking :class:`tello_asyncio.tello.Tello` drone and `bytes` frame raw data arguments
         :type on_frame: Callable, optional
-        '''
+        """
         if on_frame:
             self._on_video_frame_callback = on_frame
         self._video = TelloVideoListener()
         self._video_frame_chunk_event = asyncio.Event()
         self._video_frame_event = asyncio.Event()
-        await self._video.connect(self._loop, self._on_video_frame_chunk, self._on_video_frame)
+        await self._video.connect(
+            self._loop, self._on_video_frame_chunk, self._on_video_frame
+        )
 
     def _on_video_frame_chunk(self, frame_chunk):
         self._video_frame_chunk = frame_chunk
         self._video_frame_chunk_event.set()
         self._video_frame_chunk_event.clear()
 
     def _on_video_frame(self, frame):
         if self._on_video_frame_callback:
             self._on_video_frame_callback(self, frame)
         self._video_frame = frame
         self._video_frame_event.set()
         self._video_frame_event.clear()
 
     _video_frame = None
+
     @property
     def video_frame(self):
-        '''
+        """
         The most recent raw frame data, if any,
 
         :rtype: `bytes`
-        '''
+        """
         return self._video_frame
 
     @property
     async def video_chunk_stream(self):
-        '''
+        """
         Infinite stream of video frame data chunks.
-        
+
         :rtype: `bytes`
-        '''
+        """
         while True:
             await self._video_frame_chunk_event.wait()
             yield self._video_frame_chunk
 
     @property
     async def video_stream(self):
-        '''
+        """
         Infinite stream of video frame data.
-        
+
         :rtype: `bytes`
-        '''
+        """
         while True:
             await self._video_frame_event.wait()
             yield self._video_frame
 
     ##########################################################################
     # Tello SDK 3.x
 
     async def _require_sdk_3(self):
         v = await self.sdk_version
-        if not v.startswith('3'):
-            raise Tello.Error(f'SDK version 3 required. Drone SDK version string is "{v}"') 
+        if not v.startswith("3"):
+            raise Tello.Error(
+                f'SDK version 3 required. Drone SDK version string is "{v}"'
+            )
 
     async def _require_open_source_controller(self):
         h = await self.controller_hardware
-        if not h == ControllerHardware.OPEN_SOURCE:
-            raise Tello.Error(f'Requires the open source TT controller.  Drone hardware is "{h}"')
+        if not h == ControllerHardware.OPEN_SOURCE.value:
+            raise Tello.Error(
+                f'Requires the open source TT controller ("{ControllerHardware.OPEN_SOURCE.value}"). '
+                + f'Drone hardware is "{h}"'
+            )
 
     async def motor_on(self):
-        '''
+        """
         Starts the motors at low speed to keep the drone cool while lon the ground.
 
         Requires SDK 3+
 
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send('motoron')
+        return await self.send("motoron")
 
     async def motor_off(self):
-        '''
+        """
         Stops the motors if started in low speed mode.
 
         Requires SDK 3+
 
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send('motoroff')
+        return await self.send("motoroff")
 
     async def throw_fly(self):
-        '''
+        """
         Launch the drone by throwing horizontally within 5 seconds.
 
         Requires SDK 3+
 
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send('throwfly')
+        return await self.send("throwfly")
 
     async def reboot(self):
-        '''
+        """
         Reboot the drone.
 
         Requires SDK 3+
-        
+
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send('reboot')
+        return await self.send("reboot")
 
     async def set_wifi_channel(self, wifi_channel):
-        '''
+        """
         Sets the Wifi channel.
-        
+
         Requires SDK 3+ and the open source controller.
 
         :param wifi_channel: The WiFi channel
         :return: The response from the drone
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send(f'wifisetchannel {wifi_channel}')
+        return await self.send(f"wifisetchannel {wifi_channel}")
 
     async def set_ports(self, status_port, video_port):
-        '''
+        """
         Sets the UDP ports for status and video data.
 
         Requires SDK 3+
-        
+
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send(f'port {status_port} {video_port}')
+        return await self.send(f"port {status_port} {video_port}")
 
     async def set_video_frame_rate(self, frame_rate):
-        '''
+        """
         Sets the video frame rate.
 
         Requires SDK 3+
-        
+
         :param frame_rate: "low" (5fps), "middle" (15fps) or "high" (30fps)
         :type frame_rate: :class:`tello_asyncio.types.VideoFrameRate`
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send(f'setfps {frame_rate}')
+        return await self.send(f"setfps {frame_rate}")
 
     async def set_video_bit_rate(self, bit_rate):
-        '''
+        """
         Sets the video bit rate.
 
         Requires SDK 3+
-        
+
         :param bit_rate: 1-5Mbps, or zero for auto
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send(f'setbitrate {bit_rate}')
+        return await self.send(f"setbitrate {bit_rate}")
 
     async def set_video_resolution(self, resolution):
-        '''
+        """
         Sets the video resolution.
 
         Requires SDK 3+
 
         :param resolution: "low" 480p or "high" 720p
         :type frame_rate: :class:`tello_asyncio.types.VideoResolution`
         :return: The response from the drone
-        '''
+        """
         await self._require_sdk_3()
-        return await self.send(f'setbitrate {bit_rate}')
+        return await self.send(f"setbitrate {bit_rate}")
 
     @property
     async def controller_hardware(self):
-        '''
+        """
         The controller hardware - "TELLO" or "RMTT" for the open source controller.
 
         Requires SDK 3+
-        '''
+        """
         await self._require_sdk_3()
         if not self._controller_hardware:
-            self._controller_hardware = await self.send('hardware?')
+            self._controller_hardware = await self.send(
+                "hardware?", response_parser=lambda m: m.strip()
+            )
         return self._controller_hardware
 
     @property
     async def wifi_version(self):
-        '''
+        """
         The WiFi version.
 
         Requires SDK 3+ and the open source controller
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send('wifiversion?')
+        return await self.send("wifiversion?")
 
     @property
     async def wifi_name_and_password(self):
-        '''
+        """
         The WiFi access point name and password.
 
         Requires SDK 3+ and the open source controller
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send('ap?')
+        return await self.send("ap?")
 
     @property
     async def wifi_ssid(self):
-        '''
+        """
         The WiFi SSID.
 
         Requires SDK 3+ and the open source controller
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send('ssid?')
+        return await self.send("ssid?")
 
     async def set_multi_wifi_credentials(self, ssid, password):
-        '''
+        """
         Set WiFi credentials for connecting to multiple devices as a router.
 
         Requires SDK 3+ and the open source controller.
 
         :param ssid: Network name
         :param password: Password
         :return: The response from the drone
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send(f'multiwifi {ssid} {password}')
+        return await self.send(f"multiwifi {ssid} {password}")
 
     async def send_ext_command(self, command):
-        '''
+        """
         Sends a command like "EXT xxx" for the open source contoller, returning
         the response.
 
         See the `SDK 3.0 User Guide <https://dl.djicdn.com/downloads/RoboMaster+TT/Tello_SDK_3.0_User_Guide_en.pdf>`_ for command details.
 
         Requires SDK 3+ and the open source controller
 
         :param ssid: Network name
         :param password: Password
         :return: The response from the drone
-        '''
+        """
         await self._require_open_source_controller()
-        return await self.send(f'EXT {command}')
-                        
-    
+        return await self.send(f"EXT {command}")
```

### Comparing `tello_asyncio-2.1.2/tello_asyncio/types.py` & `tello_asyncio-2.1.3/tello_asyncio/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 from collections import namedtuple
 from enum import Enum
 
 
-Range = namedtuple('Range', 'low high')
-Range.low.__doc__ = 'minimum value'
-Range.high.__doc__ = 'maximum value'
-
-Vector = namedtuple('Vector', 'x y z')
-Vector.x.__doc__ = 'x value' 
-Vector.y.__doc__ = 'y value' 
-Vector.z.__doc__ = 'z value' 
-
-TelloState = namedtuple('TelloState', 'raw roll pitch yaw height barometer battery time_of_flight motor_time temperature acceleration velocity mission_pad mission_pad_position')
-TelloState.raw.__doc__ = 'Raw state message string'
-TelloState.roll.__doc__ = 'Rotation in degrees around the drone\'s local y axis'
-TelloState.pitch.__doc__ = 'Rotation in degrees around the drone\'s local x axis'
-TelloState.yaw.__doc__ = 'Rotation in degrees around the drone\'s local z axis'
-TelloState.height.__doc__ = 'Height in cm'
-TelloState.barometer.__doc__ = 'Atmospheric pressure'
-TelloState.battery.__doc__ = 'Remaining battery percentage'
-TelloState.time_of_flight.__doc__ = 'Time of flight returned by the height sensor'
-TelloState.motor_time.__doc__ = 'Time in seconds the motors have been active for'
-TelloState.temperature.__doc__ = 'Range in temperature in degrees Celsius'
-TelloState.acceleration.__doc__ = ':class:`tello_asyncio.types.Vector` acceleration in cm/s/s in each axis direction'
-TelloState.velocity.__doc__ = ':class:`tello_asyncio.types.Vector` speed in cm/s in each axis direction'
-TelloState.mission_pad.__doc__ = 'Mission pad ID'
-TelloState.mission_pad_position.__doc__ = ':class:`tello_asyncio.types.Vector` mission pad relative position'
+Range = namedtuple("Range", "low high")
+Range.low.__doc__ = "minimum value"
+Range.high.__doc__ = "maximum value"
+
+Vector = namedtuple("Vector", "x y z")
+Vector.x.__doc__ = "x value"
+Vector.y.__doc__ = "y value"
+Vector.z.__doc__ = "z value"
+
+TelloState = namedtuple(
+    "TelloState",
+    "raw roll pitch yaw height barometer battery time_of_flight motor_time temperature acceleration velocity mission_pad mission_pad_position",
+)
+TelloState.raw.__doc__ = "Raw state message string"
+TelloState.roll.__doc__ = "Rotation in degrees around the drone's local y axis"
+TelloState.pitch.__doc__ = "Rotation in degrees around the drone's local x axis"
+TelloState.yaw.__doc__ = "Rotation in degrees around the drone's local z axis"
+TelloState.height.__doc__ = "Height in cm"
+TelloState.barometer.__doc__ = "Atmospheric pressure"
+TelloState.battery.__doc__ = "Remaining battery percentage"
+TelloState.time_of_flight.__doc__ = "Time of flight returned by the height sensor"
+TelloState.motor_time.__doc__ = "Time in seconds the motors have been active for"
+TelloState.temperature.__doc__ = "Range in temperature in degrees Celsius"
+TelloState.acceleration.__doc__ = (
+    ":class:`tello_asyncio.types.Vector` acceleration in cm/s/s in each axis direction"
+)
+TelloState.velocity.__doc__ = (
+    ":class:`tello_asyncio.types.Vector` speed in cm/s in each axis direction"
+)
+TelloState.mission_pad.__doc__ = "Mission pad ID"
+TelloState.mission_pad_position.__doc__ = (
+    ":class:`tello_asyncio.types.Vector` mission pad relative position"
+)
 
 
 class Direction(Enum):
-    UP = 'up'
-    DOWN = 'down'
-    LEFT = 'left'
-    RIGHT = 'right'
-    FORWARD = 'forward'
-    BACK = 'back'
+    UP = "up"
+    DOWN = "down"
+    LEFT = "left"
+    RIGHT = "right"
+    FORWARD = "forward"
+    BACK = "back"
+
 
 class MissionPadDetection(Enum):
     DOWN = 0
     FORWARD = 1
-    BOTH = 2 
+    BOTH = 2
+
 
 class VideoFrameRate(Enum):
-    LOW = 'low'
-    MIDDLE = 'middle'
-    HIGH = 'high'
+    LOW = "low"
+    MIDDLE = "middle"
+    HIGH = "high"
+
 
 class VideoResolution(Enum):
-    LOW = 'low'
-    HIGH = 'high'
+    LOW = "low"
+    HIGH = "high"
 
-class ControllerHardware(Enum):
-    TELLO = 'TELLO'
-    OPEN_SOURCE = 'RMTT'
 
+class ControllerHardware(Enum):
+    TELLO = "TELLO"
+    OPEN_SOURCE = "RMTT"
```

### Comparing `tello_asyncio-2.1.2/tello_asyncio/video.py` & `tello_asyncio-2.1.3/tello_asyncio/video.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 VIDEO_UDP_PORT = 11111
-VIDEO_URL = f'udp://0.0.0.0:{VIDEO_UDP_PORT}'
+VIDEO_URL = f"udp://0.0.0.0:{VIDEO_UDP_PORT}"
 
 VIDEO_WIDTH = 960
 VIDEO_HEIGHT = 720
 
 MAX_CHUNK_SIZE = 1460
 
+
 class TelloVideoListener:
-    '''
-    Connects to the drone's video data stream and reassembles h.264 encoded 
+    """
+    Connects to the drone's video data stream and reassembles h.264 encoded
     frames from UDP packet chunks before passing them on.
-    '''
+    """
 
     _transport = None
 
     class Protocol:
         def connection_made(self, transport):
             self._chunks = []
 
         def datagram_received(self, data, addr):
             self.on_video_frame_chunk_received(data)
             self._chunks.append(data)
             if len(data) != MAX_CHUNK_SIZE:
-                frame = b''.join(self._chunks)
-                self._chunks = [] 
+                frame = b"".join(self._chunks)
+                self._chunks = []
                 self.on_frame_received(frame)
 
         def error_received(self, error):
-            print('[video] PROTOCOL ERROR', error)
+            print("[video] PROTOCOL ERROR", error)
 
         def connection_lost(self, error):
             pass
 
-    async def connect(self, loop, on_video_frame_chunk_received, on_video_frame_received):
+    async def connect(
+        self, loop, on_video_frame_chunk_received, on_video_frame_received
+    ):
         transport, protocol = await loop.create_datagram_endpoint(
-            TelloVideoListener.Protocol, 
-            local_addr=("0.0.0.0", VIDEO_UDP_PORT)
+            TelloVideoListener.Protocol, local_addr=("0.0.0.0", VIDEO_UDP_PORT)
         )
         self._transport = transport
-        protocol.on_video_frame_chunk_received = on_video_frame_chunk_received 
+        protocol.on_video_frame_chunk_received = on_video_frame_chunk_received
         protocol.on_frame_received = on_video_frame_received
 
     async def disconnect(self):
         if self._transport:
             self._transport.close()
-            self._transport = None
+            self._transport = None
```

### Comparing `tello_asyncio-2.1.2/tello_asyncio/wifi.py` & `tello_asyncio-2.1.3/tello_asyncio/wifi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 import asyncio
 import platform
 
 
 async def wait_for_wifi(ssid_prefix):
     system = platform.system()
 
-    if system == 'Linux':
+    if system == "Linux":
         await wait_for_wifi_linux(ssid_prefix)
-    elif system == 'Darwin':
+    elif system == "Darwin":
         await wait_for_wifi_macos(ssid_prefix)
     else:
-        raise Exception(f'wait_for_wifi not implemented for {system}')
+        raise Exception(f"wait_for_wifi not implemented for {system}")
 
 
 async def wait_for_wifi_linux(ssid_prefix):
     while True:
-        s,e = await run_shell('iwgetid -r')
+        s, e = await run_shell("iwgetid -r")
         if e:
             raise Exception(e)
-        if s and s.startswith(ssid_prefix): 
+        if s and s.startswith(ssid_prefix):
             return
         await asyncio.sleep(0.25)
 
 
 async def wait_for_wifi_macos(ssid_prefix):
     async def get_devices():
-        s, e = await run_shell('networksetup -listallhardwareports')
+        s, e = await run_shell("networksetup -listallhardwareports")
 
         if s:
             devices = []
             found_wifi = False
             for line in s.splitlines():
                 if not found_wifi:
                     # looking for something like "Hardware Port: Wi-Fi"
-                    if 'Wi-Fi' in line:
+                    if "Wi-Fi" in line:
                         found_wifi = True
                 else:
                     # ... then next like should be like "Device: en1"
-                    devices.append(line[len('Device: '):])
+                    devices.append(line[len("Device: ") :])
                     found_wifi = False
             return devices
         else:
             raise Exception(e)
 
     # find all WiFi devices
     devices = await get_devices()
- 
+
     # wait for any one of them to connect
-    waiting_for = f'Current Wi-Fi Network: {ssid_prefix}'
+    waiting_for = f"Current Wi-Fi Network: {ssid_prefix}"
     while True:
         for device in devices:
-            s,e = await run_shell(f'networksetup -getairportnetwork {device}')
+            s, e = await run_shell(f"networksetup -getairportnetwork {device}")
             if s and s.startswith(waiting_for):
                 return
         await asyncio.sleep(0.25)
 
 
 async def run_shell(cmd):
     proc = await asyncio.create_subprocess_shell(
-        cmd,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE)
+        cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
+    )
 
     stdout, stderr = await proc.communicate()
 
     if proc.returncode == 0:
         return stdout.decode(), None
     else:
         return None, stderr.decode()
```

### Comparing `tello_asyncio-2.1.2/tello_asyncio.egg-info/PKG-INFO` & `tello_asyncio-2.1.3/tello_asyncio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tello-asyncio
-Version: 2.1.2
+Version: 2.1.3
 Summary: Asyncio-based control library for the Tello drone
 Home-page: https://github.com/robagar/tello-asyncio
 Author: Rob Agar
 Author-email: tello_asyncio@fastmail.net
 License: LGPL
 Project-URL: Documentation, https://tello-asyncio.readthedocs.io/en/latest/
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tello-asyncio
 
 A library for controlling and interacting with the [Tello EDU](https://www.ryzerobotics.com/tello-edu) drone using [modern asynchronous Python](https://docs.python.org/3/library/asyncio.html).  All operations are implemented as awaitable coroutines, completed when the drone sends acknowledgment of the command message.
@@ -41,14 +40,16 @@
 
 See the [examples](examples) directory for more usage example scripts.
 
 Requires Python 3.6+. Developed and tested with Python 3.9.4 in Mac OS and 3.6.9 in Ubuntu 18.04 on a [Jetson Nano](https://developer.nvidia.com/embedded/jetson-nano-developer-kit).  The *tello_asyncio* package has no other dependencies (and never will have any), but some examples need other things to be installed to work.
 
 Full documentation is available on [Read the docs](https://tello-asyncio.readthedocs.io/en/latest/)
 
+(If Rust is more your thing, there is also an equivalent aynchronous Rust library [tello-edu](https://crates.io/crates/tello-edu)) 
+
 ## Tello SDK Support
 
 * [Tello SDK 2.0](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20SDK%202.0%20User%20Guide.pdf) (Tello EDU) - complete support
 * [Tello SDK 3.0](https://dl.djicdn.com/downloads/RoboMaster+TT/Tello_SDK_3.0_User_Guide_en.pdf) (RoboMaster TT) - complete support, but `EXT` commands for controlling LEDs etc must be formatted by the user
 
 ## A Note on Awaiting
 
@@ -148,10 +149,18 @@
 - Wait for Wifi network implemented for macOS as well as Linux
 - Mission pad fixes & example improvement (thanks @jsolderitsch!)
 
 **2.1.1**
 
 - Examples ask the user for the WiFi name prefix
 
+**2.1.2**
+
+- Don't wait for a response from remote control (`rc x x x x`) commands
+
+**2.1.3**
 
+- Various SDK 3.0 fixes (thanks @jdelfino!)
+- Handle "forced stop" message which arrives out of sequence
 
+
```

