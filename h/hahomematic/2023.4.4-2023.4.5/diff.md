# Comparing `tmp/hahomematic-2023.4.4.tar.gz` & `tmp/hahomematic-2023.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.4.4.tar", last modified: Fri Apr 28 07:49:30 2023, max compression
+gzip compressed data, was "hahomematic-2023.4.5.tar", last modified: Fri Apr 28 18:27:42 2023, max compression
```

## Comparing `hahomematic-2023.4.4.tar` & `hahomematic-2023.4.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.612271 hahomematic-2023.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 07:49:30.612271 hahomematic-2023.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.604270 hahomematic-2023.4.4/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.608271 hahomematic-2023.4.4/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.608271 hahomematic-2023.4.4/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.608271 hahomematic-2023.4.4/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    28032 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.608271 hahomematic-2023.4.4/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.608271 hahomematic-2023.4.4/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.612271 hahomematic-2023.4.4/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:49:30.604270 hahomematic-2023.4.4/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 07:49:29.000000 hahomematic-2023.4.4/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-28 07:49:30.000000 hahomematic-2023.4.4/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:49:29.000000 hahomematic-2023.4.4/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:49:28.000000 hahomematic-2023.4.4/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 07:49:30.000000 hahomematic-2023.4.4/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 07:49:30.000000 hahomematic-2023.4.4/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-28 07:48:52.000000 hahomematic-2023.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 07:49:30.612271 hahomematic-2023.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.508555 hahomematic-2023.4.5/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28032 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36970 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:27:42.512555 hahomematic-2023.4.5/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-28 18:27:41.000000 hahomematic-2023.4.5/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:27:41.000000 hahomematic-2023.4.5/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:27:40.000000 hahomematic-2023.4.5/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 18:27:42.000000 hahomematic-2023.4.5/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-28 18:27:11.000000 hahomematic-2023.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 18:27:42.516555 hahomematic-2023.4.5/setup.cfg
```

### Comparing `hahomematic-2023.4.4/LICENSE` & `hahomematic-2023.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/PKG-INFO` & `hahomematic-2023.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.4/README.md` & `hahomematic-2023.4.5/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/__init__.py` & `hahomematic-2023.4.5/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/backport.py` & `hahomematic-2023.4.5/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/caches/dynamic.py` & `hahomematic-2023.4.5/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/caches/persistent.py` & `hahomematic-2023.4.5/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/caches/visibility.py` & `hahomematic-2023.4.5/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/central_unit.py` & `hahomematic-2023.4.5/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/client.py` & `hahomematic-2023.4.5/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/const.py` & `hahomematic-2023.4.5/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/decorators.py` & `hahomematic-2023.4.5/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/exceptions.py` & `hahomematic-2023.4.5/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/exporter.py` & `hahomematic-2023.4.5/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/hmcli.py` & `hahomematic-2023.4.5/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/json_rpc_client.py` & `hahomematic-2023.4.5/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/__init__.py` & `hahomematic-2023.4.5/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/const.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/light.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/light.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     def brightness(self) -> int | None:
         """Return the brightness of this light between 0..255."""
         return int((self._e_level.value or 0.0) * 255)
 
     @value_property
     def color_temp(self) -> int | None:
         """Return the color temperature in mireds of this light between 153..500."""
-        if self._e_color_temperature_kelvin.value is None:
+        if not self._e_color_temperature_kelvin.value:
             return None
         return math.floor(1000000 / self._e_color_temperature_kelvin.value)
 
     @value_property
     def hs_color(self) -> tuple[float, float] | None:
         """Return the hue and saturation color value [float, float]."""
         if self._e_hue.value is not None and self._e_saturation.value is not None:
@@ -466,15 +466,15 @@
     def supports_brightness(self) -> bool:
         """Flag if light supports brightness."""
         return True
 
     @config_property
     def supports_color_temperature(self) -> bool:
         """Flag if light supports color temperature."""
-        return self._e_device_operation_mode.value in (_DOM_RGBW, _DOM_TUNABLE_WHITE)
+        return self._e_device_operation_mode.value == _DOM_TUNABLE_WHITE
 
     @config_property
     def supports_effects(self) -> bool:
         """Flag if light supports effects."""
         return True
 
     @config_property
@@ -511,15 +511,15 @@
         if (on_time := kwargs.get(HM_ARG_ON_TIME)) or (on_time := self.get_on_time_and_cleanup()):
             await self._set_on_time_value(on_time=on_time, collector=collector)
         if (hs_color := kwargs.get(_HM_ARG_HS_COLOR)) is not None:
             hue, ksaturation = hs_color
             saturation = ksaturation / 100
             await self._e_hue.send_value(value=int(hue), collector=collector)
             await self._e_saturation.send_value(value=saturation, collector=collector)
-        if (color_temp := kwargs.get(_HM_ARG_COLOR_TEMP)) is not None:
+        if color_temp := kwargs.get(_HM_ARG_COLOR_TEMP):
             color_temp_kelvin = math.floor(1000000 / color_temp)
             await self._e_color_temperature_kelvin.send_value(
                 value=color_temp_kelvin, collector=collector
             )
         if self.supports_effects and (effect := kwargs.get(_HM_ARG_EFFECT)) is not None:
             await self._e_effect.send_value(value=effect, collector=collector)
```

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/support.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.4.5/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/device.py` & `hahomematic-2023.4.5/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/entity.py` & `hahomematic-2023.4.5/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/event.py` & `hahomematic-2023.4.5/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/action.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/button.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/number.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/select.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.4.5/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/button.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/number.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/select.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/hub/text.py` & `hahomematic-2023.4.5/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/platforms/support.py` & `hahomematic-2023.4.5/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.4.5/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.4.5/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.4.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/support.py` & `hahomematic-2023.4.5/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.4.5/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic/xml_rpc_server.py` & `hahomematic-2023.4.5/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.4.5/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.4/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.4.5/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.4/pyproject.toml` & `hahomematic-2023.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.4.4"
+version     = "2023.4.5"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

