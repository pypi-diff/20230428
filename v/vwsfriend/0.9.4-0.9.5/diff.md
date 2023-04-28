# Comparing `tmp/vwsfriend-0.9.4.tar.gz` & `tmp/vwsfriend-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vwsfriend-0.9.4.tar", last modified: Wed Oct 27 20:45:36 2021, max compression
+gzip compressed data, was "vwsfriend-0.9.5.tar", last modified: Mon Nov  1 21:33:11 2021, max compression
```

## Comparing `vwsfriend-0.9.4.tar` & `vwsfriend-0.9.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.790353 vwsfriend-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/tests/test_location_util.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/tests/test_vwsfriend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.790353 vwsfriend-0.9.4/vwsfriend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/__version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5935 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agent_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.794353 vwsfriend-0.9.4/vwsfriend/agents/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.794353 vwsfriend-0.9.4/vwsfriend/agents/abrp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/abrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/abrp/abrp_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/battery_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)    14070 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/charge_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/climatization_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/range_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/refuel_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4792 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/state_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     9368 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/trip_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/agents/weconnect_error_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.794353 vwsfriend-0.9.4/vwsfriend/homekit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/battery.py
--rw-r--r--   0 runner    (1001) docker     (121)     9277 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/bridge.py
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/charging.py
--rw-r--r--   0 runner    (1001) docker     (121)     8889 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/climatization.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/custom_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/dummy_accessory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/genericAccessory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/locking_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/homekit/plug.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.798353 vwsfriend-0.9.4/vwsfriend/model/
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/battery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/charge.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/charger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/charging_session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/climatization.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/datetime_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/journey.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/location.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/online.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/refuel_session.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/trip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vehicle_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.798353 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.802353 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/023aa9f36740_added_fields_for_real_kwh_and_cost.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/06a5ec0a1af0_add_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/184bb7a71ada_added_error_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/689f13ef5c86_added_responsetime_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/90636c798967_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/f2fc2726507f_added_journey_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/f6785099280a_added_attributes_for_real_refueled_.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/weconnect_error.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/model/weconnect_responsetime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.802353 vwsfriend-0.9.4/vwsfriend/ui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34087 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     8882 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.802353 vwsfriend-0.9.4/vwsfriend/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.802353 vwsfriend-0.9.4/vwsfriend/ui/static/icons/
--rw-r--r--   0 runner    (1001) docker     (121)    11906 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/static/icons/abrp_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/static/icons/settings.png
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/static/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.802353 vwsfriend-0.9.4/vwsfriend/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/vwsfriend/ui/templates/database/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/backup.html
--rw-r--r--   0 runner    (1001) docker     (121)     9066 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/charging_session_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/journey_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     5775 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/refuel_session_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/settings_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/database/trip_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/restart.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/vwsfriend/ui/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/settings/abrpsettings.html
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/settings/homekit.html
--rw-r--r--   0 runner    (1001) docker     (121)      708 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/settings/vehicle.html
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/settings/vehicledbparameters.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/vwsfriend/ui/templates/status/
--rw-r--r--   0 runner    (1001) docker     (121)    15742 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/status/vehicle.html
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/status/vehicles.html
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (121)     4889 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/ui/vwsfriend_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.806353 vwsfriend-0.9.4/vwsfriend/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/util/location_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    10959 2021-10-27 20:45:04.000000 vwsfriend-0.9.4/vwsfriend/vwsfriend_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 20:45:36.794353 vwsfriend-0.9.4/vwsfriend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-27 20:45:36.000000 vwsfriend-0.9.4/vwsfriend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4096 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.650144 vwsfriend-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/tests/test_location_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/tests/test_vwsfriend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.650144 vwsfriend-0.9.5/vwsfriend/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/__version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5935 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agent_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.650144 vwsfriend-0.9.5/vwsfriend/agents/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.650144 vwsfriend-0.9.5/vwsfriend/agents/abrp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/abrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/abrp/abrp_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/battery_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14070 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/charge_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/climatization_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/range_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5417 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/refuel_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4792 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/state_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9368 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/trip_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/agents/weconnect_error_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.654145 vwsfriend-0.9.5/vwsfriend/homekit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/battery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9277 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7888 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/charging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8889 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/climatization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/custom_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/dummy_accessory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/genericAccessory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/locking_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/homekit/plug.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/battery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/charge.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/charger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/charging_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/climatization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/datetime_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/journey.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5762 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/online.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/refuel_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/trip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vehicle_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/env.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/023aa9f36740_added_fields_for_real_kwh_and_cost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/06a5ec0a1af0_add_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/184bb7a71ada_added_error_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/689f13ef5c86_added_responsetime_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/90636c798967_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/f2fc2726507f_added_journey_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/f6785099280a_added_attributes_for_real_refueled_.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/weconnect_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/model/weconnect_responsetime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/ui/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34087 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8882 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/ui/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)    11906 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/static/icons/abrp_icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2598 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/static/icons/settings.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.658145 vwsfriend-0.9.5/vwsfriend/ui/templates/database/
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/backup.html
+-rw-r--r--   0 runner    (1001) docker     (121)     9066 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/charging_session_edit.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1861 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/journey_edit.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5775 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/refuel_session_edit.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/settings_edit.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7606 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/database/trip_edit.html
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/restart.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/vwsfriend/ui/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/settings/abrpsettings.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/settings/homekit.html
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/settings/vehicle.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/settings/vehicledbparameters.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/vwsfriend/ui/templates/status/
+-rw-r--r--   0 runner    (1001) docker     (121)    15742 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/status/vehicle.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/status/vehicles.html
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4889 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/ui/vwsfriend_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.662145 vwsfriend-0.9.5/vwsfriend/util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/util/location_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10959 2021-11-01 21:32:33.000000 vwsfriend-0.9.5/vwsfriend/vwsfriend_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 21:33:11.650144 vwsfriend-0.9.5/vwsfriend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4096 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-01 21:33:11.000000 vwsfriend-0.9.5/vwsfriend.egg-info/top_level.txt
```

### Comparing `vwsfriend-0.9.4/PKG-INFO` & `vwsfriend-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vwsfriend
-Version: 0.9.4
+Version: 0.9.5
 Summary: UNKNOWN
 Home-page: https://github.com/tillsteinbach/VWsFriend
 Author: Till Steinbach
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/VWsFriend
 Project-URL: Source, https://github.com/tillsteinbach/VWsFriend
 Project-URL: Bug Tracker, https://github.com/tillsteinbach/VWsFriend/issues
