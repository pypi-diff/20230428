# Comparing `tmp/redis_simple_orm-1.2.6.tar.gz` & `tmp/redis_simple_orm-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-1.2.6.tar", last modified: Fri Apr 21 04:26:02 2023, max compression
+gzip compressed data, was "redis_simple_orm-1.2.7.tar", last modified: Fri Apr 28 18:00:35 2023, max compression
```

## Comparing `redis_simple_orm-1.2.6.tar` & `redis_simple_orm-1.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/aioredis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/aioredis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_model.py
```

### Comparing `redis_simple_orm-1.2.6/LICENSE` & `redis_simple_orm-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/PKG-INFO` & `redis_simple_orm-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: redis-py
 Provides-Extra: aioredis
 Provides-Extra: txredisapi
 License-File: LICENSE
 
 # WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
-If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
-> __NOTE__: Please be aware, that this module is way too simple.
-> Your data will likely will be replaced without warning.
-> Do not use for your main data storage.
+As an inspiration and a very good alternative, 
+please take a look on [walrus](https://walrus.readthedocs.org).
+
+> __NOTE__: Please be aware, Your data might be replaced without warning.
+
 
 ## Suggestion for this Module Usage
 
  - In case you need to update `index` value,
    Implement `update` method on `Model` that will remove old `index` value 
    on index data / redis, then save new `index` value
 
@@ -206,23 +208,25 @@
 	assert len(users) == 0
 
 
 main()
 ```
 
 
-## Usage Example (`asyncio` version)
+## Usage Example (`asyncio` version, also works with `aioredis`)
 
 ### Model
 
 `model.py`
 ```python
 from dataclasses import dataclass, field
 
 from aioredis import Redis
+# Alternative
+# from redis.asyncio import Redis
 from RSO.aioredis.index import (
 	HashIndex as AsyncHashIndex, 
 	SetIndex as AsyncSetIndex
 )
 from RSO.aioredis.model import Model as AsyncModel
 
 from data import USERS
@@ -262,20 +266,20 @@
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
-    	result = {}
-    	for key, value in self.dict().items():
-    		if value is None:
-    			continue
-    		result[key] = value
-    	return result
+        result = {}
+        for key, value in self.dict().items():
+            if value is None:
+                continue
+            result[key] = value
+        return result
 
 
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
         return await AsyncSingleIndexUsername.search_model(redis, username, cls)
@@ -477,9 +481,8 @@
 
 
 if __name__ == "__main__":
     main()\
         .addCallback(lambda ign: reactor.stop())\
         .addErrback(lambda ign: reactor.stop())
     reactor.run()
-
 ```
```

### Comparing `redis_simple_orm-1.2.6/README.md` & `redis_simple_orm-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
-If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
-> __NOTE__: Please be aware, that this module is way too simple.
-> Your data will likely will be replaced without warning.
-> Do not use for your main data storage.
+As an inspiration and a very good alternative, 
+please take a look on [walrus](https://walrus.readthedocs.org).
+
+> __NOTE__: Please be aware, Your data might be replaced without warning.
+
 
 ## Suggestion for this Module Usage
 
  - In case you need to update `index` value,
    Implement `update` method on `Model` that will remove old `index` value 
    on index data / redis, then save new `index` value
 
@@ -182,23 +183,25 @@
 	assert len(users) == 0
 
 
 main()
 ```
 
 
-## Usage Example (`asyncio` version)
+## Usage Example (`asyncio` version, also works with `aioredis`)
 
 ### Model
 
 `model.py`
 ```python
 from dataclasses import dataclass, field
 
 from aioredis import Redis
+# Alternative
+# from redis.asyncio import Redis
 from RSO.aioredis.index import (
 	HashIndex as AsyncHashIndex, 
 	SetIndex as AsyncSetIndex
 )
 from RSO.aioredis.model import Model as AsyncModel
 
 from data import USERS
@@ -238,20 +241,20 @@
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
-    	result = {}
-    	for key, value in self.dict().items():
-    		if value is None:
-    			continue
-    		result[key] = value
-    	return result
+        result = {}
+        for key, value in self.dict().items():
+            if value is None:
+                continue
+            result[key] = value
+        return result
 
 
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
         return await AsyncSingleIndexUsername.search_model(redis, username, cls)
@@ -453,9 +456,8 @@
 
 
 if __name__ == "__main__":
     main()\
         .addCallback(lambda ign: reactor.stop())\
         .addErrback(lambda ign: reactor.stop())
     reactor.run()
-
 ```
```

### Comparing `redis_simple_orm-1.2.6/RSO/aioredis/index.py` & `redis_simple_orm-1.2.7/RSO/aioredis/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/RSO/aioredis/model.py` & `redis_simple_orm-1.2.7/RSO/aioredis/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Union
 
 from aioredis import __version__ as aioredis_version
 try:
     from aioredis.client import Redis, Pipeline
 except ModuleNotFoundError:
     from aioredis.commands import Redis, Pipeline
-
+from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
 from RSO.base import BaseModel
 from .index import ListIndex
 
 
 old_aioredis = aioredis_version < '2.0.0'
 
 
@@ -30,30 +30,32 @@
             elif isinstance(value, (date, datetime)):
                 dict_data[key] = value.isoformat()
             elif isinstance(value, Enum):
                 dict_data[key] = value.value
         return dict_data
 
     async def save(self, redis: Union[Pipeline, Redis]):
-        if isinstance(redis, Pipeline):
+        if isinstance(redis, (Pipeline, Pipeline2)):
             pipe = redis
         else:
             pipe = redis.pipeline()
 
         if old_aioredis:
             pipe.hset_dict(self.redis_key, mapping=self.to_redis())
         else:
             pipe.hset(self.redis_key, mapping=self.to_redis())
 
         for index_class in self.__indexes__:
             index = index_class.create_from_model_class(self)
             if getattr(self, index_class.__key__, None) is None:
                 continue
             await index.save_index(pipe)
-        await pipe.execute()
+
+        if not isinstance(redis, (Pipeline, Pipeline2)):
+            await pipe.execute()
 
     async def extended_save(self, redis: Union[Pipeline, Redis]):
         """
         Extender of `save` method to avoid saving our key value
         to be saved multiple times on ListIndex
         """
         list_index_map = {}
```

### Comparing `redis_simple_orm-1.2.6/RSO/base.py` & `redis_simple_orm-1.2.7/RSO/base.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/RSO/index.py` & `redis_simple_orm-1.2.7/RSO/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/RSO/model.py` & `redis_simple_orm-1.2.7/RSO/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
         pipe.hset(self.redis_key, mapping=self.to_redis())
         for index_class in self.__indexes__ or []:
             if getattr(self, index_class.__key__) is None:
                 continue
             index = index_class.create_from_model_class(self)
             index.save_index(pipe)
-        pipe.execute()
+
+        if not isinstance(redis, Pipeline):
+            pipe.execute()
 
     @classmethod
     def search(cls, redis: Redis, value):
         redis_key = cls._to_redis_key(value)
         if bool(redis.exists(redis_key)):
             fields = cls.get_fields()
             redis_data = redis.hmget(redis_key, fields)
```

### Comparing `redis_simple_orm-1.2.6/RSO/txredisapi/index.py` & `redis_simple_orm-1.2.7/RSO/txredisapi/index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/RSO/txredisapi/model.py` & `redis_simple_orm-1.2.7/RSO/txredisapi/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-1.2.7/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: redis-py
 Provides-Extra: aioredis
 Provides-Extra: txredisapi
 License-File: LICENSE
 
 # WARNING: Old data might be replaced with new one without warning
 
 # Redis Simple ORM
 
 Redis ORM in Simple Way.
-If you find this module is too simple, please take a look on [walrus](https://walrus.readthedocs.org).
 
-> __NOTE__: Please be aware, that this module is way too simple.
-> Your data will likely will be replaced without warning.
-> Do not use for your main data storage.
+As an inspiration and a very good alternative, 
+please take a look on [walrus](https://walrus.readthedocs.org).
+
+> __NOTE__: Please be aware, Your data might be replaced without warning.
+
 
 ## Suggestion for this Module Usage
 
  - In case you need to update `index` value,
    Implement `update` method on `Model` that will remove old `index` value 
    on index data / redis, then save new `index` value
 
@@ -206,23 +208,25 @@
 	assert len(users) == 0
 
 
 main()
 ```
 
 
-## Usage Example (`asyncio` version)
+## Usage Example (`asyncio` version, also works with `aioredis`)
 
 ### Model
 
 `model.py`
 ```python
 from dataclasses import dataclass, field
 
 from aioredis import Redis
+# Alternative
+# from redis.asyncio import Redis
 from RSO.aioredis.index import (
 	HashIndex as AsyncHashIndex, 
 	SetIndex as AsyncSetIndex
 )
 from RSO.aioredis.model import Model as AsyncModel
 
 from data import USERS
@@ -262,20 +266,20 @@
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
-    	result = {}
-    	for key, value in self.dict().items():
-    		if value is None:
-    			continue
-    		result[key] = value
-    	return result
+        result = {}
+        for key, value in self.dict().items():
+            if value is None:
+                continue
+            result[key] = value
+        return result
 
 
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
         return await AsyncSingleIndexUsername.search_model(redis, username, cls)
@@ -477,9 +481,8 @@
 
 
 if __name__ == "__main__":
     main()\
         .addCallback(lambda ign: reactor.stop())\
         .addErrback(lambda ign: reactor.stop())
     reactor.run()
-
 ```
```

### Comparing `redis_simple_orm-1.2.6/setup.py` & `redis_simple_orm-1.2.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,12 +61,13 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `redis_simple_orm-1.2.6/tests/test_example.py` & `redis_simple_orm-1.2.7/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/tests/test_index.py` & `redis_simple_orm-1.2.7/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.6/tests/test_model.py` & `redis_simple_orm-1.2.7/tests/test_model.py`

 * *Files identical despite different names*

