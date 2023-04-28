# Comparing `tmp/zope.mkzeoinstance-5.0.tar.gz` & `tmp/zope.mkzeoinstance-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.mkzeoinstance-5.0.tar", last modified: Thu Feb  9 13:47:56 2023, max compression
+gzip compressed data, was "zope.mkzeoinstance-5.1.tar", last modified: Fri Apr 28 05:57:35 2023, max compression
```

## Comparing `zope.mkzeoinstance-5.0.tar` & `zope.mkzeoinstance-5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.910537 zope.mkzeoinstance-5.0/
--rw-r--r--   0 mac        (513) staff       (20)     1653 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)      196 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     2777 2023-02-09 13:47:56.910763 zope.mkzeoinstance-5.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      153 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      100 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      423 2023-02-09 13:47:56.911513 zope.mkzeoinstance-5.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2389 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.900856 zope.mkzeoinstance-5.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.905589 zope.mkzeoinstance-5.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.909341 zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/
--rw-r--r--   0 mac        (513) staff       (20)     6970 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.910100 zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/tests/
--rw-r--r--   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    18264 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/tests/test_unix.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-09 13:47:56.908934 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     2777 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      607 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       58 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       52 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1387 2023-02-09 13:47:56.000000 zope.mkzeoinstance-5.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793563 zope.mkzeoinstance-5.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1849 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)      196 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2973 2023-04-28 05:57:35.793629 zope.mkzeoinstance-5.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      153 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      100 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      423 2023-04-28 05:57:35.793931 zope.mkzeoinstance-5.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2389 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.790099 zope.mkzeoinstance-5.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.791707 zope.mkzeoinstance-5.1/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793127 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7887 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793403 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24486 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/test_unix.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.792976 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2973 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      607 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1387 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/tox.ini
```

### Comparing `zope.mkzeoinstance-5.0/CHANGES.rst` & `zope.mkzeoinstance-5.1/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+5.1 (2023-04-28)
+----------------
+
+- Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
+  path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
+
+
 5.0 (2023-02-09)
 ----------------
 
 - Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
```

### Comparing `zope.mkzeoinstance-5.0/CONTRIBUTING.md` & `zope.mkzeoinstance-5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.mkzeoinstance-5.0/PKG-INFO` & `zope.mkzeoinstance-5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.mkzeoinstance
-Version: 5.0
+Version: 5.1
 Summary: Make standalone ZEO database server instances
 Home-page: https://github.com/zopefoundation/zope.mkzeoinstance
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: ZEO ZODB instance script
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,21 @@
 
 This package provides a single script, ``mkzeoinstance``, which creates
 a standalone ZEO server instance.
 
 Changelog
 =========
 
+5.1 (2023-04-28)
+----------------
+
+- Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
+  path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
+
+
 5.0 (2023-02-09)
 ----------------
 
 - Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
```

### Comparing `zope.mkzeoinstance-5.0/setup.py` & `zope.mkzeoinstance-5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='zope.mkzeoinstance',
-    version='5.0',
+    version='5.1',
     url='https://github.com/zopefoundation/zope.mkzeoinstance',
     license='ZPL 2.1',
     description='Make standalone ZEO database server instances',
     author='Zope Foundation and Contributors',
     author_email='zope-dev@zope.dev',
     long_description=(open('README.rst').read() + "\n" +
                       open('CHANGES.rst').read()),
```

### Comparing `zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/__init__.py` & `zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,46 +8,50 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """%(program)s -- create a ZEO instance.
-
-Usage: %(program)s home [[host:]port]
+Usage: %(program)s home [[host:]port] [options]
 
 Given an "instance home directory" <home> and some configuration
 options (all of which have default values), create the following:
 
 <home>/etc/zeo.conf     -- ZEO config file
 <home>/var/             -- Directory for data files: Data.fs etc.
 <home>/log/             -- Directory for log files: zeo.log and zeoctl.log
 <home>/bin/runzeo       -- the zeo server runner
 <home>/bin/zeoctl       -- start/stop script (a shim for zeoctl.py)
 
+Options:
+    -h, --help         -- Display this help and exit
+    -b, --blobs        -- Directory for Blobs. By default, it will create
+                          a blobs directory at <home>/var/blobs unless a
+                          path is provided -b path/to/blobs
+
 The script will not overwrite existing files; instead, it will issue a
 warning if an existing file is found that differs from the file that
 would be written if it didn't exist.
 """
 
 # WARNING!  Several templates and functions here are reused by ZRS.
 # So be careful with changes.
 
