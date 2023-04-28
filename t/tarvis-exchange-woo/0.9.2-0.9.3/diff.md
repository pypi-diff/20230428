# Comparing `tmp/tarvis-exchange-woo-0.9.2.tar.gz` & `tmp/tarvis-exchange-woo-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-woo-0.9.2.tar", last modified: Tue Apr 25 23:49:57 2023, max compression
+gzip compressed data, was "tarvis-exchange-woo-0.9.3.tar", last modified: Fri Apr 28 08:03:00 2023, max compression
```

## Comparing `tarvis-exchange-woo-0.9.2.tar` & `tarvis-exchange-woo-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.974737 tarvis-exchange-woo-0.9.2/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-25 23:49:57.974737 tarvis-exchange-woo-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 23:49:57.974737 tarvis-exchange-woo-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      767 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.970737 tarvis-exchange-woo-0.9.2/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.970737 tarvis-exchange-woo-0.9.2/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.970737 tarvis-exchange-woo-0.9.2/tarvis/exchange/woo/
--rw-r--r--   0 root         (0) root         (0)    10792 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/tarvis/exchange/woo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11077 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/tarvis/exchange/woo/wooclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.970737 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      404 2023-04-25 23:49:57.000000 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-25 23:49:57.000000 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 23:49:57.000000 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 23:49:57.000000 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-25 23:49:57.000000 tarvis-exchange-woo-0.9.2/tarvis_exchange_woo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 23:49:57.974737 tarvis-exchange-woo-0.9.2/test/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/test/test_exchange_woo_margin.py
--rw-r--r--   0 root         (0) root         (0)    11996 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/test/test_exchange_woo_perpetual.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-04-25 23:49:45.000000 tarvis-exchange-woo-0.9.2/test/test_exchange_woo_spot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      767 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.453954 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/
+-rw-r--r--   0 root         (0) root         (0)    10910 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/wooclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 08:03:00.000000 tarvis-exchange-woo-0.9.3/tarvis_exchange_woo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:03:00.457955 tarvis-exchange-woo-0.9.3/test/
+-rw-r--r--   0 root         (0) root         (0)    11990 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_margin.py
+-rw-r--r--   0 root         (0) root         (0)    11996 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-04-28 08:02:50.000000 tarvis-exchange-woo-0.9.3/test/test_exchange_woo_spot.py
```

### Comparing `tarvis-exchange-woo-0.9.2/LICENSE.txt` & `tarvis-exchange-woo-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.2/setup.py` & `tarvis-exchange-woo-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-woo",
-    version="0.9.2",
+    version="0.9.3",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for Woo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-woo-0.9.2/tarvis/exchange/woo/__init__.py` & `tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,20 @@
 
         credentials = secrets.get_secret(credentials_secret, decode_json=True)
         api_key = credentials["api_key"]
         api_secret = credentials["api_secret"]
 
         if tarvis.common.environ.deployment == DeploymentType.PRODUCTION:
             base_url = "https://api.woo.org/"
+            application_id = "d5e1e017-b4b3-4cdd-9aa6-613974524596"
         else:
             base_url = "https://api.staging.woo.org/"
+            application_id = None
 
-        self._client = WooClient(base_url, api_key, api_secret)
+        self._client = WooClient(base_url, api_key, api_secret, application_id)
 
     @staticmethod
     def _convert_market_to_assets(market: str) -> (str, str, str):
         market_type, base_asset, quote_asset = market.split("_")
         return market_type, base_asset, quote_asset
 
     def _convert_assets_to_market(self, base_asset: str, quote_asset: str) -> str:
```

### Comparing `tarvis-exchange-woo-0.9.2/tarvis/exchange/woo/wooclient.py` & `tarvis-exchange-woo-0.9.3/tarvis/exchange/woo/wooclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,25 @@
         return self.__repr__()
 
     def __repr__(self):
         return f"WooClientError(status_code={self.status_code}, response={self.msg})"
 
 
 class WooClient:
-    def __init__(self, base_url: str, api_key: str = None, api_secret: str = None):
+    def __init__(
+        self,
+        base_url: str,
+        api_key: str = None,
+        api_secret: str = None,
+        application_id: str = None,
+    ):
         self._base_url = base_url.removesuffix("/")
         self._api_key = api_key
         self._api_secret = api_secret
+        self._application_id = application_id
         if api_key is not None:
             self._api_key_bytes = bytes(self._api_secret, "utf-8")
 
     @staticmethod
     def _get_request_path(version: int, end_point: str) -> str:
         return f"/v{version}/{end_point}"
 
@@ -301,14 +308,15 @@
         visible_quantity: str = None,
     ):
         self._post(
             1,
             "order",
             True,
             symbol=symbol,
+            broker_id=self._application_id,
             client_order_id=client_order_id,
             order_tag=order_tag,
             order_type=order_type,
             order_price=order_price,
             order_quantity=order_quantity,
             order_amount=order_amount,
             reduce_only=reduce_only,
@@ -337,14 +345,15 @@
     ):
         self._post(
             3,
             "algo/order",
             True,
             activatedPrice=activated_price,
             algoType=algo_type,
+            brokerId=self._application_id,
             callbackRate=callback_rate,
             callbackValue=callback_value,
             childOrders=child_orders,
             symbol=symbol,
             clientOrderId=client_order_id,
             orderTag=order_tag,
             price=order_price,
```

### Comparing `tarvis-exchange-woo-0.9.2/test/test_exchange_woo_margin.py` & `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_margin.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.2/test/test_exchange_woo_perpetual.py` & `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_perpetual.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.2/test/test_exchange_woo_spot.py` & `tarvis-exchange-woo-0.9.3/test/test_exchange_woo_spot.py`

 * *Files identical despite different names*

