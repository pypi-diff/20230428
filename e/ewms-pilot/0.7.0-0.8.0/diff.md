# Comparing `tmp/ewms-pilot-0.7.0.tar.gz` & `tmp/ewms-pilot-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewms-pilot-0.7.0.tar", last modified: Fri Apr 28 19:47:02 2023, max compression
+gzip compressed data, was "ewms-pilot-0.8.0.tar", last modified: Fri Apr 28 20:17:10 2023, max compression
```

## Comparing `ewms-pilot-0.7.0.tar` & `ewms-pilot-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.838867 ewms-pilot-0.7.0/ewms_pilot/
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 19:47:00.000000 ewms-pilot-0.7.0/ewms_pilot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/config.py
--rw-r--r--   0 root         (0) root         (0)    15500 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/pilot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/ewms_pilot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/ewms_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 19:47:02.000000 ewms-pilot-0.7.0/ewms_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 19:47:02.842867 ewms-pilot-0.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 19:46:59.000000 ewms-pilot-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/ewms_pilot/
+-rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/config.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/pilot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/ewms_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/setup.py
```

### Comparing `ewms-pilot-0.7.0/LICENSE` & `ewms-pilot-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.7.0/PKG-INFO` & `ewms-pilot-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.7.0
+Version: 0.8.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.7.0/README.md` & `ewms-pilot-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.7.0/ewms_pilot/__init__.py` & `ewms-pilot-0.8.0/ewms_pilot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 from .pilot import consume_and_reply, main
 
 __all__ = ["consume_and_reply"]
 
 # version is a human-readable version number.
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 version_info = (
```

### Comparing `ewms-pilot-0.7.0/ewms_pilot/pilot.py` & `ewms-pilot-0.8.0/ewms_pilot/pilot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """API for launching an MQ-task pilot."""
 
 
 import argparse
 import asyncio
 import enum
 import json
-import logging
 import pickle
 import shlex
 import shutil
 import subprocess
 import time
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 import mqclient as mq
 from wipac_dev_tools import argparse_tools, logging_tools
 
-from .config import ENV
-
-LOGGER = logging.getLogger("ewms-pilot")
+from .config import ENV, LOGGER
 
 # if there's an error, have the cluster try again (probably a system error)
 _EXCEPT_ERRORS = False
 
 _DEFAULT_TIMEOUT_INCOMING = 1  # second
 _DEFAULT_TIMEOUT_OUTGOING = 1  # second
 _DEFAULT_PREFETCH = 1
@@ -143,15 +140,15 @@
 
     return out_msg
 
 
 def process_msg(
     in_msg: Any,
     cmd: str,
-    subproc_timeout: Optional[int],
+    task_timeout: Optional[int],
     fpath_to_subproc: Path,
     fpath_from_subproc: Path,
     file_writer: Callable[[Any, Path], None],
     file_reader: Callable[[Path], Any],
     debug_dir: Optional[Path],
 ) -> Any:
     """Process the message in a subprocess using `cmd`."""
@@ -166,15 +163,15 @@
 
     # call & check outputs
     LOGGER.info(f"Executing: {shlex.split(cmd)}")
     try:
         subprocess.run(
             shlex.split(cmd),
             check=True,
-            timeout=subproc_timeout,
+            timeout=task_timeout,
         )
     except Exception as e:
         LOGGER.error(f"Subprocess failed: {e}")  # log the time
         raise
 
     # get
     out_msg = read_from_subproc(fpath_from_subproc, debug_subdir, file_reader)
@@ -203,15 +200,15 @@
     fpath_from_subproc: Path = Path("./out.pkl"),
     #
     file_writer: Callable[[Any, Path], None] = UniversalFileInterface.write,
     file_reader: Callable[[Path], Any] = UniversalFileInterface.read,
     #
     debug_dir: Optional[Path] = None,
     #
-    subproc_timeout: Optional[int] = ENV.EWMS_PILOT_SUBPROC_TIMEOUT,
+    task_timeout: Optional[int] = ENV.EWMS_PILOT_TASK_TIMEOUT,
     quarantine_time: int = ENV.EWMS_PILOT_QUARANTINE_TIME,
 ) -> None:
     """Communicate with server and outsource processing to subprocesses.
 
     Arguments:
         `timeout_wait_for_first_message`: if None, use 'timeout_incoming'
     """
@@ -233,15 +230,15 @@
             timeout_incoming,
             timeout_outgoing,
             fpath_to_subproc,
             fpath_from_subproc,
             file_writer,
             file_reader,
             debug_dir,
