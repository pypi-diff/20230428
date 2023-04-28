# Comparing `tmp/ewms-pilot-0.8.0.tar.gz` & `tmp/ewms-pilot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewms-pilot-0.8.0.tar", last modified: Fri Apr 28 20:17:10 2023, max compression
+gzip compressed data, was "ewms-pilot-0.9.0.tar", last modified: Fri Apr 28 21:12:54 2023, max compression
```

## Comparing `ewms-pilot-0.8.0.tar` & `ewms-pilot-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/ewms_pilot/
--rw-r--r--   0 root         (0) root         (0)      650 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/config.py
--rw-r--r--   0 root         (0) root         (0)    15391 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/pilot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/ewms_pilot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/ewms_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 20:17:10.000000 ewms-pilot-0.8.0/ewms_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 20:17:10.576128 ewms-pilot-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 20:17:07.000000 ewms-pilot-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/ewms_pilot/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-04-28 21:12:51.000000 ewms-pilot-0.9.0/ewms_pilot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/config.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/pilot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/ewms_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/setup.py
```

### Comparing `ewms-pilot-0.8.0/LICENSE` & `ewms-pilot-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.8.0/PKG-INFO` & `ewms-pilot-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.8.0
+Version: 0.9.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.8.0/README.md` & `ewms-pilot-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.8.0/ewms_pilot/__init__.py` & `ewms-pilot-0.9.0/ewms_pilot/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Init."""
 
 
-from .pilot import consume_and_reply, main
+from .pilot import FileType, consume_and_reply, main
 
-__all__ = ["consume_and_reply"]
+__all__ = [
+    "consume_and_reply",
+    "FileType",
+]
 
 # version is a human-readable version number.
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 version_info = (
```

### Comparing `ewms-pilot-0.8.0/ewms_pilot/config.py` & `ewms-pilot-0.9.0/ewms_pilot/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     # logging
     EWMS_PILOT_LOG: str = "INFO"
     EWMS_PILOT_LOG_THIRD_PARTY: str = "WARNING"
 
     # meta
     EWMS_PILOT_TASK_TIMEOUT: Optional[int] = None
     EWMS_PILOT_QUARANTINE_TIME: int = 0  # seconds
+    EWMS_PILOT_CONCURRENT_TASKS: int = 1
 
     def __post_init__(self) -> None:
         if timeout := os.getenv("EWMS_PILOT_SUBPROC_TIMEOUT"):
             LOGGER.warning(
                 "Using 'EWMS_PILOT_SUBPROC_TIMEOUT'; 'EWMS_PILOT_TASK_TIMEOUT' is preferred."
             )
             if self.EWMS_PILOT_TASK_TIMEOUT is not None:
```

### Comparing `ewms-pilot-0.8.0/ewms_pilot/pilot.py` & `ewms-pilot-0.9.0/ewms_pilot/pilot.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,63 +4,84 @@
 import argparse
 import asyncio
 import enum
 import json
 import pickle
 import shlex
 import shutil
-import subprocess
-import time
+import uuid
 from pathlib import Path
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import mqclient as mq
+from mqclient.broker_client_interface import Message
 from wipac_dev_tools import argparse_tools, logging_tools
 
 from .config import ENV, LOGGER
 
+AsyncioTaskMessages = Dict[asyncio.Task, Message]  # type: ignore[type-arg]
+
+
 # if there's an error, have the cluster try again (probably a system error)
 _EXCEPT_ERRORS = False
 
 _DEFAULT_TIMEOUT_INCOMING = 1  # second
 _DEFAULT_TIMEOUT_OUTGOING = 1  # second
 _DEFAULT_PREFETCH = 1
 
 # addl time to add to `mq.Queue.ack_timeout` for non-subproc activities
 _ACK_TIMEOUT_NONSUBPROC_OVERHEAD_TIME = 10  # second  # this is more than enough
 
 
 class FileType(enum.Enum):
     """Various file types/extensions."""
 
-    PICKLE = ".pkl"
-    PLAIN_TEXT = ".txt"
+    PKL = ".pkl"
+    TXT = ".txt"
     JSON = ".json"
 
 
+class TaskSubprocessError(Exception):
+    """Raised when the subprocess terminates in an error."""
+
+    def __init__(
+        self,
+        return_code: int,
+        debug_subdir: Optional[Path],
+    ):
+        super().__init__(
+            f"Subprocess completed with exit code {return_code} "
+            f"(debug directory: {debug_subdir})"
+        )
+
+
+def _task_exception_str(task: asyncio.Task) -> str:
+    return f'{type(task.exception()).__name__}: "{task.exception()}"'
+
+
 class UniversalFileInterface:
     """Support reading and writing for any `FileType` file extension."""
 
     @classmethod
     def write(cls, in_msg: Any, fpath: Path) -> None:
         """Write `stuff` to `fpath` per `fpath.suffix`."""
         cls._write(in_msg, fpath)
         LOGGER.info(f"File Written :: {fpath} ({fpath.stat().st_size} bytes)")
 
     @classmethod
     def _write(cls, in_msg: Any, fpath: Path) -> None:
-        LOGGER.info(f"Writing payload to file @ {fpath}")
+        LOGGER.info(f"Writing to file: {fpath}")
         LOGGER.debug(in_msg)
 
-        # PICKLE
-        if fpath.suffix == FileType.PICKLE.value:
+        # PKL
+        if fpath.suffix == FileType.PKL.value:
             with open(fpath, "wb") as f:
                 pickle.dump(in_msg, f)
-        # PLAIN_TEXT
-        elif fpath.suffix == FileType.PLAIN_TEXT.value:
+        # TXT
+        elif fpath.suffix == FileType.TXT.value:
             with open(fpath, "w") as f:
                 f.write(in_msg)
         # JSON
         elif fpath.suffix == FileType.JSON.value:
             with open(fpath, "w") as f:
                 json.dump(in_msg, f)
         # ???
@@ -73,22 +94,22 @@
         msg = cls._read(fpath)
         LOGGER.info(f"File Read :: {fpath} ({fpath.stat().st_size} bytes)")
         LOGGER.debug(msg)
         return msg
 
     @classmethod
     def _read(cls, fpath: Path) -> Any:
-        LOGGER.info(f"Reading payload from file @ {fpath}")
+        LOGGER.info(f"Reading from file: {fpath}")
 
-        # PICKLE
-        if fpath.suffix == FileType.PICKLE.value:
+        # PKL
+        if fpath.suffix == FileType.PKL.value:
             with open(fpath, "rb") as f:
                 return pickle.load(f)
-        # PLAIN_TEXT
-        elif fpath.suffix == FileType.PLAIN_TEXT.value:
+        # TXT
+        elif fpath.suffix == FileType.TXT.value:
             with open(fpath, "r") as f:
                 return f.read()
         # JSON
         elif fpath.suffix == FileType.JSON.value:
             with open(fpath, "r") as f:
                 return json.load(f)
         # ???
@@ -111,246 +132,357 @@
     # persist the file?
     if debug_subdir:
         file_writer(in_msg, debug_subdir / fpath_to_subproc.name)
 
     return fpath_to_subproc
 
 
+def mv_or_rm_file(src: Path, dest: Optional[Path]) -> None:
+    """Move the file to `dest` if not None, else rm it.
+
+    No error if file doesn't exist.
+    """
+    if not src.exists():
+        return
+    if dest:
+        # src.rename(dest / src.name)  # mv
+        # NOTE: https://github.com/python/cpython/pull/30650
+        shutil.move(src, dest / src.name)
+    else:
+        src.unlink()  # rm
+
+
 def read_from_subproc(
     fpath_from_subproc: Path,
     debug_subdir: Optional[Path],
     file_reader: Callable[[Path], Any],
 ) -> Any:
     """Read the msg from the `OUT` file.
 
     Also, dump to a file for debugging (if not "").
     """
     if not fpath_from_subproc.exists():
-        LOGGER.error("Out file was not written for in-payload")
-        raise RuntimeError("Out file was not written for in-payload")
+        msg = "Out-file cannot be found"
+        LOGGER.error(msg)
+        raise FileNotFoundError(msg)
 
     out_msg = file_reader(fpath_from_subproc)
 
-    # persist the file?
-    if debug_subdir:
-        # fpath_from_subproc.rename(debug_subdir / fpath_from_subproc.name)  # mv
-        # NOTE: https://github.com/python/cpython/pull/30650
-        shutil.move(fpath_from_subproc, debug_subdir / fpath_from_subproc.name)
-    else:
-        fpath_from_subproc.unlink()  # rm
+    mv_or_rm_file(fpath_from_subproc, debug_subdir)
 
     return out_msg
 
 
-def process_msg(
+async def process_msg_task(
     in_msg: Any,
     cmd: str,
     task_timeout: Optional[int],
-    fpath_to_subproc: Path,
-    fpath_from_subproc: Path,
+    #
+    ftype_to_subproc: FileType,
+    ftype_from_subproc: FileType,
+    #
     file_writer: Callable[[Any, Path], None],
     file_reader: Callable[[Path], Any],
+    #
     debug_dir: Optional[Path],
+    pub: mq.queue.QueuePubResource,
 ) -> Any:
-    """Process the message in a subprocess using `cmd`."""
+    """Process the message's task in a subprocess using `cmd` & respond."""
+    task_id = uuid.uuid4().hex
+
     # debugging logic
     debug_subdir = None
     if debug_dir:
