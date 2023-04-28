# Comparing `tmp/pycotap-1.2.2.tar.gz` & `tmp/pycotap-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycotap-1.2.2.tar", last modified: Mon Nov  4 12:36:17 2019, max compression
+gzip compressed data, was "pycotap-1.3.0.tar", last modified: Fri Apr 28 10:27:44 2023, max compression
```

## Comparing `pycotap-1.2.2.tar` & `pycotap-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2019-11-04 12:36:17.000000 pycotap-1.2.2/
--rw-r--r--   0 remko      (501) staff       (20)     1080 2015-01-21 16:26:27.000000 pycotap-1.2.2/COPYING
--rw-r--r--   0 remko      (501) staff       (20)     1957 2019-11-04 12:36:17.000000 pycotap-1.2.2/PKG-INFO
--rw-r--r--   0 remko      (501) staff       (20)     5099 2019-11-02 11:09:07.000000 pycotap-1.2.2/README.md
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap/
--rw-r--r--   0 remko      (501) staff       (20)     4891 2019-11-02 11:09:07.000000 pycotap-1.2.2/pycotap/__init__.py
--rw-r--r--   0 remko      (501) staff       (20)      119 2019-11-02 11:09:07.000000 pycotap-1.2.2/pycotap/__main__.py
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap.egg-info/
--rw-r--r--   0 remko      (501) staff       (20)     1957 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap.egg-info/PKG-INFO
--rw-r--r--   0 remko      (501) staff       (20)      203 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap.egg-info/SOURCES.txt
--rw-r--r--   0 remko      (501) staff       (20)        1 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap.egg-info/dependency_links.txt
--rw-r--r--   0 remko      (501) staff       (20)        8 2019-11-04 12:36:17.000000 pycotap-1.2.2/pycotap.egg-info/top_level.txt
--rw-r--r--   0 remko      (501) staff       (20)       38 2019-11-04 12:36:17.000000 pycotap-1.2.2/setup.cfg
--rwxr-xr-x   0 remko      (501) staff       (20)     1953 2019-11-04 12:35:43.000000 pycotap-1.2.2/setup.py
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2019-11-04 12:36:17.000000 pycotap-1.2.2/test/
--rw-r--r--   0 remko      (501) staff       (20)     9349 2019-11-02 11:09:07.000000 pycotap-1.2.2/test/test.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.201216 pycotap-1.3.0/
+-rw-r--r--   0 remko      (501) staff       (20)     1080 2015-01-21 16:26:27.000000 pycotap-1.3.0/COPYING
+-rw-r--r--   0 remko      (501) staff       (20)     1756 2023-04-28 10:27:44.201019 pycotap-1.3.0/PKG-INFO
+-rw-r--r--   0 remko      (501) staff       (20)     5480 2023-04-28 10:24:45.000000 pycotap-1.3.0/README.md
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.199351 pycotap-1.3.0/pycotap/
+-rw-r--r--   0 remko      (501) staff       (20)     4948 2023-04-28 10:05:29.000000 pycotap-1.3.0/pycotap/__init__.py
+-rw-r--r--   0 remko      (501) staff       (20)      123 2023-04-28 09:54:31.000000 pycotap-1.3.0/pycotap/__main__.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.200515 pycotap-1.3.0/pycotap.egg-info/
+-rw-r--r--   0 remko      (501) staff       (20)     1756 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/PKG-INFO
+-rw-r--r--   0 remko      (501) staff       (20)      218 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/SOURCES.txt
+-rw-r--r--   0 remko      (501) staff       (20)        1 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/dependency_links.txt
+-rw-r--r--   0 remko      (501) staff       (20)        8 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/top_level.txt
+-rw-r--r--   0 remko      (501) staff       (20)      869 2023-04-28 10:16:29.000000 pycotap-1.3.0/pyproject.toml
+-rw-r--r--   0 remko      (501) staff       (20)       38 2023-04-28 10:27:44.201273 pycotap-1.3.0/setup.cfg
+-rwxr-xr-x   0 remko      (501) staff       (20)     1977 2023-04-28 10:25:08.000000 pycotap-1.3.0/setup.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.200741 pycotap-1.3.0/test/
+-rw-r--r--   0 remko      (501) staff       (20)    10365 2023-04-28 10:16:27.000000 pycotap-1.3.0/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycotap-1.2.2/COPYING` & `pycotap-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `pycotap-1.2.2/PKG-INFO` & `pycotap-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pycotap
-Version: 1.2.2
+Version: 1.3.0
 Summary: A tiny test runner that outputs TAP results to standard output.
 Home-page: https://el-tramo.be/pycotap
 Author: Remko Tronçon
 Author-email: dev@el-tramo.be
 License: MIT
-Description: 
-        `pycotap` is a simple Python test runner for ``unittest`` that outputs 
-        `Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
-        
-        Contrary to other TAP runners for Python, ``pycotap`` ...
-        
-        - ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
-          allowing you to pipe it directly to TAP pretty printers and processors 
-          (such as the ones listed on
-          `the tape page <https://www.npmjs.com/package/tape#pretty-reporters>`_). By
-          piping it to other consumers, you can avoid the need to add 
-          specific test runners to your test code. Since the TAP results
-          are printed as they come in, the consumers can directly display results while 
-          the tests are run.
-        
-        - ... only contains a TAP reporter, so no parsers, no frameworks, no dependencies, ...
-        
-        - ... is configurable: you can choose how you want the test output and test result
-          diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
-          attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
-          flow.
-        
-        Documentation and examples can be found on `the pycotap page 
-        <https://el-tramo.be/pycotap>`_.
-        
 Keywords: tap unittest testing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+License-File: COPYING
