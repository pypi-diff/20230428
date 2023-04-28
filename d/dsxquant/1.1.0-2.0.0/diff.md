# Comparing `tmp/dsxquant-1.1.0.tar.gz` & `tmp/dsxquant-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsxquant-1.1.0.tar", last modified: Fri Mar  3 08:53:29 2023, max compression
+gzip compressed data, was "dsxquant-2.0.0.tar", last modified: Fri Apr 28 07:54:39 2023, max compression
```

## Comparing `dsxquant-1.1.0.tar` & `dsxquant-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,80 @@
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.692142 dsxquant-1.1.0/
--rw-r--r--   0 fengming   (501) staff       (20)     1077 2023-03-01 09:49:49.000000 dsxquant-1.1.0/LICENSE
--rw-rw-rw-   0 fengming   (501) staff       (20)       37 2023-01-13 17:11:01.000000 dsxquant-1.1.0/MANIFEST.in
--rw-r--r--   0 fengming   (501) staff       (20)    16598 2023-03-03 08:53:29.692321 dsxquant-1.1.0/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)    15871 2023-03-03 08:49:11.000000 dsxquant-1.1.0/README.md
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.684177 dsxquant-1.1.0/dsxquant.egg-info/
--rw-r--r--   0 fengming   (501) staff       (20)    16598 2023-03-03 08:53:29.000000 dsxquant-1.1.0/dsxquant.egg-info/PKG-INFO
--rw-r--r--   0 fengming   (501) staff       (20)     1136 2023-03-03 08:53:29.000000 dsxquant-1.1.0/dsxquant.egg-info/SOURCES.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-03-03 08:53:29.000000 dsxquant-1.1.0/dsxquant.egg-info/dependency_links.txt
--rw-r--r--   0 fengming   (501) staff       (20)        1 2023-01-13 17:17:35.000000 dsxquant-1.1.0/dsxquant.egg-info/not-zip-safe
--rw-r--r--   0 fengming   (501) staff       (20)        9 2023-03-03 08:53:29.000000 dsxquant-1.1.0/dsxquant.egg-info/top_level.txt
--rw-r--r--   0 fengming   (501) staff       (20)      590 2023-03-03 08:53:11.000000 dsxquant-1.1.0/pyproject.toml
--rw-rw-rw-   0 fengming   (501) staff       (20)       82 2023-03-03 08:53:29.692980 dsxquant-1.1.0/setup.cfg
--rw-r--r--   0 fengming   (501) staff       (20)     1008 2023-03-03 07:57:24.000000 dsxquant-1.1.0/setup.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.681213 dsxquant-1.1.0/src/
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.684349 dsxquant-1.1.0/src/dsxquant/
--rw-r--r--   0 fengming   (501) staff       (20)     2538 2023-03-03 07:51:06.000000 dsxquant-1.1.0/src/dsxquant/__init__.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.685060 dsxquant-1.1.0/src/dsxquant/common/
--rw-r--r--   0 fengming   (501) staff       (20)      115 2023-01-13 14:06:03.000000 dsxquant-1.1.0/src/dsxquant/common/fn.py
--rw-r--r--   0 fengming   (501) staff       (20)     1041 2023-02-08 13:44:10.000000 dsxquant-1.1.0/src/dsxquant/common/json2model.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.685913 dsxquant-1.1.0/src/dsxquant/config/
--rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:46:01.000000 dsxquant-1.1.0/src/dsxquant/config/__init__.py
--rw-r--r--   0 fengming   (501) staff       (20)     1679 2023-03-02 15:19:29.000000 dsxquant-1.1.0/src/dsxquant/config/config.py
--rw-r--r--   0 fengming   (501) staff       (20)      726 2023-02-28 10:01:42.000000 dsxquant-1.1.0/src/dsxquant/config/logconfig.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.686385 dsxquant-1.1.0/src/dsxquant/dataser/
--rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:45:54.000000 dsxquant-1.1.0/src/dsxquant/dataser/__init__.py
--rw-r--r--   0 fengming   (501) staff       (20)    19349 2023-03-03 04:29:26.000000 dsxquant-1.1.0/src/dsxquant/dataser/dsx_dataser.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.687293 dsxquant-1.1.0/src/dsxquant/dataser/models/
--rw-r--r--   0 fengming   (501) staff       (20)     1218 2023-02-20 16:10:27.000000 dsxquant-1.1.0/src/dsxquant/dataser/models/quotes.py
--rw-r--r--   0 fengming   (501) staff       (20)      398 2023-02-20 13:25:08.000000 dsxquant-1.1.0/src/dsxquant/dataser/models/result.py
-drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-03-03 08:53:29.691882 dsxquant-1.1.0/src/dsxquant/dataser/parser/
--rw-r--r--   0 fengming   (501) staff       (20)     8766 2023-03-02 08:39:55.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/base.py
--rw-r--r--   0 fengming   (501) staff       (20)      679 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_category.py
--rw-r--r--   0 fengming   (501) staff       (20)      708 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_factors.py
--rw-r--r--   0 fengming   (501) staff       (20)      923 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_finance.py
--rw-r--r--   0 fengming   (501) staff       (20)     1105 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_kline.py
--rw-r--r--   0 fengming   (501) staff       (20)      767 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_quotes.py
--rw-r--r--   0 fengming   (501) staff       (20)      878 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_sharebonus.py
--rw-r--r--   0 fengming   (501) staff       (20)     1151 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_stocks.py
--rw-r--r--   0 fengming   (501) staff       (20)      820 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_timesharing.py
--rw-r--r--   0 fengming   (501) staff       (20)      904 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/get_translist.py
--rw-r--r--   0 fengming   (501) staff       (20)      570 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/heart.py
--rw-r--r--   0 fengming   (501) staff       (20)      838 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/login.py
--rw-r--r--   0 fengming   (501) staff       (20)      594 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/register.py
--rw-r--r--   0 fengming   (501) staff       (20)      559 2023-03-01 04:18:32.000000 dsxquant-1.1.0/src/dsxquant/dataser/parser/sub_all_quotes.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.493602 dsxquant-2.0.0/
+-rw-r--r--   0 fengming   (501) staff       (20)     1087 2023-03-14 11:47:02.000000 dsxquant-2.0.0/LICENSE
+-rw-rw-rw-   0 fengming   (501) staff       (20)       37 2023-01-13 17:11:01.000000 dsxquant-2.0.0/MANIFEST.in
+-rw-r--r--   0 fengming   (501) staff       (20)    18143 2023-04-28 07:54:39.493795 dsxquant-2.0.0/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)    17417 2023-04-27 12:01:18.000000 dsxquant-2.0.0/README.md
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.451839 dsxquant-2.0.0/dsxquant.egg-info/
+-rw-r--r--   0 fengming   (501) staff       (20)    18143 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/PKG-INFO
+-rw-r--r--   0 fengming   (501) staff       (20)     2118 2023-04-28 07:54:39.000000 dsxquant-2.0.0/dsxquant.egg-info/SOURCES.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/dependency_links.txt
+-rw-r--r--   0 fengming   (501) staff       (20)        1 2023-01-13 17:17:35.000000 dsxquant-2.0.0/dsxquant.egg-info/not-zip-safe
+-rw-r--r--   0 fengming   (501) staff       (20)        9 2023-04-28 07:54:38.000000 dsxquant-2.0.0/dsxquant.egg-info/top_level.txt
+-rw-r--r--   0 fengming   (501) staff       (20)      590 2023-04-27 11:43:13.000000 dsxquant-2.0.0/pyproject.toml
+-rw-rw-rw-   0 fengming   (501) staff       (20)       82 2023-04-28 07:54:39.494717 dsxquant-2.0.0/setup.cfg
+-rw-r--r--   0 fengming   (501) staff       (20)     1008 2023-04-27 11:44:27.000000 dsxquant-2.0.0/setup.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.443703 dsxquant-2.0.0/src/
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.452635 dsxquant-2.0.0/src/dsxquant/
+-rw-r--r--   0 fengming   (501) staff       (20)     3791 2023-04-11 06:26:26.000000 dsxquant-2.0.0/src/dsxquant/__init__.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.453020 dsxquant-2.0.0/src/dsxquant/backtest/
+-rw-r--r--   0 fengming   (501) staff       (20)    14523 2023-04-27 11:58:10.000000 dsxquant-2.0.0/src/dsxquant/backtest/back_test.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.461242 dsxquant-2.0.0/src/dsxquant/common/
+-rw-r--r--   0 fengming   (501) staff       (20)    14302 2023-04-13 11:36:50.000000 dsxquant-2.0.0/src/dsxquant/common/cache.py
+-rw-r--r--   0 fengming   (501) staff       (20)      115 2023-01-13 14:06:03.000000 dsxquant-2.0.0/src/dsxquant/common/fn.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1041 2023-02-08 13:44:10.000000 dsxquant-2.0.0/src/dsxquant/common/json2model.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.461721 dsxquant-2.0.0/src/dsxquant/config/
+-rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:46:01.000000 dsxquant-2.0.0/src/dsxquant/config/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2931 2023-04-03 15:50:28.000000 dsxquant-2.0.0/src/dsxquant/config/config.py
+-rw-r--r--   0 fengming   (501) staff       (20)      726 2023-02-28 10:01:42.000000 dsxquant-2.0.0/src/dsxquant/config/logconfig.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.462503 dsxquant-2.0.0/src/dsxquant/dataser/
+-rw-r--r--   0 fengming   (501) staff       (20)        0 2023-01-13 04:45:54.000000 dsxquant-2.0.0/src/dsxquant/dataser/__init__.py
+-rw-r--r--   0 fengming   (501) staff       (20)    20357 2023-04-11 06:26:36.000000 dsxquant-2.0.0/src/dsxquant/dataser/dsx_dataser.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.465671 dsxquant-2.0.0/src/dsxquant/dataser/models/
+-rw-r--r--   0 fengming   (501) staff       (20)     1218 2023-02-20 16:10:27.000000 dsxquant-2.0.0/src/dsxquant/dataser/models/quotes.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1040 2023-04-09 15:11:20.000000 dsxquant-2.0.0/src/dsxquant/dataser/models/result.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.476785 dsxquant-2.0.0/src/dsxquant/dataser/parser/
+-rw-r--r--   0 fengming   (501) staff       (20)     9247 2023-04-11 06:12:30.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      679 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_category.py
+-rw-r--r--   0 fengming   (501) staff       (20)      708 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_factors.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2449 2023-04-06 05:38:06.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_finance.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1948 2023-04-10 13:50:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_kline.py
+-rw-r--r--   0 fengming   (501) staff       (20)      767 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_quotes.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2011 2023-04-06 05:30:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_sharebonus.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1198 2023-04-11 06:26:52.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_stocks.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1992 2023-04-06 05:30:40.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_structure.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1520 2023-04-11 01:02:42.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_timesharing.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1599 2023-04-11 01:02:27.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/get_translist.py
+-rw-r--r--   0 fengming   (501) staff       (20)      570 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/heart.py
+-rw-r--r--   0 fengming   (501) staff       (20)      838 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/login.py
+-rw-r--r--   0 fengming   (501) staff       (20)      594 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/register.py
+-rw-r--r--   0 fengming   (501) staff       (20)      559 2023-03-01 04:18:32.000000 dsxquant-2.0.0/src/dsxquant/dataser/parser/sub_all_quotes.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.479647 dsxquant-2.0.0/src/dsxquant/emulation/
+-rw-r--r--   0 fengming   (501) staff       (20)      637 2023-03-20 10:20:35.000000 dsxquant-2.0.0/src/dsxquant/emulation/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      569 2023-03-20 10:20:52.000000 dsxquant-2.0.0/src/dsxquant/emulation/buy.py
+-rw-r--r--   0 fengming   (501) staff       (20)      360 2023-03-18 13:46:31.000000 dsxquant-2.0.0/src/dsxquant/emulation/cancel.py
+-rw-r--r--   0 fengming   (501) staff       (20)      568 2023-03-20 10:21:00.000000 dsxquant-2.0.0/src/dsxquant/emulation/sell.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.483816 dsxquant-2.0.0/src/dsxquant/engins/
+-rw-r--r--   0 fengming   (501) staff       (20)     2127 2023-04-04 01:51:04.000000 dsxquant-2.0.0/src/dsxquant/engins/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1199 2023-04-03 13:32:57.000000 dsxquant-2.0.0/src/dsxquant/engins/cache_space.py
+-rw-r--r--   0 fengming   (501) staff       (20)     6634 2023-04-11 13:47:37.000000 dsxquant-2.0.0/src/dsxquant/engins/data_feed.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2022 2023-04-04 01:49:38.000000 dsxquant-2.0.0/src/dsxquant/engins/emultion_engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2055 2023-04-26 01:51:50.000000 dsxquant-2.0.0/src/dsxquant/engins/engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3914 2023-04-26 01:52:48.000000 dsxquant-2.0.0/src/dsxquant/engins/event_bus.py
+-rw-r--r--   0 fengming   (501) staff       (20)      983 2023-03-20 09:56:55.000000 dsxquant-2.0.0/src/dsxquant/engins/event_model.py
+-rw-r--r--   0 fengming   (501) staff       (20)     3503 2023-04-23 15:08:44.000000 dsxquant-2.0.0/src/dsxquant/engins/strategy_engin.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2176 2023-03-15 15:09:55.000000 dsxquant-2.0.0/src/dsxquant/engins/trade_engin.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.483988 dsxquant-2.0.0/src/dsxquant/orders/
+-rw-r--r--   0 fengming   (501) staff       (20)    14031 2023-04-27 11:39:06.000000 dsxquant-2.0.0/src/dsxquant/orders/orders.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.490837 dsxquant-2.0.0/src/dsxquant/strategy/
+-rw-r--r--   0 fengming   (501) staff       (20)     4905 2023-04-11 14:48:36.000000 dsxquant-2.0.0/src/dsxquant/strategy/base.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.492163 dsxquant-2.0.0/src/dsxquant/strategy/common/
+-rw-r--r--   0 fengming   (501) staff       (20)     1495 2023-04-26 01:36:49.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/macross_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1396 2023-03-17 11:08:35.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/myself_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1089 2023-03-17 13:58:55.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/t_strategy.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2212 2023-04-13 14:11:22.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/抛物线策略.py
+-rw-r--r--   0 fengming   (501) staff       (20)     2268 2023-04-13 14:44:39.000000 dsxquant-2.0.0/src/dsxquant/strategy/common/放量突破策略.py
+-rw-r--r--   0 fengming   (501) staff       (20)     1535 2023-04-23 15:29:19.000000 dsxquant-2.0.0/src/dsxquant/strategy/data_model.py
+drwxr-xr-x   0 fengming   (501) staff       (20)        0 2023-04-28 07:54:39.493430 dsxquant-2.0.0/src/dsxquant/trade/
+-rw-r--r--   0 fengming   (501) staff       (20)      441 2023-03-14 07:06:27.000000 dsxquant-2.0.0/src/dsxquant/trade/base.py
+-rw-r--r--   0 fengming   (501) staff       (20)      321 2023-03-14 07:11:49.000000 dsxquant-2.0.0/src/dsxquant/trade/buy.py
+-rw-r--r--   0 fengming   (501) staff       (20)      326 2023-03-14 07:11:58.000000 dsxquant-2.0.0/src/dsxquant/trade/cancel.py
+-rw-r--r--   0 fengming   (501) staff       (20)      322 2023-03-14 07:12:02.000000 dsxquant-2.0.0/src/dsxquant/trade/sell.py
```

### Comparing `dsxquant-1.1.0/LICENSE` & `dsxquant-2.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (C) <year> <copyright holders>
+Copyright (C) 2023 by fangyunsm <934476300@qq.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. [1]
```

### Comparing `dsxquant-1.1.0/PKG-INFO` & `dsxquant-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: dsxquant
-Version: 1.1.0
-Summary: Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
-Home-page: https://github.com/dsxkline/dsx_quant_python
-Author: fangyunsm
-Author-email: fangyunsm <934476300@qq.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/dsxkline/dsxquant
-Project-URL: Bug Tracker, https://github.com/dsxkline/dsxquant/issues
-Keywords: quant 量化
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6,<4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Dsxquant
+# Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
 