-        debug_subdir = debug_dir / str(time.time())
+        debug_subdir = debug_dir / task_id
         debug_subdir.mkdir(parents=True, exist_ok=False)
 
+    # create in/out filepaths
+    fpath_to_subproc = Path(f"in-{task_id}{ftype_to_subproc.value}")
+    fpath_from_subproc = Path(f"out-{task_id}{ftype_from_subproc.value}")
+
+    # insert in/out files into cmd
+    cmd = cmd.replace("{{INFILE}}", str(fpath_to_subproc))
+    cmd = cmd.replace("{{OUTFILE}}", str(fpath_from_subproc))
+
     # write
     write_to_subproc(fpath_to_subproc, in_msg, debug_subdir, file_writer)
 
     # call & check outputs
     LOGGER.info(f"Executing: {shlex.split(cmd)}")
     try:
-        subprocess.run(
-            shlex.split(cmd),
-            check=True,
+
+        # await to start & prep coroutines
+        if debug_subdir:
+            with open(debug_subdir / "stdoutfile", "wb") as stdoutf, open(
+                debug_subdir / "stderrfile", "wb"
+            ) as stderrf:
+                proc = await asyncio.create_subprocess_shell(
+                    cmd,
+                    stdout=stdoutf,
+                    stderr=stderrf,
+                )
+        else:
+            proc = await asyncio.create_subprocess_shell(cmd)
+
+        # await to finish
+        await asyncio.wait_for(  # raises TimeoutError
+            proc.wait(),
             timeout=task_timeout,
         )
+
+        LOGGER.info(f"Subprocess return code: {proc.returncode}")
+
+        # exception handling (immediately re-handled by 'except' below)
+        if proc.returncode:
+            raise TaskSubprocessError(proc.returncode, debug_subdir)
+
+    # Error Case: first, if there's a file move it to debug dir (if enabled)
     except Exception as e:
         LOGGER.error(f"Subprocess failed: {e}")  # log the time
+        mv_or_rm_file(fpath_from_subproc, debug_subdir)
         raise
 
-    # get
+    # Successful Case: get message and move to debug dir
     out_msg = read_from_subproc(fpath_from_subproc, debug_subdir, file_reader)
-    return out_msg
+
+    # send
+    LOGGER.info("Sending return message...")
+    await pub.send(out_msg)
 
 
 async def consume_and_reply(
     cmd: str,
     #
     queue_incoming: str,
     queue_outgoing: str,
     #
+    # for subprocess
+    ftype_to_subproc: Union[str, FileType],
+    ftype_from_subproc: Union[str, FileType],
+    #
     # for mq
     broker_client: str = ENV.EWMS_PILOT_BROKER_CLIENT,
     broker_address: str = ENV.EWMS_PILOT_BROKER_ADDRESS,
     auth_token: str = ENV.EWMS_PILOT_BROKER_AUTH_TOKEN,
     #
     prefetch: int = _DEFAULT_PREFETCH,
     #
     timeout_wait_for_first_message: Optional[int] = None,
     timeout_incoming: int = _DEFAULT_TIMEOUT_INCOMING,
     timeout_outgoing: int = _DEFAULT_TIMEOUT_OUTGOING,
     #
-    # for subprocess
-    fpath_to_subproc: Path = Path("./in.pkl"),
-    fpath_from_subproc: Path = Path("./out.pkl"),
-    #
     file_writer: Callable[[Any, Path], None] = UniversalFileInterface.write,
     file_reader: Callable[[Path], Any] = UniversalFileInterface.read,
     #
     debug_dir: Optional[Path] = None,
     #
     task_timeout: Optional[int] = ENV.EWMS_PILOT_TASK_TIMEOUT,
     quarantine_time: int = ENV.EWMS_PILOT_QUARANTINE_TIME,
+    #
+    multitasking: int = ENV.EWMS_PILOT_CONCURRENT_TASKS,
 ) -> None:
     """Communicate with server and outsource processing to subprocesses.
 
     Arguments:
         `timeout_wait_for_first_message`: if None, use 'timeout_incoming'
     """
     LOGGER.info("Making MQClient queue connections...")
 
     if not queue_incoming or not queue_outgoing:
         raise RuntimeError("Must define an incoming and an outgoing queue")
 
+    ack_timeout = None
+    if task_timeout:
+        ack_timeout = task_timeout + _ACK_TIMEOUT_NONSUBPROC_OVERHEAD_TIME
+
+    if not isinstance(ftype_to_subproc, FileType):
+        ftype_to_subproc = FileType(ftype_to_subproc)
+    if not isinstance(ftype_from_subproc, FileType):
+        ftype_from_subproc = FileType(ftype_from_subproc)
+
+    in_queue = mq.Queue(
+        broker_client,
+        address=broker_address,
+        name=queue_incoming,
+        prefetch=prefetch,
+        auth_token=auth_token,
+        except_errors=_EXCEPT_ERRORS,
+        # timeout=timeout_incoming, # manually set below
+        ack_timeout=ack_timeout,
+    )
+    out_queue = mq.Queue(
+        broker_client,
+        address=broker_address,
+        name=queue_outgoing,
+        auth_token=auth_token,
+        except_errors=_EXCEPT_ERRORS,
+        timeout=timeout_outgoing,
+        ack_timeout=ack_timeout,
+    )
+
     try:
         await _consume_and_reply(
             cmd,
-            queue_incoming,
-            queue_outgoing,
-            broker_client,
-            broker_address,
-            auth_token,
-            prefetch,
+            in_queue,
+            out_queue,
+            ftype_to_subproc,
+            ftype_from_subproc,
+            #
             timeout_wait_for_first_message,
             timeout_incoming,
-            timeout_outgoing,
-            fpath_to_subproc,
-            fpath_from_subproc,
             file_writer,
             file_reader,
             debug_dir,
             task_timeout,
+            multitasking,
         )
     except Exception as e:
         if quarantine_time:
             LOGGER.error(f"{e} (Quarantining for {quarantine_time} seconds)")
             await asyncio.sleep(quarantine_time)
         raise
 
 
+async def _ack_nack_finished_tasks(
+    sub: mq.queue.ManualQueueSubResource,
+    tasks: AsyncioTaskMessages,
+    return_when: str,
+    previous_failed: AsyncioTaskMessages,
+) -> Tuple[AsyncioTaskMessages, AsyncioTaskMessages]:
+    """Get finished tasks and ack/nack their messages.
+
+    Returns:
+        Tuple:
+            AsyncioTaskMessages: pending tasks and
+            AsyncioTaskMessages: failed tasks (plus those in `previous_failed`)
+    """
+    done, pending = await asyncio.wait(tasks.keys(), return_when=return_when)
+    LOGGER.info(f"{len(done)} Tasks Finished")
+
+    for task in done:
+        if task.exception():
+            await sub.nack(tasks[task])
+            previous_failed[task] = tasks[task]
+            LOGGER.error("Task failed:")
+            LOGGER.error(_task_exception_str(task))
+        else:
+            await sub.ack(tasks[task])
+
+    return (
+        {t: tasks[t] for t in pending},
+        previous_failed,
+    )
+
+
 async def _consume_and_reply(
     cmd: str,
     #
-    queue_incoming: str,
-    queue_outgoing: str,
-    #
-    # for mq
-    broker_client: str,
-    broker_address: str,
-    auth_token: str,
+    in_queue: mq.Queue,
+    out_queue: mq.Queue,
     #
-    prefetch: int,
+    # for subprocess
+    ftype_to_subproc: FileType,
+    ftype_from_subproc: FileType,
     #
     timeout_wait_for_first_message: Optional[int],
     timeout_incoming: int,
-    timeout_outgoing: int,
-    #
-    # for subprocess
-    fpath_to_subproc: Path,
-    fpath_from_subproc: Path,
     #
     file_writer: Callable[[Any, Path], None],
     file_reader: Callable[[Path], Any],
     #
     debug_dir: Optional[Path],
     #
     task_timeout: Optional[int],
-) -> None:
-    """Consume and reply loop."""
-    ack_timeout = None
-    if task_timeout:
-        ack_timeout = task_timeout + _ACK_TIMEOUT_NONSUBPROC_OVERHEAD_TIME
+    multitasking: int,
+) -> int:
+    """Consume and reply loop.
 
-    in_queue = mq.Queue(
-        broker_client,
-        address=broker_address,
-        name=queue_incoming,
-        prefetch=prefetch,
-        auth_token=auth_token,
-        except_errors=_EXCEPT_ERRORS,
-        # timeout=timeout_incoming, # manually set below
-        ack_timeout=ack_timeout,
-    )
-    out_queue = mq.Queue(
-        broker_client,
-        address=broker_address,
-        name=queue_outgoing,
-        auth_token=auth_token,
-        except_errors=_EXCEPT_ERRORS,
-        timeout=timeout_outgoing,
-        ack_timeout=ack_timeout,
+    Return number of processed tasks.
+    """
+    pending: AsyncioTaskMessages = {}
+    failed: AsyncioTaskMessages = {}
+
+    # for the first (set) of messages, use 'timeout_wait_for_first_message' if given
+    in_queue.timeout = (
+        timeout_wait_for_first_message
+        if timeout_wait_for_first_message
+        else timeout_incoming
     )
 
