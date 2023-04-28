# Comparing `tmp/minivnn-0.1.0.tar.gz` & `tmp/minivnn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minivnn-0.1.0.tar", max compression
+gzip compressed data, was "minivnn-0.1.1.tar", max compression
```

## Comparing `minivnn-0.1.0.tar` & `minivnn-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1439 2023-04-19 00:24:53.724298 minivnn-0.1.0/README.md
--rw-r--r--   0        0        0       48 2023-04-19 00:24:53.724298 minivnn-0.1.0/minivnn/__init__.py
--rw-r--r--   0        0        0     2383 2023-04-19 00:24:53.724298 minivnn-0.1.0/minivnn/minivnn.py
--rw-r--r--   0        0        0      571 2023-04-19 00:24:53.724298 minivnn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 minivnn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1462 2023-04-28 16:54:37.828875 minivnn-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2023-04-28 16:54:37.828875 minivnn-0.1.1/minivnn/__init__.py
+-rw-r--r--   0        0        0     3181 2023-04-28 16:54:37.828875 minivnn-0.1.1/minivnn/minivnn.py
+-rw-r--r--   0        0        0      684 2023-04-28 16:54:37.828875 minivnn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 minivnn-0.1.1/PKG-INFO
```

### Comparing `minivnn-0.1.0/README.md` & `minivnn-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # minivnn
 
