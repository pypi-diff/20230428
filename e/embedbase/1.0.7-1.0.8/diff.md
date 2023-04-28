# Comparing `tmp/embedbase-1.0.7.tar.gz` & `tmp/embedbase-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.7.tar", max compression
+gzip compressed data, was "embedbase-1.0.8.tar", max compression
```

## Comparing `embedbase-1.0.7.tar` & `embedbase-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-28 19:29:43.399867 embedbase-1.0.7/LICENSE
--rw-r--r--   0        0        0     5952 2023-04-28 19:29:43.399867 embedbase-1.0.7/README.md
--rw-r--r--   0        0        0      121 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/__init__.py
--rw-r--r--   0        0        0     3447 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/api.py
--rw-r--r--   0        0        0    16193 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4823 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     8011 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4479 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-28 19:29:43.463867 embedbase-1.0.7/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-28 19:29:43.467867 embedbase-1.0.7/embedbase/utils.py
--rw-r--r--   0        0        0     3584 2023-04-28 19:29:43.467867 embedbase-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 20:04:40.893352 embedbase-1.0.8/LICENSE
+-rw-r--r--   0        0        0     5952 2023-04-28 20:04:40.893352 embedbase-1.0.8/README.md
+-rw-r--r--   0        0        0      121 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/__init__.py
+-rw-r--r--   0        0        0     3447 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/api.py
+-rw-r--r--   0        0        0    16162 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2463 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/base.py
+-rw-r--r--   0        0        0     1164 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4823 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     8011 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4479 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      661 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     2101 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/utils.py
+-rw-r--r--   0        0        0     3584 2023-04-28 20:04:40.949354 embedbase-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.8/PKG-INFO
```

### Comparing `embedbase-1.0.7/LICENSE` & `embedbase-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/README.md` & `embedbase-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/__main__.py` & `embedbase-1.0.8/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/api.py` & `embedbase-1.0.8/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/app.py` & `embedbase-1.0.8/embedbase/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import asyncio
 import os
-from typing import Awaitable, Callable, Optional, Tuple, Union
+from typing import Awaitable, Callable, Optional, Tuple, Union, Any
 import warnings
 from fastapi import FastAPI, Request
 from fastapi.middleware import Middleware
 from starlette.types import Scope
 from embedbase.database.base import VectorDatabase
 from embedbase.embedding.base import Embedder
 from embedbase.logging_utils import get_logger
-from embedbase.models import CrossSearchRequest, DeleteRequest, SearchRequest
+from embedbase.models import (
+    CrossSearchRequest,
+    DeleteRequest,
+    SearchRequest,
+    AddRequest,
+)
 from embedbase.settings import Settings
 import hashlib
 import time
 import urllib.parse
 import uuid
 
 from fastapi import Request, status
-from fastapi.responses import JSONResponse
+from fastapi.responses import JSONResponse, ORJSONResponse
 from pandas import DataFrame
 
 from embedbase.database.db_utils import batch_select
-from embedbase.models import AddRequest, DeleteRequest, SearchRequest
-from embedbase.settings import Settings
 from embedbase.utils import get_user_id
 
 UPLOAD_BATCH_SIZE = int(os.environ.get("UPLOAD_BATCH_SIZE", "100"))
 
 
+
 class Embedbase:
     def __init__(self, settings: Optional[Settings] = None, **kwargs):
         self._kwargs = kwargs
-        self.fastapi_app = FastAPI()
+        self.fastapi_app = FastAPI(default_response_class=ORJSONResponse)
         self.logger = get_logger(settings)
 
     def use_db(
         self,
         db: VectorDatabase,
     ) -> "Embedbase":
         """
@@ -178,21 +182,20 @@
             )
 
             def update_embedding(row, existing_documents):
                 for doc in existing_documents:
                     if row["hash"] == doc["hash"]:
                         return doc["embedding"]
                 return row["embedding"]
-            
+
             # add existing embeddings to the dataframe
             df["embedding"] = df.apply(
                 update_embedding, args=(existing_documents,), axis=1
             )
 
-
             # generate ids using hash of uuid + time to avoid collisions
             df.id = df.apply(
                 lambda x: hashlib.sha256(
                     (str(uuid.uuid4()) + str(time.time())).encode()
                 ).hexdigest(),
                 axis=1,
             )
```

### Comparing `embedbase-1.0.7/embedbase/database/base.py` & `embedbase-1.0.8/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/database/db_utils.py` & `embedbase-1.0.8/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/database/memory_db.py` & `embedbase-1.0.8/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/database/postgres_db.py` & `embedbase-1.0.8/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/database/supabase_db.py` & `embedbase-1.0.8/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/embedding/base.py` & `embedbase-1.0.8/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/embedding/cohere.py` & `embedbase-1.0.8/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/embedding/openai.py` & `embedbase-1.0.8/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/firebase_auth.py` & `embedbase-1.0.8/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/logging_utils.py` & `embedbase-1.0.8/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/models.py` & `embedbase-1.0.8/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/settings.py` & `embedbase-1.0.8/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/strings.py` & `embedbase-1.0.8/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/embedbase/utils.py` & `embedbase-1.0.8/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.7/pyproject.toml` & `embedbase-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.7"
+version = "1.0.8"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

### Comparing `embedbase-1.0.7/PKG-INFO` & `embedbase-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.7
+Version: 1.0.8
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