+    # GO!
     total_msg_count = 0
-    LOGGER.info("Getting messages from server to process then send back...")
+    LOGGER.info(
+        "Listening for messages from server to process tasks then send results..."
+    )
     async with out_queue.open_pub() as pub:
 
-        # FIRST MESSAGE
-        in_queue.timeout = (
-            timeout_wait_for_first_message
-            if timeout_wait_for_first_message
-            else timeout_incoming
-        )
-        async with in_queue.open_sub_one() as in_msg:
-            total_msg_count += 1
-            LOGGER.info(f"Got a message to process (#{total_msg_count}): {in_msg}")
-            out_msg = process_msg(
-                in_msg,
-                cmd,
-                task_timeout,
-                fpath_to_subproc,
-                fpath_from_subproc,
-                file_writer,
-                file_reader,
-                debug_dir,
-            )
-            # send
-            LOGGER.info("Sending out-payload to server...")
-            await pub.send(out_msg)
-
-        # ADDITIONAL MESSAGES
-        in_queue.timeout = timeout_incoming
-        async with in_queue.open_sub() as sub:
-            async for in_msg in sub:
+        LOGGER.info(f"Processing up to {multitasking} tasks concurrently")
+        async with in_queue.open_sub_manual_acking(multitasking) as sub:
+
+            async for in_msg in sub.iter_messages():
                 total_msg_count += 1