-![Tests and Lint](https://github.com/aismlv/minivnn/actions/workflows/test_and_lint.yml/badge.svg)
-![Publish to PyPI](https://github.com/aismlv/minivnn/actions/workflows/publish.yml/badge.svg)
+![Tests](https://github.com/aismlv/minivnn/actions/workflows/test_and_lint.yml/badge.svg)
+[![codecov](https://codecov.io/gh/aismlv/minivnn/branch/main/graph/badge.svg?token=5J503UR8O7)](https://codecov.io/gh/aismlv/minivnn)
 [![PyPI version](https://badge.fury.io/py/minivnn.svg)](https://pypi.org/project/minivnn/)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 `minivnn` (pronounced "minivan" 🚐) is an exact nearest neighbor search Python library for those times when "approximate" just won't cut it (or is simply overkill).
 
 ## Installation
 
@@ -26,20 +26,18 @@
 index = Index(dim=128, metric="cosine")
 
 # Add embeddings to the index
 embedding1 = np.random.rand(128)
 embedding2 = np.random.rand(128)
 embedding3 = np.random.rand(128)
 
-index.add(1, embedding1)
-index.add(2, embedding2)
-index.add(3, embedding3)
+index.add([1, 2, 3], [embedding1, embedding2, embedding3])
 
 # Delete embeddings from the index
-index.delete(3)
+index.delete_items([3])
 
 # Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
 ```
```

### Comparing `minivnn-0.1.0/minivnn/minivnn.py` & `minivnn-0.1.1/minivnn/minivnn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,80 @@
+from typing import List, Tuple, Union
+
 import numpy as np
-from typing import List, Tuple
+
+DOT_PRODUCT = "dot_product"
+COSINE = "cosine"
 
 
 def normalize(embedding: np.ndarray) -> np.ndarray:
     return embedding / np.linalg.norm(embedding)
 
 
 class Index:
-    def __init__(self, dim: int, metric: str = "dot") -> None:
+    def __init__(self, dim: int, metric: str = DOT_PRODUCT) -> None:
         self.dim = dim
         self.metric = metric
         self.embeddings = np.empty((0, dim))
         self.index_map: List[int] = []
 
-    def add(self, index: int, embedding: np.ndarray) -> None:
-        if index in self.index_map:
-            raise ValueError(f"Index {index} already exists.")
-
-        embedding = embedding.reshape(1, -1)
-        if embedding.shape[1] != self.dim:
-            raise ValueError(f"Embedding has invalid dimension: {embedding.shape}. Expected dimension: {self.dim}.")
-        if self.metric == "cosine":
-            embedding = normalize(embedding)
-
-        self.embeddings = np.append(self.embeddings, embedding.reshape(1, -1), axis=0)
-        self.index_map.append(index)
-
-    def delete(self, index: int) -> None:
-        if index not in self.index_map:
-            raise ValueError(f"Index {index} not found.")
-        row_to_delete = self.index_map.index(index)
-        self.embeddings = np.delete(self.embeddings, row_to_delete, axis=0)
-        del self.index_map[row_to_delete]
+    def add_items(self, indices: List[int], embeddings: Union[List[np.ndarray], np.ndarray]) -> None:
+        for index in indices:
+            if index in self.index_map:
+                raise ValueError(f"Index {index} already exists.")
+
+        if isinstance(embeddings, list):
+            embeddings = [embedding.reshape(1, -1) for embedding in embeddings]
+            for embedding in embeddings:
+                if embedding.shape[1] != self.dim:
+                    raise ValueError(
+                        f"Embedding has invalid dimension: {embedding.shape[1]}. Expected dimension: {self.dim}."
+                    )
+            embeddings = np.vstack(embeddings)
+
+        elif isinstance(embeddings, np.ndarray):
+            if embeddings.shape != (len(indices), self.dim):
+                raise ValueError(
+                    f"Embedding has invalid shape: {embeddings.shape}. Expected shape: {(len(indices), self.dim)}."
+                )
+
+        if self.metric == COSINE:
+            embeddings = normalize(embeddings)
+
+        self.embeddings = np.append(self.embeddings, embeddings, axis=0)
+        self.index_map.extend(indices)
+
+    def delete_items(self, indices: List[int]) -> None:
+        for index in indices:
+            if index not in self.index_map:
+                raise ValueError(f"Index {index} not found.")
+
+        rows_to_delete = [self.index_map.index(index) for index in indices]
+        self.embeddings = np.delete(self.embeddings, rows_to_delete, axis=0)
+
+        for index in rows_to_delete:
+            del self.index_map[index]
 
     def save(self, filepath: str) -> None:
         np.savez_compressed(filepath, embeddings=self.embeddings, index_map=np.array(self.index_map))
 
     def load(self, filepath: str) -> None:
         with np.load(filepath) as data:
             self.embeddings = data["embeddings"]
             self.index_map = data["index_map"].tolist()
 
     def query(self, query_embedding: np.ndarray, k: int = 1) -> List[Tuple[int, float]]:
-        if self.metric == "dot":
+        if self.metric == DOT_PRODUCT:
             similarities = np.dot(self.embeddings, query_embedding)
-        elif self.metric == "cosine":
+        elif self.metric == COSINE:
             normalized_query = normalize(query_embedding)
             similarities = np.dot(self.embeddings, normalized_query)
         else:
-            raise ValueError(f"Invalid metric: {self.metric}. Supported metrics are 'dot' and 'cosine'.")
+            raise ValueError(
+                f"Invalid metric: {self.metric}. " f"Supported metrics are '{DOT_PRODUCT}' and '{COSINE}'."
+            )
 
         top_k_indices = np.argpartition(similarities, -k)[-k:]
         top_k_indices_sorted = top_k_indices[np.argsort(-similarities[top_k_indices])]
         top_k_values = similarities[top_k_indices_sorted]
 
         return [(self.index_map[i], similarity) for i, similarity in zip(top_k_indices_sorted, top_k_values)]
```

### Comparing `minivnn-0.1.0/pyproject.toml` & `minivnn-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minivnn"
-version = "0.1.0"
+version = "0.1.1"
 description = "Exact nearest neighbor search library for those times when \"approximate\" just won't cut it (or is simply overkill)"
 authors = ["aismlv <adilzhan.ismailov@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,20 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pre-commit = "^3.2.2"
+pytest-cov = "^4.0.0"
+
+[tool.poetry.group.benchmark]
+optional = true
+
+[tool.poetry.group.benchmark.dependencies]
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `minivnn-0.1.0/PKG-INFO` & `minivnn-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minivnn
-Version: 0.1.0
+Version: 0.1.1
 Summary: Exact nearest neighbor search library for those times when "approximate" just won't cut it (or is simply overkill)
 License: Apache-2.0
 Author: aismlv
 Author-email: adilzhan.ismailov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # minivnn
 
-![Tests and Lint](https://github.com/aismlv/minivnn/actions/workflows/test_and_lint.yml/badge.svg)
-![Publish to PyPI](https://github.com/aismlv/minivnn/actions/workflows/publish.yml/badge.svg)
+![Tests](https://github.com/aismlv/minivnn/actions/workflows/test_and_lint.yml/badge.svg)
+[![codecov](https://codecov.io/gh/aismlv/minivnn/branch/main/graph/badge.svg?token=5J503UR8O7)](https://codecov.io/gh/aismlv/minivnn)
 [![PyPI version](https://badge.fury.io/py/minivnn.svg)](https://pypi.org/project/minivnn/)
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 `minivnn` (pronounced "minivan" 🚐) is an exact nearest neighbor search Python library for those times when "approximate" just won't cut it (or is simply overkill).
 
 ## Installation
 
@@ -42,20 +42,18 @@
 index = Index(dim=128, metric="cosine")
 
 # Add embeddings to the index
 embedding1 = np.random.rand(128)
 embedding2 = np.random.rand(128)
 embedding3 = np.random.rand(128)
 
-index.add(1, embedding1)
-index.add(2, embedding2)
-index.add(3, embedding3)
+index.add([1, 2, 3], [embedding1, embedding2, embedding3])
 
 # Delete embeddings from the index
-index.delete(3)
+index.delete_items([3])
 
 # Query the index for the nearest neighbor of a given embedding
 query_embedding = np.random.rand(128)
 result = index.query(query_embedding, k=1)
 
 print(result)  # Returns [(index, similarity)] of the nearest neighbor
 ```
```