@@ -604,7 +588,31 @@
 4  1453  13.94  537500.0  7.465875e+06  13.890
 5  1452  13.96  356300.0  4.949007e+06  13.890
 6  1451  13.96  246100.0  3.418083e+06  13.889
 7  1450  13.95  671800.0  9.330630e+06  13.889
 8  1449  13.96  253800.0  3.525028e+06  13.889
 9  1448  13.96  423200.0  5.877402e+06  13.888
 ```
+
+## 回测
+
+目前支持简单回测功能，支持日线和分钟线级别的历史数据回测
+
+
+```python
+from dsxquant.engins.engin import Engin
+from dsxquant.backtest.back_test import BackTest
+from dsxquant import StrategyEngin,EmulationEngin,DataFeed,EventType
+from dsxquant.strategy.common.macross_strategy import MACrossStrategy
+import dsxquant
+# 先启动系统引擎
+engin = Engin().start()
+# 安装模块
+engin.install(StrategyEngin,EmulationEngin,DataFeed)
+# 调用回测,这个例子是日线回测
+backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
+engin.install(backtest)
+# 等待回测完成并显示回测结果  
+backtest.show()
+engin.shutdown()
+
+```
```

### Comparing `dsxquant-1.1.0/README.md` & `dsxquant-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,31 @@
-# Dsxquant
+Metadata-Version: 2.1
+Name: dsxquant
+Version: 2.0.0
+Summary: Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
+Home-page: https://github.com/dsxkline/dsx_quant_python
+Author: fangyunsm
+Author-email: fangyunsm <934476300@qq.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/dsxkline/dsxquant
+Project-URL: Bug Tracker, https://github.com/dsxkline/dsxquant/issues
+Keywords: quant 量化
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6,<4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
 
