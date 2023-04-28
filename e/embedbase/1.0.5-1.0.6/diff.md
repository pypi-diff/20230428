# Comparing `tmp/embedbase-1.0.5.tar.gz` & `tmp/embedbase-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.5.tar", max compression
+gzip compressed data, was "embedbase-1.0.6.tar", max compression
```

## Comparing `embedbase-1.0.5.tar` & `embedbase-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-23 15:50:48.608243 embedbase-1.0.5/LICENSE
--rw-r--r--   0        0        0     6105 2023-04-23 15:50:48.608243 embedbase-1.0.5/README.md
--rw-r--r--   0        0        0      121 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/__init__.py
--rw-r--r--   0        0        0     3447 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/api.py
--rw-r--r--   0        0        0    16171 2023-04-23 15:50:48.660244 embedbase-1.0.5/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2398 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4701 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     7938 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4084 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-23 15:50:48.664244 embedbase-1.0.5/embedbase/utils.py
--rw-r--r--   0        0        0     3585 2023-04-23 15:50:48.664244 embedbase-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     7586 1970-01-01 00:00:00.000000 embedbase-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 08:45:19.347723 embedbase-1.0.6/LICENSE
+-rw-r--r--   0        0        0     6124 2023-04-28 08:45:19.347723 embedbase-1.0.6/README.md
+-rw-r--r--   0        0        0      121 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/__init__.py
+-rw-r--r--   0        0        0     3447 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/api.py
+-rw-r--r--   0        0        0    16193 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2463 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/base.py
+-rw-r--r--   0        0        0     1164 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4823 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     8011 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4479 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      661 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     2101 2023-04-28 08:45:19.411726 embedbase-1.0.6/embedbase/utils.py
+-rw-r--r--   0        0        0     3585 2023-04-28 08:45:19.411726 embedbase-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 embedbase-1.0.6/PKG-INFO
```

### Comparing `embedbase-1.0.5/LICENSE` & `embedbase-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/README.md` & `embedbase-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 <h3 align="center">Add memory to AI with embeddings</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
     <br />
-    <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>
-  <br />
-  <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
-    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-  </a>
+    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
+      <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
+    </a>
+    <br />
+    <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
+      <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+    </a>
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
```

### Comparing `embedbase-1.0.5/embedbase/__main__.py` & `embedbase-1.0.6/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/api.py` & `embedbase-1.0.6/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/app.py` & `embedbase-1.0.6/embedbase/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             self.logger.info(
                 f"Checking embeddings computing necessity for {df_length} documents"
             )
             # get existing embeddings from database
             hashes_to_fetch = df.hash.tolist()
             existing_documents = await batch_select(
                 self.db,
-                hashes_to_fetch,
+                list(set(hashes_to_fetch)),
                 None,
                 None,
             )
 
             def update_embedding(row, existing_documents):
                 for doc in existing_documents:
                     if row["hash"] == doc["hash"]:
@@ -212,15 +212,15 @@
                     )
                 )
 
             # only insert if this dataset_id - user_id
             # pair does not have this hash
             existing_documents_in_this_pair = await batch_select(
                 self.db,
-                hashes_to_fetch,
+                list(set(hashes_to_fetch)),
                 dataset_id,
                 user_id,
             )
 
             # filter out documents that already exist
             # in this dataset_id - user_id pair
             new_df = df[  # HACK: is it fine to only return client the new documents?
```

### Comparing `embedbase-1.0.5/embedbase/database/base.py` & `embedbase-1.0.6/embedbase/database/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
     @abstractmethod
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
+        distinct: bool = True,
     ) -> List[dict]:
         """
         :param ids: list of ids
         :param hashes: list of hashes
         :param dataset_id: dataset id
         :param user_id: user id
+        :param distinct: distinct
         :return: list of documents
         """
         raise NotImplementedError
 
     @abstractmethod
     async def update(
         self,
```

### Comparing `embedbase-1.0.5/embedbase/database/db_utils.py` & `embedbase-1.0.6/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/database/memory_db.py` & `embedbase-1.0.6/embedbase/database/memory_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,23 @@
                 "metadata": row.metadata,
                 "dataset_id": dataset_id,
                 "user_id": user_id,
                 "hash": row.hash,
             }
         return True
 
-    async def select(self, ids=[], hashes=[], dataset_id=None, user_id=None):
+    async def select(
+        self,
+        ids=[],
+        hashes=[],
+        dataset_id=None,
+        user_id=None,
+        # todo: distinct is not implemented
+        distinct: bool = True,
+    ):
         if ids:
             return [
                 {
                     "id": doc_id,
                     "data": self.storage[doc_id]["data"],
                     "embedding": self.storage[doc_id]["embedding"].tolist(),
                     "metadata": self.storage[doc_id]["metadata"],
```

### Comparing `embedbase-1.0.5/embedbase/database/postgres_db.py` & `embedbase-1.0.6/embedbase/database/postgres_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,16 @@
 
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
+        # todo: distinct is not implemented
+        distinct: bool = True,
     ) -> List[dict]:
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
         from psycopg import sql
 
         query = """
 select id, data, embedding, hash, metadata
@@ -212,15 +214,15 @@
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
     ) -> List[dict]:
         d = {
             "query_embedding": str(vector),
-            "similarity_threshold": 0.1,  # TODO: make this configurable
+            "similarity_threshold": 0,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
             "query_user_id": user_id,
         }
         q = "select * from match_documents(%(query_embedding)s, %(similarity_threshold)s, %(match_count)s, %(query_dataset_ids)s, %(query_user_id)s)"
         results = self.conn.execute(q, d)
         if results.rowcount == 0:
```

### Comparing `embedbase-1.0.5/embedbase/database/supabase_db.py` & `embedbase-1.0.6/embedbase/database/supabase_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,27 +23,37 @@
 
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
+        distinct: bool = True,
     ) -> List[dict]:
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
 
         req = self.supabase.table("documents").select("*")
         if ids:
             req = req.in_("id", ids)
+            if distinct:
+                # hack: supabase does not support distinct
+                req = req.order("id", desc=True)
+                req = req.limit(len(ids))
         if hashes:
             req = req.in_("hash", hashes)
+            if distinct:
+                # hack: supabase does not support distinct
+                req = req.order("hash", desc=True)
+                req = req.limit(len(hashes))
         if dataset_id:
             req = req.eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
+        
         return req.execute().data
 
     async def update(
         self,
         df: DataFrame,
         dataset_id: str,
         user_id: Optional[str] = None,
```

### Comparing `embedbase-1.0.5/embedbase/embedding/base.py` & `embedbase-1.0.6/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/embedding/cohere.py` & `embedbase-1.0.6/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/embedding/openai.py` & `embedbase-1.0.6/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/firebase_auth.py` & `embedbase-1.0.6/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/logging_utils.py` & `embedbase-1.0.6/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/models.py` & `embedbase-1.0.6/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/settings.py` & `embedbase-1.0.6/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/strings.py` & `embedbase-1.0.6/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/embedbase/utils.py` & `embedbase-1.0.6/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.5/pyproject.toml` & `embedbase-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.5"
+version = "1.0.6"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
```

### Comparing `embedbase-1.0.5/PKG-INFO` & `embedbase-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.5
+Version: 1.0.6
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -42,22 +42,22 @@
 
 <h3 align="center">Add memory to AI with embeddings</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase">
     <br />
-    <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
-  </a>
-  <br />
-  <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
-    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-  </a>
+    <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
+      <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
+    </a>
+    <br />
+    <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
+      <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+    </a>
     <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
       ·
       <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
       ·
```

