# Comparing `tmp/gdb_plus-6.1.0.tar.gz` & `tmp/gdb_plus-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.1.0.tar", last modified: Fri Apr 28 08:19:30 2023, max compression
+gzip compressed data, was "gdb_plus-6.1.1.tar", last modified: Fri Apr 28 13:00:13 2023, max compression
```

## Comparing `gdb_plus-6.1.0.tar` & `gdb_plus-6.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.746626 gdb_plus-6.1.0/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.0/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11492 2023-04-28 08:19:30.745431 gdb_plus-6.1.0/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11251 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.667915 gdb_plus-6.1.0/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11204 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    75285 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.726381 gdb_plus-6.1.0/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11492 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-04-28 08:19:30.747006 gdb_plus-6.1.0/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.728755 gdb_plus-6.1.0/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    17642 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.963025 gdb_plus-6.1.1/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.1/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11478 2023-04-28 13:00:13.961928 gdb_plus-6.1.1/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11238 2023-04-28 10:24:27.000000 gdb_plus-6.1.1/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.913379 gdb_plus-6.1.1/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11017 2023-04-28 08:59:52.000000 gdb_plus-6.1.1/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-04-28 08:06:22.000000 gdb_plus-6.1.1/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    76108 2023-04-28 12:59:02.000000 gdb_plus-6.1.1/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-04-28 08:06:22.000000 gdb_plus-6.1.1/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.942245 gdb_plus-6.1.1/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11478 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-04-28 13:00:13.000000 gdb_plus-6.1.1/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-04-28 09:25:00.000000 gdb_plus-6.1.1/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-04-28 13:00:13.963378 gdb_plus-6.1.1/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 13:00:13.944657 gdb_plus-6.1.1/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    17641 2023-04-28 10:40:32.000000 gdb_plus-6.1.1/tests/test.py
```

### Comparing `gdb_plus-6.1.0/LICENSE` & `gdb_plus-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.0/PKG-INFO` & `gdb_plus-6.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.1.0
+Version: 6.1.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -250,18 +250,19 @@
 
 See [this example](./examples/black_box_analysis_of_function.py) for more details
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
-You may want to debug manually the function called. If this is the case set last address of your function in `call(..., end_pointer= ...)` so that the script continues only once you reach the end of the function and not while you are using gdb
+If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
 ## Alternatives
 from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
 
 # TODO
 
 * Add option to use libdebug instead of gdb
+* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
```

### Comparing `gdb_plus-6.1.0/README.md` & `gdb_plus-6.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -236,18 +236,19 @@
 
 See [this example](./examples/black_box_analysis_of_function.py) for more details
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
-You may want to debug manually the function called. If this is the case set last address of your function in `call(..., end_pointer= ...)` so that the script continues only once you reach the end of the function and not while you are using gdb
+If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
 ## Alternatives
 from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
 
 # TODO
 
 * Add option to use libdebug instead of gdb
+* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
```

### Comparing `gdb_plus-6.1.0/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.1.1/gdb_plus/Inner_Debugger.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,19 +152,17 @@
         self.wait()
         self._restore_breakpoint(ip)
 
     def next(self):
         ip = self.instruction_pointer
         inst = self.next_inst
         if inst.mnemonic == "call":
+            self._disable_breakpoint(ip)
+            self.cont(until=ip + inst.size)
             self._restore_breakpoint(ip)
-            pointer = ip + inst.size
-            self._set_breakpoint(pointer, temporary=True)
-            self._cont()
-            self.wait() # I will have to think about how to implement it, but for 1 instruction (fuck there are the function calls too)... [02/03/23]
         else:
             self.step()
 
     def wait(self):
         status_pointer = self.dbg.alloc(4)
         self.dbg.call("waitpid", [self.pid, status_pointer, 0x40000000, 0])
         # be carefull that INT3 is executed as an instruction! You have to back down
```

### Comparing `gdb_plus-6.1.0/gdb_plus/gdb_plus.py` & `gdb_plus-6.1.1/gdb_plus/gdb_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         """
         Wrapper around execute to handle commands that will require a wait
         """
         self.priority += 1
         self.__clear_stop(sender if sender is not None else command)
         self.execute(command)
 
