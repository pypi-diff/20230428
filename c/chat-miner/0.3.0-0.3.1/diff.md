# Comparing `tmp/chat-miner-0.3.0.tar.gz` & `tmp/chat-miner-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-miner-0.3.0.tar", last modified: Sat Feb  4 20:59:56 2023, max compression
+gzip compressed data, was "chat-miner-0.3.1.tar", last modified: Fri Apr 28 21:40:44 2023, max compression
```

## Comparing `chat-miner-0.3.0.tar` & `chat-miner-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:59:56.031355 chat-miner-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-04 20:59:41.000000 chat-miner-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-02-04 20:59:56.031355 chat-miner-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-04 20:59:41.000000 chat-miner-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:59:56.031355 chat-miner-0.3.0/chat_miner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-02-04 20:59:56.000000 chat-miner-0.3.0/chat_miner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-04 20:59:56.000000 chat-miner-0.3.0/chat_miner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 20:59:56.000000 chat-miner-0.3.0/chat_miner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-04 20:59:56.000000 chat-miner-0.3.0/chat_miner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-04 20:59:56.000000 chat-miner-0.3.0/chat_miner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:59:56.031355 chat-miner-0.3.0/chatminer/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-04 20:59:41.000000 chat-miner-0.3.0/chatminer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-02-04 20:59:41.000000 chat-miner-0.3.0/chatminer/chatparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-04 20:59:41.000000 chat-miner-0.3.0/chatminer/nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-02-04 20:59:41.000000 chat-miner-0.3.0/chatminer/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-04 20:59:41.000000 chat-miner-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-04 20:59:56.031355 chat-miner-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 20:59:56.031355 chat-miner-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-04 20:59:41.000000 chat-miner-0.3.0/test/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:40:44.966287 chat-miner-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 21:40:33.000000 chat-miner-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-28 21:40:44.966287 chat-miner-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 21:40:33.000000 chat-miner-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:40:44.962287 chat-miner-0.3.1/chat_miner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-28 21:40:44.000000 chat-miner-0.3.1/chat_miner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-28 21:40:44.000000 chat-miner-0.3.1/chat_miner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:40:44.000000 chat-miner-0.3.1/chat_miner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 21:40:44.000000 chat-miner-0.3.1/chat_miner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 21:40:44.000000 chat-miner-0.3.1/chat_miner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:40:44.966287 chat-miner-0.3.1/chatminer/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-28 21:40:33.000000 chat-miner-0.3.1/chatminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-04-28 21:40:33.000000 chat-miner-0.3.1/chatminer/chatparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-28 21:40:33.000000 chat-miner-0.3.1/chatminer/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-28 21:40:33.000000 chat-miner-0.3.1/chatminer/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 21:40:33.000000 chat-miner-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-28 21:40:44.966287 chat-miner-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:40:44.966287 chat-miner-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 21:40:33.000000 chat-miner-0.3.1/test/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-28 21:40:33.000000 chat-miner-0.3.1/test/test_whatsapp.py
```

### Comparing `chat-miner-0.3.0/LICENSE` & `chat-miner-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-miner-0.3.0/PKG-INFO` & `chat-miner-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-miner
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lean parsers and visualizations for chat data
 Author: Jonas Weich
 Author-email: jns.wch@gmail.com
 Maintainer: Jonas Weich
 Maintainer-email: jns.wch@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joweich/chat-miner/issues
```

### Comparing `chat-miner-0.3.0/README.md` & `chat-miner-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `chat-miner-0.3.0/chat_miner.egg-info/PKG-INFO` & `chat-miner-0.3.1/chat_miner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-miner
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lean parsers and visualizations for chat data
 Author: Jonas Weich
 Author-email: jns.wch@gmail.com
 Maintainer: Jonas Weich
 Maintainer-email: jns.wch@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/joweich/chat-miner/issues
```

