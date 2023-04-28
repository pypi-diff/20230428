# Comparing `tmp/alibabacloud_dingtalk-2.0.0.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.0.tar", last modified: Wed Apr 26 03:28:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.10.tar", last modified: Fri Apr 28 03:36:56 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.0.tar` & `alibabacloud_dingtalk-2.0.10.tar`

### file list

```diff
@@ -1,353 +1,353 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/
--rw-r--r--   0 root         (0) root         (0)    19169 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2308 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148888 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   274521 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   565599 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138334 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   325906 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34674 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   100519 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387928 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   511378 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267841 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   308062 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   429056 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89334 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133902 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86020 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    88139 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87266 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130480 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129226 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157291 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260566 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   403692 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10094 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26851 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   147980 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   459526 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   682489 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2308 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11618 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-04-26 03:28:00.000000 alibabacloud_dingtalk-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/
+-rw-r--r--   0 root         (0) root         (0)    19297 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148888 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   274109 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   565599 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138548 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   328853 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34674 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   100519 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387928 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   511378 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   308062 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   429056 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89334 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133902 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87266 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130480 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129226 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157291 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260594 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   414815 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10094 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26851 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   147980 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175082 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   370377 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   459526 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   682489 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11618 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-04-28 03:36:56.000000 alibabacloud_dingtalk-2.0.10/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.0/ChangeLog.md` & `alibabacloud_dingtalk-2.0.10/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2023-04-26 Version: 2.0.0
+- Update AddOfficialAccountFollower.
+
+2023-04-26 Version: 2.0.0
+- Update AddOfficialAccountFollower.
+
 2023-04-21 Version: 1.5.65
 - Update AddOfficialAccountFollower.
 
 2023-04-14 Version: 1.5.64
 - Update AddOfficialAccountFollower.
 
 2023-04-11 Version: 1.5.63
```

### Comparing `alibabacloud_dingtalk-2.0.0/LICENSE` & `alibabacloud_dingtalk-2.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/PKG-INFO` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dingtalk
-Version: 2.0.0
+Name: alibabacloud-dingtalk
+Version: 2.0.10
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.0/README-CN.md` & `alibabacloud_dingtalk-2.0.10/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/README.md` & `alibabacloud_dingtalk-2.0.10/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2632,43 +2632,37 @@
             self.total_page = m.get('totalPage')
         return self
 
 
 class GetAdjustmentsResponseBody(TeaModel):
     def __init__(
         self,
-        result: List[GetAdjustmentsResponseBodyResult] = None,
+        result: GetAdjustmentsResponseBodyResult = None,
     ):
         self.result = result
 
     def validate(self):
         if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['result'] = []
         if self.result is not None:
-            for k in self.result:
-                result['result'].append(k.to_map() if k else None)
+            result['result'] = self.result.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.result = []
         if m.get('result') is not None:
-            for k in m.get('result'):
-                temp_model = GetAdjustmentsResponseBodyResult()
-                self.result.append(temp_model.from_map(k))
+            temp_model = GetAdjustmentsResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
         return self
 
 
 class GetAdjustmentsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -4966,43 +4960,37 @@
             self.total_page = m.get('totalPage')
         return self
 
 
 class GetSimpleOvertimeSettingResponseBody(TeaModel):
     def __init__(
         self,
-        result: List[GetSimpleOvertimeSettingResponseBodyResult] = None,
+        result: GetSimpleOvertimeSettingResponseBodyResult = None,
     ):
         self.result = result
 
     def validate(self):
         if self.result:
-            for k in self.result:
-                if k:
-                    k.validate()
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['result'] = []
         if self.result is not None:
-            for k in self.result:
-                result['result'].append(k.to_map() if k else None)
+            result['result'] = self.result.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.result = []
         if m.get('result') is not None:
-            for k in m.get('result'):
-                temp_model = GetSimpleOvertimeSettingResponseBodyResult()
-                self.result.append(temp_model.from_map(k))
+            temp_model = GetSimpleOvertimeSettingResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
         return self
 
 
 class GetSimpleOvertimeSettingResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,14 +529,16 @@
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
+        if not UtilClient.is_unset(request.ui_configs):
+            body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -586,14 +588,16 @@
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
             body['summary'] = request.summary
