# Comparing `tmp/lk_logger-5.4.8-py3-none-any.whl.zip` & `tmp/lk_logger-5.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 33882 bytes, number of entries: 24
--rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
+Zip file size: 34029 bytes, number of entries: 24
+-rw-r--r--  2.0 unx      557 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 unx      649 b- defN 80-Jan-01 00:00 lk_logger/_print.py
 -rw-r--r--  2.0 unx     1716 b- defN 80-Jan-01 00:00 lk_logger/cache.py
 -rw-r--r--  2.0 unx     5366 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 lk_logger/control.py
--rw-r--r--  2.0 unx    10233 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 unx    10678 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 unx     4847 b- defN 80-Jan-01 00:00 lk_logger/markup.py
 -rw-r--r--  2.0 unx     5271 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 unx     7675 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
 -rw-r--r--  2.0 unx     6666 b- defN 80-Jan-01 00:00 lk_logger/sourcemap.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx     4899 b- defN 80-Jan-01 00:00 lk_logger-5.4.8.dist-info/METADATA
-?rw-r--r--  2.0 unx     1919 b- defN 16-Jan-01 00:00 lk_logger-5.4.8.dist-info/RECORD
-24 files, 104601 bytes uncompressed, 30816 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.4.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4899 b- defN 80-Jan-01 00:00 lk_logger-5.4.9.dist-info/METADATA
+?rw-r--r--  2.0 unx     1919 b- defN 16-Jan-01 00:00 lk_logger-5.4.9.dist-info/RECORD
+24 files, 105177 bytes uncompressed, 30963 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -57,17 +57,17 @@
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
 Filename: lk_logger/sourcemap.py
 Comment: 
 
-Filename: lk_logger-5.4.8.dist-info/WHEEL
+Filename: lk_logger-5.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.4.8.dist-info/METADATA
+Filename: lk_logger-5.4.9.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.4.8.dist-info/RECORD
+Filename: lk_logger-5.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -1,20 +1,23 @@
 from . import console
 from ._print import bprint
 from .control import disable
+from .control import disable as mute
 from .control import enable
+from .control import enable as unmute
 from .control import setup
 from .control import start_ipython
 from .control import unload
+from .control import unload as restore_builtin_print
 from .control import update
 from .logger import lk
 from .pipeline import pipeline
 
 
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.4.8'
+__version__ = '5.4.9'
```

## lk_logger/logger.py

```diff
@@ -92,14 +92,15 @@
                     msg, kwargs, custom_print = self._message_queue.popleft()
                     if custom_print:
                         custom_print(*msg, **kwargs)
                     else:
                         con_print(msg, **kwargs)
                 except Exception as e:
                     debug(e)
+                    # raise e
             else:
                 sleep(10E-3)
     
     def _stop_running(self):
         self._running = False
         if self._config.clear_unfinished_stream:
             self._message_queue.clear()
@@ -146,33 +147,43 @@
         """
         return: (str message, bool is_flush, bool is_drain)
             flush: print the message immediately.
             drain: drain the message queue.
                 if drain is True, the flush must be True.
         """
         frame_id = '{}:{}'.format(frame.f_code.co_filename, frame.f_lineno)
-        # frame_id = f'{id(frame)}#{frame.f_lineno}'
         args, markup_pos, markup = \
             self._extract_markup_from_arguments(frame_id, args)
         marks = self._analyser.extract(markup)
         marks_meaning = self._analyser.analyse(marks)
         
+        if marks['p']:
+            real_frame = frame
+            for _ in range(marks['p']):
+                real_frame = real_frame.f_back
+            frame_id = '{}:{}'.format(
+                real_frame.f_code.co_filename,
+                real_frame.f_lineno
+            )
+        # debug(frame_id)
+        
         flush_scheme: T.FlushScheme = 0
         if MarkMeaning.FLUSH in marks_meaning:
             flush_scheme = 1
         elif MarkMeaning.FLUSH_AND_DRAIN in marks_meaning:
             flush_scheme = 2
         elif MarkMeaning.WAIT_TO_FLUSH in marks_meaning:
             flush_scheme = 3
         
         # check cache
         if self._cache.is_cached(frame_id, markup):
             cached_info = self._cache.get_cache(frame_id, markup)
             return self._builder.compose(
-                args, marks_meaning, cached_info), flush_scheme
+                args, marks_meaning, cached_info
+            ), flush_scheme
         
         # ---------------------------------------------------------------------
         
         if MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
             return self._builder.quick_compose(args), flush_scheme
         elif MarkMeaning.RICH_OBJECT in marks_meaning:
             # assert len(args) == 1 and isinstance(args[1], rich.Renderable)