-import getopt
+import argparse
 import os
 import stat
 import sys
 
 import zdaemon
 import ZODB
 
 
 PROGRAM = os.path.basename(sys.argv[0])
 
-
 ZEO_CONF_TEMPLATE = """\
 # ZEO configuration file
 
 %%define INSTANCE %(instance_home)s
 
 <zeo>
   address %(address)s
@@ -56,14 +60,15 @@
   # pid-filename $INSTANCE/var/ZEO.pid
   # monitor-address PORT
   # transaction-timeout SECONDS
 </zeo>
 
 <filestorage 1>
   path $INSTANCE/var/Data.fs
+  %(blob_dir)s
 </filestorage>
 
 <eventlog>
   level info
   <logfile>
     path $INSTANCE/log/zeo.log
   </logfile>
@@ -126,14 +131,16 @@
 
 PYTHONPATH="$ZODB3_HOME"
 export PYTHONPATH INSTANCE_HOME
 
 exec "$PYTHON" -m ZEO.runzeo -C "$CONFIG_FILE" ${1+"$@"}
 """
 
+ZEO_DEFAULT_BLOB_DIR = '$INSTANCE/var/blobs'
+
 
 def print_(msg, *args, **kw):
     if args:
         msg = msg % args
     if kw:
         msg = msg % kw
     if not isinstance(msg, str):
@@ -150,70 +157,82 @@
     if msg:
         print_(msg)
     exit(rc)
 
 
 class ZEOInstanceBuilder:
 
-    def get_params(self, zodb_home, zdaemon_home, instance_home, address):
+    def get_params(self, zodb_home, zdaemon_home,
+                   instance_home, address, blob_dir):
         return {
             "package": "zeo",
             "PACKAGE": "ZEO",
             "zodb_home": zodb_home,
             "zdaemon_home": zdaemon_home,
             "instance_home": instance_home,
+            "blob_dir": f"blob-dir {blob_dir}" if blob_dir else "",
             "address": address,
             "python": sys.executable,
         }
 
     def create(self, home, params):
         makedir(home)
         makedir(home, "etc")
         makedir(home, "var")
         makedir(home, "log")
         makedir(home, "bin")
+
+        # Create dir only when default is selected
+        if ZEO_DEFAULT_BLOB_DIR in params.get('blob_dir', ''):
+            makedir(home, "var/blobs")
+
         makefile(ZEO_CONF_TEMPLATE, home, "etc", "zeo.conf", **params)
         makexfile(ZEOCTL_TEMPLATE, home, "bin", "zeoctl", **params)
         makexfile(RUNZEO_TEMPLATE, home, "bin", "runzeo", **params)
 
     def run(self, argv,
             usage=usage,  # testing hook
             ):
-        try:
-            opts, args = getopt.getopt(argv, "h", ["help"])
-        except getopt.error as msg:  # pragma: nocover
-            usage(msg, 1)
-
-        for k, v in opts:  # pragma: nocover
-            if k in ('-h', '--help'):
-                usage(rc=2)
 
-        if len(args) < 1 or len(args) > 2:
+        parser = argparse.ArgumentParser(add_help=False)
+        parser.add_argument('instance_home', nargs='?', default=None)
+        parser.add_argument('addr_string', nargs='?', default='9999')
+        parser.add_argument('-h', '--help', action='store_true')
+        parser.add_argument('-b', '--blobs', required=False, default=None,
+                            const=ZEO_DEFAULT_BLOB_DIR, nargs='?')
+
+        parsed_args, unknown_args = parser.parse_known_args(argv)
+
+        if len(unknown_args) > 0:
+            usage(rc=1)
+
+        if parsed_args.help:
+            usage(rc=2)
+        elif parsed_args.instance_home is None:
             usage(rc=1)
 
-        instance_home = os.path.abspath(args[0])
+        instance_home = os.path.abspath(parsed_args.instance_home)
 
         zodb_home = os.path.split(ZODB.__path__[0])[0]
         zdaemon_home = os.path.split(zdaemon.__path__[0])[0]
 
-        host = None
-        port = 9999
-        if len(args) == 2:
-            addr_string = args[1]
-            if ':' in addr_string:
-                host, port = addr_string.split(':', 1)
-            else:
-                port = addr_string
-            port = int(port)
-        address = port
-        if host:
-            address = host + ':' + str(port)
+        addr_string = parsed_args.addr_string
+
+        if ':' in addr_string:
+            host, port = addr_string.split(':', 1)
+            address = host + ':' + port
+        elif addr_string.isdigit():
+            address = int(addr_string)
+        else:
+            usage(rc=1)
+
+        blob_dir = parsed_args.blobs if parsed_args.blobs else None
 
