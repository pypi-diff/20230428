# Comparing `tmp/gdb_plus-5.4.1.tar.gz` & `tmp/gdb_plus-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-5.4.1.tar", last modified: Mon Feb 27 19:16:34 2023, max compression
+gzip compressed data, was "gdb_plus-6.1.0.tar", last modified: Fri Apr 28 08:19:30 2023, max compression
```

## Comparing `gdb_plus-5.4.1.tar` & `gdb_plus-6.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-02-27 19:16:34.649526 gdb_plus-5.4.1/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-5.4.1/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)     9613 2023-02-27 19:16:34.648430 gdb_plus-5.4.1/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)     9120 2023-02-27 19:16:20.000000 gdb_plus-5.4.1/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-02-27 19:16:34.629670 gdb_plus-5.4.1/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)       59 2023-02-27 16:58:38.000000 gdb_plus-5.4.1/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    33600 2023-02-27 19:00:59.000000 gdb_plus-5.4.1/gdb_plus/gdb_plus.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-02-27 19:16:34.643036 gdb_plus-5.4.1/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)     9613 2023-02-27 19:16:34.000000 gdb_plus-5.4.1/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      247 2023-02-27 19:16:34.000000 gdb_plus-5.4.1/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-02-27 19:16:34.000000 gdb_plus-5.4.1/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       18 2023-02-27 19:16:34.000000 gdb_plus-5.4.1/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-02-27 19:16:34.000000 gdb_plus-5.4.1/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      623 2023-02-27 19:13:29.000000 gdb_plus-5.4.1/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-02-27 19:16:34.649919 gdb_plus-5.4.1/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-02-27 19:16:34.645297 gdb_plus-5.4.1/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)     8146 2023-02-27 19:13:07.000000 gdb_plus-5.4.1/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.746626 gdb_plus-6.1.0/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.0/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11492 2023-04-28 08:19:30.745431 gdb_plus-6.1.0/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11251 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.667915 gdb_plus-6.1.0/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11204 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    75285 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.726381 gdb_plus-6.1.0/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11492 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-04-28 08:19:30.000000 gdb_plus-6.1.0/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-04-28 08:19:30.747006 gdb_plus-6.1.0/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-04-28 08:19:30.728755 gdb_plus-6.1.0/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    17642 2023-04-28 08:06:22.000000 gdb_plus-6.1.0/tests/test.py
```

### Comparing `gdb_plus-5.4.1/LICENSE` & `gdb_plus-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-5.4.1/PKG-INFO` & `gdb_plus-6.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,253 @@
-Metadata-Version: 2.1
-Name: gdb_plus
-Version: 5.4.1
-Summary: Python library to automate gdb debugging
-Author: Edoardo
-Project-URL: Homepage, https://github.com/Angelo942/pydbg
-Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Unix
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GDB+
-*Python library to automate gdb debugging* 
-
-GDB+ is a wrapper around gdb powered by pwntools. The goal is automate your interactions with gdb and add some extra features.
-
-## Main features
-
-* Include a python function as callback when you set a breakpoint.
-* Read the canary instead of bruteforcing it every time you need it while testing your exploit.
-* Test a specific function of a binary with the parameters you want at any time.
-* Log the code of a self modifying function.
-* Backup parts of your memory and restore it during future executions.
-* Don't waste time commenting your code. The arguments `NOPTRACE` and `REMOTE` make the exploit skip any action related to gdb.
-
-## Installation
-
-```
-pip3 install gdb_plus
-```
-
-
-**Warning for pwndbg users:**  
-Previous bugs in Pwndbg used to break the api for python. While GDB+ should work with the current version of pwndbg [19/12/2022], but bugs may appear again.
-you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
-
-## Debugging
-
-You can debug a program using the path to the binary.   
-If you really have to you can also use a process or even just his pid. 
-For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
-
-```py
-from gdb_plus import *
-
-gdbinit = """
-handle SIGALRM nopass
-continue
-"""
-
-dbg = Debugger("./rev_challenge", script=gdbinit, aslr=False)
-dbg = Debugger("./pwn_challenge", script=gdbinit).remote("10.10.0.1", 1337)
-
-
-p = process("./challenge", aslr=False)
-dbg = Debugger(p, script=gdbinit)
-
-#pidof process : 3134
-dbg = Debugger(3134, script=gdbinit, binary="./challenge")
-```
-
-Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
-
-**Note**  
-Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
-
-**Warning**  
-Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
-
-## Control Flow
-
-The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb.
-
-```py
-dbg.step() # Single instruction (will enter function calls)
-dbg.next() # Next instruction (will jump over function calls)
-dbg.cont() # Continue execution
-dbg.finish() # Finish current function
-dbg.interrupt() # Stop the execution of your process
-dbg.wait() # Wait untill you have control of gdb
-```
-
-**Warning**  
-* `finish` can only work if your function has a `leave; ret;` at the end
-* `wait` can take as parameter a timeout. Use it if you aren't sure gdb has already stoped to avoid waiting forever.
-* `ìnterrupt` expects that the process is currently running. If you aren't sure it will be the case use `interrupt(wait=False)`
-
-If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
-
-```py
-def MyCallback(dbg):
-    if dbg.next_inst.mnemonic == "int3":
-        dbg.step()
-        dbg.signal("SIGINT")
-    print(dbg.next_inst.toString())
-
-dbg.step_until_ret(MyCallback)
-```
-
-In this example at each step the callback will be executed decrypting the next function chunk by chunk and logging the instructions. See [this example](./examples/debug_self_modifying_function.py) for more details solving a real challenge.
-
-You could also use `dbg.step_until_address(<address>, <callback=None>)` if you just want to execute a limited area of code.  
-
-## Breakpoints
-
-Breakpoints have two main features:
-* if the address is smaller than 0x10000 the address will immediately be interpreted as relative for PIE binaries 
-* you can set callbacks and don't have the breakpoint interrupt the process to run them
-
-The callback is a function that takes the debugger as parameter and returns a boolean to tell gdb if it should stop or not. Inside you can do anything you want with the memory
-If you want to pass data from your callback function to your exploit you can use pointers (lists, dictionaries or queues)
-
-**Note**  
-Setting a breakpoint requires the process to be interrupted.
-
-```py
-from gdb_plus import *
-from queue import Queue
-
-# I let the process run in this example to reinforce the need for the interrupt later
-gdbinit = """
-handle SIGALRM nopass
-continue
-"""
-
-dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
-pointer_to_secret = Queue()
-
-def MyCallback(dbg):
-    pointer_to_secret.put(dbg.rdx)
-    return False
-
-# You have to interrupt the execution if you want a callback
-dbg.interrupt()
-dbg.breakpoint("encrypt") # Break on function "encrypt"
-dbg.breakpoint(0xdead, callback=MyCallback)
-dbg.cont()
-
-dbg.wait()
-# Read the data set by the breakpoint
-print(pointer_to_secret.get())
-# You can disable individual breakpoints 
-dbg.breakpoints[hex(dbg.base_elf + 0xdead)].enabled = False # To access a breakpoint you will need the full address
-dbg.breakpoints["encrypt"].enabled = False # And the name if you didn't set it with an address
-```
-
-Currently you can set the breakpoint to permanent or temporary. Permanent ones get saved in `dbg.breakpoints[hex(absolute_address)]`, temporary ones aren't saved and get disabled automatically when hit for the first time. 
-
-**Warning**
-"*When hit*". If the return value of a callback is False the breakpoint won't be hit. This means that a temporary breakpoint won't be removed in this situation and the callback may end up being called multiple times if you are in a loop.
-
-## Memory access
-
-All registers are accessible as properties
-
-```py
-dbg.rax = 0xdeadbeefdeadbeef
-dbg.eax = 0xfafafafa
-dbg.ax  = 0xbabe
-dbg.ah = 0x90
-assert dbg.rax == 0xdeadbeeffafa90be
-```
-
-You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
-
-```py
-pointer = dbg.alloc(8)
-dbg.write(pointer, p64(0xdeadbeef))
-secret = dbg.read(dbg.elf.symbols["secret"], 0x10)
-canary = dbg.canary
-```
-
-**Note**  
-While you can access the registers only when the process is at a stop, remember that you can read and write on the memory at any time
-
-Pwntools let you access the address where each library is loaded with `p.libs()[<path_to_library>]`
-We have two wrapper for the main ones:
-* `dbg.base_elf`
-* `dbg.base_libc`
-
-from gdb_plus >= 5.4.0 dbg.elf.address is already set to the correct address even with ASLR on, so you may need dbg.base_elf only if you debug a process for wich you don't have the binary
-
-We can also use capstone to know what is the next instruction that will be executed
-```py
-print(dbg.next_inst.toString()) # "mov rax, r12"
-print(dbg.next_inst.mnemonic)   # "mov"
-```
-
-## Black box
-
-If you want to test the effects of a specific function you can directly call it with the parameters you want
-
-```py
-pointer = dbg.alloc(100)
-# Initialize data
-dbg.write(pointer, bytes([i for i in range(100)]))
-dbg.call(dbg.p.symbols["obfuscated_pbox"], [pointer, "user_1", 1])
-dbg.read(pointer, 100)
-```
-
-See [this example](./examples/black_box_analysis_of_function.py) for more details
-
-**Note**  
-You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
-
-**Warning**  
-You may want to be careful with breakpoints inside the function called. If you don't set any the state of you process will be identical after the execution except for data writen on the stack (which shouldn't influence the future) and the bss (which you may want to correct if needed on a case by case). If you put a breakpoint you will have to handle yourself the execution from your breakpoint onward.  
-Another option would be to pass a pointer to the return instruction, it will block you python script untill you reach that specific point, so you will have to work manualy from gdb for that part.
-
-## Alternatives
-If something can be done with gdb it should be easily programable with gdb_plus, but you may find it slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit developement you may prefere something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
+# GDB+
+*Python library to automate gdb debugging* 
+
+GDB+ is a wrapper around gdb powered by pwntools. The goal is automate your interactions with gdb and add some extra features.
+
+## Main features
+
+* Include a python function as callback when you set a breakpoint.
+* Read the canary instead of bruteforcing it every time you need it while testing your exploit.
+* Test a specific function of a binary with the parameters you want at any time.
+* Log the code of a self modifying function.
+* Backup parts of your memory and restore it during future executions.
+* Don't waste time commenting your code. The arguments `NOPTRACE` and `REMOTE` make the exploit skip any action related to gdb.
+
+## Installation
+
+stable
+```
+pip3 install gdb_plus
+```
+or dev branch
+```
+pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
+```
+
+**Warning for pwndbg users:**  
+Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork.
+you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
+
+## Debugging
+
+You can debug a program using the path to the binary.   
+If you really have to you can also use a process or even just his pid. 
+For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
+
+```py
+from gdb_plus import *
+
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./rev_challenge", script=gdbinit, aslr=False)
+dbg = Debugger("./pwn_challenge", script=gdbinit).remote("10.10.0.1", 1337)
+
+
+p = process("./challenge", aslr=False)
+dbg = Debugger(p, script=gdbinit)
+
+#pidof process : 3134
+dbg = Debugger(3134, script=gdbinit, binary="./challenge")
+```
+
+By default your process will be analysed from the first instruction of the loader. If the process you are debugging has some checks you want to avoid use `Debugger(..., debug_from=<address>)` to attach with gdb at a specific address.  
+This will block you script until you reach you address. If you need to execute code in between you can use the non blocking alternative: 
+
+```py
+Im_done = Event()
+dbg = Debugger("./challenge").debug_from("main+0x34", event=Im_done)
+dbg.p.sendline("this is my input")
+Im_done.set()
+dbg.debug_from_done.wait()
+```
+
+This should pass any check for a debugger, even searches for INT3, exept a full check that the memory hasn't been edited.
+
+Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
+
+**Note**  
+Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
+
+**Warning**  
+Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
+
+## Control Flow
+
+The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require calling `dbg.wait()`.
+
+```py
+dbg.step() # Single instruction (will enter function calls)
+dbg.next() # Next instruction (will jump over function calls)
+dbg.cont() # Continue execution
+dbg.finish() # Finish current function
+dbg.interrupt() # Stop the execution of your process
+dbg.wait() # Wait until you have control of gdb
+```
+
+**Note**
+* dbg.cont(until=ADDRESS) allows you to block your script until you reach a specific address (or symbol). This means that you can debug manually with gdb while your script is waiting without problems
+
+**Warning**  
+* `finish` can only work if the stack frame hasn't been corrupted
+* you should specify if you want continue to wait or not with `dbg.cont(wait=True/False)`. We aren't sure about what should be the default behaviour and may set it to `wait=True` in a future version
+* Try avoiding `interrupt` as much as possible. 
+
+If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
+
+```py
+def MyCallback(dbg):
+    if dbg.next_inst.mnemonic == "int3":
+        dbg.step()
+        dbg.signal("SIGINT")
+    print(dbg.next_inst.toString())
+
+dbg.step_until_ret(MyCallback)
+```
+
+In this example at each step the callback will be executed decrypting the next function chunk by chunk and logging the instructions. See [this example](./examples/debug_self_modifying_function.py) for more details solving a real challenge.
+
+You could also use `dbg.step_until_address(<address>, <callback=None>)` if you just want to execute a limited area of code or `dbg.step_until_condition(<check>)` if you are not sure where to stop.  
+
+## Breakpoints
+
+Breakpoints have three main features:
+* if the address is smaller than 0x10000 the address will immediately be interpreted as relative for PIE binaries
+* you can use a symbol name instead of an address such as `"main"` or `"main+0x12"`
+* you can set callbacks to be executed when the breakpoint is reach and may choose to let the process continue after the execution.
+
+The callback is a function that takes the debugger as parameter and returns a boolean to tell gdb if it should stop or not.
+The callbacks shouldn't be limited in what you can code. If you find problems raise an issue.
+If you want to pass data from your callback function to your exploit you can use pointers (lists, dictionaries or queues)
+
+**Note**  
+Setting a breakpoint requires the process to be interrupted.
+
+```py
+from gdb_plus import *
+from queue import Queue
+
+# I let the process run in this example to reinforce the need for the interrupt later
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
+pointer = Queue()
+
+# step over an hypothetical call to a function, overwrite the return value and save it in a queue
+def MyCallback(dbg):
+    dbg.next()
+    log.info(f"I tried to return {dbg.rax}")
+    pointer.put(dbg.rax)
+    dbg.rax = 0
+    # Return False to let the process run after executing the callback
+    return False
+
+def SecondCallback(dbg):
+    log.info("now you can play around with gdb")
+    log.info("once you are done execute continue in gdb and your script will resume once we reach main+0x534")
+    # Return True to interrupt the process
+    return True
+
+# You can not set a breakpoint while the process is running
+dbg.breakpoint("main+0x42", callback=MyCallback, temporary = True)
+dbg.breakpoint("main+0x124", callback=SecondCallback)
+dbg.cont(until="main+0x534")
+
+# Read the data set by the breakpoint
+print(pointer_to_secret.get())
+dbg.delete_breakpoint("main+0x124")
+```
+
+## Memory access
+
+All registers are accessible as properties
+
+```py
+dbg.rax = 0xdeadbeefdeadbeef
+dbg.eax = 0xfafafafa
+dbg.ax  = 0xbabe
+dbg.ah = 0x90
+assert dbg.rax == 0xdeadbeeffafa90be
+```
+
+You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
+
+```py
+pointer = dbg.alloc(8)
+dbg.write(pointer, p64(0xdeadbeef))
+secret = dbg.read(dbg.elf.symbols["secret"], 0x10)
+canary = dbg.canary
+```
+
+**Note**  
+While you can access the registers only when the process is at a stop, remember that you can read and write on the memory at any time
+
+Pwntools let you access the address where each library is loaded with `p.libs()[<path_to_library>]`
+We have two wrapper for the main ones:
+* `dbg.base_elf`
+* `dbg.base_libc`
+
+from gdb_plus >= 5.4.0 dbg.elf.address is already set to the correct address even with ASLR on, so you may need dbg.base_elf only if you debug a process for wich you don't have the binary
+
+We can also use capstone to know what is the next instruction that will be executed
+```py
+print(dbg.next_inst.toString()) # "mov rax, r12"
+print(dbg.next_inst.mnemonic)   # "mov"
+```
+
+## Fork
+You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`.
+
+```py
+dbg = Debugger("http_server").set_split_on_fork()
+dbg.cont(wait=False)
+dbg.p.sendline("input")
+pid_child = dbg.wait_split()
+
+# all children are saved in dbg.children and can be accessed by the pid
+child = dbg.children[pid_child]
+```
+
+If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
+
+```py
+child.emulate_ptrace_slave(dbg)
+dbg.emulate_ptrace_master(child)
+```
+
+This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them.
+
+**Warning**
+pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+
+## Call functions
+
+If you want to test the effects of a specific function you can directly call it with the parameters you want
+
+```py
+pointer = dbg.alloc(100)
+# Initialize data
+dbg.write(pointer, bytes([i for i in range(100)]))
+dbg.call(dbg.p.symbols["obfuscated_pbox"], [pointer, "user_1", 1])
+dbg.read(pointer, 100)
+```
+
+See [this example](./examples/black_box_analysis_of_function.py) for more details
+
+**Note**  
+You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
+
+**Warning**  
+You may want to debug manually the function called. If this is the case set last address of your function in `call(..., end_pointer= ...)` so that the script continues only once you reach the end of the function and not while you are using gdb
+
+## Alternatives
+from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
+
+# TODO
+
+* Add option to use libdebug instead of gdb
+* Identify actions performed manually in gdb (overwrite finish and ni)
+* Handle fork and ptrace from syscall instead of libc
+* Improve ptrace emulation
```

### Comparing `gdb_plus-5.4.1/pyproject.toml` & `gdb_plus-6.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools",
-    "wheel",
-]
-
-[project]
-name = "gdb_plus"
-description = "Python library to automate gdb debugging"
-version = "5.4.1"
-authors = [{name = "Edoardo"}]
-readme = "README.md"
-requires-python = ">=3.9"
-dependencies = [
-    "pwntools",
-    "capstone"
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: Unix",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Angelo942/pydbg"
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools",
+    "wheel",
+]
+
+[project]
+name = "gdb_plus"
+description = "Python library to automate gdb debugging"
+version = "6.1.0"
+authors = [{name = "Edoardo"}]
+readme = "README.md"
+requires-python = ">=3.8"
+dependencies = [
+    "pwntools>=4.5.0",
+    "capstone"
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: Unix",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Angelo942/pydbg"
 "Bug Tracker" = "https://github.com/Angelo942/pydbg/issues"
```

