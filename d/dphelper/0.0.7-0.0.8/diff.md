# Comparing `tmp/dphelper-0.0.7.tar.gz` & `tmp/dphelper-0.0.8.tar.gz`

## Comparing `dphelper-0.0.7.tar` & `dphelper-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.7/steps.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/__init__.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/config.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/helper.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/schemas.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/connection/__init__.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/connection/fetch.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/snapshot/__init__.py
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 dphelper-0.0.7/src/dphelper/snapshot/snapshot.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 dphelper-0.0.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.7/license
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dphelper-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.7/readme.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dphelper-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 dphelper-0.0.8/steps.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/__init__.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/config.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/helper.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/schemas.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/connection/__init__.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/connection/fetch.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/snapshot/__init__.py
+-rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 dphelper-0.0.8/src/dphelper/snapshot/snapshot.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 dphelper-0.0.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dphelper-0.0.8/license
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dphelper-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dphelper-0.0.8/readme.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dphelper-0.0.8/PKG-INFO
```

### Comparing `dphelper-0.0.7/src/dphelper/config.py` & `dphelper-0.0.8/src/dphelper/config.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.7/src/dphelper/helper.py` & `dphelper-0.0.8/src/dphelper/helper.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.7/src/dphelper/connection/fetch.py` & `dphelper-0.0.8/src/dphelper/connection/fetch.py`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.7/src/dphelper/snapshot/snapshot.py` & `dphelper-0.0.8/src/dphelper/snapshot/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,24 @@
             raise ValueError(
                 "Cant get snapshot result without args. Please give file url of snapshot data or snapshot_id"
             )
         if is_loadable == False:
             # why bother downloading if it will be blank / corrupted / etc. ?
             # or should exception be raised?
             return {}
+        is_preview = False
         if result_file_url is None:
+            is_preview = True  # response will have to be unwrapped
             # maybe old snapshot, so ask for preview, expecting to get full snapshot result
             result_file_url = self.__get_snapshot_url(f"{snapshot_id}/preview")
         response = self.fetcher._request_or_repeat(_requests.get, url=result_file_url)
         self.fetcher._response_ok_or_raise(response)
-        return response.json()
+        return (
+            response.json() if not is_preview else response.json()["json_data_preview"]
+        )
 
     def get_result_by_id(self, snapshot_id: int) -> _typing.Any:
         "gets snapshot result by snapshot id. result might be any type but usually it is a list of objects"
         # get meta
         meta = self.get_meta_by_id(snapshot_id)
         # now result
         return self.__get_result_by_url_or_id(
```

### Comparing `dphelper-0.0.7/.gitignore` & `dphelper-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dphelper-0.0.7/PKG-INFO` & `dphelper-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dphelper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Handle common scraping problems, help linking data platform entities
 Author-email: Egidijus Gylys <EgidijusGylys1@gmail.com>
 License-File: license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Requires-Dist: fake-headers
```

