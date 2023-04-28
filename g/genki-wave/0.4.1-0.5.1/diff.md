# Comparing `tmp/genki-wave-0.4.1.tar.gz` & `tmp/genki-wave-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genki-wave-0.4.1.tar", last modified: Fri Oct 14 18:33:09 2022, max compression
+gzip compressed data, was "genki-wave-0.5.1.tar", last modified: Fri Apr 28 14:03:30 2023, max compression
```

## Comparing `genki-wave-0.4.1.tar` & `genki-wave-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-10-14 18:33:09.734200 genki-wave-0.4.1/
--rw-r--r--   0 robert     (501) staff       (20)     1079 2022-05-09 09:33:46.000000 genki-wave-0.4.1/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     4032 2022-10-14 18:33:09.734048 genki-wave-0.4.1/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     3408 2022-05-09 09:33:46.000000 genki-wave-0.4.1/README.md
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-10-14 18:33:09.730413 genki-wave-0.4.1/examples/
--rw-r--r--   0 robert     (501) staff       (20)        0 2022-05-09 09:33:46.000000 genki-wave-0.4.1/examples/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)       82 2022-05-09 09:33:46.000000 genki-wave-0.4.1/examples/discover_wave.py
--rw-r--r--   0 robert     (501) staff       (20)     1677 2022-06-28 16:34:24.000000 genki-wave-0.4.1/examples/run_async.py
--rw-r--r--   0 robert     (501) staff       (20)     6221 2022-05-09 09:33:46.000000 genki-wave-0.4.1/examples/run_midi.py
--rw-r--r--   0 robert     (501) staff       (20)     2295 2022-05-09 09:33:46.000000 genki-wave-0.4.1/examples/run_threads.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-10-14 18:33:09.731864 genki-wave-0.4.1/genki_wave/
--rw-r--r--   0 robert     (501) staff       (20)        0 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)     8694 2022-08-09 14:30:08.000000 genki-wave-0.4.1/genki_wave/asyncio_runner.py
--rw-r--r--   0 robert     (501) staff       (20)     3520 2022-08-09 14:30:08.000000 genki-wave-0.4.1/genki_wave/callbacks.py
--rw-r--r--   0 robert     (501) staff       (20)       73 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/constants.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-10-14 18:33:09.733828 genki-wave-0.4.1/genki_wave/data/
--rw-r--r--   0 robert     (501) staff       (20)      200 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/data/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)     1281 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/data/enums.py
--rw-r--r--   0 robert     (501) staff       (20)     9400 2022-10-06 10:42:08.000000 genki-wave-0.4.1/genki_wave/data/organization.py
--rw-r--r--   0 robert     (501) staff       (20)     1909 2022-08-09 14:47:13.000000 genki-wave-0.4.1/genki_wave/data/points.py
--rw-r--r--   0 robert     (501) staff       (20)      621 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/data/structures.py
--rw-r--r--   0 robert     (501) staff       (20)     1106 2022-08-09 14:30:08.000000 genki-wave-0.4.1/genki_wave/data/writing.py
--rw-r--r--   0 robert     (501) staff       (20)      649 2022-10-14 18:24:54.000000 genki-wave-0.4.1/genki_wave/discover.py
--rw-r--r--   0 robert     (501) staff       (20)     5853 2022-08-09 14:30:08.000000 genki-wave-0.4.1/genki_wave/protocols.py
--rw-r--r--   0 robert     (501) staff       (20)     4224 2022-05-09 09:33:46.000000 genki-wave-0.4.1/genki_wave/threading_runner.py
--rw-r--r--   0 robert     (501) staff       (20)     1324 2022-10-14 18:24:54.000000 genki-wave-0.4.1/genki_wave/utils.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2022-10-14 18:33:09.732537 genki-wave-0.4.1/genki_wave.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     4032 2022-10-14 18:33:09.000000 genki-wave-0.4.1/genki_wave.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      675 2022-10-14 18:33:09.000000 genki-wave-0.4.1/genki_wave.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2022-10-14 18:33:09.000000 genki-wave-0.4.1/genki_wave.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       37 2022-10-14 18:33:09.000000 genki-wave-0.4.1/genki_wave.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)       20 2022-10-14 18:33:09.000000 genki-wave-0.4.1/genki_wave.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)       38 2022-10-14 18:33:09.734244 genki-wave-0.4.1/setup.cfg
--rw-r--r--   0 robert     (501) staff       (20)      919 2022-10-14 18:30:37.000000 genki-wave-0.4.1/setup.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.385147 genki-wave-0.5.1/
+-rw-r--r--   0 egill      (501) staff       (20)     1079 2022-05-09 10:31:46.000000 genki-wave-0.5.1/LICENSE
+-rw-r--r--   0 egill      (501) staff       (20)     4012 2023-04-28 14:03:30.384994 genki-wave-0.5.1/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)     3408 2022-05-09 10:31:46.000000 genki-wave-0.5.1/README.md
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.382039 genki-wave-0.5.1/examples/
+-rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.1/examples/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)       82 2022-05-09 10:31:46.000000 genki-wave-0.5.1/examples/discover_wave.py
+-rw-r--r--   0 egill      (501) staff       (20)     1838 2023-04-28 14:02:22.000000 genki-wave-0.5.1/examples/run_async.py
+-rw-r--r--   0 egill      (501) staff       (20)     6221 2023-04-27 12:53:23.000000 genki-wave-0.5.1/examples/run_midi.py
+-rw-r--r--   0 egill      (501) staff       (20)     2295 2023-04-27 12:53:23.000000 genki-wave-0.5.1/examples/run_threads.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.383193 genki-wave-0.5.1/genki_wave/
+-rw-r--r--   0 egill      (501) staff       (20)        0 2022-05-09 10:31:46.000000 genki-wave-0.5.1/genki_wave/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     9335 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/asyncio_runner.py
+-rw-r--r--   0 egill      (501) staff       (20)     3973 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/callbacks.py
+-rw-r--r--   0 egill      (501) staff       (20)      100 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/constants.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.384824 genki-wave-0.5.1/genki_wave/data/
+-rw-r--r--   0 egill      (501) staff       (20)      274 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/__init__.py
+-rw-r--r--   0 egill      (501) staff       (20)     1412 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/enums.py
+-rw-r--r--   0 egill      (501) staff       (20)    12462 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/organization.py
+-rw-r--r--   0 egill      (501) staff       (20)     1909 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/data/points.py
+-rw-r--r--   0 egill      (501) staff       (20)      621 2022-05-09 10:31:46.000000 genki-wave-0.5.1/genki_wave/data/structures.py
+-rw-r--r--   0 egill      (501) staff       (20)     1904 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/data/writing.py
+-rw-r--r--   0 egill      (501) staff       (20)      649 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/discover.py
+-rw-r--r--   0 egill      (501) staff       (20)     6230 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/protocols.py
+-rw-r--r--   0 egill      (501) staff       (20)     4328 2023-04-28 14:02:22.000000 genki-wave-0.5.1/genki_wave/threading_runner.py
+-rw-r--r--   0 egill      (501) staff       (20)     1324 2023-04-27 12:53:23.000000 genki-wave-0.5.1/genki_wave/utils.py
+drwxr-xr-x   0 egill      (501) staff       (20)        0 2023-04-28 14:03:30.383908 genki-wave-0.5.1/genki_wave.egg-info/
+-rw-r--r--   0 egill      (501) staff       (20)     4012 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/PKG-INFO
+-rw-r--r--   0 egill      (501) staff       (20)      675 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 egill      (501) staff       (20)        1 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 egill      (501) staff       (20)       37 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/requires.txt
+-rw-r--r--   0 egill      (501) staff       (20)       20 2023-04-28 14:03:30.000000 genki-wave-0.5.1/genki_wave.egg-info/top_level.txt
+-rw-r--r--   0 egill      (501) staff       (20)       38 2023-04-28 14:03:30.385207 genki-wave-0.5.1/setup.cfg
+-rw-r--r--   0 egill      (501) staff       (20)      919 2023-04-28 14:03:02.000000 genki-wave-0.5.1/setup.py
```

### Comparing `genki-wave-0.4.1/LICENSE` & `genki-wave-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/PKG-INFO` & `genki-wave-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: genki-wave
-Version: 0.4.1
+Version: 0.5.1
 Summary: Python API for Wave by Genki
 Home-page: https://github.com/genkiinstruments/genki-wave
 Author: Robert Torfason
 Author-email: robert@genkiinstruments.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -83,9 +82,7 @@
   connected to the computer. After pairing Wave to a Linux machine Wave tends to connect automatically quite
   aggressively and cannot be accessed via bleak. One solution is to use `bluetoothctl` to disconnect before pairing
   with `genki-wave`.
 * Wave needs to be off and disconnected before receiving any data via the serial port.
 * There is an error when you have Wave connected via Bluetooth and use `asyncio` to receive data.
   If you kill the program, e.g., with a keyboard interrupt, Wave stays connected and has an invalid state.
   For the time being you can hold the top button for a few seconds to properly exit the program.
