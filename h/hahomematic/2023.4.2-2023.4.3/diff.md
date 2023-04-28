# Comparing `tmp/hahomematic-2023.4.2.tar.gz` & `tmp/hahomematic-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.4.2.tar", last modified: Mon Apr 24 18:05:07 2023, max compression
+gzip compressed data, was "hahomematic-2023.4.3.tar", last modified: Thu Apr 27 19:14:13 2023, max compression
```

## Comparing `hahomematic-2023.4.2.tar` & `hahomematic-2023.4.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 18:05:06.000000 hahomematic-2023.4.2/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:05:06.000000 hahomematic-2023.4.2/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:05:05.000000 hahomematic-2023.4.2/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.194172 hahomematic-2023.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-27 19:14:13.194172 hahomematic-2023.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.174172 hahomematic-2023.4.3/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.178173 hahomematic-2023.4.3/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.182173 hahomematic-2023.4.3/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.186173 hahomematic-2023.4.3/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28029 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.190173 hahomematic-2023.4.3/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.194172 hahomematic-2023.4.3/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.194172 hahomematic-2023.4.3/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:14:13.178173 hahomematic-2023.4.3/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-27 19:14:12.000000 hahomematic-2023.4.3/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-27 19:14:13.000000 hahomematic-2023.4.3/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:14:12.000000 hahomematic-2023.4.3/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:14:11.000000 hahomematic-2023.4.3/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 19:14:12.000000 hahomematic-2023.4.3/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 19:14:12.000000 hahomematic-2023.4.3/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-27 19:13:37.000000 hahomematic-2023.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-27 19:14:13.194172 hahomematic-2023.4.3/setup.cfg
```

### Comparing `hahomematic-2023.4.2/LICENSE` & `hahomematic-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/PKG-INFO` & `hahomematic-2023.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.2/README.md` & `hahomematic-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/__init__.py` & `hahomematic-2023.4.3/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/backport.py` & `hahomematic-2023.4.3/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/caches/dynamic.py` & `hahomematic-2023.4.3/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/caches/persistent.py` & `hahomematic-2023.4.3/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/caches/visibility.py` & `hahomematic-2023.4.3/hahomematic/caches/visibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     EVENT_CONFIG_PENDING,
     EVENT_ERROR,
     EVENT_STICKY_UN_REACH,
     EVENT_UN_REACH,
     EVENT_UPDATE_PENDING,
     FILE_CUSTOM_UN_IGNORE_PARAMETERS,
     PARAM_CHANNEL_OPERATION_MODE,
+    PARAM_DEVICE_OPERATION_MODE,
     PARAM_TEMPERATURE_MAXIMUM,
     PARAM_TEMPERATURE_MINIMUM,
     PARAMSET_KEY_MASTER,
     PARAMSET_KEY_VALUES,
     HmPlatform,
 )
 from hahomematic.platforms.custom.definition import get_required_parameters
