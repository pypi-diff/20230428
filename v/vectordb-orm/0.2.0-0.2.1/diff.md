# Comparing `tmp/vectordb_orm-0.2.0.tar.gz` & `tmp/vectordb_orm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb_orm-0.2.0.tar", max compression
+gzip compressed data, was "vectordb_orm-0.2.1.tar", max compression
```

## Comparing `vectordb_orm-0.2.0.tar` & `vectordb_orm-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1071 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/LICENSE
--rw-r--r--   0        0        0     7130 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/README.md
--rw-r--r--   0        0        0      497 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      906 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/__init__.py
--rw-r--r--   0        0        0     1582 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/attributes.py
--rw-r--r--   0        0        0        0 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/__init__.py
--rw-r--r--   0        0        0     2033 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/base.py
--rw-r--r--   0        0        0      155 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/__init__.py
--rw-r--r--   0        0        0    10264 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/indexes.py
--rw-r--r--   0        0        0    13202 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/milvus.py
--rw-r--r--   0        0        0      746 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/milvus/similarity.py
--rw-r--r--   0        0        0      107 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/__init__.py
--rw-r--r--   0        0        0      884 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/indexes.py
--rw-r--r--   0        0        0     9671 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/pinecone.py
--rw-r--r--   0        0        0     3594 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/base.py
--rw-r--r--   0        0        0      473 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/enums.py
--rw-r--r--   0        0        0      984 2023-04-21 21:31:03.366996 vectordb_orm-0.2.0/vectordb_orm/fields.py
--rw-r--r--   0        0        0       26 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/index.py
--rw-r--r--   0        0        0     4342 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/query.py
--rw-r--r--   0        0        0      364 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/results.py
--rw-r--r--   0        0        0     1435 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/session.py
--rw-r--r--   0        0        0        0 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/__init__.py
--rw-r--r--   0        0        0     1609 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/__init__.py
--rw-r--r--   0        0        0     3603 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_indexes.py
--rw-r--r--   0        0        0     1194 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_milvus.py
--rw-r--r--   0        0        0     1114 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/models.py
--rw-r--r--   0        0        0     2537 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/test_base.py
--rw-r--r--   0        0        0     2756 2023-04-21 21:31:03.370996 vectordb_orm-0.2.0/vectordb_orm/tests/test_query.py
--rw-r--r--   0        0        0     7642 1970-01-01 00:00:00.000000 vectordb_orm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8503 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/README.md
+-rw-r--r--   0        0        0      514 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      906 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/__init__.py
+-rw-r--r--   0        0        0     1582 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/attributes.py
+-rw-r--r--   0        0        0        0 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/__init__.py
+-rw-r--r--   0        0        0     2163 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/base.py
+-rw-r--r--   0        0        0      155 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/milvus/__init__.py
+-rw-r--r--   0        0        0    10264 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/milvus/indexes.py
+-rw-r--r--   0        0        0    16791 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/milvus/milvus.py
+-rw-r--r--   0        0        0      746 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/milvus/similarity.py
+-rw-r--r--   0        0        0      107 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/pinecone/__init__.py
+-rw-r--r--   0        0        0      884 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/pinecone/indexes.py
+-rw-r--r--   0        0        0    11958 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/backends/pinecone/pinecone.py
+-rw-r--r--   0        0        0     4056 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/base.py
+-rw-r--r--   0        0        0      473 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/enums.py
+-rw-r--r--   0        0        0      984 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/fields.py
+-rw-r--r--   0        0        0       26 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/index.py
+-rw-r--r--   0        0        0     4342 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/query.py
+-rw-r--r--   0        0        0      364 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/results.py
+-rw-r--r--   0        0        0     1736 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/session.py
+-rw-r--r--   0        0        0        0 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/milvus/__init__.py
+-rw-r--r--   0        0        0     3653 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/milvus/test_indexes.py
+-rw-r--r--   0        0        0     1196 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/milvus/test_milvus.py
+-rw-r--r--   0        0        0     1140 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/models.py
+-rw-r--r--   0        0        0     4031 2023-04-28 03:36:31.687984 vectordb_orm-0.2.1/vectordb_orm/tests/test_base.py
+-rw-r--r--   0        0        0     2757 2023-04-28 03:36:31.691984 vectordb_orm-0.2.1/vectordb_orm/tests/test_query.py
+-rw-r--r--   0        0        0     9053 1970-01-01 00:00:00.000000 vectordb_orm-0.2.1/PKG-INFO
```

### Comparing `vectordb_orm-0.2.0/LICENSE` & `vectordb_orm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/README.md` & `vectordb_orm-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 # vectordb-orm
 
