# Comparing `tmp/trex-model-1.0.0.tar.gz` & `tmp/trex-model-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-model-1.0.0.tar", last modified: Mon Apr 17 03:29:44 2023, max compression
+gzip compressed data, was "trex-model-1.0.1.tar", last modified: Fri Apr 28 10:31:17 2023, max compression
```

## Comparing `trex-model-1.0.0.tar` & `trex-model-1.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.462242 trex-model-1.0.0/
--rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.0/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.0/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-17 03:29:44.462462 trex-model-1.0.0/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.0/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-17 03:29:44.463124 trex-model-1.0.0/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-04-17 03:26:40.000000 trex-model-1.0.0/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.430424 trex-model-1.0.0/trex_model.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-04-17 03:29:44.000000 trex-model-1.0.0/trex_model.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.432308 trex-model-1.0.0/trexmodel/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.0/trexmodel/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.0/trexmodel/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.434164 trex-model-1.0.0/trexmodel/models/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.0/trexmodel/models/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.456400 trex-model-1.0.0/trexmodel/models/datastore/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.0/trexmodel/models/datastore/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.0/trexmodel/models/datastore/admin_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.0/trexmodel/models/datastore/analytic_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.0/trexmodel/models/datastore/coporate_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.0/trexmodel/models/datastore/customer_model_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47628 2023-04-13 05:33:49.000000 trex-model-1.0.0/trexmodel/models/datastore/customer_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.0/trexmodel/models/datastore/fb_subsriber_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.0/trexmodel/models/datastore/inventory_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5816 2023-03-02 14:42:44.000000 trex-model-1.0.0/trexmodel/models/datastore/loyalty_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.0/trexmodel/models/datastore/membership_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    57095 2023-04-13 02:21:06.000000 trex-model-1.0.0/trexmodel/models/datastore/merchant_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.0/trexmodel/models/datastore/model_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.0/trexmodel/models/datastore/ndb_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-1.0.0/trexmodel/models/datastore/pos_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.0/trexmodel/models/datastore/prepaid_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.0/trexmodel/models/datastore/product_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.0/trexmodel/models/datastore/program_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.0/trexmodel/models/datastore/redeem_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.0/trexmodel/models/datastore/reward_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.0/trexmodel/models/datastore/spending_base_program_model.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.0/trexmodel/models/datastore/system_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.0/trexmodel/models/datastore/task_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.0/trexmodel/models/datastore/test_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    33133 2023-04-11 02:45:33.000000 trex-model-1.0.0/trexmodel/models/datastore/transaction_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.0/trexmodel/models/datastore/user_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.0/trexmodel/models/datastore/voucher_models.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.0/trexmodel/models/merchant_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.0/trexmodel/models/model_decorator.py
--rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.0/trexmodel/models/prepaid_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.0/trexmodel/pos_conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.0/trexmodel/program_conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.458294 trex-model-1.0.0/trexmodel/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.459091 trex-model-1.0.0/trexmodel/utils/gcloud/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/gcloud/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/gcloud/datastore_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:29:44.461629 trex-model-1.0.0/trexmodel/utils/model/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.0/trexmodel/utils/model/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.0/trexmodel/utils/model/model_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.177978 trex-model-1.0.1/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1074 2020-09-06 08:34:15.000000 trex-model-1.0.1/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       60 2020-09-10 05:51:48.000000 trex-model-1.0.1/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-28 10:31:17.178389 trex-model-1.0.1/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       57 2020-09-06 08:43:45.000000 trex-model-1.0.1/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-28 10:31:17.179287 trex-model-1.0.1/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      922 2023-04-28 10:15:33.000000 trex-model-1.0.1/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.137434 trex-model-1.0.1/trex_model.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      492 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1799 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       95 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       16 2023-04-28 10:31:16.000000 trex-model-1.0.1/trex_model.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.140045 trex-model-1.0.1/trexmodel/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-06 08:58:46.000000 trex-model-1.0.1/trexmodel/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1122 2021-09-03 09:11:14.000000 trex-model-1.0.1/trexmodel/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.143298 trex-model-1.0.1/trexmodel/models/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-03 01:59:33.000000 trex-model-1.0.1/trexmodel/models/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.173728 trex-model-1.0.1/trexmodel/models/datastore/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 04:46:11.000000 trex-model-1.0.1/trexmodel/models/datastore/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4892 2022-11-14 06:42:31.000000 trex-model-1.0.1/trexmodel/models/datastore/admin_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3223 2023-04-11 07:48:46.000000 trex-model-1.0.1/trexmodel/models/datastore/analytic_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2155 2021-02-19 08:24:29.000000 trex-model-1.0.1/trexmodel/models/datastore/coporate_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13539 2023-03-15 08:15:01.000000 trex-model-1.0.1/trexmodel/models/datastore/customer_model_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47628 2023-04-13 05:33:49.000000 trex-model-1.0.1/trexmodel/models/datastore/customer_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1712 2020-10-26 01:02:17.000000 trex-model-1.0.1/trexmodel/models/datastore/fb_subsriber_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1351 2021-08-19 08:33:56.000000 trex-model-1.0.1/trexmodel/models/datastore/inventory_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5816 2023-03-02 14:42:44.000000 trex-model-1.0.1/trexmodel/models/datastore/loyalty_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11281 2023-04-05 03:48:05.000000 trex-model-1.0.1/trexmodel/models/datastore/membership_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    57199 2023-04-25 06:49:40.000000 trex-model-1.0.1/trexmodel/models/datastore/merchant_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1785 2021-05-17 10:44:34.000000 trex-model-1.0.1/trexmodel/models/datastore/model_decorators.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17711 2023-02-10 02:53:30.000000 trex-model-1.0.1/trexmodel/models/datastore/ndb_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    32092 2023-01-04 03:56:36.000000 trex-model-1.0.1/trexmodel/models/datastore/pos_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    20750 2023-04-10 08:59:10.000000 trex-model-1.0.1/trexmodel/models/datastore/prepaid_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    38941 2023-02-28 05:40:30.000000 trex-model-1.0.1/trexmodel/models/datastore/product_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    47521 2023-03-15 14:31:35.000000 trex-model-1.0.1/trexmodel/models/datastore/program_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36350 2023-04-13 13:46:37.000000 trex-model-1.0.1/trexmodel/models/datastore/redeem_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    31165 2023-04-10 09:19:08.000000 trex-model-1.0.1/trexmodel/models/datastore/reward_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      602 2021-02-19 08:54:31.000000 trex-model-1.0.1/trexmodel/models/datastore/spending_base_program_model.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6610 2021-03-30 06:42:06.000000 trex-model-1.0.1/trexmodel/models/datastore/system_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1348 2020-09-09 01:17:56.000000 trex-model-1.0.1/trexmodel/models/datastore/task_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1319 2022-09-09 14:28:48.000000 trex-model-1.0.1/trexmodel/models/datastore/test_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36809 2023-04-24 09:59:51.000000 trex-model-1.0.1/trexmodel/models/datastore/transaction_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15228 2022-09-23 07:10:51.000000 trex-model-1.0.1/trexmodel/models/datastore/user_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17441 2022-12-29 13:44:05.000000 trex-model-1.0.1/trexmodel/models/datastore/voucher_models.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6452 2023-03-19 11:12:11.000000 trex-model-1.0.1/trexmodel/models/merchant_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-05-16 04:55:29.000000 trex-model-1.0.1/trexmodel/models/model_decorator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      331 2021-09-02 08:53:31.000000 trex-model-1.0.1/trexmodel/models/prepaid_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2022-03-04 03:54:52.000000 trex-model-1.0.1/trexmodel/pos_conf.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16572 2023-04-07 03:52:51.000000 trex-model-1.0.1/trexmodel/program_conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.175242 trex-model-1.0.1/trexmodel/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.175877 trex-model-1.0.1/trexmodel/utils/gcloud/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/gcloud/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      291 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/gcloud/datastore_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:31:17.177110 trex-model-1.0.1/trexmodel/utils/model/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-model-1.0.1/trexmodel/utils/model/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2453 2022-09-09 14:29:07.000000 trex-model-1.0.1/trexmodel/utils/model/model_util.py
```

### Comparing `trex-model-1.0.0/LICENSE` & `trex-model-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/setup.py` & `trex-model-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='trex-model',  
-     version='1.0.0',
+     version='1.0.1',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex database module package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-model",
      packages=setuptools.find_packages(),
