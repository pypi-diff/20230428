# Comparing `tmp/pref-0.1.0-py3-none-any.whl.zip` & `tmp/pref-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5449 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      230 b- defN 20-Dec-26 01:18 pref/__init__.py
--rw-rw-rw-  2.0 fat      282 b- defN 22-Jun-08 04:19 pref/__version__.py
--rw-rw-rw-  2.0 fat     4027 b- defN 22-Jun-08 04:15 pref/pref.py
--rw-rw-rw-  2.0 fat        0 b- defN 21-Mar-26 05:01 pref/py.typed
--rw-rw-rw-  2.0 fat     1088 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1088 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1736 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      742 b- defN 22-Jun-08 04:20 pref-0.1.0.dist-info/RECORD
-10 files, 9290 bytes uncompressed, 4195 bytes compressed:  54.8%
+Zip file size: 5551 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      230 b- defN 23-Apr-28 00:23 pref/__init__.py
+-rw-rw-rw-  2.0 fat      282 b- defN 23-Apr-28 05:36 pref/__version__.py
+-rw-rw-rw-  2.0 fat     4367 b- defN 23-Apr-28 05:40 pref/pref.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-28 00:23 pref/py.typed
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1807 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      742 b- defN 23-Apr-28 05:44 pref-0.2.0.dist-info/RECORD
+10 files, 9701 bytes uncompressed, 4297 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pref/pref.py
 Comment: 
 
 Filename: pref/py.typed
 Comment: 
 
-Filename: pref-0.1.0.dist-info/LICENSE
+Filename: pref-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pref-0.1.0.dist-info/LICENSE.txt
+Filename: pref-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pref-0.1.0.dist-info/METADATA
+Filename: pref-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pref-0.1.0.dist-info/WHEEL
+Filename: pref-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pref-0.1.0.dist-info/top_level.txt
+Filename: pref-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pref-0.1.0.dist-info/RECORD
+Filename: pref-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pref/__version__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __application_name__ = "pref"
 __title__ = __application_name__
 __author__ = "abel"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/pref"
 __download_url__ = __url__
 __description__ = "persistent preferences store to local sqlite"
```

## pref/pref.py

```diff
@@ -3,16 +3,20 @@
 import warnings
 
 import appdirs
 from sqlitedict import SqliteDict
 from attr import attrib, attrs
 
 
