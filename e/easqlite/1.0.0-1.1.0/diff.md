# Comparing `tmp/easqlite-1.0.0.tar.gz` & `tmp/easqlite-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easqlite-1.0.0.tar", last modified: Thu Apr 27 19:59:29 2023, max compression
+gzip compressed data, was "easqlite-1.1.0.tar", last modified: Thu Apr 27 22:35:24 2023, max compression
```

## Comparing `easqlite-1.0.0.tar` & `easqlite-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-1.0.0/.gitignore
--rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-1.0.0/LICENSE
--rw-r--r--   0        0        0     2701 2023-04-27 19:55:10.571434 easqlite-1.0.0/README.md
--rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-1.0.0/justfile
--rw-r--r--   0        0        0      736 2023-04-27 19:56:51.973214 easqlite-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-1.0.0/src/easqlite/__init__.py
--rw-r--r--   0        0        0     4671 2023-04-27 19:55:25.776701 easqlite-1.0.0/src/easqlite/_blob.py
--rw-r--r--   0        0        0    12008 2023-04-27 19:58:02.326449 easqlite-1.0.0/src/easqlite/_connection.py
--rw-r--r--   0        0        0     6353 2023-04-27 19:55:58.788280 easqlite-1.0.0/src/easqlite/_cursor.py
--rw-r--r--   0        0        0      884 2023-04-27 18:40:07.993622 easqlite-1.0.0/src/easqlite/_global.py
--rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-1.0.0/src/easqlite/_types.py
--rw-r--r--   0        0        0     2095 2023-04-27 19:56:11.467503 easqlite-1.0.0/src/easqlite/_util.py
--rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-1.0.0/src/easqlite/py.typed
--rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-1.0.0/test/__init__.py
--rw-r--r--   0        0        0     4694 2023-04-27 19:29:49.186558 easqlite-1.0.0/test/test_simple.py
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 easqlite-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-04-26 22:47:07.420958 easqlite-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-26 22:47:07.420958 easqlite-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4128 2023-04-27 22:31:45.837592 easqlite-1.1.0/README.md
+-rwxr-xr-x   0        0        0      384 2023-04-27 18:05:33.250996 easqlite-1.1.0/justfile
+-rw-r--r--   0        0        0      736 2023-04-27 22:35:01.776050 easqlite-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-04-27 18:05:13.116642 easqlite-1.1.0/src/easqlite/__init__.py
+-rw-r--r--   0        0        0     4567 2023-04-27 22:16:19.666249 easqlite-1.1.0/src/easqlite/_blob.py
+-rw-r--r--   0        0        0    12015 2023-04-27 22:25:56.070419 easqlite-1.1.0/src/easqlite/_connection.py
+-rw-r--r--   0        0        0     5910 2023-04-27 22:16:24.010325 easqlite-1.1.0/src/easqlite/_cursor.py
+-rw-r--r--   0        0        0      884 2023-04-27 18:40:07.993622 easqlite-1.1.0/src/easqlite/_global.py
+-rw-r--r--   0        0        0      253 2023-04-27 17:36:22.830218 easqlite-1.1.0/src/easqlite/_types.py
+-rw-r--r--   0        0        0     2095 2023-04-27 19:56:11.467503 easqlite-1.1.0/src/easqlite/_util.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:34:03.975286 easqlite-1.1.0/src/easqlite/py.typed
+-rw-r--r--   0        0        0        0 2023-04-27 16:31:02.954545 easqlite-1.1.0/test/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-27 22:20:45.085930 easqlite-1.1.0/test/test_simple.py
+-rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 easqlite-1.1.0/PKG-INFO
```

### Comparing `easqlite-1.0.0/.gitignore` & `easqlite-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easqlite-1.0.0/LICENSE` & `easqlite-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easqlite-1.0.0/pyproject.toml` & `easqlite-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'easqlite'
-version = '1.0.0'
+version = '1.1.0'
 readme = 'README.md'
 license = {text = 'MIT'}
 description = "An executor-based async sqlite wrapper"
 keywords = ['asyncio', 'sqlite']
 requires-python = ">=3.8"
 
 classifiers = [
```

### Comparing `easqlite-1.0.0/src/easqlite/_blob.py` & `easqlite-1.1.0/src/easqlite/_blob.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,33 @@
             self.__readonly = readonly
             self.__name = name
             self.__setitems: deque[Coroutine[None, None, None]] = deque()
 
             # Lock for opening and closing.
             self.__lock = Lock()
 
-        async def _open(self) -> None:
+        async def __open(self) -> None:
             async with self.__lock:
                 if not self.__opened:
-                    await self.__connection._open()
                     self.__blob = await self.__connection._exec(
                         self.__connection._connection.blobopen,
                         self.__table,
                         self.__column,
                         self.__row,
                         readonly=self.__readonly,
                         name=self.__name,
                     )
                     self.__opened = True
 
-        def __await__(self) -> Generator[Any, Any, 'Blob']:
-            yield from self._open().__await__()
+        def __await__(self) -> Generator[None, None, 'Blob']:
+            yield from self.__open().__await__()
             return self
 
         async def __aenter__(self) -> 'Blob':
-            await self._open()
-            return self
+            return await self
 
         async def __aexit__(
             self,
             exc_type: Optional[Type[BaseException]],
             exc: Optional[BaseException],
             traceback: Optional[TracebackType],
         ) -> None:
@@ -99,15 +97,14 @@
             return await self.__connection._exec(self.__blob.tell)
 
         async def seek(self, offset: int, origin: int = 0) -> None:
             await self.flush()
             await self.__connection._exec(self.__blob.seek, offset, origin)
 
         async def flush(self) -> None:
-            await self._open()
             while self.__setitems:
                 await self.__setitems.popleft()
 
         async def __getitiem__(self, index: SupportsIndex | slice) -> int | bytes:
             await self.flush()
             return await self.__connection._exec(self.__blob.__getitem__, index)
```

### Comparing `easqlite-1.0.0/src/easqlite/_connection.py` & `easqlite-1.1.0/src/easqlite/_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         **kwargs: Any,
     ) -> ExecReturn:
         return await get_running_loop().run_in_executor(
             self._executor,
             partial(function, *args, **kwargs),
         )
 
