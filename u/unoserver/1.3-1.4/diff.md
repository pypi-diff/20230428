# Comparing `tmp/unoserver-1.3.tar.gz` & `tmp/unoserver-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unoserver-1.3.tar", last modified: Fri Feb  3 16:56:51 2023, max compression
+gzip compressed data, was "unoserver-1.4.tar", last modified: Fri Apr 28 12:16:30 2023, max compression
```

## Comparing `unoserver-1.3.tar` & `unoserver-1.4.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.944350 unoserver-1.3/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1848 2023-02-03 16:56:51.000000 unoserver-1.3/CHANGES.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      201 2023-02-03 16:56:51.000000 unoserver-1.3/CONTRIBUTORS.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1461 2023-02-03 16:56:51.000000 unoserver-1.3/DEVELOPMENT.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1064 2023-02-03 16:56:51.000000 unoserver-1.3/LICENSE
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-02-03 16:56:51.000000 unoserver-1.3/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1042 2023-02-03 16:56:51.000000 unoserver-1.3/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9352 2023-02-03 16:56:51.944350 unoserver-1.3/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6487 2023-02-03 16:56:51.000000 unoserver-1.3/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1321 2023-02-03 16:56:51.944350 unoserver-1.3/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-02-03 16:56:51.000000 unoserver-1.3/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.940350 unoserver-1.3/src/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.944350 unoserver-1.3/src/unoserver/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10183 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver/converter.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3386 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver/server.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.944350 unoserver-1.3/src/unoserver.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9352 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      602 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       91 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/entry_points.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/not-zip-safe
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       88 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       10 2023-02-03 16:56:51.000000 unoserver-1.3/src/unoserver.egg-info/top_level.txt
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.944350 unoserver-1.3/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.000000 unoserver-1.3/tests/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      332 2023-02-03 16:56:51.000000 unoserver-1.3/tests/conftest.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-02-03 16:56:51.944350 unoserver-1.3/tests/documents/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    29592 2023-02-03 16:56:51.000000 unoserver-1.3/tests/documents/simple.odt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4878 2023-02-03 16:56:51.000000 unoserver-1.3/tests/documents/simple.xlsx
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1809 2023-02-03 16:56:51.000000 unoserver-1.3/tests/test_converter.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5300 2023-02-03 16:56:51.000000 unoserver-1.3/tests/test_integration.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      731 2023-02-03 16:56:51.000000 unoserver-1.3/tests/test_server.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2225 2023-04-28 12:16:30.000000 unoserver-1.4/CHANGES.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      297 2023-04-28 12:16:30.000000 unoserver-1.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1461 2023-04-28 12:16:30.000000 unoserver-1.4/DEVELOPMENT.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1064 2023-04-28 12:16:30.000000 unoserver-1.4/LICENSE
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-04-28 12:16:30.000000 unoserver-1.4/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      970 2023-04-28 12:16:30.000000 unoserver-1.4/Makefile
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10659 2023-04-28 12:16:30.471495 unoserver-1.4/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7321 2023-04-28 12:16:30.000000 unoserver-1.4/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1359 2023-04-28 12:16:30.475495 unoserver-1.4/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-04-28 12:16:30.000000 unoserver-1.4/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/src/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/src/unoserver/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    11455 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver/comparer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    11440 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver/converter.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3386 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver/server.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/src/unoserver.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    10659 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      666 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      128 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/entry_points.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/not-zip-safe
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       88 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       10 2023-04-28 12:16:30.000000 unoserver-1.4/src/unoserver.egg-info/top_level.txt
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/tests/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.000000 unoserver-1.4/tests/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      332 2023-04-28 12:16:30.000000 unoserver-1.4/tests/conftest.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-04-28 12:16:30.471495 unoserver-1.4/tests/documents/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    15935 2023-04-28 12:16:30.000000 unoserver-1.4/tests/documents/index-with-fields.odt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    29592 2023-04-28 12:16:30.000000 unoserver-1.4/tests/documents/simple.odt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4878 2023-04-28 12:16:30.000000 unoserver-1.4/tests/documents/simple.xlsx
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1809 2023-04-28 12:16:30.000000 unoserver-1.4/tests/test_converter.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6455 2023-04-28 12:16:30.000000 unoserver-1.4/tests/test_integration.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      731 2023-04-28 12:16:30.000000 unoserver-1.4/tests/test_server.py
```

### Comparing `unoserver-1.3/CHANGES.rst` & `unoserver-1.4/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+1.4 (2023-04-28)
+----------------
+
+- Added new feature: comparing documents and export the result to any format.
+
+- You can run the new module as scripts, and also with ``python3 -m unoserver.comparer`` just
+  like the ``python3 -m unoserver.server`` and ``python3 -m unoserver.converter``.
+
+- Porting feature from previous release: refresh of index in the Table of Contents
+
+
 1.3 (2023-02-03)
 ----------------
 
 - Now works on Windows (although it's not officially supported).
 
 - Added --filter argument to unoconverter to allow explicit selection of which
   export filter to use for conversion.
```

### Comparing `unoserver-1.3/DEVELOPMENT.rst` & `unoserver-1.4/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/LICENSE` & `unoserver-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/Makefile` & `unoserver-1.4/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 coverage: devenv
 	$(bin_dir)/coverage run -m unittest
 	$(bin_dir)/coverage html
 	$(bin_dir)/coverage report
 
 test: devenv
-	$(bin_dir)/python -bb -X dev -W ignore::UserWarning:setuptools.dist -m unittest --verbose
+	$(bin_dir)/pytest
 
 release: devenv
 	$(bin_dir)/fullrelease
 
 
 clean:
 	rm -rf ve build htmlcov
```

### Comparing `unoserver-1.3/PKG-INFO` & `unoserver-1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unoserver
-Version: 1.3
+Version: 1.4
 Summary: A server for file conversions with Libre Office
 Home-page: https://github.com/unoconv/unoserver
 Author: Lennart Regebro
 Author-email: regebro@gmail.com
 License: MIT
 Keywords: libreoffice,conversion,documents,uno,unoconv
 Platform: UNKNOWN
@@ -39,17 +39,18 @@
 memory again.
 
 To avoid that, LibreOffice has a listener mode, where it can listen for commands via a port,
 and load and convert documents without exiting and reloading the software. This lowers the
 CPU load when converting many documents with somewhere between 50% and 75%, meaning you can
 convert somewhere between two and four times as many documents in the same time using a listener.
 
-Unoserver contains two commands to help you do this, `unoserver` which starts a listener on the
+Unoserver contains three commands to help you do this, `unoserver` which starts a listener on the
 specified IP interface and port, and `unoconverter` which will connect to a listener and ask it
-to convert a document.
+to convert a document, as well as `unocompare` which will connect to a listener and ask it
+to compare two documents and convert the result document.
 
 
 Installation
 ------------
 
 NB! Windows and Mac support is as of yet untested.
 
@@ -100,17 +101,17 @@
 `C:\\Program Files (x86)\\LibreOffice\\python.exe`. On Mac it can be for
 example `/Applications/LibreOffice.app/Contents/python`.
 
 
 Usage
 -----
 
-Installing unoserver installs two scripts, `unoserver` and `unoconverter`.
-Both can also be run as modules with `python3 -m unoserver.server` and
-`python3 -m unoserver.converter` with the same arguments as the main scripts.
+Installing unoserver installs three scripts, `unoserver`, `unoconverter` and `unocompare`.
+All can also be run as modules with `python3 -m unoserver.server`, `python3 -m unoserver.converter`
+and `python3 -m unoserver.comparer` with the same arguments as the main scripts.
 
 Unoserver
 ~~~~~~~~~
 
 ``unoserver [-h] [--interface INTERFACE] [--port PORT] [--daemon] [--executable EXECUTABLE]``
 
 * `--interface`: The interface used by the server, defaults to "localhost"
@@ -126,14 +127,26 @@
 * `infile`: The path to the file to be converted (use - for stdin)
 * `outfile`: The path to the converted file (use - for stdout)
 * `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
 * `--filter`: The export filter to use when converting. It is selected automatically if not specified.
 * `--interface`: The interface used by the server, defaults to "localhost"
 * `--port`: The port used by the server, defaults to "2002"
 
+Unocompare
+~~~~~~~~~~
+
+``unocompare [-h] [--convert-to CONVERT_TO] [--interface INTERFACE] [--port PORT] infile inorigfile outfile``
+
+* `infile`: The path to the modified file to be compared with the original one (use - for stdin)
+* `inorigfile`: The path to the original file to be compared with the modified one (use - for stdin)
+* `outfile`: The path to the result of the comparison and converted file (use - for stdout)
+* `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
+* `--interface`: The interface used by the server, defaults to "localhost"
+* `--port`: The port used by the server, defaults to "2002"
+
 
 Development and Testing
 -----------------------
 
 1. Clone the repo from `https://github.com/unoconv/unoserver`.
 
 2. Setup a virtualenv::
@@ -191,14 +204,27 @@
 Contributors
 ------------
 
 * Lennart Regebro, regebro@gmail.com
 * Stephan Richter, srichter@shoobx.com
 * Bruno Simão, https://github.com/ankology
 * Åsmund Stavdahl, https://github.com/asmundstavdahl
+* Balázs Varga, https://github.com/bvarga91
+* Alessandro Filippini, https://github.com/AlePini
+
+1.4 (2023-04-28)
+----------------
+
+- Added new feature: comparing documents and export the result to any format.
+
+- You can run the new module as scripts, and also with ``python3 -m unoserver.comparer`` just
+  like the ``python3 -m unoserver.server`` and ``python3 -m unoserver.converter``.
+
+- Porting feature from previous release: refresh of index in the Table of Contents
+
 
 1.3 (2023-02-03)
 ----------------
 
 - Now works on Windows (although it's not officially supported).
 
 - Added --filter argument to unoconverter to allow explicit selection of which
```

### Comparing `unoserver-1.3/README.rst` & `unoserver-1.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 memory again.
 
 To avoid that, LibreOffice has a listener mode, where it can listen for commands via a port,
 and load and convert documents without exiting and reloading the software. This lowers the
 CPU load when converting many documents with somewhere between 50% and 75%, meaning you can
 convert somewhere between two and four times as many documents in the same time using a listener.
 
-Unoserver contains two commands to help you do this, `unoserver` which starts a listener on the
+Unoserver contains three commands to help you do this, `unoserver` which starts a listener on the
 specified IP interface and port, and `unoconverter` which will connect to a listener and ask it
-to convert a document.
+to convert a document, as well as `unocompare` which will connect to a listener and ask it
+to compare two documents and convert the result document.
 
 
 Installation
 ------------
 
 NB! Windows and Mac support is as of yet untested.
 
@@ -77,17 +78,17 @@
 `C:\\Program Files (x86)\\LibreOffice\\python.exe`. On Mac it can be for
 example `/Applications/LibreOffice.app/Contents/python`.
 
 
 Usage
 -----
 
-Installing unoserver installs two scripts, `unoserver` and `unoconverter`.
-Both can also be run as modules with `python3 -m unoserver.server` and
-`python3 -m unoserver.converter` with the same arguments as the main scripts.
+Installing unoserver installs three scripts, `unoserver`, `unoconverter` and `unocompare`.
+All can also be run as modules with `python3 -m unoserver.server`, `python3 -m unoserver.converter`
+and `python3 -m unoserver.comparer` with the same arguments as the main scripts.
 
 Unoserver
 ~~~~~~~~~
 
 ``unoserver [-h] [--interface INTERFACE] [--port PORT] [--daemon] [--executable EXECUTABLE]``
 
 * `--interface`: The interface used by the server, defaults to "localhost"
@@ -103,14 +104,26 @@
 * `infile`: The path to the file to be converted (use - for stdin)
 * `outfile`: The path to the converted file (use - for stdout)
 * `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
 * `--filter`: The export filter to use when converting. It is selected automatically if not specified.
 * `--interface`: The interface used by the server, defaults to "localhost"
 * `--port`: The port used by the server, defaults to "2002"
 
+Unocompare
+~~~~~~~~~~
+
+``unocompare [-h] [--convert-to CONVERT_TO] [--interface INTERFACE] [--port PORT] infile inorigfile outfile``
+
+* `infile`: The path to the modified file to be compared with the original one (use - for stdin)
+* `inorigfile`: The path to the original file to be compared with the modified one (use - for stdin)
+* `outfile`: The path to the result of the comparison and converted file (use - for stdout)
+* `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
+* `--interface`: The interface used by the server, defaults to "localhost"
+* `--port`: The port used by the server, defaults to "2002"
+
 
 Development and Testing
 -----------------------
 
 1. Clone the repo from `https://github.com/unoconv/unoserver`.
 
 2. Setup a virtualenv::
```

### Comparing `unoserver-1.3/setup.cfg` & `unoserver-1.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unoserver
-version = 1.3
+version = 1.4
 description = A server for file conversions with Libre Office
 long_description = file: README.rst, CONTRIBUTORS.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Topic :: Office/Business
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
@@ -30,14 +30,15 @@
 test_suite = tests
 python_requires = >= 3.7
 
 [options.entry_points]
 console_scripts = 
 	unoserver = unoserver.server:main
 	unoconvert = unoserver.converter:main
+	unocompare = unoserver.comparer:main
 
 [options.extras_require]
 devenv = 
 	pytest
 	pytest-cov
 	black
 	flake8
```

### Comparing `unoserver-1.3/src/unoserver/converter.py` & `unoserver-1.4/src/unoserver/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,28 +110,30 @@
             # Filter DocumentService here
             yield prop2dict(export_filters.nextElement())
 
     def get_available_filter_names(self):
         return [filter["Name"] for filter in self.get_available_export_filters()]
 
     def convert(
-        self, inpath=None, indata=None, outpath=None, convert_to=None, filtername=None
+        self, inpath=None, indata=None, outpath=None, convert_to=None, filtername=None, update_index=True
     ):
         """Converts a file from one type to another
 
         inpath: A path (on the local hard disk) to a file to be converted.
 
         indata: A byte string containing the file content to be converted.
 
         outpath: A path (on the local hard disk) to store the result, or None, in which case
                  the content of the converted file will be returned as a byte string.
 
         convert_to: The extension of the desired file type, ie "pdf", "xlsx", etc.
 
         filtername: The name of the export filter to use for conversion. If None, it is auto-detected.
+
+        update_index: Updates the index before conversion
         """
         if inpath is None and indata is None:
             raise RuntimeError("Nothing to convert.")
 
         if inpath is not None and indata is not None:
             raise RuntimeError("You can only pass in inpath or indata, not both.")
 
@@ -163,14 +165,31 @@
             input_props += (PropertyValue(Name="InputStream", Value=input_stream),)
             import_path = "private:stream"
 
         document = self.desktop.loadComponentFromURL(
             import_path, "_default", 0, input_props
         )
 
+        if update_index:
+            # Update document indexes
+            for ii in range(2):
+                # At first, update Table-of-Contents.
+                # ToC grows, so page numbers grow too.
+                # On second turn, update page numbers in ToC.
+                try:
+                    document.refresh()
+                    indexes = document.getDocumentIndexes()
+                except AttributeError:
+                    # The document doesn't implement the XRefreshable and/or
+                    # XDocumentIndexesSupplier interfaces
+                    break
+                else:
+                    for i in range(0, indexes.getCount()):
+                        indexes.getByIndex(i).update()
+
         # Now do the conversion
         try:
             # Figure out document type:
             import_type = get_doc_type(document)
 
             if outpath:
                 export_path = uno.systemPathToFileUrl(os.path.abspath(outpath))
@@ -247,19 +266,30 @@
     )
     parser.add_argument(
         "--filter",
         default=None,
         help="The export filter to use when converting. It is selected automatically if not specified.",
     )
     parser.add_argument(
+        "--update-index",
+        action='store_true',
+        help="Updes the indexes before conversion. Can be time consuming.",
+    )
+    parser.add_argument(
+        "--dont-update-index",
+        action='store_false',
+        dest="update_index",
+        help="Skip updating the indexes.",
+    )
+    parser.set_defaults(update_index=True)
+    parser.add_argument(
         "--interface", default="127.0.0.1", help="The interface used by the server"
     )
     parser.add_argument("--port", default="2002", help="The port used by the server")
     args = parser.parse_args()
-
     converter = UnoConverter(args.interface, args.port)
 
     if args.outfile == "-":
         # Set outfile to None, to get the data returned from the function,
         # instead of written to a file.
         args.outfile = None
 
@@ -267,21 +297,23 @@
         # Get data from stdin
         indata = sys.stdin.buffer.read()
         result = converter.convert(
             indata=indata,
             outpath=args.outfile,
             convert_to=args.convert_to,
             filtername=args.filter,
+            update_index=args.update_index,
         )
     else:
         result = converter.convert(
             inpath=args.infile,
             outpath=args.outfile,
             convert_to=args.convert_to,
             filtername=args.filter,
+            update_index=args.update_index,
         )
 
     if args.outfile is None:
         # Pipe result to stdout
         sys.stdout.buffer.write(result)
```

### Comparing `unoserver-1.3/src/unoserver/server.py` & `unoserver-1.4/src/unoserver/server.py`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/src/unoserver.egg-info/PKG-INFO` & `unoserver-1.4/src/unoserver.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unoserver
-Version: 1.3
+Version: 1.4
 Summary: A server for file conversions with Libre Office
 Home-page: https://github.com/unoconv/unoserver
 Author: Lennart Regebro
 Author-email: regebro@gmail.com
 License: MIT
 Keywords: libreoffice,conversion,documents,uno,unoconv
 Platform: UNKNOWN
@@ -39,17 +39,18 @@
 memory again.
 
 To avoid that, LibreOffice has a listener mode, where it can listen for commands via a port,
 and load and convert documents without exiting and reloading the software. This lowers the
 CPU load when converting many documents with somewhere between 50% and 75%, meaning you can
 convert somewhere between two and four times as many documents in the same time using a listener.
 
-Unoserver contains two commands to help you do this, `unoserver` which starts a listener on the
+Unoserver contains three commands to help you do this, `unoserver` which starts a listener on the
 specified IP interface and port, and `unoconverter` which will connect to a listener and ask it
-to convert a document.
+to convert a document, as well as `unocompare` which will connect to a listener and ask it
+to compare two documents and convert the result document.
 
 
 Installation
 ------------
 
 NB! Windows and Mac support is as of yet untested.
 
@@ -100,17 +101,17 @@
 `C:\\Program Files (x86)\\LibreOffice\\python.exe`. On Mac it can be for
 example `/Applications/LibreOffice.app/Contents/python`.
 
 
 Usage
 -----
 
-Installing unoserver installs two scripts, `unoserver` and `unoconverter`.
-Both can also be run as modules with `python3 -m unoserver.server` and
-`python3 -m unoserver.converter` with the same arguments as the main scripts.
+Installing unoserver installs three scripts, `unoserver`, `unoconverter` and `unocompare`.
+All can also be run as modules with `python3 -m unoserver.server`, `python3 -m unoserver.converter`
+and `python3 -m unoserver.comparer` with the same arguments as the main scripts.
 
 Unoserver
 ~~~~~~~~~
 
 ``unoserver [-h] [--interface INTERFACE] [--port PORT] [--daemon] [--executable EXECUTABLE]``
 
 * `--interface`: The interface used by the server, defaults to "localhost"
@@ -126,14 +127,26 @@
 * `infile`: The path to the file to be converted (use - for stdin)
 * `outfile`: The path to the converted file (use - for stdout)
 * `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
 * `--filter`: The export filter to use when converting. It is selected automatically if not specified.
 * `--interface`: The interface used by the server, defaults to "localhost"
 * `--port`: The port used by the server, defaults to "2002"
 
+Unocompare
+~~~~~~~~~~
+
+``unocompare [-h] [--convert-to CONVERT_TO] [--interface INTERFACE] [--port PORT] infile inorigfile outfile``
+
+* `infile`: The path to the modified file to be compared with the original one (use - for stdin)
+* `inorigfile`: The path to the original file to be compared with the modified one (use - for stdin)
+* `outfile`: The path to the result of the comparison and converted file (use - for stdout)
+* `--convert-to`: The file type/extension of the output file (ex pdf). Required when using stdout
+* `--interface`: The interface used by the server, defaults to "localhost"
+* `--port`: The port used by the server, defaults to "2002"
+
 
 Development and Testing
 -----------------------
 
 1. Clone the repo from `https://github.com/unoconv/unoserver`.
 
 2. Setup a virtualenv::
@@ -191,14 +204,27 @@
 Contributors
 ------------
 
 * Lennart Regebro, regebro@gmail.com
 * Stephan Richter, srichter@shoobx.com
 * Bruno Simão, https://github.com/ankology
 * Åsmund Stavdahl, https://github.com/asmundstavdahl
+* Balázs Varga, https://github.com/bvarga91
+* Alessandro Filippini, https://github.com/AlePini
+
+1.4 (2023-04-28)
+----------------
+
+- Added new feature: comparing documents and export the result to any format.
+
+- You can run the new module as scripts, and also with ``python3 -m unoserver.comparer`` just
+  like the ``python3 -m unoserver.server`` and ``python3 -m unoserver.converter``.
+
+- Porting feature from previous release: refresh of index in the Table of Contents
+
 
 1.3 (2023-02-03)
 ----------------
 
 - Now works on Windows (although it's not officially supported).
 
 - Added --filter argument to unoconverter to allow explicit selection of which
```

### Comparing `unoserver-1.3/src/unoserver.egg-info/SOURCES.txt` & `unoserver-1.4/src/unoserver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 setup.cfg
 setup.py
 src/unoserver/__init__.py
+src/unoserver/comparer.py
 src/unoserver/converter.py
 src/unoserver/server.py
 src/unoserver.egg-info/PKG-INFO
 src/unoserver.egg-info/SOURCES.txt
 src/unoserver.egg-info/dependency_links.txt
 src/unoserver.egg-info/entry_points.txt
 src/unoserver.egg-info/not-zip-safe
 src/unoserver.egg-info/requires.txt
 src/unoserver.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_converter.py
 tests/test_integration.py
 tests/test_server.py
+tests/documents/index-with-fields.odt
 tests/documents/simple.odt
 tests/documents/simple.xlsx
```

### Comparing `unoserver-1.3/tests/documents/simple.odt` & `unoserver-1.4/tests/documents/simple.odt`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/tests/documents/simple.xlsx` & `unoserver-1.4/tests/documents/simple.xlsx`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/tests/test_converter.py` & `unoserver-1.4/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `unoserver-1.3/tests/test_integration.py` & `unoserver-1.4/tests/test_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests that start a real unoserver and does real things"""
 
 import io
 import os
 import pytest
+import re
 import sys
 import tempfile
 import time
 
 from unoserver import converter, server
 
 
@@ -144,7 +145,36 @@
         sys.argv = ["unoconverter", "--filter", "asdasdasd", infile, outfile.name]
         try:
             converter.main()
         except RuntimeError as err:
             assert "Office Open XML Text" in err.args[0]
             assert "writer8" in err.args[0]
             assert "writer_pdf_Export" in err.args[0]
+
+
+def test_update_index(server_fixture):
+    infile = os.path.join(TEST_DOCS, "index-with-fields.odt")
+
+    with tempfile.NamedTemporaryFile(suffix=".rtf") as outfile:
+        # Let Libreoffice write to the file and close it.
+        sys.argv = ["unoconverter", infile, outfile.name]
+        converter.main()
+
+        # We now open it to check it, we can't use the outfile object,
+        # it won't reflect the external changes.
+        with open(outfile.name, "rb") as testfile:
+            # The timestamp in Header 2 should appear exactly twice after update
+            matches = re.findall(b"13:18:27", testfile.read())
+            assert len(matches) == 2
+
+        with tempfile.NamedTemporaryFile(suffix=".rtf") as outfile:
+            # Let Libreoffice write to the file and close it.
+            sys.argv = ["unoconverter", "--dont-update-index", infile, outfile.name]
+            converter.main()
+
+            with open(outfile.name, "rb") as testfile:
+                # The timestamp in Header 2 should appear exactly once
+                matches = re.findall(b"13:18:27", testfile.read())
+                assert len(matches) == 1
+
+
+
```

### Comparing `unoserver-1.3/tests/test_server.py` & `unoserver-1.4/tests/test_server.py`

 * *Files identical despite different names*

