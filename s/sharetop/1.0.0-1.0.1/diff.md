# Comparing `tmp/sharetop-1.0.0.tar.gz` & `tmp/sharetop-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.0.0.tar", last modified: Fri Apr 28 01:05:38 2023, max compression
+gzip compressed data, was "sharetop-1.0.1.tar", last modified: Fri Apr 28 01:46:04 2023, max compression
```

## Comparing `sharetop-1.0.0.tar` & `sharetop-1.0.1.tar`

### file list

```diff
@@ -1,78 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.183934 sharetop-1.0.0/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    39592 2023-04-28 01:05:38.182933 sharetop-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    38312 2023-04-27 15:08:33.000000 sharetop-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 01:05:38.183934 sharetop-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1169 2023-04-27 23:46:58.000000 sharetop-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.076776 sharetop-1.0.0/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.0/sharetop/__init__.py
--rw-rw-rw-   0        0        0      442 2023-04-26 04:52:26.000000 sharetop-1.0.0/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.116881 sharetop-1.0.0/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.0/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.119882 sharetop-1.0.0/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.0/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4165 2023-04-21 13:29:45.000000 sharetop-1.0.0/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.125168 sharetop-1.0.0/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.0/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.132483 sharetop-1.0.0/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.0/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.0/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.0/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.0/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.0/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.136472 sharetop-1.0.0/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.0/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.0/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12266 2023-04-27 15:28:32.000000 sharetop-1.0.0/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.0/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.148571 sharetop-1.0.0/sharetop/core/fund/
--rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.0/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.0/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.0/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.0/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.0/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.0/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.0/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.0/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.0/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.0/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.150158 sharetop-1.0.0/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.0/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0    11055 2023-04-27 14:23:26.000000 sharetop-1.0.0/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.156512 sharetop-1.0.0/sharetop/core/stock/
--rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.0/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4682 2023-04-25 21:03:26.000000 sharetop-1.0.0/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.0/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.0/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10289 2023-04-27 15:28:32.000000 sharetop-1.0.0/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10050 2023-04-27 15:28:32.000000 sharetop-1.0.0/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.0/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.158521 sharetop-1.0.0/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.0/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.0/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.0/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.164474 sharetop-1.0.0/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.0/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.0/sharetop/parser/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.115868 sharetop-1.0.0/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39592 2023-04-28 01:05:38.000000 sharetop-1.0.0/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1703 2023-04-28 01:05:38.000000 sharetop-1.0.0/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:05:38.000000 sharetop-1.0.0/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-28 01:05:38.000000 sharetop-1.0.0/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 01:05:38.000000 sharetop-1.0.0/sharetop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.171128 sharetop-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-04-09 14:35:36.000000 sharetop-1.0.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.173600 sharetop-1.0.0/test/bond_test/
--rw-rw-rw-   0        0        0        0 2023-04-23 14:58:14.000000 sharetop-1.0.0/test/bond_test/__init__.py
--rw-rw-rw-   0        0        0      621 2023-04-24 04:36:54.000000 sharetop-1.0.0/test/bond_test/test1.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:05:38.181933 sharetop-1.0.0/test/fund_test/
--rw-rw-rw-   0        0        0        0 2023-04-21 04:41:13.000000 sharetop-1.0.0/test/fund_test/__init__.py
--rw-rw-rw-   0        0        0     1499 2023-04-21 13:40:27.000000 sharetop-1.0.0/test/fund_test/test1.py
--rw-rw-rw-   0        0        0      138 2023-04-22 03:14:06.000000 sharetop-1.0.0/test/fund_test/test2.py
--rw-rw-rw-   0        0        0      464 2023-04-23 04:16:37.000000 sharetop-1.0.0/test/fund_test/test3.py
--rw-rw-rw-   0        0        0      648 2023-04-27 14:40:13.000000 sharetop-1.0.0/test/test1.py
--rw-rw-rw-   0        0        0      223 2023-04-18 15:50:29.000000 sharetop-1.0.0/test/test2.py
--rw-rw-rw-   0        0        0      146 2023-04-14 01:01:19.000000 sharetop-1.0.0/test/test3.py
--rw-rw-rw-   0        0        0      964 2023-04-15 09:48:17.000000 sharetop-1.0.0/test/test4.py
--rw-rw-rw-   0        0        0      179 2023-04-19 00:40:19.000000 sharetop-1.0.0/test/test5.py
--rw-rw-rw-   0        0        0      167 2023-04-24 00:37:53.000000 sharetop-1.0.0/test/test6.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.921975 sharetop-1.0.1/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    39117 2023-04-28 01:46:04.920942 sharetop-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    37909 2023-04-28 01:45:42.000000 sharetop-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:46:04.921975 sharetop-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1169 2023-04-27 23:46:58.000000 sharetop-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.846324 sharetop-1.0.1/sharetop/
+-rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.1/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.876739 sharetop-1.0.1/sharetop/api/
+-rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.1/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.879737 sharetop-1.0.1/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.1/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4165 2023-04-21 13:29:45.000000 sharetop-1.0.1/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.883776 sharetop-1.0.1/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.1/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.891139 sharetop-1.0.1/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.1/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.1/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.1/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.894135 sharetop-1.0.1/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.1/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.1/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12266 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.1/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.906938 sharetop-1.0.1/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.1/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.908942 sharetop-1.0.1/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.1/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.912938 sharetop-1.0.1/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.1/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.1/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10125 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10050 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.1/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.914937 sharetop-1.0.1/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.1/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.1/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.1/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.919939 sharetop-1.0.1/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.1/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.1/sharetop/parser/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.874744 sharetop-1.0.1/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    39117 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.0.0/LICENSE` & `sharetop-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/PKG-INFO` & `sharetop-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
-Project-URL: Documentation, https://efinance.readthedocs.io
 Project-URL: Source, https://github.com/nrliangxy/sharetop
