# Comparing `tmp/ejtraderTH-1.0.3.tar.gz` & `tmp/ejtraderTH-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ejtraderTH-1.0.3.tar", last modified: Thu Mar  4 16:20:08 2021, max compression
+gzip compressed data, was "ejtraderTH-1.0.4.tar", last modified: Fri Apr 28 14:04:30 2023, max compression
```

## Comparing `ejtraderTH-1.0.3.tar` & `ejtraderTH-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-04 16:20:08.186492 ejtraderTH-1.0.3/
--rw-r--r--   0 sos        (501) staff       (20)     1085 2021-03-04 15:05:47.000000 ejtraderTH-1.0.3/LICENSE.txt
--rw-r--r--   0 sos        (501) staff       (20)       48 2021-03-04 16:00:37.000000 ejtraderTH-1.0.3/MANIFEST.in
--rw-r--r--   0 sos        (501) staff       (20)    13887 2021-03-04 16:20:08.186730 ejtraderTH-1.0.3/PKG-INFO
--rw-r--r--   0 sos        (501) staff       (20)    10437 2021-03-04 15:55:36.000000 ejtraderTH-1.0.3/README.md
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-04 16:20:08.184582 ejtraderTH-1.0.3/ejtraderTH/
--rw-r--r--   0 sos        (501) staff       (20)     2219 2021-03-04 16:15:35.000000 ejtraderTH-1.0.3/ejtraderTH/__init__.py
--rw-r--r--   0 sos        (501) staff       (20)     4082 2021-03-04 15:05:15.000000 ejtraderTH-1.0.3/ejtraderTH/ejtraderTH.py
-drwxr-xr-x   0 sos        (501) staff       (20)        0 2021-03-04 16:20:08.186244 ejtraderTH-1.0.3/ejtraderTH.egg-info/
--rw-r--r--   0 sos        (501) staff       (20)    13887 2021-03-04 16:20:08.000000 ejtraderTH-1.0.3/ejtraderTH.egg-info/PKG-INFO
--rw-r--r--   0 sos        (501) staff       (20)      286 2021-03-04 16:20:08.000000 ejtraderTH-1.0.3/ejtraderTH.egg-info/SOURCES.txt
--rw-r--r--   0 sos        (501) staff       (20)        1 2021-03-04 16:20:08.000000 ejtraderTH-1.0.3/ejtraderTH.egg-info/dependency_links.txt
--rw-r--r--   0 sos        (501) staff       (20)        8 2021-03-04 16:20:08.000000 ejtraderTH-1.0.3/ejtraderTH.egg-info/requires.txt
--rw-r--r--   0 sos        (501) staff       (20)       11 2021-03-04 16:20:08.000000 ejtraderTH-1.0.3/ejtraderTH.egg-info/top_level.txt
--rw-r--r--   0 sos        (501) staff       (20)        0 2021-03-04 16:14:00.000000 ejtraderTH-1.0.3/requirements.txt
--rw-r--r--   0 sos        (501) staff       (20)       67 2021-03-04 16:20:08.187236 ejtraderTH-1.0.3/setup.cfg
--rw-r--r--   0 sos        (501) staff       (20)     2148 2021-03-04 16:20:05.000000 ejtraderTH-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/ejtraderTH/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/ejtraderTH/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/ejtraderTH/ejtraderTH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/ejtraderTH.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-28 14:04:30.000000 ejtraderTH-1.0.4/ejtraderTH.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 14:04:30.000000 ejtraderTH-1.0.4/ejtraderTH.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:04:30.000000 ejtraderTH-1.0.4/ejtraderTH.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 14:04:30.000000 ejtraderTH-1.0.4/ejtraderTH.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:04:30.071299 ejtraderTH-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 14:04:16.000000 ejtraderTH-1.0.4/tests/test.py
```

### Comparing `ejtraderTH-1.0.3/LICENSE.txt` & `ejtraderTH-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ejtraderTH-1.0.3/PKG-INFO` & `ejtraderTH-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,325 +1,329 @@
 Metadata-Version: 2.1
 Name: ejtraderTH
-Version: 1.0.3
+Version: 1.0.4
 Summary: This tiny little python module is useful for creating multiple threads of any function in seconds.
 Home-page: https://ejtraderTH_mt.readthedocs.io/
+Download-URL: https://ejtraderTH.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
-Download-URL: https://ejtraderTH.com
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderTH_mt/issues
 Project-URL: Source, https://github.com/traderpedroso/ejtraderTH_mt
 Project-URL: Documentation, https://ejtraderTH.readthedocs.io/