+        if not UtilClient.is_unset(request.ui_configs):
+            body['uiConfigs'] = request.ui_configs
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1120,40 +1120,75 @@
         if m.get('dateTime') is not None:
             self.date_time = m.get('dateTime')
         if m.get('timeZone') is not None:
             self.time_zone = m.get('timeZone')
         return self
 
 
+class CreateEventRequestUiConfigs(TeaModel):
+    def __init__(
+        self,
+        ui_name: str = None,
+        ui_status: str = None,
+    ):
+        self.ui_name = ui_name
+        self.ui_status = ui_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ui_name is not None:
+            result['uiName'] = self.ui_name
+        if self.ui_status is not None:
+            result['uiStatus'] = self.ui_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uiName') is not None:
+            self.ui_name = m.get('uiName')
+        if m.get('uiStatus') is not None:
+            self.ui_status = m.get('uiStatus')
+        return self
+
+
 class CreateEventRequest(TeaModel):
     def __init__(
         self,
         attendees: List[CreateEventRequestAttendees] = None,
         description: str = None,
         end: CreateEventRequestEnd = None,
         extra: Dict[str, str] = None,
         is_all_day: bool = None,
         location: CreateEventRequestLocation = None,
         online_meeting_info: CreateEventRequestOnlineMeetingInfo = None,
         recurrence: CreateEventRequestRecurrence = None,
         reminders: List[CreateEventRequestReminders] = None,
         start: CreateEventRequestStart = None,
         summary: str = None,
+        ui_configs: List[CreateEventRequestUiConfigs] = None,
     ):
         self.attendees = attendees
         self.description = description
         self.end = end
         self.extra = extra
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.recurrence = recurrence
         self.reminders = reminders
         self.start = start
         self.summary = summary
+        self.ui_configs = ui_configs
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
         if self.end:
@@ -1166,14 +1201,18 @@
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.start:
             self.start.validate()