-
-
```

### Comparing `genki-wave-0.4.1/README.md` & `genki-wave-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/examples/run_async.py` & `genki-wave-0.5.1/examples/run_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--ble-address", type=str)
     parser.add_argument("--use-serial", action="store_true")
     parser.add_argument("--button", action="store_true", help="Handler that prints the button and the action")
     parser.add_argument(
+        "--enable-spectrogram", action="store_true", help="Enable on-device FFT and spectrogram binning"
+    )
+    parser.add_argument(
         "--csv", type=str, default=None, help="Path to the output csv. If none is given no csv is written"
     )
     parser.add_argument("--log", type=str, default=None)
     args = parser.parse_args()
     log_level = getattr(logging, args.log.upper() if args.log else "WARNING", logging.WARNING)
     logging.basicConfig(format="%(levelname).4s:%(asctime)s [%(filename)s:%(lineno)d] - %(message)s ", level=log_level)
 
@@ -34,12 +37,12 @@
         run_asyncio_serial(callbacks)
     else:
         if args.ble_address is None:
             print("No bluetooth address (--ble-address) supplied, searching for devices...")
             run_discover_bluetooth()
         else:
             print("Turn off by holding the `TOP` button")
-            run_asyncio_bluetooth(callbacks, args.ble_address)
+            run_asyncio_bluetooth(callbacks, args.ble_address, args.enable_spectrogram)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `genki-wave-0.4.1/examples/run_midi.py` & `genki-wave-0.5.1/examples/run_midi.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/examples/run_threads.py` & `genki-wave-0.5.1/examples/run_threads.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/genki_wave/asyncio_runner.py` & `genki-wave-0.5.1/genki_wave/asyncio_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 import serial
 from bleak import BleakClient
 from serial_asyncio import open_serial_connection
 
 from genki_wave.callbacks import WaveCallback
 from genki_wave.constants import API_CHAR_UUID, BAUDRATE
-from genki_wave.data.writing import get_start_api_package
+from genki_wave.data.writing import (
+    get_device_info_request,
+    get_start_api_package,
+    get_start_spectrogram_package,
+    get_default_api_config_package,
+)
 from genki_wave.protocols import ProtocolAsyncio, ProtocolThread, CommunicateCancel
 from genki_wave.utils import get_serial_port, get_or_create_event_loop
 
 logger = logging.getLogger(__name__)
 
 
 def prepare_protocol_as_bleak_callback_asyncio(protocol: ProtocolAsyncio) -> Callable:
@@ -59,14 +64,15 @@
     return cb
 
 
 async def producer_bluetooth(
     protocol: Union[ProtocolAsyncio, ProtocolThread],
     comm: CommunicateCancel,
     ble_address: str,
+    enable_spectrogram: bool = False,
 ) -> None:
     """Receives data from a serially connected wave ring and passes it to the `protocol`
 
     Args:
         protocol: An object that knows how to process the raw data sent from the Wave ring into a structured format
                   and passes it along between `producer` and `consumer`.
         comm: An object that allows `producer` and `consumer` to communicate when to cancel the process
@@ -76,16 +82,22 @@
         The producer doesn't return a value, but the data gets added to the `protocol` that can be accessed from other
         parts of the program i.e. some `consumer`
     """
     print(f"Connecting to wave at address {ble_address}")
     callback = bleak_callback(protocol)
     async with BleakClient(ble_address, disconnected_callback=make_disconnect_callback(comm)) as client:
         await client.start_notify(API_CHAR_UUID, callback)
+        await client.write_gatt_char(API_CHAR_UUID, get_device_info_request(), False)
         await client.write_gatt_char(API_CHAR_UUID, get_start_api_package(), False)
 
+        if enable_spectrogram:
+            await client.write_gatt_char(API_CHAR_UUID, get_start_spectrogram_package(), False)
+        else:
+            await client.write_gatt_char(API_CHAR_UUID, get_default_api_config_package(), False)
+
         print("Connected to Wave")
         while True:
             # This `while` loop and `asyncio.sleep` statement is some magic that is required to continually fetch
             # the data from the bluetooth device.
             await asyncio.sleep(0.1)
 
             if comm.cancel:
@@ -183,22 +195,27 @@
     loop.add_signal_handler(signal.SIGINT, make_sigint_handler(comm))
 
     # Note: The consumer and the producer send the data via the instance of `protocol`
     tasks = asyncio.gather(producer(protocol, comm), consumer(protocol, comm, callbacks))
     loop.run_until_complete(tasks)
 
 
-def run_asyncio_bluetooth(callbacks: List[WaveCallback], ble_address) -> None:
+def run_asyncio_bluetooth(callbacks: List[WaveCallback], ble_address, enable_spectrogram=False) -> None:
     """Runs an async `consumer-producer` loop using user supplied callbacks for a bluetooth device
 
     Args:
         callbacks: A list/tuple of callbacks that handle the data passed from the wave ring
         ble_address: Address of the bluetooth device to connect to. E.g. 'D5:73:DB:85:B4:A1'
+        enable_spectrogram: Enable on-device FFT and spectrogram binning
     """
-    _run_asyncio(callbacks, partial(producer_bluetooth, ble_address=ble_address), ProtocolAsyncio())
+    _run_asyncio(
+        callbacks,
+        partial(producer_bluetooth, ble_address=ble_address, enable_spectrogram=enable_spectrogram),
+        ProtocolAsyncio(),
+    )
 
 
 def run_asyncio_serial(callbacks: List[WaveCallback], serial_port: str = None) -> None:
     """Runs an async `consumer-producer` loop using user supplied callbacks for a serial device
 
     Args:
         callbacks: A list/tuple of callbacks that handle the data passed from the wave ring
```