-Description: ```python
-        pip install ejtraderTH
-        ```
-        
-        This tiny little python module is useful for creating multiple threads of any function in seconds.
-        
-        #### What's new in v1.0
-        
-        A quick launch mode is added, just type `ejtraderTH.start(func_name, repeat=10)` and it will execute the given function given number of times in parallel. A standard way of measuring elapsed time is added as well. see examples below to understand how to use quick launch mode.
-        
-        After using this library for a number of times in various projects i found that if you pass in lots of data say `1000` data in a list, it was creating `1000` threads to do it all once, how ever in the practical world most of the times cpu's are not capable of creating so many threads at once or worse it eats up all resources at once. To prevent this problem now you can pass in `max_threads` value by default if you don't pass in the value it will automatically be set equal to 4 just for the safety purpose, and passing a `0` value will throw an error while creating a `ejtraderTH` object this way it will only create specified number of threads at once and will wait untill the previously started threads has finished their job.
-        
-        Other than that to keep a track on how many threads are been created in real time you can push in a new log method inn you processing function so that whenever a new thread is created you can see it, there ar two methods of tracking them.
-        
-        - just to print out the thread number which is being created, use: ` ejtraderTH.console_log(output=True)`
-        - if you want to store it in some variable you can use: `thread_number = ejtraderTH.console_log()`
-        - in case some error occurs, the thread will keep on running
-        - if you want to kill all the threads use `ejtraderTH.stop()` inside your processing function while handling errors.
-        
-        #### Problem Statement
-        
-        - Let say for example, we have a `list` of numbers from `1 to 10` and all we wanted to do is `multiply every number by 1000` but the challenge is `it takes 5 sec` for multiplying a single number by 1000 from the list, I know its an arbitary condition, but we can create it with `time.sleep(5)` function.
-        - Or you want to make a web request million times, without waiting for the server to respond you to make the next request.
-        
-        #### Working
-        
-        So what this module does is, at the time of object initialization it takes in the function which is used for processing data and max number of thread which can be created at once, when running in multi threads, and as input it takes a list of arguments for which multiple threads will be created.
-        
-        ---
-        
-        #### Example 1
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        #the function for processing data
-        def my_func(data):
-            print(f'>> Running Thread {ejtraderTH.console_log()}')
-            data = data*1000
-            time.sleep(5)
-            return data
-        
-        #list of input data for processing
-        raw_data = [1,2,3,4,5,6,7,8,9,10]
-        
-        #sending arguments for asynchronous multi thread processing
-        processed_data = ejtraderTH.start(my_func, data=raw_data, max_threads=10)
-        
-        #printing the synchronised received results
-        print()
-        print(f'>> Input: {raw_data}')
-        print(f'>> Result: {processed_data}')
-        print(f'>> Elapsed time: {ejtraderTH.elapsed()} sec')
-        ```
-        
-        #### output
-        
-        ```python
-        >> Running Thread 1
-        >> Running Thread 2
-        >> Running Thread 3
-        >> Running Thread 4
-        >> Running Thread 5
-        >> Running Thread 6
-        >> Running Thread 7
-        >> Running Thread 8
-        >> Running Thread 9
-        >> Running Thread 10
-        
-        >> Input: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
-        >> Result: [1000, 2000, 3000, 4000, 5000, 6000, 7000, 8000, 9000, 10000]
-        >> Elapsed time: 5.0 sec
-        ```
-        
-        Now you can clearly see, if we do it without multi threading it would have taken around `50 Seconds` for processing the data while doing the task one by one and waiting for `5 Sec` after running the function each time. but since we are doing it with multithreading it will take only `5 Seconds` for processing the same task with different data, in their individual threads.
-        
-        #### Example 2
-        
-        ```python
-        #the function for processing data
-        def my_func(data):
-            ejtraderTH.console_log(output=True)
-            ip = req.request(method='GET',url="http://ipinfo.io/ip")
-        
-            return ip.content
-        
-        #sending arguments for asynchronous multi thread processing
-        processed_data = ejtraderTH.start(my_func, repeat=20, max_threads=20)
-        
-        #printing the synchronised received results
-        print()
-        print(f'>> Result: {processed_data}')
-        ejtraderTH.elapsed(output=True)
-        ```
-        
-        #### output
-        
-        ```python
-        >> Creating Threads 1
-        >> Creating Threads 2
-        >> Creating Threads 3
-        >> Creating Threads 4
-        >> Creating Threads 5
-        >> Creating Threads 6
-        >> Creating Threads 7
-        >> Creating Threads 8
-        >> Creating Threads 9
-        >> Creating Threads 10
-        >> Creating Threads 11
-        >> Creating Threads 12
-        >> Creating Threads 13
-        >> Creating Threads 14
-        >> Creating Threads 15
-        >> Creating Threads 16
-        >> Creating Threads 17
-        >> Creating Threads 18
-        >> Creating Threads 19
-        >> Creating Threads 20
-        
-        >> Result: [b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37']
-        >> Elapsed time: 0.31 sec
-        ```
-        
-        In this example we didn't used time.sleep() instead we make a request to the webserver and it took `0.5 seconds` to get the result back so we did it 20 times with multi threading and were able to receive the results in less time in a synchronous order.
-        
-        > Lets try to do it without multithreading and see how it affects the processing time.
-        
-        So in this new update `ejtraderTH v1.0` we can specify that at once how many threads should be created so lets change the input parameter as `max_threads = 1` this way it will only create one thread at a time and will wait until the previous thread has finished properly.
-        
-        #### output
-        
-        ```python
-        .
-        .
-        .
-        >> Elapsed time: 6.43 sec
-        ```
-        
-        It is clear that every request to the server was taking approx. `0.5 seconds` so while making one request at a time it took `6.43 seconds` as expected.
-        
-        ### Example 3
-        
-        Quick Launch mode, a new feature is added where you can directly use ejtraderTH to pass in the repetitive function, input data for those functions and how many threads you want it to create at a time. other than that if you just want it to repeat the function without any inputs you can do that too.
-        
-        ```python
-        import ejtraderTH
-        import time
-        import random
-        
-        names = ['April', 'May']
-        
-        #the function for processing data
-        def my_func(data):
-            ejtraderTH.console_log(output=True)
-            time.sleep(1)
-            name = random.choice(names)
-            return f'{name} says, Hello World!'
-        
-        processed_data = ejtraderTH.start(my_func, repeat=4)
-        
-        print(processed_data)
-        ejtraderTH.elapsed(output=True)
-        ```
-        
-        ### output
-        
-        ```
-        >> Creating Threads 1
-        >> Creating Threads 2
-        >> Creating Threads 3
-        >> Creating Threads 4
-        ['May says, Hello World!', 'April says, Hello World!', 'May says, Hello World!', 'April says, Hello World!']
-        >> Elapsed time: 1.0 sec
-        ```
-        
-        we kept a time gap of 1 sec inside the function still it repeated the task 4 times in same time. since it can access the global variables we can assign certain tasks that don't need different inputs every time.
-        
-        ### Decorators support
-        
-        Apart from calling the `start()` attribute we can also use decorators to explicitly make our functions for concurrent execution.
-        
-        **Example 1**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.run(repeat=5, max_threads=5)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        print(ejtraderTH.result['my_func'])
-        ```
-        
-        **Output**
-        
-        ```python
-        [0, 2, 4, 6, 8]
-        ```
-        
-        This will execute the function as soon as you run your python code, in this case we are trying to perform the same task five times in a row concurrently. The final output of all the function can be accessed by `ejtraderTH.result['function_name']`. Notice if you set your function on repeat it will always receive a parameter which is it's thread number.
-        
-        ---
-        
-        **Example 2**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.run(data=[1,2,3,4,5,6], max_threads=5)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        print(ejtraderTH.result['my_func'])
-        ```
-        
-        **Output**
-        
-        ```python
-        [2, 4, 6, 8, 10, 12]
-        ```
-        
-        In this case we are directly passing our arguments in a list via decorator and receiving the result same way as we did in previous example.
-        
-        ---
-        
-        **Exampe 3**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.set(max_threads=10)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        result = my_func(repeat=7)
-        print(result)
-        ```
-        
-        **Output**
-        
-        ```python
-        [0, 2, 4, 6, 8, 10, 12]
-        ```
-        
-        This is an another cool way to first convert your function in concurrent function and then passing the argument as how many time you want to execute that function all in parallel.
-        
-        ---
-        
-        **Example 4**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.set()
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        result = my_func([5,6,7])
-        print(result)
-        ```
-        
-        **Output**
-        
-        ```python
-        [10, 12, 14]
-        ```
-        
-        Again we can also specify what arguments we want to pass to the function to process it concurrently. if in the `@ejtraderTH.set()` decorator you won't pass any `max_threads` argument `max_threads=10` will be set.
-        
-        #### Handling errors and killing all threads
-        
-        So, by default if any error occurs the threads will keep on running, in case if you want to ignore some errors but if you want to kill all the thread at once you can use `ejtraderTH.stop()` while handling errors.
-        
-        ```python
-        #the function for processing data
-        def my_func(data):
-            thread_number = ejtraderTH.console_log(output=True)
-            try:
-                data = requests.get("http://httpbin.org/get")
-                return data
-            except Exception as e:
-                print(e) #printing other errors
-                #killing all active threads
-                ejtraderTH.stop() #use to kill all threads
-        ```
-        
-        if you don't use `ejtraderTH.stop()` function then the threads will keep on running and filling `None` in place of returned data. if you used the `ejtraderTH.stop()` it will kill all active threads immediately and will return the data that were processed by your function so far.
-        
 Keywords: metatrader,f-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
+License-File: LICENSE.txt
+
+
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderTH/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderTH)
+[![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderTH)](https://github.com/ejtraderLabs/ejtraderTH/blob/master/LICENSE)
+
+```python
+pip install ejtraderTH
+```
+
+This tiny little python module is useful for creating multiple threads of any function in seconds.
+
+#### What's new in v1.0
+
+A quick launch mode is added, just type `ejtraderTH.start(func_name, repeat=10)` and it will execute the given function given number of times in parallel. A standard way of measuring elapsed time is added as well. see examples below to understand how to use quick launch mode.
+
+After using this library for a number of times in various projects i found that if you pass in lots of data say `1000` data in a list, it was creating `1000` threads to do it all once, how ever in the practical world most of the times cpu's are not capable of creating so many threads at once or worse it eats up all resources at once. To prevent this problem now you can pass in `max_threads` value by default if you don't pass in the value it will automatically be set equal to 4 just for the safety purpose, and passing a `0` value will throw an error while creating a `ejtraderTH` object this way it will only create specified number of threads at once and will wait untill the previously started threads has finished their job.
+
+Other than that to keep a track on how many threads are been created in real time you can push in a new log method inn you processing function so that whenever a new thread is created you can see it, there ar two methods of tracking them.
+
+- just to print out the thread number which is being created, use: ` ejtraderTH.console_log(output=True)`
+- if you want to store it in some variable you can use: `thread_number = ejtraderTH.console_log()`
+- in case some error occurs, the thread will keep on running
+- if you want to kill all the threads use `ejtraderTH.stop()` inside your processing function while handling errors.
+
+#### Problem Statement
+
+- Let say for example, we have a `list` of numbers from `1 to 10` and all we wanted to do is `multiply every number by 1000` but the challenge is `it takes 5 sec` for multiplying a single number by 1000 from the list, I know its an arbitary condition, but we can create it with `time.sleep(5)` function.
+- Or you want to make a web request million times, without waiting for the server to respond you to make the next request.
+
+#### Working
+
+So what this module does is, at the time of object initialization it takes in the function which is used for processing data and max number of thread which can be created at once, when running in multi threads, and as input it takes a list of arguments for which multiple threads will be created.
+
+---
+
+#### Example 1
+
+```python
+import ejtraderTH
+import time
+
+#the function for processing data
+def my_func(data):
+    print(f'>> Running Thread {ejtraderTH.console_log()}')
+    data = data*1000
+    time.sleep(5)
+    return data
+
+#list of input data for processing
+raw_data = [1,2,3,4,5,6,7,8,9,10]
+
+#sending arguments for asynchronous multi thread processing
+processed_data = ejtraderTH.start(my_func, data=raw_data, max_threads=10)
+
+#printing the synchronised received results
+print()
+print(f'>> Input: {raw_data}')
+print(f'>> Result: {processed_data}')
+print(f'>> Elapsed time: {ejtraderTH.elapsed()} sec')
+```
+
+#### output
+
+```python
+>> Running Thread 1
+>> Running Thread 2
+>> Running Thread 3
+>> Running Thread 4
+>> Running Thread 5
+>> Running Thread 6
+>> Running Thread 7
+>> Running Thread 8
+>> Running Thread 9
+>> Running Thread 10
+
+>> Input: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+>> Result: [1000, 2000, 3000, 4000, 5000, 6000, 7000, 8000, 9000, 10000]
+>> Elapsed time: 5.0 sec
+```
+
+Now you can clearly see, if we do it without multi threading it would have taken around `50 Seconds` for processing the data while doing the task one by one and waiting for `5 Sec` after running the function each time. but since we are doing it with multithreading it will take only `5 Seconds` for processing the same task with different data, in their individual threads.
+
+#### Example 2
+
+```python
+#the function for processing data
+def my_func(data):
+    ejtraderTH.console_log(output=True)
+    ip = req.request(method='GET',url="http://ipinfo.io/ip")
+
+    return ip.content
+
+#sending arguments for asynchronous multi thread processing
+processed_data = ejtraderTH.start(my_func, repeat=20, max_threads=20)
+
+#printing the synchronised received results
+print()
+print(f'>> Result: {processed_data}')
+ejtraderTH.elapsed(output=True)
+```
+
+#### output
+
+```python
+>> Creating Threads 1
+>> Creating Threads 2
+>> Creating Threads 3
+>> Creating Threads 4
+>> Creating Threads 5
+>> Creating Threads 6
+>> Creating Threads 7
+>> Creating Threads 8
+>> Creating Threads 9
+>> Creating Threads 10
+>> Creating Threads 11
+>> Creating Threads 12
+>> Creating Threads 13
+>> Creating Threads 14
+>> Creating Threads 15
+>> Creating Threads 16
+>> Creating Threads 17
+>> Creating Threads 18
+>> Creating Threads 19
+>> Creating Threads 20
+
+>> Result: [b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37']
+>> Elapsed time: 0.31 sec
+```
+
+In this example we didn't used time.sleep() instead we make a request to the webserver and it took `0.5 seconds` to get the result back so we did it 20 times with multi threading and were able to receive the results in less time in a synchronous order.
+
+> Lets try to do it without multithreading and see how it affects the processing time.
+
+So in this new update `ejtraderTH v1.0` we can specify that at once how many threads should be created so lets change the input parameter as `max_threads = 1` this way it will only create one thread at a time and will wait until the previous thread has finished properly.
+
+#### output
+
+```python
+.
+.
+.
+>> Elapsed time: 6.43 sec
+```
+
+It is clear that every request to the server was taking approx. `0.5 seconds` so while making one request at a time it took `6.43 seconds` as expected.
+
+### Example 3
+
+Quick Launch mode, a new feature is added where you can directly use ejtraderTH to pass in the repetitive function, input data for those functions and how many threads you want it to create at a time. other than that if you just want it to repeat the function without any inputs you can do that too.
+
+```python
+import ejtraderTH
+import time
+import random
+
+names = ['April', 'May']
+
+#the function for processing data
+def my_func(data):
+    ejtraderTH.console_log(output=True)
+    time.sleep(1)
+    name = random.choice(names)
+    return f'{name} says, Hello World!'
+
+processed_data = ejtraderTH.start(my_func, repeat=4)
+
+print(processed_data)
+ejtraderTH.elapsed(output=True)
+```
+
+### output
+
+```
+>> Creating Threads 1
+>> Creating Threads 2
+>> Creating Threads 3
+>> Creating Threads 4
+['May says, Hello World!', 'April says, Hello World!', 'May says, Hello World!', 'April says, Hello World!']
+>> Elapsed time: 1.0 sec
+```
+
+we kept a time gap of 1 sec inside the function still it repeated the task 4 times in same time. since it can access the global variables we can assign certain tasks that don't need different inputs every time.
+
+### Decorators support
+
+Apart from calling the `start()` attribute we can also use decorators to explicitly make our functions for concurrent execution.
+
+**Example 1**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.run(repeat=5, max_threads=5)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+print(ejtraderTH.result['my_func'])
+```
+
+**Output**
+
+```python
+[0, 2, 4, 6, 8]
+```
+
+This will execute the function as soon as you run your python code, in this case we are trying to perform the same task five times in a row concurrently. The final output of all the function can be accessed by `ejtraderTH.result['function_name']`. Notice if you set your function on repeat it will always receive a parameter which is it's thread number.
+
+---
+
+**Example 2**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.run(data=[1,2,3,4,5,6], max_threads=5)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+print(ejtraderTH.result['my_func'])
+```
+
+**Output**
+
+```python
+[2, 4, 6, 8, 10, 12]
+```
+
+In this case we are directly passing our arguments in a list via decorator and receiving the result same way as we did in previous example.
+
+---
+
+**Exampe 3**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.set(max_threads=10)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+result = my_func(repeat=7)
+print(result)
+```
+
+**Output**
+
+```python
+[0, 2, 4, 6, 8, 10, 12]
+```
+
+This is an another cool way to first convert your function in concurrent function and then passing the argument as how many time you want to execute that function all in parallel.
+
+---
+
+**Example 4**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.set()
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+result = my_func([5,6,7])
+print(result)
+```
+
+**Output**
+
+```python
+[10, 12, 14]
+```
+
+Again we can also specify what arguments we want to pass to the function to process it concurrently. if in the `@ejtraderTH.set()` decorator you won't pass any `max_threads` argument `max_threads=10` will be set.
+
+#### Handling errors and killing all threads
+
+So, by default if any error occurs the threads will keep on running, in case if you want to ignore some errors but if you want to kill all the thread at once you can use `ejtraderTH.stop()` while handling errors.
+
+```python
+#the function for processing data
+def my_func(data):
+    thread_number = ejtraderTH.console_log(output=True)
+    try:
+        data = requests.get("http://httpbin.org/get")
+        return data
+    except Exception as e:
+        print(e) #printing other errors
+        #killing all active threads
+        ejtraderTH.stop() #use to kill all threads
+```
+
+if you don't use `ejtraderTH.stop()` function then the threads will keep on running and filling `None` in place of returned data. if you used the `ejtraderTH.stop()` it will kill all active threads immediately and will return the data that were processed by your function so far.
```

### Comparing `ejtraderTH-1.0.3/README.md` & `ejtraderTH-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,653 +1,675 @@
-00000000: 6060 6070 7974 686f 6e0d 0a70 6970 2069  ```python..pip i
-00000010: 6e73 7461 6c6c 2065 6a74 7261 6465 7254  nstall ejtraderT
-00000020: 480d 0a60 6060 0d0a 0d0a 5468 6973 2074  H..```....This t
-00000030: 696e 7920 6c69 7474 6c65 2070 7974 686f  iny little pytho
-00000040: 6e20 6d6f 6475 6c65 2069 7320 7573 6566  n module is usef
-00000050: 756c 2066 6f72 2063 7265 6174 696e 6720  ul for creating 
-00000060: 6d75 6c74 6970 6c65 2074 6872 6561 6473  multiple threads
-00000070: 206f 6620 616e 7920 6675 6e63 7469 6f6e   of any function
-00000080: 2069 6e20 7365 636f 6e64 732e 0d0a 0d0a   in seconds.....
-00000090: 2323 2323 2057 6861 7427 7320 6e65 7720  #### What's new 
-000000a0: 696e 2076 312e 300d 0a0d 0a41 2071 7569  in v1.0....A qui
-000000b0: 636b 206c 6175 6e63 6820 6d6f 6465 2069  ck launch mode i
-000000c0: 7320 6164 6465 642c 206a 7573 7420 7479  s added, just ty
-000000d0: 7065 2060 656a 7472 6164 6572 5448 2e73  pe `ejtraderTH.s
-000000e0: 7461 7274 2866 756e 635f 6e61 6d65 2c20  tart(func_name, 
-000000f0: 7265 7065 6174 3d31 3029 6020 616e 6420  repeat=10)` and 
-00000100: 6974 2077 696c 6c20 6578 6563 7574 6520  it will execute 
-00000110: 7468 6520 6769 7665 6e20 6675 6e63 7469  the given functi
-00000120: 6f6e 2067 6976 656e 206e 756d 6265 7220  on given number 
-00000130: 6f66 2074 696d 6573 2069 6e20 7061 7261  of times in para
-00000140: 6c6c 656c 2e20 4120 7374 616e 6461 7264  llel. A standard
-00000150: 2077 6179 206f 6620 6d65 6173 7572 696e   way of measurin
-00000160: 6720 656c 6170 7365 6420 7469 6d65 2069  g elapsed time i
-00000170: 7320 6164 6465 6420 6173 2077 656c 6c2e  s added as well.
-00000180: 2073 6565 2065 7861 6d70 6c65 7320 6265   see examples be
-00000190: 6c6f 7720 746f 2075 6e64 6572 7374 616e  low to understan
-000001a0: 6420 686f 7720 746f 2075 7365 2071 7569  d how to use qui
-000001b0: 636b 206c 6175 6e63 6820 6d6f 6465 2e0d  ck launch mode..
-000001c0: 0a0d 0a41 6674 6572 2075 7369 6e67 2074  ...After using t
-000001d0: 6869 7320 6c69 6272 6172 7920 666f 7220  his library for 
-000001e0: 6120 6e75 6d62 6572 206f 6620 7469 6d65  a number of time
-000001f0: 7320 696e 2076 6172 696f 7573 2070 726f  s in various pro
-00000200: 6a65 6374 7320 6920 666f 756e 6420 7468  jects i found th
-00000210: 6174 2069 6620 796f 7520 7061 7373 2069  at if you pass i
-00000220: 6e20 6c6f 7473 206f 6620 6461 7461 2073  n lots of data s
-00000230: 6179 2060 3130 3030 6020 6461 7461 2069  ay `1000` data i
-00000240: 6e20 6120 6c69 7374 2c20 6974 2077 6173  n a list, it was
-00000250: 2063 7265 6174 696e 6720 6031 3030 3060   creating `1000`
-00000260: 2074 6872 6561 6473 2074 6f20 646f 2069   threads to do i
-00000270: 7420 616c 6c20 6f6e 6365 2c20 686f 7720  t all once, how 
-00000280: 6576 6572 2069 6e20 7468 6520 7072 6163  ever in the prac
-00000290: 7469 6361 6c20 776f 726c 6420 6d6f 7374  tical world most
-000002a0: 206f 6620 7468 6520 7469 6d65 7320 6370   of the times cp
-000002b0: 7527 7320 6172 6520 6e6f 7420 6361 7061  u's are not capa
-000002c0: 626c 6520 6f66 2063 7265 6174 696e 6720  ble of creating 
-000002d0: 736f 206d 616e 7920 7468 7265 6164 7320  so many threads 
-000002e0: 6174 206f 6e63 6520 6f72 2077 6f72 7365  at once or worse
-000002f0: 2069 7420 6561 7473 2075 7020 616c 6c20   it eats up all 
-00000300: 7265 736f 7572 6365 7320 6174 206f 6e63  resources at onc
-00000310: 652e 2054 6f20 7072 6576 656e 7420 7468  e. To prevent th
-00000320: 6973 2070 726f 626c 656d 206e 6f77 2079  is problem now y
-00000330: 6f75 2063 616e 2070 6173 7320 696e 2060  ou can pass in `
-00000340: 6d61 785f 7468 7265 6164 7360 2076 616c  max_threads` val
-00000350: 7565 2062 7920 6465 6661 756c 7420 6966  ue by default if
-00000360: 2079 6f75 2064 6f6e 2774 2070 6173 7320   you don't pass 
-00000370: 696e 2074 6865 2076 616c 7565 2069 7420  in the value it 
-00000380: 7769 6c6c 2061 7574 6f6d 6174 6963 616c  will automatical
-00000390: 6c79 2062 6520 7365 7420 6571 7561 6c20  ly be set equal 
-000003a0: 746f 2034 206a 7573 7420 666f 7220 7468  to 4 just for th
-000003b0: 6520 7361 6665 7479 2070 7572 706f 7365  e safety purpose
-000003c0: 2c20 616e 6420 7061 7373 696e 6720 6120  , and passing a 
-000003d0: 6030 6020 7661 6c75 6520 7769 6c6c 2074  `0` value will t
-000003e0: 6872 6f77 2061 6e20 6572 726f 7220 7768  hrow an error wh
-000003f0: 696c 6520 6372 6561 7469 6e67 2061 2060  ile creating a `
-00000400: 656a 7472 6164 6572 5448 6020 6f62 6a65  ejtraderTH` obje
-00000410: 6374 2074 6869 7320 7761 7920 6974 2077  ct this way it w
-00000420: 696c 6c20 6f6e 6c79 2063 7265 6174 6520  ill only create 
-00000430: 7370 6563 6966 6965 6420 6e75 6d62 6572  specified number
-00000440: 206f 6620 7468 7265 6164 7320 6174 206f   of threads at o
-00000450: 6e63 6520 616e 6420 7769 6c6c 2077 6169  nce and will wai
-00000460: 7420 756e 7469 6c6c 2074 6865 2070 7265  t untill the pre
-00000470: 7669 6f75 736c 7920 7374 6172 7465 6420  viously started 
-00000480: 7468 7265 6164 7320 6861 7320 6669 6e69  threads has fini
-00000490: 7368 6564 2074 6865 6972 206a 6f62 2e0d  shed their job..
-000004a0: 0a0d 0a4f 7468 6572 2074 6861 6e20 7468  ...Other than th
-000004b0: 6174 2074 6f20 6b65 6570 2061 2074 7261  at to keep a tra
-000004c0: 636b 206f 6e20 686f 7720 6d61 6e79 2074  ck on how many t
-000004d0: 6872 6561 6473 2061 7265 2062 6565 6e20  hreads are been 
-000004e0: 6372 6561 7465 6420 696e 2072 6561 6c20  created in real 
-000004f0: 7469 6d65 2079 6f75 2063 616e 2070 7573  time you can pus
-00000500: 6820 696e 2061 206e 6577 206c 6f67 206d  h in a new log m
-00000510: 6574 686f 6420 696e 6e20 796f 7520 7072  ethod inn you pr
-00000520: 6f63 6573 7369 6e67 2066 756e 6374 696f  ocessing functio
-00000530: 6e20 736f 2074 6861 7420 7768 656e 6576  n so that whenev
-00000540: 6572 2061 206e 6577 2074 6872 6561 6420  er a new thread 
-00000550: 6973 2063 7265 6174 6564 2079 6f75 2063  is created you c
-00000560: 616e 2073 6565 2069 742c 2074 6865 7265  an see it, there
-00000570: 2061 7220 7477 6f20 6d65 7468 6f64 7320   ar two methods 
-00000580: 6f66 2074 7261 636b 696e 6720 7468 656d  of tracking them
-00000590: 2e0d 0a0d 0a2d 206a 7573 7420 746f 2070  .....- just to p
-000005a0: 7269 6e74 206f 7574 2074 6865 2074 6872  rint out the thr
-000005b0: 6561 6420 6e75 6d62 6572 2077 6869 6368  ead number which
-000005c0: 2069 7320 6265 696e 6720 6372 6561 7465   is being create
-000005d0: 642c 2075 7365 3a20 6020 656a 7472 6164  d, use: ` ejtrad
-000005e0: 6572 5448 2e63 6f6e 736f 6c65 5f6c 6f67  erTH.console_log
-000005f0: 286f 7574 7075 743d 5472 7565 2960 0d0a  (output=True)`..
-00000600: 2d20 6966 2079 6f75 2077 616e 7420 746f  - if you want to
-00000610: 2073 746f 7265 2069 7420 696e 2073 6f6d   store it in som
-00000620: 6520 7661 7269 6162 6c65 2079 6f75 2063  e variable you c
-00000630: 616e 2075 7365 3a20 6074 6872 6561 645f  an use: `thread_
-00000640: 6e75 6d62 6572 203d 2065 6a74 7261 6465  number = ejtrade
-00000650: 7254 482e 636f 6e73 6f6c 655f 6c6f 6728  rTH.console_log(
-00000660: 2960 0d0a 2d20 696e 2063 6173 6520 736f  )`..- in case so
-00000670: 6d65 2065 7272 6f72 206f 6363 7572 732c  me error occurs,
-00000680: 2074 6865 2074 6872 6561 6420 7769 6c6c   the thread will
-00000690: 206b 6565 7020 6f6e 2072 756e 6e69 6e67   keep on running
-000006a0: 0d0a 2d20 6966 2079 6f75 2077 616e 7420  ..- if you want 
-000006b0: 746f 206b 696c 6c20 616c 6c20 7468 6520  to kill all the 
-000006c0: 7468 7265 6164 7320 7573 6520 6065 6a74  threads use `ejt
-000006d0: 7261 6465 7254 482e 7374 6f70 2829 6020  raderTH.stop()` 
-000006e0: 696e 7369 6465 2079 6f75 7220 7072 6f63  inside your proc
-000006f0: 6573 7369 6e67 2066 756e 6374 696f 6e20  essing function 
-00000700: 7768 696c 6520 6861 6e64 6c69 6e67 2065  while handling e
-00000710: 7272 6f72 732e 0d0a 0d0a 2323 2323 2050  rrors.....#### P
-00000720: 726f 626c 656d 2053 7461 7465 6d65 6e74  roblem Statement
-00000730: 0d0a 0d0a 2d20 4c65 7420 7361 7920 666f  ....- Let say fo
-00000740: 7220 6578 616d 706c 652c 2077 6520 6861  r example, we ha
-00000750: 7665 2061 2060 6c69 7374 6020 6f66 206e  ve a `list` of n
-00000760: 756d 6265 7273 2066 726f 6d20 6031 2074  umbers from `1 t
-00000770: 6f20 3130 6020 616e 6420 616c 6c20 7765  o 10` and all we
-00000780: 2077 616e 7465 6420 746f 2064 6f20 6973   wanted to do is
-00000790: 2060 6d75 6c74 6970 6c79 2065 7665 7279   `multiply every
-000007a0: 206e 756d 6265 7220 6279 2031 3030 3060   number by 1000`
-000007b0: 2062 7574 2074 6865 2063 6861 6c6c 656e   but the challen
-000007c0: 6765 2069 7320 6069 7420 7461 6b65 7320  ge is `it takes 
-000007d0: 3520 7365 6360 2066 6f72 206d 756c 7469  5 sec` for multi
-000007e0: 706c 7969 6e67 2061 2073 696e 676c 6520  plying a single 
-000007f0: 6e75 6d62 6572 2062 7920 3130 3030 2066  number by 1000 f
-00000800: 726f 6d20 7468 6520 6c69 7374 2c20 4920  rom the list, I 
-00000810: 6b6e 6f77 2069 7473 2061 6e20 6172 6269  know its an arbi
-00000820: 7461 7279 2063 6f6e 6469 7469 6f6e 2c20  tary condition, 
-00000830: 6275 7420 7765 2063 616e 2063 7265 6174  but we can creat
-00000840: 6520 6974 2077 6974 6820 6074 696d 652e  e it with `time.
-00000850: 736c 6565 7028 3529 6020 6675 6e63 7469  sleep(5)` functi
-00000860: 6f6e 2e0d 0a2d 204f 7220 796f 7520 7761  on...- Or you wa
-00000870: 6e74 2074 6f20 6d61 6b65 2061 2077 6562  nt to make a web
-00000880: 2072 6571 7565 7374 206d 696c 6c69 6f6e   request million
-00000890: 2074 696d 6573 2c20 7769 7468 6f75 7420   times, without 
-000008a0: 7761 6974 696e 6720 666f 7220 7468 6520  waiting for the 
-000008b0: 7365 7276 6572 2074 6f20 7265 7370 6f6e  server to respon
-000008c0: 6420 796f 7520 746f 206d 616b 6520 7468  d you to make th
-000008d0: 6520 6e65 7874 2072 6571 7565 7374 2e0d  e next request..
-000008e0: 0a0d 0a23 2323 2320 576f 726b 696e 670d  ...#### Working.
-000008f0: 0a0d 0a53 6f20 7768 6174 2074 6869 7320  ...So what this 
-00000900: 6d6f 6475 6c65 2064 6f65 7320 6973 2c20  module does is, 
-00000910: 6174 2074 6865 2074 696d 6520 6f66 206f  at the time of o
-00000920: 626a 6563 7420 696e 6974 6961 6c69 7a61  bject initializa
-00000930: 7469 6f6e 2069 7420 7461 6b65 7320 696e  tion it takes in
-00000940: 2074 6865 2066 756e 6374 696f 6e20 7768   the function wh
-00000950: 6963 6820 6973 2075 7365 6420 666f 7220  ich is used for 
-00000960: 7072 6f63 6573 7369 6e67 2064 6174 6120  processing data 
-00000970: 616e 6420 6d61 7820 6e75 6d62 6572 206f  and max number o
-00000980: 6620 7468 7265 6164 2077 6869 6368 2063  f thread which c
-00000990: 616e 2062 6520 6372 6561 7465 6420 6174  an be created at
-000009a0: 206f 6e63 652c 2077 6865 6e20 7275 6e6e   once, when runn
-000009b0: 696e 6720 696e 206d 756c 7469 2074 6872  ing in multi thr
-000009c0: 6561 6473 2c20 616e 6420 6173 2069 6e70  eads, and as inp
-000009d0: 7574 2069 7420 7461 6b65 7320 6120 6c69  ut it takes a li
-000009e0: 7374 206f 6620 6172 6775 6d65 6e74 7320  st of arguments 
-000009f0: 666f 7220 7768 6963 6820 6d75 6c74 6970  for which multip
-00000a00: 6c65 2074 6872 6561 6473 2077 696c 6c20  le threads will 
-00000a10: 6265 2063 7265 6174 6564 2e0d 0a0d 0a2d  be created.....-
-00000a20: 2d2d 0d0a 0d0a 2323 2323 2045 7861 6d70  --....#### Examp
-00000a30: 6c65 2031 0d0a 0d0a 6060 6070 7974 686f  le 1....```pytho
-00000a40: 6e0d 0a69 6d70 6f72 7420 656a 7472 6164  n..import ejtrad
-00000a50: 6572 5448 0d0a 696d 706f 7274 2074 696d  erTH..import tim
-00000a60: 650d 0a0d 0a23 7468 6520 6675 6e63 7469  e....#the functi
-00000a70: 6f6e 2066 6f72 2070 726f 6365 7373 696e  on for processin
-00000a80: 6720 6461 7461 0d0a 6465 6620 6d79 5f66  g data..def my_f
-00000a90: 756e 6328 6461 7461 293a 0d0a 2020 2020  unc(data):..    
-00000aa0: 7072 696e 7428 6627 3e3e 2052 756e 6e69  print(f'>> Runni
-00000ab0: 6e67 2054 6872 6561 6420 7b65 6a74 7261  ng Thread {ejtra
-00000ac0: 6465 7254 482e 636f 6e73 6f6c 655f 6c6f  derTH.console_lo
-00000ad0: 6728 297d 2729 0d0a 2020 2020 6461 7461  g()}')..    data
-00000ae0: 203d 2064 6174 612a 3130 3030 0d0a 2020   = data*1000..  
-00000af0: 2020 7469 6d65 2e73 6c65 6570 2835 290d    time.sleep(5).
-00000b00: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-00000b10: 0d0a 0d0a 236c 6973 7420 6f66 2069 6e70  ....#list of inp
-00000b20: 7574 2064 6174 6120 666f 7220 7072 6f63  ut data for proc
-00000b30: 6573 7369 6e67 0d0a 7261 775f 6461 7461  essing..raw_data
-00000b40: 203d 205b 312c 322c 332c 342c 352c 362c   = [1,2,3,4,5,6,
-00000b50: 372c 382c 392c 3130 5d0d 0a0d 0a23 7365  7,8,9,10]....#se
-00000b60: 6e64 696e 6720 6172 6775 6d65 6e74 7320  nding arguments 
-00000b70: 666f 7220 6173 796e 6368 726f 6e6f 7573  for asynchronous
-00000b80: 206d 756c 7469 2074 6872 6561 6420 7072   multi thread pr
-00000b90: 6f63 6573 7369 6e67 0d0a 7072 6f63 6573  ocessing..proces
-00000ba0: 7365 645f 6461 7461 203d 2065 6a74 7261  sed_data = ejtra
-00000bb0: 6465 7254 482e 7374 6172 7428 6d79 5f66  derTH.start(my_f
-00000bc0: 756e 632c 2064 6174 613d 7261 775f 6461  unc, data=raw_da
-00000bd0: 7461 2c20 6d61 785f 7468 7265 6164 733d  ta, max_threads=
-00000be0: 3130 290d 0a0d 0a23 7072 696e 7469 6e67  10)....#printing
-00000bf0: 2074 6865 2073 796e 6368 726f 6e69 7365   the synchronise
-00000c00: 6420 7265 6365 6976 6564 2072 6573 756c  d received resul
-00000c10: 7473 0d0a 7072 696e 7428 290d 0a70 7269  ts..print()..pri
-00000c20: 6e74 2866 273e 3e20 496e 7075 743a 207b  nt(f'>> Input: {
-00000c30: 7261 775f 6461 7461 7d27 290d 0a70 7269  raw_data}')..pri
-00000c40: 6e74 2866 273e 3e20 5265 7375 6c74 3a20  nt(f'>> Result: 
-00000c50: 7b70 726f 6365 7373 6564 5f64 6174 617d  {processed_data}
-00000c60: 2729 0d0a 7072 696e 7428 6627 3e3e 2045  ')..print(f'>> E
-00000c70: 6c61 7073 6564 2074 696d 653a 207b 656a  lapsed time: {ej
-00000c80: 7472 6164 6572 5448 2e65 6c61 7073 6564  traderTH.elapsed
-00000c90: 2829 7d20 7365 6327 290d 0a60 6060 0d0a  ()} sec')..```..
-00000ca0: 0d0a 2323 2323 206f 7574 7075 740d 0a0d  ..#### output...
-00000cb0: 0a60 6060 7079 7468 6f6e 0d0a 3e3e 2052  .```python..>> R
-00000cc0: 756e 6e69 6e67 2054 6872 6561 6420 310d  unning Thread 1.
-00000cd0: 0a3e 3e20 5275 6e6e 696e 6720 5468 7265  .>> Running Thre
-00000ce0: 6164 2032 0d0a 3e3e 2052 756e 6e69 6e67  ad 2..>> Running
-00000cf0: 2054 6872 6561 6420 330d 0a3e 3e20 5275   Thread 3..>> Ru
-00000d00: 6e6e 696e 6720 5468 7265 6164 2034 0d0a  nning Thread 4..
-00000d10: 3e3e 2052 756e 6e69 6e67 2054 6872 6561  >> Running Threa
-00000d20: 6420 350d 0a3e 3e20 5275 6e6e 696e 6720  d 5..>> Running 
-00000d30: 5468 7265 6164 2036 0d0a 3e3e 2052 756e  Thread 6..>> Run
-00000d40: 6e69 6e67 2054 6872 6561 6420 370d 0a3e  ning Thread 7..>
-00000d50: 3e20 5275 6e6e 696e 6720 5468 7265 6164  > Running Thread
-00000d60: 2038 0d0a 3e3e 2052 756e 6e69 6e67 2054   8..>> Running T
-00000d70: 6872 6561 6420 390d 0a3e 3e20 5275 6e6e  hread 9..>> Runn
-00000d80: 696e 6720 5468 7265 6164 2031 300d 0a0d  ing Thread 10...
-00000d90: 0a3e 3e20 496e 7075 743a 205b 312c 2032  .>> Input: [1, 2
-00000da0: 2c20 332c 2034 2c20 352c 2036 2c20 372c  , 3, 4, 5, 6, 7,
-00000db0: 2038 2c20 392c 2031 305d 0d0a 3e3e 2052   8, 9, 10]..>> R
-00000dc0: 6573 756c 743a 205b 3130 3030 2c20 3230  esult: [1000, 20
-00000dd0: 3030 2c20 3330 3030 2c20 3430 3030 2c20  00, 3000, 4000, 
-00000de0: 3530 3030 2c20 3630 3030 2c20 3730 3030  5000, 6000, 7000
-00000df0: 2c20 3830 3030 2c20 3930 3030 2c20 3130  , 8000, 9000, 10
-00000e00: 3030 305d 0d0a 3e3e 2045 6c61 7073 6564  000]..>> Elapsed
-00000e10: 2074 696d 653a 2035 2e30 2073 6563 0d0a   time: 5.0 sec..
-00000e20: 6060 600d 0a0d 0a4e 6f77 2079 6f75 2063  ```....Now you c
-00000e30: 616e 2063 6c65 6172 6c79 2073 6565 2c20  an clearly see, 
-00000e40: 6966 2077 6520 646f 2069 7420 7769 7468  if we do it with
-00000e50: 6f75 7420 6d75 6c74 6920 7468 7265 6164  out multi thread
-00000e60: 696e 6720 6974 2077 6f75 6c64 2068 6176  ing it would hav
-00000e70: 6520 7461 6b65 6e20 6172 6f75 6e64 2060  e taken around `
-00000e80: 3530 2053 6563 6f6e 6473 6020 666f 7220  50 Seconds` for 
-00000e90: 7072 6f63 6573 7369 6e67 2074 6865 2064  processing the d
-00000ea0: 6174 6120 7768 696c 6520 646f 696e 6720  ata while doing 
-00000eb0: 7468 6520 7461 736b 206f 6e65 2062 7920  the task one by 
-00000ec0: 6f6e 6520 616e 6420 7761 6974 696e 6720  one and waiting 
-00000ed0: 666f 7220 6035 2053 6563 6020 6166 7465  for `5 Sec` afte
-00000ee0: 7220 7275 6e6e 696e 6720 7468 6520 6675  r running the fu
-00000ef0: 6e63 7469 6f6e 2065 6163 6820 7469 6d65  nction each time
-00000f00: 2e20 6275 7420 7369 6e63 6520 7765 2061  . but since we a
-00000f10: 7265 2064 6f69 6e67 2069 7420 7769 7468  re doing it with
-00000f20: 206d 756c 7469 7468 7265 6164 696e 6720   multithreading 
-00000f30: 6974 2077 696c 6c20 7461 6b65 206f 6e6c  it will take onl
-00000f40: 7920 6035 2053 6563 6f6e 6473 6020 666f  y `5 Seconds` fo
-00000f50: 7220 7072 6f63 6573 7369 6e67 2074 6865  r processing the
-00000f60: 2073 616d 6520 7461 736b 2077 6974 6820   same task with 
-00000f70: 6469 6666 6572 656e 7420 6461 7461 2c20  different data, 
-00000f80: 696e 2074 6865 6972 2069 6e64 6976 6964  in their individ
-00000f90: 7561 6c20 7468 7265 6164 732e 0d0a 0d0a  ual threads.....
-00000fa0: 2323 2323 2045 7861 6d70 6c65 2032 0d0a  #### Example 2..
-00000fb0: 0d0a 6060 6070 7974 686f 6e0d 0a23 7468  ..```python..#th
-00000fc0: 6520 6675 6e63 7469 6f6e 2066 6f72 2070  e function for p
-00000fd0: 726f 6365 7373 696e 6720 6461 7461 0d0a  rocessing data..
-00000fe0: 6465 6620 6d79 5f66 756e 6328 6461 7461  def my_func(data
-00000ff0: 293a 0d0a 2020 2020 656a 7472 6164 6572  ):..    ejtrader
-00001000: 5448 2e63 6f6e 736f 6c65 5f6c 6f67 286f  TH.console_log(o
-00001010: 7574 7075 743d 5472 7565 290d 0a20 2020  utput=True)..   
-00001020: 2069 7020 3d20 7265 712e 7265 7175 6573   ip = req.reques
-00001030: 7428 6d65 7468 6f64 3d27 4745 5427 2c75  t(method='GET',u
-00001040: 726c 3d22 6874 7470 3a2f 2f69 7069 6e66  rl="http://ipinf
-00001050: 6f2e 696f 2f69 7022 290d 0a0d 0a20 2020  o.io/ip")....   
-00001060: 2072 6574 7572 6e20 6970 2e63 6f6e 7465   return ip.conte
-00001070: 6e74 0d0a 0d0a 2373 656e 6469 6e67 2061  nt....#sending a
-00001080: 7267 756d 656e 7473 2066 6f72 2061 7379  rguments for asy
-00001090: 6e63 6872 6f6e 6f75 7320 6d75 6c74 6920  nchronous multi 
-000010a0: 7468 7265 6164 2070 726f 6365 7373 696e  thread processin
-000010b0: 670d 0a70 726f 6365 7373 6564 5f64 6174  g..processed_dat
-000010c0: 6120 3d20 656a 7472 6164 6572 5448 2e73  a = ejtraderTH.s
-000010d0: 7461 7274 286d 795f 6675 6e63 2c20 7265  tart(my_func, re
-000010e0: 7065 6174 3d32 302c 206d 6178 5f74 6872  peat=20, max_thr
-000010f0: 6561 6473 3d32 3029 0d0a 0d0a 2370 7269  eads=20)....#pri
-00001100: 6e74 696e 6720 7468 6520 7379 6e63 6872  nting the synchr
-00001110: 6f6e 6973 6564 2072 6563 6569 7665 6420  onised received 
-00001120: 7265 7375 6c74 730d 0a70 7269 6e74 2829  results..print()
-00001130: 0d0a 7072 696e 7428 6627 3e3e 2052 6573  ..print(f'>> Res
-00001140: 756c 743a 207b 7072 6f63 6573 7365 645f  ult: {processed_
-00001150: 6461 7461 7d27 290d 0a65 6a74 7261 6465  data}')..ejtrade
-00001160: 7254 482e 656c 6170 7365 6428 6f75 7470  rTH.elapsed(outp
-00001170: 7574 3d54 7275 6529 0d0a 6060 600d 0a0d  ut=True)..```...
-00001180: 0a23 2323 2320 6f75 7470 7574 0d0a 0d0a  .#### output....
-00001190: 6060 6070 7974 686f 6e0d 0a3e 3e20 4372  ```python..>> Cr
-000011a0: 6561 7469 6e67 2054 6872 6561 6473 2031  eating Threads 1
-000011b0: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-000011c0: 7265 6164 7320 320d 0a3e 3e20 4372 6561  reads 2..>> Crea
-000011d0: 7469 6e67 2054 6872 6561 6473 2033 0d0a  ting Threads 3..
-000011e0: 3e3e 2043 7265 6174 696e 6720 5468 7265  >> Creating Thre
-000011f0: 6164 7320 340d 0a3e 3e20 4372 6561 7469  ads 4..>> Creati
-00001200: 6e67 2054 6872 6561 6473 2035 0d0a 3e3e  ng Threads 5..>>
-00001210: 2043 7265 6174 696e 6720 5468 7265 6164   Creating Thread
-00001220: 7320 360d 0a3e 3e20 4372 6561 7469 6e67  s 6..>> Creating
-00001230: 2054 6872 6561 6473 2037 0d0a 3e3e 2043   Threads 7..>> C
-00001240: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
-00001250: 380d 0a3e 3e20 4372 6561 7469 6e67 2054  8..>> Creating T
-00001260: 6872 6561 6473 2039 0d0a 3e3e 2043 7265  hreads 9..>> Cre
-00001270: 6174 696e 6720 5468 7265 6164 7320 3130  ating Threads 10
-00001280: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-00001290: 7265 6164 7320 3131 0d0a 3e3e 2043 7265  reads 11..>> Cre
-000012a0: 6174 696e 6720 5468 7265 6164 7320 3132  ating Threads 12
-000012b0: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-000012c0: 7265 6164 7320 3133 0d0a 3e3e 2043 7265  reads 13..>> Cre
-000012d0: 6174 696e 6720 5468 7265 6164 7320 3134  ating Threads 14
-000012e0: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-000012f0: 7265 6164 7320 3135 0d0a 3e3e 2043 7265  reads 15..>> Cre
-00001300: 6174 696e 6720 5468 7265 6164 7320 3136  ating Threads 16
-00001310: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-00001320: 7265 6164 7320 3137 0d0a 3e3e 2043 7265  reads 17..>> Cre
-00001330: 6174 696e 6720 5468 7265 6164 7320 3138  ating Threads 18
+00000000: 0d0a 215b 5079 7069 2050 7562 6c69 7368  ..![Pypi Publish
+00000010: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000020: 2e63 6f6d 2f65 6a74 7261 6465 724c 6162  .com/ejtraderLab
+00000030: 732f 656a 7472 6164 6572 5448 2f61 6374  s/ejtraderTH/act
+00000040: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00000050: 7974 686f 6e2d 7075 626c 6973 682e 796d  ython-publish.ym
+00000060: 6c2f 6261 6467 652e 7376 6729 0d0a 215b  l/badge.svg)..![
+00000070: 4769 7448 7562 2072 656c 6561 7365 2028  GitHub release (
+00000080: 6c61 7465 7374 2062 7920 6461 7465 295d  latest by date)]
+00000090: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000000a0: 656c 6473 2e69 6f2f 6769 7468 7562 2f76  elds.io/github/v
+000000b0: 2f72 656c 6561 7365 2f65 6a74 7261 6465  /release/ejtrade
+000000c0: 724c 6162 732f 656a 7472 6164 6572 5448  rLabs/ejtraderTH
+000000d0: 290d 0a5b 215b 4c69 6365 6e73 655d 2868  )..[![License](h
+000000e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000f0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+00000100: 656e 7365 2f65 6a74 7261 6465 724c 6162  ense/ejtraderLab
+00000110: 732f 656a 7472 6164 6572 5448 295d 2868  s/ejtraderTH)](h
+00000120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000130: 6d2f 656a 7472 6164 6572 4c61 6273 2f65  m/ejtraderLabs/e
+00000140: 6a74 7261 6465 7254 482f 626c 6f62 2f6d  jtraderTH/blob/m
+00000150: 6173 7465 722f 4c49 4345 4e53 4529 0d0a  aster/LICENSE)..
+00000160: 0d0a 6060 6070 7974 686f 6e0d 0a70 6970  ..```python..pip
+00000170: 2069 6e73 7461 6c6c 2065 6a74 7261 6465   install ejtrade
+00000180: 7254 480d 0a60 6060 0d0a 0d0a 5468 6973  rTH..```....This
+00000190: 2074 696e 7920 6c69 7474 6c65 2070 7974   tiny little pyt
+000001a0: 686f 6e20 6d6f 6475 6c65 2069 7320 7573  hon module is us
+000001b0: 6566 756c 2066 6f72 2063 7265 6174 696e  eful for creatin
+000001c0: 6720 6d75 6c74 6970 6c65 2074 6872 6561  g multiple threa
+000001d0: 6473 206f 6620 616e 7920 6675 6e63 7469  ds of any functi
+000001e0: 6f6e 2069 6e20 7365 636f 6e64 732e 0d0a  on in seconds...
+000001f0: 0d0a 2323 2323 2057 6861 7427 7320 6e65  ..#### What's ne
+00000200: 7720 696e 2076 312e 300d 0a0d 0a41 2071  w in v1.0....A q
+00000210: 7569 636b 206c 6175 6e63 6820 6d6f 6465  uick launch mode
+00000220: 2069 7320 6164 6465 642c 206a 7573 7420   is added, just 
+00000230: 7479 7065 2060 656a 7472 6164 6572 5448  type `ejtraderTH
+00000240: 2e73 7461 7274 2866 756e 635f 6e61 6d65  .start(func_name
+00000250: 2c20 7265 7065 6174 3d31 3029 6020 616e  , repeat=10)` an
+00000260: 6420 6974 2077 696c 6c20 6578 6563 7574  d it will execut
+00000270: 6520 7468 6520 6769 7665 6e20 6675 6e63  e the given func
+00000280: 7469 6f6e 2067 6976 656e 206e 756d 6265  tion given numbe
+00000290: 7220 6f66 2074 696d 6573 2069 6e20 7061  r of times in pa
+000002a0: 7261 6c6c 656c 2e20 4120 7374 616e 6461  rallel. A standa
+000002b0: 7264 2077 6179 206f 6620 6d65 6173 7572  rd way of measur
+000002c0: 696e 6720 656c 6170 7365 6420 7469 6d65  ing elapsed time
+000002d0: 2069 7320 6164 6465 6420 6173 2077 656c   is added as wel
+000002e0: 6c2e 2073 6565 2065 7861 6d70 6c65 7320  l. see examples 
+000002f0: 6265 6c6f 7720 746f 2075 6e64 6572 7374  below to underst
+00000300: 616e 6420 686f 7720 746f 2075 7365 2071  and how to use q
+00000310: 7569 636b 206c 6175 6e63 6820 6d6f 6465  uick launch mode
+00000320: 2e0d 0a0d 0a41 6674 6572 2075 7369 6e67  .....After using
+00000330: 2074 6869 7320 6c69 6272 6172 7920 666f   this library fo
+00000340: 7220 6120 6e75 6d62 6572 206f 6620 7469  r a number of ti
+00000350: 6d65 7320 696e 2076 6172 696f 7573 2070  mes in various p
+00000360: 726f 6a65 6374 7320 6920 666f 756e 6420  rojects i found 
+00000370: 7468 6174 2069 6620 796f 7520 7061 7373  that if you pass
+00000380: 2069 6e20 6c6f 7473 206f 6620 6461 7461   in lots of data
+00000390: 2073 6179 2060 3130 3030 6020 6461 7461   say `1000` data
+000003a0: 2069 6e20 6120 6c69 7374 2c20 6974 2077   in a list, it w
+000003b0: 6173 2063 7265 6174 696e 6720 6031 3030  as creating `100
+000003c0: 3060 2074 6872 6561 6473 2074 6f20 646f  0` threads to do
+000003d0: 2069 7420 616c 6c20 6f6e 6365 2c20 686f   it all once, ho
+000003e0: 7720 6576 6572 2069 6e20 7468 6520 7072  w ever in the pr
+000003f0: 6163 7469 6361 6c20 776f 726c 6420 6d6f  actical world mo
+00000400: 7374 206f 6620 7468 6520 7469 6d65 7320  st of the times 
+00000410: 6370 7527 7320 6172 6520 6e6f 7420 6361  cpu's are not ca
+00000420: 7061 626c 6520 6f66 2063 7265 6174 696e  pable of creatin
+00000430: 6720 736f 206d 616e 7920 7468 7265 6164  g so many thread
+00000440: 7320 6174 206f 6e63 6520 6f72 2077 6f72  s at once or wor
+00000450: 7365 2069 7420 6561 7473 2075 7020 616c  se it eats up al
+00000460: 6c20 7265 736f 7572 6365 7320 6174 206f  l resources at o
+00000470: 6e63 652e 2054 6f20 7072 6576 656e 7420  nce. To prevent 
+00000480: 7468 6973 2070 726f 626c 656d 206e 6f77  this problem now
+00000490: 2079 6f75 2063 616e 2070 6173 7320 696e   you can pass in
+000004a0: 2060 6d61 785f 7468 7265 6164 7360 2076   `max_threads` v
+000004b0: 616c 7565 2062 7920 6465 6661 756c 7420  alue by default 
+000004c0: 6966 2079 6f75 2064 6f6e 2774 2070 6173  if you don't pas
+000004d0: 7320 696e 2074 6865 2076 616c 7565 2069  s in the value i
+000004e0: 7420 7769 6c6c 2061 7574 6f6d 6174 6963  t will automatic
+000004f0: 616c 6c79 2062 6520 7365 7420 6571 7561  ally be set equa
+00000500: 6c20 746f 2034 206a 7573 7420 666f 7220  l to 4 just for 
+00000510: 7468 6520 7361 6665 7479 2070 7572 706f  the safety purpo
+00000520: 7365 2c20 616e 6420 7061 7373 696e 6720  se, and passing 
+00000530: 6120 6030 6020 7661 6c75 6520 7769 6c6c  a `0` value will
+00000540: 2074 6872 6f77 2061 6e20 6572 726f 7220   throw an error 
+00000550: 7768 696c 6520 6372 6561 7469 6e67 2061  while creating a
+00000560: 2060 656a 7472 6164 6572 5448 6020 6f62   `ejtraderTH` ob
+00000570: 6a65 6374 2074 6869 7320 7761 7920 6974  ject this way it
+00000580: 2077 696c 6c20 6f6e 6c79 2063 7265 6174   will only creat
+00000590: 6520 7370 6563 6966 6965 6420 6e75 6d62  e specified numb
+000005a0: 6572 206f 6620 7468 7265 6164 7320 6174  er of threads at
+000005b0: 206f 6e63 6520 616e 6420 7769 6c6c 2077   once and will w
+000005c0: 6169 7420 756e 7469 6c6c 2074 6865 2070  ait untill the p
+000005d0: 7265 7669 6f75 736c 7920 7374 6172 7465  reviously starte
+000005e0: 6420 7468 7265 6164 7320 6861 7320 6669  d threads has fi
+000005f0: 6e69 7368 6564 2074 6865 6972 206a 6f62  nished their job
+00000600: 2e0d 0a0d 0a4f 7468 6572 2074 6861 6e20  .....Other than 
+00000610: 7468 6174 2074 6f20 6b65 6570 2061 2074  that to keep a t
+00000620: 7261 636b 206f 6e20 686f 7720 6d61 6e79  rack on how many
+00000630: 2074 6872 6561 6473 2061 7265 2062 6565   threads are bee
+00000640: 6e20 6372 6561 7465 6420 696e 2072 6561  n created in rea
+00000650: 6c20 7469 6d65 2079 6f75 2063 616e 2070  l time you can p
+00000660: 7573 6820 696e 2061 206e 6577 206c 6f67  ush in a new log
+00000670: 206d 6574 686f 6420 696e 6e20 796f 7520   method inn you 
+00000680: 7072 6f63 6573 7369 6e67 2066 756e 6374  processing funct
+00000690: 696f 6e20 736f 2074 6861 7420 7768 656e  ion so that when
+000006a0: 6576 6572 2061 206e 6577 2074 6872 6561  ever a new threa
+000006b0: 6420 6973 2063 7265 6174 6564 2079 6f75  d is created you
+000006c0: 2063 616e 2073 6565 2069 742c 2074 6865   can see it, the
+000006d0: 7265 2061 7220 7477 6f20 6d65 7468 6f64  re ar two method
+000006e0: 7320 6f66 2074 7261 636b 696e 6720 7468  s of tracking th
+000006f0: 656d 2e0d 0a0d 0a2d 206a 7573 7420 746f  em.....- just to
+00000700: 2070 7269 6e74 206f 7574 2074 6865 2074   print out the t
+00000710: 6872 6561 6420 6e75 6d62 6572 2077 6869  hread number whi
+00000720: 6368 2069 7320 6265 696e 6720 6372 6561  ch is being crea
+00000730: 7465 642c 2075 7365 3a20 6020 656a 7472  ted, use: ` ejtr
+00000740: 6164 6572 5448 2e63 6f6e 736f 6c65 5f6c  aderTH.console_l
+00000750: 6f67 286f 7574 7075 743d 5472 7565 2960  og(output=True)`
+00000760: 0d0a 2d20 6966 2079 6f75 2077 616e 7420  ..- if you want 
+00000770: 746f 2073 746f 7265 2069 7420 696e 2073  to store it in s
+00000780: 6f6d 6520 7661 7269 6162 6c65 2079 6f75  ome variable you
+00000790: 2063 616e 2075 7365 3a20 6074 6872 6561   can use: `threa
+000007a0: 645f 6e75 6d62 6572 203d 2065 6a74 7261  d_number = ejtra
+000007b0: 6465 7254 482e 636f 6e73 6f6c 655f 6c6f  derTH.console_lo
+000007c0: 6728 2960 0d0a 2d20 696e 2063 6173 6520  g()`..- in case 
+000007d0: 736f 6d65 2065 7272 6f72 206f 6363 7572  some error occur
+000007e0: 732c 2074 6865 2074 6872 6561 6420 7769  s, the thread wi
+000007f0: 6c6c 206b 6565 7020 6f6e 2072 756e 6e69  ll keep on runni
+00000800: 6e67 0d0a 2d20 6966 2079 6f75 2077 616e  ng..- if you wan
+00000810: 7420 746f 206b 696c 6c20 616c 6c20 7468  t to kill all th
+00000820: 6520 7468 7265 6164 7320 7573 6520 6065  e threads use `e
+00000830: 6a74 7261 6465 7254 482e 7374 6f70 2829  jtraderTH.stop()
+00000840: 6020 696e 7369 6465 2079 6f75 7220 7072  ` inside your pr
+00000850: 6f63 6573 7369 6e67 2066 756e 6374 696f  ocessing functio
+00000860: 6e20 7768 696c 6520 6861 6e64 6c69 6e67  n while handling
+00000870: 2065 7272 6f72 732e 0d0a 0d0a 2323 2323   errors.....####
+00000880: 2050 726f 626c 656d 2053 7461 7465 6d65   Problem Stateme
+00000890: 6e74 0d0a 0d0a 2d20 4c65 7420 7361 7920  nt....- Let say 
+000008a0: 666f 7220 6578 616d 706c 652c 2077 6520  for example, we 
+000008b0: 6861 7665 2061 2060 6c69 7374 6020 6f66  have a `list` of
+000008c0: 206e 756d 6265 7273 2066 726f 6d20 6031   numbers from `1
+000008d0: 2074 6f20 3130 6020 616e 6420 616c 6c20   to 10` and all 
+000008e0: 7765 2077 616e 7465 6420 746f 2064 6f20  we wanted to do 
+000008f0: 6973 2060 6d75 6c74 6970 6c79 2065 7665  is `multiply eve
+00000900: 7279 206e 756d 6265 7220 6279 2031 3030  ry number by 100
+00000910: 3060 2062 7574 2074 6865 2063 6861 6c6c  0` but the chall
+00000920: 656e 6765 2069 7320 6069 7420 7461 6b65  enge is `it take
+00000930: 7320 3520 7365 6360 2066 6f72 206d 756c  s 5 sec` for mul
+00000940: 7469 706c 7969 6e67 2061 2073 696e 676c  tiplying a singl
+00000950: 6520 6e75 6d62 6572 2062 7920 3130 3030  e number by 1000
+00000960: 2066 726f 6d20 7468 6520 6c69 7374 2c20   from the list, 
+00000970: 4920 6b6e 6f77 2069 7473 2061 6e20 6172  I know its an ar
+00000980: 6269 7461 7279 2063 6f6e 6469 7469 6f6e  bitary condition
+00000990: 2c20 6275 7420 7765 2063 616e 2063 7265  , but we can cre
+000009a0: 6174 6520 6974 2077 6974 6820 6074 696d  ate it with `tim
+000009b0: 652e 736c 6565 7028 3529 6020 6675 6e63  e.sleep(5)` func
+000009c0: 7469 6f6e 2e0d 0a2d 204f 7220 796f 7520  tion...- Or you 
+000009d0: 7761 6e74 2074 6f20 6d61 6b65 2061 2077  want to make a w
+000009e0: 6562 2072 6571 7565 7374 206d 696c 6c69  eb request milli
+000009f0: 6f6e 2074 696d 6573 2c20 7769 7468 6f75  on times, withou
+00000a00: 7420 7761 6974 696e 6720 666f 7220 7468  t waiting for th
+00000a10: 6520 7365 7276 6572 2074 6f20 7265 7370  e server to resp
+00000a20: 6f6e 6420 796f 7520 746f 206d 616b 6520  ond you to make 
+00000a30: 7468 6520 6e65 7874 2072 6571 7565 7374  the next request
+00000a40: 2e0d 0a0d 0a23 2323 2320 576f 726b 696e  .....#### Workin
+00000a50: 670d 0a0d 0a53 6f20 7768 6174 2074 6869  g....So what thi
+00000a60: 7320 6d6f 6475 6c65 2064 6f65 7320 6973  s module does is
+00000a70: 2c20 6174 2074 6865 2074 696d 6520 6f66  , at the time of
+00000a80: 206f 626a 6563 7420 696e 6974 6961 6c69   object initiali
+00000a90: 7a61 7469 6f6e 2069 7420 7461 6b65 7320  zation it takes 
+00000aa0: 696e 2074 6865 2066 756e 6374 696f 6e20  in the function 
+00000ab0: 7768 6963 6820 6973 2075 7365 6420 666f  which is used fo
+00000ac0: 7220 7072 6f63 6573 7369 6e67 2064 6174  r processing dat
+00000ad0: 6120 616e 6420 6d61 7820 6e75 6d62 6572  a and max number
+00000ae0: 206f 6620 7468 7265 6164 2077 6869 6368   of thread which
+00000af0: 2063 616e 2062 6520 6372 6561 7465 6420   can be created 
+00000b00: 6174 206f 6e63 652c 2077 6865 6e20 7275  at once, when ru
+00000b10: 6e6e 696e 6720 696e 206d 756c 7469 2074  nning in multi t
+00000b20: 6872 6561 6473 2c20 616e 6420 6173 2069  hreads, and as i
+00000b30: 6e70 7574 2069 7420 7461 6b65 7320 6120  nput it takes a 
+00000b40: 6c69 7374 206f 6620 6172 6775 6d65 6e74  list of argument
+00000b50: 7320 666f 7220 7768 6963 6820 6d75 6c74  s for which mult
+00000b60: 6970 6c65 2074 6872 6561 6473 2077 696c  iple threads wil
+00000b70: 6c20 6265 2063 7265 6174 6564 2e0d 0a0d  l be created....
+00000b80: 0a2d 2d2d 0d0a 0d0a 2323 2323 2045 7861  .---....#### Exa
+00000b90: 6d70 6c65 2031 0d0a 0d0a 6060 6070 7974  mple 1....```pyt
+00000ba0: 686f 6e0d 0a69 6d70 6f72 7420 656a 7472  hon..import ejtr
+00000bb0: 6164 6572 5448 0d0a 696d 706f 7274 2074  aderTH..import t
+00000bc0: 696d 650d 0a0d 0a23 7468 6520 6675 6e63  ime....#the func
+00000bd0: 7469 6f6e 2066 6f72 2070 726f 6365 7373  tion for process
+00000be0: 696e 6720 6461 7461 0d0a 6465 6620 6d79  ing data..def my
+00000bf0: 5f66 756e 6328 6461 7461 293a 0d0a 2020  _func(data):..  
+00000c00: 2020 7072 696e 7428 6627 3e3e 2052 756e    print(f'>> Run
+00000c10: 6e69 6e67 2054 6872 6561 6420 7b65 6a74  ning Thread {ejt
+00000c20: 7261 6465 7254 482e 636f 6e73 6f6c 655f  raderTH.console_
+00000c30: 6c6f 6728 297d 2729 0d0a 2020 2020 6461  log()}')..    da
+00000c40: 7461 203d 2064 6174 612a 3130 3030 0d0a  ta = data*1000..
+00000c50: 2020 2020 7469 6d65 2e73 6c65 6570 2835      time.sleep(5
+00000c60: 290d 0a20 2020 2072 6574 7572 6e20 6461  )..    return da
+00000c70: 7461 0d0a 0d0a 236c 6973 7420 6f66 2069  ta....#list of i
+00000c80: 6e70 7574 2064 6174 6120 666f 7220 7072  nput data for pr
+00000c90: 6f63 6573 7369 6e67 0d0a 7261 775f 6461  ocessing..raw_da
+00000ca0: 7461 203d 205b 312c 322c 332c 342c 352c  ta = [1,2,3,4,5,
+00000cb0: 362c 372c 382c 392c 3130 5d0d 0a0d 0a23  6,7,8,9,10]....#
+00000cc0: 7365 6e64 696e 6720 6172 6775 6d65 6e74  sending argument
+00000cd0: 7320 666f 7220 6173 796e 6368 726f 6e6f  s for asynchrono
+00000ce0: 7573 206d 756c 7469 2074 6872 6561 6420  us multi thread 
+00000cf0: 7072 6f63 6573 7369 6e67 0d0a 7072 6f63  processing..proc
+00000d00: 6573 7365 645f 6461 7461 203d 2065 6a74  essed_data = ejt
+00000d10: 7261 6465 7254 482e 7374 6172 7428 6d79  raderTH.start(my
+00000d20: 5f66 756e 632c 2064 6174 613d 7261 775f  _func, data=raw_
+00000d30: 6461 7461 2c20 6d61 785f 7468 7265 6164  data, max_thread
+00000d40: 733d 3130 290d 0a0d 0a23 7072 696e 7469  s=10)....#printi
+00000d50: 6e67 2074 6865 2073 796e 6368 726f 6e69  ng the synchroni
+00000d60: 7365 6420 7265 6365 6976 6564 2072 6573  sed received res
+00000d70: 756c 7473 0d0a 7072 696e 7428 290d 0a70  ults..print()..p
+00000d80: 7269 6e74 2866 273e 3e20 496e 7075 743a  rint(f'>> Input:
+00000d90: 207b 7261 775f 6461 7461 7d27 290d 0a70   {raw_data}')..p
+00000da0: 7269 6e74 2866 273e 3e20 5265 7375 6c74  rint(f'>> Result
+00000db0: 3a20 7b70 726f 6365 7373 6564 5f64 6174  : {processed_dat
+00000dc0: 617d 2729 0d0a 7072 696e 7428 6627 3e3e  a}')..print(f'>>
+00000dd0: 2045 6c61 7073 6564 2074 696d 653a 207b   Elapsed time: {
+00000de0: 656a 7472 6164 6572 5448 2e65 6c61 7073  ejtraderTH.elaps
+00000df0: 6564 2829 7d20 7365 6327 290d 0a60 6060  ed()} sec')..```
+00000e00: 0d0a 0d0a 2323 2323 206f 7574 7075 740d  ....#### output.
+00000e10: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 3e3e  ...```python..>>
+00000e20: 2052 756e 6e69 6e67 2054 6872 6561 6420   Running Thread 
+00000e30: 310d 0a3e 3e20 5275 6e6e 696e 6720 5468  1..>> Running Th
+00000e40: 7265 6164 2032 0d0a 3e3e 2052 756e 6e69  read 2..>> Runni
+00000e50: 6e67 2054 6872 6561 6420 330d 0a3e 3e20  ng Thread 3..>> 
+00000e60: 5275 6e6e 696e 6720 5468 7265 6164 2034  Running Thread 4
+00000e70: 0d0a 3e3e 2052 756e 6e69 6e67 2054 6872  ..>> Running Thr
+00000e80: 6561 6420 350d 0a3e 3e20 5275 6e6e 696e  ead 5..>> Runnin
+00000e90: 6720 5468 7265 6164 2036 0d0a 3e3e 2052  g Thread 6..>> R
+00000ea0: 756e 6e69 6e67 2054 6872 6561 6420 370d  unning Thread 7.
+00000eb0: 0a3e 3e20 5275 6e6e 696e 6720 5468 7265  .>> Running Thre
+00000ec0: 6164 2038 0d0a 3e3e 2052 756e 6e69 6e67  ad 8..>> Running
+00000ed0: 2054 6872 6561 6420 390d 0a3e 3e20 5275   Thread 9..>> Ru
+00000ee0: 6e6e 696e 6720 5468 7265 6164 2031 300d  nning Thread 10.
+00000ef0: 0a0d 0a3e 3e20 496e 7075 743a 205b 312c  ...>> Input: [1,
+00000f00: 2032 2c20 332c 2034 2c20 352c 2036 2c20   2, 3, 4, 5, 6, 
+00000f10: 372c 2038 2c20 392c 2031 305d 0d0a 3e3e  7, 8, 9, 10]..>>
+00000f20: 2052 6573 756c 743a 205b 3130 3030 2c20   Result: [1000, 
+00000f30: 3230 3030 2c20 3330 3030 2c20 3430 3030  2000, 3000, 4000
+00000f40: 2c20 3530 3030 2c20 3630 3030 2c20 3730  , 5000, 6000, 70
+00000f50: 3030 2c20 3830 3030 2c20 3930 3030 2c20  00, 8000, 9000, 
+00000f60: 3130 3030 305d 0d0a 3e3e 2045 6c61 7073  10000]..>> Elaps
+00000f70: 6564 2074 696d 653a 2035 2e30 2073 6563  ed time: 5.0 sec
+00000f80: 0d0a 6060 600d 0a0d 0a4e 6f77 2079 6f75  ..```....Now you
+00000f90: 2063 616e 2063 6c65 6172 6c79 2073 6565   can clearly see
+00000fa0: 2c20 6966 2077 6520 646f 2069 7420 7769  , if we do it wi
+00000fb0: 7468 6f75 7420 6d75 6c74 6920 7468 7265  thout multi thre
+00000fc0: 6164 696e 6720 6974 2077 6f75 6c64 2068  ading it would h
+00000fd0: 6176 6520 7461 6b65 6e20 6172 6f75 6e64  ave taken around
+00000fe0: 2060 3530 2053 6563 6f6e 6473 6020 666f   `50 Seconds` fo
+00000ff0: 7220 7072 6f63 6573 7369 6e67 2074 6865  r processing the
+00001000: 2064 6174 6120 7768 696c 6520 646f 696e   data while doin
+00001010: 6720 7468 6520 7461 736b 206f 6e65 2062  g the task one b
+00001020: 7920 6f6e 6520 616e 6420 7761 6974 696e  y one and waitin
+00001030: 6720 666f 7220 6035 2053 6563 6020 6166  g for `5 Sec` af
+00001040: 7465 7220 7275 6e6e 696e 6720 7468 6520  ter running the 
+00001050: 6675 6e63 7469 6f6e 2065 6163 6820 7469  function each ti
+00001060: 6d65 2e20 6275 7420 7369 6e63 6520 7765  me. but since we
+00001070: 2061 7265 2064 6f69 6e67 2069 7420 7769   are doing it wi
+00001080: 7468 206d 756c 7469 7468 7265 6164 696e  th multithreadin
+00001090: 6720 6974 2077 696c 6c20 7461 6b65 206f  g it will take o
+000010a0: 6e6c 7920 6035 2053 6563 6f6e 6473 6020  nly `5 Seconds` 
+000010b0: 666f 7220 7072 6f63 6573 7369 6e67 2074  for processing t
+000010c0: 6865 2073 616d 6520 7461 736b 2077 6974  he same task wit
+000010d0: 6820 6469 6666 6572 656e 7420 6461 7461  h different data
+000010e0: 2c20 696e 2074 6865 6972 2069 6e64 6976  , in their indiv
+000010f0: 6964 7561 6c20 7468 7265 6164 732e 0d0a  idual threads...
+00001100: 0d0a 2323 2323 2045 7861 6d70 6c65 2032  ..#### Example 2
+00001110: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
+00001120: 7468 6520 6675 6e63 7469 6f6e 2066 6f72  the function for
+00001130: 2070 726f 6365 7373 696e 6720 6461 7461   processing data
+00001140: 0d0a 6465 6620 6d79 5f66 756e 6328 6461  ..def my_func(da
+00001150: 7461 293a 0d0a 2020 2020 656a 7472 6164  ta):..    ejtrad
+00001160: 6572 5448 2e63 6f6e 736f 6c65 5f6c 6f67  erTH.console_log
+00001170: 286f 7574 7075 743d 5472 7565 290d 0a20  (output=True).. 
+00001180: 2020 2069 7020 3d20 7265 712e 7265 7175     ip = req.requ
+00001190: 6573 7428 6d65 7468 6f64 3d27 4745 5427  est(method='GET'
+000011a0: 2c75 726c 3d22 6874 7470 3a2f 2f69 7069  ,url="http://ipi
+000011b0: 6e66 6f2e 696f 2f69 7022 290d 0a0d 0a20  nfo.io/ip").... 
+000011c0: 2020 2072 6574 7572 6e20 6970 2e63 6f6e     return ip.con
+000011d0: 7465 6e74 0d0a 0d0a 2373 656e 6469 6e67  tent....#sending
+000011e0: 2061 7267 756d 656e 7473 2066 6f72 2061   arguments for a
+000011f0: 7379 6e63 6872 6f6e 6f75 7320 6d75 6c74  synchronous mult
+00001200: 6920 7468 7265 6164 2070 726f 6365 7373  i thread process
+00001210: 696e 670d 0a70 726f 6365 7373 6564 5f64  ing..processed_d
+00001220: 6174 6120 3d20 656a 7472 6164 6572 5448  ata = ejtraderTH
+00001230: 2e73 7461 7274 286d 795f 6675 6e63 2c20  .start(my_func, 
+00001240: 7265 7065 6174 3d32 302c 206d 6178 5f74  repeat=20, max_t
+00001250: 6872 6561 6473 3d32 3029 0d0a 0d0a 2370  hreads=20)....#p
+00001260: 7269 6e74 696e 6720 7468 6520 7379 6e63  rinting the sync
+00001270: 6872 6f6e 6973 6564 2072 6563 6569 7665  hronised receive
+00001280: 6420 7265 7375 6c74 730d 0a70 7269 6e74  d results..print
+00001290: 2829 0d0a 7072 696e 7428 6627 3e3e 2052  ()..print(f'>> R
+000012a0: 6573 756c 743a 207b 7072 6f63 6573 7365  esult: {processe
+000012b0: 645f 6461 7461 7d27 290d 0a65 6a74 7261  d_data}')..ejtra
+000012c0: 6465 7254 482e 656c 6170 7365 6428 6f75  derTH.elapsed(ou
+000012d0: 7470 7574 3d54 7275 6529 0d0a 6060 600d  tput=True)..```.
+000012e0: 0a0d 0a23 2323 2320 6f75 7470 7574 0d0a  ...#### output..
+000012f0: 0d0a 6060 6070 7974 686f 6e0d 0a3e 3e20  ..```python..>> 
+00001300: 4372 6561 7469 6e67 2054 6872 6561 6473  Creating Threads
+00001310: 2031 0d0a 3e3e 2043 7265 6174 696e 6720   1..>> Creating 
+00001320: 5468 7265 6164 7320 320d 0a3e 3e20 4372  Threads 2..>> Cr
+00001330: 6561 7469 6e67 2054 6872 6561 6473 2033  eating Threads 3
 00001340: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-00001350: 7265 6164 7320 3139 0d0a 3e3e 2043 7265  reads 19..>> Cre
-00001360: 6174 696e 6720 5468 7265 6164 7320 3230  ating Threads 20
-00001370: 0d0a 0d0a 3e3e 2052 6573 756c 743a 205b  ....>> Result: [
-00001380: 6227 3230 302c 3233 342e 3138 322e 3337  b'200,234.182.37
-00001390: 272c 2062 2732 3030 2c32 3334 2e31 3832  ', b'200,234.182
-000013a0: 2e33 3727 2c20 6227 3230 302c 3233 342e  .37', b'200,234.
-000013b0: 3138 322e 3337 272c 2062 2732 3030 2c32  182.37', b'200,2
-000013c0: 3334 2e31 3832 2e33 3727 2c20 6227 3230  34.182.37', b'20
-000013d0: 302c 3233 342e 3138 322e 3337 272c 2062  0,234.182.37', b
-000013e0: 2732 3030 2c32 3334 2e31 3832 2e33 3727  '200,234.182.37'
-000013f0: 2c20 6227 3230 302c 3233 342e 3138 322e  , b'200,234.182.
-00001400: 3337 272c 2062 2732 3030 2c32 3334 2e31  37', b'200,234.1
-00001410: 3832 2e33 3727 2c20 6227 3230 302c 3233  82.37', b'200,23
-00001420: 342e 3138 322e 3337 272c 2062 2732 3030  4.182.37', b'200
-00001430: 2c32 3334 2e31 3832 2e33 3727 2c20 6227  ,234.182.37', b'
-00001440: 3230 302c 3233 342e 3138 322e 3337 272c  200,234.182.37',
-00001450: 2062 2732 3030 2c32 3334 2e31 3832 2e33   b'200,234.182.3
-00001460: 3727 2c20 6227 3230 302c 3233 342e 3138  7', b'200,234.18
-00001470: 322e 3337 272c 2062 2732 3030 2c32 3334  2.37', b'200,234
-00001480: 2e31 3832 2e33 3727 2c20 6227 3230 302c  .182.37', b'200,
-00001490: 3233 342e 3138 322e 3337 272c 2062 2732  234.182.37', b'2
-000014a0: 3030 2c32 3334 2e31 3832 2e33 3727 2c20  00,234.182.37', 
-000014b0: 6227 3230 302c 3233 342e 3138 322e 3337  b'200,234.182.37
-000014c0: 272c 2062 2732 3030 2c32 3334 2e31 3832  ', b'200,234.182
-000014d0: 2e33 3727 2c20 6227 3230 302c 3233 342e  .37', b'200,234.
-000014e0: 3138 322e 3337 272c 2062 2732 3030 2c32  182.37', b'200,2
-000014f0: 3334 2e31 3832 2e33 3727 5d0d 0a3e 3e20  34.182.37']..>> 
-00001500: 456c 6170 7365 6420 7469 6d65 3a20 302e  Elapsed time: 0.
-00001510: 3331 2073 6563 0d0a 6060 600d 0a0d 0a49  31 sec..```....I
-00001520: 6e20 7468 6973 2065 7861 6d70 6c65 2077  n this example w
-00001530: 6520 6469 646e 2774 2075 7365 6420 7469  e didn't used ti
-00001540: 6d65 2e73 6c65 6570 2829 2069 6e73 7465  me.sleep() inste
-00001550: 6164 2077 6520 6d61 6b65 2061 2072 6571  ad we make a req
-00001560: 7565 7374 2074 6f20 7468 6520 7765 6273  uest to the webs
-00001570: 6572 7665 7220 616e 6420 6974 2074 6f6f  erver and it too
-00001580: 6b20 6030 2e35 2073 6563 6f6e 6473 6020  k `0.5 seconds` 
-00001590: 746f 2067 6574 2074 6865 2072 6573 756c  to get the resul
-000015a0: 7420 6261 636b 2073 6f20 7765 2064 6964  t back so we did
-000015b0: 2069 7420 3230 2074 696d 6573 2077 6974   it 20 times wit
-000015c0: 6820 6d75 6c74 6920 7468 7265 6164 696e  h multi threadin
-000015d0: 6720 616e 6420 7765 7265 2061 626c 6520  g and were able 
-000015e0: 746f 2072 6563 6569 7665 2074 6865 2072  to receive the r
-000015f0: 6573 756c 7473 2069 6e20 6c65 7373 2074  esults in less t
-00001600: 696d 6520 696e 2061 2073 796e 6368 726f  ime in a synchro
-00001610: 6e6f 7573 206f 7264 6572 2e0d 0a0d 0a3e  nous order.....>
-00001620: 204c 6574 7320 7472 7920 746f 2064 6f20   Lets try to do 
-00001630: 6974 2077 6974 686f 7574 206d 756c 7469  it without multi
-00001640: 7468 7265 6164 696e 6720 616e 6420 7365  threading and se
-00001650: 6520 686f 7720 6974 2061 6666 6563 7473  e how it affects
-00001660: 2074 6865 2070 726f 6365 7373 696e 6720   the processing 
-00001670: 7469 6d65 2e0d 0a0d 0a53 6f20 696e 2074  time.....So in t
-00001680: 6869 7320 6e65 7720 7570 6461 7465 2060  his new update `
-00001690: 656a 7472 6164 6572 5448 2076 312e 3060  ejtraderTH v1.0`
-000016a0: 2077 6520 6361 6e20 7370 6563 6966 7920   we can specify 
-000016b0: 7468 6174 2061 7420 6f6e 6365 2068 6f77  that at once how
-000016c0: 206d 616e 7920 7468 7265 6164 7320 7368   many threads sh
-000016d0: 6f75 6c64 2062 6520 6372 6561 7465 6420  ould be created 
-000016e0: 736f 206c 6574 7320 6368 616e 6765 2074  so lets change t
-000016f0: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
-00001700: 6572 2061 7320 606d 6178 5f74 6872 6561  er as `max_threa
-00001710: 6473 203d 2031 6020 7468 6973 2077 6179  ds = 1` this way
-00001720: 2069 7420 7769 6c6c 206f 6e6c 7920 6372   it will only cr
-00001730: 6561 7465 206f 6e65 2074 6872 6561 6420  eate one thread 
-00001740: 6174 2061 2074 696d 6520 616e 6420 7769  at a time and wi
-00001750: 6c6c 2077 6169 7420 756e 7469 6c20 7468  ll wait until th
-00001760: 6520 7072 6576 696f 7573 2074 6872 6561  e previous threa
-00001770: 6420 6861 7320 6669 6e69 7368 6564 2070  d has finished p
-00001780: 726f 7065 726c 792e 0d0a 0d0a 2323 2323  roperly.....####
-00001790: 206f 7574 7075 740d 0a0d 0a60 6060 7079   output....```py
-000017a0: 7468 6f6e 0d0a 2e0d 0a2e 0d0a 2e0d 0a3e  thon...........>
-000017b0: 3e20 456c 6170 7365 6420 7469 6d65 3a20  > Elapsed time: 
-000017c0: 362e 3433 2073 6563 0d0a 6060 600d 0a0d  6.43 sec..```...
-000017d0: 0a49 7420 6973 2063 6c65 6172 2074 6861  .It is clear tha
-000017e0: 7420 6576 6572 7920 7265 7175 6573 7420  t every request 
-000017f0: 746f 2074 6865 2073 6572 7665 7220 7761  to the server wa
-00001800: 7320 7461 6b69 6e67 2061 7070 726f 782e  s taking approx.
-00001810: 2060 302e 3520 7365 636f 6e64 7360 2073   `0.5 seconds` s
-00001820: 6f20 7768 696c 6520 6d61 6b69 6e67 206f  o while making o
-00001830: 6e65 2072 6571 7565 7374 2061 7420 6120  ne request at a 
-00001840: 7469 6d65 2069 7420 746f 6f6b 2060 362e  time it took `6.
-00001850: 3433 2073 6563 6f6e 6473 6020 6173 2065  43 seconds` as e
-00001860: 7870 6563 7465 642e 0d0a 0d0a 2323 2320  xpected.....### 
-00001870: 4578 616d 706c 6520 330d 0a0d 0a51 7569  Example 3....Qui
-00001880: 636b 204c 6175 6e63 6820 6d6f 6465 2c20  ck Launch mode, 
-00001890: 6120 6e65 7720 6665 6174 7572 6520 6973  a new feature is
-000018a0: 2061 6464 6564 2077 6865 7265 2079 6f75   added where you
-000018b0: 2063 616e 2064 6972 6563 746c 7920 7573   can directly us
-000018c0: 6520 656a 7472 6164 6572 5448 2074 6f20  e ejtraderTH to 
-000018d0: 7061 7373 2069 6e20 7468 6520 7265 7065  pass in the repe
-000018e0: 7469 7469 7665 2066 756e 6374 696f 6e2c  titive function,
-000018f0: 2069 6e70 7574 2064 6174 6120 666f 7220   input data for 
-00001900: 7468 6f73 6520 6675 6e63 7469 6f6e 7320  those functions 
-00001910: 616e 6420 686f 7720 6d61 6e79 2074 6872  and how many thr
-00001920: 6561 6473 2079 6f75 2077 616e 7420 6974  eads you want it
-00001930: 2074 6f20 6372 6561 7465 2061 7420 6120   to create at a 
-00001940: 7469 6d65 2e20 6f74 6865 7220 7468 616e  time. other than
-00001950: 2074 6861 7420 6966 2079 6f75 206a 7573   that if you jus
-00001960: 7420 7761 6e74 2069 7420 746f 2072 6570  t want it to rep
-00001970: 6561 7420 7468 6520 6675 6e63 7469 6f6e  eat the function
-00001980: 2077 6974 686f 7574 2061 6e79 2069 6e70   without any inp
-00001990: 7574 7320 796f 7520 6361 6e20 646f 2074  uts you can do t
-000019a0: 6861 7420 746f 6f2e 0d0a 0d0a 6060 6070  hat too.....```p
-000019b0: 7974 686f 6e0d 0a69 6d70 6f72 7420 656a  ython..import ej
-000019c0: 7472 6164 6572 5448 0d0a 696d 706f 7274  traderTH..import
-000019d0: 2074 696d 650d 0a69 6d70 6f72 7420 7261   time..import ra
-000019e0: 6e64 6f6d 0d0a 0d0a 6e61 6d65 7320 3d20  ndom....names = 
-000019f0: 5b27 4170 7269 6c27 2c20 274d 6179 275d  ['April', 'May']
-00001a00: 0d0a 0d0a 2374 6865 2066 756e 6374 696f  ....#the functio
-00001a10: 6e20 666f 7220 7072 6f63 6573 7369 6e67  n for processing
-00001a20: 2064 6174 610d 0a64 6566 206d 795f 6675   data..def my_fu
-00001a30: 6e63 2864 6174 6129 3a0d 0a20 2020 2065  nc(data):..    e
-00001a40: 6a74 7261 6465 7254 482e 636f 6e73 6f6c  jtraderTH.consol
-00001a50: 655f 6c6f 6728 6f75 7470 7574 3d54 7275  e_log(output=Tru
-00001a60: 6529 0d0a 2020 2020 7469 6d65 2e73 6c65  e)..    time.sle
-00001a70: 6570 2831 290d 0a20 2020 206e 616d 6520  ep(1)..    name 
-00001a80: 3d20 7261 6e64 6f6d 2e63 686f 6963 6528  = random.choice(
-00001a90: 6e61 6d65 7329 0d0a 2020 2020 7265 7475  names)..    retu
-00001aa0: 726e 2066 277b 6e61 6d65 7d20 7361 7973  rn f'{name} says
-00001ab0: 2c20 4865 6c6c 6f20 576f 726c 6421 270d  , Hello World!'.
-00001ac0: 0a0d 0a70 726f 6365 7373 6564 5f64 6174  ...processed_dat
-00001ad0: 6120 3d20 656a 7472 6164 6572 5448 2e73  a = ejtraderTH.s
-00001ae0: 7461 7274 286d 795f 6675 6e63 2c20 7265  tart(my_func, re
-00001af0: 7065 6174 3d34 290d 0a0d 0a70 7269 6e74  peat=4)....print
-00001b00: 2870 726f 6365 7373 6564 5f64 6174 6129  (processed_data)
-00001b10: 0d0a 656a 7472 6164 6572 5448 2e65 6c61  ..ejtraderTH.ela
-00001b20: 7073 6564 286f 7574 7075 743d 5472 7565  psed(output=True
-00001b30: 290d 0a60 6060 0d0a 0d0a 2323 2320 6f75  )..```....### ou
-00001b40: 7470 7574 0d0a 0d0a 6060 600d 0a3e 3e20  tput....```..>> 
-00001b50: 4372 6561 7469 6e67 2054 6872 6561 6473  Creating Threads
-00001b60: 2031 0d0a 3e3e 2043 7265 6174 696e 6720   1..>> Creating 
-00001b70: 5468 7265 6164 7320 320d 0a3e 3e20 4372  Threads 2..>> Cr
-00001b80: 6561 7469 6e67 2054 6872 6561 6473 2033  eating Threads 3
-00001b90: 0d0a 3e3e 2043 7265 6174 696e 6720 5468  ..>> Creating Th
-00001ba0: 7265 6164 7320 340d 0a5b 274d 6179 2073  reads 4..['May s
-00001bb0: 6179 732c 2048 656c 6c6f 2057 6f72 6c64  ays, Hello World
-00001bc0: 2127 2c20 2741 7072 696c 2073 6179 732c  !', 'April says,
-00001bd0: 2048 656c 6c6f 2057 6f72 6c64 2127 2c20   Hello World!', 
-00001be0: 274d 6179 2073 6179 732c 2048 656c 6c6f  'May says, Hello
-00001bf0: 2057 6f72 6c64 2127 2c20 2741 7072 696c   World!', 'April
-00001c00: 2073 6179 732c 2048 656c 6c6f 2057 6f72   says, Hello Wor
-00001c10: 6c64 2127 5d0d 0a3e 3e20 456c 6170 7365  ld!']..>> Elapse
-00001c20: 6420 7469 6d65 3a20 312e 3020 7365 630d  d time: 1.0 sec.
-00001c30: 0a60 6060 0d0a 0d0a 7765 206b 6570 7420  .```....we kept 
-00001c40: 6120 7469 6d65 2067 6170 206f 6620 3120  a time gap of 1 
-00001c50: 7365 6320 696e 7369 6465 2074 6865 2066  sec inside the f
-00001c60: 756e 6374 696f 6e20 7374 696c 6c20 6974  unction still it
-00001c70: 2072 6570 6561 7465 6420 7468 6520 7461   repeated the ta
-00001c80: 736b 2034 2074 696d 6573 2069 6e20 7361  sk 4 times in sa
-00001c90: 6d65 2074 696d 652e 2073 696e 6365 2069  me time. since i
-00001ca0: 7420 6361 6e20 6163 6365 7373 2074 6865  t can access the
-00001cb0: 2067 6c6f 6261 6c20 7661 7269 6162 6c65   global variable
-00001cc0: 7320 7765 2063 616e 2061 7373 6967 6e20  s we can assign 
-00001cd0: 6365 7274 6169 6e20 7461 736b 7320 7468  certain tasks th
-00001ce0: 6174 2064 6f6e 2774 206e 6565 6420 6469  at don't need di
-00001cf0: 6666 6572 656e 7420 696e 7075 7473 2065  fferent inputs e
-00001d00: 7665 7279 2074 696d 652e 0d0a 0d0a 2323  very time.....##
-00001d10: 2320 4465 636f 7261 746f 7273 2073 7570  # Decorators sup
-00001d20: 706f 7274 0d0a 0d0a 4170 6172 7420 6672  port....Apart fr
-00001d30: 6f6d 2063 616c 6c69 6e67 2074 6865 2060  om calling the `
-00001d40: 7374 6172 7428 2960 2061 7474 7269 6275  start()` attribu
-00001d50: 7465 2077 6520 6361 6e20 616c 736f 2075  te we can also u
-00001d60: 7365 2064 6563 6f72 6174 6f72 7320 746f  se decorators to
-00001d70: 2065 7870 6c69 6369 746c 7920 6d61 6b65   explicitly make
-00001d80: 206f 7572 2066 756e 6374 696f 6e73 2066   our functions f
-00001d90: 6f72 2063 6f6e 6375 7272 656e 7420 6578  or concurrent ex
-00001da0: 6563 7574 696f 6e2e 0d0a 0d0a 2a2a 4578  ecution.....**Ex
-00001db0: 616d 706c 6520 312a 2a0d 0a0d 0a60 6060  ample 1**....```
-00001dc0: 7079 7468 6f6e 0d0a 696d 706f 7274 2065  python..import e
-00001dd0: 6a74 7261 6465 7254 480d 0a69 6d70 6f72  jtraderTH..impor
-00001de0: 7420 7469 6d65 0d0a 0d0a 4065 6a74 7261  t time....@ejtra
-00001df0: 6465 7254 482e 7275 6e28 7265 7065 6174  derTH.run(repeat
-00001e00: 3d35 2c20 6d61 785f 7468 7265 6164 733d  =5, max_threads=
-00001e10: 3529 0d0a 6465 6620 6d79 5f66 756e 6328  5)..def my_func(
-00001e20: 6929 3a0d 0a20 2020 2074 696d 652e 736c  i):..    time.sl
-00001e30: 6565 7028 3129 0d0a 2020 2020 7265 7475  eep(1)..    retu
-00001e40: 726e 2069 2a32 0d0a 0d0a 7072 696e 7428  rn i*2....print(
-00001e50: 656a 7472 6164 6572 5448 2e72 6573 756c  ejtraderTH.resul
-00001e60: 745b 276d 795f 6675 6e63 275d 290d 0a60  t['my_func'])..`
-00001e70: 6060 0d0a 0d0a 2a2a 4f75 7470 7574 2a2a  ``....**Output**
-00001e80: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a5b  ....```python..[
-00001e90: 302c 2032 2c20 342c 2036 2c20 385d 0d0a  0, 2, 4, 6, 8]..
-00001ea0: 6060 600d 0a0d 0a54 6869 7320 7769 6c6c  ```....This will
-00001eb0: 2065 7865 6375 7465 2074 6865 2066 756e   execute the fun
-00001ec0: 6374 696f 6e20 6173 2073 6f6f 6e20 6173  ction as soon as
-00001ed0: 2079 6f75 2072 756e 2079 6f75 7220 7079   you run your py
-00001ee0: 7468 6f6e 2063 6f64 652c 2069 6e20 7468  thon code, in th
-00001ef0: 6973 2063 6173 6520 7765 2061 7265 2074  is case we are t
-00001f00: 7279 696e 6720 746f 2070 6572 666f 726d  rying to perform
-00001f10: 2074 6865 2073 616d 6520 7461 736b 2066   the same task f
-00001f20: 6976 6520 7469 6d65 7320 696e 2061 2072  ive times in a r
-00001f30: 6f77 2063 6f6e 6375 7272 656e 746c 792e  ow concurrently.
-00001f40: 2054 6865 2066 696e 616c 206f 7574 7075   The final outpu
-00001f50: 7420 6f66 2061 6c6c 2074 6865 2066 756e  t of all the fun
-00001f60: 6374 696f 6e20 6361 6e20 6265 2061 6363  ction can be acc
-00001f70: 6573 7365 6420 6279 2060 656a 7472 6164  essed by `ejtrad
-00001f80: 6572 5448 2e72 6573 756c 745b 2766 756e  erTH.result['fun
-00001f90: 6374 696f 6e5f 6e61 6d65 275d 602e 204e  ction_name']`. N
-00001fa0: 6f74 6963 6520 6966 2079 6f75 2073 6574  otice if you set
-00001fb0: 2079 6f75 7220 6675 6e63 7469 6f6e 206f   your function o
-00001fc0: 6e20 7265 7065 6174 2069 7420 7769 6c6c  n repeat it will
-00001fd0: 2061 6c77 6179 7320 7265 6365 6976 6520   always receive 
-00001fe0: 6120 7061 7261 6d65 7465 7220 7768 6963  a parameter whic
-00001ff0: 6820 6973 2069 7427 7320 7468 7265 6164  h is it's thread
-00002000: 206e 756d 6265 722e 0d0a 0d0a 2d2d 2d0d   number.....---.
-00002010: 0a0d 0a2a 2a45 7861 6d70 6c65 2032 2a2a  ...**Example 2**
-00002020: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002030: 6d70 6f72 7420 656a 7472 6164 6572 5448  mport ejtraderTH
-00002040: 0d0a 696d 706f 7274 2074 696d 650d 0a0d  ..import time...
-00002050: 0a40 656a 7472 6164 6572 5448 2e72 756e  .@ejtraderTH.run
-00002060: 2864 6174 613d 5b31 2c32 2c33 2c34 2c35  (data=[1,2,3,4,5
-00002070: 2c36 5d2c 206d 6178 5f74 6872 6561 6473  ,6], max_threads
-00002080: 3d35 290d 0a64 6566 206d 795f 6675 6e63  =5)..def my_func
-00002090: 2869 293a 0d0a 2020 2020 7469 6d65 2e73  (i):..    time.s
-000020a0: 6c65 6570 2831 290d 0a20 2020 2072 6574  leep(1)..    ret
-000020b0: 7572 6e20 692a 320d 0a0d 0a70 7269 6e74  urn i*2....print
-000020c0: 2865 6a74 7261 6465 7254 482e 7265 7375  (ejtraderTH.resu
-000020d0: 6c74 5b27 6d79 5f66 756e 6327 5d29 0d0a  lt['my_func'])..
-000020e0: 6060 600d 0a0d 0a2a 2a4f 7574 7075 742a  ```....**Output*
-000020f0: 2a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  *....```python..
-00002100: 5b32 2c20 342c 2036 2c20 382c 2031 302c  [2, 4, 6, 8, 10,
-00002110: 2031 325d 0d0a 6060 600d 0a0d 0a49 6e20   12]..```....In 
-00002120: 7468 6973 2063 6173 6520 7765 2061 7265  this case we are
-00002130: 2064 6972 6563 746c 7920 7061 7373 696e   directly passin
-00002140: 6720 6f75 7220 6172 6775 6d65 6e74 7320  g our arguments 
-00002150: 696e 2061 206c 6973 7420 7669 6120 6465  in a list via de
-00002160: 636f 7261 746f 7220 616e 6420 7265 6365  corator and rece
-00002170: 6976 696e 6720 7468 6520 7265 7375 6c74  iving the result
-00002180: 2073 616d 6520 7761 7920 6173 2077 6520   same way as we 
-00002190: 6469 6420 696e 2070 7265 7669 6f75 7320  did in previous 
-000021a0: 6578 616d 706c 652e 0d0a 0d0a 2d2d 2d0d  example.....---.
-000021b0: 0a0d 0a2a 2a45 7861 6d70 6520 332a 2a0d  ...**Exampe 3**.
-000021c0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  ...```python..im
-000021d0: 706f 7274 2065 6a74 7261 6465 7254 480d  port ejtraderTH.
-000021e0: 0a69 6d70 6f72 7420 7469 6d65 0d0a 0d0a  .import time....
-000021f0: 4065 6a74 7261 6465 7254 482e 7365 7428  @ejtraderTH.set(
-00002200: 6d61 785f 7468 7265 6164 733d 3130 290d  max_threads=10).
-00002210: 0a64 6566 206d 795f 6675 6e63 2869 293a  .def my_func(i):
-00002220: 0d0a 2020 2020 7469 6d65 2e73 6c65 6570  ..    time.sleep
-00002230: 2831 290d 0a20 2020 2072 6574 7572 6e20  (1)..    return 
-00002240: 692a 320d 0a0d 0a72 6573 756c 7420 3d20  i*2....result = 
-00002250: 6d79 5f66 756e 6328 7265 7065 6174 3d37  my_func(repeat=7
-00002260: 290d 0a70 7269 6e74 2872 6573 756c 7429  )..print(result)
-00002270: 0d0a 6060 600d 0a0d 0a2a 2a4f 7574 7075  ..```....**Outpu
-00002280: 742a 2a0d 0a0d 0a60 6060 7079 7468 6f6e  t**....```python
-00002290: 0d0a 5b30 2c20 322c 2034 2c20 362c 2038  ..[0, 2, 4, 6, 8
-000022a0: 2c20 3130 2c20 3132 5d0d 0a60 6060 0d0a  , 10, 12]..```..
-000022b0: 0d0a 5468 6973 2069 7320 616e 2061 6e6f  ..This is an ano
-000022c0: 7468 6572 2063 6f6f 6c20 7761 7920 746f  ther cool way to
-000022d0: 2066 6972 7374 2063 6f6e 7665 7274 2079   first convert y
-000022e0: 6f75 7220 6675 6e63 7469 6f6e 2069 6e20  our function in 
-000022f0: 636f 6e63 7572 7265 6e74 2066 756e 6374  concurrent funct
-00002300: 696f 6e20 616e 6420 7468 656e 2070 6173  ion and then pas
-00002310: 7369 6e67 2074 6865 2061 7267 756d 656e  sing the argumen
-00002320: 7420 6173 2068 6f77 206d 616e 7920 7469  t as how many ti
-00002330: 6d65 2079 6f75 2077 616e 7420 746f 2065  me you want to e
-00002340: 7865 6375 7465 2074 6861 7420 6675 6e63  xecute that func
-00002350: 7469 6f6e 2061 6c6c 2069 6e20 7061 7261  tion all in para
-00002360: 6c6c 656c 2e0d 0a0d 0a2d 2d2d 0d0a 0d0a  llel.....---....
-00002370: 2a2a 4578 616d 706c 6520 342a 2a0d 0a0d  **Example 4**...
-00002380: 0a60 6060 7079 7468 6f6e 0d0a 696d 706f  .```python..impo
-00002390: 7274 2065 6a74 7261 6465 7254 480d 0a69  rt ejtraderTH..i
-000023a0: 6d70 6f72 7420 7469 6d65 0d0a 0d0a 4065  mport time....@e
-000023b0: 6a74 7261 6465 7254 482e 7365 7428 290d  jtraderTH.set().
-000023c0: 0a64 6566 206d 795f 6675 6e63 2869 293a  .def my_func(i):
-000023d0: 0d0a 2020 2020 7469 6d65 2e73 6c65 6570  ..    time.sleep
-000023e0: 2831 290d 0a20 2020 2072 6574 7572 6e20  (1)..    return 
-000023f0: 692a 320d 0a0d 0a72 6573 756c 7420 3d20  i*2....result = 
-00002400: 6d79 5f66 756e 6328 5b35 2c36 2c37 5d29  my_func([5,6,7])
-00002410: 0d0a 7072 696e 7428 7265 7375 6c74 290d  ..print(result).
-00002420: 0a60 6060 0d0a 0d0a 2a2a 4f75 7470 7574  .```....**Output
-00002430: 2a2a 0d0a 0d0a 6060 6070 7974 686f 6e0d  **....```python.
-00002440: 0a5b 3130 2c20 3132 2c20 3134 5d0d 0a60  .[10, 12, 14]..`
-00002450: 6060 0d0a 0d0a 4167 6169 6e20 7765 2063  ``....Again we c
-00002460: 616e 2061 6c73 6f20 7370 6563 6966 7920  an also specify 
-00002470: 7768 6174 2061 7267 756d 656e 7473 2077  what arguments w
-00002480: 6520 7761 6e74 2074 6f20 7061 7373 2074  e want to pass t
-00002490: 6f20 7468 6520 6675 6e63 7469 6f6e 2074  o the function t
-000024a0: 6f20 7072 6f63 6573 7320 6974 2063 6f6e  o process it con
-000024b0: 6375 7272 656e 746c 792e 2069 6620 696e  currently. if in
-000024c0: 2074 6865 2060 4065 6a74 7261 6465 7254   the `@ejtraderT
-000024d0: 482e 7365 7428 2960 2064 6563 6f72 6174  H.set()` decorat
-000024e0: 6f72 2079 6f75 2077 6f6e 2774 2070 6173  or you won't pas
-000024f0: 7320 616e 7920 606d 6178 5f74 6872 6561  s any `max_threa
-00002500: 6473 6020 6172 6775 6d65 6e74 2060 6d61  ds` argument `ma
-00002510: 785f 7468 7265 6164 733d 3130 6020 7769  x_threads=10` wi
-00002520: 6c6c 2062 6520 7365 742e 0d0a 0d0a 2323  ll be set.....##
-00002530: 2323 2048 616e 646c 696e 6720 6572 726f  ## Handling erro
-00002540: 7273 2061 6e64 206b 696c 6c69 6e67 2061  rs and killing a
-00002550: 6c6c 2074 6872 6561 6473 0d0a 0d0a 536f  ll threads....So
-00002560: 2c20 6279 2064 6566 6175 6c74 2069 6620  , by default if 
-00002570: 616e 7920 6572 726f 7220 6f63 6375 7273  any error occurs
-00002580: 2074 6865 2074 6872 6561 6473 2077 696c   the threads wil
-00002590: 6c20 6b65 6570 206f 6e20 7275 6e6e 696e  l keep on runnin
-000025a0: 672c 2069 6e20 6361 7365 2069 6620 796f  g, in case if yo
-000025b0: 7520 7761 6e74 2074 6f20 6967 6e6f 7265  u want to ignore
-000025c0: 2073 6f6d 6520 6572 726f 7273 2062 7574   some errors but
-000025d0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
-000025e0: 6b69 6c6c 2061 6c6c 2074 6865 2074 6872  kill all the thr
-000025f0: 6561 6420 6174 206f 6e63 6520 796f 7520  ead at once you 
-00002600: 6361 6e20 7573 6520 6065 6a74 7261 6465  can use `ejtrade
-00002610: 7254 482e 7374 6f70 2829 6020 7768 696c  rTH.stop()` whil
-00002620: 6520 6861 6e64 6c69 6e67 2065 7272 6f72  e handling error
-00002630: 732e 0d0a 0d0a 6060 6070 7974 686f 6e0d  s.....```python.
-00002640: 0a23 7468 6520 6675 6e63 7469 6f6e 2066  .#the function f
-00002650: 6f72 2070 726f 6365 7373 696e 6720 6461  or processing da
-00002660: 7461 0d0a 6465 6620 6d79 5f66 756e 6328  ta..def my_func(
-00002670: 6461 7461 293a 0d0a 2020 2020 7468 7265  data):..    thre
-00002680: 6164 5f6e 756d 6265 7220 3d20 656a 7472  ad_number = ejtr
-00002690: 6164 6572 5448 2e63 6f6e 736f 6c65 5f6c  aderTH.console_l
-000026a0: 6f67 286f 7574 7075 743d 5472 7565 290d  og(output=True).
-000026b0: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-000026c0: 2020 2064 6174 6120 3d20 7265 7175 6573     data = reques
-000026d0: 7473 2e67 6574 2822 6874 7470 3a2f 2f68  ts.get("http://h
-000026e0: 7474 7062 696e 2e6f 7267 2f67 6574 2229  ttpbin.org/get")
-000026f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002700: 2064 6174 610d 0a20 2020 2065 7863 6570   data..    excep
-00002710: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00002720: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00002730: 2865 2920 2370 7269 6e74 696e 6720 6f74  (e) #printing ot
-00002740: 6865 7220 6572 726f 7273 0d0a 2020 2020  her errors..    
-00002750: 2020 2020 236b 696c 6c69 6e67 2061 6c6c      #killing all
-00002760: 2061 6374 6976 6520 7468 7265 6164 730d   active threads.
-00002770: 0a20 2020 2020 2020 2065 6a74 7261 6465  .        ejtrade
-00002780: 7254 482e 7374 6f70 2829 2023 7573 6520  rTH.stop() #use 
-00002790: 746f 206b 696c 6c20 616c 6c20 7468 7265  to kill all thre
-000027a0: 6164 730d 0a60 6060 0d0a 0d0a 6966 2079  ads..```....if y
-000027b0: 6f75 2064 6f6e 2774 2075 7365 2060 656a  ou don't use `ej
-000027c0: 7472 6164 6572 5448 2e73 746f 7028 2960  traderTH.stop()`
-000027d0: 2066 756e 6374 696f 6e20 7468 656e 2074   function then t
-000027e0: 6865 2074 6872 6561 6473 2077 696c 6c20  he threads will 
-000027f0: 6b65 6570 206f 6e20 7275 6e6e 696e 6720  keep on running 
-00002800: 616e 6420 6669 6c6c 696e 6720 604e 6f6e  and filling `Non
-00002810: 6560 2069 6e20 706c 6163 6520 6f66 2072  e` in place of r
-00002820: 6574 7572 6e65 6420 6461 7461 2e20 6966  eturned data. if
-00002830: 2079 6f75 2075 7365 6420 7468 6520 6065   you used the `e
-00002840: 6a74 7261 6465 7254 482e 7374 6f70 2829  jtraderTH.stop()
-00002850: 6020 6974 2077 696c 6c20 6b69 6c6c 2061  ` it will kill a
-00002860: 6c6c 2061 6374 6976 6520 7468 7265 6164  ll active thread
-00002870: 7320 696d 6d65 6469 6174 656c 7920 616e  s immediately an
-00002880: 6420 7769 6c6c 2072 6574 7572 6e20 7468  d will return th
-00002890: 6520 6461 7461 2074 6861 7420 7765 7265  e data that were
-000028a0: 2070 726f 6365 7373 6564 2062 7920 796f   processed by yo
-000028b0: 7572 2066 756e 6374 696f 6e20 736f 2066  ur function so f
-000028c0: 6172 2e0d 0a                             ar...
+00001350: 7265 6164 7320 340d 0a3e 3e20 4372 6561  reads 4..>> Crea
+00001360: 7469 6e67 2054 6872 6561 6473 2035 0d0a  ting Threads 5..
+00001370: 3e3e 2043 7265 6174 696e 6720 5468 7265  >> Creating Thre
+00001380: 6164 7320 360d 0a3e 3e20 4372 6561 7469  ads 6..>> Creati
+00001390: 6e67 2054 6872 6561 6473 2037 0d0a 3e3e  ng Threads 7..>>
+000013a0: 2043 7265 6174 696e 6720 5468 7265 6164   Creating Thread
+000013b0: 7320 380d 0a3e 3e20 4372 6561 7469 6e67  s 8..>> Creating
+000013c0: 2054 6872 6561 6473 2039 0d0a 3e3e 2043   Threads 9..>> C
+000013d0: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+000013e0: 3130 0d0a 3e3e 2043 7265 6174 696e 6720  10..>> Creating 
+000013f0: 5468 7265 6164 7320 3131 0d0a 3e3e 2043  Threads 11..>> C
+00001400: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+00001410: 3132 0d0a 3e3e 2043 7265 6174 696e 6720  12..>> Creating 
+00001420: 5468 7265 6164 7320 3133 0d0a 3e3e 2043  Threads 13..>> C
+00001430: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+00001440: 3134 0d0a 3e3e 2043 7265 6174 696e 6720  14..>> Creating 
+00001450: 5468 7265 6164 7320 3135 0d0a 3e3e 2043  Threads 15..>> C
+00001460: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+00001470: 3136 0d0a 3e3e 2043 7265 6174 696e 6720  16..>> Creating 
+00001480: 5468 7265 6164 7320 3137 0d0a 3e3e 2043  Threads 17..>> C
+00001490: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+000014a0: 3138 0d0a 3e3e 2043 7265 6174 696e 6720  18..>> Creating 
+000014b0: 5468 7265 6164 7320 3139 0d0a 3e3e 2043  Threads 19..>> C
+000014c0: 7265 6174 696e 6720 5468 7265 6164 7320  reating Threads 
+000014d0: 3230 0d0a 0d0a 3e3e 2052 6573 756c 743a  20....>> Result:
+000014e0: 205b 6227 3230 302c 3233 342e 3138 322e   [b'200,234.182.
+000014f0: 3337 272c 2062 2732 3030 2c32 3334 2e31  37', b'200,234.1
+00001500: 3832 2e33 3727 2c20 6227 3230 302c 3233  82.37', b'200,23
+00001510: 342e 3138 322e 3337 272c 2062 2732 3030  4.182.37', b'200
+00001520: 2c32 3334 2e31 3832 2e33 3727 2c20 6227  ,234.182.37', b'
+00001530: 3230 302c 3233 342e 3138 322e 3337 272c  200,234.182.37',
+00001540: 2062 2732 3030 2c32 3334 2e31 3832 2e33   b'200,234.182.3
+00001550: 3727 2c20 6227 3230 302c 3233 342e 3138  7', b'200,234.18
+00001560: 322e 3337 272c 2062 2732 3030 2c32 3334  2.37', b'200,234
+00001570: 2e31 3832 2e33 3727 2c20 6227 3230 302c  .182.37', b'200,
+00001580: 3233 342e 3138 322e 3337 272c 2062 2732  234.182.37', b'2
+00001590: 3030 2c32 3334 2e31 3832 2e33 3727 2c20  00,234.182.37', 
+000015a0: 6227 3230 302c 3233 342e 3138 322e 3337  b'200,234.182.37
+000015b0: 272c 2062 2732 3030 2c32 3334 2e31 3832  ', b'200,234.182
+000015c0: 2e33 3727 2c20 6227 3230 302c 3233 342e  .37', b'200,234.
+000015d0: 3138 322e 3337 272c 2062 2732 3030 2c32  182.37', b'200,2
+000015e0: 3334 2e31 3832 2e33 3727 2c20 6227 3230  34.182.37', b'20
+000015f0: 302c 3233 342e 3138 322e 3337 272c 2062  0,234.182.37', b
+00001600: 2732 3030 2c32 3334 2e31 3832 2e33 3727  '200,234.182.37'
+00001610: 2c20 6227 3230 302c 3233 342e 3138 322e  , b'200,234.182.
+00001620: 3337 272c 2062 2732 3030 2c32 3334 2e31  37', b'200,234.1
+00001630: 3832 2e33 3727 2c20 6227 3230 302c 3233  82.37', b'200,23
+00001640: 342e 3138 322e 3337 272c 2062 2732 3030  4.182.37', b'200
+00001650: 2c32 3334 2e31 3832 2e33 3727 5d0d 0a3e  ,234.182.37']..>
+00001660: 3e20 456c 6170 7365 6420 7469 6d65 3a20  > Elapsed time: 
+00001670: 302e 3331 2073 6563 0d0a 6060 600d 0a0d  0.31 sec..```...
+00001680: 0a49 6e20 7468 6973 2065 7861 6d70 6c65  .In this example
+00001690: 2077 6520 6469 646e 2774 2075 7365 6420   we didn't used 
+000016a0: 7469 6d65 2e73 6c65 6570 2829 2069 6e73  time.sleep() ins
+000016b0: 7465 6164 2077 6520 6d61 6b65 2061 2072  tead we make a r
+000016c0: 6571 7565 7374 2074 6f20 7468 6520 7765  equest to the we
+000016d0: 6273 6572 7665 7220 616e 6420 6974 2074  bserver and it t
+000016e0: 6f6f 6b20 6030 2e35 2073 6563 6f6e 6473  ook `0.5 seconds
+000016f0: 6020 746f 2067 6574 2074 6865 2072 6573  ` to get the res
+00001700: 756c 7420 6261 636b 2073 6f20 7765 2064  ult back so we d
+00001710: 6964 2069 7420 3230 2074 696d 6573 2077  id it 20 times w
+00001720: 6974 6820 6d75 6c74 6920 7468 7265 6164  ith multi thread
+00001730: 696e 6720 616e 6420 7765 7265 2061 626c  ing and were abl
+00001740: 6520 746f 2072 6563 6569 7665 2074 6865  e to receive the
+00001750: 2072 6573 756c 7473 2069 6e20 6c65 7373   results in less
+00001760: 2074 696d 6520 696e 2061 2073 796e 6368   time in a synch
+00001770: 726f 6e6f 7573 206f 7264 6572 2e0d 0a0d  ronous order....
+00001780: 0a3e 204c 6574 7320 7472 7920 746f 2064  .> Lets try to d
+00001790: 6f20 6974 2077 6974 686f 7574 206d 756c  o it without mul
+000017a0: 7469 7468 7265 6164 696e 6720 616e 6420  tithreading and 
+000017b0: 7365 6520 686f 7720 6974 2061 6666 6563  see how it affec
+000017c0: 7473 2074 6865 2070 726f 6365 7373 696e  ts the processin
+000017d0: 6720 7469 6d65 2e0d 0a0d 0a53 6f20 696e  g time.....So in
+000017e0: 2074 6869 7320 6e65 7720 7570 6461 7465   this new update
+000017f0: 2060 656a 7472 6164 6572 5448 2076 312e   `ejtraderTH v1.
+00001800: 3060 2077 6520 6361 6e20 7370 6563 6966  0` we can specif
+00001810: 7920 7468 6174 2061 7420 6f6e 6365 2068  y that at once h
+00001820: 6f77 206d 616e 7920 7468 7265 6164 7320  ow many threads 
+00001830: 7368 6f75 6c64 2062 6520 6372 6561 7465  should be create
+00001840: 6420 736f 206c 6574 7320 6368 616e 6765  d so lets change
+00001850: 2074 6865 2069 6e70 7574 2070 6172 616d   the input param
+00001860: 6574 6572 2061 7320 606d 6178 5f74 6872  eter as `max_thr
+00001870: 6561 6473 203d 2031 6020 7468 6973 2077  eads = 1` this w
+00001880: 6179 2069 7420 7769 6c6c 206f 6e6c 7920  ay it will only 
+00001890: 6372 6561 7465 206f 6e65 2074 6872 6561  create one threa
+000018a0: 6420 6174 2061 2074 696d 6520 616e 6420  d at a time and 
+000018b0: 7769 6c6c 2077 6169 7420 756e 7469 6c20  will wait until 
+000018c0: 7468 6520 7072 6576 696f 7573 2074 6872  the previous thr
+000018d0: 6561 6420 6861 7320 6669 6e69 7368 6564  ead has finished
+000018e0: 2070 726f 7065 726c 792e 0d0a 0d0a 2323   properly.....##
+000018f0: 2323 206f 7574 7075 740d 0a0d 0a60 6060  ## output....```
+00001900: 7079 7468 6f6e 0d0a 2e0d 0a2e 0d0a 2e0d  python..........
+00001910: 0a3e 3e20 456c 6170 7365 6420 7469 6d65  .>> Elapsed time
+00001920: 3a20 362e 3433 2073 6563 0d0a 6060 600d  : 6.43 sec..```.
+00001930: 0a0d 0a49 7420 6973 2063 6c65 6172 2074  ...It is clear t
+00001940: 6861 7420 6576 6572 7920 7265 7175 6573  hat every reques
+00001950: 7420 746f 2074 6865 2073 6572 7665 7220  t to the server 
+00001960: 7761 7320 7461 6b69 6e67 2061 7070 726f  was taking appro
+00001970: 782e 2060 302e 3520 7365 636f 6e64 7360  x. `0.5 seconds`
+00001980: 2073 6f20 7768 696c 6520 6d61 6b69 6e67   so while making
+00001990: 206f 6e65 2072 6571 7565 7374 2061 7420   one request at 
+000019a0: 6120 7469 6d65 2069 7420 746f 6f6b 2060  a time it took `
+000019b0: 362e 3433 2073 6563 6f6e 6473 6020 6173  6.43 seconds` as
+000019c0: 2065 7870 6563 7465 642e 0d0a 0d0a 2323   expected.....##
+000019d0: 2320 4578 616d 706c 6520 330d 0a0d 0a51  # Example 3....Q
+000019e0: 7569 636b 204c 6175 6e63 6820 6d6f 6465  uick Launch mode
+000019f0: 2c20 6120 6e65 7720 6665 6174 7572 6520  , a new feature 
+00001a00: 6973 2061 6464 6564 2077 6865 7265 2079  is added where y
+00001a10: 6f75 2063 616e 2064 6972 6563 746c 7920  ou can directly 
+00001a20: 7573 6520 656a 7472 6164 6572 5448 2074  use ejtraderTH t
+00001a30: 6f20 7061 7373 2069 6e20 7468 6520 7265  o pass in the re
+00001a40: 7065 7469 7469 7665 2066 756e 6374 696f  petitive functio
+00001a50: 6e2c 2069 6e70 7574 2064 6174 6120 666f  n, input data fo
+00001a60: 7220 7468 6f73 6520 6675 6e63 7469 6f6e  r those function
+00001a70: 7320 616e 6420 686f 7720 6d61 6e79 2074  s and how many t
+00001a80: 6872 6561 6473 2079 6f75 2077 616e 7420  hreads you want 
+00001a90: 6974 2074 6f20 6372 6561 7465 2061 7420  it to create at 
+00001aa0: 6120 7469 6d65 2e20 6f74 6865 7220 7468  a time. other th
+00001ab0: 616e 2074 6861 7420 6966 2079 6f75 206a  an that if you j
+00001ac0: 7573 7420 7761 6e74 2069 7420 746f 2072  ust want it to r
+00001ad0: 6570 6561 7420 7468 6520 6675 6e63 7469  epeat the functi
+00001ae0: 6f6e 2077 6974 686f 7574 2061 6e79 2069  on without any i
+00001af0: 6e70 7574 7320 796f 7520 6361 6e20 646f  nputs you can do
+00001b00: 2074 6861 7420 746f 6f2e 0d0a 0d0a 6060   that too.....``
+00001b10: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
+00001b20: 656a 7472 6164 6572 5448 0d0a 696d 706f  ejtraderTH..impo
+00001b30: 7274 2074 696d 650d 0a69 6d70 6f72 7420  rt time..import 
+00001b40: 7261 6e64 6f6d 0d0a 0d0a 6e61 6d65 7320  random....names 
+00001b50: 3d20 5b27 4170 7269 6c27 2c20 274d 6179  = ['April', 'May
+00001b60: 275d 0d0a 0d0a 2374 6865 2066 756e 6374  ']....#the funct
+00001b70: 696f 6e20 666f 7220 7072 6f63 6573 7369  ion for processi
+00001b80: 6e67 2064 6174 610d 0a64 6566 206d 795f  ng data..def my_
+00001b90: 6675 6e63 2864 6174 6129 3a0d 0a20 2020  func(data):..   
+00001ba0: 2065 6a74 7261 6465 7254 482e 636f 6e73   ejtraderTH.cons
+00001bb0: 6f6c 655f 6c6f 6728 6f75 7470 7574 3d54  ole_log(output=T
+00001bc0: 7275 6529 0d0a 2020 2020 7469 6d65 2e73  rue)..    time.s
+00001bd0: 6c65 6570 2831 290d 0a20 2020 206e 616d  leep(1)..    nam
+00001be0: 6520 3d20 7261 6e64 6f6d 2e63 686f 6963  e = random.choic
+00001bf0: 6528 6e61 6d65 7329 0d0a 2020 2020 7265  e(names)..    re
+00001c00: 7475 726e 2066 277b 6e61 6d65 7d20 7361  turn f'{name} sa
+00001c10: 7973 2c20 4865 6c6c 6f20 576f 726c 6421  ys, Hello World!
+00001c20: 270d 0a0d 0a70 726f 6365 7373 6564 5f64  '....processed_d
+00001c30: 6174 6120 3d20 656a 7472 6164 6572 5448  ata = ejtraderTH
+00001c40: 2e73 7461 7274 286d 795f 6675 6e63 2c20  .start(my_func, 
+00001c50: 7265 7065 6174 3d34 290d 0a0d 0a70 7269  repeat=4)....pri
+00001c60: 6e74 2870 726f 6365 7373 6564 5f64 6174  nt(processed_dat
+00001c70: 6129 0d0a 656a 7472 6164 6572 5448 2e65  a)..ejtraderTH.e
+00001c80: 6c61 7073 6564 286f 7574 7075 743d 5472  lapsed(output=Tr
+00001c90: 7565 290d 0a60 6060 0d0a 0d0a 2323 2320  ue)..```....### 
+00001ca0: 6f75 7470 7574 0d0a 0d0a 6060 600d 0a3e  output....```..>
+00001cb0: 3e20 4372 6561 7469 6e67 2054 6872 6561  > Creating Threa
+00001cc0: 6473 2031 0d0a 3e3e 2043 7265 6174 696e  ds 1..>> Creatin
+00001cd0: 6720 5468 7265 6164 7320 320d 0a3e 3e20  g Threads 2..>> 
+00001ce0: 4372 6561 7469 6e67 2054 6872 6561 6473  Creating Threads
+00001cf0: 2033 0d0a 3e3e 2043 7265 6174 696e 6720   3..>> Creating 
+00001d00: 5468 7265 6164 7320 340d 0a5b 274d 6179  Threads 4..['May
+00001d10: 2073 6179 732c 2048 656c 6c6f 2057 6f72   says, Hello Wor
+00001d20: 6c64 2127 2c20 2741 7072 696c 2073 6179  ld!', 'April say
+00001d30: 732c 2048 656c 6c6f 2057 6f72 6c64 2127  s, Hello World!'
+00001d40: 2c20 274d 6179 2073 6179 732c 2048 656c  , 'May says, Hel
+00001d50: 6c6f 2057 6f72 6c64 2127 2c20 2741 7072  lo World!', 'Apr
+00001d60: 696c 2073 6179 732c 2048 656c 6c6f 2057  il says, Hello W
+00001d70: 6f72 6c64 2127 5d0d 0a3e 3e20 456c 6170  orld!']..>> Elap
+00001d80: 7365 6420 7469 6d65 3a20 312e 3020 7365  sed time: 1.0 se
+00001d90: 630d 0a60 6060 0d0a 0d0a 7765 206b 6570  c..```....we kep
+00001da0: 7420 6120 7469 6d65 2067 6170 206f 6620  t a time gap of 
+00001db0: 3120 7365 6320 696e 7369 6465 2074 6865  1 sec inside the
+00001dc0: 2066 756e 6374 696f 6e20 7374 696c 6c20   function still 
+00001dd0: 6974 2072 6570 6561 7465 6420 7468 6520  it repeated the 
+00001de0: 7461 736b 2034 2074 696d 6573 2069 6e20  task 4 times in 
+00001df0: 7361 6d65 2074 696d 652e 2073 696e 6365  same time. since
+00001e00: 2069 7420 6361 6e20 6163 6365 7373 2074   it can access t
+00001e10: 6865 2067 6c6f 6261 6c20 7661 7269 6162  he global variab
+00001e20: 6c65 7320 7765 2063 616e 2061 7373 6967  les we can assig
+00001e30: 6e20 6365 7274 6169 6e20 7461 736b 7320  n certain tasks 
+00001e40: 7468 6174 2064 6f6e 2774 206e 6565 6420  that don't need 
+00001e50: 6469 6666 6572 656e 7420 696e 7075 7473  different inputs
+00001e60: 2065 7665 7279 2074 696d 652e 0d0a 0d0a   every time.....
+00001e70: 2323 2320 4465 636f 7261 746f 7273 2073  ### Decorators s
+00001e80: 7570 706f 7274 0d0a 0d0a 4170 6172 7420  upport....Apart 
+00001e90: 6672 6f6d 2063 616c 6c69 6e67 2074 6865  from calling the
+00001ea0: 2060 7374 6172 7428 2960 2061 7474 7269   `start()` attri
+00001eb0: 6275 7465 2077 6520 6361 6e20 616c 736f  bute we can also
+00001ec0: 2075 7365 2064 6563 6f72 6174 6f72 7320   use decorators 
+00001ed0: 746f 2065 7870 6c69 6369 746c 7920 6d61  to explicitly ma
+00001ee0: 6b65 206f 7572 2066 756e 6374 696f 6e73  ke our functions
+00001ef0: 2066 6f72 2063 6f6e 6375 7272 656e 7420   for concurrent 
+00001f00: 6578 6563 7574 696f 6e2e 0d0a 0d0a 2a2a  execution.....**
+00001f10: 4578 616d 706c 6520 312a 2a0d 0a0d 0a60  Example 1**....`
+00001f20: 6060 7079 7468 6f6e 0d0a 696d 706f 7274  ``python..import
+00001f30: 2065 6a74 7261 6465 7254 480d 0a69 6d70   ejtraderTH..imp
+00001f40: 6f72 7420 7469 6d65 0d0a 0d0a 4065 6a74  ort time....@ejt
+00001f50: 7261 6465 7254 482e 7275 6e28 7265 7065  raderTH.run(repe
+00001f60: 6174 3d35 2c20 6d61 785f 7468 7265 6164  at=5, max_thread
+00001f70: 733d 3529 0d0a 6465 6620 6d79 5f66 756e  s=5)..def my_fun
+00001f80: 6328 6929 3a0d 0a20 2020 2074 696d 652e  c(i):..    time.
+00001f90: 736c 6565 7028 3129 0d0a 2020 2020 7265  sleep(1)..    re
+00001fa0: 7475 726e 2069 2a32 0d0a 0d0a 7072 696e  turn i*2....prin
+00001fb0: 7428 656a 7472 6164 6572 5448 2e72 6573  t(ejtraderTH.res
+00001fc0: 756c 745b 276d 795f 6675 6e63 275d 290d  ult['my_func']).
+00001fd0: 0a60 6060 0d0a 0d0a 2a2a 4f75 7470 7574  .```....**Output
+00001fe0: 2a2a 0d0a 0d0a 6060 6070 7974 686f 6e0d  **....```python.
+00001ff0: 0a5b 302c 2032 2c20 342c 2036 2c20 385d  .[0, 2, 4, 6, 8]
+00002000: 0d0a 6060 600d 0a0d 0a54 6869 7320 7769  ..```....This wi
+00002010: 6c6c 2065 7865 6375 7465 2074 6865 2066  ll execute the f
+00002020: 756e 6374 696f 6e20 6173 2073 6f6f 6e20  unction as soon 
+00002030: 6173 2079 6f75 2072 756e 2079 6f75 7220  as you run your 
+00002040: 7079 7468 6f6e 2063 6f64 652c 2069 6e20  python code, in 
+00002050: 7468 6973 2063 6173 6520 7765 2061 7265  this case we are
+00002060: 2074 7279 696e 6720 746f 2070 6572 666f   trying to perfo
+00002070: 726d 2074 6865 2073 616d 6520 7461 736b  rm the same task
+00002080: 2066 6976 6520 7469 6d65 7320 696e 2061   five times in a
+00002090: 2072 6f77 2063 6f6e 6375 7272 656e 746c   row concurrentl
+000020a0: 792e 2054 6865 2066 696e 616c 206f 7574  y. The final out
+000020b0: 7075 7420 6f66 2061 6c6c 2074 6865 2066  put of all the f
+000020c0: 756e 6374 696f 6e20 6361 6e20 6265 2061  unction can be a
+000020d0: 6363 6573 7365 6420 6279 2060 656a 7472  ccessed by `ejtr
+000020e0: 6164 6572 5448 2e72 6573 756c 745b 2766  aderTH.result['f
+000020f0: 756e 6374 696f 6e5f 6e61 6d65 275d 602e  unction_name']`.
+00002100: 204e 6f74 6963 6520 6966 2079 6f75 2073   Notice if you s
+00002110: 6574 2079 6f75 7220 6675 6e63 7469 6f6e  et your function
+00002120: 206f 6e20 7265 7065 6174 2069 7420 7769   on repeat it wi
+00002130: 6c6c 2061 6c77 6179 7320 7265 6365 6976  ll always receiv
+00002140: 6520 6120 7061 7261 6d65 7465 7220 7768  e a parameter wh
+00002150: 6963 6820 6973 2069 7427 7320 7468 7265  ich is it's thre
+00002160: 6164 206e 756d 6265 722e 0d0a 0d0a 2d2d  ad number.....--
+00002170: 2d0d 0a0d 0a2a 2a45 7861 6d70 6c65 2032  -....**Example 2
+00002180: 2a2a 0d0a 0d0a 6060 6070 7974 686f 6e0d  **....```python.
+00002190: 0a69 6d70 6f72 7420 656a 7472 6164 6572  .import ejtrader
+000021a0: 5448 0d0a 696d 706f 7274 2074 696d 650d  TH..import time.
+000021b0: 0a0d 0a40 656a 7472 6164 6572 5448 2e72  ...@ejtraderTH.r
+000021c0: 756e 2864 6174 613d 5b31 2c32 2c33 2c34  un(data=[1,2,3,4
+000021d0: 2c35 2c36 5d2c 206d 6178 5f74 6872 6561  ,5,6], max_threa
+000021e0: 6473 3d35 290d 0a64 6566 206d 795f 6675  ds=5)..def my_fu
+000021f0: 6e63 2869 293a 0d0a 2020 2020 7469 6d65  nc(i):..    time
+00002200: 2e73 6c65 6570 2831 290d 0a20 2020 2072  .sleep(1)..    r
+00002210: 6574 7572 6e20 692a 320d 0a0d 0a70 7269  eturn i*2....pri
+00002220: 6e74 2865 6a74 7261 6465 7254 482e 7265  nt(ejtraderTH.re
+00002230: 7375 6c74 5b27 6d79 5f66 756e 6327 5d29  sult['my_func'])
+00002240: 0d0a 6060 600d 0a0d 0a2a 2a4f 7574 7075  ..```....**Outpu
+00002250: 742a 2a0d 0a0d 0a60 6060 7079 7468 6f6e  t**....```python
+00002260: 0d0a 5b32 2c20 342c 2036 2c20 382c 2031  ..[2, 4, 6, 8, 1
+00002270: 302c 2031 325d 0d0a 6060 600d 0a0d 0a49  0, 12]..```....I
+00002280: 6e20 7468 6973 2063 6173 6520 7765 2061  n this case we a
+00002290: 7265 2064 6972 6563 746c 7920 7061 7373  re directly pass
+000022a0: 696e 6720 6f75 7220 6172 6775 6d65 6e74  ing our argument
+000022b0: 7320 696e 2061 206c 6973 7420 7669 6120  s in a list via 
+000022c0: 6465 636f 7261 746f 7220 616e 6420 7265  decorator and re
+000022d0: 6365 6976 696e 6720 7468 6520 7265 7375  ceiving the resu
+000022e0: 6c74 2073 616d 6520 7761 7920 6173 2077  lt same way as w
+000022f0: 6520 6469 6420 696e 2070 7265 7669 6f75  e did in previou
+00002300: 7320 6578 616d 706c 652e 0d0a 0d0a 2d2d  s example.....--
+00002310: 2d0d 0a0d 0a2a 2a45 7861 6d70 6520 332a  -....**Exampe 3*
+00002320: 2a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  *....```python..
+00002330: 696d 706f 7274 2065 6a74 7261 6465 7254  import ejtraderT
+00002340: 480d 0a69 6d70 6f72 7420 7469 6d65 0d0a  H..import time..
+00002350: 0d0a 4065 6a74 7261 6465 7254 482e 7365  ..@ejtraderTH.se
+00002360: 7428 6d61 785f 7468 7265 6164 733d 3130  t(max_threads=10
+00002370: 290d 0a64 6566 206d 795f 6675 6e63 2869  )..def my_func(i
+00002380: 293a 0d0a 2020 2020 7469 6d65 2e73 6c65  ):..    time.sle
+00002390: 6570 2831 290d 0a20 2020 2072 6574 7572  ep(1)..    retur
+000023a0: 6e20 692a 320d 0a0d 0a72 6573 756c 7420  n i*2....result 
+000023b0: 3d20 6d79 5f66 756e 6328 7265 7065 6174  = my_func(repeat
+000023c0: 3d37 290d 0a70 7269 6e74 2872 6573 756c  =7)..print(resul
+000023d0: 7429 0d0a 6060 600d 0a0d 0a2a 2a4f 7574  t)..```....**Out
+000023e0: 7075 742a 2a0d 0a0d 0a60 6060 7079 7468  put**....```pyth
+000023f0: 6f6e 0d0a 5b30 2c20 322c 2034 2c20 362c  on..[0, 2, 4, 6,
+00002400: 2038 2c20 3130 2c20 3132 5d0d 0a60 6060   8, 10, 12]..```
+00002410: 0d0a 0d0a 5468 6973 2069 7320 616e 2061  ....This is an a
+00002420: 6e6f 7468 6572 2063 6f6f 6c20 7761 7920  nother cool way 
+00002430: 746f 2066 6972 7374 2063 6f6e 7665 7274  to first convert
+00002440: 2079 6f75 7220 6675 6e63 7469 6f6e 2069   your function i
+00002450: 6e20 636f 6e63 7572 7265 6e74 2066 756e  n concurrent fun
+00002460: 6374 696f 6e20 616e 6420 7468 656e 2070  ction and then p
+00002470: 6173 7369 6e67 2074 6865 2061 7267 756d  assing the argum
+00002480: 656e 7420 6173 2068 6f77 206d 616e 7920  ent as how many 
+00002490: 7469 6d65 2079 6f75 2077 616e 7420 746f  time you want to
+000024a0: 2065 7865 6375 7465 2074 6861 7420 6675   execute that fu
+000024b0: 6e63 7469 6f6e 2061 6c6c 2069 6e20 7061  nction all in pa
+000024c0: 7261 6c6c 656c 2e0d 0a0d 0a2d 2d2d 0d0a  rallel.....---..
+000024d0: 0d0a 2a2a 4578 616d 706c 6520 342a 2a0d  ..**Example 4**.
+000024e0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  ...```python..im
+000024f0: 706f 7274 2065 6a74 7261 6465 7254 480d  port ejtraderTH.
+00002500: 0a69 6d70 6f72 7420 7469 6d65 0d0a 0d0a  .import time....
+00002510: 4065 6a74 7261 6465 7254 482e 7365 7428  @ejtraderTH.set(
+00002520: 290d 0a64 6566 206d 795f 6675 6e63 2869  )..def my_func(i
+00002530: 293a 0d0a 2020 2020 7469 6d65 2e73 6c65  ):..    time.sle
+00002540: 6570 2831 290d 0a20 2020 2072 6574 7572  ep(1)..    retur
+00002550: 6e20 692a 320d 0a0d 0a72 6573 756c 7420  n i*2....result 
+00002560: 3d20 6d79 5f66 756e 6328 5b35 2c36 2c37  = my_func([5,6,7
+00002570: 5d29 0d0a 7072 696e 7428 7265 7375 6c74  ])..print(result
+00002580: 290d 0a60 6060 0d0a 0d0a 2a2a 4f75 7470  )..```....**Outp
+00002590: 7574 2a2a 0d0a 0d0a 6060 6070 7974 686f  ut**....```pytho
+000025a0: 6e0d 0a5b 3130 2c20 3132 2c20 3134 5d0d  n..[10, 12, 14].
+000025b0: 0a60 6060 0d0a 0d0a 4167 6169 6e20 7765  .```....Again we
+000025c0: 2063 616e 2061 6c73 6f20 7370 6563 6966   can also specif
+000025d0: 7920 7768 6174 2061 7267 756d 656e 7473  y what arguments
+000025e0: 2077 6520 7761 6e74 2074 6f20 7061 7373   we want to pass
+000025f0: 2074 6f20 7468 6520 6675 6e63 7469 6f6e   to the function
+00002600: 2074 6f20 7072 6f63 6573 7320 6974 2063   to process it c
+00002610: 6f6e 6375 7272 656e 746c 792e 2069 6620  oncurrently. if 
+00002620: 696e 2074 6865 2060 4065 6a74 7261 6465  in the `@ejtrade
+00002630: 7254 482e 7365 7428 2960 2064 6563 6f72  rTH.set()` decor
+00002640: 6174 6f72 2079 6f75 2077 6f6e 2774 2070  ator you won't p
+00002650: 6173 7320 616e 7920 606d 6178 5f74 6872  ass any `max_thr
+00002660: 6561 6473 6020 6172 6775 6d65 6e74 2060  eads` argument `
+00002670: 6d61 785f 7468 7265 6164 733d 3130 6020  max_threads=10` 
+00002680: 7769 6c6c 2062 6520 7365 742e 0d0a 0d0a  will be set.....
+00002690: 2323 2323 2048 616e 646c 696e 6720 6572  #### Handling er
+000026a0: 726f 7273 2061 6e64 206b 696c 6c69 6e67  rors and killing
+000026b0: 2061 6c6c 2074 6872 6561 6473 0d0a 0d0a   all threads....
+000026c0: 536f 2c20 6279 2064 6566 6175 6c74 2069  So, by default i
+000026d0: 6620 616e 7920 6572 726f 7220 6f63 6375  f any error occu
+000026e0: 7273 2074 6865 2074 6872 6561 6473 2077  rs the threads w
+000026f0: 696c 6c20 6b65 6570 206f 6e20 7275 6e6e  ill keep on runn
+00002700: 696e 672c 2069 6e20 6361 7365 2069 6620  ing, in case if 
+00002710: 796f 7520 7761 6e74 2074 6f20 6967 6e6f  you want to igno
+00002720: 7265 2073 6f6d 6520 6572 726f 7273 2062  re some errors b
+00002730: 7574 2069 6620 796f 7520 7761 6e74 2074  ut if you want t
+00002740: 6f20 6b69 6c6c 2061 6c6c 2074 6865 2074  o kill all the t
+00002750: 6872 6561 6420 6174 206f 6e63 6520 796f  hread at once yo
+00002760: 7520 6361 6e20 7573 6520 6065 6a74 7261  u can use `ejtra
+00002770: 6465 7254 482e 7374 6f70 2829 6020 7768  derTH.stop()` wh
+00002780: 696c 6520 6861 6e64 6c69 6e67 2065 7272  ile handling err
+00002790: 6f72 732e 0d0a 0d0a 6060 6070 7974 686f  ors.....```pytho
+000027a0: 6e0d 0a23 7468 6520 6675 6e63 7469 6f6e  n..#the function
+000027b0: 2066 6f72 2070 726f 6365 7373 696e 6720   for processing 
+000027c0: 6461 7461 0d0a 6465 6620 6d79 5f66 756e  data..def my_fun
+000027d0: 6328 6461 7461 293a 0d0a 2020 2020 7468  c(data):..    th
+000027e0: 7265 6164 5f6e 756d 6265 7220 3d20 656a  read_number = ej
+000027f0: 7472 6164 6572 5448 2e63 6f6e 736f 6c65  traderTH.console
+00002800: 5f6c 6f67 286f 7574 7075 743d 5472 7565  _log(output=True
+00002810: 290d 0a20 2020 2074 7279 3a0d 0a20 2020  )..    try:..   
+00002820: 2020 2020 2064 6174 6120 3d20 7265 7175       data = requ
+00002830: 6573 7473 2e67 6574 2822 6874 7470 3a2f  ests.get("http:/
+00002840: 2f68 7474 7062 696e 2e6f 7267 2f67 6574  /httpbin.org/get
+00002850: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00002860: 726e 2064 6174 610d 0a20 2020 2065 7863  rn data..    exc
+00002870: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00002880: 2065 3a0d 0a20 2020 2020 2020 2070 7269   e:..        pri
+00002890: 6e74 2865 2920 2370 7269 6e74 696e 6720  nt(e) #printing 
+000028a0: 6f74 6865 7220 6572 726f 7273 0d0a 2020  other errors..  
+000028b0: 2020 2020 2020 236b 696c 6c69 6e67 2061        #killing a
+000028c0: 6c6c 2061 6374 6976 6520 7468 7265 6164  ll active thread
+000028d0: 730d 0a20 2020 2020 2020 2065 6a74 7261  s..        ejtra
+000028e0: 6465 7254 482e 7374 6f70 2829 2023 7573  derTH.stop() #us
+000028f0: 6520 746f 206b 696c 6c20 616c 6c20 7468  e to kill all th
+00002900: 7265 6164 730d 0a60 6060 0d0a 0d0a 6966  reads..```....if
+00002910: 2079 6f75 2064 6f6e 2774 2075 7365 2060   you don't use `
+00002920: 656a 7472 6164 6572 5448 2e73 746f 7028  ejtraderTH.stop(
+00002930: 2960 2066 756e 6374 696f 6e20 7468 656e  )` function then
+00002940: 2074 6865 2074 6872 6561 6473 2077 696c   the threads wil
+00002950: 6c20 6b65 6570 206f 6e20 7275 6e6e 696e  l keep on runnin
+00002960: 6720 616e 6420 6669 6c6c 696e 6720 604e  g and filling `N
+00002970: 6f6e 6560 2069 6e20 706c 6163 6520 6f66  one` in place of
+00002980: 2072 6574 7572 6e65 6420 6461 7461 2e20   returned data. 
+00002990: 6966 2079 6f75 2075 7365 6420 7468 6520  if you used the 
+000029a0: 6065 6a74 7261 6465 7254 482e 7374 6f70  `ejtraderTH.stop
+000029b0: 2829 6020 6974 2077 696c 6c20 6b69 6c6c  ()` it will kill
+000029c0: 2061 6c6c 2061 6374 6976 6520 7468 7265   all active thre
+000029d0: 6164 7320 696d 6d65 6469 6174 656c 7920  ads immediately 
+000029e0: 616e 6420 7769 6c6c 2072 6574 7572 6e20  and will return 
+000029f0: 7468 6520 6461 7461 2074 6861 7420 7765  the data that we
+00002a00: 7265 2070 726f 6365 7373 6564 2062 7920  re processed by 
+00002a10: 796f 7572 2066 756e 6374 696f 6e20 736f  your function so
+00002a20: 2066 6172 2e0d 0a                         far...
```

### Comparing `ejtraderTH-1.0.3/ejtraderTH/__init__.py` & `ejtraderTH-1.0.4/ejtraderTH/__init__.py`

 * *Files identical despite different names*

### Comparing `ejtraderTH-1.0.3/ejtraderTH/ejtraderTH.py` & `ejtraderTH-1.0.4/ejtraderTH/ejtraderTH.py`

 * *Files identical despite different names*

### Comparing `ejtraderTH-1.0.3/ejtraderTH.egg-info/PKG-INFO` & `ejtraderTH-1.0.4/ejtraderTH.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,325 +1,329 @@
 Metadata-Version: 2.1
 Name: ejtraderTH
-Version: 1.0.3
+Version: 1.0.4
 Summary: This tiny little python module is useful for creating multiple threads of any function in seconds.
 Home-page: https://ejtraderTH_mt.readthedocs.io/
+Download-URL: https://ejtraderTH.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: MIT License
-Download-URL: https://ejtraderTH.com
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderTH_mt/issues
 Project-URL: Source, https://github.com/traderpedroso/ejtraderTH_mt
 Project-URL: Documentation, https://ejtraderTH.readthedocs.io/
-Description: ```python
-        pip install ejtraderTH
-        ```
-        
-        This tiny little python module is useful for creating multiple threads of any function in seconds.
-        
-        #### What's new in v1.0
-        
-        A quick launch mode is added, just type `ejtraderTH.start(func_name, repeat=10)` and it will execute the given function given number of times in parallel. A standard way of measuring elapsed time is added as well. see examples below to understand how to use quick launch mode.
-        
-        After using this library for a number of times in various projects i found that if you pass in lots of data say `1000` data in a list, it was creating `1000` threads to do it all once, how ever in the practical world most of the times cpu's are not capable of creating so many threads at once or worse it eats up all resources at once. To prevent this problem now you can pass in `max_threads` value by default if you don't pass in the value it will automatically be set equal to 4 just for the safety purpose, and passing a `0` value will throw an error while creating a `ejtraderTH` object this way it will only create specified number of threads at once and will wait untill the previously started threads has finished their job.
-        
-        Other than that to keep a track on how many threads are been created in real time you can push in a new log method inn you processing function so that whenever a new thread is created you can see it, there ar two methods of tracking them.
-        
-        - just to print out the thread number which is being created, use: ` ejtraderTH.console_log(output=True)`
-        - if you want to store it in some variable you can use: `thread_number = ejtraderTH.console_log()`
-        - in case some error occurs, the thread will keep on running
-        - if you want to kill all the threads use `ejtraderTH.stop()` inside your processing function while handling errors.
-        
-        #### Problem Statement
-        
-        - Let say for example, we have a `list` of numbers from `1 to 10` and all we wanted to do is `multiply every number by 1000` but the challenge is `it takes 5 sec` for multiplying a single number by 1000 from the list, I know its an arbitary condition, but we can create it with `time.sleep(5)` function.
-        - Or you want to make a web request million times, without waiting for the server to respond you to make the next request.
-        
-        #### Working
-        
-        So what this module does is, at the time of object initialization it takes in the function which is used for processing data and max number of thread which can be created at once, when running in multi threads, and as input it takes a list of arguments for which multiple threads will be created.
-        
-        ---
-        
-        #### Example 1
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        #the function for processing data
-        def my_func(data):
-            print(f'>> Running Thread {ejtraderTH.console_log()}')
-            data = data*1000
-            time.sleep(5)
-            return data
-        
-        #list of input data for processing
-        raw_data = [1,2,3,4,5,6,7,8,9,10]
-        
-        #sending arguments for asynchronous multi thread processing
-        processed_data = ejtraderTH.start(my_func, data=raw_data, max_threads=10)
-        
-        #printing the synchronised received results
-        print()
-        print(f'>> Input: {raw_data}')
-        print(f'>> Result: {processed_data}')
-        print(f'>> Elapsed time: {ejtraderTH.elapsed()} sec')
-        ```
-        
-        #### output
-        
-        ```python
-        >> Running Thread 1
-        >> Running Thread 2
-        >> Running Thread 3
-        >> Running Thread 4
-        >> Running Thread 5
-        >> Running Thread 6
-        >> Running Thread 7
-        >> Running Thread 8
-        >> Running Thread 9
-        >> Running Thread 10
-        
-        >> Input: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
-        >> Result: [1000, 2000, 3000, 4000, 5000, 6000, 7000, 8000, 9000, 10000]
-        >> Elapsed time: 5.0 sec
-        ```
-        
-        Now you can clearly see, if we do it without multi threading it would have taken around `50 Seconds` for processing the data while doing the task one by one and waiting for `5 Sec` after running the function each time. but since we are doing it with multithreading it will take only `5 Seconds` for processing the same task with different data, in their individual threads.
-        
-        #### Example 2
-        
-        ```python
-        #the function for processing data
-        def my_func(data):
-            ejtraderTH.console_log(output=True)
-            ip = req.request(method='GET',url="http://ipinfo.io/ip")
-        
-            return ip.content
-        
-        #sending arguments for asynchronous multi thread processing
-        processed_data = ejtraderTH.start(my_func, repeat=20, max_threads=20)
-        
-        #printing the synchronised received results
-        print()
-        print(f'>> Result: {processed_data}')
-        ejtraderTH.elapsed(output=True)
-        ```
-        
-        #### output
-        
-        ```python
-        >> Creating Threads 1
-        >> Creating Threads 2
-        >> Creating Threads 3
-        >> Creating Threads 4
-        >> Creating Threads 5
-        >> Creating Threads 6
-        >> Creating Threads 7
-        >> Creating Threads 8
-        >> Creating Threads 9
-        >> Creating Threads 10
-        >> Creating Threads 11
-        >> Creating Threads 12
-        >> Creating Threads 13
-        >> Creating Threads 14
-        >> Creating Threads 15
-        >> Creating Threads 16
-        >> Creating Threads 17
-        >> Creating Threads 18
-        >> Creating Threads 19
-        >> Creating Threads 20
-        
-        >> Result: [b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37']
-        >> Elapsed time: 0.31 sec
-        ```
-        
-        In this example we didn't used time.sleep() instead we make a request to the webserver and it took `0.5 seconds` to get the result back so we did it 20 times with multi threading and were able to receive the results in less time in a synchronous order.
-        
-        > Lets try to do it without multithreading and see how it affects the processing time.
-        
-        So in this new update `ejtraderTH v1.0` we can specify that at once how many threads should be created so lets change the input parameter as `max_threads = 1` this way it will only create one thread at a time and will wait until the previous thread has finished properly.
-        
-        #### output
-        
-        ```python
-        .
-        .
-        .
-        >> Elapsed time: 6.43 sec
-        ```
-        
-        It is clear that every request to the server was taking approx. `0.5 seconds` so while making one request at a time it took `6.43 seconds` as expected.
-        
-        ### Example 3
-        
-        Quick Launch mode, a new feature is added where you can directly use ejtraderTH to pass in the repetitive function, input data for those functions and how many threads you want it to create at a time. other than that if you just want it to repeat the function without any inputs you can do that too.
-        
-        ```python
-        import ejtraderTH
-        import time
-        import random
-        
-        names = ['April', 'May']
-        
-        #the function for processing data
-        def my_func(data):
-            ejtraderTH.console_log(output=True)
-            time.sleep(1)
-            name = random.choice(names)
-            return f'{name} says, Hello World!'
-        
-        processed_data = ejtraderTH.start(my_func, repeat=4)
-        
-        print(processed_data)
-        ejtraderTH.elapsed(output=True)
-        ```
-        
-        ### output
-        
-        ```
-        >> Creating Threads 1
-        >> Creating Threads 2
-        >> Creating Threads 3
-        >> Creating Threads 4
-        ['May says, Hello World!', 'April says, Hello World!', 'May says, Hello World!', 'April says, Hello World!']
-        >> Elapsed time: 1.0 sec
-        ```
-        
-        we kept a time gap of 1 sec inside the function still it repeated the task 4 times in same time. since it can access the global variables we can assign certain tasks that don't need different inputs every time.
-        
-        ### Decorators support
-        
-        Apart from calling the `start()` attribute we can also use decorators to explicitly make our functions for concurrent execution.
-        
-        **Example 1**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.run(repeat=5, max_threads=5)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        print(ejtraderTH.result['my_func'])
-        ```
-        
-        **Output**
-        
-        ```python
-        [0, 2, 4, 6, 8]
-        ```
-        
-        This will execute the function as soon as you run your python code, in this case we are trying to perform the same task five times in a row concurrently. The final output of all the function can be accessed by `ejtraderTH.result['function_name']`. Notice if you set your function on repeat it will always receive a parameter which is it's thread number.
-        
-        ---
-        
-        **Example 2**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.run(data=[1,2,3,4,5,6], max_threads=5)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        print(ejtraderTH.result['my_func'])
-        ```
-        
-        **Output**
-        
-        ```python
-        [2, 4, 6, 8, 10, 12]
-        ```
-        
-        In this case we are directly passing our arguments in a list via decorator and receiving the result same way as we did in previous example.
-        
-        ---
-        
-        **Exampe 3**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.set(max_threads=10)
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        result = my_func(repeat=7)
-        print(result)
-        ```
-        
-        **Output**
-        
-        ```python
-        [0, 2, 4, 6, 8, 10, 12]
-        ```
-        
-        This is an another cool way to first convert your function in concurrent function and then passing the argument as how many time you want to execute that function all in parallel.
-        
-        ---
-        
-        **Example 4**
-        
-        ```python
-        import ejtraderTH
-        import time
-        
-        @ejtraderTH.set()
-        def my_func(i):
-            time.sleep(1)
-            return i*2
-        
-        result = my_func([5,6,7])
-        print(result)
-        ```
-        
-        **Output**
-        
-        ```python
-        [10, 12, 14]
-        ```
-        
-        Again we can also specify what arguments we want to pass to the function to process it concurrently. if in the `@ejtraderTH.set()` decorator you won't pass any `max_threads` argument `max_threads=10` will be set.
-        
-        #### Handling errors and killing all threads
-        
-        So, by default if any error occurs the threads will keep on running, in case if you want to ignore some errors but if you want to kill all the thread at once you can use `ejtraderTH.stop()` while handling errors.
-        
-        ```python
-        #the function for processing data
-        def my_func(data):
-            thread_number = ejtraderTH.console_log(output=True)
-            try:
-                data = requests.get("http://httpbin.org/get")
-                return data
-            except Exception as e:
-                print(e) #printing other errors
-                #killing all active threads
-                ejtraderTH.stop() #use to kill all threads
-        ```
-        
-        if you don't use `ejtraderTH.stop()` function then the threads will keep on running and filling `None` in place of returned data. if you used the `ejtraderTH.stop()` it will kill all active threads immediately and will return the data that were processed by your function so far.
-        
 Keywords: metatrader,f-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-Provides-Extra: docs
+License-File: LICENSE.txt
+
+
+![Pypi Publish](https://github.com/ejtraderLabs/ejtraderTH/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderTH)
+[![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderTH)](https://github.com/ejtraderLabs/ejtraderTH/blob/master/LICENSE)
+
+```python
+pip install ejtraderTH
+```
+
+This tiny little python module is useful for creating multiple threads of any function in seconds.
+
+#### What's new in v1.0
+
+A quick launch mode is added, just type `ejtraderTH.start(func_name, repeat=10)` and it will execute the given function given number of times in parallel. A standard way of measuring elapsed time is added as well. see examples below to understand how to use quick launch mode.
+
+After using this library for a number of times in various projects i found that if you pass in lots of data say `1000` data in a list, it was creating `1000` threads to do it all once, how ever in the practical world most of the times cpu's are not capable of creating so many threads at once or worse it eats up all resources at once. To prevent this problem now you can pass in `max_threads` value by default if you don't pass in the value it will automatically be set equal to 4 just for the safety purpose, and passing a `0` value will throw an error while creating a `ejtraderTH` object this way it will only create specified number of threads at once and will wait untill the previously started threads has finished their job.
+
+Other than that to keep a track on how many threads are been created in real time you can push in a new log method inn you processing function so that whenever a new thread is created you can see it, there ar two methods of tracking them.
+
+- just to print out the thread number which is being created, use: ` ejtraderTH.console_log(output=True)`
+- if you want to store it in some variable you can use: `thread_number = ejtraderTH.console_log()`
+- in case some error occurs, the thread will keep on running
+- if you want to kill all the threads use `ejtraderTH.stop()` inside your processing function while handling errors.
+
+#### Problem Statement
+
+- Let say for example, we have a `list` of numbers from `1 to 10` and all we wanted to do is `multiply every number by 1000` but the challenge is `it takes 5 sec` for multiplying a single number by 1000 from the list, I know its an arbitary condition, but we can create it with `time.sleep(5)` function.
+- Or you want to make a web request million times, without waiting for the server to respond you to make the next request.
+
+#### Working
+
+So what this module does is, at the time of object initialization it takes in the function which is used for processing data and max number of thread which can be created at once, when running in multi threads, and as input it takes a list of arguments for which multiple threads will be created.
+
+---
+
+#### Example 1
+
+```python
+import ejtraderTH
+import time
+
+#the function for processing data
+def my_func(data):
+    print(f'>> Running Thread {ejtraderTH.console_log()}')
+    data = data*1000
+    time.sleep(5)
+    return data
+
+#list of input data for processing
+raw_data = [1,2,3,4,5,6,7,8,9,10]
+
+#sending arguments for asynchronous multi thread processing
+processed_data = ejtraderTH.start(my_func, data=raw_data, max_threads=10)
+
+#printing the synchronised received results
+print()
+print(f'>> Input: {raw_data}')
+print(f'>> Result: {processed_data}')
+print(f'>> Elapsed time: {ejtraderTH.elapsed()} sec')
+```
+
+#### output
+
+```python
+>> Running Thread 1
+>> Running Thread 2
+>> Running Thread 3
+>> Running Thread 4
+>> Running Thread 5
+>> Running Thread 6
+>> Running Thread 7
+>> Running Thread 8
+>> Running Thread 9
+>> Running Thread 10
+
+>> Input: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+>> Result: [1000, 2000, 3000, 4000, 5000, 6000, 7000, 8000, 9000, 10000]
+>> Elapsed time: 5.0 sec
+```
+
+Now you can clearly see, if we do it without multi threading it would have taken around `50 Seconds` for processing the data while doing the task one by one and waiting for `5 Sec` after running the function each time. but since we are doing it with multithreading it will take only `5 Seconds` for processing the same task with different data, in their individual threads.
+
+#### Example 2
+
+```python
+#the function for processing data
+def my_func(data):
+    ejtraderTH.console_log(output=True)
+    ip = req.request(method='GET',url="http://ipinfo.io/ip")
+
+    return ip.content
+
+#sending arguments for asynchronous multi thread processing
+processed_data = ejtraderTH.start(my_func, repeat=20, max_threads=20)
+
+#printing the synchronised received results
+print()
+print(f'>> Result: {processed_data}')
+ejtraderTH.elapsed(output=True)
+```
+
+#### output
+
+```python
+>> Creating Threads 1
+>> Creating Threads 2
+>> Creating Threads 3
+>> Creating Threads 4
+>> Creating Threads 5
+>> Creating Threads 6
+>> Creating Threads 7
+>> Creating Threads 8
+>> Creating Threads 9
+>> Creating Threads 10
+>> Creating Threads 11
+>> Creating Threads 12
+>> Creating Threads 13
+>> Creating Threads 14
+>> Creating Threads 15
+>> Creating Threads 16
+>> Creating Threads 17
+>> Creating Threads 18
+>> Creating Threads 19
+>> Creating Threads 20
+
+>> Result: [b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37', b'200,234.182.37']
+>> Elapsed time: 0.31 sec
+```
+
+In this example we didn't used time.sleep() instead we make a request to the webserver and it took `0.5 seconds` to get the result back so we did it 20 times with multi threading and were able to receive the results in less time in a synchronous order.
+
+> Lets try to do it without multithreading and see how it affects the processing time.
+
+So in this new update `ejtraderTH v1.0` we can specify that at once how many threads should be created so lets change the input parameter as `max_threads = 1` this way it will only create one thread at a time and will wait until the previous thread has finished properly.
+
+#### output
+
+```python
+.
+.
+.
+>> Elapsed time: 6.43 sec
+```
+
+It is clear that every request to the server was taking approx. `0.5 seconds` so while making one request at a time it took `6.43 seconds` as expected.
+
+### Example 3
+
+Quick Launch mode, a new feature is added where you can directly use ejtraderTH to pass in the repetitive function, input data for those functions and how many threads you want it to create at a time. other than that if you just want it to repeat the function without any inputs you can do that too.
+
+```python
+import ejtraderTH
+import time
+import random
+
+names = ['April', 'May']
+
+#the function for processing data
+def my_func(data):
+    ejtraderTH.console_log(output=True)
+    time.sleep(1)
+    name = random.choice(names)
+    return f'{name} says, Hello World!'
+
+processed_data = ejtraderTH.start(my_func, repeat=4)
+
+print(processed_data)
+ejtraderTH.elapsed(output=True)
+```
+
+### output
+
+```
+>> Creating Threads 1
+>> Creating Threads 2
+>> Creating Threads 3
+>> Creating Threads 4
+['May says, Hello World!', 'April says, Hello World!', 'May says, Hello World!', 'April says, Hello World!']
+>> Elapsed time: 1.0 sec
+```
+
+we kept a time gap of 1 sec inside the function still it repeated the task 4 times in same time. since it can access the global variables we can assign certain tasks that don't need different inputs every time.
+
+### Decorators support
+
+Apart from calling the `start()` attribute we can also use decorators to explicitly make our functions for concurrent execution.
+
+**Example 1**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.run(repeat=5, max_threads=5)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+print(ejtraderTH.result['my_func'])
+```
+
+**Output**
+
+```python
+[0, 2, 4, 6, 8]
+```
+
+This will execute the function as soon as you run your python code, in this case we are trying to perform the same task five times in a row concurrently. The final output of all the function can be accessed by `ejtraderTH.result['function_name']`. Notice if you set your function on repeat it will always receive a parameter which is it's thread number.
+
+---
+
+**Example 2**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.run(data=[1,2,3,4,5,6], max_threads=5)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+print(ejtraderTH.result['my_func'])
+```
+
+**Output**
+
+```python
+[2, 4, 6, 8, 10, 12]
+```
+
+In this case we are directly passing our arguments in a list via decorator and receiving the result same way as we did in previous example.
+
+---
+
+**Exampe 3**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.set(max_threads=10)
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+result = my_func(repeat=7)
+print(result)
+```
+
+**Output**
+
+```python
+[0, 2, 4, 6, 8, 10, 12]
+```
+
+This is an another cool way to first convert your function in concurrent function and then passing the argument as how many time you want to execute that function all in parallel.
+
+---
+
+**Example 4**
+
+```python
+import ejtraderTH
+import time
+
+@ejtraderTH.set()
+def my_func(i):
+    time.sleep(1)
+    return i*2
+
+result = my_func([5,6,7])
+print(result)
+```
+
+**Output**
+
+```python
+[10, 12, 14]
+```
+
+Again we can also specify what arguments we want to pass to the function to process it concurrently. if in the `@ejtraderTH.set()` decorator you won't pass any `max_threads` argument `max_threads=10` will be set.
+
+#### Handling errors and killing all threads
+
+So, by default if any error occurs the threads will keep on running, in case if you want to ignore some errors but if you want to kill all the thread at once you can use `ejtraderTH.stop()` while handling errors.
+
+```python
+#the function for processing data
+def my_func(data):
+    thread_number = ejtraderTH.console_log(output=True)
+    try:
+        data = requests.get("http://httpbin.org/get")
+        return data
+    except Exception as e:
+        print(e) #printing other errors
+        #killing all active threads
+        ejtraderTH.stop() #use to kill all threads
+```
+
+if you don't use `ejtraderTH.stop()` function then the threads will keep on running and filling `None` in place of returned data. if you used the `ejtraderTH.stop()` it will kill all active threads immediately and will return the data that were processed by your function so far.
```

### Comparing `ejtraderTH-1.0.3/setup.py` & `ejtraderTH-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderTH',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     url='https://ejtraderTH_mt.readthedocs.io/',
     download_url='https://ejtraderTH.com',
     license='MIT License',
     author='Emerson Pedroso',
     author_email='support@ejtrader.com',
     description='This tiny little python module is useful for creating multiple threads of any function in seconds.',
@@ -39,17 +39,14 @@
         "Intended Audience :: Developers",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries"
     ],
     python_requires='>=3',
-    extras_require={
-        "docs": requirements(filename='docs/requirements.txt')
-    },
     keywords=', '.join([
         'metatrader', 'f-api', 'historical-data',
         'financial-data', 'stocks', 'funds', 'etfs',
         'indices', 'currency crosses', 'bonds', 'commodities',
         'crypto currencies'
     ]),
     project_urls={
```

