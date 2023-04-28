# Comparing `tmp/com_digitalruiz_shopify_tools-0.0.8.tar.gz` & `tmp/com_digitalruiz_shopify_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com_digitalruiz_shopify_tools-0.0.8.tar", last modified: Thu Mar  9 20:14:13 2023, max compression
+gzip compressed data, was "com_digitalruiz_shopify_tools-0.0.9.tar", last modified: Thu Mar  9 20:40:44 2023, max compression
```

## Comparing `com_digitalruiz_shopify_tools-0.0.8.tar` & `com_digitalruiz_shopify_tools-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:14:13.468582 com_digitalruiz_shopify_tools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-09 20:14:13.468582 com_digitalruiz_shopify_tools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:14:13.468582 com_digitalruiz_shopify_tools-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:14:13.464583 com_digitalruiz_shopify_tools-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:14:13.464583 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools/shopify_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:14:13.464583 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-09 20:14:13.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-09 20:14:13.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:14:13.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-09 20:14:13.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-09 20:14:13.000000 com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:14:13.468582 com_digitalruiz_shopify_tools-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-09 20:13:59.000000 com_digitalruiz_shopify_tools-0.0.8/tests/test_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools/shopify_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-09 20:40:44.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-09 20:40:44.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:40:44.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-09 20:40:44.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-09 20:40:44.000000 com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:40:44.880690 com_digitalruiz_shopify_tools-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-09 20:40:32.000000 com_digitalruiz_shopify_tools-0.0.9/tests/test_pass.py
```

### Comparing `com_digitalruiz_shopify_tools-0.0.8/LICENSE` & `com_digitalruiz_shopify_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `com_digitalruiz_shopify_tools-0.0.8/PKG-INFO` & `com_digitalruiz_shopify_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com_digitalruiz_shopify_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collections of custom shopify functions
 Author-email: Reyes Ruiz <reyes@digitalruiz.com>
 Project-URL: Homepage, https://github.com/reyesruiz/shopify_tools
 Project-URL: Bug Tracker, https://github.com/reyesruiz/shopify_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `com_digitalruiz_shopify_tools-0.0.8/pyproject.toml` & `com_digitalruiz_shopify_tools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "com_digitalruiz_shopify_tools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Reyes Ruiz", email="reyes@digitalruiz.com" },
 ]
 description = "Collections of custom shopify functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools/shopify_tools.py` & `com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools/shopify_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -375,7 +375,20 @@
         for product in products:
             for variant in product['variants']:
                 variant_barcode = variant['barcode']
                 if barcode == variant_barcode:
                     return variant
         return False
     return False
+
+def find_product_by_sku(sku, products = None):
+    '''
+    Function to find products by sku
+    '''
+    if not products:
+        products = shopify.get_all_products()
+    if products:
+        for product in products:
+            for variant in product['variants']:
+                if sku == variant['sku']:
+                    return product
+    return False
```

### Comparing `com_digitalruiz_shopify_tools-0.0.8/src/com_digitalruiz_shopify_tools.egg-info/PKG-INFO` & `com_digitalruiz_shopify_tools-0.0.9/src/com_digitalruiz_shopify_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com-digitalruiz-shopify-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collections of custom shopify functions
 Author-email: Reyes Ruiz <reyes@digitalruiz.com>
 Project-URL: Homepage, https://github.com/reyesruiz/shopify_tools
 Project-URL: Bug Tracker, https://github.com/reyesruiz/shopify_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