@@ -188,14 +199,16 @@
         
         show_source = self._config.show_source
         show_funcname = self._config.show_funcname
         show_varnames = self._config.show_varnames and \
                         MarkMeaning.MODERATE_PRUNE not in marks_meaning
         
         if any((show_source, show_funcname, show_varnames)):
+            # PERF: here does redundant work in tracing real frame. we need to
+            #   merge this with the above tracing.
             srcmap = sourcemap.get_sourcemap(
                 frame=frame,
                 traceback_level=marks['p'],
                 advanced=show_varnames,
             )
             
             if show_source:
```

## Comparing `lk_logger-5.4.8.dist-info/METADATA` & `lk_logger-5.4.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.4.8
+Version: 5.4.9
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.4.8.dist-info/RECORD` & `lk_logger-5.4.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-lk_logger/__init__.py,sha256=1k1PCrVX1dV2cCSEwhcnnokgUPup633HHijTwE1Hr68,426
+lk_logger/__init__.py,sha256=3qOTqZqhSl0hYc8MZ-ao12bt2qjLcWnwMFR-RWR6Jzs,557
 lk_logger/_print.py,sha256=gg_OC-kftX3Foo40-zXGVAjGIMttAdZZWF78YWgga9U,649
 lk_logger/cache.py,sha256=kqa-3p3S9oNkv3f6TWAQX_1clx-pJ_iFED7z8cjh1SM,1716
 lk_logger/config.py,sha256=l0bGytY-Imd4VJiE_S62OuTqZKcoVzt6fYucC2RcZhc,5366
 lk_logger/console.py,sha256=GSoFWXBybfNuF7S7b3_OJL70h52OSlTPnCbpay1pL60,1563
 lk_logger/control.py,sha256=Fk8o5aGjTAAxhJs6G1EvTUZ3ERvlQ13H-cpX_Mn5CSQ,4503
-lk_logger/logger.py,sha256=3l5op4eoQHWatZrNjg-uSgnZvNkoKME-7E1id8Dzdrc,10233
+lk_logger/logger.py,sha256=HwPBsJfx671t3U4HS0Nm9C0xHt7E9rKVxzUJIOl6450,10678
 lk_logger/markup.py,sha256=q9Z6N6NFNQ1jP4nbdE5FVHlhgHKvMR779Ir3MeZgOYg,4847
 lk_logger/message_builder.py,sha256=bZAxrtGdC22D4a2-ZdYREeuU18CrLldAgDkZQBg0KY4,5271
 lk_logger/message_formatter.py,sha256=uqL-qP5T7Eoo77CtokAKhdcTAxFfoQmW_Xeof6_kZ-w,7675
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
 lk_logger/pipeline.py,sha256=bo-Z9367i2TxxJOCS5_Rk_6CFccFyJYgp3-uw9q9LzQ,2559
 lk_logger/scanner/__init__.py,sha256=er6nQAKVaYpdk30878kEDo5vKTSa6CzR-CdxNJiaODo,71
 lk_logger/scanner/analyser.py,sha256=tbI48nDcBPthZoD8jlnpap7S6FIHs4u8pUMQpsmh6r4,6247
 lk_logger/scanner/const.py,sha256=pRfHUK2huF2oLkd-ZpGtGUKQ2T4K3EnlSI0pUGGnp6Q,1128
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=7Ase1WyHD87cBr4k9zYehe9LgL91r0L1_XlgKHg1_Eg,9594
 lk_logger/scanner/symbols.py,sha256=ibW1-n7Xigo9LvowUSn6dIrx-UmiJyuxN321bSCilSg,3238
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=Vr929B1w9UGiLVEMIJJIyE6gULjd_NxmNVpssyZW_JI,491
 lk_logger/sourcemap.py,sha256=bg0JC24cxGcxdxk-_46pOu_DDSucuBr3Q-NYol4vYNw,6666
-lk_logger-5.4.8.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-lk_logger-5.4.8.dist-info/METADATA,sha256=9jvYylgeRlXfD9QkfRBcYfHgQmuhd_gJV3xBbcvnb9M,4899
-lk_logger-5.4.8.dist-info/RECORD,,
+lk_logger-5.4.9.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+lk_logger-5.4.9.dist-info/METADATA,sha256=WFGoSL_eTQN6LLXNUnTMNE1fNeAtVFqnIL2mKG1atpQ,4899
+lk_logger-5.4.9.dist-info/RECORD,,
```