-        params = self.get_params(zodb_home, zdaemon_home,
-                                 instance_home, address)
+        params = self.get_params(
+            zodb_home, zdaemon_home, instance_home, address, blob_dir)
         self.create(instance_home, params)
 
 
 def makedir(*args):
     path = ""
     for arg in args:
         path = os.path.join(path, arg)
```

### Comparing `zope.mkzeoinstance-5.0/src/zope/mkzeoinstance/tests/test_unix.py` & `zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/test_unix.py`

 * *Files 18% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     def _getTargetClass(self):
         from zope.mkzeoinstance import ZEOInstanceBuilder
         return ZEOInstanceBuilder
 
     def _makeOne(self):
         return self._getTargetClass()()
 
-    def _makeParams(self, instance_home=None):
+    def _makeParams(self, instance_home=None, blob_dir=None):
         import os
         import sys
 
         import zdaemon
         import ZODB
 
         if instance_home is None:
@@ -128,32 +128,37 @@
                 'python': sys.executable,
                 'executable': sys.executable,
                 'package': 'zeo',
                 'zdaemon_home': zdaemon_home,
                 'instance_home': instance_home,
                 'address': '99999',
                 'zodb_home': zodb_home,
+                'blob_dir': f"blob-dir {blob_dir}" if blob_dir else "",
                 }
 
     def test_get_params(self):
         import sys
 
         expected_params = {'PACKAGE': 'ZEO',
                            'python': sys.executable,
                            'package': 'zeo',
                            'zdaemon_home': '',
                            'instance_home': '',
                            'address': '',
-                           'zodb_home': ''}
+                           'zodb_home': '',
+                           'blob_dir': ''
+                           }
 
         builder = self._makeOne()
         params = builder.get_params(zodb_home='',
                                     zdaemon_home='',
                                     instance_home='',
-                                    address='')
+                                    address='',
+                                    blob_dir=''
+                                    )
 
         self.assertEqual(params, expected_params)
 
     def test_create_folders_and_files(self):
         import os
 
         params = self._makeParams()
@@ -166,14 +171,56 @@
             "Created directory %(instance_home)s/log",
             "Created directory %(instance_home)s/bin",
             "Wrote file %(instance_home)s/etc/zeo.conf",
             "Wrote file %(instance_home)s/bin/zeoctl",
             "Changed mode for %(instance_home)s/bin/zeoctl to 755",
             "Wrote file %(instance_home)s/bin/runzeo",
             "Changed mode for %(instance_home)s/bin/runzeo to 755",
+            ""
+        ]) % params
+
+        builder = self._makeOne()
+        with TempStdout() as temp_out_file:
+
+            with TempUmask(0o022):
+                builder.create(instance_home, params)
+
+            self.assertEqual(temp_out_file.getvalue(), expected_out)
+
+        self.assertTrue(os.path.exists(os.path.join(instance_home, 'etc')))
+        self.assertTrue(os.path.exists(os.path.join(instance_home, 'var')))
+        self.assertTrue(os.path.exists(os.path.join(instance_home, 'log')))
+        self.assertTrue(os.path.exists(os.path.join(instance_home, 'bin')))
+        self.assertTrue(
+            os.path.exists(os.path.join(instance_home, 'etc', 'zeo.conf')))
+        self.assertTrue(
+            os.path.exists(os.path.join(instance_home, 'bin', 'zeoctl')))
+        self.assertTrue(
+            os.path.exists(os.path.join(instance_home, 'bin', 'runzeo')))
+
+    def test_create_folders_and_files_w_blobs(self):
+        import os
+
+        from zope.mkzeoinstance import ZEO_DEFAULT_BLOB_DIR
+
+        params = self._makeParams(blob_dir=ZEO_DEFAULT_BLOB_DIR)
+        instance_home = params['instance_home']
+
+        expected_out = "\n".join([
+            "Created directory %(instance_home)s",
+            "Created directory %(instance_home)s/etc",
+            "Created directory %(instance_home)s/var",
+            "Created directory %(instance_home)s/log",
+            "Created directory %(instance_home)s/bin",
+            "Created directory %(instance_home)s/var/blobs",
+            "Wrote file %(instance_home)s/etc/zeo.conf",
+            "Wrote file %(instance_home)s/bin/zeoctl",
+            "Changed mode for %(instance_home)s/bin/zeoctl to 755",
+            "Wrote file %(instance_home)s/bin/runzeo",
+            "Changed mode for %(instance_home)s/bin/runzeo to 755",
             "",
         ]) % params
 
         builder = self._makeOne()
         with TempStdout() as temp_out_file:
 
             with TempUmask(0o022):
@@ -210,14 +257,79 @@
             "  # pid-filename $INSTANCE/var/ZEO.pid",
             "  # monitor-address PORT",
             "  # transaction-timeout SECONDS",
             "</zeo>",
             "",
             "<filestorage 1>",
             "  path $INSTANCE/var/Data.fs",
+            "  %(blob_dir)s",
+            "</filestorage>",
+            "",
+            "<eventlog>",
+            "  level info",
+            "  <logfile>",
+            "    path $INSTANCE/log/zeo.log",
+            "  </logfile>",
+            "</eventlog>",
+            "",
+            "<runner>",
+            "  program $INSTANCE/bin/runzeo",
+            "  socket-name $INSTANCE/var/zeo.zdsock",
+            "  daemon true",
+            "  forever false",
+            "  backoff-limit 10",
+            "  exit-codes 0, 2",
+            "  directory $INSTANCE",
+            "  default-to-interactive true",
+            "  # user zope",
+            "  python %(executable)s",
+            "  zdrun %(zdaemon_home)s/zdaemon/zdrun.py",
+            "",
+            "  # This logfile should match the one in the zeo.conf file.",
+            ("  # It is used by zdctl's logtail command, "
+             "zdrun/zdctl doesn't write it."),
+            "  logfile $INSTANCE/log/zeo.log",
+            "</runner>",
+            '',
+        ]) % params
+
+        builder = self._makeOne()
+        with TempStdout():
+            builder.create(instance_home, params)
+
+        with open(zeo_conf_path) as f:
+            self.assertEqual(f.read(), expected_out)
+
+    def test_zeo_conf_content_w_default_blobs(self):
+        import os
+
+        from zope.mkzeoinstance import ZEO_DEFAULT_BLOB_DIR
+
+        builder = self._makeOne()
+        params = self._makeParams(blob_dir=ZEO_DEFAULT_BLOB_DIR)
+
+        instance_home = params['instance_home']
+        zeo_conf_path = os.path.join(instance_home, 'etc', 'zeo.conf')
+        expected_out = "\n".join([
+            "# ZEO configuration file",
+            "",
+            "%%define INSTANCE %(instance_home)s",
+            "",
+            "<zeo>",
+            "  address 99999",
+            "  read-only false",
+            "  invalidation-queue-size 100",
+            "  # pid-filename $INSTANCE/var/ZEO.pid",
+            "  # monitor-address PORT",
+            "  # transaction-timeout SECONDS",
+            "</zeo>",
+            "",
+            "<filestorage 1>",
+            "  path $INSTANCE/var/Data.fs",
+            "  %(blob_dir)s",
             "</filestorage>",
             "",
             "<eventlog>",
             "  level info",
             "  <logfile>",
             "    path $INSTANCE/log/zeo.log",
             "  </logfile>",
@@ -240,15 +352,75 @@
             ("  # It is used by zdctl's logtail command, "
              "zdrun/zdctl doesn't write it."),
             "  logfile $INSTANCE/log/zeo.log",
             "</runner>",
             '',
         ]) % params
 
+        with TempStdout():
+            builder.create(instance_home, params)
+
+        with open(zeo_conf_path) as f:
+            self.assertEqual(f.read(), expected_out)
+
+    def test_zeo_conf_content_w_specified_blobs(self):
+        import os
+
         builder = self._makeOne()
+        params = self._makeParams(blob_dir="/usr/local/blobs")
+
+        instance_home = params['instance_home']
+        zeo_conf_path = os.path.join(instance_home, 'etc', 'zeo.conf')
+        expected_out = "\n".join([
+            "# ZEO configuration file",
+            "",
+            "%%define INSTANCE %(instance_home)s",
+            "",
+            "<zeo>",
+            "  address 99999",
+            "  read-only false",
+            "  invalidation-queue-size 100",
+            "  # pid-filename $INSTANCE/var/ZEO.pid",
+            "  # monitor-address PORT",
+            "  # transaction-timeout SECONDS",
+            "</zeo>",
+            "",
+            "<filestorage 1>",
+            "  path $INSTANCE/var/Data.fs",
+            "  %(blob_dir)s",
+            "</filestorage>",
+            "",
+            "<eventlog>",
+            "  level info",
+            "  <logfile>",
+            "    path $INSTANCE/log/zeo.log",
+            "  </logfile>",
+            "</eventlog>",
+            "",
+            "<runner>",
+            "  program $INSTANCE/bin/runzeo",
+            "  socket-name $INSTANCE/var/zeo.zdsock",
+            "  daemon true",
+            "  forever false",
+            "  backoff-limit 10",
+            "  exit-codes 0, 2",
+            "  directory $INSTANCE",
+            "  default-to-interactive true",
+            "  # user zope",
+            "  python %(executable)s",
+            "  zdrun %(zdaemon_home)s/zdaemon/zdrun.py",
+            "",
+            "  # This logfile should match the one in the zeo.conf file.",
+            ("  # It is used by zdctl's logtail command, "
+             "zdrun/zdctl doesn't write it."),
+            "  logfile $INSTANCE/log/zeo.log",
+            "</runner>",
+            '',
+        ]) % params
+
         with TempStdout():
             builder.create(instance_home, params)
 
         with open(zeo_conf_path) as f:
             self.assertEqual(f.read(), expected_out)
 
     def test_zeoctl_content(self):
@@ -292,15 +464,15 @@
             self.assertEqual(f.read(), expected_out)
 
     def test_run_w_invalid_opt(self):
         builder = self._makeOne()
         usage = UsageStub()
         self.assertRaises(UsageExit, builder.run, ['--nonesuch'], usage=usage)
         self.assertEqual(usage._called_with,
-                         ('option --nonesuch not recognized', 1))
+                         ('NO MESSAGE', 1))
 
     def test_run_w_help(self):
         builder = self._makeOne()
         usage = UsageStub()
         self.assertRaises(UsageExit, builder.run, ['--help'], usage=usage)
         self.assertEqual(usage._called_with, ('NO MESSAGE', 2))
 
@@ -314,15 +486,15 @@
         builder = self._makeOne()
         usage = UsageStub()
         self.assertRaises(UsageExit, builder.run, ['a', 'b', 'c'], usage=usage)
         self.assertEqual(usage._called_with, ('NO MESSAGE', 1))
 
     def test_run_wo_single_arg_non_absolute(self):
         import os
-
+        self.maxDiff = None
         builder = self._makeOne()
         tempdir = self._makeTempDir()
         where = os.path.join(tempdir, 'foo', '..', 'bar')
         abswhere = os.path.abspath(where)
 
         params = self._makeParams()
         params['instance_home'] = abswhere
@@ -333,22 +505,21 @@
             "Created directory %(instance_home)s/log",
             "Created directory %(instance_home)s/bin",
             "Wrote file %(instance_home)s/etc/zeo.conf",
             "Wrote file %(instance_home)s/bin/zeoctl",
             "Changed mode for %(instance_home)s/bin/zeoctl to 755",
             "Wrote file %(instance_home)s/bin/runzeo",
             "Changed mode for %(instance_home)s/bin/runzeo to 755",
-            "",
+            ""
         ]) % params
 
         with TempStdout() as temp_out_file:
             with TempUmask(0o022):
                 builder.run([where])
-
-            self.assertEqual(temp_out_file.getvalue(), expected_out)
+                self.assertEqual(temp_out_file.getvalue(), expected_out)
 
         self.assertTrue(os.path.exists(os.path.join(abswhere, 'etc')))
         self.assertTrue(os.path.exists(os.path.join(abswhere, 'var')))
         self.assertTrue(os.path.exists(os.path.join(abswhere, 'log')))
         self.assertTrue(os.path.exists(os.path.join(abswhere, 'bin')))
         self.assertTrue(
             os.path.exists(os.path.join(abswhere, 'etc', 'zeo.conf')))
```

### Comparing `zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/PKG-INFO` & `zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.mkzeoinstance
-Version: 5.0
+Version: 5.1
 Summary: Make standalone ZEO database server instances
 Home-page: https://github.com/zopefoundation/zope.mkzeoinstance
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: ZEO ZODB instance script
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,21 @@
 
 This package provides a single script, ``mkzeoinstance``, which creates
 a standalone ZEO server instance.
 
 Changelog
 =========
 
+5.1 (2023-04-28)
+----------------
+
+- Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
+  path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
+
+
 5.0 (2023-02-09)
 ----------------
 
 - Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
 - Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
```

### Comparing `zope.mkzeoinstance-5.0/src/zope.mkzeoinstance.egg-info/SOURCES.txt` & `zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.mkzeoinstance-5.0/tox.ini` & `zope.mkzeoinstance-5.1/tox.ini`

 * *Files identical despite different names*

