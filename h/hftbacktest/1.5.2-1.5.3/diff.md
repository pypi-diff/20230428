# Comparing `tmp/hftbacktest-1.5.2.tar.gz` & `tmp/hftbacktest-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.5.2.tar", last modified: Sun Apr 16 13:59:13 2023, max compression
+gzip compressed data, was "hftbacktest-1.5.3.tar", last modified: Fri Apr 28 14:15:39 2023, max compression
```

## Comparing `hftbacktest-1.5.2.tar` & `hftbacktest-1.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1079 2022-11-14 13:24:06.000000 hftbacktest-1.5.2/LICENSE
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5763 2023-04-16 13:46:03.000000 hftbacktest-1.5.2/README.rst
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.750521 hftbacktest-1.5.2/hftbacktest/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    11501 2023-04-16 13:48:02.000000 hftbacktest-1.5.2/hftbacktest/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     1011 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/assettype.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    13846 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/backtest.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.754521 hftbacktest-1.5.2/hftbacktest/data/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1592 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/__init__.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/data/utils/
--rw-r--r--   0 kaz       (1000) kaz       (1000)       44 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)    11299 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     2160 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     6707 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)    11514 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/data/validation.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6194 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/marketdepth.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/models/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    10007 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/latencies.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     3305 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/models/queue.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     4143 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/order.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/hftbacktest/proc/
--rw-r--r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5866 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/local.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    14794 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/nopartialfillexchange.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    22145 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     5903 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/proc/proc.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     3252 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/reader.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    13631 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/stat.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     2149 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/state.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)      876 2023-04-16 12:29:54.000000 hftbacktest-1.5.2/hftbacktest/typing.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:59:13.754521 hftbacktest-1.5.2/hftbacktest.egg-info/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)      908 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/SOURCES.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/dependency_links.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-02-22 13:33:16.000000 hftbacktest-1.5.2/hftbacktest.egg-info/not-zip-safe
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       48 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/requires.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       12 2023-04-16 13:59:13.000000 hftbacktest-1.5.2/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1249 2023-04-16 13:59:13.758521 hftbacktest-1.5.2/setup.cfg
--rw-r--r--   0 kaz       (1000) kaz       (1000)       61 2023-02-22 13:27:55.000000 hftbacktest-1.5.2/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6895 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5786 2023-04-28 14:13:16.000000 hftbacktest-1.5.3/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-04-28 13:24:01.000000 hftbacktest-1.5.3/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.3/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.3/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.3/hftbacktest/data/validation.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10007 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4143 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5903 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13631 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-28 14:15:39.344537 hftbacktest-1.5.3/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6895 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      908 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-04-28 14:15:39.000000 hftbacktest-1.5.3/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-04-28 14:15:39.345537 hftbacktest-1.5.3/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.3/setup.py
```

### Comparing `hftbacktest-1.5.2/LICENSE` & `hftbacktest-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/PKG-INFO` & `hftbacktest-1.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.2
+Version: 1.5.3
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -40,14 +40,18 @@
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
+Documentation
+=============
+
+See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
 
@@ -81,86 +85,81 @@
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
         while hbt.run:
-            # Check every 0.1s
+            # Checks every 0.1s
             if not hbt.elapse(0.1 * 1e6):
                 return False
 
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-            # Obtain the current mid-price and compute the reservation price.
+            # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
             buy_order_price = reservation_price - half_spread
             sell_order_price = reservation_price + half_spread
 
             last_order_id = -1
             # Cancel all outstanding orders
             for order in hbt.orders.values():
                 if order.cancellable:
                     hbt.cancel(order.order_id)
                     last_order_id = order.order_id    
 			
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order cancellation responses is received.
+            # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
 	    last_order_id = -1
             if hbt.position < max_position:
-                # Submit a new post-only limit bid order.
+                # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             if hbt.position > -max_position:
-                # Submit a new post-only limit ask order.
+                # Submits a new post-only limit ask order.
                 order_id += 1
                 hbt.submit_sell_order(
                     order_id,
                     sell_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order responses is received.
+            # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
-            # Record the current state for stat calculation.
+            # Records the current state for stat calculation.
             stat.record(hbt)
         return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Documentation
-=============
-
-See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
-
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
     :alt: |Python Version
     :target: https://badge.fury.io/py/tensorflow
 
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
     :alt: |Codacy
```

### Comparing `hftbacktest-1.5.2/README.rst` & `hftbacktest-1.5.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
+Documentation
+=============
+
+See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
 
@@ -55,86 +59,81 @@
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
         while hbt.run:
-            # Check every 0.1s
+            # Checks every 0.1s
             if not hbt.elapse(0.1 * 1e6):
                 return False
 
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-            # Obtain the current mid-price and compute the reservation price.
+            # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
             buy_order_price = reservation_price - half_spread
             sell_order_price = reservation_price + half_spread
 
             last_order_id = -1
             # Cancel all outstanding orders
             for order in hbt.orders.values():
                 if order.cancellable:
                     hbt.cancel(order.order_id)
                     last_order_id = order.order_id    
 			
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order cancellation responses is received.
+            # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
 	    last_order_id = -1
             if hbt.position < max_position:
-                # Submit a new post-only limit bid order.
+                # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             if hbt.position > -max_position:
-                # Submit a new post-only limit ask order.
+                # Submits a new post-only limit ask order.
                 order_id += 1
                 hbt.submit_sell_order(
                     order_id,
                     sell_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order responses is received.
+            # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
-            # Record the current state for stat calculation.
+            # Records the current state for stat calculation.
             stat.record(hbt)
         return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Documentation
-=============
-
-See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
-
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
     :alt: |Python Version
     :target: https://badge.fury.io/py/tensorflow
 
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
     :alt: |Codacy
```

### Comparing `hftbacktest-1.5.2/hftbacktest/__init__.py` & `hftbacktest-1.5.3/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.5.2'
+__version__ = '1.5.3'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.5.2/hftbacktest/assettype.py` & `hftbacktest-1.5.3/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/backtest.py` & `hftbacktest-1.5.3/hftbacktest/backtest.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         r"""
         Places a buy order.
 
         Args:
             order_id: The unique order ID; there should not be any existing order with the same ID on both local and
                       exchange sides.
             price: Order price.
-            qty: Quantity to sell.
+            qty: Quantity to buy.
             time_in_force: Available Time-In-Force options vary depending on the exchange model. See to the exchange
                            model for details.
 
                            - ``GTX``: Post-only
                            - ``GTC``: Good 'till Cancel
                            - ``FOK``: Fill or Kill
                            - ``IOC``: Immediate or Cancel
@@ -299,17 +299,35 @@
         if timeout >= 0:
             timestamp = self.current_timestamp + timeout
         else:
             timestamp = UNTIL_END_OF_DATA
 
         return self.goto(timestamp, wait_order_response=order_id)
 
-    # todo: implement
-    # def wait_next_feed(self, include_order_resp, timeout=-1):
-    #     raise NotImplementedError
+    def wait_next_feed(self, include_order_resp: bool, timeout: int = -1):
+        """
+        Waits until the next feed is received.
+
+        Args:
+            include_order_resp: Whether to include order responses in the feed to wait for.
+            timeout: Maximum waiting time; The default value of `-1` indicates no timeout.
+
+        Returns:
+            ``True`` if the method reaches the specified timestamp within the data. If the end of the data is reached
+            before the specified timestamp, it returns ``False``.
+        """
+        if include_order_resp:
+            timestamp = self.local.next_timestamp()
+        else:
+            timestamp = self.local._next_data_timestamp()
+        if timestamp == -1:
+            return False
+        if timeout >= 0:
+            timestamp = min(timestamp, self.current_timestamp + timeout)
+        return self.goto(timestamp)
 
     def clear_inactive_orders(self):
         r"""
         Clear inactive(``CANCELED``, ``FILLED``, or ``EXPIRED``) orders from the local ``orders`` dictionary.
         """
         self.local.clear_inactive_orders()
 
@@ -365,16 +383,14 @@
         """
         found_order_resp_timestamp = False
         while True:
             # Select which side will be processed next.
             next_local_timestamp = self.local.next_timestamp()
             next_exch_timestamp = self.exch.next_timestamp()
 
-            # print(next_local_timestamp, next_exch_timestamp)
-
             # Local will be processed.
             if (0 < next_local_timestamp < next_exch_timestamp) \
                     or (next_local_timestamp > 0 >= next_exch_timestamp):
                 if next_local_timestamp > timestamp:
                     break
                 resp_timestamp = self.local.process(WAIT_ORDER_RESPONSE_NONE)
```

### Comparing `hftbacktest-1.5.2/hftbacktest/data/__init__.py` & `hftbacktest-1.5.3/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.5.3/hftbacktest/data/utils/binancefutures.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from .. import correct, validate_data
 
 
 def convert(
         input_filename: str,
         output_filename: Optional[str] = None,
         opt: Literal['', 'm', 't', 'mt'] = '',
-        base_latency: float = 0
+        base_latency: float = 0,
+        method: Literal['separate', 'adjust'] = 'separate'
 ) -> NDArray:
     r"""
     Converts raw Binance Futures feed stream file into a format compatible with HftBacktest.
 
     File Format:
 
     .. code-block::
@@ -47,14 +48,15 @@
              - ``t``: Processes ``bookTicker`` stream with the following custom event IDs.
 
                 - best bid: ``103``
                 - best ask: ``104``
 
         base_latency: The value to be added to the feed latency.
                       See :func:`.correct_local_timestamp`.
+        method: The method to correct reversed exchange timestamp events. See :func:`..validation.correct`.
     Returns:
         Converted data compatible with HftBacktest.
     """
     rows = []
     with gzip.open(input_filename, 'r') as f:
         while True:
             line = f.readline()
@@ -114,15 +116,15 @@
                 rows.append([3, exch_timestamp, local_timestamp, 1, bid_clear_upto, 0])
                 rows.append([3, exch_timestamp, local_timestamp, -1, ask_clear_upto, 0])
                 # insert the snapshot.
                 rows += [[4, exch_timestamp, local_timestamp, 1, float(bid[0]), float(bid[1])] for bid in bids]
                 rows += [[4, exch_timestamp, local_timestamp, -1, float(ask[0]), float(ask[1])] for ask in asks]
 
     data = np.asarray(rows, np.float64)
-    data = correct(data, base_latency=base_latency)
+    data = correct(data, base_latency=base_latency, method=method)
 
     # Validate again.
     num_corr = validate_data(data)
     if num_corr < 0:
         raise ValueError
 
     if output_filename is not None:
```

### Comparing `hftbacktest-1.5.2/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.5.3/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.5.3/hftbacktest/data/utils/tardis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import gzip
-from typing import List, Optional
+from typing import List, Optional, Literal
 
 import numpy as np
 from numpy.typing import NDArray
 
 from .. import merge_on_local_timestamp, correct, validate_data
 
 
 def convert(
         input_files: List[str],
         output_filename: Optional[str] = None,
         buffer_size: int = 100_000_000,
-        base_latency: float = 0
+        base_latency: float = 0,
+        method: Literal['separate', 'adjust'] = 'separate'
 ) -> NDArray:
     r"""
     Converts Tardis.dev data files into a format compatible with HftBacktest.
 
     Args:
         input_files: Input filenames for both incremental book and trades files,
                      e.g. ['incremental_book.csv', 'trades.csv'].
         output_filename: If provided, the converted data will be saved to the specified filename in ``npz`` format.
         buffer_size: Sets a preallocated row size for the buffer.
         base_latency: The value to be added to the feed latency.
                       See :func:`.correct_local_timestamp`.
+        method: The method to correct reversed exchange timestamp events. See :func:`..validation.correct`.
 
     Returns:
         Converted data compatible with HftBacktest.
     """
     TRADE = 0
     DEPTH = 1
 
@@ -157,15 +159,15 @@
     print('Merging')
     data = sets[0]
     del sets[0]
     while len(sets) > 0:
         data = merge_on_local_timestamp(data, sets[0])
         del sets[0]
 
-    data = correct(data, base_latency=base_latency)
+    data = correct(data, base_latency=base_latency, method=method)
 
     # Validate again.
     num_corr = validate_data(data)
     if num_corr < 0:
         raise ValueError
 
     if output_filename is not None:
```

### Comparing `hftbacktest-1.5.2/hftbacktest/data/validation.py` & `hftbacktest-1.5.3/hftbacktest/data/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,16 @@
                         corr[i, COL_LOCAL_TIMESTAMP] = -1
                         out_row_num += 1
                         break
             corr[out_row_num, :] = data[row_num, :]
             corr[out_row_num, COL_EXCH_TIMESTAMP] = -1
         else:
             corr[out_row_num, :] = data[row_num, :]
-            prev_exch_timestamp = exch_timestamp
+            if exch_timestamp > 0:
+                prev_exch_timestamp = exch_timestamp
         out_row_num += 1
     return corr[:out_row_num, :]
 
 
 def correct_exch_timestamp(data: Data, num_corr: int) -> Data:
     r"""
     Corrects exchange timestamps that are reversed by splitting each row into separate events, ordered by both exchange
```

### Comparing `hftbacktest-1.5.2/hftbacktest/marketdepth.py` & `hftbacktest-1.5.3/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/models/latencies.py` & `hftbacktest-1.5.3/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/models/queue.py` & `hftbacktest-1.5.3/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/order.py` & `hftbacktest-1.5.3/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/proc/local.py` & `hftbacktest-1.5.3/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.5.3/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.5.3/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/proc/proc.py` & `hftbacktest-1.5.3/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/reader.py` & `hftbacktest-1.5.3/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/stat.py` & `hftbacktest-1.5.3/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/state.py` & `hftbacktest-1.5.3/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest/typing.py` & `hftbacktest-1.5.3/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.5.3/hftbacktest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.2
+Version: 1.5.3
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -40,14 +40,18 @@
 
 * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
 * Complete tick-by-tick simulation with a variable time interval.
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
+Documentation
+=============
+
+See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
 
@@ -81,86 +85,81 @@
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
         order_id = 0
 
         while hbt.run:
-            # Check every 0.1s
+            # Checks every 0.1s
             if not hbt.elapse(0.1 * 1e6):
                 return False
 
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
-            # Obtain the current mid-price and compute the reservation price.
+            # Obtains the current mid-price and computes the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
             buy_order_price = reservation_price - half_spread
             sell_order_price = reservation_price + half_spread
 
             last_order_id = -1
             # Cancel all outstanding orders
             for order in hbt.orders.values():
                 if order.cancellable:
                     hbt.cancel(order.order_id)
                     last_order_id = order.order_id    
 			
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order cancellation responses is received.
+            # Waits until one of the order cancellation responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 				
-            # Clear cancelled, filled or expired orders.
+            # Clears cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
 	    last_order_id = -1
             if hbt.position < max_position:
-                # Submit a new post-only limit bid order.
+                # Submits a new post-only limit bid order.
                 order_id += 1
                 hbt.submit_buy_order(
                     order_id,
                     buy_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             if hbt.position > -max_position:
-                # Submit a new post-only limit ask order.
+                # Submits a new post-only limit ask order.
                 order_id += 1
                 hbt.submit_sell_order(
                     order_id,
                     sell_order_price,
                     order_qty,
                     GTX
                 )
                 last_order_id = order_id
 
             # All order requests are considered to be requested at the same time.
-            # Wait until one of the order responses is received.
+            # Waits until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
-            # Record the current state for stat calculation.
+            # Records the current state for stat calculation.
             stat.record(hbt)
         return True
 
     
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
-Documentation
-=============
-
-See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
-
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
     :alt: |Python Version
     :target: https://badge.fury.io/py/tensorflow
 
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
     :alt: |Codacy
```

### Comparing `hftbacktest-1.5.2/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.5.3/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.2/setup.cfg` & `hftbacktest-1.5.3/setup.cfg`

 * *Files identical despite different names*

