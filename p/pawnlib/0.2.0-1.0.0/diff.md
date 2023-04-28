# Comparing `tmp/pawnlib-0.2.0-py3-none-any.whl.zip` & `tmp/pawnlib-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 108324 bytes, number of entries: 48
+Zip file size: 108326 bytes, number of entries: 48
 -rw-r--r--  2.0 unx     1188 b- defN 23-Jan-31 08:49 pawnlib/__init__.py
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jan-31 08:49 pawnlib/__main__.py
--rw-r--r--  2.0 unx      296 b- defN 23-Apr-28 03:08 pawnlib/__version__.py
+-rw-r--r--  2.0 unx      296 b- defN 23-Apr-28 03:15 pawnlib/__version__.py
 -rw-r--r--  2.0 unx       19 b- defN 22-Jul-21 06:00 pawnlib/asyncio/__init__.py
 -rw-r--r--  2.0 unx     4261 b- defN 23-Feb-22 08:29 pawnlib/asyncio/run.py
 -rw-r--r--  2.0 unx       36 b- defN 22-Jul-28 01:54 pawnlib/builder/__init__.py
 -rw-r--r--  2.0 unx     5382 b- defN 23-Jan-31 06:30 pawnlib/builder/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:35 pawnlib/builder/templates/__init__.py
 -rw-r--r--  2.0 unx     2343 b- defN 23-Feb-16 09:40 pawnlib/builder/templates/app_with_logging.tmpl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-28 04:34 pawnlib/cli/__init__.py
@@ -33,18 +33,18 @@
 -rw-r--r--  2.0 unx     9094 b- defN 23-Apr-26 05:18 pawnlib/typing/check.py
 -rw-r--r--  2.0 unx      823 b- defN 23-Apr-18 05:35 pawnlib/typing/constants.py
 -rw-r--r--  2.0 unx    59328 b- defN 23-Apr-28 01:05 pawnlib/typing/converter.py
 -rw-r--r--  2.0 unx     7137 b- defN 23-Jan-31 09:13 pawnlib/typing/date_utils.py
 -rw-r--r--  2.0 unx     3365 b- defN 23-Apr-18 05:35 pawnlib/typing/defines.py
 -rw-r--r--  2.0 unx    12711 b- defN 23-Jan-31 06:35 pawnlib/typing/generator.py
 -rw-r--r--  2.0 unx      552 b- defN 23-Apr-18 05:35 pawnlib/utils/__init__.py
--rw-r--r--  2.0 unx    48448 b- defN 23-Apr-28 03:06 pawnlib/utils/http.py
+-rw-r--r--  2.0 unx    48447 b- defN 23-Apr-28 03:15 pawnlib/utils/http.py
 -rw-r--r--  2.0 unx    25587 b- defN 23-Apr-28 03:07 pawnlib/utils/icx_signer.py
 -rw-r--r--  2.0 unx    12172 b- defN 23-Jan-31 05:22 pawnlib/utils/log.py
 -rw-r--r--  2.0 unx     7014 b- defN 23-Apr-18 05:35 pawnlib/utils/notify.py
 -rw-r--r--  2.0 unx    23248 b- defN 23-Apr-18 05:35 pawnlib/utils/operate_handler.py
--rw-r--r--  2.0 unx     5131 b- defN 23-Apr-28 03:09 pawnlib-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 03:09 pawnlib-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Apr-28 03:09 pawnlib-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 03:09 pawnlib-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3917 b- defN 23-Apr-28 03:09 pawnlib-0.2.0.dist-info/RECORD
-48 files, 390917 bytes uncompressed, 102156 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx     5131 b- defN 23-Apr-28 03:15 pawnlib-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 03:15 pawnlib-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Apr-28 03:15 pawnlib-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 03:15 pawnlib-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Apr-28 03:15 pawnlib-1.0.0.dist-info/RECORD
+48 files, 390916 bytes uncompressed, 102158 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -123,23 +123,23 @@
 
 Filename: pawnlib/utils/notify.py
 Comment: 
 
 Filename: pawnlib/utils/operate_handler.py
 Comment: 
 
-Filename: pawnlib-0.2.0.dist-info/METADATA
+Filename: pawnlib-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pawnlib-0.2.0.dist-info/WHEEL
+Filename: pawnlib-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pawnlib-0.2.0.dist-info/entry_points.txt
+Filename: pawnlib-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pawnlib-0.2.0.dist-info/top_level.txt
+Filename: pawnlib-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pawnlib-0.2.0.dist-info/RECORD
+Filename: pawnlib-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pawnlib/__version__.py

```diff
@@ -1,9 +1,9 @@
 ####
 __title__ = 'pawnlib'
 __description__ = 'pawnlib is a collection of libraries for IaC.'
 __url__ = 'https://github.com/jinwoo-j/pawnlib'
-__version__ = '0.2.0'
+__version__ = '1.0.0'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@parametacorp.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022 JINWOO'
```

## pawnlib/utils/http.py

