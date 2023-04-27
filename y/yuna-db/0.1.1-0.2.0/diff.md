# Comparing `tmp/yuna-db-0.1.1.tar.gz` & `tmp/yuna-db-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.1.1.tar", last modified: Sat Apr 22 09:09:37 2023, max compression
+gzip compressed data, was "yuna-db-0.2.0.tar", last modified: Thu Apr 27 18:45:56 2023, max compression
```

## Comparing `yuna-db-0.1.1.tar` & `yuna-db-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.1.1/LICENSE
--rw-r--r--   0        0        0     1623 2023-04-22 08:52:20.397496 yuna-db-0.1.1/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.1/__init__.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.1.1/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     9010 2023-04-22 08:53:31.206956 yuna-db-0.1.1/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-22 05:28:48.552375 yuna-db-0.1.1/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    15469 2023-04-22 08:02:32.127615 yuna-db-0.1.1/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     1776 2023-04-22 05:31:18.871506 yuna-db-0.1.1/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.1.1/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.1.1/version.txt
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 yuna-db-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1579 2023-04-27 18:41:03.641249 yuna-db-0.2.0/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.0/__init__.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.0/src/__init__.py
+-rw-r--r--   0        0        0    14786 2023-04-27 18:42:59.934318 yuna-db-0.2.0/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8857 2023-04-26 20:56:38.448341 yuna-db-0.2.0/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    31075 2023-04-27 01:30:51.912829 yuna-db-0.2.0/src/yuna/plugins.py
+-rwxr-xr-x   0        0        0     3276 2023-04-27 18:42:00.065767 yuna-db-0.2.0/test_yuna.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.2.0/tests/test_simple.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.0/version.txt
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 yuna-db-0.2.0/PKG-INFO
```

### Comparing `yuna-db-0.1.1/LICENSE` & `yuna-db-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.1/README.md` & `yuna-db-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,35 +21,33 @@
 
 
 # Example
 
 ```
 from yuna import Yuna, SERIALIZE_JSON, SERIALIZE_STR
 
-db = Yuna("/tmp/test.ydb", create=True)
-db.new_table("names", serialize=SERIALIZE_JSON)
+with Yuna("/tmp/test.ydb", create=True) as db:
+	db.new_table("names", serialize=SERIALIZE_JSON)
 
-key = "feynman"
-value = dict(first_name="Richard", last_name="Feynman")
-db.tables.names.put(key, value)
-
-temp = db.tables.names.get(key)
-assert temp == value
-
-db.new_table("abbrevs", serialize=SERIALIZE_STR)
-key = "l8r"
-value = "see you later"
-
-db.tables.abbrevs.put(key, value)
-temp = db.tables.abbrevs.get(key)
-assert temp == value
-
-db.close()
+	key = "feynman"
+	value = dict(first_name="Richard", last_name="Feynman")
+	db.tables.names.put(key, value)
+
+	temp = db.tables.names.get(key)
+	assert temp == value
+
+	db.new_table("abbrevs", serialize=SERIALIZE_STR)
+	key = "l8r"
+	value = "see you later"
+
+	db.tables.abbrevs.put(key, value)
+	temp = db.tables.abbrevs.get(key)
+	assert temp == value
 ```
 
 # Planned new features to come:
 
-* Implement a context manager on the Yuna class
 * Support integer keys with a .insert() method providing autoincrement
 * Finish the Zstandard compression support
-* Add iterators to quickly find keys within a specified range
+* Add docstrings to the iterators
 * Add a REPL (Python with the yuna module already loaded and the DB open)
+* Add lots of unit tests
```

### Comparing `yuna-db-0.1.1/src/yuna/lmdb_util.py` & `yuna-db-0.2.0/src/yuna/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `yuna-db-0.1.1/PKG-INFO` & `yuna-db-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.1.1
+Version: 0.2.0
 Summary: Yuna DB: dict-like semantics for LMDB
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lmdb >=1.4.1,<2
 
@@ -31,36 +31,34 @@
 
 
 # Example
 
 ```
 from yuna import Yuna, SERIALIZE_JSON, SERIALIZE_STR
 
-db = Yuna("/tmp/test.ydb", create=True)
-db.new_table("names", serialize=SERIALIZE_JSON)
+with Yuna("/tmp/test.ydb", create=True) as db:
+	db.new_table("names", serialize=SERIALIZE_JSON)
 
-key = "feynman"
-value = dict(first_name="Richard", last_name="Feynman")
-db.tables.names.put(key, value)
-
-temp = db.tables.names.get(key)
-assert temp == value
-
-db.new_table("abbrevs", serialize=SERIALIZE_STR)
-key = "l8r"
-value = "see you later"
-
-db.tables.abbrevs.put(key, value)
-temp = db.tables.abbrevs.get(key)
-assert temp == value
-
-db.close()
+	key = "feynman"
+	value = dict(first_name="Richard", last_name="Feynman")
+	db.tables.names.put(key, value)
+
+	temp = db.tables.names.get(key)
+	assert temp == value
+
+	db.new_table("abbrevs", serialize=SERIALIZE_STR)
+	key = "l8r"
+	value = "see you later"
+
+	db.tables.abbrevs.put(key, value)
+	temp = db.tables.abbrevs.get(key)
+	assert temp == value
 ```
 
 # Planned new features to come:
 
-* Implement a context manager on the Yuna class
 * Support integer keys with a .insert() method providing autoincrement
 * Finish the Zstandard compression support
-* Add iterators to quickly find keys within a specified range
+* Add docstrings to the iterators
 * Add a REPL (Python with the yuna module already loaded and the DB open)
+* Add lots of unit tests
```