+        if self.ui_configs:
+            for k in self.ui_configs:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1199,14 +1238,18 @@
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
+        result['uiConfigs'] = []
+        if self.ui_configs is not None:
+            for k in self.ui_configs:
+                result['uiConfigs'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
@@ -1236,14 +1279,19 @@
                 temp_model = CreateEventRequestReminders()
                 self.reminders.append(temp_model.from_map(k))
         if m.get('start') is not None:
             temp_model = CreateEventRequestStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
+        self.ui_configs = []
+        if m.get('uiConfigs') is not None:
+            for k in m.get('uiConfigs'):
+                temp_model = CreateEventRequestUiConfigs()
+                self.ui_configs.append(temp_model.from_map(k))
         return self
 
 
 class CreateEventResponseBodyAttendees(TeaModel):
     def __init__(
         self,
         display_name: str = None,
@@ -1646,14 +1694,47 @@
         if m.get('dateTime') is not None:
             self.date_time = m.get('dateTime')
         if m.get('timeZone') is not None:
             self.time_zone = m.get('timeZone')
         return self
 
 
+class CreateEventResponseBodyUiConfigs(TeaModel):
+    def __init__(
+        self,
+        ui_name: str = None,
+        ui_status: str = None,
+    ):
+        self.ui_name = ui_name
+        self.ui_status = ui_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ui_name is not None:
+            result['uiName'] = self.ui_name
+        if self.ui_status is not None:
+            result['uiStatus'] = self.ui_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uiName') is not None:
+            self.ui_name = m.get('uiName')
+        if m.get('uiStatus') is not None:
+            self.ui_status = m.get('uiStatus')
+        return self
+
+
 class CreateEventResponseBody(TeaModel):
     def __init__(
         self,
         attendees: List[CreateEventResponseBodyAttendees] = None,
         create_time: str = None,
         description: str = None,
         end: CreateEventResponseBodyEnd = None,
@@ -1662,14 +1743,15 @@
         location: CreateEventResponseBodyLocation = None,
         online_meeting_info: CreateEventResponseBodyOnlineMeetingInfo = None,
         organizer: CreateEventResponseBodyOrganizer = None,
         recurrence: CreateEventResponseBodyRecurrence = None,
         reminders: List[CreateEventResponseBodyReminders] = None,
         start: CreateEventResponseBodyStart = None,
         summary: str = None,
+        ui_configs: List[CreateEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
         self.create_time = create_time
         self.description = description
         self.end = end
         self.id = id
@@ -1677,14 +1759,15 @@
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.recurrence = recurrence
         self.reminders = reminders
         self.start = start
         self.summary = summary
+        self.ui_configs = ui_configs
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
@@ -1700,14 +1783,18 @@
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.start:
             self.start.validate()
+        if self.ui_configs:
+            for k in self.ui_configs:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1737,14 +1824,18 @@
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.summary is not None:
             result['summary'] = self.summary
+        result['uiConfigs'] = []
+        if self.ui_configs is not None:
+            for k in self.ui_configs:
+                result['uiConfigs'].append(k.to_map() if k else None)
         if self.update_time is not None:
             result['updateTime'] = self.update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
@@ -1781,14 +1872,19 @@
                 temp_model = CreateEventResponseBodyReminders()
                 self.reminders.append(temp_model.from_map(k))
         if m.get('start') is not None:
             temp_model = CreateEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('summary') is not None:
             self.summary = m.get('summary')
+        self.ui_configs = []
+        if m.get('uiConfigs') is not None:
+            for k in m.get('uiConfigs'):
+                temp_model = CreateEventResponseBodyUiConfigs()
+                self.ui_configs.append(temp_model.from_map(k))
         if m.get('updateTime') is not None:
             self.update_time = m.get('updateTime')
         return self
 
 
 class CreateEventResponse(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1398,14 +1398,47 @@
         if m.get('deptId') is not None:
             self.dept_id = m.get('deptId')
         if m.get('deptName') is not None:
             self.dept_name = m.get('deptName')
         return self
 
 
+class TeamVOShareScopeInfo(TeaModel):
+    def __init__(
+        self,
+        role_id: str = None,
+        scope: int = None,
+    ):
+        self.role_id = role_id
+        self.scope = scope
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.role_id is not None:
+            result['roleId'] = self.role_id
+        if self.scope is not None:
+            result['scope'] = self.scope
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('roleId') is not None:
+            self.role_id = m.get('roleId')
+        if m.get('scope') is not None:
+            self.scope = m.get('scope')
+        return self
+
+
 class TeamVOUpdater(TeaModel):
     def __init__(
         self,
         name: str = None,
         union_id: str = None,
     ):
         self.name = name
@@ -1469,14 +1502,15 @@
         created_time: int = None,
         creator: TeamVOCreator = None,
         description: str = None,
         icon: str = None,
         id: str = None,
         name: str = None,
         related_dept_info: TeamVORelatedDeptInfo = None,
+        share_scope_info: TeamVOShareScopeInfo = None,
         status: int = None,
         type: int = None,
         updated_time: int = None,
         updater: TeamVOUpdater = None,
         url: str = None,
         visit_info: TeamVOVisitInfo = None,
     ):
@@ -1484,26 +1518,29 @@
         self.created_time = created_time
         self.creator = creator
         self.description = description
         self.icon = icon
         self.id = id
         self.name = name
         self.related_dept_info = related_dept_info
+        self.share_scope_info = share_scope_info
         self.status = status
         self.type = type
         self.updated_time = updated_time
         self.updater = updater
         self.url = url
         self.visit_info = visit_info
 
     def validate(self):
         if self.creator:
             self.creator.validate()
         if self.related_dept_info:
             self.related_dept_info.validate()
+        if self.share_scope_info:
+            self.share_scope_info.validate()
         if self.updater:
             self.updater.validate()
         if self.visit_info:
             self.visit_info.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -1523,14 +1560,16 @@
             result['icon'] = self.icon
         if self.id is not None:
             result['id'] = self.id
         if self.name is not None:
             result['name'] = self.name
         if self.related_dept_info is not None:
             result['relatedDeptInfo'] = self.related_dept_info.to_map()
+        if self.share_scope_info is not None:
+            result['shareScopeInfo'] = self.share_scope_info.to_map()
         if self.status is not None:
             result['status'] = self.status
         if self.type is not None:
             result['type'] = self.type
         if self.updated_time is not None:
             result['updatedTime'] = self.updated_time
         if self.updater is not None:
@@ -1557,14 +1596,17 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('relatedDeptInfo') is not None:
             temp_model = TeamVORelatedDeptInfo()
             self.related_dept_info = temp_model.from_map(m['relatedDeptInfo'])
+        if m.get('shareScopeInfo') is not None:
+            temp_model = TeamVOShareScopeInfo()
+            self.share_scope_info = temp_model.from_map(m['shareScopeInfo'])
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('type') is not None:
             self.type = m.get('type')
         if m.get('updatedTime') is not None:
             self.updated_time = m.get('updatedTime')
         if m.get('updater') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1910,7 +1910,105 @@
     async def update_group_owner_async(
         self,
         request: dingtalkimpaas__1__0_models.UpdateGroupOwnerRequest,
     ) -> dingtalkimpaas__1__0_models.UpdateGroupOwnerResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkimpaas__1__0_models.UpdateGroupOwnerHeaders()
         return await self.update_group_owner_with_options_async(request, headers, runtime)
+
+    def upload_file_with_options(
+        self,
+        request: dingtalkimpaas__1__0_models.UploadFileRequest,
+        headers: dingtalkimpaas__1__0_models.UploadFileHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkimpaas__1__0_models.UploadFileResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.file_name):
+            body['fileName'] = request.file_name
+        if not UtilClient.is_unset(request.file_type):
+            body['fileType'] = request.file_type
+        if not UtilClient.is_unset(request.file_url):
+            body['fileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.sender_uid):
+            body['senderUid'] = request.sender_uid
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UploadFile',
+            version='impaas_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/impaas/interconnections/files/upload',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkimpaas__1__0_models.UploadFileResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def upload_file_with_options_async(
+        self,
+        request: dingtalkimpaas__1__0_models.UploadFileRequest,
+        headers: dingtalkimpaas__1__0_models.UploadFileHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkimpaas__1__0_models.UploadFileResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.file_name):
+            body['fileName'] = request.file_name
+        if not UtilClient.is_unset(request.file_type):
+            body['fileType'] = request.file_type
+        if not UtilClient.is_unset(request.file_url):
+            body['fileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.sender_uid):
+            body['senderUid'] = request.sender_uid
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UploadFile',
+            version='impaas_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/impaas/interconnections/files/upload',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkimpaas__1__0_models.UploadFileResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def upload_file(
+        self,
+        request: dingtalkimpaas__1__0_models.UploadFileRequest,
+    ) -> dingtalkimpaas__1__0_models.UploadFileResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkimpaas__1__0_models.UploadFileHeaders()
+        return self.upload_file_with_options(request, headers, runtime)
+
+    async def upload_file_async(
+        self,
+        request: dingtalkimpaas__1__0_models.UploadFileRequest,
+    ) -> dingtalkimpaas__1__0_models.UploadFileResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkimpaas__1__0_models.UploadFileHeaders()
+        return await self.upload_file_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2881,7 +2881,156 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateGroupOwnerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UploadFileHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UploadFileRequest(TeaModel):
+    def __init__(
+        self,
+        file_name: str = None,
+        file_type: str = None,
+        file_url: str = None,
+        sender_uid: str = None,
+    ):
+        self.file_name = file_name
+        self.file_type = file_type
+        self.file_url = file_url
+        self.sender_uid = sender_uid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.file_name is not None:
+            result['fileName'] = self.file_name
+        if self.file_type is not None:
+            result['fileType'] = self.file_type
+        if self.file_url is not None:
+            result['fileUrl'] = self.file_url
+        if self.sender_uid is not None:
+            result['senderUid'] = self.sender_uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('fileName') is not None:
+            self.file_name = m.get('fileName')
+        if m.get('fileType') is not None:
+            self.file_type = m.get('fileType')
+        if m.get('fileUrl') is not None:
+            self.file_url = m.get('fileUrl')
+        if m.get('senderUid') is not None:
+            self.sender_uid = m.get('senderUid')
+        return self
+
+
+class UploadFileResponseBody(TeaModel):
+    def __init__(
+        self,
+        media_id: str = None,
+    ):
+        self.media_id = media_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.media_id is not None:
+            result['mediaId'] = self.media_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('mediaId') is not None:
+            self.media_id = m.get('mediaId')
+        return self
+
+
+class UploadFileResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UploadFileResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UploadFileResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5455,16 +5455,16 @@
         task_id: str,
         request: dingtalkproject__1__0_models.UpdateTaskStageRequest,
         headers: dingtalkproject__1__0_models.UpdateTaskStageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateTaskStageResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.stage_id):
-            body['stageId'] = request.stage_id
+        if not UtilClient.is_unset(request.task_stage_id):
+            body['taskStageId'] = request.task_stage_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -5492,16 +5492,16 @@
         task_id: str,
         request: dingtalkproject__1__0_models.UpdateTaskStageRequest,
         headers: dingtalkproject__1__0_models.UpdateTaskStageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkproject__1__0_models.UpdateTaskStageResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.stage_id):
-            body['stageId'] = request.stage_id
+        if not UtilClient.is_unset(request.task_stage_id):
+            body['taskStageId'] = request.task_stage_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -8482,23 +8482,23 @@
 class SearchTaskListResponseBodyResult(TeaModel):
     def __init__(
         self,
         created: str = None,
         creator_id: str = None,
         description: str = None,
         project_id: str = None,
-        task_id: str = None,
+        task_list_id: str = None,
         title: str = None,
         updated: str = None,
     ):
         self.created = created
         self.creator_id = creator_id
         self.description = description
         self.project_id = project_id
-        self.task_id = task_id
+        self.task_list_id = task_list_id
         self.title = title
         self.updated = updated
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -8511,16 +8511,16 @@
             result['created'] = self.created
         if self.creator_id is not None:
             result['creatorId'] = self.creator_id
         if self.description is not None:
             result['description'] = self.description
         if self.project_id is not None:
             result['projectId'] = self.project_id
-        if self.task_id is not None:
-            result['taskId'] = self.task_id
+        if self.task_list_id is not None:
+            result['taskListId'] = self.task_list_id
         if self.title is not None:
             result['title'] = self.title
         if self.updated is not None:
             result['updated'] = self.updated
         return result
 
     def from_map(self, m: dict = None):
@@ -8529,16 +8529,16 @@
             self.created = m.get('created')
         if m.get('creatorId') is not None:
             self.creator_id = m.get('creatorId')
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('projectId') is not None:
             self.project_id = m.get('projectId')
-        if m.get('taskId') is not None:
-            self.task_id = m.get('taskId')
+        if m.get('taskListId') is not None:
+            self.task_list_id = m.get('taskListId')
         if m.get('title') is not None:
             self.title = m.get('title')
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         return self
 
 
@@ -8951,54 +8951,351 @@
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('tql') is not None:
             self.tql = m.get('tql')
         return self
 
 
+class SearchUserTaskResponseBodyResultCustomfieldsValue(TeaModel):
+    def __init__(
+        self,
+        fieldvalue_id: str = None,
+        meta_string: str = None,
+        title: str = None,
+        total_count: int = None,
+    ):
+        self.fieldvalue_id = fieldvalue_id
+        self.meta_string = meta_string
+        self.title = title
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fieldvalue_id is not None:
+            result['fieldvalueId'] = self.fieldvalue_id
+        if self.meta_string is not None:
+            result['metaString'] = self.meta_string
+        if self.title is not None:
+            result['title'] = self.title
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('fieldvalueId') is not None:
+            self.fieldvalue_id = m.get('fieldvalueId')
+        if m.get('metaString') is not None:
+            self.meta_string = m.get('metaString')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class SearchUserTaskResponseBodyResultCustomfields(TeaModel):
+    def __init__(
+        self,
+        customfield_id: str = None,
+        type: str = None,
+        value: List[SearchUserTaskResponseBodyResultCustomfieldsValue] = None,
+    ):
+        self.customfield_id = customfield_id
+        self.type = type
+        self.value = value
+
+    def validate(self):
+        if self.value:
+            for k in self.value:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.customfield_id is not None:
+            result['customfieldId'] = self.customfield_id
+        if self.type is not None:
+            result['type'] = self.type
+        result['value'] = []
+        if self.value is not None:
+            for k in self.value:
+                result['value'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customfieldId') is not None:
+            self.customfield_id = m.get('customfieldId')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        self.value = []
+        if m.get('value') is not None:
+            for k in m.get('value'):
+                temp_model = SearchUserTaskResponseBodyResultCustomfieldsValue()
+                self.value.append(temp_model.from_map(k))
+        return self
+
+
+class SearchUserTaskResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        accomplish_time: str = None,
+        ancestor_ids: List[str] = None,
+        content: str = None,
+        created: str = None,
+        creator_id: str = None,
+        customfields: List[SearchUserTaskResponseBodyResultCustomfields] = None,
+        due_date: str = None,
+        executor_id: str = None,
+        involve_members: List[str] = None,
+        is_archived: bool = None,
+        is_done: bool = None,
+        note: str = None,
+        parent_task_id: str = None,
+        priority: int = None,
+        project_id: str = None,
+        recurrence: List[str] = None,
+        sfc_id: str = None,
+        sprint_id: str = None,
+        start_date: str = None,
+        story_point: str = None,
+        tag_ids: List[str] = None,
+        task_id: str = None,
+        task_list_id: str = None,
+        taskflowstatus_id: str = None,
+        taskstage_id: str = None,
+        unique_id: str = None,
+        updated: str = None,
+        visible: str = None,
+    ):
+        self.accomplish_time = accomplish_time
+        self.ancestor_ids = ancestor_ids
+        self.content = content
+        self.created = created
+        self.creator_id = creator_id
+        self.customfields = customfields
+        self.due_date = due_date
+        self.executor_id = executor_id
+        self.involve_members = involve_members
+        self.is_archived = is_archived
+        self.is_done = is_done
+        self.note = note
+        self.parent_task_id = parent_task_id
+        self.priority = priority
+        self.project_id = project_id
+        self.recurrence = recurrence
+        self.sfc_id = sfc_id
+        self.sprint_id = sprint_id
+        self.start_date = start_date
+        self.story_point = story_point
+        self.tag_ids = tag_ids
+        self.task_id = task_id
+        self.task_list_id = task_list_id
+        self.taskflowstatus_id = taskflowstatus_id
+        self.taskstage_id = taskstage_id
+        self.unique_id = unique_id
+        self.updated = updated
+        self.visible = visible
+
+    def validate(self):
+        if self.customfields:
+            for k in self.customfields:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accomplish_time is not None:
+            result['accomplishTime'] = self.accomplish_time
+        if self.ancestor_ids is not None:
+            result['ancestorIds'] = self.ancestor_ids
+        if self.content is not None:
+            result['content'] = self.content
+        if self.created is not None:
+            result['created'] = self.created
+        if self.creator_id is not None:
+            result['creatorId'] = self.creator_id
+        result['customfields'] = []
+        if self.customfields is not None:
+            for k in self.customfields:
+                result['customfields'].append(k.to_map() if k else None)
+        if self.due_date is not None:
+            result['dueDate'] = self.due_date
+        if self.executor_id is not None:
+            result['executorId'] = self.executor_id
+        if self.involve_members is not None:
+            result['involveMembers'] = self.involve_members
+        if self.is_archived is not None:
+            result['isArchived'] = self.is_archived
+        if self.is_done is not None:
+            result['isDone'] = self.is_done
+        if self.note is not None:
+            result['note'] = self.note
+        if self.parent_task_id is not None:
+            result['parentTaskId'] = self.parent_task_id
+        if self.priority is not None:
+            result['priority'] = self.priority
+        if self.project_id is not None:
+            result['projectId'] = self.project_id
+        if self.recurrence is not None:
+            result['recurrence'] = self.recurrence
+        if self.sfc_id is not None:
+            result['sfcId'] = self.sfc_id
+        if self.sprint_id is not None:
+            result['sprintId'] = self.sprint_id
+        if self.start_date is not None:
+            result['startDate'] = self.start_date
+        if self.story_point is not None:
+            result['storyPoint'] = self.story_point
+        if self.tag_ids is not None:
+            result['tagIds'] = self.tag_ids
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        if self.task_list_id is not None:
+            result['taskListId'] = self.task_list_id
+        if self.taskflowstatus_id is not None:
+            result['taskflowstatusId'] = self.taskflowstatus_id
+        if self.taskstage_id is not None:
+            result['taskstageId'] = self.taskstage_id
+        if self.unique_id is not None:
+            result['uniqueId'] = self.unique_id
+        if self.updated is not None:
+            result['updated'] = self.updated
+        if self.visible is not None:
+            result['visible'] = self.visible
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('accomplishTime') is not None:
+            self.accomplish_time = m.get('accomplishTime')
+        if m.get('ancestorIds') is not None:
+            self.ancestor_ids = m.get('ancestorIds')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('created') is not None:
+            self.created = m.get('created')
+        if m.get('creatorId') is not None:
+            self.creator_id = m.get('creatorId')
+        self.customfields = []
+        if m.get('customfields') is not None:
+            for k in m.get('customfields'):
+                temp_model = SearchUserTaskResponseBodyResultCustomfields()
+                self.customfields.append(temp_model.from_map(k))
+        if m.get('dueDate') is not None:
+            self.due_date = m.get('dueDate')
+        if m.get('executorId') is not None:
+            self.executor_id = m.get('executorId')
+        if m.get('involveMembers') is not None:
+            self.involve_members = m.get('involveMembers')
+        if m.get('isArchived') is not None:
+            self.is_archived = m.get('isArchived')
+        if m.get('isDone') is not None:
+            self.is_done = m.get('isDone')
+        if m.get('note') is not None:
+            self.note = m.get('note')
+        if m.get('parentTaskId') is not None:
+            self.parent_task_id = m.get('parentTaskId')
+        if m.get('priority') is not None:
+            self.priority = m.get('priority')
+        if m.get('projectId') is not None:
+            self.project_id = m.get('projectId')
+        if m.get('recurrence') is not None:
+            self.recurrence = m.get('recurrence')
+        if m.get('sfcId') is not None:
+            self.sfc_id = m.get('sfcId')
+        if m.get('sprintId') is not None:
+            self.sprint_id = m.get('sprintId')
+        if m.get('startDate') is not None:
+            self.start_date = m.get('startDate')
+        if m.get('storyPoint') is not None:
+            self.story_point = m.get('storyPoint')
+        if m.get('tagIds') is not None:
+            self.tag_ids = m.get('tagIds')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        if m.get('taskListId') is not None:
+            self.task_list_id = m.get('taskListId')
+        if m.get('taskflowstatusId') is not None:
+            self.taskflowstatus_id = m.get('taskflowstatusId')
+        if m.get('taskstageId') is not None:
+            self.taskstage_id = m.get('taskstageId')
+        if m.get('uniqueId') is not None:
+            self.unique_id = m.get('uniqueId')
+        if m.get('updated') is not None:
+            self.updated = m.get('updated')
+        if m.get('visible') is not None:
+            self.visible = m.get('visible')
+        return self
+
+
 class SearchUserTaskResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
-        result: List[str] = None,
+        result: List[SearchUserTaskResponseBodyResult] = None,
         total_size: int = None,
     ):
         self.next_token = next_token
         self.request_id = request_id
         self.result = result
         self.total_size = total_size
 
     def validate(self):
-        pass
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.request_id is not None:
             result['requestId'] = self.request_id
+        result['result'] = []
         if self.result is not None:
-            result['result'] = self.result
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
         if self.total_size is not None:
             result['totalSize'] = self.total_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('requestId') is not None:
             self.request_id = m.get('requestId')
+        self.result = []
         if m.get('result') is not None:
-            self.result = m.get('result')
+            for k in m.get('result'):
+                temp_model = SearchUserTaskResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
         if m.get('totalSize') is not None:
             self.total_size = m.get('totalSize')
         return self
 
 
 class SearchUserTaskResponse(TeaModel):
     def __init__(
@@ -12205,35 +12502,35 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class UpdateTaskStageRequest(TeaModel):
     def __init__(
         self,
-        stage_id: str = None,
+        task_stage_id: str = None,
     ):
-        self.stage_id = stage_id
+        self.task_stage_id = task_stage_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.stage_id is not None:
-            result['stageId'] = self.stage_id
+        if self.task_stage_id is not None:
+            result['taskStageId'] = self.task_stage_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('stageId') is not None:
-            self.stage_id = m.get('stageId')
+        if m.get('taskStageId') is not None:
+            self.task_stage_id = m.get('taskStageId')
         return self
 
 
 class UpdateTaskStageResponseBodyResult(TeaModel):
     def __init__(
         self,
         accomplish_time: str = None,
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.10/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dingtalk
-Version: 2.0.0
+Name: alibabacloud_dingtalk
+Version: 2.0.10
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.0/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.10/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.0/setup.py` & `alibabacloud_dingtalk-2.0.10/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 26/04/2023
+Created on 28/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