@@ -585,8 +605,32 @@
 3  1454  13.95  404100.0  5.612949e+06  13.890
 4  1453  13.94  537500.0  7.465875e+06  13.890
 5  1452  13.96  356300.0  4.949007e+06  13.890
 6  1451  13.96  246100.0  3.418083e+06  13.889
 7  1450  13.95  671800.0  9.330630e+06  13.889
 8  1449  13.96  253800.0  3.525028e+06  13.889
 9  1448  13.96  423200.0  5.877402e+06  13.888
-```
+```
+
+## 回测
+
+目前支持简单回测功能，支持日线和分钟线级别的历史数据回测
+
+
+```python
+from dsxquant.engins.engin import Engin
+from dsxquant.backtest.back_test import BackTest
+from dsxquant import StrategyEngin,EmulationEngin,DataFeed,EventType
+from dsxquant.strategy.common.macross_strategy import MACrossStrategy
+import dsxquant
+# 先启动系统引擎
+engin = Engin().start()
+# 安装模块
+engin.install(StrategyEngin,EmulationEngin,DataFeed)
+# 调用回测,这个例子是日线回测
+backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
+engin.install(backtest)
+# 等待回测完成并显示回测结果  
+backtest.show()
+engin.shutdown()
+
+```
```

### Comparing `dsxquant-1.1.0/dsxquant.egg-info/PKG-INFO` & `dsxquant-2.0.0/dsxquant.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsxquant
-Version: 1.1.0
+Version: 2.0.0
 Summary: Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 Home-page: https://github.com/dsxkline/dsx_quant_python
 Author: fangyunsm
 Author-email: fangyunsm <934476300@qq.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/dsxkline/dsxquant
 Project-URL: Bug Tracker, https://github.com/dsxkline/dsxquant/issues