-    # TODO handle case where I use gdb manually for more than reading the memory [26/04/23]
+    # TODO make the option to have "until" be non blocking with an event when we reach the address [28/04/23] In other words migrate wait=False to wait=Event()
     def c(self, wait=False, force = False, until = None):
         """
         Continue execution of the process
 
         Arguments:
             wait: Should block your script until the next interruption ?
             until: Continue until a specified location. Your script will wait if you have to play with gdb manually.
@@ -387,17 +387,16 @@
         if force:
             self.__broken_step()
         # Remember not to put the breakpoint yourself !
         if until is not None:
             address = self.parse_address(until)
             self.b(address, temporary=True)
             wait = True
-        self.priority += 1
-        self.__clear_stop("continue")
-        self.execute("continue")
+            log.debug(f"continuing until {hex(address)}")
+        self.execute_action("continue", sender="continue")
         if wait:
             self.priority_wait()
         #else:
         #    log.warn_once("remember about priority")
         if until:
             while self.instruction_pointer != address:
                 log.info(f"debugger stopped at {hex(self.instruction_pointer)} for '{self._stop_reason}' instead of {hex(address)}")
@@ -594,32 +593,39 @@
             self.step()
 
         log.warn_once(f"I made {limit} steps and haven't found what you are looking for...")
         return -1
 
     # May not want to wait if you are going over a functions that need user interaction
     def next(self, wait:bool=True, repeat:int=1):
-        for _ in range(repeat):
+        if wait == False:
             self.execute_action("ni", sender="next")
-            if wait:
-                self.priority_wait()
-            #else:
             #    log.warn_once("remember about priority")
+        else:
+            for _ in range(repeat):
+                next_inst = self.next_inst
+                if next_inst.mnemonic == "call":
+                    self.c(until=self.instruction_pointer+next_inst.size)
+                else:
+                    self.step()
 
     ni = next
 
     # Don't use repeat and no_wait together ... [06/03/23]
     # Not sure if repeat is so useful... [21/03/23]
     # May be dependent on the stack frame and cause problems after a jump [27/04/23]
     def finish(self, *, wait:bool=True, repeat = 1):
-        for _ in range(repeat):
-            self.stepped = True # No really stepped, But I don't want a new variable
+        if wait == False:
             self.execute_action("finish", sender="finish")
-            if wait:
-                self.priority_wait()
+
+        for _ in range(repeat):
+            ip = self.__saved_ip
+            if ip == 0:
+                raise Exception("stack frame is broken or we are not in a function")
+            self.c(until=ip)
 
     # How to handle a jump no wait without destroying the priority queue ? [17/04/23]
     # Don't let it as an option... [17/04/23]
     def jump(self, location: [int, str], stop = True):
         """
         Jump to specified location
         """
@@ -630,14 +636,15 @@
         self.b(address, temporary=True)
         self.execute_action(f"jump *{hex(address)}", sender="jump")
         log.debug("Waiting for jump to conclude")
         self.priority_wait()
 
     # Now can return from anywhere in the function
     # Works only for standard functions (push rbp; mov rbp, rsp; ...; leave; ret;). May crash if used in the libc
+    # Can't I use __saved_ip now ? [28/04/23]
     def ret(self, value: int = None):
         """
         Exit from current function without executing it. 
 
         Warning: Experimental and depends on the stack frame
         """
         log.warn_once(f"ret is still at an experimental stage and may not work properly")
@@ -747,15 +754,14 @@
             if end_pointer is None:
                 self.finish() # Finish can only work if you have a leave ret. Set the last address otherwise
                 # Wait why don't I just put a breakpoint on my address before calling the function instead ? Because the user may call the function from inside itself...
                 #self.c(until=return_address)
                 log.debug("call finished")
                 
             else:
-                log.warn_once("You chose to use 'end_pointer'. Only do it if you need breakpoints in the function and to restore memory when exiting!")
                 self.c(until=end_pointer)
                 # Exit the function
                 self.step()
             
             res = self.return_value
             self.restore_backup(backup)
             for pointer, n in to_free[::-1]: #I do it backward to have a coherent behaviour with heap=False, but I still don't really know if I should implement a free in that case
@@ -1252,14 +1258,15 @@
             self.rbp = value
 
     # Prevent null pointers
     @property
     def instruction_pointer(self):
         ans = 0
         while ans == 0:
+            # what about self.gdb.newest_frame().pc() ? [28/04/23]
             if context.bits == 32:
                 ans = self.eip
             else:
                 ans = self.rip
             # log
             if ans == 0:
                 log.debug("null pointer in ip ! retrying...")
@@ -1268,14 +1275,28 @@
     @instruction_pointer.setter
     def instruction_pointer(self, value):
         if context.bits == 32:
             self.eip = value
         else:
             self.rip = value
 
+    @property
+    def __saved_ip(self):
+        return self.gdb.newest_frame().older().pc()
+
+        ## rip = 0x7ffff7fe45b8 in _dl_start_final (./elf/rtld.c:507); saved rip = 0x7ffff7fe32b8
+        #data = self.execute("info frame 0").split("\n")
+        #print(data)
+        #for line in data:
+        #    if " saved " in line and "ip = " in line:
+        #        ip = line.split("saved ")[-1].split("= ")[-1]
+        #        if "<" in ip:
+        #            return 0
+        #        return int(ip, 16)
+
     ########################## FORKS ##########################
     # TODO find a better name [28/02/23]
     # TODO make inferior and n the same parameter ? [04/03/23]
 
     # Call shellcode has problems: https://sourceware.org/gdb/onlinedocs/gdb/Registers.html. Can't push rip
     # Warn that the child will still be in the middle of the fork [26/04/23]
     def split_child(self, n = None, /, inferior = None):
```

### Comparing `gdb_plus-6.1.0/gdb_plus/utils.py` & `gdb_plus-6.1.1/gdb_plus/utils.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.0/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.1.1/gdb_plus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.1.0
+Version: 6.1.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -250,18 +250,19 @@
 
 See [this example](./examples/black_box_analysis_of_function.py) for more details
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
-You may want to debug manually the function called. If this is the case set last address of your function in `call(..., end_pointer= ...)` so that the script continues only once you reach the end of the function and not while you are using gdb
+If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
 ## Alternatives
 from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
 
 # TODO
 
 * Add option to use libdebug instead of gdb
+* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
```

### Comparing `gdb_plus-6.1.0/pyproject.toml` & `gdb_plus-6.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools",
     "wheel",
 ]
 
 [project]
 name = "gdb_plus"
 description = "Python library to automate gdb debugging"
-version = "6.1.0"
+version = "6.1.1"
 authors = [{name = "Edoardo"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "pwntools>=4.5.0",
     "capstone"
 ]
```

### Comparing `gdb_plus-6.1.0/tests/test.py` & `gdb_plus-6.1.1/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
 				second_child.c(wait=True)
 			
 			self.assertTrue(b"YES !" in dbg.p.recv())
 
 			second_child.close()
 			dbg.close()
 
-#@unittest.skip
+@unittest.skip
 class Debugger_signals(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		warnings.simplefilter("ignore", ImportWarning)
 		self.dbg = Debugger("./ExceptionalChecking_patched")
 
 	def tearDown(self):
```

