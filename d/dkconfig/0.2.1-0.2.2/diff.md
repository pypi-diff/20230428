# Comparing `tmp/dkconfig-0.2.1.tar.gz` & `tmp/dkconfig-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dkconfig-0.2.1.tar", last modified: Mon Feb 15 10:38:46 2021, max compression
+gzip compressed data, was "dkconfig-0.2.2.tar", last modified: Fri Apr 28 15:12:53 2023, max compression
```

## Comparing `dkconfig-0.2.1.tar` & `dkconfig-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-02-15 10:38:46.000000 dkconfig-0.2.1/
-drwxrwxrwx   0        0        0        0 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig/
--rw-rw-rw-   0        0        0    11765 2021-02-15 10:25:22.000000 dkconfig-0.2.1/dkconfig/dkconfig.py
--rw-rw-rw-   0        0        0       52 2021-02-15 10:33:05.000000 dkconfig-0.2.1/dkconfig/_version.py
--rw-rw-rw-   0        0        0       35 2021-02-15 10:08:12.000000 dkconfig-0.2.1/dkconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/
--rw-rw-rw-   0        0        0        1 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-02-15 10:35:54.000000 dkconfig-0.2.1/dkconfig.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4071 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0      329 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2021-02-15 10:38:46.000000 dkconfig-0.2.1/dkconfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2021-02-15 10:08:12.000000 dkconfig-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4071 2021-02-15 10:38:46.000000 dkconfig-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2386 2021-02-15 10:08:12.000000 dkconfig-0.2.1/README.rst
--rw-rw-rw-   0        0        0       68 2021-02-15 10:38:46.000000 dkconfig-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1772 2021-02-15 10:33:05.000000 dkconfig-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:53.580980 dkconfig-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 15:12:42.000000 dkconfig-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:42.000000 dkconfig-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 15:12:53.580980 dkconfig-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-28 15:12:42.000000 dkconfig-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:53.580980 dkconfig-0.2.2/dkconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 15:12:42.000000 dkconfig-0.2.2/dkconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:12:42.000000 dkconfig-0.2.2/dkconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-04-28 15:12:42.000000 dkconfig-0.2.2/dkconfig/dkconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:53.580980 dkconfig-0.2.2/dkconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 15:12:53.000000 dkconfig-0.2.2/dkconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 15:12:53.580980 dkconfig-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-28 15:12:42.000000 dkconfig-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dkconfig-0.2.1/dkconfig/dkconfig.py` & `dkconfig-0.2.2/dkconfig/dkconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/local/bin/python
-# -*- coding: utf-8 -*-
 """
 Basic usage
 -----------
 Most of the methods of ConfigParser
 (https://docs.python.org/2/library/configparser.html#ConfigParser.RawConfigParser)
 should be usable in a relatively obvious way, however, ``dkconfig`` tries to
 give you some sane defaults to make your life easier, e.g. it will create
@@ -71,51 +70,45 @@
     1
 
     /tst> dkconfig foo.ini get header key
     value
     /tst> echo %ERRORLEVEL%
     0
 """
-from __future__ import print_function
-import inspect
-import sys
+import argparse
+import configparser
 import glob
-import tempfile
+import inspect
 import os
 import re
-import argparse
+import sys
+import tempfile
 from contextlib import contextmanager
+
 from lockfile import LockFile
+
 from ._version import __version__
-try:  # pragma: nocover
-    import ConfigParser as configparser  # pylint:disable=import-error
-except ImportError:  # pragma: nocover
-    import configparser  # pylint:disable=import-error
-try:  # pragma: nocover
-    basestring
-except NameError:
-    basestring = (str, bytes)
-    unicode = str
 
 
 def _is_items(lst):
     """Is ``lst`` an items list?
     """
     try:
-        return [(a, b) for a, b in lst]
-    except ValueError:
+        res = list(lst)
+        return False if any(len(item) != 2 for item in res) else res
+    except (ValueError, TypeError):
         return False
 
 
 def _is_iter(lst):
     """Is ``lst`` an iterator?
     """
     try:
         return list(lst)
-    except:  # pragma: nocover
+    except Exception:
         return False
 
 
 def format_items(items):
     """Print items formatted in two columns.
     """
     keylen = max(len(k) for k, v in items)