### Comparing `chat-miner-0.3.0/chatminer/__init__.py` & `chat-miner-0.3.1/chatminer/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   X.Y.ZbN   # Beta release
 #   X.Y.ZrcN  # Release Candidate
 #   X.Y.Z     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `chat-miner-0.3.0/chatminer/chatparsers.py` & `chat-miner-0.3.1/chatminer/chatparsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,19 @@
 
     def _parse_message(self, mess):
         datestr, author_and_body = mess.split(self._datefmt.date_author_sep, 1)
         time = datetimeparser.parse(
             datestr, dayfirst=self._datefmt.is_dayfirst, fuzzy=True
         )
 
-        if ":" in author_and_body:
+        if ": " in author_and_body:
             author, body = [x.strip() for x in author_and_body.split(": ", 1)]
+        elif ":." in author_and_body:
+            author = [x.strip() for x in author_and_body.split(":.", 1)][0]
+            body = "<Disappearing Message>"
         else:
             author = "System"
             body = author_and_body.strip()
         return ParsedMessage(time, author, body)
 
 
 class FacebookMessengerParser(Parser):
```

### Comparing `chat-miner-0.3.0/chatminer/nlp.py` & `chat-miner-0.3.1/chatminer/nlp.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.3.0/chatminer/visualizations.py` & `chat-miner-0.3.1/chatminer/visualizations.py`

 * *Files identical despite different names*

### Comparing `chat-miner-0.3.0/setup.cfg` & `chat-miner-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat-miner-0.3.0/test/test_parsers.py` & `chat-miner-0.3.1/test/test_whatsapp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,40 @@
 import pandas as pd
 from pandas.testing import assert_frame_equal
 
-from chatminer.chatparsers import InstagramJsonParser, WhatsAppParser
+from chatminer.chatparsers import WhatsAppParser
 
 
-def test_whatsapp():
-    def assert_equal_from_file(file):
-        parser = WhatsAppParser(f"test/whatsapp/test_{file}.txt")
-        parser.parse_file()
-        df_res = parser.parsed_messages.get_df()
-        df_test = pd.read_csv(
-            f"test/whatsapp/test_{file}_target.csv",
-            parse_dates=["timestamp"],
-            infer_datetime_format=True,
-        )
-        assert_frame_equal(df_test, df_res)
+def assert_equal_from_file(file):
+    parser = WhatsAppParser(f"test/whatsapp/test_{file}.txt")
+    parser.parse_file()
+    df_res = parser.parsed_messages.get_df()
+    df_test = pd.read_csv(
+        f"test/whatsapp/test_{file}_target.csv",
+        parse_dates=["timestamp"],
+        infer_datetime_format=True,
+    )
+    assert_frame_equal(df_test, df_res, check_dtype=False)
 
-    def test_dateformat1():
-        assert_equal_from_file("dateformat1")
 
-    def test_dateformat2():
-        assert_equal_from_file("dateformat2")
+def test_dateformat1():
+    assert_equal_from_file("dateformat1")
 
-    def test_dateformat3():
-        assert_equal_from_file("dateformat3")
 
-    def test_dateformat4():
-        assert_equal_from_file("dateformat4")
+def test_dateformat2():
+    assert_equal_from_file("dateformat2")
 
-    def test_dateformat5():
-        assert_equal_from_file("dateformat5")
 
-    def test_unicode():
-        assert_equal_from_file("unicode")
+def test_dateformat3():
+    assert_equal_from_file("dateformat3")
 
-    test_dateformat1()
-    test_dateformat2()
-    test_dateformat3()
-    test_dateformat4()
-    test_dateformat5()
-    test_unicode()
 
+def test_dateformat4():
+    assert_equal_from_file("dateformat4")
 
-def test_instagram():
-    parser = InstagramJsonParser("test/instagram/testlog.json")
-    parser.parse_file()
-    df_res = parser.parsed_messages.get_df()
-    df_test = pd.read_csv(
-        "test/instagram/testlog_target.csv",
-        parse_dates=["timestamp"],
-        infer_datetime_format=True,
-    )
-    assert_frame_equal(
-        df_test[["author", "message", "words", "letters"]],
-        df_res[["author", "message", "words", "letters"]],
-    )
+
+def test_dateformat5():
+    assert_equal_from_file("dateformat5")
+
+
+def test_unicode():
+    assert_equal_from_file("unicode")
```