-def get_sqlite_path(name: str, author: str) -> Path:
-    sqlite_path = Path(appdirs.user_config_dir(name, author), f"{name}.db")
+def get_sqlite_path(name: str, author: str, file_name: str = "") -> Path:
+    assert len(name) > 0
+    assert len(author) > 0
+    if file_name is None or len(file_name) < 1:
+        file_name = f"{name}.db"
+    sqlite_path = Path(appdirs.user_config_dir(name, author), file_name)
     sqlite_path.parent.mkdir(parents=True, exist_ok=True)
     return sqlite_path
 
 
 class _PreferenceMeta:
     """
     Values of type _PreferenceMeta (or derived classes) don't get written to the DB
@@ -36,14 +40,15 @@
     """
     store/retrieve preferences as a set of attrs attributes to/from a sqlite database
     """
 
     application_name = attrib(type=_PreferenceMetaStr, converter=_to_preferences_meta_str)
     application_author = attrib(type=_PreferenceMetaStr, converter=_to_preferences_meta_str)
     table = attrib(default=_PreferenceMetaStr("preferences"), type=_PreferenceMetaStr, converter=_to_preferences_meta_str)
+    file_name = attrib(default=_PreferenceMetaStr(""), type=_PreferenceMetaStr, converter=_to_preferences_meta_str)  # default of "" means use f"{application_name}.db"
     _pref_init = _PreferenceMetaBool(False)  # starts as a class variable, then set to True as a class instance variable once all initialization is complete
 
     def __attrs_post_init__(self):
         # initialize values from the DB for the derived class's attributes
         sqlite_dict = self.get_sqlite_dict()
         for key in self.__dict__:
             value = sqlite_dict.get(key)
@@ -59,15 +64,15 @@
             sql_lite_dict = self.get_sqlite_dict()
             existing_value = sql_lite_dict.get(key)
             if existing_value != value:
                 sql_lite_dict[key] = value  # does the DB write
 
     def get_sqlite_dict(self) -> SqliteDict:
         # override this method if you don't like this "pass through" encoding, or want a different sqlite file path, etc.
-        return SqliteDict(get_sqlite_path(self.application_name, self.application_author), self.table, autocommit=True, encode=lambda x: x, decode=lambda x: x)
+        return SqliteDict(get_sqlite_path(self.application_name, self.application_author, self.file_name), self.table, autocommit=True, encode=lambda x: x, decode=lambda x: x)
 
 
 # legacy
 class PrefDict(Pref):
     def __attrs_post_init__(self):
         warnings.warn("use Pref class instead of PrefDict", DeprecationWarning)
         super().__attrs_post_init__()
```

## Comparing `pref-0.1.0.dist-info/LICENSE` & `pref-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pref-0.1.0.dist-info/LICENSE.txt` & `pref-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pref-0.1.0.dist-info/METADATA` & `pref-0.2.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1
-Name: pref
-Version: 0.1.0
-Summary: persistent preferences store to local sqlite
-Home-page: https://github.com/jamesabel/pref
-Download-URL: https://github.com/jamesabel/pref
-Author: abel
-Author-email: j@abel.co
-License: MIT
-Keywords: local,preferences,sqlite
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-Requires-Dist: sqlitedict
-Requires-Dist: attrs
-Requires-Dist: appdirs
-
-
-# pref - a simple local preferences store
-
-Persistent storage of `attrs` attributes or an ordered set (like a list, but no duplicates) to 
-a local SQLite database file. 
-
-# Example
-
-```
-from attr import attrib, attrs
-from ismain import is_main
-
-from pref import Pref, PrefOrderedSet
-
-application_name = "myapp"
-author = "me"
-
-
-@attrs
-class MyPref(Pref):
-    first_name: str = attrib(default=None)
-    last_name: str = attrib(default=None)
-    has_subscription: bool = attrib(default=False)  # start off with no subscription
-
-
-def get_pref() -> MyPref:
-    return MyPref(application_name, author)
-
-
-def get_ordered_set() -> PrefOrderedSet:
-    return PrefOrderedSet(application_name, author, "mylist")
-
-
-if is_main():
-
-    # set a variable
-    preferences = get_pref()
-    preferences.first_name = "James"
-    preferences.last_name = "Abel"
-
-    # read it back
-    preferences = get_pref()
-    print(preferences.first_name)  # James
-    print(preferences.last_name)  # Abel
-    print(preferences.has_subscription)  # evaluates as False (is actually int of 0)
-
-    # set an ordered set (list-like, but no duplicates)
-    my_list = get_ordered_set()
-    my_list.set(["a", "b", "c"])
-
-    # read the ordered set back in
-    my_list = get_ordered_set()
-    print(my_list.get())  # ['a', 'b', 'c']
-```
+Metadata-Version: 2.1
+Name: pref
+Version: 0.2.0
+Summary: persistent preferences store to local sqlite
+Home-page: https://github.com/jamesabel/pref
+Download-URL: https://github.com/jamesabel/pref
+Author: abel
+Author-email: j@abel.co
+License: MIT
+Keywords: local,preferences,sqlite
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
+Requires-Dist: sqlitedict
+Requires-Dist: attrs
+Requires-Dist: appdirs
+
+
+# pref - a simple local preferences store
+
+Persistent storage of `attrs` attributes or an ordered set (like a list, but no duplicates) to 
+a local SQLite database file. 
+
+# Example
+
+```
+from attr import attrib, attrs
+from ismain import is_main
+
+from pref import Pref, PrefOrderedSet
+
+application_name = "myapp"
+author = "me"
+
+
+@attrs
+class MyPref(Pref):
+    first_name: str = attrib(default=None)
+    last_name: str = attrib(default=None)
+    has_subscription: bool = attrib(default=False)  # start off with no subscription
+
+
+def get_pref() -> MyPref:
+    return MyPref(application_name, author)
+
+
+def get_ordered_set() -> PrefOrderedSet:
+    return PrefOrderedSet(application_name, author, "mylist")
+
+
+if is_main():
+
+    # set a variable
+    preferences = get_pref()
+    preferences.first_name = "James"
+    preferences.last_name = "Abel"
+
+    # read it back
+    preferences = get_pref()
+    print(preferences.first_name)  # James
+    print(preferences.last_name)  # Abel
+    print(preferences.has_subscription)  # evaluates as False (is actually int of 0)
+
+    # set an ordered set (list-like, but no duplicates)
+    my_list = get_ordered_set()
+    my_list.set(["a", "b", "c"])
+
+    # read the ordered set back in
+    my_list = get_ordered_set()
+    print(my_list.get())  # ['a', 'b', 'c']
+```
```