@@ -12,18 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Dsxquant
+# Dsxquant 开源量化工具箱
 
 Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。
 
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dsxquant"> <img alt="PyPI" src="https://img.shields.io/pypi/v/dsxquant?label=dsxquant"> <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/dsxkline/dsxquant"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/dsxquant"> <img alt="Libraries.io dependency status for GitHub repo" src="https://img.shields.io/librariesio/github/dsxkline/dsxquant"> <img alt="GitHub" src="https://img.shields.io/github/license/dsxkline/dsxquant"> <img alt="GitHub search hit counter" src="https://img.shields.io/github/search/dsxkline/dsxquant/dsxquant"> <img alt="Website" src="https://img.shields.io/website?label=dsxquant%20website&up_message=online&url=https%3A%2F%2Fwww.dsxquant.com">
+
 ## 一、简介
 Dsxquant 采用模块化设计思想，框架集成了数据、回测、策略、因子、仿真、资管、交易等模块。
 
 技术架构
 
 <img src="https://www.dsxquant.com/wp-content/uploads/2023/03/Dsxquant-Main-Engine-2-1024x985.png" width="300" />
 
@@ -604,7 +606,31 @@
 4  1453  13.94  537500.0  7.465875e+06  13.890
 5  1452  13.96  356300.0  4.949007e+06  13.890
 6  1451  13.96  246100.0  3.418083e+06  13.889
 7  1450  13.95  671800.0  9.330630e+06  13.889
 8  1449  13.96  253800.0  3.525028e+06  13.889
 9  1448  13.96  423200.0  5.877402e+06  13.888
 ```
+
+## 回测
+
+目前支持简单回测功能，支持日线和分钟线级别的历史数据回测
+
+
+```python
+from dsxquant.engins.engin import Engin
+from dsxquant.backtest.back_test import BackTest
+from dsxquant import StrategyEngin,EmulationEngin,DataFeed,EventType
+from dsxquant.strategy.common.macross_strategy import MACrossStrategy
+import dsxquant
+# 先启动系统引擎
+engin = Engin().start()
+# 安装模块
+engin.install(StrategyEngin,EmulationEngin,DataFeed)
+# 调用回测,这个例子是日线回测
+backtest = BackTest(MACrossStrategy,"sz000001",start="20200412",end="20230427",data=EventType.DAYLINE)
+engin.install(backtest)
+# 等待回测完成并显示回测结果  
+backtest.show()
+engin.shutdown()
+
+```
```