-Keywords: finance,quant,stock,fund,futures,share,data
+Keywords: data,finance,quant,stock,fund,futures,share
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
-[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/efinance)
-[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/efinance)
+[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
+[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 [![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Docs](https://readthedocs.org/projects/sharetop/badge/?version=latest)](https://efinance.readthedocs.io)
-[![CodeFactor](https://www.codefactor.io/repository/github/micro-sheep/efinance/badge)](https://www.codefactor.io/repository/github/micro-sheep/efinance/overview/main)
 [![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`efinance`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -43,23 +40,14 @@
 
 - 通过 `pip` 更新
 
 ```bash
 pip install sharetop --upgrade
 ```
 
-
-- 源码安装（用于开发）
-
-```bash
-git clone https://github.com/Micro-sheep/efinance
-cd efinance
-pip install -e .
-```
-
 ---
 
 ## Examples
 
 ### Stock
 
 - 获取股票历史日 K 线数据
```

### Comparing `sharetop-1.0.0/README.md` & `sharetop-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 ## Introduction
 
-[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/efinance)
-[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/efinance)
+[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
+[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 [![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Docs](https://readthedocs.org/projects/sharetop/badge/?version=latest)](https://efinance.readthedocs.io)
-[![CodeFactor](https://www.codefactor.io/repository/github/micro-sheep/efinance/badge)](https://www.codefactor.io/repository/github/micro-sheep/efinance/overview/main)
 [![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`efinance`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -23,23 +21,14 @@
 
 - 通过 `pip` 更新
 
 ```bash
 pip install sharetop --upgrade
 ```
 
-
-- 源码安装（用于开发）
-
-```bash
-git clone https://github.com/Micro-sheep/efinance
-cd efinance
-pip install -e .
-```
-
 ---
 
 ## Examples
 
 ### Stock
 
 - 获取股票历史日 K 线数据
```

### Comparing `sharetop-1.0.0/setup.py` & `sharetop-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/application/base.py` & `sharetop-1.0.1/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/bond/__init__.py` & `sharetop-1.0.1/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/bond/config.py` & `sharetop-1.0.1/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/bond/get_bond_info.py` & `sharetop-1.0.1/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.0.1/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/cache.py` & `sharetop-1.0.1/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/common/config.py` & `sharetop-1.0.1/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/common/getter.py` & `sharetop-1.0.1/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/config.py` & `sharetop-1.0.1/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/__init__.py` & `sharetop-1.0.1/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/fund_list.py` & `sharetop-1.0.1/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.0.1/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.0.1/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.0.1/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.0.1/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.0.1/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.0.1/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.0.1/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/futures/get_futures_info.py` & `sharetop-1.0.1/sharetop/core/futures/get_futures_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     846  jm2109    焦煤2109  114.jm2109        大商所
     847  071108    IH2108    8.071108        中金所
     848  070131   IH次主力合约    8.070131        中金所
     849  070120    IH当月连续     8.07012        中金所
     850  lu2109  低硫燃油2109  142.lu2109  上海能源期货交易所
     Notes
     -----
-    这里的 行情ID 主要作用是为使用函数 ``efinance.futures.get_quote_history``
-    获取期货行情信息提供参数
     """
     columns = ['期货代码', '期货名称', '行情ID', '市场类型']
     df = get_realtime_quotes()
     df = df[columns]
     return df
 
 
@@ -82,45 +80,27 @@
         期货的 K 线数据
 
         - ``DataFrame`` : 当 ``secids`` 是 ``str`` 时
         - ``Dict[str, DataFrame]`` : 当 ``quote_ids`` 是 ``List[str]`` 时
 
     Examples
     --------
-    >>> import efinance as ef
-    >>> # 获取全部期货行情ID列表
-    >>> quote_ids = ef.futures.get_realtime_quotes()['行情ID']
-    >>> # 指定单个期货的行情ID(以上面获得到的行情ID列表为例)
-    >>> quote_id = quote_ids[0]
-    >>> # 查看第一个行情ID
-    >>> quote_ids[0]
-    '115.ZCM'
-    >>> # 获取第行情ID为第一个的期货日 K 线数据
-    >>> ef.futures.get_quote_history(quote_id)
         期货代码   期货名称          日期     开盘     收盘     最高     最低    成交量           成交额    振幅   涨跌幅   涨跌额  换手率
     0     ZCM  动力煤主力  2015-05-18  440.0  437.6  440.2  437.6     64  2.806300e+06  0.00  0.00   0.0  0.0
     1     ZCM  动力煤主力  2015-05-19  436.0  437.0  437.6  436.0      6  2.621000e+05  0.36 -0.32  -1.4  0.0
     2     ZCM  动力煤主力  2015-05-20  436.8  435.8  437.0  434.8      8  3.487500e+05  0.50 -0.23  -1.0  0.0
     3     ZCM  动力煤主力  2015-05-21  438.0  443.2  446.8  437.8     37  1.631850e+06  2.06  1.65   7.2  0.0
     4     ZCM  动力煤主力  2015-05-22  439.2  441.4  443.8  439.2     34  1.502500e+06  1.04  0.09   0.4  0.0
     ...   ...    ...         ...    ...    ...    ...    ...    ...           ...   ...   ...   ...  ...
     1524  ZCM  动力煤主力  2021-08-17  755.0  770.8  776.0  750.6  82373  6.288355e+09  3.25 -1.26  -9.8  0.0
     1525  ZCM  动力煤主力  2021-08-18  770.8  776.8  785.8  766.0  77392  6.016454e+09  2.59  1.76  13.4  0.0
     1526  ZCM  动力煤主力  2021-08-19  776.8  777.6  798.0  764.6  97229  7.597474e+09  4.30  0.03   0.2  0.0
     1527  ZCM  动力煤主力  2021-08-20  778.0  793.0  795.0  775.2  70549  5.553617e+09  2.53  1.48  11.6  0.0
     1528  ZCM  动力煤主力  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
-    >>> # 指定多个期货的 行情ID
-    >>> quote_ids = ['115.ZCM','115.ZC109']
-    >>> futures_df = ef.futures.get_quote_history(quote_ids)
-    >>> type(futures_df)
-    <class 'dict'>
-    >>> futures_df.keys()
-    dict_keys(['115.ZC109', '115.ZCM'])
-    >>> futures_df['115.ZCM']
         期货名称 期货代码          日期     开盘     收盘     最高     最低    成交量           成交额    振幅   涨跌幅   涨跌额  换手率
     0     动力煤主力  ZCM  2015-05-18  440.0  437.6  440.2  437.6     64  2.806300e+06  0.00  0.00   0.0  0.0
     1     动力煤主力  ZCM  2015-05-19  436.0  437.0  437.6  436.0      6  2.621000e+05  0.36 -0.32  -1.4  0.0
     2     动力煤主力  ZCM  2015-05-20  436.8  435.8  437.0  434.8      8  3.487500e+05  0.50 -0.23  -1.0  0.0
     3     动力煤主力  ZCM  2015-05-21  438.0  443.2  446.8  437.8     37  1.631850e+06  2.06  1.65   7.2  0.0
     4     动力煤主力  ZCM  2015-05-22  439.2  441.4  443.8  439.2     34  1.502500e+06  1.04  0.09   0.4  0.0
     ...     ...  ...         ...    ...    ...    ...    ...    ...           ...   ...   ...   ...  ...
@@ -171,16 +151,14 @@
     847  071108    IH2108 -2.52  3060.0  3130.0  3043.0  3111.2  -79.0   -  0.39     -   14384  13315567616.0  3139.2  918000    -    8.071108        中金所
     848  070131   IH次主力合约 -2.52  3060.0  3130.0  3043.0  3111.2  -79.0   -  0.57     -   14384  13315567616.0  3139.2  918000    -    8.070131        中金所
     849  070120    IH当月连续 -2.52  3060.0  3130.0  3043.0  3111.2  -79.0   -  0.39     -   14384  13315567616.0  3139.2  918000    -    8.070120        中金所
     850  lu2109  低硫燃油2109 -3.79  3123.0  3127.0  3121.0  3121.0 -123.0   -     -     -      22       687420.0  3143.0       -    -  142.lu2109  上海能源期货交易所
 
     Notes
     -----
-    如果不记得行情ID,则可以调用函数 ``efinance.futures.get_realtime_quotes`` 获取
-    接着便可以使用函数 ``efinance.futures.get_quote_history``
     来获取期货 K 线数据
     """
     fs = FS_DICT['futures']
     df = get_market_realtime_by_fs(fs)
     df = df.rename(columns={'代码': '期货代码', '名称': '期货名称'})
     return df
 
@@ -197,15 +175,14 @@
     Returns
     -------
     DataFrame
         期货最新交易日成交明细
 
     Notes
     -----
-    行情ID 格式参考 ``efinance.futures.get_futures_base_info`` 中得到的数据
 
     Examples
     --------
         期货名称 期货代码        时间   昨收    成交价  成交量     单数
     0  动力煤主力  ZCM  21:00:00  0.0  879.0   23    0.0
     1  动力煤主力  ZCM  21:00:00  0.0  879.0    0 -373.0
     2  动力煤主力  ZCM  21:00:00  0.0  879.0    0    0.0
```

### Comparing `sharetop-1.0.0/sharetop/core/stock/bill_monitor.py` & `sharetop-1.0.1/sharetop/core/stock/bill_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,14 @@
         股票代码
     Returns
     -------
     DataFrame
         沪深市场单只股票历史单子流入流出数据
     Examples
     --------
-    >>> import efinance as ef
-    >>> ef.stock.get_history_bill('600519')
         股票名称    股票代码          日期         主力净流入       小单净流入         中单净流入         大单净流入        超大单净流入  主力净流入占比  小单流入净占比  中单流入净占比  大单流入净占比  超大单流入净占比      收盘价   涨跌幅
     0    贵州茅台  600519  2021-03-04 -3.670272e+06  -2282056.0  5.952143e+06  1.461528e+09 -1.465199e+09    -0.03    -0.02     0.04    10.99    -11.02  2013.71 -5.05
     1    贵州茅台  600519  2021-03-05 -1.514880e+07  -1319066.0  1.646793e+07 -2.528896e+07  1.014016e+07    -0.12    -0.01     0.13    -0.19      0.08  2040.82  1.35
     2    贵州茅台  600519  2021-03-08 -8.001702e+08   -877074.0  8.010473e+08  5.670671e+08 -1.367237e+09    -6.29    -0.01     6.30     4.46    -10.75  1940.71 -4.91
     3    贵州茅台  600519  2021-03-09 -2.237770e+08  -6391767.0  2.301686e+08 -1.795013e+08 -4.427571e+07    -1.39    -0.04     1.43    -1.11     -0.27  1917.70 -1.19
     4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
     ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
```

### Comparing `sharetop-1.0.0/sharetop/core/stock/config.py` & `sharetop-1.0.1/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/stock/getter.py` & `sharetop-1.0.1/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/stock/quarterly_report.py` & `sharetop-1.0.1/sharetop/core/stock/quarterly_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,14 @@
     4441  002838  道恩股份  2020-04-09 00:00:00  6.191659e+08 -8.019810  -16.5445  6.939886e+07   91.601624  76.7419  0.1700   2.840665    6.20  22.575224  0.186421
     4442  600396  金山股份  2020-04-08 00:00:00  2.023133e+09  0.518504   -3.0629  1.878432e+08  114.304022  61.2733  0.1275   1.511012    8.81  21.422393  0.085698
     4443  002913   奥士康  2020-04-08 00:00:00  4.898977e+08 -3.883035  -23.2268  2.524717e+07  -47.239162 -58.8136  0.1700  16.666749    1.03  22.470020  0.552624
     4444  002007  华兰生物  2020-04-08 00:00:00  6.775414e+08 -2.622289  -36.1714  2.472864e+08   -4.708821 -22.6345  0.1354   4.842456    3.71  61.408522  0.068341
 
     Notes
     -----
-    当输入的日期不正确时，会输出可选的日期列表。
-    你也可以通过函数 ``efinance.stock.get_all_report_dates`` 来获取可选日期
 
     """
     # TODO 加速
     fields = {
         'SECURITY_CODE': '股票代码',
         'SECURITY_NAME_ABBR': '股票简称',
         'NOTICE_DATE': '公告日期',
```

### Comparing `sharetop-1.0.0/sharetop/core/stock/rank_list.py` & `sharetop-1.0.1/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/core/utils.py` & `sharetop-1.0.1/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/crawl/base.py` & `sharetop-1.0.1/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop/crawl/settings.py` & `sharetop-1.0.1/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.0/sharetop.egg-info/PKG-INFO` & `sharetop-1.0.1/sharetop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
-Project-URL: Documentation, https://efinance.readthedocs.io
 Project-URL: Source, https://github.com/nrliangxy/sharetop
-Keywords: finance,quant,stock,fund,futures,share,data
+Keywords: data,finance,quant,stock,fund,futures,share
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
-[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/efinance)
-[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/efinance)
+[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
+[![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
 [![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Docs](https://readthedocs.org/projects/sharetop/badge/?version=latest)](https://efinance.readthedocs.io)
-[![CodeFactor](https://www.codefactor.io/repository/github/micro-sheep/efinance/badge)](https://www.codefactor.io/repository/github/micro-sheep/efinance/overview/main)
 [![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`efinance`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -43,23 +40,14 @@
 
 - 通过 `pip` 更新
 
 ```bash
 pip install sharetop --upgrade
 ```
 
-
-- 源码安装（用于开发）
-
-```bash
-git clone https://github.com/Micro-sheep/efinance
-cd efinance
-pip install -e .
-```
-
 ---
 
 ## Examples
 
 ### Stock
 
 - 获取股票历史日 K 线数据
```

### Comparing `sharetop-1.0.0/sharetop.egg-info/SOURCES.txt` & `sharetop-1.0.1/sharetop.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -40,21 +40,8 @@
 sharetop/core/stock/getter.py
 sharetop/core/stock/quarterly_report.py
 sharetop/core/stock/rank_list.py
 sharetop/crawl/__init__.py
 sharetop/crawl/base.py
 sharetop/crawl/settings.py
 sharetop/parser/__init__.py
-sharetop/parser/base.py
-test/__init__.py
-test/test1.py
-test/test2.py
-test/test3.py
-test/test4.py
-test/test5.py
-test/test6.py
-test/bond_test/__init__.py
-test/bond_test/test1.py
-test/fund_test/__init__.py
-test/fund_test/test1.py
-test/fund_test/test2.py
-test/fund_test/test3.py
+sharetop/parser/base.py
```