-                LOGGER.info(f"Got a message to process (#{total_msg_count}): {in_msg}")
-                out_msg = process_msg(
-                    in_msg,
-                    cmd,
-                    task_timeout,
-                    fpath_to_subproc,
-                    fpath_from_subproc,
-                    file_writer,
-                    file_reader,
-                    debug_dir,
+                LOGGER.info(f"Got a task to process (#{total_msg_count}): {in_msg}")
+                task = asyncio.create_task(
+                    process_msg_task(
+                        in_msg.data,
+                        cmd,
+                        task_timeout,
+                        ftype_to_subproc,
+                        ftype_from_subproc,
+                        file_writer,
+                        file_reader,
+                        debug_dir,
+                        pub,
+                    )
+                )
+                pending[task] = in_msg
+
+                # if we've met max concurrent tasks, wait for the next one to finish
+                while len(pending) >= multitasking:
+                    LOGGER.info("Reached max task concurrency limit, waiting...")
+                    pending, failed = await _ack_nack_finished_tasks(
+                        sub,
+                        pending,
+                        return_when=asyncio.FIRST_COMPLETED,
+                        previous_failed=failed,
+                    )
+                    # after the first set of messages, set the timeout to the "normal" amount
+                    if in_queue.timeout != timeout_incoming:
+                        in_queue.timeout = timeout_incoming
+
+                # if 1+ fail, then don't consume anymore; wait for remaining tasks
+                if failed:
+                    LOGGER.info("1+ Tasks Failed: waiting for remaining tasks")
+                    break
+
+            LOGGER.info("No more new tasks to process")
+
+            # wait for remaining tasks
+            if pending:
+                LOGGER.info("Waiting for remaining tasks to finish...")
+                pending, failed = await _ack_nack_finished_tasks(
+                    sub,
+                    pending,
+                    return_when=asyncio.ALL_COMPLETED,
+                    previous_failed=failed,
                 )
-                # send
-                LOGGER.info("Sending out-payload to server...")
-                await pub.send(out_msg)
+                if pending:
+                    LOGGER.error(f"{len(pending)} tasks are pending after finish")
 
-    # check if anything was actually processed
+    # cleanup
+    if failed:
+        raise RuntimeError(
+            f"{len(failed)} Task(s) Failed: "
+            f"{', '.join(type(f.exception()).__name__ for f in failed)}"
+        )
+    # check if anything actually processed
     if not total_msg_count:
         LOGGER.warning("No Messages Were Received.")
-    LOGGER.info(f"Done Processing: handled {total_msg_count} messages")
+    LOGGER.info(f"Done Processing: completed {total_msg_count} tasks")
+    return total_msg_count
 
 
 def main() -> None:
     """Start up EWMS Pilot subprocess to perform an MQ task."""
 
     parser = argparse.ArgumentParser(
         description="Start up EWMS Pilot subprocess to perform an MQ task",
@@ -359,34 +491,28 @@
     )
     parser.add_argument(
         "--cmd",  # alternatively we can go with a condor-like --executable and --arguments
         required=True,
         help="the command to give the subprocess script",
     )
     parser.add_argument(
-        "--in",
-        dest="infile",
-        default=Path("./in.pkl"),
-        type=lambda x: argparse_tools.validate_arg(
-            Path(x),
-            Path(x).suffix in [e.value for e in FileType],
-            argparse.ArgumentTypeError(f"Unsupported file type: {x}"),
-        ),
-        help="which file to write for the client/pilot's subprocess",
-    )
-    parser.add_argument(
-        "--out",
-        dest="outfile",
-        default=Path("./out.pkl"),
-        type=lambda x: argparse_tools.validate_arg(
-            Path(x),
-            Path(x).suffix in [e.value for e in FileType],
-            argparse.ArgumentTypeError(f"Unsupported file type: {x}"),
-        ),
-        help="which file to read from the client/pilot's subprocess",
+        "--infile-type",
+        type=FileType,
+        help="the file type (extension) to use for files written for the pilot's subprocess",
+    )
+    parser.add_argument(
+        "--outfile-type",
+        type=FileType,
+        help="the file type (exception) of the file to read from the pilot's subprocess",
+    )
+    parser.add_argument(
+        "--multitasking",
+        type=int,
+        default=ENV.EWMS_PILOT_CONCURRENT_TASKS,
+        help="the max number of tasks to process in parallel",
     )
 
     # mq args
     parser.add_argument(
         "--queue-incoming",
         required=True,
         help="the name of the incoming queue",
@@ -486,29 +612,31 @@
     LOGGER.info(
         f"Starting up an EWMS Pilot for MQ task: {args.queue_incoming} -> {args.queue_outgoing}"
     )
     asyncio.run(
         consume_and_reply(
             cmd=args.cmd,
             broker_client=args.broker_client,
+            ftype_to_subproc=args.infile_type,
+            ftype_from_subproc=args.outfile_type,
+            #
             broker_address=args.broker,
             auth_token=args.auth_token,
             queue_incoming=args.queue_incoming,
             queue_outgoing=args.queue_outgoing,
             prefetch=args.prefetch,
             timeout_wait_for_first_message=args.timeout_wait_for_first_message,
             timeout_incoming=args.timeout_incoming,
             timeout_outgoing=args.timeout_outgoing,
-            fpath_to_subproc=args.infile,
-            fpath_from_subproc=args.outfile,
             # file_writer=UniversalFileInterface.write,
             # file_reader=UniversalFileInterface.read,
             debug_dir=args.debug_directory,
             task_timeout=args.task_timeout,
             quarantine_time=args.quarantine_time,
+            multitasking=args.multitasking,
         )
     )
     LOGGER.info("Done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ewms-pilot-0.8.0/ewms_pilot.egg-info/PKG-INFO` & `ewms-pilot-0.9.0/ewms_pilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.8.0
+Version: 0.9.0
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.8.0/setup.cfg` & `ewms-pilot-0.9.0/setup.cfg`

 * *Files identical despite different names*