### Comparing `genki-wave-0.4.1/genki_wave/callbacks.py` & `genki-wave-0.5.1/genki_wave/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import abc
 import csv
 from pathlib import Path
 from typing import Union, Optional, TextIO
 
-from genki_wave.data import ButtonEvent, DataPackage
+from genki_wave.data import DeviceInfo, ButtonEvent, Package, DataPackage, RawDataPackage, SpectrogramDataPackage
+from genki_wave.constants import FIRMWARE_VERSION
 
 
 class WaveCallback(abc.ABC):
     @abc.abstractmethod
     def _button_handler(self, data: ButtonEvent) -> None:
         pass
 
     @abc.abstractmethod
-    def _data_handler(self, data: DataPackage) -> None:
+    def _data_handler(self, data: Package) -> None:
         pass
 
-    def __call__(self, data: Union[ButtonEvent, DataPackage]) -> None:
+    def __call__(self, data: Union[ButtonEvent, Package]) -> None:
         if isinstance(data, ButtonEvent):
             self._button_handler(data)
-        elif isinstance(data, DataPackage):
+        elif isinstance(data, (DataPackage, RawDataPackage, SpectrogramDataPackage)):
             self._data_handler(data)
+        elif isinstance(data, DeviceInfo):
+            if data.version != FIRMWARE_VERSION:
+                raise ValueError(f"Firmware not up to date, required: {FIRMWARE_VERSION}, device has: {data.version}")
         else:
             raise ValueError(f"Got data of unexpected type {type(data)}")
 
 
 class ButtonAndDataPrint(WaveCallback):
     """
     Callback that prints out all button presses received and prints a data package every `print_data_every_n_seconds`
@@ -37,20 +41,20 @@
         self._last_time = None
         self._print_data_every_n_seconds = print_data_every_n_seconds
 
     def _button_handler(self, data: ButtonEvent) -> None:
         # We use `str` to force the `enum` to print the long version of the name e.g. `ButtonId.MIDDLE` instead of `1`
         print(f"Button: {str(data.button_id)}, Action: {str(data.action)}")
 
-    def _data_handler(self, data: DataPackage) -> None:
+    def _data_handler(self, data: Package) -> None:
         """If there are more than `_print_data_every_n_seconds` seconds since something was printed out, print it"""
         if self._print_data_every_n_seconds is None:
             return
 
-        if self._last_time is None:
+        if self._last_time is None or self._last_time > data.timestamp_us:
             self._last_time = data.timestamp_us
 
         if (data.timestamp_us - self._last_time) > self._print_data_every_n_seconds * 10**6:  # s to us
             print(data)
             self._last_time = data.timestamp_us
 
 
@@ -82,15 +86,18 @@
 
     def _reset_state(self) -> None:
         self._events = []
 
     def _button_handler(self, data: ButtonEvent) -> None:
         pass
 
-    def _data_handler(self, data: DataPackage) -> None:
+    def _data_handler(self, data: Package) -> None:
+        if not isinstance(data, DataPackage):
+            return
+
         """Receives the data and writes it out if enough data points have been collected"""
         self._events.append(data)
 
         if len(self._events) < self._flush_len:
             return
 
         with open(self._filename, "a") as f:
```

### Comparing `genki-wave-0.4.1/genki_wave/data/enums.py` & `genki-wave-0.5.1/genki_wave/data/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     DEVICE_INFO = 3
     BUTTON_EVENT = 4
     DEVICE_MODE = 5
     IDENTIFY = 6
     RECENTER = 7
     DISPLAY_FRAME = 8
     RAW_DATA = 9
+    SPECTROGRAM = 10
+    MODIFY_API_CONFIG = 11
 
 
 class PackageType(IntEnum):
     REQUEST = 1
     RESPONSE = 2
     STREAM = 3
 
@@ -30,14 +32,20 @@
     """Which button is a package representing"""
 
     TOP = 0
     MIDDLE = 1
     BOTTOM = 2
 
 
+class DatastreamType(IntEnum):
+    NONE = 0
+    MOTION_DATA = 1
+    RAW_DATA = 2
+
+
 class ButtonAction(IntEnum):
     """The action of a button package
 
     Up: button was released
     Down: button was pressed down
     Long: a long press was detected (button down for 500ms or more)
     LongUp: a long press was released (I think you'll always receive an "up" event with this one)
```

### Comparing `genki-wave-0.4.1/genki_wave/data/organization.py` & `genki-wave-0.5.1/genki_wave/data/organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import struct
 from dataclasses import Field, dataclass, field
 from struct import unpack_from
 from typing import Optional, Union
 
 from genki_wave.data.enums import ButtonAction, ButtonId, PackageId, PackageType
 from genki_wave.data.points import Euler3d, Point3d, Quaternion, rotate_vector
@@ -34,17 +36,23 @@
 
     def is_data(self):
         return self.id == PackageId.DATASTREAM
 
     def is_button(self):
         return self.id == PackageId.BUTTON_EVENT
 
+    def is_device_info(self):
+        return self.id == PackageId.DEVICE_INFO
+
     def is_raw_gyro_accel(self):
         return self.id == PackageId.RAW_DATA
 
+    def is_spectrogram(self):
+        return self.id == PackageId.SPECTROGRAM
+
 
 @dataclass(frozen=True)
 class DataPackage:
     """Represents a data package sent from wave
 
     Note: Initializing DataClasses is (relatively) slow, if in the unlikely event this becomes a bottleneck,
           refactor into a new structure
@@ -186,14 +194,89 @@
     def from_raw_bytes(cls, data: Union[bytearray, bytes]) -> "ButtonEvent":
         """Decomposes raw bytes into its components and returns them as a :class:`ButtonEvent`"""
         assert len(data) == cls._raw_len, f"Expected to get {cls._raw_len} bytes, got {len(data)}"
         button_id, action = unpack_from("<BB", data, 0)
         return cls(button_id=ButtonId(button_id), action=ButtonAction(action))
 
 
+@dataclass(frozen=True)
+class DeviceInfo:
+    """Represents a button event sent from wave"""
+
+    _raw_len = 35
+
+    version: str
+    board_version: str
+    mac_address: str
+    serial_number: str
+
+    @classmethod
+    def from_raw_bytes(cls, data: Union[bytearray, bytes]) -> "DeviceInfo":
+        """Decomposes raw bytes into its components and returns them as a :class:`ButtonEvent`"""
+        assert len(data) == cls._raw_len, f"Expected to get {cls._raw_len} bytes, got {len(data)}"
+
+        version = unpack_from("<3B", data[0:3])
+        board_version = unpack_from("9s", data[3:12])
+        mac_address = unpack_from("<6B", data[12:18])
+        serial_number = unpack_from("17s", data[18:35])
+
+        return cls(
+            version=".".join(f"{x}" for x in version),
+            board_version=board_version[0].decode("utf-8").rstrip("\x00"),
+            mac_address=":".join(f"{b:02x}" for b in mac_address).strip().upper(),
+            serial_number=serial_number[0].decode("utf-8").rstrip("\x00"),
+        )
+
+
+@dataclass(frozen=True)
+class SpectrogramDataPackage:
+    """Represents a column in a spectrogram sent from wave"""
+
+    _num_bins_per_channel = 16
+    _num_channels = 6
+    _num_floats = _num_bins_per_channel * _num_channels
+
+    _data_len = _num_floats * 4
+    _timestamp_bytes = 8
+    _raw_len = _data_len + _timestamp_bytes
+
+    _data_format_str = f"<{_num_floats}f"
+
+    data: list[float]
+    timestamp_us: int
+
+    @classmethod
+    def from_raw_bytes(cls, data: Union[bytearray, bytes]) -> "SpectrogramDataPackage":
+        if len(data) != cls._raw_len:
+            raise ValueError(f"Expected spectrogram data to have len={cls._raw_len}, got len={len(data)}", data)
+
+        return cls(
+            data=[x for x in unpack_from(cls._data_format_str, data, 0)],
+            timestamp_us=unpack_from("<Q", data, cls._data_len)[0],
+        )
+
+    def _channel_slice(self, index) -> list:
+        start = index * self._num_bins_per_channel
+        s = slice(start, start + self._num_bins_per_channel, None)
+        return self.data[s]
+
+    def as_dict(self) -> dict:
+        # This is (and should be) equivalent to `asdict(self)`, but is about 20-30x faster since it doesn't have
+        # to recursively expand all dataclass fields
+        return {
+            "acc_x": self._channel_slice(0),
+            "acc_y": self._channel_slice(1),
+            "acc_z": self._channel_slice(2),
+            "gyro_x": self._channel_slice(3),
+            "gyro_y": self._channel_slice(4),
+            "gyro_z": self._channel_slice(5),
+            "timestamp_us": self.timestamp_us,
+        }
+
+
 def flatten_nested_dataclass_fields(d: Union[Field, type], name: Optional[str]) -> list:
     """Analogous to `flatten_nested_dicts`, but returns the key names and works on the static class, not an instance
 
     Args:
         d: A dataclass e.g. `DataPackage`
         name: The prefix to this level, or more specifically, the key for the next higher level. If `None`, no prefix
               is used
@@ -242,13 +325,20 @@
     q = PackageMetadata.from_raw_bytes(raw_bytes)
     raw_bytes_data = PackageMetadata.split_out_data_from_metadata(raw_bytes)
 
     if q.is_data():
         package = DataPackage.from_raw_bytes(raw_bytes_data)
     elif q.is_button():
         package = ButtonEvent.from_raw_bytes(raw_bytes_data)
+    elif q.is_device_info():
+        package = DeviceInfo.from_raw_bytes(raw_bytes_data)
     elif q.is_raw_gyro_accel():
         package = RawDataPackage.from_raw_bytes(raw_bytes_data)
+    elif q.is_spectrogram():
+        package = SpectrogramDataPackage.from_raw_bytes(raw_bytes_data)
     else:
         raise ValueError(f"Unknown value for q.id={q.id}")
 
     return package
+
+
+Package = Union[DataPackage, RawDataPackage, SpectrogramDataPackage]
```

### Comparing `genki-wave-0.4.1/genki_wave/data/points.py` & `genki-wave-0.5.1/genki_wave/data/points.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/genki_wave/data/structures.py` & `genki-wave-0.5.1/genki_wave/data/structures.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/genki_wave/data/writing.py` & `genki-wave-0.5.1/genki_wave/data/writing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import struct
 
 from cobs import cobs
 
 from genki_wave.data.organization import PackageMetadata
-from genki_wave.data.enums import DeviceMode, PackageId, PackageType
+from genki_wave.data.enums import DeviceMode, PackageId, PackageType, DatastreamType
 
 
 def pad_with_zero_byte(b: bytes) -> bytes:
     return b + struct.pack("<B", 0)
 
 
-def create_package_to_write(p: PackageMetadata, data: bytes) -> bytes:
+def create_package_to_write(p: PackageMetadata, data: bytes = bytearray()) -> bytes:
     """Package the data in the correct format before sending it to a Wave ring"""
     # TODO(robert): `data` should probably be a class that has a `to_bytes` method
     if p.payload_size != len(data):
         raise ValueError(
             f"Expected payload_size and the size of the data to match. Got {p.payload_size} and {len(data)}"
         )
     b_tot = p.to_bytes() + data
@@ -25,7 +25,28 @@
 
 def get_start_api_package():
     """Get the package that puts the Wave ring into 'API mode' when it's sent to the device"""
     return create_package_to_write(
         PackageMetadata(type=PackageType.REQUEST, id=PackageId.DEVICE_MODE, payload_size=1),
         struct.pack("<B", DeviceMode.API.value),
     )
+
+
+def get_start_spectrogram_package():
+    """"""
+    return create_package_to_write(
+        PackageMetadata(type=PackageType.REQUEST, id=PackageId.MODIFY_API_CONFIG, payload_size=8),
+        struct.pack("<BBxxf", DatastreamType.NONE.value, True, 2000.0),
+    )
+
+
+def get_default_api_config_package():
+    """"""
+    return create_package_to_write(
+        PackageMetadata(type=PackageType.REQUEST, id=PackageId.MODIFY_API_CONFIG, payload_size=8),
+        struct.pack("<BBxxf", DatastreamType.MOTION_DATA.value, False, 400.0),
+    )
+
+
+def get_device_info_request():
+    """Get the package that requests device info when it's sent to the device"""
+    return create_package_to_write(PackageMetadata(type=PackageType.REQUEST, id=PackageId.DEVICE_INFO, payload_size=0))
```

### Comparing `genki-wave-0.4.1/genki_wave/discover.py` & `genki-wave-0.5.1/genki_wave/discover.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/genki_wave/protocols.py` & `genki-wave-0.5.1/genki_wave/protocols.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cobs import cobs
 from serial.threaded import Packetizer
 
 from genki_wave.constants import API_CHAR_UUID
 from genki_wave.data import ButtonAction, ButtonEvent, ButtonId, DataPackage
 from genki_wave.data.organization import process_byte_data
 from genki_wave.data.structures import QueueWithPop
-from genki_wave.data.writing import get_start_api_package
+from genki_wave.data.writing import get_start_api_package, get_start_spectrogram_package, get_default_api_config_package
 from genki_wave.utils import get_or_create_event_loop
 
 logger = logging.getLogger(__name__)
 
 
 class CommunicateCancel:
     """
@@ -27,17 +27,19 @@
 
     cancel = False
     is_connected = False
 
     @staticmethod
     def is_cancel(button_event: Union[ButtonEvent, DataPackage]) -> bool:
         """Checks for a hard coded cancel event"""
-        if isinstance(button_event, DataPackage):
-            return False
-        return button_event.button_id == ButtonId.TOP and button_event.action == ButtonAction.EXTRALONG
+        return (
+            isinstance(button_event, ButtonEvent)
+            and button_event.button_id == ButtonId.TOP  # noqa: W503
+            and button_event.action == ButtonAction.EXTRALONG  # noqa: W503
+        )
 
 
 class ProtocolAbc(abc.ABC):
     """A protocol decodes raw data and connects producers and consumers af data from the input device
 
     It's a common abstraction that might be slightly abused here.
 
@@ -138,22 +140,29 @@
     async def _inner(sender: str, data: bytearray) -> None:
         # NOTE: `bleak` expects a function with this signature
         await protocol.data_received(data)
 
     return _inner
 
 
-async def bluetooth_task(ble_address: str, comm: CommunicateCancel, callbacks: List[Callable]) -> None:
+async def bluetooth_task(
+    ble_address: str, comm: CommunicateCancel, callbacks: List[Callable], enable_spectrogram=False
+) -> None:
     protocol = ProtocolAsyncio()
     callback = prepare_protocol_as_bleak_callback_asyncio(protocol)
     print(f"Connecting to wave at address {ble_address}")
     async with BleakClient(ble_address) as client:
         await client.start_notify(API_CHAR_UUID, callback)
         await client.write_gatt_char(API_CHAR_UUID, get_start_api_package(), False)
 
+        if enable_spectrogram:
+            await client.write_gatt_char(API_CHAR_UUID, get_start_spectrogram_package(), False)
+        else:
+            await client.write_gatt_char(API_CHAR_UUID, get_default_api_config_package(), False)
+
         print("Connected to Wave")
         comm.is_connected = True
         while True:
             package = await protocol.queue.get()
 
             if comm.is_cancel(package) or comm.cancel:
                 print("Got a cancel message, exiting.")
```

### Comparing `genki-wave-0.4.1/genki_wave/threading_runner.py` & `genki-wave-0.5.1/genki_wave/threading_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,22 +98,23 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Leave context: close port"""
         self.close()
 
 
 class WaveListener(threading.Thread):
-    def __init__(self, ble_address, callbacks):
+    def __init__(self, ble_address, callbacks, enable_spectrogram=False):
         self.ble_address = ble_address
         self.callbacks = callbacks
+        self.enable_spectrogram = enable_spectrogram
         super().__init__()
 
     def run(self):
         self.comm = CommunicateCancel()
-        task = bluetooth_task(self.ble_address, self.comm, self.callbacks)
+        task = bluetooth_task(self.ble_address, self.comm, self.callbacks, self.enable_spectrogram)
         loop = get_or_create_event_loop()
         loop.run_until_complete(task)
 
     def stop(self):
         self.comm.cancel = True
 
     def __enter__(self):
```

### Comparing `genki-wave-0.4.1/genki_wave/utils.py` & `genki-wave-0.5.1/genki_wave/utils.py`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/genki_wave.egg-info/PKG-INFO` & `genki-wave-0.5.1/genki_wave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: genki-wave
-Version: 0.4.1
+Version: 0.5.1
 Summary: Python API for Wave by Genki
 Home-page: https://github.com/genkiinstruments/genki-wave
 Author: Robert Torfason
 Author-email: robert@genkiinstruments.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
@@ -83,9 +82,7 @@
   connected to the computer. After pairing Wave to a Linux machine Wave tends to connect automatically quite
   aggressively and cannot be accessed via bleak. One solution is to use `bluetoothctl` to disconnect before pairing
   with `genki-wave`.
 * Wave needs to be off and disconnected before receiving any data via the serial port.
 * There is an error when you have Wave connected via Bluetooth and use `asyncio` to receive data.
   If you kill the program, e.g., with a keyboard interrupt, Wave stays connected and has an invalid state.
   For the time being you can hold the top button for a few seconds to properly exit the program.
-
-
```

### Comparing `genki-wave-0.4.1/genki_wave.egg-info/SOURCES.txt` & `genki-wave-0.5.1/genki_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genki-wave-0.4.1/setup.py` & `genki-wave-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md") as f:
     readme = f.read()
 
 requires = ["bleak", "cobs", "pyserial", "pyserial-asyncio"]
 
 setup(
     name="genki-wave",
-    version="0.4.1",
+    version="0.5.1",
     description="Python API for Wave by Genki",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Robert Torfason",
     author_email="robert@genkiinstruments.com",
     url="https://github.com/genkiinstruments/genki-wave",
     license="MIT",
```

