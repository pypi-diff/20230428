# Comparing `tmp/pawnlib-1.0.1-py3-none-any.whl.zip` & `tmp/pawnlib-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 108344 bytes, number of entries: 48
+Zip file size: 108525 bytes, number of entries: 48
 -rw-r--r--  2.0 unx     1188 b- defN 23-Jan-31 08:49 pawnlib/__init__.py
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jan-31 08:49 pawnlib/__main__.py
--rw-r--r--  2.0 unx      296 b- defN 23-Apr-28 03:34 pawnlib/__version__.py
+-rw-r--r--  2.0 unx      296 b- defN 23-Apr-28 05:02 pawnlib/__version__.py
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
--rw-r--r--  2.0 unx    48645 b- defN 23-Apr-28 03:34 pawnlib/utils/http.py
+-rw-r--r--  2.0 unx    49618 b- defN 23-Apr-28 05:01 pawnlib/utils/http.py
 -rw-r--r--  2.0 unx    25587 b- defN 23-Apr-28 03:07 pawnlib/utils/icx_signer.py
 -rw-r--r--  2.0 unx    12172 b- defN 23-Jan-31 05:22 pawnlib/utils/log.py
 -rw-r--r--  2.0 unx     7014 b- defN 23-Apr-18 05:35 pawnlib/utils/notify.py
 -rw-r--r--  2.0 unx    23248 b- defN 23-Apr-18 05:35 pawnlib/utils/operate_handler.py
--rw-r--r--  2.0 unx     5131 b- defN 23-Apr-28 03:34 pawnlib-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 03:34 pawnlib-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Apr-28 03:34 pawnlib-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 03:34 pawnlib-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3917 b- defN 23-Apr-28 03:34 pawnlib-1.0.1.dist-info/RECORD
-48 files, 391114 bytes uncompressed, 102176 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx     5131 b- defN 23-Apr-28 05:02 pawnlib-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 05:02 pawnlib-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Apr-28 05:02 pawnlib-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 05:02 pawnlib-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Apr-28 05:02 pawnlib-1.0.2.dist-info/RECORD
+48 files, 392087 bytes uncompressed, 102357 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -123,23 +123,23 @@
 
 Filename: pawnlib/utils/notify.py
 Comment: 
 
 Filename: pawnlib/utils/operate_handler.py
 Comment: 
 
-Filename: pawnlib-1.0.1.dist-info/METADATA
+Filename: pawnlib-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pawnlib-1.0.1.dist-info/WHEEL
+Filename: pawnlib-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pawnlib-1.0.1.dist-info/entry_points.txt
+Filename: pawnlib-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pawnlib-1.0.1.dist-info/top_level.txt
+Filename: pawnlib-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pawnlib-1.0.1.dist-info/RECORD
+Filename: pawnlib-1.0.2.dist-info/RECORD
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
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@parametacorp.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022 JINWOO'
```

## pawnlib/utils/http.py

```diff
@@ -1,18 +1,17 @@
 import re
 import json
 import sys
 from pawnlib.config.globalconfig import pawnlib_config as pawn, global_verbose, pconf, SimpleNamespace
-from pawnlib.output import NoTraceBackException, dump, syntax_highlight, kvPrint, debug_logging
+from pawnlib.output import NoTraceBackException, dump, syntax_highlight, kvPrint, debug_logging, PrintRichTable
 from pawnlib.resource import net
 from pawnlib.typing.converter import append_suffix, append_prefix, hex_to_number, FlatDict, FlatterDict, flatten, const
 from pawnlib.typing.constants import const
 from pawnlib.typing.generator import json_rpc, random_token_address
 from pawnlib.typing.check import keys_exists, is_int, is_float, list_depth, is_valid_token_address
-
 try:
     from pawnlib.utils import icx_signer
 except ImportError:
     pass
 
 from typing import Union
 
@@ -580,14 +579,15 @@
         else:
             self._set_governance_address(method=method)
 
         self._can_be_signed = sign
         _request_payload = self._make_governance_payload(method, params)
 
         if self._can_be_signed:
+            # if _request_payload['params'].get('value', None):
             _request_payload['params']['value'] = "0x0"
             self.sign_tx(payload=_request_payload)
             response = self.sign_send(is_wait=is_wait)
             return response
         else:
             response = self.rpc_call(
                 url=url,
@@ -688,50 +688,73 @@
         if not tx_hash and isinstance(self.response, dict):
             if keys_exists(self.response, 'json', 'result', 'txHash'):
                 tx_hash = self.response['json']['result']['txHash']
             elif keys_exists(self.response, 'json', 'result'):
                 tx_hash = self.response['json']['result']
 
         if not tx_hash:
-            pawn.console.log(f"[red] Not found tx_hash='{tx_hash}', response={self.response}")
+            pawn.console.log(f"[red] Not found tx_hash='{tx_hash}'")
             return
-
+        tx_status_result = True
         pawn.console.log(f"Check a transaction by {tx_hash}")
         with pawn.console.status("[magenta] Wait for transaction to be generated.") as status:
             count = 0
             while True:
                 resp = self.get_tx(url=url, tx_hash=tx_hash)
                 exit_loop = False
                 prefix_text = f"[bold cyan][Wait TX][{count}][/bold cyan] "
                 if resp.get('error'):
                     exit_msg = ""
                     if "InvalidParams" in resp['error'].get('message'):
                         exit_loop = True
-                        exit_msg = f"[red][FAIL][/red]"
+                        exit_msg = "[red][FAIL][/red]"
                     text = f"{prefix_text}{exit_msg}[white] {resp['error']['message']}"
 
                 elif resp.get('result'):
                     if resp['result'].get('logsBloom'):
                         resp['result']['logsBloom'] = int(resp['result']['logsBloom'], 16)
 
+                    if resp['result'].get('failure'):
+                        _resp_status = "[FAIL]"
+                        tx_status_result = False
+                    else:
+                        _resp_status = "[OK]"
+
                     exit_loop = True
-                    text = f"{prefix_text}[OK] {json.dumps(resp['result'])}"
+                    text = f"{prefix_text}[red]{_resp_status}[red] {json.dumps(resp['result'])}"
                 else:
                     text = resp
                 status.update(
                     status=f"[bold red]{text}",
                     spinner_style="yellow",
                 )
                 if exit_loop:
                     pawn.console.log(f"[bold green][white] {text}")
                     break
                 count += 1
                 time.sleep(1)
+
+            if not tx_status_result and tx_hash:
+                print("*" * 10)
+                self.get_debug_trace(tx_hash)
         return resp
 
+    def get_debug_trace(self, tx_hash, print_table=True):
+        response = self.rpc_call(
+            url=self.debug_url,
+            method="debug_getTrace",
+            params={"txHash": tx_hash},
+            store_request_payload=False,
+        )
+        if isinstance(response, dict) and keys_exists(response, "result", "logs") and print_table:
+            PrintRichTable(f"debug_getTrace={tx_hash}", data=response['result']['logs'])
+        else:
+            pawn.console.log(response)
+        return response
+
     def auto_fill_parameter(self):
         if isinstance(self.request_payload, dict) and self.request_payload.get('params'):
             self.request_payload['params']['from'] = self.wallet.get('address')
 
             if not self.request_payload['params'].get('nonce'):
                 self.request_payload['params']['nonce'] = "0x1"
```

## Comparing `pawnlib-1.0.1.dist-info/METADATA` & `pawnlib-1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawnlib
-Version: 1.0.1
+Version: 1.0.2
 Summary: pawnlib is a collection of libraries for IaC.
 Home-page: https://github.com/jinwoo-j/pawnlib
 Author: Jinwoo Jeong
 Author-email: jinwoo@parametacorp.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `pawnlib-1.0.1.dist-info/RECORD` & `pawnlib-1.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pawnlib/__init__.py,sha256=FXDHsJ3zZkGKwHLxXvy0z-DLH9UwQvGh7SoLiigPptw,1188
 pawnlib/__main__.py,sha256=wmMMh9f5l39HY6p_IfARRZwRDcK1rnfENZdCb9tzJYg,1224
-pawnlib/__version__.py,sha256=_mDGYXVCk_455XSEn6LZPJ1V9C0nTrZQCWx8b0eLikw,296
+pawnlib/__version__.py,sha256=adFpVTFGmLIjLlckq0-by6b-KsTrQ1iCaroZZJsRbPg,296
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
-pawnlib/utils/http.py,sha256=bpmd7sWrKq-K-sa53g_VabX5bEniJe1iJjFcYUQ2kM8,48645
+pawnlib/utils/http.py,sha256=tt6fylx694jGimQWOdwe4y1rWGv1UEBWl8L-OAmruH8,49618
 pawnlib/utils/icx_signer.py,sha256=ELnAB98vI7JOvDKlVWSlT5mqCy5tRvLDysk0EIRmlBw,25587
 pawnlib/utils/log.py,sha256=zYClSlvFJt9ZxZpApWvFZ7EcFRFtwUIyCyrtmUdfiLI,12172
 pawnlib/utils/notify.py,sha256=MybDFmnnwMm2AYp9pHmKatFnPO1IGpw65ZWF2MTcYds,7014
 pawnlib/utils/operate_handler.py,sha256=LMf41828PACtmmxnkR_zz0VD7s8F--Cqcdl9Efk4hV0,23248
-pawnlib-1.0.1.dist-info/METADATA,sha256=SlSQDdy5UiEvHfoLzTW7kwrYSYIgi-cXDZmfDIT_Pmo,5131
-pawnlib-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pawnlib-1.0.1.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
-pawnlib-1.0.1.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
-pawnlib-1.0.1.dist-info/RECORD,,
+pawnlib-1.0.2.dist-info/METADATA,sha256=i9qkwwCAXY1d6d_RkQsjbP5-xsbBpWyi14z1CmJ9uhE,5131
+pawnlib-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pawnlib-1.0.2.dist-info/entry_points.txt,sha256=gfwAzqk-lzSb_VFiXmGg4Xn-8TUu_TMcM3QBjdyEAAE,52
+pawnlib-1.0.2.dist-info/top_level.txt,sha256=a6t_hQ3MagyRwwliF91xPgBk12g6a7O84C4GiY3fKQE,8
+pawnlib-1.0.2.dist-info/RECORD,,
```