@@ -42,14 +43,15 @@
     "HmIP-DRSI4": ((1, 2, 3, 4), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-DSD-PCB": ((1,), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-FCI1": ((1,), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-FCI6": (tuple(range(1, 7)), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-FSI16": ((1,), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-MIO16-PCB": ((13, 14, 15, 16), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIP-MOD-RC8": (tuple(range(1, 9)), (PARAM_CHANNEL_OPERATION_MODE,)),
+    "HmIP-RGBW": ((0,), (PARAM_DEVICE_OPERATION_MODE,)),
     "HmIPW-DRBL4": ((1, 5, 9, 13), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIPW-DRI16": (tuple(range(1, 17)), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIPW-DRI32": (tuple(range(1, 33)), (PARAM_CHANNEL_OPERATION_MODE,)),
     "HmIPW-FIO6": (tuple(range(1, 7)), (PARAM_CHANNEL_OPERATION_MODE,)),
     "ALPHA-IP-RBG": ((1,), (PARAM_TEMPERATURE_MAXIMUM, PARAM_TEMPERATURE_MINIMUM)),
     "HM-CC-RT-DN": ((1,), (PARAM_TEMPERATURE_MAXIMUM, PARAM_TEMPERATURE_MINIMUM)),
     "HM-CC-VG-1": ((1,), (PARAM_TEMPERATURE_MAXIMUM, PARAM_TEMPERATURE_MINIMUM)),
```

### Comparing `hahomematic-2023.4.2/hahomematic/central_unit.py` & `hahomematic-2023.4.3/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/client.py` & `hahomematic-2023.4.3/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/const.py` & `hahomematic-2023.4.3/hahomematic/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 
 OPERATION_NONE: Final = 0
 OPERATION_READ: Final = 1
 OPERATION_WRITE: Final = 2
 OPERATION_EVENT: Final = 4
 
 PARAM_CHANNEL_OPERATION_MODE: Final = "CHANNEL_OPERATION_MODE"
+PARAM_DEVICE_OPERATION_MODE: Final = "DEVICE_OPERATION_MODE"
 PARAM_TEMPERATURE_MAXIMUM: Final = "TEMPERATURE_MAXIMUM"
 PARAM_TEMPERATURE_MINIMUM: Final = "TEMPERATURE_MINIMUM"
 
 PARAMSET_KEY_MASTER: Final = "MASTER"
 PARAMSET_KEY_VALUES: Final = "VALUES"
 
 PROGRAM_ID: Final = "id"
```

### Comparing `hahomematic-2023.4.2/hahomematic/decorators.py` & `hahomematic-2023.4.3/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/exceptions.py` & `hahomematic-2023.4.3/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/exporter.py` & `hahomematic-2023.4.3/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/hmcli.py` & `hahomematic-2023.4.3/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/json_rpc_client.py` & `hahomematic-2023.4.3/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/__init__.py` & `hahomematic-2023.4.3/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/const.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     """Enum for entity definitions."""
 
     IP_COVER = "IPCover"
     IP_DIMMER = "IPDimmer"
     IP_FIXED_COLOR_LIGHT = "IPFixedColorLight"
     IP_GARAGE = "IPGarage"
     IP_LOCK = "IPLock"
+    IP_RGBW_LIGHT = "IPRGBW"
     IP_SIMPLE_FIXED_COLOR_LIGHT = "IPSimpleFixedColorLight"
     IP_SIREN = "IPSiren"
     IP_SIREN_SMOKE = "IPSirenSmoke"
     IP_SWITCH = "IPSwitch"
     IP_THERMOSTAT = "IPThermostat"
     IP_THERMOSTAT_GROUP = "IPThermostatGroup"
     RF_COVER = "RfCover"
@@ -42,28 +43,32 @@
 FIELD_CHANNEL_LEVEL: Final = "channel_level"
 FIELD_CHANNEL_LEVEL_2: Final = "channel_level_2"
 FIELD_CHANNEL_OPERATION_MODE: Final = "channel_operation_mode"
 FIELD_CHANNEL_STATE: Final = "channel_state"
 FIELD_COLOR: Final = "color"
 FIELD_COLOR_LEVEL: Final = "color_temp"
 FIELD_COMBINED_PARAMETER = "combined_parameter"
+FIELD_COLOR_TEMPERATURE = "color_temperature"
 FIELD_COMFORT_MODE: Final = "comfort_mode"
 FIELD_CONTROL_MODE: Final = "control_mode"
 FIELD_CURRENT: Final = "current"
+FIELD_DEVICE_OPERATION_MODE = "device_operation_mode"
 FIELD_DIRECTION: Final = "direction"
 FIELD_DOOR_COMMAND: Final = "door_command"
 FIELD_DOOR_STATE: Final = "door_state"
 FIELD_DURATION: Final = "duration"
 FIELD_DURATION_UNIT: Final = "duration_unit"
 FIELD_DUTYCYCLE: Final = "dutycycle"
 FIELD_DUTY_CYCLE: Final = "duty_cycle"
+FIELD_EFFECT = "effect"
 FIELD_ENERGY_COUNTER: Final = "energy_counter"
 FIELD_ERROR: Final = "error"
 FIELD_FREQUENCY: Final = "frequency"
 FIELD_HEATING_COOLING: Final = "heating_cooling"
+FIELD_HUE = "hue"
 FIELD_HUMIDITY: Final = "humidity"
 FIELD_INHIBIT: Final = "inhibit"
 FIELD_LEVEL: Final = "level"
 FIELD_LEVEL_2: Final = "level_2"
 FIELD_LEVEL_COMBINED: Final = "level_combined"
 FIELD_LOCK_STATE: Final = "lock_state"
 FIELD_LOCK_TARGET_LEVEL: Final = "lock_target_level"
@@ -76,19 +81,22 @@
 FIELD_OPEN: Final = "open"
 FIELD_OPERATING_VOLTAGE: Final = "operating_voltage"
 FIELD_OPTICAL_ALARM_ACTIVE: Final = "optical_alarm_active"
 FIELD_OPTICAL_ALARM_SELECTION: Final = "optical_alarm_selection"
 FIELD_PARTY_MODE: Final = "party_mode"
 FIELD_POWER: Final = "power"
 FIELD_PROGRAM: Final = "program"
+FIELD_RAMP_TIME_TO_OFF_UNIT = "ramp_time_to_off_unit"
+FIELD_RAMP_TIME_TO_OFF_VALUE = "ramp_time_to_off_value"
 FIELD_RAMP_TIME_UNIT: Final = "ramp_time_unit"
 FIELD_RAMP_TIME_VALUE: Final = "ramp_time_value"
 FIELD_RSSI_DEVICE: Final = "rssi_device"
 FIELD_RSSI_PEER: Final = "rssi_peer"
 FIELD_SABOTAGE: Final = "sabotage"
+FIELD_SATURATION = "saturation"
 FIELD_SECTION: Final = "section"
 FIELD_SETPOINT: Final = "setpoint"
 FIELD_SET_POINT_MODE: Final = "set_point_mode"
 FIELD_SMOKE_DETECTOR_ALARM_STATUS = "smoke_detector_alarm_status"
 FIELD_SMOKE_DETECTOR_COMMAND = "smoke_detector_command"
 FIELD_STATE: Final = "state"
 FIELD_STOP: Final = "stop"
```

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,28 @@
     FIELD_CHANNEL_COLOR,
     FIELD_CHANNEL_LEVEL,
     FIELD_CHANNEL_LEVEL_2,
     FIELD_CHANNEL_OPERATION_MODE,
     FIELD_CHANNEL_STATE,
     FIELD_COLOR,
     FIELD_COLOR_LEVEL,
+    FIELD_COLOR_TEMPERATURE,
     FIELD_COMBINED_PARAMETER,
     FIELD_COMFORT_MODE,
     FIELD_CONTROL_MODE,
+    FIELD_DEVICE_OPERATION_MODE,
     FIELD_DIRECTION,
     FIELD_DOOR_COMMAND,
     FIELD_DOOR_STATE,
     FIELD_DURATION,
     FIELD_DURATION_UNIT,
+    FIELD_EFFECT,
     FIELD_ERROR,
     FIELD_HEATING_COOLING,
+    FIELD_HUE,
     FIELD_HUMIDITY,
     FIELD_LEVEL,
     FIELD_LEVEL_2,
     FIELD_LEVEL_COMBINED,
     FIELD_LOCK_STATE,
     FIELD_LOCK_TARGET_LEVEL,
     FIELD_LOWERING_MODE,
@@ -44,16 +48,19 @@
     FIELD_ON_TIME_UNIT,
     FIELD_ON_TIME_VALUE,
     FIELD_OPEN,
     FIELD_OPTICAL_ALARM_ACTIVE,
     FIELD_OPTICAL_ALARM_SELECTION,
     FIELD_PARTY_MODE,
     FIELD_PROGRAM,
+    FIELD_RAMP_TIME_TO_OFF_UNIT,
+    FIELD_RAMP_TIME_TO_OFF_VALUE,
     FIELD_RAMP_TIME_UNIT,
     FIELD_RAMP_TIME_VALUE,
+    FIELD_SATURATION,
     FIELD_SECTION,
     FIELD_SET_POINT_MODE,
     FIELD_SETPOINT,
     FIELD_SMOKE_DETECTOR_ALARM_STATUS,
     FIELD_SMOKE_DETECTOR_COMMAND,
     FIELD_STATE,
     FIELD_STOP,
@@ -218,14 +225,39 @@
                     FIELD_ON_TIME_UNIT: "DURATION_UNIT",
                     FIELD_ON_TIME_VALUE: "DURATION_VALUE",
                     FIELD_RAMP_TIME_UNIT: "RAMP_TIME_UNIT",
                     FIELD_RAMP_TIME_VALUE: "RAMP_TIME_VALUE",
                 },
             },
         },
+        HmEntityDefinition.IP_RGBW_LIGHT: {
+            ED_DEVICE_GROUP: {
+                ED_PRIMARY_CHANNEL: 2,
+                ED_SECONDARY_CHANNELS: (3, 4),
+                ED_REPEATABLE_FIELDS: {
+                    FIELD_DIRECTION: "ACTIVITY_STATE",
+                    FIELD_COLOR_TEMPERATURE: "COLOR_TEMPERATURE",
+                    FIELD_ON_TIME_UNIT: "DURATION_UNIT",
+                    FIELD_ON_TIME_VALUE: "DURATION_VALUE",
+                    FIELD_EFFECT: "EFFECT",
+                    FIELD_HUE: "HUE",
+                    FIELD_LEVEL: "LEVEL",
+                    FIELD_RAMP_TIME_TO_OFF_UNIT: "RAMP_TIME_TO_OFF_UNIT",
+                    FIELD_RAMP_TIME_TO_OFF_VALUE: "RAMP_TIME_TO_OFF_VALUE",
+                    FIELD_RAMP_TIME_UNIT: "RAMP_TIME_UNIT",
+                    FIELD_RAMP_TIME_VALUE: "RAMP_TIME_VALUE",
+                    FIELD_SATURATION: "SATURATION",
+                },
+                ED_FIELDS: {
+                    0: {
+                        FIELD_DEVICE_OPERATION_MODE: "DEVICE_OPERATION_MODE",
+                    },
+                },
+            },
+        },
         HmEntityDefinition.IP_SWITCH: {
             ED_DEVICE_GROUP: {
                 ED_PRIMARY_CHANNEL: 1,
                 ED_SECONDARY_CHANNELS: (2, 3),
                 ED_REPEATABLE_FIELDS: {
                     FIELD_STATE: "STATE",
                     FIELD_ON_TIME_VALUE: "ON_TIME",
```

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/light.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/light.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 Module for entities implemented using the light platform.
 
 See https://www.home-assistant.io/integrations/light/.
 """
 from __future__ import annotations
 
 from abc import abstractmethod
+import math
 from typing import Any, Final, TypedDict
 
 from hahomematic.const import HM_ARG_OFF, HM_ARG_ON, HM_ARG_ON_TIME, HmPlatform
 from hahomematic.decorators import bind_collector
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import (
     FIELD_CHANNEL_COLOR,
     FIELD_CHANNEL_LEVEL,
     FIELD_COLOR,
     FIELD_COLOR_LEVEL,
+    FIELD_COLOR_TEMPERATURE,
+    FIELD_DEVICE_OPERATION_MODE,
+    FIELD_DIRECTION,
+    FIELD_EFFECT,
+    FIELD_HUE,
     FIELD_LEVEL,
     FIELD_ON_TIME_UNIT,
     FIELD_ON_TIME_VALUE,
     FIELD_PROGRAM,
+    FIELD_RAMP_TIME_TO_OFF_UNIT,
+    FIELD_RAMP_TIME_TO_OFF_VALUE,
     FIELD_RAMP_TIME_UNIT,
     FIELD_RAMP_TIME_VALUE,
+    FIELD_SATURATION,
     HmEntityDefinition,
 )
 from hahomematic.platforms.custom.entity import CustomEntity
 from hahomematic.platforms.custom.support import CustomConfig, ExtendedConfig
 from hahomematic.platforms.entity import CallParameterCollector
 from hahomematic.platforms.generic.action import HmAction
 from hahomematic.platforms.generic.number import HmFloat, HmInteger
@@ -39,14 +48,19 @@
 _HM_ARG_COLOR_TEMP: Final = "color_temp"
 _HM_ARG_CHANNEL_COLOR: Final = "channel_color"
 _HM_ARG_CHANNEL_LEVEL: Final = "channel_level"
 _HM_ARG_EFFECT: Final = "effect"
 _HM_ARG_HS_COLOR: Final = "hs_color"
 _HM_ARG_RAMP_TIME: Final = "ramp_time"
 
+_DOM_PWM: Final = "PWM"
+_DOM_RGB: Final = "RGB"
+_DOM_RGBW: Final = "RGBW"
+_DOM_TUNABLE_WHITE: Final = "TUNABLE_WHITE"
+
 HM_EFFECT_OFF: Final = "Off"
 
 HM_MAX_MIREDS: Final = 500
 HM_MIN_MIREDS: Final = 153
 
 HM_DIMMER_OFF: Final = 0.0
 
@@ -145,15 +159,15 @@
         collector: CallParameterCollector | None = None,
         **kwargs: Any,
     ) -> None:
         """Turn the light on."""
         if not self.is_state_change(on=True, **kwargs):
             return
         if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
-            await self._set_ramp_time_value(ramp_time=float(ramp_time), collector=collector)
+            await self._set_ramp_time_on_value(ramp_time=float(ramp_time), collector=collector)
         if (on_time := kwargs.get(HM_ARG_ON_TIME)) or (on_time := self.get_on_time_and_cleanup()):
             await self._set_on_time_value(on_time=on_time, collector=collector)
 
         brightness = kwargs.get(_HM_ARG_BRIGHTNESS, self.brightness)
         if not brightness:
             brightness = 255
         level = brightness / 255.0
@@ -163,31 +177,37 @@
     async def turn_off(
         self, collector: CallParameterCollector | None = None, **kwargs: Any
     ) -> None:
         """Turn the light off."""
         if not self.is_state_change(off=True, **kwargs):
             return
         if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
-            await self._set_ramp_time_value(ramp_time=float(ramp_time), collector=collector)
+            await self._set_ramp_time_off_value(ramp_time=float(ramp_time), collector=collector)
 
         await self._e_level.send_value(value=HM_DIMMER_OFF, collector=collector)
 
     @bind_collector
     async def _set_on_time_value(
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         await self._e_on_time_value.send_value(value=on_time, collector=collector)
 
-    async def _set_ramp_time_value(
+    async def _set_ramp_time_on_value(
         self, ramp_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the ramp time value in seconds."""
         await self._e_ramp_time_value.send_value(value=ramp_time, collector=collector)
 
+    async def _set_ramp_time_off_value(
+        self, ramp_time: float, collector: CallParameterCollector | None = None
+    ) -> None:
+        """Set the ramp time value in seconds."""
+        await self._set_ramp_time_on_value(ramp_time=ramp_time, collector=collector)
+
     def is_state_change(self, **kwargs: Any) -> bool:
         """Check if the state changes due to kwargs."""
         if kwargs.get(HM_ARG_ON) is not None and self.is_on is not True and len(kwargs) == 1:
             return True
         if kwargs.get(HM_ARG_OFF) is not None and self.is_on is not False and len(kwargs) == 1:
             return True
         if (
@@ -374,14 +394,207 @@
         if (color_temp := kwargs.get(_HM_ARG_COLOR_TEMP)) is not None:
             color_level = (HM_MAX_MIREDS - color_temp) / (HM_MAX_MIREDS - HM_MIN_MIREDS)
             await self._e_color_level.send_value(value=color_level, collector=collector)
 
         await super().turn_on(collector=collector, **kwargs)
 
 
+class CeIpRGBWLight(BaseHmLight):
+    """Class for HomematicIP HmIP-RGBW light entities."""
+
+    def _init_entity_fields(self) -> None:
+        """Init the entity fields."""
+        OnTimeMixin.__init__(self)
+        self._e_activity_state: HmSelect = self._get_entity(
+            field_name=FIELD_DIRECTION, entity_type=HmSelect
+        )
+        self._e_color_temperature_kelvin: HmInteger = self._get_entity(
+            field_name=FIELD_COLOR_TEMPERATURE, entity_type=HmInteger
+        )
+        self._e_on_time_value: HmAction = self._get_entity(
+            field_name=FIELD_ON_TIME_VALUE, entity_type=HmAction
+        )
+        self._e_on_time_unit: HmAction = self._get_entity(
+            field_name=FIELD_ON_TIME_UNIT, entity_type=HmAction
+        )
+        self._e_device_operation_mode: HmSelect = self._get_entity(
+            field_name=FIELD_DEVICE_OPERATION_MODE, entity_type=HmSelect
+        )
+        self._e_effect: HmAction = self._get_entity(field_name=FIELD_EFFECT, entity_type=HmAction)
+        self._e_hue: HmInteger = self._get_entity(field_name=FIELD_HUE, entity_type=HmInteger)
+        self._e_level: HmFloat = self._get_entity(field_name=FIELD_LEVEL, entity_type=HmFloat)
+        self._e_ramp_time_to_off_unit: HmAction = self._get_entity(
+            field_name=FIELD_RAMP_TIME_TO_OFF_UNIT, entity_type=HmAction
+        )
+        self._e_ramp_time_to_off_value: HmAction = self._get_entity(
+            field_name=FIELD_RAMP_TIME_TO_OFF_VALUE, entity_type=HmAction
+        )
+        self._e_ramp_time_value: HmAction = self._get_entity(
+            field_name=FIELD_RAMP_TIME_VALUE, entity_type=HmAction
+        )
+        self._e_ramp_time_unit: HmAction = self._get_entity(
+            field_name=FIELD_RAMP_TIME_UNIT, entity_type=HmAction
+        )
+        self._e_saturation: HmFloat = self._get_entity(
+            field_name=FIELD_SATURATION, entity_type=HmFloat
+        )
+
+    @value_property
+    def is_on(self) -> bool | None:
+        """Return true if light is on."""
+        return self._e_level.value is not None and self._e_level.value > HM_DIMMER_OFF
+
+    @value_property
+    def brightness(self) -> int | None:
+        """Return the brightness of this light between 0..255."""
+        return int((self._e_level.value or 0.0) * 255)
+
+    @value_property
+    def color_temp(self) -> int | None:
+        """Return the color temperature in mireds of this light between 153..500."""
+        if self._e_color_temperature_kelvin.value is None:
+            return None
+        return math.floor(1000000 / self._e_color_temperature_kelvin.value)
+
+    @value_property
+    def hs_color(self) -> tuple[float, float] | None:
+        """Return the hue and saturation color value [float, float]."""
+        if self._e_hue.value is not None and self._e_saturation.value is not None:
+            return self._e_hue.value, self._e_saturation.value * 100
+        return None
+
+    @config_property
+    def supports_brightness(self) -> bool:
+        """Flag if light supports brightness."""
+        return True
+
+    @config_property
+    def supports_color_temperature(self) -> bool:
+        """Flag if light supports color temperature."""
+        return self._e_device_operation_mode.value in (_DOM_RGBW, _DOM_TUNABLE_WHITE)
+
+    @config_property
+    def supports_effects(self) -> bool:
+        """Flag if light supports effects."""
+        return True
+
+    @config_property
+    def supports_hs_color(self) -> bool:
+        """Flag if light supports color."""
+        return self._e_device_operation_mode.value in (_DOM_RGBW, _DOM_RGB)
+
+    @config_property
+    def supports_transition(self) -> bool:
+        """Flag if light supports transition."""
+        return True
+
+    @value_property
+    def effect(self) -> str | None:
+        """Return the current effect."""
+        return None
+
+    @value_property
+    def effect_list(self) -> list[str] | None:
+        """Return the list of supported effects."""
+        return list(self._e_effect.value_list or ())
+
+    @bind_collector
+    async def turn_on(
+        self,
+        collector: CallParameterCollector | None = None,
+        **kwargs: Any,
+    ) -> None:
+        """Turn the light on."""
+        if not self.is_state_change(on=True, **kwargs):
+            return
+        if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
+            await self._set_ramp_time_on_value(ramp_time=float(ramp_time), collector=collector)
+        if (on_time := kwargs.get(HM_ARG_ON_TIME)) or (on_time := self.get_on_time_and_cleanup()):
+            await self._set_on_time_value(on_time=on_time, collector=collector)
+        if (hs_color := kwargs.get(_HM_ARG_HS_COLOR)) is not None:
+            hue, ksaturation = hs_color
+            saturation = ksaturation / 100
+            await self._e_hue.send_value(value=int(hue), collector=collector)
+            await self._e_saturation.send_value(value=saturation, collector=collector)
+        if (color_temp := kwargs.get(_HM_ARG_COLOR_TEMP)) is not None:
+            color_temp_kelvin = math.floor(1000000 / color_temp)
+            await self._e_color_temperature_kelvin.send_value(
+                value=color_temp_kelvin, collector=collector
+            )
+        if self.supports_effects and (effect := kwargs.get(_HM_ARG_EFFECT)) is not None:
+            await self._e_effect.send_value(value=effect, collector=collector)
+
+        brightness = kwargs.get(_HM_ARG_BRIGHTNESS, self.brightness)
+        if not brightness:
+            brightness = 255
+        level = brightness / 255.0
+        await self._e_level.send_value(value=level, collector=collector)
+
+    @bind_collector
+    async def turn_off(
+        self, collector: CallParameterCollector | None = None, **kwargs: Any
+    ) -> None:
+        """Turn the light off."""
+        if not self.is_state_change(off=True, **kwargs):
+            return
+        if ramp_time := kwargs.get(_HM_ARG_RAMP_TIME):
+            await self._set_ramp_time_off_value(ramp_time=float(ramp_time), collector=collector)
+
+        await self._e_level.send_value(value=HM_DIMMER_OFF, collector=collector)
+
+    @bind_collector
+    async def _set_on_time_value(
+        self, on_time: float, collector: CallParameterCollector | None = None
+    ) -> None:
+        """Set the on time value in seconds."""
+        on_time, on_time_unit = _recalc_unit_timer(time=on_time)
+        await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
+        await self._e_on_time_value.send_value(value=float(on_time), collector=collector)
+
+    async def _set_ramp_time_on_value(
+        self, ramp_time: float, collector: CallParameterCollector | None = None
+    ) -> None:
+        """Set the ramp time value in seconds."""
+        ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
+        await self._e_ramp_time_unit.send_value(value=ramp_time_unit, collector=collector)
+        await self._e_ramp_time_value.send_value(value=float(ramp_time), collector=collector)
+
+    async def _set_ramp_time_off_value(
+        self, ramp_time: float, collector: CallParameterCollector | None = None
+    ) -> None:
+        """Set the ramp time value in seconds."""
+        ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
+        await self._e_ramp_time_to_off_unit.send_value(value=ramp_time_unit, collector=collector)
+        await self._e_ramp_time_to_off_value.send_value(
+            value=float(ramp_time), collector=collector
+        )
+
+    def is_state_change(self, **kwargs: Any) -> bool:
+        """Check if the state changes due to kwargs."""
+        if kwargs.get(HM_ARG_ON) is not None and self.is_on is not True and len(kwargs) == 1:
+            return True
+        if kwargs.get(HM_ARG_OFF) is not None and self.is_on is not False and len(kwargs) == 1:
+            return True
+        if (
+            brightness := kwargs.get(_HM_ARG_BRIGHTNESS)
+        ) is not None and brightness != self.brightness:
+            return True
+        if (hs_color := kwargs.get(_HM_ARG_HS_COLOR)) is not None and hs_color != self.hs_color:
+            return True
+        if (
+            color_temp := kwargs.get(_HM_ARG_COLOR_TEMP)
+        ) is not None and color_temp != self.color_temp:
+            return True
+        if kwargs.get(_HM_ARG_RAMP_TIME) is not None:
+            return True
+        if kwargs.get(HM_ARG_ON_TIME) is not None:
+            return True
+        return super().is_state_change(**kwargs)
+
+
 class CeIpFixedColorLight(BaseHmLight):
     """Class for HomematicIP HmIP-BSL, HmIPW-WRC6 light entities."""
 
     _color_switcher: dict[str, tuple[float, float]] = {
         "WHITE": (0.0, 0.0),
         "RED": (0.0, 100.0),
         "YELLOW": (60.0, 100.0),
@@ -476,15 +689,15 @@
         self, on_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the on time value in seconds."""
         on_time, on_time_unit = _recalc_unit_timer(time=on_time)
         await self._e_on_time_unit.send_value(value=on_time_unit, collector=collector)
         await self._e_on_time_value.send_value(value=float(on_time), collector=collector)
 
-    async def _set_ramp_time_value(
+    async def _set_ramp_time_on_value(
         self, ramp_time: float, collector: CallParameterCollector | None = None
     ) -> None:
         """Set the ramp time value in seconds."""
         ramp_time, ramp_time_unit = _recalc_unit_timer(time=ramp_time)
         await self._e_ramp_time_unit.send_value(value=ramp_time_unit, collector=collector)
         await self._e_ramp_time_value.send_value(value=float(ramp_time), collector=collector)
 
@@ -641,14 +854,29 @@
         custom_entity_class=CeIpFixedColorLight,
         device_enum=HmEntityDefinition.IP_SIMPLE_FIXED_COLOR_LIGHT,
         group_base_channels=group_base_channels,
         extended=extended,
     )
 
 
+def make_ip_rgbw_light(
+    device: hmd.HmDevice,
+    group_base_channels: tuple[int, ...],
+    extended: ExtendedConfig | None = None,
+) -> tuple[CustomEntity, ...]:
+    """Create simple fixed color light entities like HmIP-RGBW."""
+    return hmed.make_custom_entity(
+        device=device,
+        custom_entity_class=CeIpRGBWLight,
+        device_enum=HmEntityDefinition.IP_RGBW_LIGHT,
+        group_base_channels=group_base_channels,
+        extended=extended,
+    )
+
+
 # Case for device model is not relevant
 DEVICES: dict[str, CustomConfig | tuple[CustomConfig, ...]] = {
     "263 132": CustomConfig(func=make_rf_dimmer, channels=(1,)),
     "263 133": CustomConfig(func=make_rf_dimmer_with_virt_channel, channels=(1,)),
     "263 134": CustomConfig(func=make_rf_dimmer, channels=(1,)),
     "HBW-LC-RGBWW-IN6-DR": (
         CustomConfig(
@@ -720,14 +948,15 @@
             additional_entities={
                 0: ("ACTUAL_TEMPERATURE",),
             }
         ),
     ),
     "HmIP-FDT": CustomConfig(func=make_ip_dimmer, channels=(1,)),
     "HmIP-PDT": CustomConfig(func=make_ip_dimmer, channels=(2,)),
+    "HmIP-RGBW": CustomConfig(func=make_ip_rgbw_light, channels=(0,)),
     "HmIP-SCTH230": CustomConfig(
         func=make_ip_dimmer,
         channels=(11,),
         extended=ExtendedConfig(
             additional_entities={
                 1: ("CONCENTRATION",),
                 4: (
```

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/support.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.4.3/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/device.py` & `hahomematic-2023.4.3/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/entity.py` & `hahomematic-2023.4.3/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/event.py` & `hahomematic-2023.4.3/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/action.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/button.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/number.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/select.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.4.3/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/button.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/number.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/select.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/hub/text.py` & `hahomematic-2023.4.3/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/platforms/support.py` & `hahomematic-2023.4.3/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.4.3/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.4.3/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.4.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/support.py` & `hahomematic-2023.4.3/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.4.3/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic/xml_rpc_server.py` & `hahomematic-2023.4.3/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.4.3/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.2/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.4.3/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.2/pyproject.toml` & `hahomematic-2023.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.4.2"
+version     = "2023.4.3"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