-`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases. This project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax. Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
+`vectordb-orm` is an Object-Relational Mapping (ORM) library for vector databases. Define your data as objects and query for them using familiar SQL syntax, with all the added power of lighting fast vector search.
+
+Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
 
 ## Getting Started
 
-Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with python typehints that define the type of vector and metadata that will be stored alongisde the objects.
+Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with typehints that define the type of vector and metadata that will be stored alongisde the objects.
 
 You create a class definition by subclassing `VectorSchemaBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.
 
-Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
-
-```bash
-git clone https://github.com/piercefreeman/vectordb-orm.git
-cd vectordb-orm
-docker-compose up -d
-```
-
-| Field Type      | Description                                                                                                                                                                                                                                |
-|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
-| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
-| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
-| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
-
 ### Object Definition
 
-Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation.
+Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation. In the below example the Milvus schema requires a Milvus index like `Milvus_IVF_FLAT` (for the full list of supported values see [here](./tree/main/vectordb_orm/backends/milvus/indexes.py)) and the Pinecone schema uses the default `PineconeIndex` with a cosine similarity metric.
 
 Milvus:
 
 ```python
 from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, Milvus_IVF_FLAT
 import numpy as np
 
@@ -51,76 +38,124 @@
     __collection_name__ = 'my_object_collection'
 
     id: int = PrimaryKeyField()
     text: str = VarCharField(max_length=128)
     embedding: np.ndarray = EmbeddingField(dim=128, index=PineconeIndex(metric_type=PineconeSimilarityMetric.COSINE))
 ```
 
-## Embedding Types
+### Indexing Data
 
-We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+To insert objects into the database, create a new instance of your object class and insert into the current session. The arguments to the init function mirror the typehinted schema that you defined above.
 
-For binary:
+```python
+obj = MyObject(text="my_text", embedding=np.array([1.0]*128))
+session.insert(obj)
+```
+
+Once inserted, this object will be populated with a new `id` by the database engine. At this point it should be queryable (modulo some backends taking time for eventual consistency across different shards).
+
+`vectordb-orm` also supports batch insertion. This is recommended in cases where you have a lot of data to insert at one time, since latencies can be significant on individual datapoints.
 
 ```python
-embedding: np.ndarray[np.bool_] = EmbeddingField(
-    dim=128,
-    index=FLAT()
-)
+obj = MyObject(text="my_text", embedding=np.array([1.0]*128))
+session.insert_batch([obj], show_progress=True)
 ```
 
-For floating point:
+The optional `show_progress` allows you to show a progress bar to show the current status of the insertion and the estimated time remaining for the whole dataset.
+
+### Querying Syntax
 
 ```python
-embedding: np.ndarray = EmbeddingField(
-    dim=128,
-    index=BIN_FLAT()
-)
+session = VectorSession(...)
+
+# Perform a simple boolean query
+results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
+
+# Rank results by their similarity to a given reference vector
+query_vector = np.array([8.0]*128)
+results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
 ```
 
-## Querying Syntax
+### Session Creation
+
+Milvus:
 
 ```python
 from pymilvus import Milvus, connections
 from vectordb_orm import MilvusBackend, VectorSession
 
 # Instantiate a Milvus session
 session = VectorSession(MilvusBackend(Milvus()))
 connections.connect("default", host="localhost", port="19530")
+session.create_collection(MyObject)
 ```
 
+Pinecone:
+
 ```python
 from vectordb_orm import PineconeBackend, VectorSession
 
 # Instantiate a Pinecone session
 session = VectorSession(
     PineconeBackend(
         api_key=getenv("PINECONE_API_KEY"),
         environment=getenv("PINECONE_ENVIRONMENT"),
     )
 )
+session.create_collection(MyObject)
 ```
 
+## Embedding Types
+
+We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+
+For binary:
+
 ```python
-# Perform a simple boolean query
-results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
+embedding: np.ndarray[np.bool_] = EmbeddingField(
+    dim=128,
+    index=FLAT()
+)
+```
 
-# Rank results by their similarity to a given reference vector
-query_vector = np.array([8.0]*128)
-results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
+For floating point:
+
+```python
+embedding: np.ndarray = EmbeddingField(
+    dim=128,
+    index=BIN_FLAT()
+)
 ```
 