```diff
@@ -385,15 +385,15 @@
         return {}
 
     def get_required_params(self):
         return self._params
 
 
 class IconRpcHelper:
-    def __init__(self, url="", wallet=None, network_info: NetworkInfo = None, raise_on_failure=False):
+    def __init__(self, url="", wallet=None, network_info: NetworkInfo = None, raise_on_failure=True):
         self.wallet = wallet
         self.governance_address = None
         self.request_payload = None
         self.response = None
         self.network_info = network_info
         self.raise_on_failure = raise_on_failure
```

## Comparing `pawnlib-0.2.0.dist-info/METADATA` & `pawnlib-1.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 0.2.0
+Version: 1.0.0
 Summary: pawnlib is a collection of libraries for IaC.
 Home-page: https://github.com/jinwoo-j/pawnlib
 Author: Jinwoo Jeong
 Author-email: jinwoo@parametacorp.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `pawnlib-0.2.0.dist-info/RECORD` & `pawnlib-1.0.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pawnlib/__init__.py,sha256=FXDHsJ3zZkGKwHLxXvy0z-DLH9UwQvGh7SoLiigPptw,1188
 pawnlib/__main__.py,sha256=wmMMh9f5l39HY6p_IfARRZwRDcK1rnfENZdCb9tzJYg,1224
-pawnlib/__version__.py,sha256=Fhln7WMC7iu8zoe2cgzYWbZ7_4TycU4R0EjJ1dMOfNI,296
+pawnlib/__version__.py,sha256=CTLSLrr8p0Up6nKvJQ_gR3PeqHbjKVa2jc2AFp5UG2U,296
 pawnlib/asyncio/__init__.py,sha256=ToWEND0eBP0YeJw4xZaBPLgQ-BGSeIvIApyysQMCsgo,19
 pawnlib/asyncio/run.py,sha256=WnZ8JWa5hnntds4wItvPtYy7HbJ7fLMvHbP04uXi05o,4261
 pawnlib/builder/__init__.py,sha256=2uuVV8xTTPsD8SCN1PDLhAcKOKISEZLQCQgOeritMrE,36
 pawnlib/builder/generator.py,sha256=4nsaQvZpzaLpIYLovIqmofBmyItj6nApae9zFdmvIuQ,5382
 pawnlib/builder/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pawnlib/builder/templates/app_with_logging.tmpl,sha256=UpxeQgys681Q1B-mADpEpRaG47RccWwwsdKigHL-ECU,2343
 pawnlib/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -32,17 +32,17 @@
 pawnlib/typing/check.py,sha256=GTYRaQ1ubMYTEiKa1463SWub_oitBjSFFltnOCDdRvg,9094
 pawnlib/typing/constants.py,sha256=9mbzRKWZw9p2ByzWairAT1zZv-qgd_7WVOEIVwUbX_0,823
 pawnlib/typing/converter.py,sha256=9E3nM8e40Fi5Qb0vdVc5FwzcH-wfX8VabD_djHArF1k,59328
 pawnlib/typing/date_utils.py,sha256=nNpliOVgREsQiBlynoqI26jWIc8NdZ7QaXjNmXGCj0U,7137
 pawnlib/typing/defines.py,sha256=V3NbriLXzb0iEKitUv47VoHtGhEOvwCg4krt9Y_qmnc,3365
 pawnlib/typing/generator.py,sha256=tAzkL5hJt0le958oYkVjTMbRGmlOwP3gE7mZaD-yXJY,12711
 pawnlib/utils/__init__.py,sha256=nO-vGtRB4UIImOLlJO-gN7SWoXYLcXqfc3LLyoCEAxM,552
-pawnlib/utils/http.py,sha256=J30cG7FlCT0DcFTtUKtRlptu0KnjEWXHQfqaOHwNKkY,48448
+pawnlib/utils/http.py,sha256=V3zEkcqofccMP6KNyvetYlzJw81jTrjRbhhON6JxYko,48447
 pawnlib/utils/icx_signer.py,sha256=ELnAB98vI7JOvDKlVWSlT5mqCy5tRvLDysk0EIRmlBw,25587
 pawnlib/utils/log.py,sha256=zYClSlvFJt9ZxZpApWvFZ7EcFRFtwUIyCyrtmUdfiLI,12172
 pawnlib/utils/notify.py,sha256=MybDFmnnwMm2AYp9pHmKatFnPO1IGpw65ZWF2MTcYds,7014
 pawnlib/utils/operate_handler.py,sha256=LMf41828PACtmmxnkR_zz0VD7s8F--Cqcdl9Efk4hV0,23248
-pawnlib-0.2.0.dist-info/METADATA,sha256=d3Q421DCA-95elO-cGr5CnZSdSPXKy07BU-LRel1U3w,5131
-pawnlib-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pawnlib-0.2.0.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
-pawnlib-0.2.0.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
-pawnlib-0.2.0.dist-info/RECORD,,
+pawnlib-1.0.0.dist-info/METADATA,sha256=U6kKu-oREpAXECclYGd44GkHnRcsM9qlVIT-xIX6co4,5131
+pawnlib-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pawnlib-1.0.0.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
+pawnlib-1.0.0.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
+pawnlib-1.0.0.dist-info/RECORD,,
```

