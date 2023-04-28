# Comparing `tmp/estimenergy-1.9.2.tar.gz` & `tmp/estimenergy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-1.9.2.tar", max compression
+gzip compressed data, was "estimenergy-2.0.0.tar", max compression
```

## Comparing `estimenergy-1.9.2.tar` & `estimenergy-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,46 @@
--rw-r--r--   0        0        0     1089 2023-03-10 13:35:51.710370 estimenergy-1.9.2/LICENSE
--rw-r--r--   0        0        0     2705 2023-03-10 13:35:51.710370 estimenergy-1.9.2/README.md
--rw-r--r--   0        0        0        0 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/__init__.py
--rw-r--r--   0        0        0       37 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      972 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/client/client.py
--rw-r--r--   0        0        0       74 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/__init__.py
--rw-r--r--   0        0        0      238 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/collector.py
--rw-r--r--   0        0        0     4461 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/collectors/glow_collector.py
--rw-r--r--   0        0        0      598 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/common.py
--rw-r--r--   0        0        0     4896 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/const.py
--rw-r--r--   0        0        0      582 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/helpers.py
--rw-r--r--   0        0        0     2468 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/main.py
--rw-r--r--   0        0        0       47 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/metrics/__init__.py
--rw-r--r--   0        0        0      873 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/metrics/collector_metrics.py
--rw-r--r--   0        0        0      110 2023-03-10 13:35:51.710370 estimenergy-1.9.2/estimenergy/models/__init__.py
--rw-r--r--   0        0        0     6861 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/collector_data.py
--rw-r--r--   0        0        0      711 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/energy_data.py
--rw-r--r--   0        0        0      381 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/models/settings.py
--rw-r--r--   0        0        0        0 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0      270 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/collector_router.py
--rw-r--r--   0        0        0      255 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/routers/energy_router.py
--rw-r--r--   0        0        0       85 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/__init__.py
--rw-r--r--   0        0        0      184 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/collector_schema.py
--rw-r--r--   0        0        0      172 2023-03-10 13:35:51.714370 estimenergy-1.9.2/estimenergy/schemas/energy_schema.py
--rw-r--r--   0        0        0     1173 2023-03-10 13:36:19.246579 estimenergy-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 estimenergy-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-28 13:23:32.168234 estimenergy-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4481 2023-04-28 13:23:32.168234 estimenergy-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/client/__init__.py
+-rw-r--r--   0        0        0      631 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/client/client.py
+-rw-r--r--   0        0        0      451 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/config.py
+-rw-r--r--   0        0        0     6030 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/const.py
+-rw-r--r--   0        0        0      665 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/db.py
+-rw-r--r--   0        0        0      133 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/devices/__init__.py
+-rw-r--r--   0        0        0     3108 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/devices/base_device.py
+-rw-r--r--   0        0        0       99 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/devices/device_error.py
+-rw-r--r--   0        0        0     4048 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/devices/device_registry.py
+-rw-r--r--   0        0        0     6177 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/devices/glow_device.py
+-rw-r--r--   0        0        0      540 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/helpers.py
+-rw-r--r--   0        0        0      318 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/influx.py
+-rw-r--r--   0        0        0      613 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/log.py
+-rw-r--r--   0        0        0     2088 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/main.py
+-rw-r--r--   0        0        0       94 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/__init__.py
+-rw-r--r--   0        0        0     1500 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/config.py
+-rw-r--r--   0        0        0       86 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/dev_config.py
+-rw-r--r--   0        0        0      138 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/influx_config.py
+-rw-r--r--   0        0        0      208 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/logging_config.py
+-rw-r--r--   0        0        0      212 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/networking_config.py
+-rw-r--r--   0        0        0      186 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/config/sql_config.py
+-rw-r--r--   0        0        0      896 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/day.py
+-rw-r--r--   0        0        0      912 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/device_config.py
+-rw-r--r--   0        0        0       76 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/message.py
+-rw-r--r--   0        0        0      874 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/month.py
+-rw-r--r--   0        0        0      335 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/total.py
+-rw-r--r--   0        0        0      799 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/models/year.py
+-rw-r--r--   0        0        0      479 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/prometheus.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/day_router.py
+-rw-r--r--   0        0        0     4293 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/device_router.py
+-rw-r--r--   0        0        0     1466 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/month_router.py
+-rw-r--r--   0        0        0     1466 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/total_router.py
+-rw-r--r--   0        0        0     1436 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/routers/year_router.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/data_service.py
+-rw-r--r--   0        0        0     3098 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/influx_service.py
+-rw-r--r--   0        0        0     4486 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/prediction_service.py
+-rw-r--r--   0        0        0     1725 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/prometheus_service.py
+-rw-r--r--   0        0        0    15611 2023-04-28 13:23:32.172234 estimenergy-2.0.0/estimenergy/services/sql_service.py
+-rw-r--r--   0        0        0     2495 2023-04-28 13:24:03.444681 estimenergy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.0/PKG-INFO
```

### Comparing `estimenergy-1.9.2/LICENSE` & `estimenergy-2.0.0/LICENSE`

 * *Files identical despite different names*

