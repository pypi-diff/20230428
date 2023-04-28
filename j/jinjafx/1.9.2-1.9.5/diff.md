# Comparing `tmp/jinjafx-1.9.2.tar.gz` & `tmp/jinjafx-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjafx-1.9.2.tar", last modified: Tue Feb  8 17:39:58 2022, max compression
+gzip compressed data, was "jinjafx-1.9.5.tar", last modified: Thu Feb 17 14:27:16 2022, max compression
```

## Comparing `jinjafx-1.9.2.tar` & `jinjafx-1.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:39:58.066596 jinjafx-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-02-08 17:39:55.000000 jinjafx-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    29404 2022-02-08 17:39:58.066596 jinjafx-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    29509 2022-02-08 17:39:55.000000 jinjafx-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:39:58.062595 jinjafx-1.9.2/jinjafx/
--rwxr-xr-x   0 runner    (1001) docker     (121)    30176 2022-02-08 17:39:55.000000 jinjafx-1.9.2/jinjafx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-02-08 17:39:55.000000 jinjafx-1.9.2/jinjafx/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:39:58.066596 jinjafx-1.9.2/jinjafx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    29404 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-08 17:39:58.000000 jinjafx-1.9.2/jinjafx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 17:39:58.066596 jinjafx-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-02-08 17:39:55.000000 jinjafx-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 14:27:16.782399 jinjafx-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-02-17 14:27:09.000000 jinjafx-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    30242 2022-02-17 14:27:16.782399 jinjafx-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    30347 2022-02-17 14:27:09.000000 jinjafx-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 14:27:16.782399 jinjafx-1.9.5/jinjafx/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    30176 2022-02-17 14:27:09.000000 jinjafx-1.9.5/jinjafx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-02-17 14:27:09.000000 jinjafx-1.9.5/jinjafx/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 14:27:16.782399 jinjafx-1.9.5/jinjafx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    30242 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-17 14:27:16.000000 jinjafx-1.9.5/jinjafx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 14:27:16.782399 jinjafx-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-02-17 14:27:09.000000 jinjafx-1.9.5/setup.py
```

### Comparing `jinjafx-1.9.2/LICENSE` & `jinjafx-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjafx-1.9.2/PKG-INFO` & `jinjafx-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjafx
-Version: 1.9.2
+Version: 1.9.5
 Summary: JinjaFx - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -502,8 +502,21 @@
 
 This filter will encode a string using Cisco's Type 7 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
 
 - <b><code>junos9encode("string", ["seed"])</code></b>
 
 This filter will encode a string using Juniper's Type 9 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
 
+- <b><code>cisco8hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 8 hashing scheme (SHA256 with PBKDF2). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>cisco9hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 9 hashing scheme (SCrypt). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>junos6hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Juniper's Type 6 hashing scheme (Unix Crypt based SHA512). An optional "salt" (length must be 8 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+
```

### Comparing `jinjafx-1.9.2/README.md` & `jinjafx-1.9.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -487,7 +487,20 @@
 - <b><code>cisco7encode("string", ["seed"])</code></b>
 
 This filter will encode a string using Cisco's Type 7 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
 
 - <b><code>junos9encode("string", ["seed"])</code></b>
 
 This filter will encode a string using Juniper's Type 9 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
+
+- <b><code>cisco8hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 8 hashing scheme (SHA256 with PBKDF2). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>cisco9hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 9 hashing scheme (SCrypt). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>junos6hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Juniper's Type 6 hashing scheme (Unix Crypt based SHA512). An optional "salt" (length must be 8 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
```

#### html2text {}

```diff
@@ -369,8 +369,18 @@
 { authPassword|junos_snmpv3_key(engineID) }} set snmp v3 usm local-engine user
 {{ snmpUser }} privacy-aes128 privacy-key {{ privPassword|junos_snmpv3_key
 (engineID) }} ``` - cisco7encode("string", ["seed"]) This filter will encode a
 string using Cisco's Type 7 encoding scheme. An optional "seed" can be provided
 which makes the encoded string deterministic for idempotent operations. -
 junos9encode("string", ["seed"]) This filter will encode a string using
 Juniper's Type 9 encoding scheme. An optional "seed" can be provided which
-makes the encoded string deterministic for idempotent operations.
+makes the encoded string deterministic for idempotent operations. - cisco8hash
+("string", ["salt"]) This filter will hash a string using Cisco's Type 8
+hashing scheme (SHA256 with PBKDF2). An optional "salt" (length must be 14
+characters) can be provided which makes the hashed string deterministic for
+idempotent operations. - cisco9hash("string", ["salt"]) This filter will hash a
+string using Cisco's Type 9 hashing scheme (SCrypt). An optional "salt" (length
+must be 14 characters) can be provided which makes the hashed string
+deterministic for idempotent operations. - junos6hash("string", ["salt"]) This
+filter will hash a string using Juniper's Type 6 hashing scheme (Unix Crypt
+based SHA512). An optional "salt" (length must be 8 characters) can be provided
+which makes the hashed string deterministic for idempotent operations.
```

### Comparing `jinjafx-1.9.2/jinjafx/__init__.py` & `jinjafx-1.9.5/jinjafx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import sys, os, io, argparse, re, copy, getpass, datetime, traceback
 import jinja2, yaml, pytz
 
-__version__ = '1.9.2'
+__version__ = '1.9.5'
 jinja2_filters = []
 
 def import_filters(errc = 0):
   try:
     from ansible.plugins.filter import core
     jinja2_filters.append(core.FilterModule().filters())
   except Exception:
```

### Comparing `jinjafx-1.9.2/jinjafx/__main__.py` & `jinjafx-1.9.5/jinjafx/__main__.py`

 * *Files identical despite different names*

### Comparing `jinjafx-1.9.2/jinjafx.egg-info/PKG-INFO` & `jinjafx-1.9.5/jinjafx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjafx
-Version: 1.9.2
+Version: 1.9.5
 Summary: JinjaFx - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -502,8 +502,21 @@
 
 This filter will encode a string using Cisco's Type 7 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
 
 - <b><code>junos9encode("string", ["seed"])</code></b>
 
 This filter will encode a string using Juniper's Type 9 encoding scheme. An optional "seed" can be provided which makes the encoded string deterministic for idempotent operations.
 
+- <b><code>cisco8hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 8 hashing scheme (SHA256 with PBKDF2). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>cisco9hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Cisco's Type 9 hashing scheme (SCrypt). An optional "salt" (length must be 14 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+- <b><code>junos6hash("string", ["salt"])</code></b>
+
+This filter will hash a string using Juniper's Type 6 hashing scheme (Unix Crypt based SHA512). An optional "salt" (length must be 8 characters) can be provided which makes the hashed string deterministic for idempotent operations.
+
+
```

### Comparing `jinjafx-1.9.2/setup.py` & `jinjafx-1.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,14 @@
   classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
   ],
   packages=["jinjafx"],
   include_package_data=True,
   package_data={'': ['extensions/*.py']},
-  install_requires=["jinja2", "netaddr", "pytz", "pyyaml"],
+  install_requires=["jinja2", "netaddr", "pytz", "pyyaml", "cryptography"],
   entry_points={
     "console_scripts": [
       "jinjafx=jinjafx:main",
     ]
   }
 )
```

