# Comparing `tmp/seven_studio-1.3.2.tar.gz` & `tmp/seven_studio-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_studio-1.3.2.tar", last modified: Thu Apr 27 11:20:01 2023, max compression
+gzip compressed data, was "dist/seven_studio-1.4.0.tar", last modified: Fri Apr 28 07:40:19 2023, max compression
```

## Comparing `seven_studio-1.3.2.tar` & `seven_studio-1.4.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.711851 seven_studio-1.3.2/
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-27 11:20:01.710851 seven_studio-1.3.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1494 2023-04-27 11:19:10.000000 seven_studio-1.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 11:20:01.711851 seven_studio-1.3.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1265 2023-04-27 11:19:10.000000 seven_studio-1.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.645852 seven_studio-1.3.2/seven_studio/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.652852 seven_studio-1.3.2/seven_studio/handlers/
--rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    25307 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/studio_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.657852 seven_studio-1.3.2/seven_studio/handlers/system/
--rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9186 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/core.py
--rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/file.py
--rwxrwxrwx   0 root         (0) root         (0)    17591 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/menu.py
--rwxrwxrwx   0 root         (0) root         (0)    31748 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/power.py
--rwxrwxrwx   0 root         (0) root         (0)     6606 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/product.py
--rwxrwxrwx   0 root         (0) root         (0)     2582 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/handlers/system/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.659852 seven_studio-1.3.2/seven_studio/libs/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.670852 seven_studio-1.3.2/seven_studio/libs/file/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/bos.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/cos.py
--rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/ks3.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/oss2.py
--rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/s3.py
--rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/file/upload.py
--rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/libs/geetest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.679852 seven_studio-1.3.2/seven_studio/models/
--rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.679852 seven_studio-1.3.2/seven_studio/models/db_models/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.686852 seven_studio-1.3.2/seven_studio/models/db_models/file/
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_history_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_resource_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_pic_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_storage_path_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/file/file_water_image_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.690852 seven_studio-1.3.2/seven_studio/models/db_models/log/
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/log/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/log/log_action_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.692852 seven_studio-1.3.2/seven_studio/models/db_models/menu/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_cote_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model_ex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.695851 seven_studio-1.3.2/seven_studio/models/db_models/product/
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/product_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/product/product_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.700852 seven_studio-1.3.2/seven_studio/models/db_models/role/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model.py
--rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/role/role_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.704851 seven_studio-1.3.2/seven_studio/models/db_models/settings/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/settings/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/settings/settings_base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.706851 seven_studio-1.3.2/seven_studio/models/db_models/user/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1125 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/db_models/user/user_login_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/dto_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/enum.py
--rwxrwxrwx   0 root         (0) root         (0)    37518 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/power_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/models/seven_model.py
--rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.709851 seven_studio-1.3.2/seven_studio/utils/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/dict.py
--rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-27 11:19:10.000000 seven_studio-1.3.2/seven_studio/utils/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 11:20:01.649852 seven_studio-1.3.2/seven_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2636 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 11:20:01.000000 seven_studio-1.3.2/seven_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.818382 seven_studio-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-04-28 07:40:19.818382 seven_studio-1.4.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1556 2023-04-28 07:39:41.000000 seven_studio-1.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 07:40:19.818382 seven_studio-1.4.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1262 2023-04-28 07:39:41.000000 seven_studio-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.801374 seven_studio-1.4.0/seven_studio/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.804376 seven_studio-1.4.0/seven_studio/handlers/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26036 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/studio_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.805376 seven_studio-1.4.0/seven_studio/handlers/system/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9452 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/file.py
+-rwxrwxrwx   0 root         (0) root         (0)    17655 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/menu.py
+-rwxrwxrwx   0 root         (0) root         (0)    32048 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/power.py
+-rwxrwxrwx   0 root         (0) root         (0)     6678 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/product.py
+-rwxrwxrwx   0 root         (0) root         (0)     2636 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.806377 seven_studio-1.4.0/seven_studio/libs/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.808378 seven_studio-1.4.0/seven_studio/libs/file/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/bos.py
+-rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/cos.py
+-rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/ks3.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/oss2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/s3.py
+-rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/geetest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.810378 seven_studio-1.4.0/seven_studio/models/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.810378 seven_studio-1.4.0/seven_studio/models/db_models/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.812379 seven_studio-1.4.0/seven_studio/models/db_models/file/
+-rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_history_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_resource_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_pic_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_storage_path_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_water_image_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.812379 seven_studio-1.4.0/seven_studio/models/db_models/log/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/log/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/log/log_action_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.813380 seven_studio-1.4.0/seven_studio/models/db_models/menu/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_cote_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model_ex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.814381 seven_studio-1.4.0/seven_studio/models/db_models/product/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/product_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/product_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.816381 seven_studio-1.4.0/seven_studio/models/db_models/role/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.816381 seven_studio-1.4.0/seven_studio/models/db_models/settings/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/settings/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/settings/settings_base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.817382 seven_studio-1.4.0/seven_studio/models/db_models/user/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_login_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/dto_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/enum.py
+-rwxrwxrwx   0 root         (0) root         (0)    37633 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/seven_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.818382 seven_studio-1.4.0/seven_studio/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/dict.py
+-rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.803375 seven_studio-1.4.0/seven_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/top_level.txt
```

### Comparing `seven_studio-1.3.2/PKG-INFO` & `seven_studio-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: seven_studio
-Version: 1.3.2
+Version: 1.4.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
-Description: 
-        
-        <!--
+Description: <!--
          * @Author: ChenXiaolei
          * @Date: 2022-01-18 18:52:26
          * @LastEditTime: 2022-11-22 16:41:30
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.4.0 更新内容
+        * 优化配置文件
+        * 修改json_dumps
+        
         ### 1.3.2 更新内容
         * 登录问题修改
         
         ### 1.2.0 更新内容
         * GetUserInfoHandler增加字段返回
         
         ### 1.1.9 更新内容