```

### Comparing `trex-model-1.0.0/trex_model.egg-info/SOURCES.txt` & `trex-model-1.0.1/trex_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/conf.py` & `trex-model-1.0.1/trexmodel/conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/admin_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/admin_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/analytic_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/analytic_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/coporate_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/coporate_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/customer_model_helpers.py` & `trex-model-1.0.1/trexmodel/models/datastore/customer_model_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/customer_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/customer_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/fb_subsriber_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/fb_subsriber_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/inventory_model.py` & `trex-model-1.0.1/trexmodel/models/datastore/inventory_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/loyalty_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/loyalty_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/membership_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/membership_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/merchant_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/merchant_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,18 @@
                 'plan_end_date'     : self.plan_end_date,
                 'currency_code'     : self.currency_code,
                 'country'           : self.country,
                 }
     
     @property
     def program_configuration_list(self):
-        return self.published_program_configuration.get('programs')
+        if is_not_empty(self.published_program_configuration):
+            return  self.published_program_configuration.get('programs')
+        else:
+            return []
     
     
     @property
     def is_tier_membership_configured(self):
         return is_not_empty(self.tier_membership_configuration)
```

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/model_decorators.py` & `trex-model-1.0.1/trexmodel/models/datastore/model_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/ndb_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/ndb_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/pos_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/pos_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/prepaid_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/prepaid_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/product_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/product_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/program_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/program_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/redeem_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/redeem_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/reward_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/reward_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/spending_base_program_model.py` & `trex-model-1.0.1/trexmodel/models/datastore/spending_base_program_model.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/system_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/system_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/task_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/task_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/test_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/test_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/transaction_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/transaction_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 from trexmodel.program_conf import REWARD_FORMAT_POINT
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
 
 logger = logging.getLogger('model')
 
-
-class CustomerTransaction(BaseNModel, DictModel):
-    '''
-    
-    '''
+class SalesTransaction(BaseNModel, DictModel):
     transact_merchant           = ndb.KeyProperty(name="transact_merchant", kind=MerchantAcct)
     transact_outlet             = ndb.KeyProperty(name="transact_outlet", kind=Outlet)
     
     transact_datetime           = ndb.DateTimeProperty(required=True)
     created_datetime            = ndb.DateTimeProperty(required=True, auto_now=True)
     
+    reverted_datetime           = ndb.DateTimeProperty(required=False)
+    reverted_by                 = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
+    reverted_by_username        = ndb.StringProperty(required=False)
+    
     transact_timestamp          = ndb.FloatProperty(required=False)
     
     transaction_id              = ndb.StringProperty(required=True)
     invoice_id                  = ndb.StringProperty(required=False)
     remarks                     = ndb.StringProperty(required=False)
     system_remarks              = ndb.StringProperty(required=False)
     
@@ -47,31 +47,139 @@
     transact_amount             = ndb.FloatProperty(required=True)
     
     transact_by                 = ndb.KeyProperty(name="created_by", kind=MerchantUser)
     transact_by_username        = ndb.StringProperty(required=False)
     
     sales_channel               = ndb.StringProperty(required=False)
     
+    is_revert                   = ndb.BooleanProperty(required=False, default=False)
+    is_sales_transaction        = ndb.BooleanProperty(required=False, default=True)
+    allow_to_revert             = ndb.BooleanProperty(required=False, default=True)
+    
+    reward_expiry_date          = ndb.DateProperty(required=False)
+    
+    dict_properties         = [
+                               'transaction_id', 'invoice_id', 'remarks', 'system_remarks', 'tax_amount', 'transact_amount', 
+                               'transact_customer_acct', 'transact_outlet_details', 'transact_merchant_acct',
+                               'transact_datetime', 'created_datetime',  'transact_outlet_key', 
+                               'is_sales_transaction', 'allow_to_revert', 'reward_expiry_date',
+                               'transact_by', 'transact_by_username', 
+                               
+                               ]
+    
+    @property
+    def transact_customer_key(self):
+        return ''
+    
+    @property
+    def transact_merchant_acct(self):
+        return MerchantAcct.fetch(self.transact_merchant.urlsafe())
+    
+    @property
+    def transact_outlet_key(self):
+        if self.transact_outlet:
+            return self.transact_outlet.urlsafe().decode('utf-8')
+    
+    @property
+    def transact_merchant_acct_key(self):
+        return self.transact_merchant.urlsafe().decode('utf-8')
+
+    @property
+    def transact_by_user(self):
+        if self.transact_by:
+            return MerchantUser.fetch(self.transact_by.urlsafe())
+        
+    @property
+    def transact_user_acct_key(self):
+        return self.transact_by.urlsafe()
+        
+    @property
+    def after_deduct_tax_sales_amount(self):
+        if self.tax_amount:
+            return self.transact_amount - self.tax_amount
+        else:
+            return self.transact_amount
+    
+    @classmethod
+    def get_by_invoice_id(cls, invoice_id):
+        return cls.query(cls.invoice_id==invoice_id).get()
+    
+    @staticmethod
+    def create(transact_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, system_remarks=None,
+               transact_outlet=None, transact_by=None, transact_datetime=None, 
+               
+               ):
+        
+        transact_by_username = None
+        
+        if is_not_empty(transact_by):
+            if isinstance(transact_by, MerchantUser):
+                transact_by_username = transact_by.username
+
+        
+        transaction_id = generate_transaction_id()
+        
+        if transact_datetime is None:
+            transact_datetime = datetime.utcnow()
+        
+        logger.debug('generated transaction_id=%s', transaction_id)
+        logger.debug('invoice_id=%s', invoice_id)
+        logger.debug('tax_amount=%s', tax_amount)
+        logger.debug('transact_amount=%s', transact_amount)
+        logger.debug('transact_datetime=%s', transact_datetime)
+        logger.debug('transact_by_username=%s', transact_by_username)
+        logger.debug('system_remarks=%s', system_remarks)
+        
+        customer_transaction = SalesTransaction(
+                                transact_merchant               = transact_outlet.merchant_acct_entity.create_ndb_key(),
+                                transact_outlet                 = transact_outlet.create_ndb_key() if transact_outlet else None,
+                                
+                                tax_amount                      = tax_amount,
+                                transact_amount                 = transact_amount,
+                                
+                                transaction_id                  = transaction_id,
+                                invoice_id                      = invoice_id,
+                                remarks                         = remarks,
+                                system_remarks                  = system_remarks,
+                                
+                                transact_by                     = transact_by.create_ndb_key() if transact_by else None,
+                                transact_by_username            = transact_by_username,
+                                
+                                transact_datetime               = transact_datetime,
+                                
+                                is_sales_transaction            = True,
+                                allow_to_revert                 = True,
+                                
+                                )
+        
+        customer_transaction.put()
+        #customer.put()
+        
+        return customer_transaction
+    
+class CustomerTransaction(SalesTransaction):
+    '''
+    Customer as ancestor
+    '''
+    
+    
     entitled_reward_summary     = ndb.JsonProperty()
     entitled_voucher_summary    = ndb.JsonProperty()
     entitled_prepaid_summary    = ndb.JsonProperty()
     entitled_program_summary    = ndb.JsonProperty()
     
     reward_giveaway_method      = ndb.StringProperty(required=False, default=program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM)
     
-    allow_to_revert             = ndb.BooleanProperty(required=False, default=True)
     
-    is_revert                   = ndb.BooleanProperty(required=False, default=False)
-    reverted_datetime           = ndb.DateTimeProperty(required=False)
-    reverted_by                 = ndb.KeyProperty(name="reverted_by", kind=MerchantUser)
-    reverted_by_username        = ndb.StringProperty(required=False)
+    
+    is_from_instant_transaction = ndb.BooleanProperty(required=False, default=False)
     
     is_reward_redeemed          = ndb.BooleanProperty(required=False, default=False)
     
-    is_sales_transaction        = ndb.BooleanProperty(required=False, default=True)
+    
     
     is_membership_purchase      = ndb.BooleanProperty(required=False, default=False)
     is_membership_renew         = ndb.BooleanProperty(required=False, default=False)
     
     is_tier_membership_upgraded = ndb.BooleanProperty(required=False, default=False)
     
     upgraded_merchant_tier_membership   = ndb.KeyProperty(name="upgraded_merchant_tier_membership", kind=MerchantTierMembership)
@@ -117,55 +225,32 @@
         return False
     
     @property
     def transact_customer_acct(self):
         return Customer.fetch(self.key.parent().urlsafe())
     
     @property
-    def transact_user_acct_key(self):
-        return Customer.fetch(self.key.parent().urlsafe()).registered_user_acct_key
-    
-    @property
-    def transact_merchant_acct(self):
-        return MerchantAcct.fetch(self.transact_merchant.urlsafe())
-    
-    @property
-    def transact_outlet_key(self):
-        if self.transact_outlet:
-            return self.transact_outlet.urlsafe().decode('utf-8')
-    
-    @property
-    def transact_merchant_acct_key(self):
-        return self.transact_merchant.urlsafe().decode('utf-8')
-    
-    @property
     def transact_customer_key(self):
         return self.key.parent().urlsafe().decode('utf-8')
     
     @property
     def transact_outlet_details(self):
         if self.transact_outlet:
             return Outlet.fetch(self.transact_outlet.urlsafe())
     
-    @property
-    def transact_by_user(self):
-        if self.transact_by:
-            return MerchantUser.fetch(self.transact_by.urlsafe())
-        
-    @property
-    def after_deduct_tax_sales_amount(self):
-        if self.tax_amount:
-            return self.transact_amount - self.tax_amount
-        else:
-            return self.transact_amount
     
     @property
     def purchased_merchant_membership_key(self):
         if self.purchased_merchant_membership:
             return self.purchased_merchant_membership.urlsafe().decode('utf-8')
+        
+    @property
+    def purchased_merchant_membership_entity(self):
+        if self.purchased_merchant_membership:
+            return MerchantMembership.fetch(self.purchased_merchant_membership.urlsafe())    
     
     @property
     def purchased_customer_membership_entity(self):
         if self.purchased_customer_membership:
             return CustomerMembership.fetch(self.purchased_customer_membership.urlsafe())
     
     @property
@@ -450,18 +535,14 @@
                                                   ),ancestor = customer_acct.create_ndb_key()).fetch(limit=conf.MAX_FETCH_RECORD)    
     
     @staticmethod
     def get_by_transaction_id(transaction_id):
         return CustomerTransaction.query(CustomerTransaction.transaction_id==transaction_id).get()
     
     @staticmethod
-    def get_by_invoice_id(invoice_id):
-        return CustomerTransaction.query(CustomerTransaction.invoice_id==invoice_id).get()
-    
-    @staticmethod
     def list_transaction_by_date(transact_date, transact_outlet=None, including_reverted_transaction=True, offset=0, limit=conf.PAGINATION_SIZE, start_cursor=None, return_with_cursor=False):
         
         transact_datetime           = datetime.combine(transact_date, datetime.min.time())
         next_day_transact_datetime  = transact_datetime + timedelta(days=1)
         
         logger.debug('transact_datetime=%s',transact_datetime)
         logger.debug('next_day_transact_datetime=%s',next_day_transact_datetime)
```

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/user_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/user_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/datastore/voucher_models.py` & `trex-model-1.0.1/trexmodel/models/datastore/voucher_models.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/models/merchant_helpers.py` & `trex-model-1.0.1/trexmodel/models/merchant_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/program_conf.py` & `trex-model-1.0.1/trexmodel/program_conf.py`

 * *Files identical despite different names*

### Comparing `trex-model-1.0.0/trexmodel/utils/model/model_util.py` & `trex-model-1.0.1/trexmodel/utils/model/model_util.py`

 * *Files identical despite different names*