@@ -132,15 +125,15 @@
 
 def format_result(val):
     """Pretty print val.
     """
     if not val:
         return print("")
 
-    if isinstance(val, (int, float, str, unicode)):
+    if isinstance(val, (int, float, str)):
         return print(val)
 
     items = _is_items(val)
     if items:
         return format_items(items)
 
     lst = _is_iter(val)
@@ -148,27 +141,27 @@
         return format_list(lst)
 
     # mystery item
     print(val)  # pragma: nocover
     return None
 
 
-class Config(configparser.RawConfigParser):  # pylint:disable=too-many-ancestors
+class Config(configparser.RawConfigParser):
     """CLI Interface to configparser.
     """
     exit = 0
     _meta_commands = ['help']
 
     @property
     def commands(self):
         """Return all methods defined as self as a list.
         """
         def _ismethod(m):
             return inspect.ismethod(getattr(self, m))
-        
+
         res = []
         for n in dir(self):
             if n != 'commands' and not n.startswith('_') and _ismethod(n):
                 res.append(n)
         return res
 
     def help(self, cmdname=None):
@@ -177,19 +170,19 @@
         cmds = self.commands
 
         if cmdname is None or cmdname not in cmds:
             return [' ' * 4 + cmd for cmd in cmds]
 
         firstline = inspect.getsourcelines(getattr(self, cmdname))[0][0]
         docstring = inspect.getdoc(getattr(self, cmdname))
-        return '''
-        %s
+        return f'''
+        {firstline.strip()}
             """
-            %s
-            """''' % (firstline.strip(), docstring)
+            {docstring}
+            """'''
 
     def cat(self):
         """Output the contents to stdout.
         """
         self.write(sys.stdout)
 
     def read(self, fname, *args, **kw):  # pylint:disable=arguments-differ
@@ -248,21 +241,21 @@
             """
             m = re.match(r'\w:(?:/[^/]*)*', v)
             if m:
                 # it's a path
                 return v.replace('/', '\\')
             return v
 
-        return ['set "%s=%s"' % (k.upper(), convert_val(v))
+        return [f'set "{k.upper()}={convert_val(v)}"'
                 for k, v in self.values(*sections)]
 
     def bash(self, *sections):
         """Return values as bash export statements.
         """
-        return ['export %s="%s"' % (k.upper(), v)
+        return [f'export {k.upper()}="{v}"'
                 for k, v in self.values(*sections)]
 
 
 VAR_LOCK = '/var/lock'
 
 
 def make_lock(fname, timeout=0):
@@ -286,15 +279,15 @@
 def parser(fname):
     """Context manager that provides locking semantics.
     """
     cp = Config()
     with make_lock(fname, timeout=7):
         try:
             cp.read(fname)
-        except IOError as e:
+        except OSError as e:
             # file not found: errno == 2 (it will be created below)
             if e.errno != 2:
                 raise
         yield cp
         cp.write(open(fname, 'w'))
 
 
@@ -333,15 +326,15 @@
 
           $ find . -maxdepth 2 -name "*.ini" -print | dkconfig - get site dns
           www.example.com
           www.example2.com
           ...
 
     """