```

### Comparing `vwsfriend-0.9.4/README.md` & `vwsfriend-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/setup.cfg` & `vwsfriend-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/setup.py` & `vwsfriend-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/tests/test_location_util.py` & `vwsfriend-0.9.5/tests/test_location_util.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agent_connector.py` & `vwsfriend-0.9.5/vwsfriend/agent_connector.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/abrp/abrp_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/abrp/abrp_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/battery_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/battery_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/charge_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/charge_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/climatization_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/climatization_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/range_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/range_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/refuel_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/refuel_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/state_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/state_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/trip_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/trip_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/agents/weconnect_error_agent.py` & `vwsfriend-0.9.5/vwsfriend/agents/weconnect_error_agent.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/battery.py` & `vwsfriend-0.9.5/vwsfriend/homekit/battery.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/bridge.py` & `vwsfriend-0.9.5/vwsfriend/homekit/bridge.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/charging.py` & `vwsfriend-0.9.5/vwsfriend/homekit/charging.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/climatization.py` & `vwsfriend-0.9.5/vwsfriend/homekit/climatization.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/genericAccessory.py` & `vwsfriend-0.9.5/vwsfriend/homekit/genericAccessory.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/locking_system.py` & `vwsfriend-0.9.5/vwsfriend/homekit/locking_system.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/homekit/plug.py` & `vwsfriend-0.9.5/vwsfriend/homekit/plug.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/__init__.py` & `vwsfriend-0.9.5/vwsfriend/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/battery.py` & `vwsfriend-0.9.5/vwsfriend/model/battery.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/charge.py` & `vwsfriend-0.9.5/vwsfriend/model/charge.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/charger.py` & `vwsfriend-0.9.5/vwsfriend/model/charger.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/charging_session.py` & `vwsfriend-0.9.5/vwsfriend/model/charging_session.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/climatization.py` & `vwsfriend-0.9.5/vwsfriend/model/climatization.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/datetime_decorator.py` & `vwsfriend-0.9.5/vwsfriend/model/datetime_decorator.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/journey.py` & `vwsfriend-0.9.5/vwsfriend/model/journey.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/location.py` & `vwsfriend-0.9.5/vwsfriend/model/location.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/migrations.py` & `vwsfriend-0.9.5/vwsfriend/model/migrations.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/online.py` & `vwsfriend-0.9.5/vwsfriend/model/online.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/range.py` & `vwsfriend-0.9.5/vwsfriend/model/range.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/refuel_session.py` & `vwsfriend-0.9.5/vwsfriend/model/refuel_session.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/settings.py` & `vwsfriend-0.9.5/vwsfriend/model/settings.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/trip.py` & `vwsfriend-0.9.5/vwsfriend/model/trip.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vehicle.py` & `vwsfriend-0.9.5/vwsfriend/model/vehicle.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vehicle_settings.py` & `vwsfriend-0.9.5/vwsfriend/model/vehicle_settings.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/env.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/env.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/023aa9f36740_added_fields_for_real_kwh_and_cost.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/023aa9f36740_added_fields_for_real_kwh_and_cost.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/06a5ec0a1af0_add_settings.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/06a5ec0a1af0_add_settings.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/184bb7a71ada_added_error_table.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/184bb7a71ada_added_error_table.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/689f13ef5c86_added_responsetime_table.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/689f13ef5c86_added_responsetime_table.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/f2fc2726507f_added_journey_table.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/f2fc2726507f_added_journey_table.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/vwsfriend-schema/versions/f6785099280a_added_attributes_for_real_refueled_.py` & `vwsfriend-0.9.5/vwsfriend/model/vwsfriend-schema/versions/f6785099280a_added_attributes_for_real_refueled_.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/weconnect_error.py` & `vwsfriend-0.9.5/vwsfriend/model/weconnect_error.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/model/weconnect_responsetime.py` & `vwsfriend-0.9.5/vwsfriend/model/weconnect_responsetime.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/database.py` & `vwsfriend-0.9.5/vwsfriend/ui/database.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/settings.py` & `vwsfriend-0.9.5/vwsfriend/ui/settings.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/static/icons/abrp_icon.png` & `vwsfriend-0.9.5/vwsfriend/ui/static/icons/abrp_icon.png`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/static/icons/settings.png` & `vwsfriend-0.9.5/vwsfriend/ui/static/icons/settings.png`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/static/style.css` & `vwsfriend-0.9.5/vwsfriend/ui/static/style.css`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/status.py` & `vwsfriend-0.9.5/vwsfriend/ui/status.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/base.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/backup.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/backup.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/charging_session_edit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/charging_session_edit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/journey_edit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/journey_edit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/refuel_session_edit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/refuel_session_edit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/settings_edit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/settings_edit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/database/trip_edit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/database/trip_edit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/settings/abrpsettings.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/settings/abrpsettings.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/settings/homekit.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/settings/homekit.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/settings/vehicle.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/settings/vehicle.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/settings/vehicledbparameters.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/settings/vehicledbparameters.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/status/vehicle.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/status/vehicle.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/templates/status/vehicles.html` & `vwsfriend-0.9.5/vwsfriend/ui/templates/status/vehicles.html`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/ui/vwsfriend_ui.py` & `vwsfriend-0.9.5/vwsfriend/ui/vwsfriend_ui.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/util/location_util.py` & `vwsfriend-0.9.5/vwsfriend/util/location_util.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend/vwsfriend_base.py` & `vwsfriend-0.9.5/vwsfriend/vwsfriend_base.py`

 * *Files identical despite different names*

### Comparing `vwsfriend-0.9.4/vwsfriend.egg-info/PKG-INFO` & `vwsfriend-0.9.5/vwsfriend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vwsfriend
-Version: 0.9.4
+Version: 0.9.5
 Summary: UNKNOWN
 Home-page: https://github.com/tillsteinbach/VWsFriend
 Author: Till Steinbach
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/VWsFriend
 Project-URL: Source, https://github.com/tillsteinbach/VWsFriend
 Project-URL: Bug Tracker, https://github.com/tillsteinbach/VWsFriend/issues
```

### Comparing `vwsfriend-0.9.4/vwsfriend.egg-info/SOURCES.txt` & `vwsfriend-0.9.5/vwsfriend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