-            subproc_timeout,
+            task_timeout,
         )
     except Exception as e:
         if quarantine_time:
             LOGGER.error(f"{e} (Quarantining for {quarantine_time} seconds)")
             await asyncio.sleep(quarantine_time)
         raise
 
@@ -268,20 +265,20 @@
     fpath_from_subproc: Path,
     #
     file_writer: Callable[[Any, Path], None],
     file_reader: Callable[[Path], Any],
     #
     debug_dir: Optional[Path],
     #
-    subproc_timeout: Optional[int],
+    task_timeout: Optional[int],
 ) -> None:
     """Consume and reply loop."""
     ack_timeout = None
-    if subproc_timeout:
-        ack_timeout = subproc_timeout + _ACK_TIMEOUT_NONSUBPROC_OVERHEAD_TIME
+    if task_timeout:
+        ack_timeout = task_timeout + _ACK_TIMEOUT_NONSUBPROC_OVERHEAD_TIME
 
     in_queue = mq.Queue(
         broker_client,
         address=broker_address,
         name=queue_incoming,
         prefetch=prefetch,
         auth_token=auth_token,
@@ -311,15 +308,15 @@
         )
         async with in_queue.open_sub_one() as in_msg:
             total_msg_count += 1
             LOGGER.info(f"Got a message to process (#{total_msg_count}): {in_msg}")
             out_msg = process_msg(
                 in_msg,
                 cmd,
-                subproc_timeout,
+                task_timeout,
                 fpath_to_subproc,
                 fpath_from_subproc,
                 file_writer,
                 file_reader,
                 debug_dir,
             )
             # send
@@ -331,15 +328,15 @@
         async with in_queue.open_sub() as sub:
             async for in_msg in sub:
                 total_msg_count += 1
                 LOGGER.info(f"Got a message to process (#{total_msg_count}): {in_msg}")
                 out_msg = process_msg(
                     in_msg,
                     cmd,
-                    subproc_timeout,
+                    task_timeout,
                     fpath_to_subproc,
                     fpath_from_subproc,
                     file_writer,
                     file_reader,
                     debug_dir,
                 )
                 # send
@@ -422,34 +419,34 @@
         type=int,
         help="prefetch for incoming messages",
     )
     parser.add_argument(
         "--timeout-wait-for-first-message",
         default=None,
         type=int,
-        help="timeout (seconds) for the first message to arrive at the client(s); "
+        help="timeout (seconds) for the first message to arrive at the pilot; "
         "defaults to `--timeout-incoming` value",
     )
     parser.add_argument(
         "--timeout-incoming",
         default=_DEFAULT_TIMEOUT_INCOMING,
         type=int,
-        help="timeout (seconds) for messages TO client(s)",
+        help="timeout (seconds) for messages TO pilot",
     )
     parser.add_argument(
         "--timeout-outgoing",
         default=_DEFAULT_TIMEOUT_OUTGOING,
         type=int,
-        help="timeout (seconds) for messages FROM client(s)",
+        help="timeout (seconds) for messages FROM pilot",
     )
     parser.add_argument(
-        "--subproc-timeout",
-        default=ENV.EWMS_PILOT_SUBPROC_TIMEOUT,
+        "--task-timeout",
+        default=ENV.EWMS_PILOT_TASK_TIMEOUT,
         type=int,
-        help="timeout (seconds) for each subprocess",
+        help="timeout (seconds) for each task",
     )
     parser.add_argument(
         "--quarantine-time",
         default=ENV.EWMS_PILOT_QUARANTINE_TIME,
         type=int,
         help="amount of time to sleep after error (useful for preventing blackhole scenarios on condor)",
     )
@@ -502,15 +499,15 @@
             timeout_incoming=args.timeout_incoming,
             timeout_outgoing=args.timeout_outgoing,
             fpath_to_subproc=args.infile,
             fpath_from_subproc=args.outfile,
             # file_writer=UniversalFileInterface.write,
             # file_reader=UniversalFileInterface.read,
             debug_dir=args.debug_directory,
-            subproc_timeout=args.subproc_timeout,
+            task_timeout=args.task_timeout,
             quarantine_time=args.quarantine_time,
         )
     )
     LOGGER.info("Done.")
 
 
 if __name__ == "__main__":
```

### Comparing `ewms-pilot-0.7.0/ewms_pilot.egg-info/PKG-INFO` & `ewms-pilot-0.8.0/ewms_pilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.7.0
+Version: 0.8.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.7.0/setup.cfg` & `ewms-pilot-0.8.0/setup.cfg`

 * *Files identical despite different names*