-    async def _open(self) -> None:
+    async def __open(self) -> None:
         '''Open the connection if it's not opened.
         '''
         async with self.__lock:
             if not self.__opened:
                 if self.__executor_arg is None:
                     self._executor = ThreadPoolExecutor(max_workers=1)
                 else:
@@ -99,21 +99,20 @@
                     _close_in_executor,
                     self._executor,
                     self._connection,
                 )
 
                 self.__opened = True
 
-    def __await__(self) -> Generator[Any, Any, 'Connection']:
-        yield from self._open().__await__()
+    def __await__(self) -> Generator[None, None, 'Connection']:
+        yield from self.__open().__await__()
         return self
 
     async def __aenter__(self) -> 'Connection':
-        await self._open()
-        return self
+        return await self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
@@ -169,25 +168,25 @@
         await self._exec(self._connection.rollback)
 
     async def execute(
         self,
         sql: str,
         parameters: Iterable[Any] = (),
     ) -> '_cursor.Cursor':
-        return await self.cursor().execute(sql, parameters)
+        return await (await self.cursor()).execute(sql, parameters)
 
     async def executemany(
         self,
         sql: str,
         parameters: Iterable[Any],
     ) -> '_cursor.Cursor':
-        return await self.cursor().executemany(sql, parameters)
+        return await (await self.cursor()).executemany(sql, parameters)
 
     async def executescript(self, sql_script: str) -> '_cursor.Cursor':
