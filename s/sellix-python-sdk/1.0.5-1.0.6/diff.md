# Comparing `tmp/sellix-python-sdk-1.0.5.tar.gz` & `tmp/sellix-python-sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sellix-python-sdk-1.0.5.tar", last modified: Mon Nov 21 15:55:59 2022, max compression
+gzip compressed data, was "sellix-python-sdk-1.0.6.tar", last modified: Fri Apr 28 18:03:14 2023, max compression
```

## Comparing `sellix-python-sdk-1.0.5.tar` & `sellix-python-sdk-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:55:59.801538 sellix-python-sdk-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-11-21 15:55:59.801538 sellix-python-sdk-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:55:59.797538 sellix-python-sdk-1.0.5/sellix/
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:55:59.797538 sellix-python-sdk-1.0.5/sellix/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/coupons.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/feedback.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/products.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/resources/whitelists.py
--rw-r--r--   0 runner    (1001) docker     (121)    11587 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/sellix/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 15:55:59.797538 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-11-21 15:55:59.000000 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-11-21 15:55:59.000000 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 15:55:59.000000 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-21 15:55:59.000000 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-21 15:55:59.000000 sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 15:55:59.801538 sellix-python-sdk-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-21 15:55:33.000000 sellix-python-sdk-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:03:14.120041 sellix-python-sdk-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-28 18:03:14.120041 sellix-python-sdk-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:03:14.112039 sellix-python-sdk-1.0.6/sellix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:03:14.116040 sellix-python-sdk-1.0.6/sellix/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/coupons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/resources/whitelists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/sellix/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:03:14.120041 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-28 18:03:14.000000 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-28 18:03:14.000000 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:03:14.000000 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 18:03:14.000000 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 18:03:14.000000 sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:03:14.120041 sellix-python-sdk-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 18:03:00.000000 sellix-python-sdk-1.0.6/setup.py
```

### Comparing `sellix-python-sdk-1.0.5/LICENSE` & `sellix-python-sdk-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/PKG-INFO` & `sellix-python-sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sellix-python-sdk
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://github.com/Sellix/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sellix Python SDK 
 
 ![tag](https://img.shields.io/github/v/tag/sellix/python-sdk?sort=date&color=blueviolet)
```

### Comparing `sellix-python-sdk-1.0.5/README.md` & `sellix-python-sdk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/__init__.py` & `sellix-python-sdk-1.0.6/sellix/__init__.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/blacklist.py` & `sellix-python-sdk-1.0.6/sellix/resources/blacklist.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/categories.py` & `sellix-python-sdk-1.0.6/sellix/resources/categories.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/coupons.py` & `sellix-python-sdk-1.0.6/sellix/resources/coupons.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/customers.py` & `sellix-python-sdk-1.0.6/sellix/resources/customers.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/groups.py` & `sellix-python-sdk-1.0.6/sellix/resources/groups.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/orders.py` & `sellix-python-sdk-1.0.6/sellix/resources/orders.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/products.py` & `sellix-python-sdk-1.0.6/sellix/resources/products.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,12 @@
     )
 
 
 def delete_product(self, uniqid):
     return self.handle_response(
         self.request(f"/products/{uniqid}", "DELETE")
     )
+
+def licensing_check(self, **kwargs):
+    return self.handle_response(
+        self.request(f"/products/licensing/check", "POST", kwargs)
+    )
```

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/queries.py` & `sellix-python-sdk-1.0.6/sellix/resources/queries.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/subscriptions.py` & `sellix-python-sdk-1.0.6/sellix/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/resources/whitelists.py` & `sellix-python-sdk-1.0.6/sellix/resources/whitelists.py`

 * *Files identical despite different names*

### Comparing `sellix-python-sdk-1.0.5/sellix/test.py` & `sellix-python-sdk-1.0.6/sellix/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
                                 type="SERIALS",
                                 serials=[
                                     "activation-key-#1"
                                 ])
             print("  Update product passed ✓")
             self.delete_product(product_uniqid)
             print("  Delete product passed ✓")
+            self.licensing_check(key="activation-key-#1",
+                                 product_id="demo",
+                                 hardware_id="example-id")
+            print("  Licensing check passed ✓")
 
         if "queries" in components:
             print("Testing queries")
             queries = self.get_queries()
             print("  Get queries passed ✓")
             if queries:
                 self.get_query(queries[0]["uniqid"])
```

### Comparing `sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/PKG-INFO` & `sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sellix-python-sdk
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://github.com/Sellix/python-sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sellix Python SDK 
 
 ![tag](https://img.shields.io/github/v/tag/sellix/python-sdk?sort=date&color=blueviolet)
```

### Comparing `sellix-python-sdk-1.0.5/sellix_python_sdk.egg-info/SOURCES.txt` & `sellix-python-sdk-1.0.6/sellix_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