```

### Comparing `seven_studio-1.3.2/README.md` & `seven_studio-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-
-
 <!--
  * @Author: ChenXiaolei
  * @Date: 2022-01-18 18:52:26
  * @LastEditTime: 2022-11-22 16:41:30
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 # seven_studio
 
 ## 天志互联Python公共基础后台管理平台
 
+### 1.4.0 更新内容
+* 优化配置文件
+* 修改json_dumps
+
 ### 1.3.2 更新内容
 * 登录问题修改
 
 ### 1.2.0 更新内容
 * GetUserInfoHandler增加字段返回
 
 ### 1.1.9 更新内容
```

### Comparing `seven_studio-1.3.2/setup.py` & `seven_studio-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_studio",
-    version="1.3.2",
+    version="1.4.0",
     author="seven",
     author_email="tech@gao7.com",
     description="seven studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_studio",
     packages=find_packages(),
     install_requires=[
-        "seven-framework >=1.0.134.3",
+        "seven-framework >=1.1.28",
         "asq>=1.3"
     ],
     classifiers=[
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/studio_base.py` & `seven_studio-1.4.0/seven_studio/handlers/studio_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 :Author: ChenXiaolei
 :Date: 2020-03-24 10:42:34
-:LastEditTime: 2023-04-27 18:19:33
+:LastEditTime: 2023-04-28 15:26:27
 :LastEditors: HuangJingCan
 :Description: StudioBaseHandler
 """
-
+import ast
 from seven_framework.web_tornado.base_handler.base_cookie_handler import *
 from seven_framework.redis import *
 
 from seven_studio.models.db_models.product.product_info_model import *
 from seven_studio.models.db_models.user.user_login_model import *
 from seven_studio.models.db_models.user.user_info_model import *
 from seven_studio.models.db_models.menu.menu_info_model_ex import *
@@ -60,22 +60,37 @@
             return op_result
         except:
             self.logger_error.error(f"添加平台行为日志时异常:{traceback.format_exc()}")
             return False
 
     def json_dumps(self, rep_dic):
         """
-        :description: 用于将字典形式的数据转化为字符串
+        :description: 对象编码成Json字符串
         :param rep_dic：字典对象
         :return: str
-        :last_editors: HuangJingCan
+        :last_editors: HuangJianYi
         """
+        try:
+            if rep_dic == "":
+                return ""
+            rep_dic = ast.literal_eval(rep_dic)
+        except Exception:
+            pass
+
         if hasattr(rep_dic, '__dict__'):
             rep_dic = rep_dic.__dict__
-        return json.dumps(rep_dic, ensure_ascii=False, cls=JsonEncoder)
+
+        return json.dumps(
+            rep_dic,
+            ensure_ascii=False,
+            cls=JsonEncoder,
+            default=lambda x: (datetime.datetime.strftime(x, '%Y-%m-%d %H:%M:%S') if isinstance(x, datetime.datetime) else x.__dict__) if not isinstance(x, decimal.Decimal) else float(x),
+            sort_keys=False,
+            indent=None,
+        )
 
     def json_loads(self, rep_str):
         """
         :description: 将Json字符串解码成python对象
         :param rep_str：str
         :return: dict
         :last_editors: HuangJingCan
@@ -189,44 +204,44 @@
         return product_id
 
     def request_manage_page_id(self):
         return (self.request.headers["Manage-PageID"] if self.request.headers.__contains__("Manage-PageID") else "")
 
     def get_product_info(self):
         product_id = self.request_product_id()
-        return (ProductInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(product_id) if product_id > 0 else None)
+        return (ProductInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio")).get_entity_by_id(product_id) if product_id > 0 else None)
 
     def get_curr_user_info(self):
         user_id = self.request_user_id()
         return (UserInfoModel(self.get_manage_context_key()).get_entity_by_id(user_id) if user_id else None)
 
     def get_base_user_info(self):
         user_id = self.request_user_id()
-        return (UserInfoModel(config.get_value("base_manage_context_key")).get_entity_by_id(user_id) if user_id else None)
+        return (UserInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio")).get_entity_by_id(user_id) if user_id else None)
 
     def get_is_super(self):
         base_user_info = self.get_base_user_info()
         return base_user_info.IsSuper == 1 if base_user_info else False
 
     def get_manage_context_key(self):
-        manage_context_key = config.get_value("manage_context_key")
+        manage_context_key = config.get_value("manage_context_key", "db_sevenstudio")
         product_info = self.get_product_info()
         if product_info:
             manage_context_key = product_info.ManageContextKey
         return manage_context_key
 
     def get_file_context_key(self):
-        file_context_key = config.get_value("file_context_key")
+        file_context_key = config.get_value("file_context_key", "db_sevenstudio")
         product_info = self.get_product_info()
         if product_info:
             file_context_key = product_info.FileContextKey
         return file_context_key
 
     def get_log_context_key(self):
-        log_context_key = config.get_value("log_context_key")
+        log_context_key = config.get_value("log_context_key", "db_sevenstudio")
         product_info = self.get_product_info()
         if product_info:
             log_context_key = product_info.LogContextKey
         return log_context_key
 
     def get_page_index(self):
         page_index = 0
@@ -340,18 +355,18 @@
         :description: 用户退出
         :param user_id：用户id
         :return: 
         :last_editors: HuangJingCan
         """
         if user_id.strip() == "":
             return
-        if config.get_value("login_type") == "redis":
-            self.redis_init().hdel(config.get_value("redis_provider_name_user_login"), user_id)
+        if config.get_value("login_type", "redis") == "redis":
+            self.redis_init().hdel(config.get_value("redis_provider_name_user_login", "user_login"), user_id)
         else:
-            UserLoginModel(config.get_value("manage_context_key")).del_entity("UserID=%s", user_id)
+            UserLoginModel(config.get_value("manage_context_key", "db_sevenstudio")).del_entity("UserID=%s", user_id)
 
         self.clear_user_cookie()
 
     def clear_user_cookie(self):
         """
         :description: 清理用户登录cookie
         """
@@ -362,18 +377,18 @@
     def login_cookie(self, user_login):
         """
         :description: 登录状态设置
         :param user_login: 登录信息
         :return: user_login
         :last_editors: HuangJingCan
         """
-        if config.get_value("login_type") == "redis":
-            self.redis_init().hset(config.get_value("redis_provider_name_user_login"), user_login.UserID, self.json_dumps(user_login))
+        if config.get_value("login_type", "redis") == "redis":
+            self.redis_init().hset(config.get_value("redis_provider_name_user_login", "user_login"), user_login.UserID, self.json_dumps(user_login))
         else:
-            user_login_base = UserLoginModel(config.get_value("base_manage_context_key"))
+            user_login_base = UserLoginModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
             user_login_base.add_update_entity(user_login, "UserIDMD5=%s,ExpireTime=%s,UserToken=%s", [user_login.UserIDMD5, user_login.ExpireTime, user_login.UserToken])
 
         cookie_domain = config.get_value("cookie_domain")
         if cookie_domain:
             self.set_cookie("UserID", user_login.UserID, domain=cookie_domain)
             self.set_cookie("UserIDMD5", user_login.UserIDMD5, domain=cookie_domain)
             self.set_cookie("UserToken", user_login.UserToken, domain=cookie_domain)
@@ -421,16 +436,16 @@
         :description: 登录用户检查
         :param user_id：用户id
         :param user_token：用户user_token
         :return: 
         """
         invoke_result = InvokeResult()
         # 登陆日志判断，Redis还是MySQL
-        if config.get_value("login_type") == "redis":
-            redis_user_login = self.redis_init().hget(config.get_value("redis_provider_name_user_login"), user_id)
+        if config.get_value("login_type", "redis") == "redis":
+            redis_user_login = self.redis_init().hget(config.get_value("redis_provider_name_user_login", "user_login"), user_id)
             user_login = json.loads(redis_user_login) if redis_user_login else {}
             if not user_login or TimeHelper.format_time_to_datetime(user_login["ExpireTime"]) < TimeHelper.get_now_datetime():
                 if not is_need_login:
                     return invoke_result
                 self.clear_user_cookie()
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户已过期，请重新登录"
@@ -439,24 +454,24 @@
                 if not is_need_login:
                     return invoke_result
                 self.clear_user_cookie()
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户在其他终端登录，请重新登录"
                 return invoke_result
 
-            curr_user_info = UserInfoModel(config.get_value("manage_context_key")).get_entity_by_id(user_id)
+            curr_user_info = UserInfoModel(config.get_value("manage_context_key", "db_sevenstudio")).get_entity_by_id(user_id)
             if curr_user_info.IsLock == 1:
                 invoke_result.ResultCode = "login_expire"
                 invoke_result.ResultMessage = "用户已被锁，请联系管理员"
                 return invoke_result
 
-            user_login["ExpireTime"] = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire"))
-            self.redis_init().hset(config.get_value("redis_provider_name_user_login"), user_id, self.json_dumps(user_login))
+            user_login["ExpireTime"] = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire", 10))
+            self.redis_init().hset(config.get_value("redis_provider_name_user_login", "user_login"), user_id, self.json_dumps(user_login))
         else:
-            base_manage_context_key = config.get_value("base_manage_context_key")
+            base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
             manage_context_key = self.get_manage_context_key()
 
             user_login_model = UserLoginModel(base_manage_context_key)
             user_login = user_login_model.get_entity_by_id(user_id)
 
             if not user_login or TimeHelper.format_time_to_datetime(user_login.ExpireTime) < TimeHelper.get_now_datetime():
                 if not is_need_login:
@@ -490,15 +505,15 @@
                     invoke_result.ResultMessage = "用户已过期，请重新登录"
                     return invoke_result
                 if curr_user_info.IsLock == 1:
                     invoke_result.ResultCode = "login_expire"
                     invoke_result.ResultMessage = "用户已被锁，请联系管理员"
                     return invoke_result
 
-            user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire"))
+            user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire", 10))
             user_login_model.update_table(f"ExpireTime='{user_login.ExpireTime}'", "UserID=%s", user_login.UserID)
 
         return invoke_result
 
     def login_filter(self, is_need_login, optional_params):
         # sourcery skip: class-extract-method
         """
@@ -513,15 +528,15 @@
         user_id = header_token["UserID"] if header_token.__contains__("UserID") else ""
         user_token = header_token["UserToken"] if header_token.__contains__("UserToken") else ""
         user_id_md5 = header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else ""
         if user_id.strip() == "" or user_token.strip() == "" or user_id_md5.strip() == "":
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
-        if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key")) != user_id_md5:
+        if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key", "7C34A5212F7845CB85D4BBB589502D9B")) != user_id_md5:
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
 
         invoke_result = self.check_login_user(user_id, user_token, is_need_login)
 
         return invoke_result
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/core.py` & `seven_studio-1.4.0/seven_studio/handlers/system/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-03-24 19:48:05
-:LastEditTime: 2023-04-27 18:13:33
+:LastEditTime: 2023-04-28 14:03:41
 :LastEditors: HuangJingCan
 :Description: 
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.libs.geetest import *
 
 from seven_studio.models.db_models.user.user_info_model_ex import *
@@ -24,15 +24,15 @@
 
 class GeetestCodeHandler(StudioBaseHandler):
     """
     :description: 获取极验证的验证码
     """
     def get_async(self):
         user_id = 'test'
-        gt = GeetestLib(config.get_value("pc_geetest_id"), config.get_value("pc_geetest_key"))
+        gt = GeetestLib(config.get_value("pc_geetest_id", "5993a5801d01dd43a07452be135a7381"), config.get_value("pc_geetest_key", "e5bd10f056d92ee46d2ac7cd0356a979"))
         status = gt.pre_process(user_id, JSON_FORMAT=0, ip_address="127.0.0.1")
         if not status:
             status = 2
         response_str = gt.get_response_str()
 
         return self.response_json_success(response_str)
 
@@ -55,15 +55,15 @@
 
         if account == "":
             return self.response_common("EmptyAccount", "对不起，请你输入账号")
 
         if password == "":
             return self.response_common("EmptyPassword", "对不起，请您输入密码")
 
-        if config.get_value("is_captcha_check"):
+        if config.get_value("is_captcha_check", True):
             if challenge == "" or validate == "" or seccode == "":
                 return self.response_common("CaptchaError", "对不起，请先校验验证码")
 
             result = self.check_code(challenge, validate, seccode)
             if not result:
                 return self.response_common("CaptchaError", "对不起，验证码验证失败")
 
@@ -81,29 +81,29 @@
         :description: 验证码校验
         :param challenge：极验证参数challenge
         :param validate：极验证参数validate
         :param seccode：极验证参数seccode
         :return: true or false
         :last_editors: HuangJingCan
         """
-        gt = GeetestLib(config.get_value("pc_geetest_id"), config.get_value("pc_geetest_key"))
+        gt = GeetestLib(config.get_value("pc_geetest_id", "5993a5801d01dd43a07452be135a7381"), config.get_value("pc_geetest_key", "e5bd10f056d92ee46d2ac7cd0356a979"))
         result = gt.success_validate(challenge, validate, seccode, JSON_FORMAT=0)
         return result == 1
 
     def login(self, account="", password="", is_platform=False):
         """
         :description: 登录验证
         :param account：账号
         :param password：密码
         :param is_platform：是否平台用户
         :return: invoke_result
         :last_editors: HuangJingCan
         """
-        manage_context_key = config.get_value("manage_context_key")
-        base_manage_context_key = config.get_value("base_manage_context_key")
+        manage_context_key = config.get_value("manage_context_key", "db_sevenstudio")
+        base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         invoke_result = InvokeResult()
         user_info_model = UserInfoModel(base_manage_context_key)
         user_info = user_info_model.get_entity("Account=%s", params=account)
         if not user_info:
             invoke_result.ResultCode = "NoExistAccount"
             invoke_result.ResultMessage = "账号不存在"
             return invoke_result
@@ -146,15 +146,15 @@
         #     role_user_list = RoleUserModel(manage_context_key).get_list("UserID=%s", params=user_info.UserID)
         #     if len(role_user_list) == 0:
         #         invoke_result.ResultCode = "AccountLock"
         #         invoke_result.ResultMessage = "对不起该账号没有平台管理权限"
         #         return invoke_result
 
         #     role_power_list = RolePowerModelEx(manage_context_key).get_role_power_list([i.RoleID for i in role_user_list])
-        #     if not [i for i in role_power_list if i.MenuID == config.get_value("menu_id_platform")]:
+        #     if not [i for i in role_power_list if i.MenuID == config.get_value("menu_id_platform", "03E5D2A0-DB59-47F6-8F10-1ACDEFE9BDDD")]:
         #         invoke_result.ResultCode = "AccountLock"
         #         invoke_result.ResultMessage = "对不起该账号没有平台管理权限"
         #         return invoke_result
 
         user_info.FaildLoginCount = 0
         user_info.LoginDate = TimeHelper.get_now_datetime()
         user_info.LoginIP = self.get_remote_ip()
@@ -171,17 +171,17 @@
         :description: 登录状态设置
         :param user_info：当前登录用户信息
         :return: user_login
         :last_editors: HuangJingCan
         """
         user_login = UserLogin()
         user_login.UserID = user_info.UserID
-        user_login.UserIDMD5 = CryptoHelper.md5_encrypt(user_info.UserID, config.get_value("login_encrypt_key"))
+        user_login.UserIDMD5 = CryptoHelper.md5_encrypt(user_info.UserID, config.get_value("login_encrypt_key", "7C34A5212F7845CB85D4BBB589502D9B"))
         user_login.UserToken = UUIDHelper.get_uuid()
-        user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire"))
+        user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire", 10))
 
         self.login_cookie(user_login)
 
         return user_login
 
 
 class LogoutHandler(StudioBaseHandler):
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/file.py` & `seven_studio-1.4.0/seven_studio/handlers/system/file.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/menu.py` & `seven_studio-1.4.0/seven_studio/handlers/system/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: dongyu
 :Date: 2020-04-11 18:44:08
-:LastEditTime: 2023-02-08 16:50:13
+:LastEditTime: 2023-04-28 13:51:41
 :LastEditors: HuangJingCan
 :Description: 菜单相关类
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.models.db_models.menu.menu_cote_model import *
 from seven_studio.models.db_models.menu.menu_info_model_ex import *
 from seven_studio.models.power_model import *
@@ -53,22 +53,22 @@
         :last_editors: HuangJingCan
         """
         manage_context_key = self.get_manage_context_key()
         is_super = self.get_is_super()
         curr_user_id = self.request_user_id()
         product_id = self.request_product_id()
         # 是否权限无限下放（0-无限等级，1-下放一级）
-        power_grade = int(config.get_value("power_grade", 0))
+        power_grade = int(config.get_value("power_grade", 1))
 
         power_model = PowerModel(manage_context_key, is_super, curr_user_id, product_id)
         result = power_model.get_menu_item_tree()
 
         # 非超管则无权限下放功能，没有用户和角色添加权限
         if not is_super and power_grade > 0:
-            result = [i for i in result if i['MenuID'] != config.get_value("menu_id_platform")]
+            result = [i for i in result if i['MenuID'] != config.get_value("menu_id_platform", "03E5D2A0-DB59-47F6-8F10-1ACDEFE9BDDD")]
 
         return self.response_json_success(result)
 
 
 class MenuTreeHandler(StudioBaseHandler):
     """
     :description: 系统菜单路由
@@ -462,15 +462,15 @@
         # 栏目ID
         menu_id = self.get_param("menuID")
         if menu_id == "":
             return self.response_common("MenuIDEmpty", "栏目ID为空")
 
         sql = PowerModel().export_sql(menu_id)
 
-        sql_file_name = config.get_value("export_sql_folder") + "SyncSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
+        sql_file_name = config.get_value("export_sql_folder", "c:\\") + "SyncSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
         with open(sql_file_name, 'a') as file_handle:
             file_handle.write("{}\n".format(sql))
 
         return self.response_json_success()
 
 
 class InsertSqlHandler(StudioBaseHandler):
@@ -486,15 +486,15 @@
         """
         menu_id = self.get_param("menuID")
         if menu_id == "":
             return self.response_common("MenuIDEmpty", "栏目ID为空")
 
         sql = PowerModel().export_sql(menu_id, 1)
 
-        sql_file_name = config.get_value("export_sql_folder") + "InsertSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
+        sql_file_name = config.get_value("export_sql_folder", "c:\\") + "InsertSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
         with open(sql_file_name, 'a') as file_handle:
             file_handle.write("{}\n".format(sql))
 
         return self.response_json_success()
 
 
 class UpdateSqlHandler(StudioBaseHandler):
@@ -510,12 +510,12 @@
         """
         menu_id = self.get_param("menuID")
         if menu_id == "":
             return self.response_common("MenuIDEmpty", "栏目ID为空")
 
         sql = PowerModel().export_sql(menu_id, 2)
 
-        sql_file_name = config.get_value("export_sql_folder") + "UpdateSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
+        sql_file_name = config.get_value("export_sql_folder", "c:\\") + "UpdateSql" + TimeHelper.get_now_format_time("%Y-%m-%d") + ".sql"
         with open(sql_file_name, 'a') as file_handle:
             file_handle.write("{}\n".format(sql))
 
         return self.response_json_success()
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/power.py` & `seven_studio-1.4.0/seven_studio/handlers/system/power.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: wang kui
 :Date: 2020-03-24 16:32:52
-:LastEditTime: 2023-04-10 15:18:57
+:LastEditTime: 2023-04-28 13:55:49
 :LastEditors: HuangJingCan
 :Description: power 用户权限相关接口
 """
 from seven_studio.handlers.studio_base import *
 from seven_studio.utils.dict import *
 
 from seven_studio.models.db_models.product.product_info_model import *
@@ -57,15 +57,15 @@
         :description: 获取用户产品列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
         user_id = self.request_user_id()
         product_id = self.request_product_id()
-        base_manage_context_key = config.get_value("base_manage_context_key")
+        base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         product_info_model = ProductInfoModel(base_manage_context_key)
         product_user_model = ProductUserModel(base_manage_context_key)
         product_data = []
         product_infos = []
         home_info = {"Title": "平台管理", "ImageUrl": "", "ManageUrl": "", "WebUrl": "", "ProductID": 0}
         is_super = self.get_is_super()
 
@@ -104,17 +104,19 @@
         has_role_manage = False
         if is_super:
             has_user_manage = True
             has_role_manage = True
         else:
             role_user_list = RoleUserModel(product_info.ManageContextKey).get_list("UserID=%s", params=user_id)
             role_power_list = RolePowerModelEx(product_info.ManageContextKey).get_role_power_list([i.RoleID for i in role_user_list])
-            if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_user")]:
+            # 用户管理
+            if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_user", "80ce2364-368f-47ac-98c8-819fcb521bab")]:
                 has_user_manage = True
-            if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_role")]:
+            # 角色管理
+            if [i for i in role_power_list if i.MenuID == config.get_value("menu_id_role", "47a90fe3-012b-49b6-af27-5293124ce827")]:
                 has_role_manage = True
 
         return {
             "Title": product_info.ProductName,
             "SubTitle": product_info.ProductSubName,
             "ImageUrl": product_info.ImageUrl,
             "ManageUrl": product_info.ManageUrl,
@@ -131,26 +133,26 @@
         :param user_info：用户信息
         :return: 
         :last_editors: HuangJingCan
         """
         invoke_result = InvokeResult()
         invoke_result.ResultCode = "AccountLock"
         invoke_result.ResultMessage = "对不起该账号没有平台管理权限"
-        context_key = config.get_value("base_manage_context_key")
+        context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         user_info_model_ex = UserInfoModel(context_key)
         base_user_info = user_info_model_ex.get_entity_by_id(user_info.UserID)
         if not base_user_info:
             return invoke_result
         if base_user_info.IsSuper == 1:
             return InvokeResult()
         role_user_list = RoleUserModel(context_key).get_list("UserID=%s", params=self.request_user_id())
         if not role_user_list:
             return invoke_result
         role_power_list = RolePowerModelEx(context_key).get_role_power_list([i.RoleID for i in role_user_list])
-        role_power_info = [i for i in role_power_list if i.MenuID == config.get_value("menu_id_platform")]
+        role_power_info = [i for i in role_power_list if i.MenuID == config.get_value("menu_id_platform", "03E5D2A0-DB59-47F6-8F10-1ACDEFE9BDDD")]
 
         return InvokeResult() if role_power_info else invoke_result
 
 
 class FocusPasswordHandler(StudioBaseHandler):
     """
     :description: 强制修改密码弹窗
@@ -184,15 +186,15 @@
         :return: 
         :last_editors: HuangJingCan
         """
         # 密码
         password = self.get_param("password")
 
         invoke_result = InvokeResult()
-        user_info_model_ex = UserInfoModel(config.get_value("base_manage_context_key"))
+        user_info_model_ex = UserInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
         user_info_ex = UserInfoModelEx()
         base_user_info = self.get_base_user_info()
 
         user_id = base_user_info.UserID if base_user_info else ""
         is_force_password = user_info_ex.is_force_password(base_user_info)
         if not is_force_password:
             return self.response_common("Error", "无需强制更改密码")
@@ -219,15 +221,15 @@
         """
         # 旧密码
         password = self.get_param("Password")
         # 新密码
         new_password = self.get_param("NewPassword")
 
         invoke_result = InvokeResult()
-        user_info_model_ex = UserInfoModelEx(config.get_value("base_manage_context_key"))
+        user_info_model_ex = UserInfoModelEx(config.get_value("base_manage_context_key", "db_sevenstudio"))
         base_user_info = self.get_base_user_info()
 
         user_id = base_user_info.UserID if base_user_info else ""
         if not user_info_model_ex.verify_password(password, base_user_info.Password, user_id):
             return self.response_common("ErrorPassword", "旧密码错误，请重新输入")
 
         sign_password = user_info_model_ex.sign_password(new_password, user_id)
@@ -374,15 +376,15 @@
 
         user_ids_list = [i.UserID for i in page_list]
         user_ids_str = str(user_ids_list).strip('[').strip(']')
         role_user_list = RoleUserModel(manage_context_key).get_list(f"UserID IN({user_ids_str})")
 
         product_user_list = []
         if product_id == 0:
-            product_user_list = ProductUserModel(config.get_value("base_manage_context_key")).get_list(f"UserID IN({user_ids_str})")
+            product_user_list = ProductUserModel(config.get_value("base_manage_context_key", "db_sevenstudio")).get_list(f"UserID IN({user_ids_str})")
 
         for curr_user_info in page_list:
             curr_user_role_dto = DictUtil.auto_mapper(UserRoleDto(), curr_user_info.__dict__)
             curr_user_role_dto.UserRoleIds = [i.RoleID for i in role_user_list if i.UserID == curr_user_info.UserID]
             if product_id == 0:
                 curr_user_role_dto.UserProductIds = [i.ProductID for i in product_user_list if i.UserID == curr_user_info.UserID]
             chief_user_info = [i for i in chief_user_info_list if curr_user_info.ChiefUserID and i.UserID == curr_user_info.ChiefUserID]
@@ -766,15 +768,15 @@
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
         # 用户id
         user_id = self.get_param("UserID")
         # 数据库连接串
-        base_manage_context_key = config.get_value("base_manage_context_key")
+        base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         # 当前用户id
         curr_user_id = self.request_user_id()
         # 是否超管
         is_super = self.get_is_super()
 
         user_info_model = UserInfoModel(base_manage_context_key)
         user_info = UserInfoModel(base_manage_context_key).get_entity_by_id(user_id)
@@ -805,15 +807,15 @@
         :description: 登录失败重置
         :param {type}
         :return:
         :last_editors: HuangJingCan
         """
         user_id = self.get_param("UserID")
         # 数据库连接串
-        base_manage_context_key = config.get_value("base_manage_context_key")
+        base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         # 当前用户id
         curr_user_id = self.request_user_id()
         # 是否超管
         is_super = self.get_is_super()
 
         user_info_model = UserInfoModel(base_manage_context_key)
         user_info = UserInfoModel(base_manage_context_key).get_entity_by_id(user_id)
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/product.py` & `seven_studio-1.4.0/seven_studio/handlers/system/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJingCan
 :Date: 2020-04-22 14:32:40
-:LastEditTime: 2023-02-07 14:59:25
+:LastEditTime: 2023-04-28 11:44:06
 :LastEditors: HuangJingCan
 :Description: 产品相关Handler
 """
 
 from seven_studio.handlers.studio_base import *
 from seven_studio.models.db_models.product.product_info_model import *
 from seven_studio.models.db_models.product.product_user_model import *
@@ -22,15 +22,15 @@
         """
         :description: 产品列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
         # 数据库连接串
-        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key"))
+        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
         # 页索引
         page_index = self.get_page_index()
         # 页大小
         page_size = self.get_page_size()
         # 查询条件,排序字段
         condition, order = self.get_condition_by_body()
 
@@ -51,15 +51,15 @@
     def get_async(self):
         """
         :description: 全部产品列表
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
-        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key"))
+        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
         source_dict_list = product_info_model.get_dict_list()
 
         return self.response_json_success(source_dict_list)
 
 
 class SaveProductHandler(StudioBaseHandler):
     """
@@ -71,15 +71,15 @@
         """
         :description: 保存产品
         :param {type} 
         :return: 
         :last_editors: HuangJingCan
         """
         # 数据库连接串
-        base_manage_context_key = config.get_value("base_manage_context_key")
+        base_manage_context_key = config.get_value("base_manage_context_key", "db_sevenstudio")
         # 产品id
         product_id = int(self.get_param("ProductID", "0"))
         # 产品名称
         product_name = self.get_param("ProductName")
         # 产品子名称
         product_sub_name = self.get_param("ProductSubName")
         # 业务地址
@@ -170,12 +170,12 @@
         :last_editors: HuangJingCan
         """
         product_id = int(self.get_param("ProductID", 0))
 
         if product_id <= 0:
             return self.response_json_error_params()
 
-        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key"))
+        product_info_model = ProductInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
 
         product_info_model.del_entity("ProductID=%s", product_id)
 
         return self.response_json_success()
```

### Comparing `seven_studio-1.3.2/seven_studio/handlers/system/settings.py` & `seven_studio-1.4.0/seven_studio/handlers/system/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 :Author: ChenXiaolei
 :Date: 2020-12-09 19:11:51
-:LastEditTime: 2022-12-08 10:13:51
+:LastEditTime: 2023-04-28 13:36:44
 :LastEditors: HuangJingCan
 :Description: 
 """
 
 from seven_studio.handlers.studio_base import *
 from seven_studio.models.db_models.settings.settings_base_model import *
 
@@ -26,15 +26,15 @@
         # 首页顶部logo
         banner_logo = self.get_param("banner_logo")
         # 标题
         title = self.get_param("title")
         # 登录过期时间(小时)
         login_expire = int(self.get_param("login_expire", 2))
 
-        settings_base_model = SettingsBaseModel(config.get_value("manage_context_key"))
+        settings_base_model = SettingsBaseModel(config.get_value("manage_context_key", "db_sevenstudio"))
 
         settings_base = settings_base_model.get_entity()
 
         if not settings_base:
             settings_base = SettingsBase()
 
         settings_base.login_background = login_background
@@ -44,30 +44,30 @@
         settings_base.login_expire = login_expire
 
         if settings_base.id > 0:
             settings_base_model.update_entity(settings_base)
         else:
             settings_base_model.add_entity(settings_base)
 
-        if config.get_value("login_type") == "redis":
+        if config.get_value("login_type", "redis") == "redis":
             redis_init = self.redis_init()
             settings_base = redis_init.delete("settings_base")
 
         return self.response_json_success(settings_base)
 
     def get_async(self):
         """
         :description: 获取站点基础信息
         :return 基础信息
         :last_editors: ChenXiaolei
         """
-        settings_base_model = SettingsBaseModel(config.get_value("manage_context_key"))
+        settings_base_model = SettingsBaseModel(config.get_value("manage_context_key", "db_sevenstudio"))
 
         settings_base = None
-        if config.get_value("login_type") == "redis":
+        if config.get_value("login_type", "redis") == "redis":
             redis_init = self.redis_init()
             settings_base = redis_init.get("settings_base")
             if not settings_base:
                 settings_base = settings_base_model.get_dict()
                 redis_init.set("settings_base", self.json_dumps(settings_base))
             else:
                 settings_base = self.json_loads(settings_base)
```

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/bos.py` & `seven_studio-1.4.0/seven_studio/libs/file/bos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/cos.py` & `seven_studio-1.4.0/seven_studio/libs/file/cos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/ks3.py` & `seven_studio-1.4.0/seven_studio/libs/file/ks3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/oss2.py` & `seven_studio-1.4.0/seven_studio/libs/file/oss2.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/s3.py` & `seven_studio-1.4.0/seven_studio/libs/file/s3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/file/upload.py` & `seven_studio-1.4.0/seven_studio/libs/file/upload.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/libs/geetest.py` & `seven_studio-1.4.0/seven_studio/libs/geetest.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_history_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_history_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_resource_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_resource_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_restrict_pic_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_pic_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_storage_path_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_storage_path_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/file/file_water_image_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/file/file_water_image_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/log/log_action_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/log/log_action_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_cote_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_cote_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/menu/menu_info_model_ex.py` & `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/product/product_info_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/product/product_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/product/product_user_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/product/product_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/role/role_info_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/role/role_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/role/role_power_model_ex.py` & `seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/role/role_user_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/role/role_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/settings/settings_base_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/settings/settings_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/user/user_info_model_ex.py` & `seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model_ex.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from seven_studio.models.db_models.user.user_info_model import *
 from seven_framework.crypto import *
 
 
 class UserInfoModelEx(UserInfoModel):
     def __init__(self, db_connect_key='db_sevenstudio', sub_table=None, db_transaction=None):
         super().__init__(db_connect_key=db_connect_key, sub_table=sub_table)
+
     def sign_password(self, login_password="", userid=""):
         if login_password.strip() == '':
-            return CryptoHelper.md5_encrypt(config.get_value("default_password"), userid)
+            return CryptoHelper.md5_encrypt(config.get_value("default_password", "7777777"), userid)
         return CryptoHelper.md5_encrypt(login_password, userid).upper()
 
     def verify_password(self, login_password="", password="", userid=""):
         return password.upper() == CryptoHelper.md5_encrypt(login_password, userid).upper()
 
     def is_force_password(self, user_info):
         if user_info:
-            return self.verify_password(config.get_value("default_password"), user_info.Password, user_info.UserID)
+            return self.verify_password(config.get_value("default_password", "7777777"), user_info.Password, user_info.UserID)
         return False
```

### Comparing `seven_studio-1.3.2/seven_studio/models/db_models/user/user_login_model.py` & `seven_studio-1.4.0/seven_studio/models/db_models/user/user_login_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/dto_model.py` & `seven_studio-1.4.0/seven_studio/models/dto_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/enum.py` & `seven_studio-1.4.0/seven_studio/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/models/power_model.py` & `seven_studio-1.4.0/seven_studio/models/power_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: HuangJingCan
 :Date: 2020-04-15 09:56:24
-:LastEditTime: 2023-02-08 17:30:15
+:LastEditTime: 2023-04-28 13:51:57
 :LastEditors: HuangJingCan
 :Description: 权限角色栏目相关
 """
 from asq.initiators import query
 from seven_studio.utils.dict import *
 from seven_framework.time import *
 
@@ -66,15 +66,15 @@
         :return: 
         :last_editors: HuangJingCan
         """
         menu_info_list = self.get_power_menu_list()
         menu_item_list = []
 
         # 平台管理权限
-        # menu_info_list_plat = [i for i in menu_info_list if i.MenuType == 1 and i.MenuID == config.get_value("menu_id_platform")]
+        # menu_info_list_plat = [i for i in menu_info_list if i.MenuType == 1 and i.MenuID == config.get_value("menu_id_platform", "03E5D2A0-DB59-47F6-8F10-1ACDEFE9BDDD")]
         menu_info_list_plat = [i for i in menu_info_list if i.MenuType == 1]
         for menu_info in menu_info_list_plat:
             curr_menu_item_dto = PowerMenuInfoDto()
             curr_menu_item_dto.MenuID = menu_info.MenuID
             curr_menu_item_dto.MenuName = menu_info.MenuName
             curr_menu_item_dto.MenuIcon = menu_info.MenuIcon
             curr_menu_item_dto.ApiPath = menu_info.ApiPathValue
@@ -591,15 +591,15 @@
         :param password: 密码
         :param change_pw: 修改密码
         :param is_add: 是否添加
         :return: 
         :last_editors: HuangJingCan
         """
         user_info_model = UserInfoModel(self.db_connect_key)
-        base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key"))
+        base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
         role_id_list = [i for i in role_id_list if i != ""]
         product_id_list = [i for i in product_id_list if i != ""]
         update_field = ["IsSuper", "Account", "Email", "LoginIP", "PasswordQuestion", "PasswordAnswer", "IsLock", "FaildLoginCount", "FaildQuestionCount", "UserName", "NickName", "JobNo", "Avatar", "LoginDate", "Phone", "PersonalitySignature", "ChiefUserID"]
 
         if change_pw:
             update_field.append("Password")
         if is_add:
@@ -610,15 +610,15 @@
                 user_info.UserID = UUIDHelper.get_uuid()
                 base_user_info_model.add_entity(user_info)
             user_info_model.add_entity(user_info, True)
             
             if change_pw:
                 user_info.Password = UserInfoModelEx().sign_password(password, user_info.UserID)
             else:
-                user_info.Password = UserInfoModelEx().sign_password(config.get_value("default_password"))
+                user_info.Password = UserInfoModelEx().sign_password(config.get_value("default_password", "7777777"))
         elif change_pw:
             user_info.Password = UserInfoModelEx().sign_password(password, user_info.UserID)
 
         user_info_model.update_entity(user_info, field_list=update_field)
         base_user_info_model.update_table("Password=%s", "UserID=%s", params=[user_info.Password, user_info.UserID])
 
         if role_id_list:
@@ -658,15 +658,15 @@
         """
         :description: 添加产品用户
         :param user_id: 用户id
         :param role_id_list: 产品id列表
         :return: 
         :last_editors: HuangJingCan
         """
-        product_user_model = ProductUserModel(config.get_value("base_manage_context_key"))
+        product_user_model = ProductUserModel(config.get_value("base_manage_context_key", "db_sevenstudio"))
         product_user_model.del_entity("UserID=%s", user_id)
         if len(product_id_list) > 0:
             product_user_list = []
             for product_id in product_id_list:
                 product_user = ProductUser()
                 product_user.UserID = user_id
                 product_user.ProductID = product_id
@@ -677,16 +677,16 @@
         """
         :description: 子产品将用户同步回主库之中
         :param user_info: 用户信息
         :return: 
         :last_editors: HuangJingCan
         """
         if self.product_id > 0:
-            base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key"), "")
-            base_product_user_model = ProductUserModel(config.get_value("base_manage_context_key"), "")
+            base_user_info_model = UserInfoModel(config.get_value("base_manage_context_key"), "db_sevenstudio")
+            base_product_user_model = ProductUserModel(config.get_value("base_manage_context_key"), "db_sevenstudio")
 
             base_product_user = base_product_user_model.get_entity("ProductID=%s and UserID=%s", params=[self.product_id, user_info.UserID])
 
             if not base_product_user:
                 product_user = ProductUser()
                 product_user.ProductID = self.product_id
                 product_user.UserID = user_info.UserID
```

### Comparing `seven_studio-1.3.2/seven_studio/models/seven_model.py` & `seven_studio-1.4.0/seven_studio/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/route.py` & `seven_studio-1.4.0/seven_studio/route.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/utils/dict.py` & `seven_studio-1.4.0/seven_studio/utils/dict.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio/utils/random.py` & `seven_studio-1.4.0/seven_studio/utils/random.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.3.2/seven_studio.egg-info/PKG-INFO` & `seven_studio-1.4.0/seven_studio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: seven-studio
-Version: 1.3.2
+Version: 1.4.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
-Description: 
-        
-        <!--
+Description: <!--
          * @Author: ChenXiaolei
          * @Date: 2022-01-18 18:52:26
          * @LastEditTime: 2022-11-22 16:41:30
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.4.0 更新内容
+        * 优化配置文件
+        * 修改json_dumps
+        
         ### 1.3.2 更新内容
         * 登录问题修改
         
         ### 1.2.0 更新内容
         * GetUserInfoHandler增加字段返回
         
         ### 1.1.9 更新内容
```

### Comparing `seven_studio-1.3.2/seven_studio.egg-info/SOURCES.txt` & `seven_studio-1.4.0/seven_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