-        return await self.cursor().executescript(sql_script)
+        return await (await self.cursor()).executescript(sql_script)
 
     if version_info >= (3, 8):
         async def create_function( # type: ignore
             self,
             name: str,
             narg: int,
             func: Callable[..., Optional[Any]],
```

### Comparing `easqlite-1.0.0/src/easqlite/_cursor.py` & `easqlite-1.1.0/src/easqlite/_cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,96 +44,85 @@
         self.__connection = connection
         self.__factory = factory
         self.__opened = False
 
         # Lock for opening and closing.
         self.__lock = Lock()
 
-    async def _open(self) -> None:
+    async def __open(self) -> None:
         async with self.__lock:
             if not self.__opened:
-                await self.__connection._open()
                 self.__cursor = await self.__connection._exec(
                     self.__connection._connection.cursor,
                     self.__factory,
                 )
                 self.__opened = True
 
     async def __aenter__(self) -> 'Cursor':
-        await self._open()
-        return self
+        return await self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         await self.close()
 
-    def __await__(self) -> Generator[Any, Any, 'Cursor']:
-        yield from self._open().__await__()
+    def __await__(self) -> Generator[None, None, 'Cursor']:
+        yield from self.__open().__await__()
         return self
 
     async def execute(self, sql: str, parameters: Iterable[Any] = ()) -> 'Cursor':
-        await self._open()
         await self.__connection._exec(self.__cursor.execute, sql, parameters)
         return self
 
     async def executemany(self, sql: str, parameters: Iterable[Any]) -> 'Cursor':
-        await self._open()
         await self.__connection._exec(self.__cursor.executemany, sql, parameters)
         return self
 
     async def executescript(self, sql_script: str) -> 'Cursor':
-        await self._open()
         await self.__connection._exec(self.__cursor.executescript, sql_script)
         return self
 
     async def close(self) -> None:
         async with self.__lock:
             if self.__opened:
                 try:
                     await self.__connection._exec(self.__cursor.close)
                 finally:
                     self.__opened = False
 
     async def fetchone(self) -> Any:
-        await self._open()
         return await self.__connection._exec(self.__cursor.fetchone)
 
     async def fetchmany(self, size: Optional[int] = None) -> List[Any]:
-        await self._open()
         if size is not None:
             return await self.__connection._exec(self.__cursor.fetchmany, size)
         else:
             return await self.__connection._exec(self.__cursor.fetchmany)
 
     async def fetchall(self) -> List[Any]:
-        await self._open()
         return await self.__connection._exec(self.__cursor.fetchall)
 
     async def setinputsizes(self, sizes: Any) -> None:
-        await self._open()
         await self.__connection._exec(self.__cursor.setinputsizes, sizes)
 
     async def setoutputsize(self, size: Any, column: Any = None) -> None:
-        await self._open()
         await self.__connection._exec(self.__cursor.setoutputsize, size, column)
 
     @overload
     async def arraysize(self) -> int:
         ...
 
     @overload
     async def arraysize(self, value: int) -> None:
         ...
 
     async def arraysize(self, value: Union[int, _Unset] = _unset) -> Optional[int]:
-        await self._open()
         if value is _unset:
             return await self.__connection._exec(
                 getattr,
                 self.__cursor,
                 'arraysize',
             )
         else:
@@ -147,31 +136,28 @@
     @property
     def connection(self) -> '_connection.Connection':
         return self.__connection
 
     async def description(
         self,
     ) -> Optional[Tuple[Tuple[str, None, None, None, None, None, None], ...]]:
-        await self._open()
         return await self.__connection._exec(
             getattr,
             self.__cursor,
             'description',
         )
 
     async def lastrowid(self) -> Optional[int]:
-        await self._open()
         return await self.__connection._exec(
             getattr,
             self.__cursor,
             'lastrowid',
         )
 
     async def rowcount(self) -> int:
-        await self._open()
         return await self.__connection._exec(
             getattr,
             self.__cursor,
             'rowcount',
         )
 
     @overload
@@ -182,15 +168,14 @@
     async def row_factory(self, value: Optional[RowFactory]) -> None:
         ...
             
     async def row_factory(
         self,
         value: Optional[Union[RowFactory, _Unset]] = _unset,
     ) -> Optional[RowFactory]:
-        await self._open()
         if value is _unset:
             return await self.__connection._exec(
                 getattr,
                 self.__cursor,
                 'row_factory',
         )
         else:
@@ -201,15 +186,14 @@
                 value,
         )
 
     def __aiter__(self) -> 'Cursor':
         return self
 
     async def __anext__(self) -> Any:
-        await self._open()
         # We need this because coroutines are not allowed to throw StopIteration
         # at all.  They get converted to RuntimeError.
         item = await self.__connection._exec(
             _next,
             self.__cursor,
         )
         if item is _raised_stop_iteration:
```

### Comparing `easqlite-1.0.0/src/easqlite/_global.py` & `easqlite-1.1.0/src/easqlite/_global.py`

 * *Files identical despite different names*

### Comparing `easqlite-1.0.0/src/easqlite/_util.py` & `easqlite-1.1.0/src/easqlite/_util.py`

 * *Files identical despite different names*

### Comparing `easqlite-1.0.0/test/test_simple.py` & `easqlite-1.1.0/test/test_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import easqlite
 import tempfile
 from pathlib import Path
 
 class SimpleTests(unittest.IsolatedAsyncioTestCase):
     async def test_some_queries(self):
         with tempfile.TemporaryDirectory() as dir:
-            Path(dir) / "test.db"
             async with easqlite.connect(
                 Path(dir) / "test.db",
                 isolation_level=None,
             ) as connection:
                 await connection.execute('''
                     CREATE TABLE foo (
                         id INTEGER PRIMARY KEY NOT NULL,
```