### Comparing `dsxquant-1.1.0/pyproject.toml` & `dsxquant-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsxquant"
-version = "1.1.0"
+version = "2.0.0"
 authors = [
   { name="fangyunsm", email="934476300@qq.com" },
 ]
 description = "Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dsxquant-1.1.0/setup.py` & `dsxquant-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', encoding='utf-8') as f:
         content = f.read()
     return content
 
 
 setup(
     name="dsxquant",  # 包名称
-    version="1.1.0",  # 版本号
+    version="2.0.0",  # 版本号
     author="fangyunsm",  # 作者
     author_email="934476300@qq.com",  # 作者邮箱
     description="Dsxquant 是一个基于python语言开发的的量化工具箱，主要特征是其工具属性，专为上层策略应用提供服务。",  # 描述
     long_description=readme(),  # 长文描述
     keywords="quant 量化",  # 项目关键词
     url="https://github.com/dsxkline/dsx_quant_python",  # 项目主页
     license="MIT License",  # 许可证
```

### Comparing `dsxquant-1.1.0/src/dsxquant/common/json2model.py` & `dsxquant-2.0.0/src/dsxquant/common/json2model.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/config/logconfig.py` & `dsxquant-2.0.0/src/dsxquant/config/logconfig.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/dsx_dataser.py` & `dsxquant-2.0.0/src/dsxquant/dataser/dsx_dataser.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from dsxquant.dataser.parser.get_factors import GetFactorsParser
 from dsxquant.dataser.parser.get_sharebonus import GetShareBonusParser
 from dsxquant.dataser.parser.get_timesharing import GetTimeSharingParser
 from dsxquant.dataser.parser.get_translist import GetTransListParser
 from dsxquant.dataser.parser.get_category import GetCategoryParser
 from dsxquant.dataser.models.result import ResultModel
 from dsxquant.dataser.parser.sub_all_quotes import SubAllQuotesParser
+from dsxquant.dataser.parser.get_structure import GetStructureParser
+from dsxquant.common.cache import CacheHelper
 
 class WithExpationFails(BaseException):
     pass
 
 class DsxDataser(object):
 
     lock = threading.Lock()
@@ -372,24 +374,24 @@
         return self.get_category(1)
     def get_diyu(self):
         """请求地域分类
         """
         return self.get_category(2)
     
     # 请求证券信息
-    def get_stocks(self,market:int=None,symbol:str=None,hangye:str=None,gainian:str=None,diyu:str=None,listing_date:str=None):
+    def get_stocks(self,market:int=None,symbol:str=None,hangye:str=None,gainian:str=None,diyu:str=None,listing_date:str=None,category:int=0):
         """请求证券详情信息
 
         Args:
             market (int): 市场编号 
             symbol (str): 证券代码 为空返回市场股票代码列表
         """
         if not self.connected:return
         r =  GetStocksParser(self.client)
-        r.setParams(symbol,market,hangye,gainian,diyu,listing_date)
+        r.setParams(symbol,market,hangye,gainian,diyu,listing_date,category)
         return r.call_api()
 
     def get_quotes(self,symbols:Union[list,str,tuple]):
         """请求实时行情
 
         Args:
             symbol (str): 证券代码
@@ -420,15 +422,15 @@
         if not self.connected:return
         r =  SubAllQuotesParser(self.client,self.sync,callback)
         r.setParams()
         if(not self.sync): self.__save_api(r)
         return r.call_api()
         
 
-    def get_klines(self,symbol:str,market:int,page:int=1,page_size:int=320,fq:str=config.FQ.DEFAULT,cycle:config.CYCLE=config.CYCLE.DAY):
+    def get_klines(self,symbol:str,market:int,page:int=1,page_size:int=320,fq:str=config.FQ.DEFAULT,cycle:config.CYCLE=config.CYCLE.DAY,start:str=None,end:str=None,enable_cache:bool=True):
         """请求历史K线图
 
         Args:
             symbol (str): 证券代码
             market (int): 市场代码
             page (int, optional): 页码. Defaults to 1.
             page_size (int, optional): 每页大小. Defaults to 320.
@@ -436,20 +438,20 @@
             callback (callable, optional): 回调函数. Defaults to None.
 
         Returns:
             _type_: 历史行情数据
         """
         if not self.connected:return
         r =  GetKlinesParser(self.client,self.sync,None)
-        r.setParams(symbol,market,page,page_size,fq,cycle)
+        r.setParams(symbol,market,page,page_size,fq,cycle,start,end,enable_cache)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
 
 
-    def get_finance(self,symbol,market:int,report_type:config.REPORT_TYPE=config.REPORT_TYPE.DEFAULT,report_date=""):
+    def get_finance(self,symbol,market:int,report_type:config.REPORT_TYPE=config.REPORT_TYPE.DEFAULT,report_date="",start:str=None,end:str=None,enable_cache:bool=True):
         """请求财务信息
 
         Args:
             symbol (str): 证券代码
             market (int): 市场代码
             report_type (config.REPORT_TYPE): 财务报表类型 
             class REPORT_TYPE:
@@ -460,61 +462,78 @@
             report_date (str): 报表日期 %Y-%m-%d，默认为空是取最新日期的报表
            
         Returns:
             dict: 财务数据
         """
         if not self.connected:return
         r =  GetFinanceParser(self.client)
-        r.setParams(symbol,market,report_type,report_date)
+        r.setParams(symbol,market,report_type,report_date,start,end,enable_cache)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
 
-    def get_sharebonus(self,symbol:str,market:int,start:str=None,end:str=None):
+    def get_sharebonus(self,symbol:str,market:int,start:str=None,end:str=None,enable_cache:bool=True):
         """请求分红配股信息
 
         Args:
             symbol (str): 证券代码
             market (int): 市场编号
             start (str, optional): 开始日期 %Y-%m-%d Defaults to None.
             end (str, optional): 结束日期 %Y-%m-%d. Defaults to None.
 
         Returns:
             _type_: _description_
         """
         if not self.connected:return
         r =  GetShareBonusParser(self.client)
-        r.setParams(symbol,market,start,end)
+        r.setParams(symbol,market,start,end,enable_cache)
+        return r.call_api()
+
+    def get_structure(self,symbol:str,market:int,start:str=None,end:str=None,enable_cache:bool=True):
+        """请求股本结构信息
+
+        Args:
+            symbol (str): 证券代码
+            market (int): 市场编号
+            start (str, optional): 开始日期 %Y-%m-%d Defaults to None.
+            end (str, optional): 结束日期 %Y-%m-%d. Defaults to None.
+
+        Returns:
+            _type_: _description_
+        """
+        if not self.connected:return
+        r =  GetStructureParser(self.client)
+        r.setParams(symbol,market,start,end,enable_cache)
         return r.call_api()
     
     def get_factors(self,symbol:str,market:int):
         """请求复权因子信息
 
         Args:
             symbol (str): 证券代码
             market (str): 市场代码
         """
         if not self.connected:return
         r =  GetFactorsParser(self.client)
         r.setParams(symbol,market)
         return r.call_api()
     
-    def get_timeshring(self,symbol:str,market:int,trade_date:str=""):
+    def get_timeshring(self,symbol:str,market:int,trade_date:str="",enable_cache:bool=True):
         """请求分时线
 
         Args:
             symbol (str): 证券代码
             market (int): 市场编号
             trade_date (str, optional): 交易日期 %Y-%m-%d. Defaults to "".
 
         Returns:
             _type_: _description_
         """
         if not self.connected:return
         r =  GetTimeSharingParser(self.client,self.sync,None)
-        r.setParams(symbol,market,trade_date)
+        r.setParams(symbol,market,trade_date,enable_cache)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
 
     def sub_timeshring(self,symbol:str,market:int,trade_date:str="",callback=None):
         """订阅分时线
         订阅后会主动推送每分钟的分时数据过来，用户需自行实现callback函数
 
@@ -529,24 +548,24 @@
         """
         if not self.connected:return
         r =  GetTimeSharingParser(self.client,self.sync,callback)
         r.setParams(symbol,market,trade_date)
         if(not self.sync): self.__save_api(r)
         return r.call_api()
     
-    def get_translist(self,symbol:str,market:int,trade_date:str="",page:int=1,page_size:int=10):
+    def get_translist(self,symbol:str,market:int,trade_date:str="",page:int=1,page_size:int=10,enable_cache:bool=True):
         """获取逐笔交易信息
 
         Args:
             symbol (str): 证券代码
             market (int): 市场编号
             trade_date (str, optional): 交易日期 %Y-%m-%d. Defaults to "".
             page (int, optional): 页码. Defaults to 1.
             page_size (int, optional): 每页大小. Defaults to 10.
 
         Returns:
             _type_: GetTransListParser
         """
         if not self.connected:return
         r =  GetTransListParser(self.client)
-        r.setParams(symbol,market,trade_date,page,page_size)
+        r.setParams(symbol,market,trade_date,page,page_size,enable_cache)
         return r.call_api()
```

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/models/quotes.py` & `dsxquant-2.0.0/src/dsxquant/dataser/models/quotes.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/base.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dsxquant.config import config
 import gzip
 import pandas
 from typing import Union,TypeVar,Callable
 
 from dsxquant.common.json2model import Json2Model
 from dsxquant.dataser.models.result import ResultModel
+from dsxquant.common.cache import CacheHelper
 
 T = TypeVar("T")
 
 class SocketClientNotReady(BaseException):
     pass
 
 class SendPkgNotReady(BaseException):
@@ -52,19 +53,26 @@
         self.request_id = fn.create_unique_id()
         # 发送后返回
         self.send_result = None
         # 定义接口协议名称
         self.api_name = None
         # 返回结果
         self.result:dict = None
+        # 缓存数据
+        self.cache = None
+        # 是否开启缓存
+        self.enable_cache = False
         # 设置好api的名称
         self.setApiName()
         
         # logger.debug("base parser init ...")
     
+    def open_cache(self):
+        self.enable_cache = True
+    
     def setApiName(self):
         pass
 
     def setParams(self, *args, **xargs):
         """
         构建请求
         :return:
@@ -116,14 +124,15 @@
         except json.JSONDecodeError as ex:
             logger.error(ex)
         except Exception as ex:
             logger.error(ex)
         self.result = result
         return self
     def _send(self):
+        if self.cache: return
         try:
             with BaseParser.lock:
                 # 设置一些公共信息
                 self.setup()
                 # 第一步：将json格式的数据转换为字符串
                 body_info = not self.send_datas == None and json.dumps(self.send_datas) or ''
                 # 第二步：对数据body_info进行编码为二进制数据
@@ -153,14 +162,19 @@
             logger.error(traceback.format_exc())
             logger.error(ex)
         # logger.debug("_send:"+self.send_result.__str__())
         # logger.debug(self.send_pkg)
 
     def _call_api(self):
 
+        # 如果有缓存，启用缓存数据
+        if self.cache:
+            result = ResultModel().show("缓存数据",True,0,self.cache,self.request_id,self.api_name).dict()
+            return result
+
         if self.send_result != len(self.send_pkg):
             logger.debug("send bytes error")
             raise SendRequestPkgFails("send fails")
         else:
             try:
                 with BaseParser.reclock:
                     # 接收客户端发送过来的数据，因为使用了struct模块中"i"模式，它对任何长度的数据加密出来的长度为固定4字节，所以接收这里使用4
@@ -211,27 +225,27 @@
     
     def dataframe(self) ->Union[pandas.DataFrame,pandas.Series]:
         """转成pandas对象
         """
         if self.result:
             data = "data" in self.result.keys() and self.result.get("data") or None
             if data:
-                if type(data)==list:
-                    return pandas.DataFrame(data)
+                if type(data)==dict:
+                    return pandas.DataFrame(data.values(),data.keys())
                 else:
                     return pandas.Series(data)
         return pandas.DataFrame()
     
     def series(self) ->Union[pandas.DataFrame,pandas.Series]:
         """转成pandas对象
         """
         if self.result:
             data = "data" in self.result.keys() and self.result.get("data") or None
             if data:
-                if type(data)==dict:
+                if type(data)==list:
                     return pandas.Series(data)
                 else:
                     return pandas.DataFrame(data)
         return pandas.Series()
     
     def csv(self,file_path:str=None) ->Union[list,dict ,None]:
         """转成csv文件格式
```

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/get_category.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_category.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/get_factors.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_factors.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/get_quotes.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_quotes.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/get_stocks.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_stocks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dsxquant.dataser.parser.base import BaseParser
 class GetStocksParser(BaseParser):
 
     def setApiName(self):
         self.api_name = "stocks"
     
-    def setParams(self,symbol:str=None,market:int=None,hangye:str=None,gainian:str=None,diyu:str=None,listing_date:str=None):
+    def setParams(self,symbol:str=None,market:int=None,hangye:str=None,gainian:str=None,diyu:str=None,listing_date:str=None,category:int=0):
         """构建请求参数
         Args:
             symbol (str): 证券代码
             market (int): 市场代码
             hangye (str): 行业名称 例如 汽车
             gainian (str): 概念名称 例如 5G
             diyu (str): 地域名称 例如 北京
@@ -17,14 +17,15 @@
         datas = self.transdata({
             "symbol":symbol,
             "market":market,
             "hangye":hangye,
             "gainian":gainian,
             "diyu":diyu,
             "listing_date":listing_date,
+            "category":category
 
         })
         self.send_datas = datas
         
     
     def parseResponse(self, datas):
         """解析返回的数据
```

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/get_translist.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/get_translist.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,50 @@
+import datetime
 from dsxquant.dataser.parser.base import BaseParser
+from dsxquant.common.cache import CacheHelper
 class GetTransListParser(BaseParser):
 
     def setApiName(self):
         self.api_name = "translist"
     
-    def setParams(self, symbol:str,market:int,trade_date:str="",page:int=1,page_size:int=10):
+    def setParams(self, symbol:str,market:int,trade_date:str="",page:int=1,page_size:int=10,enable_cache:bool=True):
         """构建请求参数
         Args:
             symbol (str): 证券代码
             market (int): 市场代码
             trade_date (str): 交易日期 Y-m-d
         """
+        self.enable_cache = enable_cache
+        self.symbol = symbol
+        self.market = market
+        self.trade_date = trade_date
         datas = self.transdata({
             "symbol":symbol,
             "market":market,
             "trade_date":trade_date,
             "page":page,
             "page_size":page_size
         })
         self.send_datas = datas
-        
+        if self.enable_cache:
+            self.cache = CacheHelper.get_translist(symbol,market,trade_date,page,page_size)
     
     def parseResponse(self, datas):
         """解析返回的数据
 
         Args:
             datas (str): 服务端返回
         """
 
         # logger.debug("parseResponse  "+__name__+" ")
+        # 保存缓存数据
+        if datas and self.enable_cache:
+            if datas["success"]:
+                data = datas["data"]
+                if data:
+                    if not self.trade_date:self.trade_date = datetime.datetime.now().strftime("%Y%m%d")
+                    CacheHelper.save_translist(self.symbol,self.market,self.trade_date,data)
 
         return datas
```

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/heart.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/heart.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/login.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/login.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/register.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/register.py`

 * *Files identical despite different names*

### Comparing `dsxquant-1.1.0/src/dsxquant/dataser/parser/sub_all_quotes.py` & `dsxquant-2.0.0/src/dsxquant/dataser/parser/sub_all_quotes.py`

 * *Files identical despite different names*

