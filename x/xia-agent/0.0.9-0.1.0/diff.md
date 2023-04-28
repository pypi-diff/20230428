# Comparing `tmp/xia_agent-0.0.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent-0.1.0-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 112251 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-13 16:44 xia_agent/__init__.py
--rw-r--r--  2.0 unx   266752 b- defN 23-Feb-13 17:02 xia_agent/agent.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      155 b- defN 23-Feb-13 17:02 xia_agent-0.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      660 b- defN 23-Feb-13 17:02 xia_agent-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Feb-13 17:02 xia_agent-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-13 17:02 xia_agent-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      568 b- defN 23-Feb-13 17:02 xia_agent-0.0.9.dist-info/RECORD
-7 files, 268360 bytes uncompressed, 111241 bytes compressed:  58.5%
+Zip file size: 110465 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      146 b- defN 23-Apr-28 19:22 xia_agent/__init__.py
+-rw-r--r--  2.0 unx   303056 b- defN 23-Apr-28 19:22 xia_agent/agent.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-28 19:22 xia_agent-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      649 b- defN 23-Apr-28 19:22 xia_agent-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-28 19:22 xia_agent-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 19:22 xia_agent-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      572 b- defN 23-Apr-28 19:22 xia_agent-0.1.0.dist-info/RECORD
+7 files, 304693 bytes uncompressed, 109449 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent/__init__.py
 Comment: 
 
-Filename: xia_agent/agent.cp39-win_amd64.pyd
+Filename: xia_agent/agent.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_agent-0.0.9.dist-info/LICENSE.txt
+Filename: xia_agent-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent-0.0.9.dist-info/METADATA
+Filename: xia_agent-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent-0.0.9.dist-info/WHEEL
+Filename: xia_agent-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent-0.0.9.dist-info/top_level.txt
+Filename: xia_agent-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent-0.0.9.dist-info/RECORD
+Filename: xia_agent-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent/__init__.py

```diff
@@ -1,7 +1,7 @@
-from xia_agent.agent import Agent, AgentFunction
+from xia_agent.agent import Agent, AgentFunction, MetaFunction
 
 __all__ = [
-    "Agent", "AgentFunction"
+    "Agent", "AgentFunction", "MetaFunction"
 ]
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
```

## Comparing `xia_agent-0.0.9.dist-info/METADATA` & `xia_agent-0.1.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: xia-agent
-Version: 0.0.9
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-agent/0.0.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-agent/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine
 Requires-Dist: xia-models
+Requires-Dist: xia-logger
 
 .. image:: https://img.shields.io/pypi/v/xia-agent.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-agent/
 
 ====================================
 X-I-A
@@ -27,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

