# Comparing `tmp/msg2bytes-0.1.2.tar.gz` & `tmp/msg2bytes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg2bytes-0.1.2.tar", last modified: Thu Apr 27 15:25:39 2023, max compression
+gzip compressed data, was "msg2bytes-0.1.3.tar", last modified: Fri Apr 28 11:50:55 2023, max compression
```

## Comparing `msg2bytes-0.1.2.tar` & `msg2bytes-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-27 15:25:39.273616 msg2bytes-0.1.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-26 05:03:42.000000 msg2bytes-0.1.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      167 2023-04-26 05:03:46.000000 msg2bytes-0.1.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2142 2023-04-27 15:25:39.273500 msg2bytes-0.1.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1443 2023-04-27 14:52:54.000000 msg2bytes-0.1.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-27 15:25:39.272661 msg2bytes-0.1.2/msg2bytes/
--rw-r--r--   0 test       (501) staff       (20)       20 2023-04-26 04:58:02.000000 msg2bytes-0.1.2/msg2bytes/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    33137 2023-04-27 14:52:22.000000 msg2bytes-0.1.2/msg2bytes/core.py
--rw-r--r--   0 test       (501) staff       (20)     7082 2023-04-27 01:35:43.000000 msg2bytes-0.1.2/msg2bytes/tests.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-27 15:25:39.273317 msg2bytes-0.1.2/msg2bytes.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2142 2023-04-27 15:25:39.000000 msg2bytes-0.1.2/msg2bytes.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      310 2023-04-27 15:25:39.000000 msg2bytes-0.1.2/msg2bytes.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-27 15:25:39.000000 msg2bytes-0.1.2/msg2bytes.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-27 15:25:38.000000 msg2bytes-0.1.2/msg2bytes.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       16 2023-04-27 15:25:39.000000 msg2bytes-0.1.2/msg2bytes.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       10 2023-04-27 15:25:39.000000 msg2bytes-0.1.2/msg2bytes.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       15 2023-04-26 05:04:22.000000 msg2bytes-0.1.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-04-27 15:25:39.273651 msg2bytes-0.1.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1395 2023-04-27 14:52:56.000000 msg2bytes-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.678440 msg2bytes-0.1.3/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-26 05:03:42.000000 msg2bytes-0.1.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      167 2023-04-26 05:03:46.000000 msg2bytes-0.1.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2984 2023-04-28 11:50:55.678324 msg2bytes-0.1.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     2286 2023-04-28 11:46:21.000000 msg2bytes-0.1.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.677471 msg2bytes-0.1.3/msg2bytes/
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-04-26 04:58:02.000000 msg2bytes-0.1.3/msg2bytes/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    35495 2023-04-28 04:25:50.000000 msg2bytes-0.1.3/msg2bytes/core.py
+-rw-r--r--   0 test       (501) staff       (20)     7756 2023-04-28 04:25:07.000000 msg2bytes-0.1.3/msg2bytes/tests.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-28 11:50:55.678144 msg2bytes-0.1.3/msg2bytes.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2984 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      310 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       16 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       10 2023-04-28 11:50:55.000000 msg2bytes-0.1.3/msg2bytes.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       15 2023-04-26 05:04:22.000000 msg2bytes-0.1.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-28 11:50:55.678473 msg2bytes-0.1.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1395 2023-04-28 04:26:27.000000 msg2bytes-0.1.3/setup.py
```

### Comparing `msg2bytes-0.1.2/LICENSE` & `msg2bytes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msg2bytes-0.1.2/msg2bytes/core.py` & `msg2bytes-0.1.3/msg2bytes/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import sys
+import uuid
 import struct
 import datetime
 import binascii
 import tempfile
 from io import BytesIO
 from decimal import Decimal