+
+
+`pycotap` is a simple Python test runner for ``unittest`` that outputs 
+`Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
+
+Contrary to other TAP runners for Python, ``pycotap`` ...
+
+- ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
+  allowing you to pipe it directly to TAP pretty printers and processors 
+  (such as the ones listed on
+  `the tape page <https://www.npmjs.com/package/tape#pretty-reporters>`_). By
+  piping it to other consumers, you can avoid the need to add 
+  specific test runners to your test code. Since the TAP results
+  are printed as they come in, the consumers can directly display results while 
+  the tests are run.
+
+- ... only contains a TAP reporter, so no parsers, no frameworks, no dependencies, ...
+
+- ... is configurable: you can choose how you want the test output and test result
+  diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
+  attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
+  flow.
+
+Documentation and examples can be found on `the pycotap page 
+<https://el-tramo.be/pycotap>`_.
```

### Comparing `pycotap-1.2.2/README.md` & `pycotap-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-# [pycotap: Tiny Python TAP Test Runner](https://el-tramo.be/pycotap)
+# pycotap: Tiny Python TAP Test Runner
 
-`pycotap` is a simple Python test runner for ``unittest`` that outputs 
-[Test Anything Protocol](http://testanything.org) results to standard output 
-(similar to what [`tape`](https://www.npmjs.com/package/tape) does for JavaScript).
+[![Build](https://github.com/remko/pycotap/actions/workflows/build.yml/badge.svg)](https://github.com/remko/pycotap/actions/workflows/build.yml)
+[![PyPI
+version](https://badge.fury.io/py/pycotap.svg)](https://badge.fury.io/py/pycotap)
+
+`pycotap` is a simple Python test runner for `unittest` that outputs
+[Test Anything Protocol](http://testanything.org) results to standard
+output (similar to what [`tape`](https://www.npmjs.com/package/tape)
+does for JavaScript).
 
 Contrary to other TAP runners for Python, `pycotap` ...
 
-- ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
-  allowing you to pipe it directly to TAP pretty printers and processors 
-  (such as the ones listed on
-  the [`tape` page](https://www.npmjs.com/package/tape#pretty-reporters)). By
-  piping it to other consumers, you can avoid the need to add 
-  specific test runners to your test code. Since the TAP results
-  are printed as they come in, the consumers can directly display results while 
-  the tests are run.
-- ... only contains a TAP reporter, so no parsers, no frameworks, no dependencies, ...
-- ... is configurable: you can choose how you want the test output and test result
-  diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
-  attachments). The defaults are optimized for a [Jenkins](http://jenkins-ci.org) based
-  flow.
-
-
-> Nice work with pycotap! I took a "kitchen sink" approach with tappy so I'm
-> glad someone made a no dependency TAP unittest runner. :)
->   -- [Matt Layman](http://www.mattlayman.com), author of [tappy](http://tappy.readthedocs.org/en/latest/)
-
+  - ... prints TAP (and *only* TAP) to standard output instead of to a
+    separate file, allowing you to pipe it directly to TAP pretty
+    printers and processors (such as the ones listed on the [`tape`
+    page](https://www.npmjs.com/package/tape#pretty-reporters)). By
+    piping it to other consumers, you can avoid the need to add specific
+    test runners to your test code. Since the TAP results are printed as
+    they come in, the consumers can directly display results while the
+    tests are run.
+  - ... only contains a TAP reporter, so no parsers, no frameworks, no
+    dependencies, ...
+  - ... is configurable: you can choose how you want the test output and
+    test result diagnostics to end up in your TAP output (as TAP
+    diagnostics, YAML blocks, or attachments). The defaults are
+    optimized for a [Jenkins](http://jenkins-ci.org) based flow.
+
+> Nice work with pycotap\! I took a "kitchen sink" approach with tappy
+> so I'm glad someone made a no dependency TAP unittest runner. :) --
+> [Matt Layman](http://www.mattlayman.com), author of
+> [tappy](http://tappy.readthedocs.org/en/latest/)
 
 ## Installation
 
-You can install the package directly from [PIP](https://pypi.python.org):
+You can install the package directly from
+[PIP](https://pypi.python.org):
 
     pip install pycotap
 
 Alternatively, you can build and install the package yourself:
 
     python setup.py install
 
-Since the module just consists of one file, you can also just drop the file into
-your project somewhere.
-
+Since the module just consists of one file, you can also just drop the
+file into your project somewhere.
 
 ## Usage
 
 Create a test suite, and run it with `-mpycotap` flag.
 
 For example, given the following test suite in `test_example.py`:
 
-```python
+``` python
 import unittest
 
 class MyTests(unittest.TestCase):
   def test_that_it_passes(self):
     self.assertEqual(0, 0)
 
   @unittest.skip("not finished yet")
@@ -66,44 +71,43 @@
     $ python -mpycotap test_example
     not ok 1 __main__.MyTests.test_that_it_fails
     ok 2 __main__.MyTests.test_that_it_passes
     ok 3 __main__.MyTests.test_that_it_skips # Skipped: not finished yet
     1..3
 
 Alternatively, you can pipe the test to any TAP pretty printer, such as
-[faucet](https://github.com/substack/faucet) or 
+[faucet](https://github.com/substack/faucet) or
 [tap-dot](https://github.com/scottcorgan/tap-dot):
 
     $ python -mpycotap test_example  | faucet
     ⨯ __main__.MyTests.test_that_it_fails
     ✓ __main__.MyTests.test_that_it_passes
     ✓ __main__.MyTests.test_that_it_skips # Skipped: not finished yet
     ⨯ fail  1
-
-
+    
+    
     $ python -mpycotap test_example  | tap-dot 
     x  ..  
-
+    
       3 tests
       2 passed
       1 failed  
-
+    
       Failed Tests:   There was 1 failure
         x __main__.MyTests.test_that_it_fails
 
-
 ### Bring your own `__main__`
 
-You can create a `TAPTestRunner` yourself (e.g. to pass custom parameters),
-and use it to drive your own main function.
+You can create a `TAPTestRunner` yourself (e.g. to pass custom
+parameters), and use it to drive your own main function.
 
-For example, the following can be added to the test example suite above to create
-a runnable Python script:
+For example, the following can be added to the test example suite above
+to create a runnable Python script:
 
-```python
+``` python
 if __name__ == '__main__':
   from pycotap import TAPTestRunner
   suite = unittest.TestLoader().loadTestsFromTestCase(MyTests)
   TAPTestRunner().run(suite)
 ```
 
 This script can now be run:
@@ -114,48 +118,53 @@
     ok 3 __main__.MyTests.test_that_it_skips # Skipped: not finished yet
     1..3
 
 ## API
 
 ### `TAPTestRunner([message_log], [test_output_log])`
 
-- `message_log` (Optional; Default: `LogMode.LogToYAML`):  
-  What to do with test messages (e.g. assertion failure details). 
-  See `LogMode` for possible values.
-- `test_output_log` (Optional; Default: `LogMode.LogToDiagnostics`):  
-  What to do with output printed by the tests.
-  See `LogMode` for possible values.
-
+  - `message_log` (Optional; Default: `LogMode.LogToYAML`):  
+    What to do with test messages (e.g. assertion failure details). See
+    `LogMode` for possible values.
+  - `test_output_log` (Optional; Default: `LogMode.LogToDiagnostics`):  
+    What to do with output printed by the tests. See `LogMode` for
+    possible values.
 
 ### `LogMode`
 
-Enumeration of different destinations to log information. Possible values:
-
-- `LogMode.LogToError`: Log all output to standard error. This means no output 
-  information will end up in the TAP stream, and so will not be processed by any 
-  processors.
-- `LogMode.LogToDiagnostics`: Put output in a diagnostics message 
-  after the test result. This means all output will end up in the TAP stream. How 
-  this is displayed depends on the processor.
-- `LogMode.LogToYAML`: Put output in a YAML block.
-- `LogMode.LogToAttachment`: Put output in a downloadable attachment in a YAML block. 
-  This is an extension supported by e.g. [`tap4j`](http://tap4j.org).
+Enumeration of different destinations to log information. Possible
+values:
 
+  - `LogMode.LogToError`: Log all output to standard error. This means
+    no output information will end up in the TAP stream, and so will not
+    be processed by any processors.
+  - `LogMode.LogToDiagnostics`: Put output in a diagnostics message
+    after the test result. This means all output will end up in the TAP
+    stream. How this is displayed depends on the processor.
+  - `LogMode.LogToYAML`: Put output in a YAML block.
+  - `LogMode.LogToAttachment`: Put output in a downloadable attachment
+    in a YAML block. This is an extension supported by e.g.
+    [`tap4j`](http://tap4j.org).
 
 ## Changelog
 
+### 1.3.0 (2023-04-28)
+
+  - Fix problem with garbage output (thanks
+    [wjt](https://github.com/wjt))
+
 ### 1.1.0 (2015-07-29)
 
-- Don't print message for expected failures
-- Fix problem with unexpected success
+  - Don't print message for expected failures
+  - Fix problem with unexpected success
 
 ### 1.0.1 (2015-07-28)
 
-- Fix problem with tests that cache `sys.std*` output streams
+  - Fix problem with tests that cache `sys.std*` output streams
 
 ### 1.0.0 (2015-01-24)
 
-- Initial stable version
+  - Initial stable version
 
 ### 0.1.0 (2015-01-21)
 
-- Initial version
+  - Initial version
```

### Comparing `pycotap-1.2.2/pycotap/__init__.py` & `pycotap-1.3.0/pycotap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 # Copyright (c) 2015 Remko Tronçon (https://el-tramo.be)
 # Released under the MIT license
 # See COPYING for details
 
-
-import unittest
-import sys
 import base64
+import sys
+import unittest
+
 if sys.hexversion >= 0x03000000:
   from io import StringIO
 else:
   from StringIO import StringIO
 
+
 # Log modes
-class LogMode(object) :
+class LogMode(object):
   LogToError, LogToDiagnostics, LogToYAML, LogToAttachment = range(4)
 
 
 class TAPTestResult(unittest.TestResult):
   def __init__(self, output_stream, error_stream, message_log, test_output_log):
     super(TAPTestResult, self).__init__(self, output_stream)
     self.output_stream = output_stream
@@ -53,15 +54,14 @@
       self.test_output = self.message
     sys.stdout = sys.stderr = self.test_output
 
   def _reset_streams(self):
     sys.stdout = self.orig_stdout
     sys.stderr = self.orig_stderr
 
-
   def print_raw(self, text):
     self.output_stream.write(text)
     self.output_stream.flush()
 
   def print_result(self, result, test, directive = None):
     self.output_stream.write("%s %d %s" % (result, self.testsRun, test.id()))
     if directive:
@@ -80,35 +80,37 @@
 
   def stopTest(self, test):
     super(TAPTestResult, self).stopTest(test)
     if self.message_log == self.test_output_log:
       logs = [(self.message_log, self.message, "output")]
     else:
       logs = [
-          (self.test_output_log, self.test_output, "test_output"),
-          (self.message_log, self.message, "message")
+        (self.test_output_log, self.test_output, "test_output"),
+        (self.message_log, self.message, "message")
       ]
     for log_mode, log, log_name in logs:
       if log_mode != LogMode.LogToError:
         output = log.getvalue()
         if len(output):
           if log_mode == LogMode.LogToYAML:
             self.print_raw("  ---\n")
             self.print_raw("    " + log_name + ": |\n")
             self.print_raw("      " + output.rstrip().replace("\n", "\n      ") + "\n")
             self.print_raw("  ...\n")
           elif log_mode == LogMode.LogToAttachment:
+            content = base64.b64encode(output.encode("utf-8")).decode("utf-8")
             self.print_raw("  ---\n")
             self.print_raw("    " + log_name + ":\n")
             self.print_raw("      File-Name: " + log_name + ".txt\n")
             self.print_raw("      File-Type: text/plain\n")
-            self.print_raw("      File-Content: " + base64.b64encode(output) + "\n")
+            self.print_raw("      File-Content: " + content + "\n")
             self.print_raw("  ...\n")
           else:
             self.print_raw("# " + output.rstrip().replace("\n", "\n# ") + "\n")
+        log.seek(0)
         log.truncate(0)
 
   def addSuccess(self, test):
     super(TAPTestResult, self).addSuccess(test)
     self.ok(test)
 
   def addError(self, test, err):
@@ -132,26 +134,27 @@
   def addUnexpectedSuccess(self, test):
     super(TAPTestResult, self).addUnexpectedSuccess(test)
     self.message.write("Unexpected success" + "\n")
     self.not_ok(test)
 
 
 class TAPTestRunner(object):
-  def __init__(self, 
-      message_log = LogMode.LogToYAML,
-      test_output_log = LogMode.LogToDiagnostics, 
-      output_stream = sys.stdout, error_stream = sys.stderr):
+  def __init__(
+    self,
+    message_log = LogMode.LogToYAML,
+    test_output_log = LogMode.LogToDiagnostics,
+    output_stream = sys.stdout,
+    error_stream = sys.stderr
+  ):
     self.output_stream = output_stream
     self.error_stream = error_stream
     self.message_log = message_log
     self.test_output_log = test_output_log
 
   def run(self, test):
     result = TAPTestResult(
-        self.output_stream, 
-        self.error_stream, 
-        self.message_log, 
-        self.test_output_log)
+      self.output_stream, self.error_stream, self.message_log, self.test_output_log
+    )
     test(result)
     result.printErrors()
 
     return result
```

### Comparing `pycotap-1.2.2/pycotap.egg-info/PKG-INFO` & `pycotap-1.3.0/pycotap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pycotap
-Version: 1.2.2
+Version: 1.3.0
 Summary: A tiny test runner that outputs TAP results to standard output.
 Home-page: https://el-tramo.be/pycotap
 Author: Remko Tronçon
 Author-email: dev@el-tramo.be
 License: MIT
-Description: 
-        `pycotap` is a simple Python test runner for ``unittest`` that outputs 
-        `Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
-        
-        Contrary to other TAP runners for Python, ``pycotap`` ...
-        
-        - ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
-          allowing you to pipe it directly to TAP pretty printers and processors 
-          (such as the ones listed on
-          `the tape page <https://www.npmjs.com/package/tape#pretty-reporters>`_). By
-          piping it to other consumers, you can avoid the need to add 
-          specific test runners to your test code. Since the TAP results
-          are printed as they come in, the consumers can directly display results while 
-          the tests are run.
-        
-        - ... only contains a TAP reporter, so no parsers, no frameworks, no dependencies, ...
-        
-        - ... is configurable: you can choose how you want the test output and test result
-          diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
-          attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
-          flow.
-        
-        Documentation and examples can be found on `the pycotap page 
-        <https://el-tramo.be/pycotap>`_.
-        
 Keywords: tap unittest testing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
+License-File: COPYING
+
+
+`pycotap` is a simple Python test runner for ``unittest`` that outputs 
+`Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
+
+Contrary to other TAP runners for Python, ``pycotap`` ...
+
+- ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
+  allowing you to pipe it directly to TAP pretty printers and processors 
+  (such as the ones listed on
+  `the tape page <https://www.npmjs.com/package/tape#pretty-reporters>`_). By
+  piping it to other consumers, you can avoid the need to add 
+  specific test runners to your test code. Since the TAP results
+  are printed as they come in, the consumers can directly display results while 
+  the tests are run.
+
+- ... only contains a TAP reporter, so no parsers, no frameworks, no dependencies, ...
+
+- ... is configurable: you can choose how you want the test output and test result
+  diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
+  attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
+  flow.
+
+Documentation and examples can be found on `the pycotap page 
+<https://el-tramo.be/pycotap>`_.
```

### Comparing `pycotap-1.2.2/setup.py` & `pycotap-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # coding=utf-8
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 setup(
-  name = "pycotap",
-  version = "1.2.2",
-  packages = find_packages(),
-
-  # Metadata
-  author = "Remko Tronçon",
-  author_email = "dev@el-tramo.be",
-  description = """A tiny test runner that outputs TAP results to standard output.""",
-  long_description = """
+    name="pycotap",
+    version="1.3.0",
+    packages=find_packages(),
+
+    # Metadata
+    author="Remko Tronçon",
+    author_email="dev@el-tramo.be",
+    description=
+    """A tiny test runner that outputs TAP results to standard output.""",
+    long_description="""
 `pycotap` is a simple Python test runner for ``unittest`` that outputs 
 `Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
 
 Contrary to other TAP runners for Python, ``pycotap`` ...
 
 - ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
   allowing you to pipe it directly to TAP pretty printers and processors 
@@ -33,20 +34,18 @@
   diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
   attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
   flow.
 
 Documentation and examples can be found on `the pycotap page 
 <https://el-tramo.be/pycotap>`_.
 """,
-  license = "MIT",
-  keywords = "tap unittest testing",
-  url = "https://el-tramo.be/pycotap",
-  classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Topic :: Utilities",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Software Development :: Testing"
-  ],
-  data_files = [("", ["COPYING"])]
-)
+    license="MIT",
+    keywords="tap unittest testing",
+    url="https://el-tramo.be/pycotap",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers", "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Testing"
+    ],
+    data_files=[("", ["COPYING"])])
```

### Comparing `pycotap-1.2.2/test/test.py` & `pycotap-1.3.0/test/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,267 +1,335 @@
 #!/usr/bin/env python
 
-# pylint: disable=C0325
+# pylint: disable=C0325,E402,E501
+
+import os
+import re
+import sys
+import unittest
 
-import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
 
-import unittest
-import re
 if sys.hexversion >= 0x03000000:
   from io import StringIO
 else:
   from StringIO import StringIO
 
-from pycotap import TAPTestRunner, LogMode
+from pycotap import LogMode, TAPTestRunner
 
 cached_stream = None
 
+
 class TAPTestRunnerTest(unittest.TestCase):
   class OutputTest(unittest.TestCase):
     def test_failing(self):
       print("Foo")
       self.assertEqual(1, 2)
       print("Bar")
+
     def test_passing(self):
       print("Foo")
       sys.stderr.write("Baz\n")
       print("Bar")
 
   class CachingTest(unittest.TestCase):
     def test_passing_1(self):
       global cached_stream
       cached_stream = cached_stream or sys.stdout
       cached_stream.write("Baz1\n")
+
     def test_passing_2(TAPTestRunnerTest):
       global cached_stream
       cached_stream = cached_stream or sys.stdout
       cached_stream.write("Baz2\n")
 
   def setUp(self):
     self.output_stream = StringIO()
     self.error_stream = StringIO()
 
   def run_test(self, test_class, **kwargs):
     suite = unittest.TestLoader().loadTestsFromTestCase(test_class)
-    return TAPTestRunner(output_stream = self.output_stream, error_stream = self.error_stream, **kwargs).run(suite)
+    return TAPTestRunner(
+      output_stream = self.output_stream, error_stream = self.error_stream, **kwargs
+    ).run(suite)
 
   def process_output(self, output):
     return re.sub(
-        r"File \".*\"",
-        "File \"test.py\"",
-        re.sub(r"line \d+", "line X", output))
+      r"Rm9vClRy.*", "Rm9vClRy...",
+      re.sub(r"File \".*\"", "File \"test.py\"", re.sub(r"line \d+", "line X", output))
+    )
 
   def test_all_test_outcomes(self):
     class Test(unittest.TestCase):
       def test_passing(self):
         self.assertEqual(1, 1)
+
       def test_failing(self):
         self.assertEqual(1, 2)
+
       @unittest.skip("Not finished yet")
       def test_skipped(self):
         self.assertEqual(1, 2)
 
-    self.run_test(Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.Test.test_failing\n"
-      "# Traceback (most recent call last):\n"
-      "#   File \"test.py\", line X, in test_failing\n"
-      "#     self.assertEqual(1, 2)\n"
-      "# AssertionError: 1 != 2\n"
-      "ok 2 __main__.Test.test_passing\n"
-      "ok 3 __main__.Test.test_skipped # SKIP Not finished yet\n"
-      "1..3\n"
-    ))
+    self.run_test(
+      Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.test_all_test_outcomes.<locals>.Test.test_failing\n"
+        "# Traceback (most recent call last):\n"
+        "#   File \"test.py\", line X, in test_failing\n"
+        "#     self.assertEqual(1, 2)\n"
+        "# AssertionError: 1 != 2\n"
+        "ok 2 __main__.TAPTestRunnerTest.test_all_test_outcomes.<locals>.Test.test_passing\n"
+        "ok 3 __main__.TAPTestRunnerTest.test_all_test_outcomes.<locals>.Test.test_skipped # SKIP Not finished yet\n"
+        "1..3\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_error(self):
     class Test(unittest.TestCase):
       def test_error(self):
         raise Exception("Some error happened")
 
-    self.run_test(Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.Test.test_error\n"
-      "# Traceback (most recent call last):\n"
-      "#   File \"test.py\", line X, in test_error\n"
-      "#     raise Exception(\"Some error happened\")\n"
-      "# Exception: Some error happened\n"
-      "1..1\n"
-    ))
+    self.run_test(
+      Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.test_error.<locals>.Test.test_error\n"
+        "# Traceback (most recent call last):\n"
+        "#   File \"test.py\", line X, in test_error\n"
+        "#     raise Exception(\"Some error happened\")\n"
+        "# Exception: Some error happened\n"
+        "1..1\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_expected_error(self):
     class Test(unittest.TestCase):
       @unittest.expectedFailure
       def test_expected_error(self):
         self.assertEqual(1, 2)
 
-    self.run_test(Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "ok 1 __main__.Test.test_expected_error\n"
-      "1..1\n"
-    ))
+    self.run_test(
+      Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "ok 1 __main__.TAPTestRunnerTest.test_expected_error.<locals>.Test.test_expected_error\n"
+        "1..1\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_unexpected_success(self):
     class Test(unittest.TestCase):
       @unittest.expectedFailure
       def test_unexpected_success(self):
         self.assertEqual(1, 1)
 
-    self.run_test(Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.Test.test_unexpected_success\n"
-      "# Unexpected success\n"
-      "1..1\n"
-    ))
+    self.run_test(
+      Test, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.test_unexpected_success.<locals>.Test.test_unexpected_success\n"
+        "# Unexpected success\n"
+        "1..1\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_log_output_to_diagnostics(self):
-    self.run_test(TAPTestRunnerTest.OutputTest, message_log = LogMode.LogToDiagnostics, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "# Foo\n"
-      "# Traceback (most recent call last):\n"
-      "#   File \"test.py\", line X, in test_failing\n"
-      "#     self.assertEqual(1, 2)\n"
-      "# AssertionError: 1 != 2\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "# Foo\n"
-      "# Baz\n"
-      "# Bar\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToDiagnostics,
+      test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "# Foo\n"
+        "# Traceback (most recent call last):\n"
+        "#   File \"test.py\", line X, in test_failing\n"
+        "#     self.assertEqual(1, 2)\n"
+        "# AssertionError: 1 != 2\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "# Foo\n"
+        "# Baz\n"
+        "# Bar\n"
+        "1..2\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_log_output_to_yaml(self):
-    self.run_test(TAPTestRunnerTest.OutputTest, message_log = LogMode.LogToYAML, test_output_log = LogMode.LogToYAML)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "  ---\n"
-      "    output: |\n"  
-      "      Foo\n"  
-      "      Traceback (most recent call last):\n"  
-      "        File \"test.py\", line X, in test_failing\n"  
-      "          self.assertEqual(1, 2)\n"  
-      "      AssertionError: 1 != 2\n"  
-      "  ...\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "  ---\n"
-      "    output: |\n"  
-      "      Foo\n"
-      "      Baz\n"
-      "      Bar\n"
-      "  ...\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToYAML,
+      test_output_log = LogMode.LogToYAML
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "  ---\n"
+        "    output: |\n"
+        "      Foo\n"
+        "      Traceback (most recent call last):\n"
+        "        File \"test.py\", line X, in test_failing\n"
+        "          self.assertEqual(1, 2)\n"
+        "      AssertionError: 1 != 2\n"
+        "  ...\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "  ---\n"
+        "    output: |\n"
+        "      Foo\n"
+        "      Baz\n"
+        "      Bar\n"
+        "  ...\n"
+        "1..2\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_log_output_to_attachment(self):
-    self.run_test(TAPTestRunnerTest.OutputTest, message_log = LogMode.LogToAttachment, test_output_log = LogMode.LogToAttachment)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "  ---\n"
-      "    output:\n"  
-      "      File-Name: output.txt\n"
-      "      File-Type: text/plain\n"
-      "      File-Content: Rm9vClRyYWNlYmFjayAobW9zdCByZWNlbnQgY2FsbCBsYXN0KToKICBGaWxlICJ0ZXN0L3Rlc3QucHkiLCBsaW5lIDIzLCBpbiB0ZXN0X2ZhaWxpbmcKICAgIHNlbGYuYXNzZXJ0RXF1YWwoMSwgMikKQXNzZXJ0aW9uRXJyb3I6IDEgIT0gMgoK\n"
-      "  ...\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "  ---\n"
-      "    output:\n"  
-      "      File-Name: output.txt\n"
-      "      File-Type: text/plain\n"
-      "      File-Content: Rm9vCkJhegpCYXIK\n"
-      "  ...\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToAttachment,
+      test_output_log = LogMode.LogToAttachment
+    )
+    self.maxDiff = None
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "  ---\n"
+        "    output:\n"
+        "      File-Name: output.txt\n"
+        "      File-Type: text/plain\n"
+        "      File-Content: Rm9vClRy...\n"
+        "  ...\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "  ---\n"
+        "    output:\n"
+        "      File-Name: output.txt\n"
+        "      File-Type: text/plain\n"
+        "      File-Content: Rm9vCkJhegpCYXIK\n"
+        "  ...\n"
+        "1..2\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_log_output_to_error(self):
-    self.run_test(TAPTestRunnerTest.OutputTest, message_log = LogMode.LogToError, test_output_log = LogMode.LogToError)
-    self.assertEqual(self.output_stream.getvalue(), (
-      "TAP version 13\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "1..2\n"
-    ))
-    self.assertEqual(self.process_output(self.error_stream.getvalue()), (
-      "Foo\n"
-      "Traceback (most recent call last):\n"
-      "  File \"test.py\", line X, in test_failing\n"
-      "    self.assertEqual(1, 2)\n"
-      "AssertionError: 1 != 2\n"
-      "\n"
-      "Foo\n"
-      "Baz\n"
-      "Bar\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToError,
+      test_output_log = LogMode.LogToError
+    )
+    self.assertEqual(
+      self.output_stream.getvalue(), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "1..2\n"
+      )
+    )
+    self.assertEqual(
+      self.process_output(self.error_stream.getvalue()), (
+        "Foo\n"
+        "Traceback (most recent call last):\n"
+        "  File \"test.py\", line X, in test_failing\n"
+        "    self.assertEqual(1, 2)\n"
+        "AssertionError: 1 != 2\n"
+        "\n"
+        "Foo\n"
+        "Baz\n"
+        "Bar\n"
+      )
+    )
 
   def test_log_to_error_order(self):
     self.output_stream = self.error_stream
-    self.run_test(TAPTestRunnerTest.OutputTest, message_log = LogMode.LogToError, test_output_log = LogMode.LogToError)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "Foo\n"
-      "Traceback (most recent call last):\n"
-      "  File \"test.py\", line X, in test_failing\n"
-      "    self.assertEqual(1, 2)\n"
-      "AssertionError: 1 != 2\n"
-      "\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "Foo\n"
-      "Baz\n"
-      "Bar\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToError,
+      test_output_log = LogMode.LogToError
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "Foo\n"
+        "Traceback (most recent call last):\n"
+        "  File \"test.py\", line X, in test_failing\n"
+        "    self.assertEqual(1, 2)\n"
+        "AssertionError: 1 != 2\n"
+        "\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "Foo\n"
+        "Baz\n"
+        "Bar\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "1..2\n"
+      )
+    )
 
   def test_different_error_and_test_output_log(self):
-    self.run_test(TAPTestRunnerTest.OutputTest, 
-        message_log = LogMode.LogToYAML, test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "not ok 1 __main__.OutputTest.test_failing\n"
-      "# Foo\n"
-      "  ---\n"
-      "    message: |\n"  
-      "      Traceback (most recent call last):\n"  
-      "        File \"test.py\", line X, in test_failing\n"  
-      "          self.assertEqual(1, 2)\n"  
-      "      AssertionError: 1 != 2\n"  
-      "  ...\n"
-      "ok 2 __main__.OutputTest.test_passing\n"
-      "# Foo\n"
-      "# Baz\n"
-      "# Bar\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.OutputTest,
+      message_log = LogMode.LogToYAML,
+      test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "not ok 1 __main__.TAPTestRunnerTest.OutputTest.test_failing\n"
+        "# Foo\n"
+        "  ---\n"
+        "    message: |\n"
+        "      Traceback (most recent call last):\n"
+        "        File \"test.py\", line X, in test_failing\n"
+        "          self.assertEqual(1, 2)\n"
+        "      AssertionError: 1 != 2\n"
+        "  ...\n"
+        "ok 2 __main__.TAPTestRunnerTest.OutputTest.test_passing\n"
+        "# Foo\n"
+        "# Baz\n"
+        "# Bar\n"
+        "1..2\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
   def test_stream_caching(self):
-    self.run_test(TAPTestRunnerTest.CachingTest, 
-        message_log = LogMode.LogToDiagnostics, 
-        test_output_log = LogMode.LogToDiagnostics)
-    self.assertEqual(self.process_output(self.output_stream.getvalue()), (
-      "TAP version 13\n"
-      "ok 1 __main__.CachingTest.test_passing_1\n"
-      "# Baz1\n"
-      "ok 2 __main__.CachingTest.test_passing_2\n"
-      "# Baz2\n"
-      "1..2\n"
-    ))
+    self.run_test(
+      TAPTestRunnerTest.CachingTest,
+      message_log = LogMode.LogToDiagnostics,
+      test_output_log = LogMode.LogToDiagnostics
+    )
+    self.assertEqual(
+      self.process_output(self.output_stream.getvalue()), (
+        "TAP version 13\n"
+        "ok 1 __main__.TAPTestRunnerTest.CachingTest.test_passing_1\n"
+        "# Baz1\n"
+        "ok 2 __main__.TAPTestRunnerTest.CachingTest.test_passing_2\n"
+        "# Baz2\n"
+        "1..2\n"
+      )
+    )
     self.assertEqual("", self.error_stream.getvalue())
 
+
 if __name__ == '__main__':
   if os.environ.get("NO_PYCOTAP"):
     unittest.main()
   else:
     TAPTestRunner().run(unittest.TestLoader().loadTestsFromTestCase(TAPTestRunnerTest))
```