-    string_cmdline = isinstance(cmdline, basestring)
+    string_cmdline = isinstance(cmdline, str)
     params = cmdline.split() if string_cmdline else sys.argv[1:]
     p = argparse.ArgumentParser(
         description="Command line interface to ConfigParser"
     )
     p.add_argument('filename', nargs='?')
     p.add_argument('command')
     p.add_argument('--version', action='version',
@@ -386,15 +379,15 @@
         return None
 
     def call_config(cp):
         """Call config command specified in args.command.
         """
         try:
             cmd = getattr(cp, args.command)
-        except:  # pragma: nocover
+        except Exception:  # pragma: nocover
             print('error:', cp, args)
             raise
         remaining_opts = [param for param in unparsed if param.startswith('-')]
         pos_opts = [param for param in unparsed if not param.startswith('-')]
         for item in [parse_kwarg(opt) for opt in remaining_opts]:
             if item:
                 pos_opts += item
```

### Comparing `dkconfig-0.2.1/README.rst` & `dkconfig-0.2.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 
-.. image:: https://travis-ci.org/datakortet/dkconfig.svg?branch=master
-  :target: https://travis-ci.org/datakortet/dkconfig
+.. image:: https://github.com/datakortet/dkconfig/actions/workflows/ci-cd.yml/badge.svg
+    :target: https://github.com/datakortet/dkconfig/actions/workflows/ci-cd.yml
+    :alt: CI/CD Pipeline
 
 .. image:: https://readthedocs.org/projects/dkconfig/badge/?version=latest
    :target: https://readthedocs.org/projects/dkconfig/?badge=latest
    :alt: Documentation Status
 
-
-.. image:: https://coveralls.io/repos/datakortet/dkconfig/badge.png
-   :target: https://coveralls.io/r/datakortet/dkconfig
-   :alt: Coverage Status
-
+.. image:: https://codecov.io/gh/datakortet/dkconfig/branch/master/graph/badge.svg?token=EEyMx6KE7e
+    :target: https://codecov.io/gh/datakortet/dkconfig
+    :alt: Code Coverage
 
 dkconfig -- command line access to ConfigParser
 ==================================================
 
 
 Installing from PyPI
 --------------------
```

### Comparing `dkconfig-0.2.1/setup.py` & `dkconfig-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,61 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-"""dkconfig - command line access to ConfigParser
-"""
-
-classifiers = """\
-Development Status :: 4 - Beta
-Intended Audience :: Developers
-License :: OSI Approved :: MIT License
-Programming Language :: Python
-Programming Language :: Python :: 2
-Programming Language :: Python :: 2.7
-Programming Language :: Python :: 3
-Programming Language :: Python :: 3.4
-Programming Language :: Python :: 3.5
-Programming Language :: Python :: 3.6
-Topic :: Software Development :: Libraries
-"""
-import sys
-import setuptools
-from distutils.core import setup, Command
-from setuptools.command.test import test as TestCommand
-
-version = '0.2.1'
-
-
-class PyTest(TestCommand):
-    user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
-
-    def initialize_options(self):
-        TestCommand.initialize_options(self)
-        self.pytest_args = []
-
-    def finalize_options(self):
-        TestCommand.finalize_options(self)
-        self.test_args = []
-        self.test_suite = True
-
-    def run_tests(self):
-        # import here, cause outside the eggs aren't loaded
-        import pytest
-        errno = pytest.main(self.pytest_args)
-        sys.exit(errno)
-
-
-setup(
-    name='dkconfig',
-    version=version,
-    license='MIT',
-    url='https://github.com/datakortet/dkconfig',
-    install_requires=[
-        'lockfile>=0.10.2',
-    ],
-    description=__doc__.strip(),
-    classifiers=[line for line in classifiers.split('\n') if line],
-    long_description=open('README.rst').read(),
-    cmdclass={'test': PyTest},
-    packages=['dkconfig'],
-    zip_safe=False,
-    entry_points={
-        'console_scripts': [
-            'dkconfig=dkconfig:main'
-        ]
-    }
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+"""dkconfig - command line access to ConfigParser
+"""
+
+classifiers = """\
+Development Status :: 4 - Beta
+Intended Audience :: Developers
+License :: OSI Approved :: MIT License
+Programming Language :: Python
+Programming Language :: Python :: 3
+Topic :: Software Development :: Libraries
+"""
+import sys
+import setuptools
+from distutils.core import setup, Command
+from setuptools.command.test import test as TestCommand
+
+version = '0.2.2'
+
+
+class PyTest(TestCommand):
+    user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
+
+    def initialize_options(self):
+        TestCommand.initialize_options(self)
+        self.pytest_args = []
+
+    def finalize_options(self):
+        TestCommand.finalize_options(self)
+        self.test_args = []
+        self.test_suite = True
+
+    def run_tests(self):
+        # import here, cause outside the eggs aren't loaded
+        import pytest
+        errno = pytest.main(self.pytest_args)
+        sys.exit(errno)
+
+
+setup(
+    name='dkconfig',
+    version=version,
+    license='MIT',
+    url='https://github.com/datakortet/dkconfig',
+    install_requires=[
+        'lockfile>=0.10.2',
+    ],
+    description=__doc__.strip(),
+    classifiers=[line for line in classifiers.split('\n') if line],
+    long_description=open('README.rst').read(),
+    cmdclass={'test': PyTest},
+    packages=['dkconfig'],
+    zip_safe=False,
+    entry_points={
+        'console_scripts': [
+            'dkconfig=dkconfig:main'
+        ]
+    }
+)
```