+## Field Types
+
+
+| Field Type      | Description                                                                                                                                                                                                                                |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
+| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
+| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
+| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
+
 ## Installation
 
 To get started with vectordb-orm, simply install the package and its dependencies, then import the necessary modules:
 
 ```bash
 pip install vectordb-orm
 ```
 
+Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
+
+```bash
+git clone https://github.com/piercefreeman/vectordb-orm.git
+cd vectordb-orm
+docker-compose up -d
+```
+
 We use poetry for local development work:
 
 ```bash
 poetry install
 poetry run pytest
 ```
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/__init__.py` & `vectordb_orm-0.2.1/vectordb_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/attributes.py` & `vectordb_orm-0.2.1/vectordb_orm/attributes.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/base.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         pass
 
     @abstractmethod
     def insert(self, entity: VectorSchemaBase) -> int:
         pass
 
     @abstractmethod
+    def insert_batch(self, entities: list[VectorSchemaBase], show_progress: bool) -> list[int]:
+        pass
+
+    @abstractmethod
     def delete(self, entity: VectorSchemaBase):
         pass
 
     @abstractmethod
     def search(
         self,
         schema: Type[VectorSchemaBase],
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/milvus/indexes.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/milvus/indexes.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/milvus/milvus.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/milvus/milvus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from logging import info
 from typing import Any, Type, get_args, get_origin
 
 import numpy as np
 from pymilvus import Collection, Milvus
 from pymilvus.client.abstract import ChunkedQueryResult
 from pymilvus.client.types import DataType
@@ -68,14 +69,89 @@
 
     def insert(self, entity: VectorSchemaBase) -> int:
         entities = self._dict_representation(entity)
         print("Entity insertion", entities)
         mutation_result = self.client.insert(collection_name=entity.__class__.collection_name(), entities=entities)
         return mutation_result.primary_keys[0]
 
+    def insert_batch(
+        self,
+        entities: list[VectorSchemaBase],
+        show_progress: bool,
+    ) -> list[int]:
+        if show_progress:
+            raise ValueError("Milvus backend does not support batch insertion progress logging because it is done in one operation.")
+
+        # Group by the schema type since we allow for the insertion of multiple different schema
+        # `schema_to_entities` - input entities grouped by the schema name
+        # `schema_to_original_index` - since we switch to a per-schema representation, keep track of a mapping
+        #    from the schema to the original index in `entities`
+        # `schema_to_ids` - map of schema to the resulting primary keys
+        schema_to_original_index = defaultdict(list)
+        schema_to_class = {}
+        schema_to_ids = {}
+
+        for i, entity in enumerate(entities):
+            schema = entity.__class__
+            schema_name = schema.collection_name()
+
+            schema_to_original_index[schema_name].append(i)
+            schema_to_class[schema_name] = schema
+
+        for schema_name, schema_indexes in schema_to_original_index.items():
+            schema = schema_to_class[schema_name]
+            schema_entities = [entities[index] for index in schema_indexes]
+
+            # The primary key should be null at this stage of things, so we ignore it
+            # during the insertion
+            ignore_keys = {
+                self._get_primary(schema)
+            }
+
+            # Group this schema's objects by their keys
+            by_key_values = defaultdict(list)
+            by_key_type = {}
+
+            for entity in schema_entities:
+                for attribute_name, type_hint in entity.__annotations__.items():
+                    value = getattr(entity, attribute_name)
+                    db_type, value = self._type_to_value(type_hint, value)
+                    by_key_values[attribute_name].append(value)
+                    by_key_type[attribute_name] = db_type
+
+            # Ensure each key in `schema_to_objects` matches the quantity of objects
+            # that should have been created. This *shouldn't* happen but it's possible
+            # some combination of programatically deleting attributes or annotations will
+            # lead to this case. We proactively raise an error because this could result in
+            # data corruption.
+            all_lengths = {len(values) for values in by_key_values.values()}
+            if len(all_lengths) > 1:
+                raise ValueError(f"Inserted objects don't align for schema `{schema_name}`")
+
+            payload = [
+                {
+                    "name": attribute_name,
+                    "type": by_key_type[attribute_name],
+                    "values": values,
+                }
+                for attribute_name, values in by_key_values.items()
+                if attribute_name not in ignore_keys
+            ]
+
+            mutation_result = self.client.insert(collection_name=schema_name, entities=payload)
+            schema_to_ids[schema_name] = mutation_result.primary_keys
+
+        # Reorder ids to match the input entities
+        ordered_ids = [None] * len(entities)
+        for schema_name, primary_keys in schema_to_ids.items():
+            for i, original_index in enumerate(schema_to_original_index[schema_name]):
+                ordered_ids[original_index] = primary_keys[i]
+
+        return ordered_ids
+
     def delete(self, entity: VectorSchemaBase):
         schema = entity.__class__
         identifier_key = self._get_primary(schema)
         # Milvus only supports deleting entities with the `in` conditional; equality doesn't work
         delete_expression = f"{identifier_key} in [{entity.id}]"
         self.client.delete(collection_name=schema.collection_name(), expr=delete_expression)
 
@@ -224,15 +300,21 @@
         """
         payload = []
 
         for attribute_name, type_hint in entity.__annotations__.items():
             value = getattr(entity, attribute_name)
             if value is not None:
                 db_type, value = self._type_to_value(type_hint, value)
-                payload.append({"name": attribute_name, "type": db_type, "values": [value]})
+                payload.append(
+                    {
+                        "name": attribute_name,
+                        "type": db_type,
+                        "values": [value]
+                    }
+                )
         return payload
 
     def _assert_embedding_validity(self, schema: Type[VectorSchemaBase]):
         """
         Ensure that the embedding configurations align with the typehinting
         """
         # For all embeddings, create an associated index
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/milvus/similarity.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/milvus/similarity.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/indexes.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/pinecone/indexes.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/backends/pinecone/pinecone.py` & `vectordb_orm-0.2.1/vectordb_orm/backends/pinecone/pinecone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from collections import defaultdict
 from logging import info
 from re import match as re_match
 from typing import Type
 from uuid import uuid4
 
 import numpy as np
 import pinecone
+from tqdm import tqdm
 
-from vectordb_orm.attributes import AttributeCompare
+from vectordb_orm.attributes import AttributeCompare, OperationType
 from vectordb_orm.backends.base import BackendBase
 from vectordb_orm.backends.pinecone.indexes import PineconeIndex
 from vectordb_orm.base import VectorSchemaBase
 from vectordb_orm.fields import EmbeddingField
 from vectordb_orm.results import QueryResult
-from vectordb_orm.attributes import OperationType
 
 
 class PineconeBackend(BackendBase):
     max_fetch_size = 1000
 
     def __init__(
         self,
@@ -95,40 +96,80 @@
 
         pinecone.delete_index(collection_name)
 
     def insert(self, entity: VectorSchemaBase) -> list:
         schema = entity.__class__
         collection_name = self.transform_collection_name(schema.collection_name())
 
-        schema = entity.__class__
         embedding_field_key, _ = self._get_embedding_field(schema)
         primary_key = self._get_primary(schema)
 
-        id = uuid4().int & (1<<64)-1
-
-        embedding_value : np.ndarray = getattr(entity, embedding_field_key)
-        metadata_fields = {
-            key: getattr(entity, key)
-            for key in schema.__annotations__.keys()
-            if key not in {embedding_field_key, primary_key}
-        }
+        identifier = uuid4().int & (1<<64)-1
 
         index = pinecone.Index(index_name=collection_name)
         index.upsert([
-            (
-                str(id),
-                embedding_value.tolist(),
-                {
-                    **metadata_fields,
-                    primary_key: id,
-                }
-            ),
+            self._prepare_upsert_tuple(
+                entity,
+                identifier,
+                embedding_field_key=embedding_field_key,
+                primary_key=primary_key,
+            )
         ])
 
-        return id
+        return identifier
+
+    def insert_batch(
+        self,
+        entities: list[VectorSchemaBase],
+        show_progress: bool,
+        batch_size: int = 100
+    ) -> list[int]:
+        identifiers = [
+            uuid4().int & (1<<64)-1
+            for _ in range(len(entities))
+        ]
+
+        # Group by the objects
+        schema_to_original_index = defaultdict(list)
+        schema_to_class = {}
+
+        for i, entity in enumerate(entities):
+            schema = entity.__class__
+            schema_name = schema.collection_name()
+
+            schema_to_original_index[schema_name].append(i)
+            schema_to_class[schema_name] = schema
+
+        for schema_name, original_indexes in schema_to_original_index.items():
+            schema = schema_to_class[schema_name]
+            collection_name = self.transform_collection_name(schema.collection_name())
+
+            index = pinecone.Index(index_name=collection_name)
+
+            embedding_field_key, _ = self._get_embedding_field(schema)
+            primary_key = self._get_primary(schema)
+
+            for i in tqdm(range(0, len(original_indexes), batch_size)):
+                batch_indexes = original_indexes[i:i+batch_size]
+                batch_entities = [entities[index] for index in batch_indexes]
+                batch_identifiers = [identifiers[index] for index in batch_indexes]
+
+                index.upsert(
+                    [
+                        self._prepare_upsert_tuple(
+                            entity,
+                            identifier,
+                            embedding_field_key=embedding_field_key,
+                            primary_key=primary_key,
+                        )
+                        for entity, identifier in zip(batch_entities, batch_identifiers)
+                    ]
+                )
+
+        return identifiers
 
     def delete(self, entity: VectorSchemaBase):
         schema = entity.__class__
         collection_name = self.transform_collection_name(schema.collection_name())
         index = pinecone.Index(index_name=collection_name)
         delete_response = index.delete(ids=[str(entity.id)])
         if delete_response:
@@ -250,7 +291,35 @@
             OperationType.NOT_EQUAL: "$ne",
             # TODO: Support $in and $nin
         }
 
         return {
             operation_type_maps[attribute.op]: attribute.value
         }
+
+    def _prepare_upsert_tuple(
+        self,
+        entity: VectorSchemaBase,
+        identifier: int,
+        embedding_field_key: str,
+        primary_key: str,
+    ):
+        """
+        Formats a tuple for upsert
+        """
+        schema = entity.__class__
+
+        embedding_value : np.ndarray = getattr(entity, embedding_field_key)
+        metadata_fields = {
+            key: getattr(entity, key)
+            for key in schema.__annotations__.keys()
+            if key not in {embedding_field_key, primary_key}
+        }
+
+        return (
+            str(identifier),
+            embedding_value.tolist(),
+            {
+                **metadata_fields,
+                primary_key: identifier,
+            }
+        )
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/base.py` & `vectordb_orm-0.2.1/vectordb_orm/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,15 +49,20 @@
         # Cache the type configurations and then remove the values. We want accessing the property of the
         # class to return the value of the field (or default to AttributeCompare via __getattr__ in the case of
         # a direct class attribute), not the field configuration itself.
         cls._type_configuration = {}
         for key in cls.__annotations__.keys():
             attribute_value = getattr(cls, key)
             cls._type_configuration[key] = attribute_value if isinstance(attribute_value, BaseField) else None
-            delattr(cls, key)
+            # All attributes will result in some value because we return a AttributeCompare by default
+            # for non-configured objects. Checking that the field is actually equal to a base
+            # value allows us to only delete legitimate configuration objects. Otherwise attempting to delete
+            # the synthetic AttributeCompare object will throw an error.
+            if isinstance(attribute_value, BaseField):
+                delattr(cls, key)
 
     @classmethod
     def collection_name(self) -> str:
         if not hasattr(self, '__collection_name__'):
             raise ValueError(f"Class {self.__name__} does not have a collection name, specify `__collection_name__` on the class definition.")
         return self.__collection_name__
 
@@ -72,14 +77,14 @@
         """
         Create a MilvusBase object from a dictionary.
 
         :param data: A dictionary containing the attribute names and values.
         :returns: A MilvusBase object.
         :raises ValueError: If an unexpected attribute name is encountered in the dictionary.
         """
-        obj = cls()
+        init_payload = {}
         allowed_keys = list(cls.__annotations__.keys())
         for attribute_name, value in data.items():
             if attribute_name not in allowed_keys:
                 raise ValueError(f"Key `{attribute_name}` is not allowed on {cls.__name__}")
-            setattr(obj, attribute_name, value)
-        return obj
+            init_payload[attribute_name] = value
+        return cls(**init_payload)
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/fields.py` & `vectordb_orm-0.2.1/vectordb_orm/fields.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/query.py` & `vectordb_orm-0.2.1/vectordb_orm/query.py`

 * *Files identical despite different names*

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/conftest.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from time import sleep
 
 import pytest
 from dotenv import load_dotenv
 from pymilvus import Milvus, connections
 
 from vectordb_orm import MilvusBackend, PineconeBackend, VectorSession
-from vectordb_orm.tests.models import MilvusBinaryEmbeddingObject, MilvusMyObject, PineconeMyObject
+from vectordb_orm.tests.models import (MilvusBinaryEmbeddingObject,
+                                       MilvusMyObject, PineconeMyObject)
 
 
 @pytest.fixture()
 def milvus_session():
     session = VectorSession(MilvusBackend(Milvus()))
     connections.connect("default", host="localhost", port="19530")
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_indexes.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/milvus/test_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import numpy as np
 import pytest
 from pymilvus import Milvus
 
 from vectordb_orm import (EmbeddingField, PrimaryKeyField, VectorSchemaBase,
                           VectorSession)
 from vectordb_orm.backends.milvus.indexes import (BINARY_INDEXES,
-                                                  FLOATING_INDEXES, MilvusIndexBase)
+                                                  FLOATING_INDEXES,
+                                                  MilvusIndexBase)
 from vectordb_orm.backends.milvus.similarity import (
     MilvusBinarySimilarityMetric, MilvusFloatSimilarityMetric)
 
 # Different index definitions require different kwarg arguments; we centralize
 # them here for ease of accessing them during different test runs
 INDEX_DEFAULTS = {
     "IVF_FLAT": dict(
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/milvus/test_milvus.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/milvus/test_milvus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from vectordb_orm.tests.models import MilvusBinaryEmbeddingObject
+import numpy as np
 import pytest
+
 from vectordb_orm import VectorSession
-import numpy as np
+from vectordb_orm.tests.models import MilvusBinaryEmbeddingObject
+
 
 # @pierce 04-21- 2023: Currently flaky
 # https://github.com/piercefreeman/vectordb-orm/pull/5
 @pytest.mark.xfail(strict=False)
 def test_binary_collection_query(session: VectorSession):
     # Create some MyObject instances
     obj1 = MilvusBinaryEmbeddingObject(embedding=np.array([True] * 128))
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/models.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 from vectordb_orm import (ConsistencyType, EmbeddingField, Milvus_BIN_FLAT,
-                          Milvus_IVF_FLAT, PineconeIndex, PrimaryKeyField,
-                          VarCharField, VectorSchemaBase, PineconeSimilarityMetric)
+                          Milvus_IVF_FLAT, PineconeIndex,
+                          PineconeSimilarityMetric, PrimaryKeyField,
+                          VarCharField, VectorSchemaBase)
 
 
 class MilvusMyObject(VectorSchemaBase):
     __collection_name__ = 'my_collection'
     __consistency_type__ = ConsistencyType.STRONG
 
     id: int = PrimaryKeyField()
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/test_base.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,40 @@
+from typing import Type
+
 import numpy as np
 import pytest
 
 from vectordb_orm import (EmbeddingField, PrimaryKeyField, VectorSchemaBase,
                           VectorSession)
 from vectordb_orm.backends.milvus.indexes import Milvus_IVF_FLAT
 from vectordb_orm.tests.conftest import SESSION_MODEL_PAIRS
-from typing import Type
 
 
 @pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
 def test_create_object(session: str, model: Type[VectorSchemaBase]):
     my_object = model(text='example', embedding=np.array([1.0] * 128))
     assert my_object.text == 'example'
     assert np.array_equal(my_object.embedding, np.array([1.0] * 128))
     assert my_object.id is None
 
 
 @pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
+def test_from_dict(session: str, model: Type[VectorSchemaBase]):
+    my_object = model.from_dict(
+        {
+            "text": 'example',
+            "embedding": np.array([1.0] * 128)
+        }
+    )
+    assert my_object.text == 'example'
+    assert np.array_equal(my_object.embedding, np.array([1.0] * 128))
+    assert my_object.id is None
+
+
+@pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
 def test_insert_object(session: str, model: Type[VectorSchemaBase], request):
     session : VectorSession = request.getfixturevalue(session)
 
     my_object = model(text='example', embedding=np.array([1.0] * 128))
     session.insert(my_object)
     assert my_object.id is not None
 
@@ -30,14 +44,26 @@
     # Retrieve the object and ensure the values are equivalent
     results = session.query(model).filter(model.id == my_object.id).all()
     assert len(results) == 1
 
     result : model = results[0].result
     assert result.text == my_object.text
 
+@pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
+def test_insert_batch(session: str, model: Type[VectorSchemaBase], request):
+    session : VectorSession = request.getfixturevalue(session)
+
+    obj1 = model(text='example1', embedding=np.array([1.0] * 128))
+    obj2 = model(text='example2', embedding=np.array([2.0] * 128))
+    obj3 = model(text='example3', embedding=np.array([3.0] * 128))
+
+    session.insert_batch([obj1, obj2, obj3])
+
+    for obj in [obj1, obj2, obj3]:
+        assert obj.id is not None
 
 @pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
 def test_delete_object(session: str, model: Type[VectorSchemaBase],request):
     session : VectorSession = request.getfixturevalue(session)
 
     my_object = model(text='example', embedding=np.array([1.0] * 128))
     session.insert(my_object)
@@ -67,7 +93,23 @@
         __collection_name__ = 'invalid_collection'
 
         id: int = PrimaryKeyField()
         embedding: np.ndarray[np.bool_] = EmbeddingField(dim=128, index=Milvus_IVF_FLAT(cluster_units=128))
 
     with pytest.raises(ValueError, match="not compatible with binary vectors"):
         milvus_session.create_collection(TestInvalidObject)
+
+
+def test_mixed_configuration_fields(milvus_session: VectorSession):
+    """
+    Confirm that schema definitions can mix typehints that have configuration values
+    and those that only have vanilla markup.
+
+    """
+    class TestMixedConfigurationObject(VectorSchemaBase):
+        __collection_name__ = 'mixed_configuration_collection'
+
+        id: int = PrimaryKeyField()
+        is_valid: bool
+        embedding: np.ndarray = EmbeddingField(dim=128, index=Milvus_IVF_FLAT(cluster_units=128))
+
+    milvus_session.create_collection(TestMixedConfigurationObject)
```

### Comparing `vectordb_orm-0.2.0/vectordb_orm/tests/test_query.py` & `vectordb_orm-0.2.1/vectordb_orm/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from typing import Type
+
 import numpy as np
 import pytest
 
-from vectordb_orm import VectorSession, VectorSchemaBase
+from vectordb_orm import VectorSchemaBase, VectorSession
 from vectordb_orm.tests.conftest import SESSION_MODEL_PAIRS
-from typing import Type
 
 
 @pytest.mark.parametrize("session,model", SESSION_MODEL_PAIRS)
 def test_query(session: str, model: Type[VectorSchemaBase], request):
     """
     General test of querying and query chaining
     """
```

### Comparing `vectordb_orm-0.2.0/PKG-INFO` & `vectordb_orm-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 Metadata-Version: 2.1
 Name: vectordb-orm
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pinecone-client (>=2.2.1,<3.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: pymilvus (>=2.2.6,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # vectordb-orm
 
-`vectordb-orm` is an Object-Relational Mapping (ORM) library designed to work with vector databases. This project aims to provide a consistent and convenient interface for working with vector data, allowing you to interact with vector databases using familiar ORM concepts and syntax. Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
+`vectordb-orm` is an Object-Relational Mapping (ORM) library for vector databases. Define your data as objects and query for them using familiar SQL syntax, with all the added power of lighting fast vector search.
+
+Right now [Milvus](https://milvus.io/) and [Pinecone](https://www.pinecone.io/) are supported with more backend engines planned for the future.
 
 ## Getting Started
 
-Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with python typehints that define the type of vector and metadata that will be stored alongisde the objects.
+Here are some simple examples demonstrating common behavior with vectordb-orm. First a note on structure. vectordb-orm is designed around the idea of a `Schema`, which is logically equivalent to a table in classic relational databases. This schema is marked up with typehints that define the type of vector and metadata that will be stored alongisde the objects.
 
 You create a class definition by subclassing `VectorSchemaBase` and providing typehints for the keys of your model, similar to pydantic. These fields also support custom initialization behavior if you want (or need) to modify their configuration options.
 
-Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
-
-```bash
-git clone https://github.com/piercefreeman/vectordb-orm.git
-cd vectordb-orm
-docker-compose up -d
-```
-
-| Field Type      | Description                                                                                                                                                                                                                                |
-|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
-| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
-| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
-| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
-
 ### Object Definition
 
-Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation.
+Defining a schema is almost entirely the same between backends but there are some small differences when it comes to index creation. In the below example the Milvus schema requires a Milvus index like `Milvus_IVF_FLAT` (for the full list of supported values see [here](./tree/main/vectordb_orm/backends/milvus/indexes.py)) and the Pinecone schema uses the default `PineconeIndex` with a cosine similarity metric.
 
 Milvus:
 
 ```python
 from vectordb_orm import VectorSchemaBase, EmbeddingField, VarCharField, PrimaryKeyField, Milvus_IVF_FLAT
 import numpy as np
 
@@ -67,76 +55,124 @@
     __collection_name__ = 'my_object_collection'
 
     id: int = PrimaryKeyField()
     text: str = VarCharField(max_length=128)
     embedding: np.ndarray = EmbeddingField(dim=128, index=PineconeIndex(metric_type=PineconeSimilarityMetric.COSINE))
 ```
 
-## Embedding Types
+### Indexing Data
 
-We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+To insert objects into the database, create a new instance of your object class and insert into the current session. The arguments to the init function mirror the typehinted schema that you defined above.
 
-For binary:
+```python
+obj = MyObject(text="my_text", embedding=np.array([1.0]*128))
+session.insert(obj)
+```
+
+Once inserted, this object will be populated with a new `id` by the database engine. At this point it should be queryable (modulo some backends taking time for eventual consistency across different shards).
+
+`vectordb-orm` also supports batch insertion. This is recommended in cases where you have a lot of data to insert at one time, since latencies can be significant on individual datapoints.
 
 ```python
-embedding: np.ndarray[np.bool_] = EmbeddingField(
-    dim=128,
-    index=FLAT()
-)
+obj = MyObject(text="my_text", embedding=np.array([1.0]*128))
+session.insert_batch([obj], show_progress=True)
 ```
 
-For floating point:
+The optional `show_progress` allows you to show a progress bar to show the current status of the insertion and the estimated time remaining for the whole dataset.
+
+### Querying Syntax
 
 ```python
-embedding: np.ndarray = EmbeddingField(
-    dim=128,
-    index=BIN_FLAT()
-)
+session = VectorSession(...)
+
+# Perform a simple boolean query
+results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
+
+# Rank results by their similarity to a given reference vector
+query_vector = np.array([8.0]*128)
+results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
 ```
 
-## Querying Syntax
+### Session Creation
+
+Milvus:
 
 ```python
 from pymilvus import Milvus, connections
 from vectordb_orm import MilvusBackend, VectorSession
 
 # Instantiate a Milvus session
 session = VectorSession(MilvusBackend(Milvus()))
 connections.connect("default", host="localhost", port="19530")
+session.create_collection(MyObject)
 ```
 
+Pinecone:
+
 ```python
 from vectordb_orm import PineconeBackend, VectorSession
 
 # Instantiate a Pinecone session
 session = VectorSession(
     PineconeBackend(
         api_key=getenv("PINECONE_API_KEY"),
         environment=getenv("PINECONE_ENVIRONMENT"),
     )
 )
+session.create_collection(MyObject)
 ```
 
+## Embedding Types
+
+We currently support two different types of embeddings: floating point and binary. We distinguish these based on the type signatures of the embedding array.
+
+For binary:
+
 ```python
-# Perform a simple boolean query
-results = session.query(MyObject).filter(MyObject.text == 'bar').limit(2).all()
+embedding: np.ndarray[np.bool_] = EmbeddingField(
+    dim=128,
+    index=FLAT()
+)
+```
 
-# Rank results by their similarity to a given reference vector
-query_vector = np.array([8.0]*128)
-results = session.query(MyObject).filter(MyObject.text == 'bar').order_by_similarity(MyObject.embedding, query_vector).limit(2).all()
+For floating point:
+
+```python
+embedding: np.ndarray = EmbeddingField(
+    dim=128,
+    index=BIN_FLAT()
+)
 ```
 
+## Field Types
+
+
+| Field Type      | Description                                                                                                                                                                                                                                |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| BaseField       | The `BaseField` provides the ability to add a default value for a given field. This should be used in cases where the more specific field types aren't relevant.                                                                           |
+| PrimaryKeyField | The `PrimaryKeyField` is used to specify the primary key of your model, and one is required per class.                                                                                                                                     |
+| VarCharField    | The `VarCharField` is used to specify a string field, and the `EmbeddingField` is used to specify a vector field.                                                                                                                          |
+| EmbeddingField  | The `EmbeddingField` also supports specifying an index type, which is used to specify the index type for the field. The `EmbeddingField` also supports specifying a dimension, which is used to specify the dimension of the vector field. |
+
 ## Installation
 
 To get started with vectordb-orm, simply install the package and its dependencies, then import the necessary modules:
 
 ```bash
 pip install vectordb-orm
 ```
 
+Make sure to have a vector database running on your system before connecting. We provide an archive of the [official](https://milvus.io/docs/install_standalone-docker.md) docker-compose that's mainly used for testing Milvus. Pinecone requires your API key and environment parameters.
+
+```bash
+git clone https://github.com/piercefreeman/vectordb-orm.git
+cd vectordb-orm
+docker-compose up -d
+```
+
 We use poetry for local development work:
 
 ```bash
 poetry install
 poetry run pytest
 ```
```