-import uuid
 
 from dateutil.parser import parse as datetime_parse
 
 __all__ = [
     "LIST",
     "SET",
     "TUPLE",
@@ -19,14 +19,16 @@
     "BOOLEAN",
     "TRUE",
     "FALSE",
     "STR",
     "BYTES",
     "DATETIME",
     "DECIMAL",
+    "DATE",
+    "TIME",
     "INT",
     "INT8",
     "INT16",
     "INT32",
     "INT64",
     "UINT8",
     "UINT16",
@@ -60,14 +62,16 @@
     "SetCodec",
     "TupleCodec",
     "DictCodec",
     "BooleanCodec",
     "TrueCodec",
     "FalseCodec",
     "DatetimeCodec",
+    "DateCodec",
+    "TimeCodec",
     "DecimalCodec",
     "FileCodec",
     "Int8Codec",
     "Int16Codec",
     "Int32Codec",
     "Int64Codec",
     "Uint8Codec",
@@ -75,16 +79,17 @@
     "Uint32Codec",
     "Uint64Codec",
     "BigIntCodec",
     "IntCodec",
     "DoubleCodec",
     "BigFloatCodec",
     "FloatCodec",
-    "NoCodecFound",
-    "CodecLoadFinished",
+    "NoDumpCodecFound",
+    "NoLoadCodecFound",
+    "CodecReadFailed",
     "register_codec",
     "register_dump_codec",
     "register_load_codec",
     "get_dump_codec",
     "get_load_codec",
     "msg2bytes_dump",
     "msg2bytes_load",
@@ -120,14 +125,16 @@
 FALSE = bytes([8])
 
 STR = bytes([9])
 BYTES = bytes([10])
 DATETIME = bytes([11])
 DECIMAL = bytes([12])
 FILE = bytes([13])
+DATE = bytes([14])  # v0.1.3引入
+TIME = bytes([15])  # v0.1.3引入
 
 INT = bytes([20])  # 抽象类型。实际不会使用的编码code。
 INT8 = bytes([21])
 INT16 = bytes([22])
 INT32 = bytes([23])
 INT64 = bytes([24])
 UINT8 = bytes([25])
@@ -653,14 +660,80 @@
     @classmethod
     async def async_load(cls, rfile, **kwargs):
         size = await async_read_size(rfile)
         data = await rfile.read(size)
         return datetime_parse(data)
 
 
+class DateCodec(Msg2bytesCodec):
+    type = datetime.date
+    code = DATE
+
+    @classmethod
+    def dump(cls, data, wfile, **kwargs):
+        encoding = cls.get_encoding(**kwargs)
+        data = data.isoformat().encode(encoding)
+        wfile.write(cls.code)
+        write_size(len(data), wfile)
+        wfile.write(data)
+
+    @classmethod
+    def load(cls, rfile, **kwargs):
+        size = read_size(rfile)
+        data = rfile.read(size)
+        return datetime_parse(data).date()
+
+    @classmethod
+    async def async_dump(cls, data, wfile, **kwargs):
+        encoding = cls.get_encoding(**kwargs)
+        data = data.isoformat().encode(encoding)
+        await wfile.write(cls.code)
+        await async_write_size(len(data), wfile)
+        await wfile.write(data)
+
+    @classmethod
+    async def async_load(cls, rfile, **kwargs):
+        size = await async_read_size(rfile)
+        data = await rfile.read(size)
+        return datetime_parse(data).date()
+
+
+class TimeCodec(Msg2bytesCodec):
+    type = datetime.time
+    code = TIME
+
+    @classmethod
+    def dump(cls, data, wfile, **kwargs):
+        encoding = cls.get_encoding(**kwargs)
+        data = data.isoformat().encode(encoding)
+        wfile.write(cls.code)
+        write_size(len(data), wfile)
+        wfile.write(data)
+
+    @classmethod
+    def load(cls, rfile, **kwargs):
+        size = read_size(rfile)
+        data = rfile.read(size)
+        return datetime_parse(data).time()
+
+    @classmethod
+    async def async_dump(cls, data, wfile, **kwargs):
+        encoding = cls.get_encoding(**kwargs)
+        data = data.isoformat().encode(encoding)
+        await wfile.write(cls.code)
+        await async_write_size(len(data), wfile)
+        await wfile.write(data)
+
+    @classmethod
+    async def async_load(cls, rfile, **kwargs):
+        size = await async_read_size(rfile)
+        data = await rfile.read(size)
+        return datetime_parse(data).time()
+
+
 class DecimalCodec(Msg2bytesCodec):
     type = Decimal
     code = DECIMAL
 
     @classmethod
     def dump(cls, data, wfile, **kwargs):
         encoding = cls.get_encoding(**kwargs)
@@ -1130,19 +1203,29 @@
 class __NoCodec(object):
     pass
 
 
 _NoCodec = __NoCodec()
 
 
-class NoCodecFound(RuntimeError):
+class NoDumpCodecFound(RuntimeError):
+    """没有相应数据类型的编码器。"""
+
+    pass
+
+
+class NoLoadCodecFound(RuntimeError):
+    """没有相应数据类型的解码器。"""
+
     pass
 
 
-class CodecLoadFinished(RuntimeError):
+class CodecReadFailed(RuntimeError):
+    """读取数据内容失败。"""
+
     pass
 
 
 _msg2bytes_dump_codecs = {}
 _msg2bytes_load_codecs = {}
 
 
@@ -1178,14 +1261,16 @@
 register_codec(TupleCodec)
 register_codec(DictCodec)
 
 register_codec(StrCodec)
 register_codec(BytesCodec)
 register_codec(DatetimeCodec)
 register_codec(DecimalCodec)
+register_codec(DateCodec)  # v0.1.3引入
+register_codec(TimeCodec)  # v0.1.3引入
 
 register_codec(TrueCodec)
 register_codec(FalseCodec)
 register_codec(BooleanCodec)  # 必须要在所有bool类型编解码器后注册
 
 register_codec(Int8Codec)
 register_codec(Int16Codec)
@@ -1207,37 +1292,37 @@
 
 
 def msg2bytes_dump(value, wfile, **kwargs):
     codec = get_dump_codec(value)
     if codec != _NoCodec:
         codec.dump(value, wfile, **kwargs)
     else:
-        raise NoCodecFound("no codec found for type: {}".format(type(value)))
+        raise NoDumpCodecFound("no codec found for type: {}".format(type(value)))
 
 
 def msg2bytes_load(rfile, **kwargs):
     code = rfile.read(1)
     if not code:
-        raise CodecLoadFinished()
+        raise CodecReadFailed()
     codec = get_load_codec(code)
     if codec != _NoCodec:
         return codec.load(rfile, **kwargs)
     else:
-        raise NoCodecFound(
+        raise NoLoadCodecFound(
             "no codec found for code: 0x{}".format(binascii.hexlify(code))
         )
 
 
 def msg2bytes_load_all(rfile, **kwargs):
     data = []
     while True:
         try:
             item = msg2bytes_load(rfile, **kwargs)
             data.append(item)
-        except CodecLoadFinished:
+        except CodecReadFailed:
             break
     if len(data) == 1:
         return data[0]
     else:
         return data
 
 
@@ -1253,37 +1338,37 @@
 
 
 async def msg2bytes_async_dump(value, wfile, **kwargs):
     codec = get_dump_codec(value)
     if codec != _NoCodec:
         await codec.async_dump(value, wfile, **kwargs)
     else:
-        raise NoCodecFound("no codec found for type: {}".format(type(value)))
+        raise NoDumpCodecFound("no codec found for type: {}".format(type(value)))
 
 
 async def msg2bytes_async_load(rfile, **kwargs):
     code = await rfile.read(1)
     if not code:
-        raise CodecLoadFinished()
+        raise CodecReadFailed()
     codec = get_load_codec(code)
     if codec != _NoCodec:
         return await codec.async_load(rfile, **kwargs)
     else:
-        raise NoCodecFound(
+        raise NoLoadCodecFound(
             "no codec found for code: 0x{}".format(binascii.hexlify(code))
         )
 
 
 async def msg2bytes_async_load_all(rfile, **kwargs):
     data = []
     while True:
         try:
             item = await msg2bytes_async_load(rfile, **kwargs)
             data.append(item)
-        except CodecLoadFinished:
+        except CodecReadFailed:
             break
     if len(data) == 1:
         return data[0]
     else:
         return data
```

### Comparing `msg2bytes-0.1.2/msg2bytes/tests.py` & `msg2bytes-0.1.3/msg2bytes/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
-import random
 import os
+import random
+import datetime
 
 from unittest import TestCase
 import msg2bytes
 
 
 class TestMsg2bytes(TestCase):
     def test1(self):
@@ -225,15 +226,15 @@
         assert data1 == data3
 
     def test36(self):
         class A(object):
             pass
 
         data1 = A()
-        with self.assertRaises(msg2bytes.NoCodecFound):
+        with self.assertRaises(msg2bytes.NoDumpCodecFound):
             data2 = msg2bytes.dumps(data1)
             data3 = msg2bytes.loads(data2)
 
     def test37(self):
         data1 = os.urandom(1024)
         file1 = msg2bytes.File()
         with open(file1.filepath, "wb") as fobj:
@@ -248,7 +249,30 @@
             file1content = fobj.read()
         with open(file1.filepath, "rb") as fobj:
             file2content = fobj.read()
         assert file1content == file2content
 
         os.unlink(file1.filepath)
         os.unlink(file2.filepath)
+
+    def test38(self):
+        data1 = datetime.datetime.now().date()
+        data2 = msg2bytes.dumps(data1)
+        data3 = msg2bytes.loads(data2)
+        assert data1 == data3
+
+    def test39(self):
+        data1 = datetime.datetime.now().time()
+        data2 = msg2bytes.dumps(data1)
+        data3 = msg2bytes.loads(data2)
+        assert data1 == data3
+
+    def test40(self):
+        today = datetime.datetime.now()
+        data1 = {
+            "datetime": today,
+            "date": today.date(),
+            "time": today.time(),
+        }
+        data2 = msg2bytes.dumps(data1)
+        data3 = msg2bytes.loads(data2)
+        assert data1 == data3
```

### Comparing `msg2bytes-0.1.2/setup.py` & `msg2bytes-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="msg2bytes",
-    version="0.1.2",
+    version="0.1.3",
     description="MessageToBytes(msg2bytes) is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
```

