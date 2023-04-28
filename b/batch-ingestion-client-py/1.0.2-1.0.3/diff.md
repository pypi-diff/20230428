# Comparing `tmp/batch_ingestion_client_py-1.0.2.tar.gz` & `tmp/batch_ingestion_client_py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_ingestion_client_py-1.0.2.tar", last modified: Thu Apr 20 14:13:10 2023, max compression
+gzip compressed data, was "batch_ingestion_client_py-1.0.3.tar", last modified: Fri Apr 28 13:47:18 2023, max compression
```

## Comparing `batch_ingestion_client_py-1.0.2.tar` & `batch_ingestion_client_py-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4092 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     3456 2023-04-20 14:12:30.000000 batch_ingestion_client_py-1.0.2/README.md
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.414461 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      265 2023-04-20 14:08:41.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/__init__.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     5750 2023-04-20 13:08:39.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/data.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      642 2023-04-20 14:08:52.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/main.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1422 2023-04-20 13:08:18.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/response.py
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     4092 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      406 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/SOURCES.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        1 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/dependency_links.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        9 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/requires.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       26 2023-04-20 14:13:10.000000 batch_ingestion_client_py-1.0.2/batch_ingestion_client_py.egg-info/top_level.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       38 2023-04-20 14:13:10.418461 batch_ingestion_client_py-1.0.2/setup.cfg
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1102 2023-04-20 14:12:56.000000 batch_ingestion_client_py-1.0.2/setup.py
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1069 2023-04-20 14:24:25.000000 batch_ingestion_client_py-1.0.3/LICENSE
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     2030 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/PKG-INFO
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1372 2023-04-28 13:44:26.000000 batch_ingestion_client_py-1.0.3/README.md
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      254 2023-04-28 12:51:27.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/__init__.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1436 2023-04-28 13:17:43.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/curl.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     5271 2023-04-28 13:40:54.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/data.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1946 2023-04-28 13:28:14.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/lib.py
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1422 2023-04-20 13:08:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/response.py
+drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     2030 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/PKG-INFO
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      399 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        1 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       26 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/top_level.txt
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       38 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/setup.cfg
+-rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1092 2023-04-28 13:23:49.000000 batch_ingestion_client_py-1.0.3/setup.py
```

### Comparing `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/data.py` & `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,34 +126,38 @@
 
 
 class Entity:
     TYPE = Dict[str, str | List[Claim.TYPE] | Dict[str, ValueInLanguage.TYPE]]
 
     def __init__(
         self,
-        id: str,
+        id: str | None = None,
         mode: Literal["add", "remove"] | None = None,
-        type: str = "item",
+        type: Literal["item", "property"] = "item",
         labels: Dict[str, ValueInLanguage] | None = None,
         descriptions: Dict[str, ValueInLanguage] | None = None,
         claims: Dict[str, List[Claim]] | None = None,
     ):
+        if id is None and mode is not None:
+            raise ValueError("id must be set if mode is set")
         self.id = id
         self.mode = mode
         self.type = type
         self.labels = labels
         self.descriptions = descriptions
         self.claims = claims
 
     def serialize(self):
-        e = {
-            "id": self.id,
-            "mode": self.mode,
+        e: dict[str, Any] = {
             "type": self.type,
         }
+        if self.id is not None:
+            e["id"] = self.id
+        if self.mode is not None:
+            e["mode"] = self.mode
         if self.labels is not None:
             e["labels"] = {
                 key: value.serialize()
                 for key, value in self.labels.items()
             }
         if self.descriptions is not None:
             e["descriptions"] = {
@@ -166,16 +170,16 @@
                 for key, value in self.claims.items()
             }
         return e
 
     @staticmethod
     def parse(data: TYPE):
         return Entity(
-            id=data["id"],  # type: ignore
-            mode=data["mode"],  # type: ignore
+            id=data["id"] if "id" in data else None,  # type: ignore
+            mode=data["mode"] if "mode" in data else None,  # type: ignore
             type=data["type"],  # type: ignore
             labels={
                 key: ValueInLanguage.parse(value)
                 for key, value in data["labels"].items()  # type: ignore
             } if "labels" in data else None,
             descriptions={
                 key: ValueInLanguage.parse(value)
@@ -185,41 +189,7 @@
                 key: [Claim.parse(claim) for claim in value]  # type: ignore
                 for key, value in data["claims"].items()  # type: ignore
             } if "claims" in data else None,
         )
 
     def __repr__(self) -> str:
         return self.serialize().__repr__()
-
-
-class Data:
-    TYPE = Dict[str, str | List[Entity.TYPE | Any]]
-
-    def __init__(
-        self,
-        key: str,
-        entities: List[Entity],
-    ):
-        self.key = key
-        self.entities = entities
-
-    def serialize(self):
-        return {
-            "key": self.key,
-            "entities": [
-                entity.serialize()
-                for entity in self.entities
-            ],
-        }
-
-    @staticmethod
-    def parse(data: TYPE):
-        return Data(
-            key=data["key"],  # type: ignore
-            entities=[
-                Entity.parse(entity)  # type: ignore
-                for entity in data["entities"]  # type: ignore
-            ],
-        )
-
-    def __repr__(self) -> str:
-        return self.serialize().__repr__()
```

### Comparing `batch_ingestion_client_py-1.0.2/batch_ingestion_client_py/response.py` & `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/response.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.2/setup.py` & `batch_ingestion_client_py-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DESCRIPTION = "A client for the BatchIngestion mediawiki API"
 
 setup(
     name="batch_ingestion_client_py",
     version=VERSION,
     author="QuentinJanuel",
     author_email="<quentinjanuelkij@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["requests"],
+    install_requires=[],
     keywords=[
         'python',
         'mediawiki',
         'batchingestion',
         'wikidata',
         'wikibase',
         'api',
```

