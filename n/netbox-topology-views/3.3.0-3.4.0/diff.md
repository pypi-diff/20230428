# Comparing `tmp/netbox-topology-views-3.3.0.tar.gz` & `tmp/netbox-topology-views-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-views-3.3.0.tar", last modified: Thu Mar 23 09:10:20 2023, max compression
+gzip compressed data, was "netbox-topology-views-3.4.0.tar", last modified: Fri Apr 28 14:09:41 2023, max compression
```

## Comparing `netbox-topology-views-3.3.0.tar` & `netbox-topology-views-3.4.0.tar`

### file list

```diff
@@ -1,68 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.580981 netbox-topology-views-3.3.0/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.584981 netbox-topology-views-3.3.0/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.584981 netbox-topology-views-3.3.0/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.576981 netbox-topology-views-3.3.0/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.576981 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.584981 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/backup.png
--rw-r--r--   0 runner    (1001) docker     (123)    28633 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/circuit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/firewall.png
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/internal-switch.png
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/isp-cpe-material.png
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/non-racked-devices.png
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/power-feed.png
--rw-r--r--   0 runner    (1001) docker     (123)    18685 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.png
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/power-units.png
--rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.png
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.png
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/router.png
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/server.png
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/storage.png
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.png
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (123)   350064 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.576981 netbox-topology-views-3.3.0/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:10:20.584981 netbox-topology-views-3.3.0/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-03-23 09:10:20.000000 netbox-topology-views-3.3.0/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-23 09:10:20.000000 netbox-topology-views-3.3.0/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:10:20.000000 netbox-topology-views-3.3.0/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 09:10:20.000000 netbox-topology-views-3.3.0/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 09:10:20.588981 netbox-topology-views-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-23 09:10:07.000000 netbox-topology-views-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.006084 netbox-topology-views-3.4.0/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.006084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.018084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   349261 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.010084 netbox-topology-views-3.4.0/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31580 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-28 14:09:41.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/setup.py
```

### Comparing `netbox-topology-views-3.3.0/LICENSE` & `netbox-topology-views-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/PKG-INFO` & `netbox-topology-views-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.3.0
+Version: 3.4.0
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -57,14 +57,15 @@
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
 
 | netbox version | netbox-topology-views version |
 | -------------- | ----------------------------- |
+| >= 3.5.0       | >= v3.4.X                     |
 | >= 3.4.0       | >= v3.X.X                     |
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
```

### Comparing `netbox-topology-views-3.3.0/README.md` & `netbox-topology-views-3.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
 
 | netbox version | netbox-topology-views version |
 | -------------- | ----------------------------- |
+| >= 3.5.0       | >= v3.4.X                     |
 | >= 3.4.0       | >= v3.X.X                     |
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
```

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/__init__.py` & `netbox-topology-views-3.4.0/netbox_topology_views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.3.0"
+    version = "3.4.0"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
         "always_save_coordinates": False,
-
     }
 
+    def ready(self):
+        from . import signals
+
+        super().ready()
+
 
 config = TopologyViewsConfig
```

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/api/serializers.py` & `netbox-topology-views-3.4.0/netbox_topology_views/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/api/views.py` & `netbox-topology-views-3.4.0/netbox_topology_views/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/filters.py` & `netbox-topology-views-3.4.0/netbox_topology_views/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/forms.py` & `netbox-topology-views-3.4.0/netbox_topology_views/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 from django import forms
 from dcim.choices import DeviceStatusChoices
 from tenancy.models import TenantGroup, Tenant
 from tenancy.forms import TenancyFilterForm
 from django.conf import settings
 from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm
-from utilities.forms import (
+from utilities.forms.fields import (
     TagFilterField,
     DynamicModelMultipleChoiceField,
-    MultipleChoiceField,
-    widgets,
+    MultipleChoiceField
 )
+
+
 from .models import IndividualOptions
 
 class DeviceFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = Device
     fieldsets = (
         (
             None,
@@ -174,15 +175,14 @@
         help_text=_("Select Device Roles that you want to have "
             "preselected in the filter tab.")
     )
     preselected_tags = forms.ModelMultipleChoiceField(
         label=_("Preselected Tags"),
         queryset=Device.tags.all(),
         required=False,
-        widget=widgets.StaticSelectMultiple,
         help_text=_("Select Tags that you want to have "
             "preselected in the filter tab.")
     )
     show_unconnected = forms.BooleanField(
         label=_("Show Unconnected"), 
         required=False, 
         initial=False,
```

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.4.0/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.4.0/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/models.py` & `netbox-topology-views-3.4.0/netbox_topology_views/models.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/navigation.py` & `netbox-topology-views-3.4.0/netbox_topology_views/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,46 @@
 (() => {
-    var Bn = Object.create;
+    var In = Object.create;
     var kt = Object.defineProperty,
-        An = Object.defineProperties,
-        zn = Object.getOwnPropertyDescriptor,
-        Ln = Object.getOwnPropertyDescriptors,
-        Rn = Object.getOwnPropertyNames,
+        Pn = Object.defineProperties,
+        Mn = Object.getOwnPropertyDescriptor,
+        Dn = Object.getOwnPropertyDescriptors,
+        Fn = Object.getOwnPropertyNames,
         Ui = Object.getOwnPropertySymbols,
-        Hn = Object.getPrototypeOf,
+        Nn = Object.getPrototypeOf,
         Yi = Object.prototype.hasOwnProperty,
-        jn = Object.prototype.propertyIsEnumerable;
+        Bn = Object.prototype.propertyIsEnumerable;
     var Jt = (n, e, t) => e in n ? kt(n, e, {
             enumerable: !0,
             configurable: !0,
             writable: !0,
             value: t
         }) : n[e] = t,
         de = (n, e) => {
             for (var t in e || (e = {})) Yi.call(e, t) && Jt(n, t, e[t]);
             if (Ui)
-                for (var t of Ui(e)) jn.call(e, t) && Jt(n, t, e[t]);
+                for (var t of Ui(e)) Bn.call(e, t) && Jt(n, t, e[t]);
             return n
         },
-        Be = (n, e) => An(n, Ln(e)),
-        Wn = n => kt(n, "__esModule", {
+        Be = (n, e) => Pn(n, Dn(e)),
+        An = n => kt(n, "__esModule", {
             value: !0
         });
     var ei = (n, e) => () => (e || n((e = {
         exports: {}
     }).exports, e), e.exports);
-    var Vn = (n, e, t) => {
+    var zn = (n, e, t) => {
             if (e && typeof e == "object" || typeof e == "function")
-                for (let i of Rn(e)) !Yi.call(n, i) && i !== "default" && kt(n, i, {
+                for (let i of Fn(e)) !Yi.call(n, i) && i !== "default" && kt(n, i, {
                     get: () => e[i],
-                    enumerable: !(t = zn(e, i)) || t.enumerable
+                    enumerable: !(t = Mn(e, i)) || t.enumerable
                 });
             return n
         },
-        ti = n => Vn(Wn(kt(n != null ? Bn(Hn(n)) : {}, "default", n && n.__esModule && "default" in n ? {
+        ti = n => zn(An(kt(n != null ? In(Nn(n)) : {}, "default", n && n.__esModule && "default" in n ? {
             get: () => n.default,
             enumerable: !0
         } : {
             value: n,
             enumerable: !0
         })), n);
     var $ = (n, e, t) => (Jt(n, typeof e != "symbol" ? e + "" : e, t), t);
@@ -62,18 +62,18 @@
             a = d => d.done ? i(d.value) : Promise.resolve(d.value).then(o, r);
         a((t = t.apply(n, e)).next())
     });
     var si = ei((ja, ii) => {
         typeof ii != "undefined" && (ii.exports = ne);
 
         function ne(n) {
-            if (n) return qn(n)
+            if (n) return Ln(n)
         }
 
-        function qn(n) {
+        function Ln(n) {
             for (var e in ne.prototype) n[e] = ne.prototype[e];
             return n
         }
         ne.prototype.on = ne.prototype.addEventListener = function(n, e) {
             return this._callbacks = this._callbacks || {}, (this._callbacks["$" + n] = this._callbacks["$" + n] || []).push(e), this
         };
         ne.prototype.once = function(n, e) {
@@ -462,57 +462,57 @@
             if (s != null)
                 for (var o in s) s.hasOwnProperty(o) && (t[o] = s[o])
         }
         return t
     } : oi = Object.assign;
     var Ae = oi,
         Gi = ["", "webkit", "Moz", "MS", "ms", "o"],
-        Un = typeof document == "undefined" ? {
+        Rn = typeof document == "undefined" ? {
             style: {}
         } : document.createElement("div"),
-        Yn = "function",
+        Hn = "function",
         Ze = Math.round,
         ze = Math.abs,
         ni = Date.now;
 
     function Ot(n, e) {
         for (var t, i, s = e[0].toUpperCase() + e.slice(1), o = 0; o < Gi.length;) {
             if (t = Gi[o], i = t ? t + s : e, i in n) return i;
             o++
         }
     }
     var ye;
     typeof window == "undefined" ? ye = {} : ye = window;
-    var Ki = Ot(Un.style, "touchAction"),
+    var Ki = Ot(Rn.style, "touchAction"),
         Zi = Ki !== void 0;
 
-    function Xn() {
+    function jn() {
         if (!Zi) return !1;
         var n = {},
             e = ye.CSS && ye.CSS.supports;
         return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach(function(t) {
             return n[t] = e ? ye.CSS.supports("touch-action", t) : !0
         }), n
     }
     var Qi = "compute",
         $i = "auto",
         ri = "manipulation",
         Le = "none",
         nt = "pan-x",
         rt = "pan-y",
-        It = Xn(),
-        Gn = /mobile|tablet|ip(ad|hone|od)|android/i,
+        It = jn(),
+        Wn = /mobile|tablet|ip(ad|hone|od)|android/i,
         Ji = "ontouchstart" in ye,
-        Kn = Ot(ye, "PointerEvent") !== void 0,
-        Zn = Ji && Gn.test(navigator.userAgent),
+        Vn = Ot(ye, "PointerEvent") !== void 0,
+        qn = Ji && Wn.test(navigator.userAgent),
         at = "touch",
-        Qn = "pen",
+        Un = "pen",
         ai = "mouse",
-        $n = "kinect",
-        Jn = 25,
+        Yn = "kinect",
+        Xn = 25,
         ee = 1,
         Re = 2,
         K = 4,
         se = 8,
         Pt = 1,
         dt = 2,
         ht = 4,
@@ -531,22 +531,22 @@
             else if (n.length !== void 0)
             for (i = 0; i < n.length;) e.call(t, n[i], i, n), i++;
         else
             for (i in n) n.hasOwnProperty(i) && e.call(t, n[i], i, n)
     }
 
     function Dt(n, e) {
-        return typeof n === Yn ? n.apply(e && e[0] || void 0, e) : n
+        return typeof n === Hn ? n.apply(e && e[0] || void 0, e) : n
     }
 
     function je(n, e) {
         return n.indexOf(e) > -1
     }
 
-    function er(n) {
+    function Gn(n) {
         if (je(n, Le)) return Le;
         var e = je(n, nt),
             t = je(n, rt);
         return e && t ? Le : e || t ? e ? nt : rt : je(n, ri) ? ri : $i
     }
     var is = function() {
         function n(t, i) {
@@ -557,15 +557,15 @@
             i === Qi && (i = this.compute()), Zi && this.manager.element.style && It[i] && (this.manager.element.style[Ki] = i), this.actions = i.toLowerCase().trim()
         }, e.update = function() {
             this.set(this.manager.options.touchAction)
         }, e.compute = function() {
             var i = [];
             return be(this.manager.recognizers, function(s) {
                 Dt(s.options.enable, [s]) && (i = i.concat(s.getTouchAction()))
-            }), er(i.join(" "))
+            }), Gn(i.join(" "))
         }, e.preventDefaults = function(i) {
             var s = i.srcEvent,
                 o = i.offsetDirection;
             if (this.manager.session.prevented) {
                 s.preventDefault();
                 return
             }
@@ -634,15 +634,15 @@
         return Math.atan2(s, i) * 180 / Math.PI
     }
 
     function ns(n, e) {
         return n === e ? Pt : ze(n) >= ze(e) ? n < 0 ? dt : ht : e < 0 ? lt : Qe
     }
 
-    function tr(n, e) {
+    function Kn(n, e) {
         var t = e.center,
             i = n.offsetDelta || {},
             s = n.prevDelta || {},
             o = n.prevInput || {};
         (e.eventType === ee || o.eventType === K) && (s = n.prevDelta = {
             x: o.deltaX || 0,
             y: o.deltaY || 0
@@ -655,59 +655,59 @@
     function rs(n, e, t) {
         return {
             x: e / n || 0,
             y: t / n || 0
         }
     }
 
-    function ir(n, e) {
+    function Zn(n, e) {
         return Ft(e[0], e[1], Mt) / Ft(n[0], n[1], Mt)
     }
 
-    function sr(n, e) {
+    function Qn(n, e) {
         return hi(e[1], e[0], Mt) + hi(n[1], n[0], Mt)
     }
 
-    function or(n, e) {
+    function $n(n, e) {
         var t = n.lastInterval || e,
             i = e.timeStamp - t.timeStamp,
             s, o, r, a;
-        if (e.eventType !== se && (i > Jn || t.velocity === void 0)) {
+        if (e.eventType !== se && (i > Xn || t.velocity === void 0)) {
             var d = e.deltaX - t.deltaX,
                 h = e.deltaY - t.deltaY,
                 l = rs(i, d, h);
             o = l.x, r = l.y, s = ze(l.x) > ze(l.y) ? l.x : l.y, a = ns(d, h), n.lastInterval = e
         } else s = t.velocity, o = t.velocityX, r = t.velocityY, a = t.direction;
         e.velocity = s, e.velocityX = o, e.velocityY = r, e.direction = a
     }
 
-    function nr(n, e) {
+    function Jn(n, e) {
         var t = n.session,
             i = e.pointers,
             s = i.length;
         t.firstInput || (t.firstInput = os(e)), s > 1 && !t.firstMultiple ? t.firstMultiple = os(e) : s === 1 && (t.firstMultiple = !1);
         var o = t.firstInput,
             r = t.firstMultiple,
             a = r ? r.center : o.center,
             d = e.center = ss(i);
-        e.timeStamp = ni(), e.deltaTime = e.timeStamp - o.timeStamp, e.angle = hi(a, d), e.distance = Ft(a, d), tr(t, e), e.offsetDirection = ns(e.deltaX, e.deltaY);
+        e.timeStamp = ni(), e.deltaTime = e.timeStamp - o.timeStamp, e.angle = hi(a, d), e.distance = Ft(a, d), Kn(t, e), e.offsetDirection = ns(e.deltaX, e.deltaY);
         var h = rs(e.deltaTime, e.deltaX, e.deltaY);
-        e.overallVelocityX = h.x, e.overallVelocityY = h.y, e.overallVelocity = ze(h.x) > ze(h.y) ? h.x : h.y, e.scale = r ? ir(r.pointers, i) : 1, e.rotation = r ? sr(r.pointers, i) : 0, e.maxPointers = t.prevInput ? e.pointers.length > t.prevInput.maxPointers ? e.pointers.length : t.prevInput.maxPointers : e.pointers.length, or(t, e);
+        e.overallVelocityX = h.x, e.overallVelocityY = h.y, e.overallVelocity = ze(h.x) > ze(h.y) ? h.x : h.y, e.scale = r ? Zn(r.pointers, i) : 1, e.rotation = r ? Qn(r.pointers, i) : 0, e.maxPointers = t.prevInput ? e.pointers.length > t.prevInput.maxPointers ? e.pointers.length : t.prevInput.maxPointers : e.pointers.length, $n(t, e);
         var l = n.element,
             c = e.srcEvent,
             u;
         c.composedPath ? u = c.composedPath()[0] : c.path ? u = c.path[0] : u = c.target, di(u, l) && (l = u), e.target = l
     }
 
-    function rr(n, e, t) {
+    function er(n, e, t) {
         var i = t.pointers.length,
             s = t.changedPointers.length,
             o = e & ee && i - s == 0,
             r = e & (K | se) && i - s == 0;
-        t.isFirst = !!o, t.isFinal = !!r, o && (n.session = {}), t.eventType = e, nr(n, t), n.emit("hammer.input", t), n.recognize(t), n.session.prevInput = t
+        t.isFirst = !!o, t.isFinal = !!r, o && (n.session = {}), t.eventType = e, Jn(n, t), n.emit("hammer.input", t), n.recognize(t), n.session.prevInput = t
     }
 
     function ct(n) {
         return n.trim().split(/\s+/g)
     }
 
     function ut(n, e, t) {
@@ -745,26 +745,26 @@
         if (n.indexOf && !t) return n.indexOf(e);
         for (var i = 0; i < n.length;) {
             if (t && n[i][t] == e || !t && n[i] === e) return i;
             i++
         }
         return -1
     }
-    var ar = {
+    var tr = {
             pointerdown: ee,
             pointermove: Re,
             pointerup: K,
             pointercancel: se,
             pointerout: se
         },
-        dr = {
+        ir = {
             2: at,
-            3: Qn,
+            3: Un,
             4: ai,
-            5: $n
+            5: Yn
         },
         ds = "pointerdown",
         hs = "pointermove pointerup pointercancel";
     ye.MSPointerEvent && !ye.PointerEvent && (ds = "MSPointerDown", hs = "MSPointerMove MSPointerUp MSPointerCancel");
     var ls = function(n) {
         he(e, n);
 
@@ -773,16 +773,16 @@
             return s.evEl = ds, s.evWin = hs, i = n.apply(this, arguments) || this, i.store = i.manager.session.pointerEvents = [], i
         }
         var t = e.prototype;
         return t.handler = function(s) {
             var o = this.store,
                 r = !1,
                 a = s.type.toLowerCase().replace("ms", ""),
-                d = ar[a],
-                h = dr[s.pointerType] || s.pointerType,
+                d = tr[a],
+                h = ir[s.pointerType] || s.pointerType,
                 l = h === at,
                 c = We(o, s.pointerId, "pointerId");
             d & ee && (s.button === 0 || l) ? c < 0 && (o.push(s), c = o.length - 1) : d & (K | se) && (r = !0), !(c < 0) && (o[c] = s, this.callback(this.manager, d, {
                 pointers: o,
                 changedPointers: [s],
                 pointerType: h,
                 srcEvent: s
@@ -799,81 +799,81 @@
             var r = e ? n[o][e] : n[o];
             We(s, r) < 0 && i.push(n[o]), s[o] = r, o++
         }
         return t && (e ? i = i.sort(function(a, d) {
             return a[e] > d[e]
         }) : i = i.sort()), i
     }
-    var hr = {
+    var sr = {
             touchstart: ee,
             touchmove: Re,
             touchend: K,
             touchcancel: se
         },
-        lr = "touchstart touchmove touchend touchcancel",
+        or = "touchstart touchmove touchend touchcancel",
         ci = function(n) {
             he(e, n);
 
             function e() {
                 var i;
-                return e.prototype.evTarget = lr, i = n.apply(this, arguments) || this, i.targetIds = {}, i
+                return e.prototype.evTarget = or, i = n.apply(this, arguments) || this, i.targetIds = {}, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
-                var o = hr[s.type],
-                    r = cr.call(this, s, o);
+                var o = sr[s.type],
+                    r = nr.call(this, s, o);
                 !r || this.callback(this.manager, o, {
                     pointers: r[0],
                     changedPointers: r[1],
                     pointerType: at,
                     srcEvent: s
                 })
             }, e
         }($e);
 
-    function cr(n, e) {
+    function nr(n, e) {
         var t = pt(n.touches),
             i = this.targetIds;
         if (e & (ee | Re) && t.length === 1) return i[t[0].identifier] = !0, [t, t];
         var s, o, r = pt(n.changedTouches),
             a = [],
             d = this.target;
         if (o = t.filter(function(h) {
                 return di(h.target, d)
             }), e === ee)
             for (s = 0; s < o.length;) i[o[s].identifier] = !0, s++;
         for (s = 0; s < r.length;) i[r[s].identifier] && a.push(r[s]), e & (K | se) && delete i[r[s].identifier], s++;
         if (!!a.length) return [li(o.concat(a), "identifier", !0), a]
     }
-    var ur = {
+    var rr = {
             mousedown: ee,
             mousemove: Re,
             mouseup: K
         },
-        fr = "mousedown",
-        pr = "mousemove mouseup",
+        ar = "mousedown",
+        dr = "mousemove mouseup",
         ui = function(n) {
             he(e, n);
 
             function e() {
                 var i, s = e.prototype;
-                return s.evEl = fr, s.evWin = pr, i = n.apply(this, arguments) || this, i.pressed = !1, i
+                return s.evEl = ar, s.evWin = dr, i = n.apply(this, arguments) || this, i.pressed = !1, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
-                var o = ur[s.type];
+                var o = rr[s.type];
                 o & ee && s.button === 0 && (this.pressed = !0), o & Re && s.which !== 1 && (o = K), !!this.pressed && (o & K && (this.pressed = !1), this.callback(this.manager, o, {
                     pointers: [s],
                     changedPointers: [s],
                     pointerType: ai,
                     srcEvent: s
                 }))
             }, e
         }($e),
-        gr = 2500,
+        hr = 2500,
         cs = 25;
 
     function us(n) {
         var e = n.changedPointers,
             t = e[0];
         if (t.identifier === this.primaryTouch) {
             var i = {
@@ -882,23 +882,23 @@
                 },
                 s = this.lastTouches;
             this.lastTouches.push(i);
             var o = function() {
                 var a = s.indexOf(i);
                 a > -1 && s.splice(a, 1)
             };
-            setTimeout(o, gr)
+            setTimeout(o, hr)
         }
     }
 
-    function mr(n, e) {
+    function lr(n, e) {
         n & ee ? (this.primaryTouch = e.changedPointers[0].identifier, us.call(this, e)) : n & (K | se) && us.call(this, e)
     }
 
-    function yr(n) {
+    function cr(n) {
         for (var e = n.srcEvent.clientX, t = n.srcEvent.clientY, i = 0; i < this.lastTouches.length; i++) {
             var s = this.lastTouches[i],
                 o = Math.abs(e - s.x),
                 r = Math.abs(t - s.y);
             if (o <= cs && r <= cs) return !0
         }
         return !1
@@ -909,62 +909,62 @@
 
             function t(s, o) {
                 var r;
                 return r = e.call(this, s, o) || this, r.handler = function(a, d, h) {
                     var l = h.pointerType === at,
                         c = h.pointerType === ai;
                     if (!(c && h.sourceCapabilities && h.sourceCapabilities.firesTouchEvents)) {
-                        if (l) mr.call(St(St(r)), d, h);
-                        else if (c && yr.call(St(St(r)), h)) return;
+                        if (l) lr.call(St(St(r)), d, h);
+                        else if (c && cr.call(St(St(r)), h)) return;
                         r.callback(a, d, h)
                     }
                 }, r.touch = new ci(r.manager, r.handler), r.mouse = new ui(r.manager, r.handler), r.primaryTouch = null, r.lastTouches = [], r
             }
             var i = t.prototype;
             return i.destroy = function() {
                 this.touch.destroy(), this.mouse.destroy()
             }, t
         }($e);
         return n
     }();
 
-    function br(n) {
+    function ur(n) {
         var e, t = n.options.inputClass;
-        return t ? e = t : Kn ? e = ls : Zn ? e = ci : Ji ? e = fs : e = ui, new e(n, rr)
+        return t ? e = t : Vn ? e = ls : qn ? e = ci : Ji ? e = fs : e = ui, new e(n, er)
     }
 
     function Je(n, e, t) {
         return Array.isArray(n) ? (be(n, t[e], t), !0) : !1
     }
     var Nt = 1,
         le = 2,
         et = 4,
         Oe = 8,
         ve = Oe,
         gt = 16,
         ge = 32,
-        vr = 1;
+        fr = 1;
 
-    function wr() {
-        return vr++
+    function pr() {
+        return fr++
     }
 
     function Bt(n, e) {
         var t = e.manager;
         return t ? t.get(n) : n
     }
 
     function ps(n) {
         return n & gt ? "cancel" : n & Oe ? "end" : n & et ? "move" : n & le ? "start" : ""
     }
     var mt = function() {
             function n(t) {
                 t === void 0 && (t = {}), this.options = fe({
                     enable: !0
-                }, t), this.id = wr(), this.manager = null, this.state = Nt, this.simultaneous = {}, this.requireFail = []
+                }, t), this.id = pr(), this.manager = null, this.state = Nt, this.simultaneous = {}, this.requireFail = []
             }
             var e = n.prototype;
             return e.set = function(i) {
                 return Ae(this.options, i), this.manager && this.manager.touchAction.update(), this
             }, e.recognizeWith = function(i) {
                 if (Je(i, "recognizeWith", this)) return this;
                 var s = this.simultaneous;
@@ -1248,44 +1248,44 @@
                     event: "doubletap",
                     taps: 2
                 },
                 ["tap"]
             ],
             [vs]
         ],
-        _r = 1,
+        gr = 1,
         Es = 2;
 
     function xs(n, e) {
         var t = n.element;
         if (!!t.style) {
             var i;
             be(n.options.cssProps, function(s, o) {
                 i = Ot(t.style, o), e ? (n.oldCssProps[i] = t.style[i], t.style[i] = s) : t.style[i] = n.oldCssProps[i] || ""
             }), e || (n.oldCssProps = {})
         }
     }
 
-    function Er(n, e) {
+    function mr(n, e) {
         var t = document.createEvent("Event");
         t.initEvent(n, !0, !0), t.gesture = e, e.target.dispatchEvent(t)
     }
     var Cs = function() {
             function n(t, i) {
                 var s = this;
-                this.options = Ae({}, ws, i || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = br(this), this.touchAction = new is(this, this.options.touchAction), xs(this, !0), be(this.options.recognizers, function(o) {
+                this.options = Ae({}, ws, i || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = ur(this), this.touchAction = new is(this, this.options.touchAction), xs(this, !0), be(this.options.recognizers, function(o) {
                     var r = s.add(new o[0](o[1]));
                     o[2] && r.recognizeWith(o[2]), o[3] && r.requireFailure(o[3])
                 }, this)
             }
             var e = n.prototype;
             return e.set = function(i) {
                 return Ae(this.options, i), i.touchAction && this.touchAction.update(), i.inputTarget && (this.input.destroy(), this.input.target = i.inputTarget, this.input.init()), this
             }, e.stop = function(i) {
-                this.session.stopped = i ? Es : _r
+                this.session.stopped = i ? Es : gr
             }, e.recognize = function(i) {
                 var s = this.session;
                 if (!s.stopped) {
                     this.touchAction.preventDefaults(i);
                     var o, r = this.recognizers,
                         a = s.curRecognizer;
                     (!a || a && a.state & ve) && (s.curRecognizer = null, a = null);
@@ -1318,57 +1318,57 @@
             }, e.off = function(i, s) {
                 if (i === void 0) return this;
                 var o = this.handlers;
                 return be(ct(i), function(r) {
                     s ? o[r] && o[r].splice(We(o[r], s), 1) : delete o[r]
                 }), this
             }, e.emit = function(i, s) {
-                this.options.domEvents && Er(i, s);
+                this.options.domEvents && mr(i, s);
                 var o = this.handlers[i] && this.handlers[i].slice();
                 if (!(!o || !o.length)) {
                     s.type = i, s.preventDefault = function() {
                         s.srcEvent.preventDefault()
                     };
                     for (var r = 0; r < o.length;) o[r](s), r++
                 }
             }, e.destroy = function() {
                 this.element && xs(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
             }, n
         }(),
-        xr = {
+        yr = {
             touchstart: ee,
             touchmove: Re,
             touchend: K,
             touchcancel: se
         },
-        Cr = "touchstart",
-        Tr = "touchstart touchmove touchend touchcancel",
-        kr = function(n) {
+        br = "touchstart",
+        vr = "touchstart touchmove touchend touchcancel",
+        wr = function(n) {
             he(e, n);
 
             function e() {
                 var i, s = e.prototype;
-                return s.evTarget = Cr, s.evWin = Tr, i = n.apply(this, arguments) || this, i.started = !1, i
+                return s.evTarget = br, s.evWin = vr, i = n.apply(this, arguments) || this, i.started = !1, i
             }
             var t = e.prototype;
             return t.handler = function(s) {
-                var o = xr[s.type];
+                var o = yr[s.type];
                 if (o === ee && (this.started = !0), !!this.started) {
-                    var r = Sr.call(this, s, o);
+                    var r = _r.call(this, s, o);
                     o & (K | se) && r[0].length - r[1].length == 0 && (this.started = !1), this.callback(this.manager, o, {
                         pointers: r[0],
                         changedPointers: r[1],
                         pointerType: at,
                         srcEvent: s
                     })
                 }
             }, e
         }($e);
 
-    function Sr(n, e) {
+    function _r(n, e) {
         var t = pt(n.touches),
             i = pt(n.changedTouches);
         return e & (K | se) && (t = li(t.concat(i), "identifier", !0)), [t, i]
     }
 
     function Ts(n, e, t) {
         var i = "DEPRECATED METHOD: " + e + `
@@ -1381,19 +1381,19 @@
             return r && r.call(window.console, i, o), n.apply(this, arguments)
         }
     }
     var ks = Ts(function(n, e, t) {
             for (var i = Object.keys(e), s = 0; s < i.length;)(!t || t && n[i[s]] === void 0) && (n[i[s]] = e[i[s]]), s++;
             return n
         }, "extend", "Use `assign`."),
-        Or = Ts(function(n, e) {
+        Er = Ts(function(n, e) {
             return ks(n, e, !0)
         }, "merge", "Use `assign`.");
 
-    function Ir(n, e, t) {
+    function xr(n, e, t) {
         var i = e.prototype,
             s;
         s = n.prototype = Object.create(i), s.constructor = n, s._super = i, t && Ae(s, t)
     }
 
     function Ss(n, e) {
         return function() {
@@ -1402,15 +1402,15 @@
     }
     var Os = function() {
             var n = function(t, i) {
                 return i === void 0 && (i = {}), new Cs(t, fe({
                     recognizers: _s.concat()
                 }, i))
             };
-            return n.VERSION = "2.0.17-rc", n.DIRECTION_ALL = es, n.DIRECTION_DOWN = Qe, n.DIRECTION_LEFT = dt, n.DIRECTION_RIGHT = ht, n.DIRECTION_UP = lt, n.DIRECTION_HORIZONTAL = pe, n.DIRECTION_VERTICAL = He, n.DIRECTION_NONE = Pt, n.DIRECTION_DOWN = Qe, n.INPUT_START = ee, n.INPUT_MOVE = Re, n.INPUT_END = K, n.INPUT_CANCEL = se, n.STATE_POSSIBLE = Nt, n.STATE_BEGAN = le, n.STATE_CHANGED = et, n.STATE_ENDED = Oe, n.STATE_RECOGNIZED = ve, n.STATE_CANCELLED = gt, n.STATE_FAILED = ge, n.Manager = Cs, n.Input = $e, n.TouchAction = is, n.TouchInput = ci, n.MouseInput = ui, n.PointerEventInput = ls, n.TouchMouseInput = fs, n.SingleTouchInput = kr, n.Recognizer = mt, n.AttrRecognizer = tt, n.Tap = fi, n.Pan = pi, n.Swipe = ms, n.Pinch = ys, n.Rotate = bs, n.Press = vs, n.on = ut, n.off = ft, n.each = be, n.merge = Or, n.extend = ks, n.bindFn = Ss, n.assign = Ae, n.inherit = Ir, n.bindFn = Ss, n.prefixed = Ot, n.toArray = pt, n.inArray = We, n.uniqueArray = li, n.splitStr = ct, n.boolOrFn = Dt, n.hasParent = di, n.addEventListeners = ut, n.removeEventListeners = ft, n.defaults = Ae({}, ws, {
+            return n.VERSION = "2.0.17-rc", n.DIRECTION_ALL = es, n.DIRECTION_DOWN = Qe, n.DIRECTION_LEFT = dt, n.DIRECTION_RIGHT = ht, n.DIRECTION_UP = lt, n.DIRECTION_HORIZONTAL = pe, n.DIRECTION_VERTICAL = He, n.DIRECTION_NONE = Pt, n.DIRECTION_DOWN = Qe, n.INPUT_START = ee, n.INPUT_MOVE = Re, n.INPUT_END = K, n.INPUT_CANCEL = se, n.STATE_POSSIBLE = Nt, n.STATE_BEGAN = le, n.STATE_CHANGED = et, n.STATE_ENDED = Oe, n.STATE_RECOGNIZED = ve, n.STATE_CANCELLED = gt, n.STATE_FAILED = ge, n.Manager = Cs, n.Input = $e, n.TouchAction = is, n.TouchInput = ci, n.MouseInput = ui, n.PointerEventInput = ls, n.TouchMouseInput = fs, n.SingleTouchInput = wr, n.Recognizer = mt, n.AttrRecognizer = tt, n.Tap = fi, n.Pan = pi, n.Swipe = ms, n.Pinch = ys, n.Rotate = bs, n.Press = vs, n.on = ut, n.off = ft, n.each = be, n.merge = Er, n.extend = ks, n.bindFn = Ss, n.assign = Ae, n.inherit = xr, n.bindFn = Ss, n.prefixed = Ot, n.toArray = pt, n.inArray = We, n.uniqueArray = li, n.splitStr = ct, n.boolOrFn = Dt, n.hasParent = di, n.addEventListeners = ut, n.removeEventListeners = ft, n.defaults = Ae({}, ws, {
                 preset: _s
             }), n
         }(),
         Wa = Os.defaults,
         Is = Os;
     var gi = Symbol("DELETE");
 
@@ -1437,63 +1437,63 @@
     }
 
     function Ns(n) {
         for (let e of Object.keys(n)) n[e] === gi ? delete n[e] : typeof n[e] == "object" && n[e] !== null && Ns(n[e])
     }
 
     function yt(...n) {
-        return Pr(n.length ? n : [Date.now()])
+        return Cr(n.length ? n : [Date.now()])
     }
 
-    function Pr(n) {
-        let [e, t, i] = Mr(n), s = 1, o = () => {
+    function Cr(n) {
+        let [e, t, i] = Tr(n), s = 1, o = () => {
             let r = 2091639 * e + s * 23283064365386963e-26;
             return e = t, t = i, i = r - (s = r | 0)
         };
         return o.uint32 = () => o() * 4294967296, o.fract53 = () => o() + (o() * 2097152 | 0) * 11102230246251565e-32, o.algorithm = "Alea", o.seed = n, o.version = "0.9", o
     }
 
-    function Mr(...n) {
-        let e = Dr(),
+    function Tr(...n) {
+        let e = kr(),
             t = e(" "),
             i = e(" "),
             s = e(" ");
         for (let o = 0; o < n.length; o++) t -= e(n[o]), t < 0 && (t += 1), i -= e(n[o]), i < 0 && (i += 1), s -= e(n[o]), s < 0 && (s += 1);
         return [t, i, s]
     }
 
-    function Dr() {
+    function kr() {
         let n = 4022871197;
         return function(e) {
             let t = e.toString();
             for (let i = 0; i < t.length; i++) {
                 n += t.charCodeAt(i);
                 let s = .02519603282416938 * n;
                 n = s >>> 0, s -= n, s *= n, n = s >>> 0, s -= n, n += s * 4294967296
             }
             return (n >>> 0) * 23283064365386963e-26
         }
     }
 
-    function Fr() {
+    function Sr() {
         let n = () => {};
         return {
             on: n,
             off: n,
             destroy: n,
             emit: n,
             get() {
                 return {
                     set: n
                 }
             }
         }
     }
     var mi = typeof window != "undefined" ? window.Hammer || Is : function() {
-        return Fr()
+        return Sr()
     };
 
     function me(n) {
         this._cleanupQueue = [], this.active = !1, this._dom = {
             container: n,
             overlay: document.createElement("div")
         }, this._dom.overlay.classList.add("vis-overlay"), this._dom.container.appendChild(this._dom.overlay), this._cleanupQueue.push(() => {
@@ -1503,15 +1503,15 @@
         e.on("tap", this._onTapOverlay.bind(this)), this._cleanupQueue.push(() => {
             e.destroy()
         }), ["tap", "doubletap", "press", "pinch", "pan", "panstart", "panmove", "panend"].forEach(i => {
             e.on(i, s => {
                 s.srcEvent.stopPropagation()
             })
         }), document && document.body && (this._onClick = i => {
-            Nr(i.target, n) || this.deactivate()
+            Or(i.target, n) || this.deactivate()
         }, document.body.addEventListener("click", this._onClick), this._cleanupQueue.push(() => {
             document.body.removeEventListener("click", this._onClick)
         })), this._escListener = i => {
             ("key" in i ? i.key === "Escape" : i.keyCode === 27) && this.deactivate()
         }
     }(0, Ps.default)(me.prototype);
     me.current = null;
@@ -1525,25 +1525,25 @@
     me.prototype.deactivate = function() {
         this.active = !1, this._dom.overlay.style.display = "block", this._dom.container.classList.remove("vis-active"), document.body.removeEventListener("keydown", this._escListener), this.emit("change"), this.emit("deactivate")
     };
     me.prototype._onTapOverlay = function(n) {
         this.activate(), n.srcEvent.stopPropagation()
     };
 
-    function Nr(n, e) {
+    function Or(n, e) {
         for (; n;) {
             if (n === e) return !0;
             n = n.parentNode
         }
         return !1
     }
-    var Br = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i,
-        Ar = /^#?([a-f\d])([a-f\d])([a-f\d])$/i,
-        zr = /^rgb\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *\)$/i,
-        Lr = /^rgba\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *([01]|0?\.\d+) *\)$/i;
+    var Ir = /^#?([a-f\d]{2})([a-f\d]{2})([a-f\d]{2})$/i,
+        Pr = /^#?([a-f\d])([a-f\d])([a-f\d])$/i,
+        Mr = /^rgb\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *\)$/i,
+        Dr = /^rgba\( *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *(1?\d{1,2}|2[0-4]\d|25[0-5]) *, *([01]|0?\.\d+) *\)$/i;
 
     function we(n) {
         if (n)
             for (; n.hasChildNodes() === !0;) {
                 let e = n.firstChild;
                 e && (we(e), n.removeChild(e))
             }
@@ -1604,15 +1604,15 @@
         return n
     }
 
     function zt(n, e) {
         return [...n, e]
     }
 
-    function Rr(n) {
+    function Fr(n) {
         return n.slice()
     }
 
     function As(n) {
         return n.getBoundingClientRect().left
     }
 
@@ -1637,22 +1637,22 @@
     }
 
     function bi(n) {
         let e;
         switch (n.length) {
             case 3:
             case 4:
-                return e = Ar.exec(n), e ? {
+                return e = Pr.exec(n), e ? {
                     r: parseInt(e[1] + e[1], 16),
                     g: parseInt(e[2] + e[2], 16),
                     b: parseInt(e[3] + e[3], 16)
                 } : null;
             case 6:
             case 7:
-                return e = Br.exec(n), e ? {
+                return e = Ir.exec(n), e ? {
                     r: parseInt(e[1], 16),
                     g: parseInt(e[2], 16),
                     b: parseInt(e[3], 16)
                 } : null;
             default:
                 return null
         }
@@ -1679,15 +1679,15 @@
             if (Ws(t)) {
                 let i = t.substr(4).substr(0, t.length - 5).split(",").map(function(s) {
                     return parseInt(s)
                 });
                 t = Hs(i[0], i[1], i[2])
             }
             if (js(t) === !0) {
-                let i = Hr(t),
+                let i = Nr(t),
                     s = {
                         h: i.h,
                         s: i.s * .8,
                         v: Math.min(1, i.v * 1.02)
                     },
                     o = {
                         h: i.h,
@@ -1810,30 +1810,30 @@
     }
 
     function Ht(n, e, t) {
         let i = Rt(n, e, t);
         return Hs(i.r, i.g, i.b)
     }
 
-    function Hr(n) {
+    function Nr(n) {
         let e = bi(n);
         if (!e) throw new TypeError(`'${n}' is not a valid color.`);
         return vt(e.r, e.g, e.b)
     }
 
     function js(n) {
         return /(^#[0-9A-F]{6}$)|(^#[0-9A-F]{3}$)/i.test(n)
     }
 
     function Ws(n) {
-        return zr.test(n)
+        return Mr.test(n)
     }
 
-    function jr(n) {
-        return Lr.test(n)
+    function Br(n) {
+        return Dr.test(n)
     }
 
     function Ee(n) {
         if (n === null || typeof n != "object") return null;
         if (n instanceof Element) return n;
         let e = Object.create(n);
         for (let t in n) Object.prototype.hasOwnProperty.call(n, t) && typeof n[t] == "object" && (e[t] = Ee(n[t]));
@@ -1925,15 +1925,15 @@
         for (let i of n)
             if (i) {
                 t = i[e[0]];
                 for (let s = 1; s < e.length; s++) t && (t = t[e[s]]);
                 if (typeof t != "undefined") break
             } return t
     }
-    var Wr = {
+    var Ar = {
             black: "#000000",
             navy: "#000080",
             darkblue: "#00008B",
             mediumblue: "#0000CD",
             blue: "#0000FF",
             darkgreen: "#006400",
             green: "#008000",
@@ -2096,29 +2096,29 @@
                 else throw new Error("Function attempted to set as colorPicker update callback is not a function.")
             }
             setCloseCallback(e) {
                 if (typeof e == "function") this.closeCallback = e;
                 else throw new Error("Function attempted to set as colorPicker closing callback is not a function.")
             }
             _isColorString(e) {
-                if (typeof e == "string") return Wr[e]
+                if (typeof e == "string") return Ar[e]
             }
             setColor(e, t = !0) {
                 if (e === "none") return;
                 let i, s = this._isColorString(e);
                 if (s !== void 0 && (e = s), _e(e) === !0) {
                     if (Ws(e) === !0) {
                         let o = e.substr(4).substr(0, e.length - 5).split(",");
                         i = {
                             r: o[0],
                             g: o[1],
                             b: o[2],
                             a: 1
                         }
-                    } else if (jr(e) === !0) {
+                    } else if (Br(e) === !0) {
                         let o = e.substr(5).substr(0, e.length - 6).split(",");
                         i = {
                             r: o[0],
                             g: o[1],
                             b: o[2],
                             a: o[3]
                         }
@@ -2638,15 +2638,15 @@
                     d = e.toLowerCase(),
                     h;
                 for (let l in t) {
                     let c;
                     if (t[l].__type__ !== void 0 && s === !0) {
                         let u = X.findInOptions(e, t[l], zt(i, l));
                         o > u.distance && (r = u.closestMatch, a = u.path, o = u.distance, h = u.indexMatch)
-                    } else l.toLowerCase().indexOf(d) !== -1 && (h = l), c = X.levenshteinDistance(e, l), o > c && (r = l, a = Rr(i), o = c)
+                    } else l.toLowerCase().indexOf(d) !== -1 && (h = l), c = X.levenshteinDistance(e, l), o > c && (r = l, a = Fr(i), o = c)
                 }
                 return {
                     closestMatch: r,
                     path: a,
                     distance: o,
                     indexMatch: h
                 }
@@ -2692,49 +2692,49 @@
         },
         Gs = me;
     var Ks = Us,
         Ue = mi,
         Zs = Ys,
         _i = wi,
         Qs = X;
-    var jt, Vr = new Uint8Array(16);
+    var jt, zr = new Uint8Array(16);
 
     function Ei() {
         if (!jt && (jt = typeof crypto != "undefined" && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || typeof msCrypto != "undefined" && typeof msCrypto.getRandomValues == "function" && msCrypto.getRandomValues.bind(msCrypto), !jt)) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
-        return jt(Vr)
+        return jt(zr)
     }
     var $s = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
 
-    function qr(n) {
+    function Lr(n) {
         return typeof n == "string" && $s.test(n)
     }
-    var Js = qr;
+    var Js = Lr;
     var Q = [];
     for (Wt = 0; Wt < 256; ++Wt) Q.push((Wt + 256).toString(16).substr(1));
     var Wt;
 
-    function Ur(n) {
+    function Rr(n) {
         var e = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0,
             t = (Q[n[e + 0]] + Q[n[e + 1]] + Q[n[e + 2]] + Q[n[e + 3]] + "-" + Q[n[e + 4]] + Q[n[e + 5]] + "-" + Q[n[e + 6]] + Q[n[e + 7]] + "-" + Q[n[e + 8]] + Q[n[e + 9]] + "-" + Q[n[e + 10]] + Q[n[e + 11]] + Q[n[e + 12]] + Q[n[e + 13]] + Q[n[e + 14]] + Q[n[e + 15]]).toLowerCase();
         if (!Js(t)) throw TypeError("Stringified UUID is invalid");
         return t
     }
-    var eo = Ur;
+    var eo = Rr;
 
-    function Yr(n, e, t) {
+    function Hr(n, e, t) {
         n = n || {};
         var i = n.random || (n.rng || Ei)();
         if (i[6] = i[6] & 15 | 64, i[8] = i[8] & 63 | 128, e) {
             t = t || 0;
             for (var s = 0; s < 16; ++s) e[t + s] = i[s];
             return e
         }
         return eo(i)
     }
-    var Ce = Yr;
+    var Ce = Hr;
 
     function to(n) {
         return typeof n == "string" || typeof n == "number"
     }
     var Vt = class {
             constructor(e) {
                 $(this, "delay");
@@ -2927,15 +2927,15 @@
             sort(e) {
                 return new Ie({
                     [Symbol.iterator]: () => [...this._pairs].sort(([t, i], [s, o]) => e(i, o, t, s))[Symbol.iterator]()
                 })
             }
         };
 
-    function Xr(n, e) {
+    function jr(n, e) {
         return n[e] == null && (n[e] = Ce()), n
     }
     var Te = class extends _t {
         constructor(e, t) {
             super();
             $(this, "flush");
             $(this, "length");
@@ -3206,15 +3206,15 @@
                         c = !0;
                         break
                     }! c && l !== void 0 && (s[o] = l, o++)
             }
             return s
         }
         _addItem(e) {
-            let t = Xr(e, this._idProp),
+            let t = jr(e, this._idProp),
                 i = t[this._idProp];
             if (this._data.has(i)) throw new Error("Cannot add item: item with id " + i + " already exists");
             return this._data.set(i, t), ++this.length, i
         }
         _updateItem(e) {
             let t = e[this._idProp];
             if (t == null) throw new Error("Cannot update item: item has no id (item: " + JSON.stringify(e) + ")");
@@ -3235,20 +3235,20 @@
                 })
             } else return new Ie({
                 [Symbol.iterator]: this._data.entries.bind(this._data)
             })
         }
     };
 
-    function Gr(n, e) {
+    function Wr(n, e) {
         return typeof e == "object" && e !== null && n === e.idProp && typeof e.add == "function" && typeof e.clear == "function" && typeof e.distinct == "function" && typeof e.forEach == "function" && typeof e.get == "function" && typeof e.getDataSet == "function" && typeof e.getIds == "function" && typeof e.length == "number" && typeof e.map == "function" && typeof e.max == "function" && typeof e.min == "function" && typeof e.off == "function" && typeof e.on == "function" && typeof e.remove == "function" && typeof e.setOptions == "function" && typeof e.stream == "function" && typeof e.update == "function" && typeof e.updateOnly == "function"
     }
 
     function xi(n, e) {
-        return typeof e == "object" && e !== null && n === e.idProp && typeof e.forEach == "function" && typeof e.get == "function" && typeof e.getDataSet == "function" && typeof e.getIds == "function" && typeof e.length == "number" && typeof e.map == "function" && typeof e.off == "function" && typeof e.on == "function" && typeof e.stream == "function" && Gr(n, e.getDataSet())
+        return typeof e == "object" && e !== null && n === e.idProp && typeof e.forEach == "function" && typeof e.get == "function" && typeof e.getDataSet == "function" && typeof e.getIds == "function" && typeof e.length == "number" && typeof e.map == "function" && typeof e.off == "function" && typeof e.on == "function" && typeof e.stream == "function" && Wr(n, e.getDataSet())
     }
     var no = ti(si());
 
     function qt(n) {
         var e = n && n.preventDefault || !1,
             t = n && n.container || window,
             i = {},
@@ -3402,46 +3402,46 @@
     }
     var Et = ti(oo());
 
     function Ci(n, e, t, i) {
         n.beginPath(), n.arc(e, t, i, 0, 2 * Math.PI, !1), n.closePath()
     }
 
-    function Kr(n, e, t, i) {
+    function Vr(n, e, t, i) {
         n.beginPath(), n.rect(e - i, t - i, i * 2, i * 2), n.closePath()
     }
 
-    function Zr(n, e, t, i) {
+    function qr(n, e, t, i) {
         n.beginPath(), i *= 1.15, t += .275 * i;
         let s = i * 2,
             o = s / 2,
             r = Math.sqrt(3) / 6 * s,
             a = Math.sqrt(s * s - o * o);
         n.moveTo(e, t - (a - r)), n.lineTo(e + o, t + r), n.lineTo(e - o, t + r), n.lineTo(e, t - (a - r)), n.closePath()
     }
 
-    function Qr(n, e, t, i) {
+    function Ur(n, e, t, i) {
         n.beginPath(), i *= 1.15, t -= .275 * i;
         let s = i * 2,
             o = s / 2,
             r = Math.sqrt(3) / 6 * s,
             a = Math.sqrt(s * s - o * o);
         n.moveTo(e, t + (a - r)), n.lineTo(e + o, t - r), n.lineTo(e - o, t - r), n.lineTo(e, t + (a - r)), n.closePath()
     }
 
-    function $r(n, e, t, i) {
+    function Yr(n, e, t, i) {
         n.beginPath(), i *= .82, t += .1 * i;
         for (let s = 0; s < 10; s++) {
             let o = s % 2 == 0 ? i * 1.3 : i * .5;
             n.lineTo(e + o * Math.sin(s * 2 * Math.PI / 10), t - o * Math.cos(s * 2 * Math.PI / 10))
         }
         n.closePath()
     }
 
-    function Jr(n, e, t, i) {
+    function Xr(n, e, t, i) {
         n.beginPath(), n.lineTo(e, t + i), n.lineTo(e + i, t), n.lineTo(e, t - i), n.lineTo(e - i, t), n.closePath()
     }
 
     function ro(n, e, t, i, s, o) {
         let r = Math.PI / 180;
         i - 2 * o < 0 && (o = i / 2), s - 2 * o < 0 && (o = s / 2), n.beginPath(), n.moveTo(e + o, t), n.lineTo(e + i - o, t), n.arc(e + i - o, t + o, o, r * 270, r * 360, !1), n.lineTo(e + i, t + s - o), n.arc(e + i - o, t + s - o, o, 0, r * 90, !1), n.lineTo(e + o, t + s), n.arc(e + o, t + s - o, o, r * 90, r * 180, !1), n.lineTo(e, t + o), n.arc(e + o, t + o, o, r * 180, r * 270, !1), n.closePath()
     }
@@ -3483,45 +3483,45 @@
             c = 0,
             u = !0,
             p = 0,
             b = +o[0];
         for (; l >= .1;) b = +o[c++ % r], b > l && (b = l), p = Math.sqrt(b * b / (1 + h * h)), p = a < 0 ? -p : p, e += p, t += h * p, u === !0 ? n.lineTo(e, t) : n.moveTo(e, t), l -= b, u = !u
     }
 
-    function ea(n, e, t, i) {
+    function Gr(n, e, t, i) {
         n.beginPath();
         let s = 6,
             o = Math.PI * 2 / s;
         n.moveTo(e + i, t);
         for (let r = 1; r < s; r++) n.lineTo(e + i * Math.cos(o * r), t + i * Math.sin(o * r));
         n.closePath()
     }
     var lo = {
         circle: Ci,
         dashedLine: ho,
         database: ao,
-        diamond: Jr,
+        diamond: Xr,
         ellipse: Ti,
         ellipse_vis: Ti,
-        hexagon: ea,
+        hexagon: Gr,
         roundRect: ro,
-        square: Kr,
-        star: $r,
-        triangle: Zr,
-        triangleDown: Qr
+        square: Vr,
+        star: Yr,
+        triangle: qr,
+        triangleDown: Ur
     };
 
-    function ta(n) {
+    function Kr(n) {
         return Object.prototype.hasOwnProperty.call(lo, n) ? lo[n] : function(e, ...t) {
             CanvasRenderingContext2D.prototype[n].call(e, t)
         }
     }
 
-    function ia(n) {
-        return Pe = n, ra()
+    function Zr(n) {
+        return Pe = n, ea()
     }
     var co = {
             fontsize: "font.size",
             fontcolor: "font.color",
             labelfontcolor: "font.color",
             fontname: "font.face",
             color: ["color.border", "color.background"],
@@ -3551,15 +3551,15 @@
         },
         Pe = "",
         it = 0,
         z = "",
         M = "",
         oe = te.NULL;
 
-    function sa() {
+    function Qr() {
         it = 0, z = Pe.charAt(0)
     }
 
     function Z() {
         it++, z = Pe.charAt(it)
     }
 
@@ -3574,15 +3574,15 @@
 
     function Me(n, e) {
         if (n || (n = {}), e)
             for (var t in e) e.hasOwnProperty(t) && (n[t] = e[t]);
         return n
     }
 
-    function oa(n, e, t) {
+    function $r(n, e, t) {
         for (var i = e.split("."), s = n; i.length;) {
             var o = i.shift();
             i.length ? (s[o] || (s[o] = {}), s = s[o]) : s[o] = t
         }
     }
 
     function po(n, e) {
@@ -3599,15 +3599,15 @@
             }, n.node && (s.attr = Me(s.attr, n.node))), t = o.length - 1; t >= 0; t--) {
             var a = o[t];
             a.nodes || (a.nodes = []), a.nodes.indexOf(s) === -1 && a.nodes.push(s)
         }
         e.attr && (s.attr = Me(s.attr, e.attr))
     }
 
-    function na(n, e) {
+    function Jr(n, e) {
         if (n.edges || (n.edges = []), n.edges.push(e), n.edge) {
             var t = Me({}, n.edge);
             e.attr = Me(t, e.attr)
         }
     }
 
     function go(n, e, t, i, s) {
@@ -3679,57 +3679,57 @@
             Z(), oe = te.IDENTIFIER;
             return
         }
         for (oe = te.UNKNOWN; z != "";) M += z, Z();
         throw new SyntaxError('Syntax error in part "' + vo(M, 30) + '"')
     }
 
-    function ra() {
+    function ea() {
         var n = {};
-        if (sa(), V(), M === "strict" && (n.strict = !0, V()), (M === "graph" || M === "digraph") && (n.type = M, V()), oe === te.IDENTIFIER && (n.id = M, V()), M != "{") throw ie("Angle bracket { expected");
+        if (Qr(), V(), M === "strict" && (n.strict = !0, V()), (M === "graph" || M === "digraph") && (n.type = M, V()), oe === te.IDENTIFIER && (n.id = M, V()), M != "{") throw ie("Angle bracket { expected");
         if (V(), mo(n), M != "}") throw ie("Angle bracket } expected");
         if (V(), M !== "") throw ie("End of file expected");
         return V(), delete n.node, delete n.edge, delete n.graph, n
     }
 
     function mo(n) {
-        for (; M !== "" && M != "}";) aa(n), M === ";" && V()
+        for (; M !== "" && M != "}";) ta(n), M === ";" && V()
     }
 
-    function aa(n) {
+    function ta(n) {
         var e = yo(n);
         if (e) {
             bo(n, e);
             return
         }
-        var t = da(n);
+        var t = ia(n);
         if (!t) {
             if (oe != te.IDENTIFIER) throw ie("Identifier expected");
             var i = M;
             if (V(), M === "=") {
                 if (V(), oe != te.IDENTIFIER) throw ie("Identifier expected");
                 n[i] = M, V()
-            } else ha(n, i)
+            } else sa(n, i)
         }
     }
 
     function yo(n) {
         var e = null;
         if (M === "subgraph" && (e = {}, e.type = "subgraph", V(), oe === te.IDENTIFIER && (e.id = M, V())), M === "{") {
             if (V(), e || (e = {}), e.parent = n, e.node = n.node, e.edge = n.edge, e.graph = n.graph, mo(e), M != "}") throw ie("Angle bracket } expected");
             V(), delete e.node, delete e.edge, delete e.graph, delete e.parent, n.subgraphs || (n.subgraphs = []), n.subgraphs.push(e)
         }
         return e
     }
 
-    function da(n) {
+    function ia(n) {
         return M === "node" ? (V(), n.node = xt(), "node") : M === "edge" ? (V(), n.edge = xt(), "edge") : M === "graph" ? (V(), n.graph = xt(), "graph") : null
     }
 
-    function ha(n, e) {
+    function sa(n, e) {
         var t = {
                 id: e
             },
             i = xt();
         i && (t.attr = i), po(n, t), bo(n, e)
     }
 
@@ -3743,15 +3743,15 @@
                 if (oe != te.IDENTIFIER) throw ie("Identifier or subgraph expected");
                 t = M, po(n, {
                     id: t
                 }), V()
             }
             var o = xt(),
                 r = go(n, e, t, i, o);
-            na(n, r), e = t
+            Jr(n, r), e = t
         }
     }
 
     function xt() {
         for (var n, e = null, t = {
                 dashed: !0,
                 solid: !1,
@@ -3997,27 +3997,27 @@
         }
         var b;
         if (o.includes("penwidth")) {
             var C = [];
             for (b = s.length, n = 0; n < b; n++) s[n].name !== "width" && (s[n].name === "penwidth" && (s[n].name = "width"), C.push(s[n]));
             s = C
         }
-        for (b = s.length, n = 0; n < b; n++) oa(s[n].attr, s[n].name, s[n].value);
+        for (b = s.length, n = 0; n < b; n++) $r(s[n].attr, s[n].name, s[n].value);
         return e
     }
 
     function ie(n) {
         return new SyntaxError(n + ', got "' + vo(M, 30) + '" (char ' + it + ")")
     }
 
     function vo(n, e) {
         return n.length <= e ? n : n.substr(0, 27) + "..."
     }
 
-    function la(n, e, t) {
+    function oa(n, e, t) {
         Array.isArray(n) ? n.forEach(function(i) {
             Array.isArray(e) ? e.forEach(function(s) {
                 t(i, s)
             }) : t(i, e)
         }) : Array.isArray(e) ? e.forEach(function(i) {
             t(n, i)
         }) : t(n, e)
@@ -4038,16 +4038,16 @@
                 var s = e[i];
                 Array.isArray(s) ? s.forEach(function(o) {
                     Si(t, o, n[i])
                 }) : typeof s == "string" ? Si(t, s, n[i]) : Si(t, i, n[i])
             } return t
     }
 
-    function ca(n) {
-        var e = ia(n),
+    function na(n) {
+        var e = Zr(n),
             t = {
                 nodes: [],
                 edges: [],
                 options: {}
             };
         if (e.nodes && e.nodes.forEach(function(s) {
                 var o = {
@@ -4068,28 +4068,28 @@
                 s.from instanceof Object ? o = s.from.nodes : o = {
                     id: s.from
                 }, s.to instanceof Object ? r = s.to.nodes : r = {
                     id: s.to
                 }, s.from instanceof Object && s.from.edges && s.from.edges.forEach(function(a) {
                     var d = i(a);
                     t.edges.push(d)
-                }), la(o, r, function(a, d) {
+                }), oa(o, r, function(a, d) {
                     var h = go(t, a.id, d.id, s.type, s.attr),
                         l = i(h);
                     t.edges.push(l)
                 }), s.to instanceof Object && s.to.edges && s.to.edges.forEach(function(a) {
                     var d = i(a);
                     t.edges.push(d)
                 })
             })
         }
         return e.attr && (t.options = e.attr), t
     }
 
-    function ua(n, e) {
+    function ra(n, e) {
         let t = {
             edges: {
                 inheritColor: !1
             },
             nodes: {
                 fixed: !1,
                 parseColor: !1
@@ -4122,15 +4122,15 @@
                         border: r.color
                     }
                 }), a
             }),
             edges: s
         }
     }
-    var fa = {
+    var aa = {
             addDescription: "Click in an empty space to place a new node.",
             addEdge: "Add Edge",
             addNode: "Add Node",
             back: "Back",
             close: "Close",
             createEdgeError: "Cannot link edges to a cluster.",
             del: "Delete selected",
@@ -4138,15 +4138,15 @@
             edgeDescription: "Click on a node and drag the edge to another node to connect them.",
             edit: "Edit",
             editClusterError: "Clusters cannot be edited.",
             editEdge: "Edit Edge",
             editEdgeDescription: "Click on the control points and drag them to a node to connect to it.",
             editNode: "Edit Node"
         },
-        pa = {
+        da = {
             addDescription: "Klicke auf eine freie Stelle, um einen neuen Knoten zu plazieren.",
             addEdge: "Kante hinzuf\xFCgen",
             addNode: "Knoten hinzuf\xFCgen",
             back: "Zur\xFCck",
             close: "Schlie\xDFen",
             createEdgeError: "Es ist nicht m\xF6glich, Kanten mit Clustern zu verbinden.",
             del: "L\xF6sche Auswahl",
@@ -4154,15 +4154,15 @@
             edgeDescription: "Klicke auf einen Knoten und ziehe die Kante zu einem anderen Knoten, um diese zu verbinden.",
             edit: "Editieren",
             editClusterError: "Cluster k\xF6nnen nicht editiert werden.",
             editEdge: "Kante editieren",
             editEdgeDescription: "Klicke auf die Verbindungspunkte und ziehe diese auf einen Knoten, um sie zu verbinden.",
             editNode: "Knoten editieren"
         },
-        ga = {
+        ha = {
             addDescription: "Haga clic en un lugar vac\xEDo para colocar un nuevo nodo.",
             addEdge: "A\xF1adir arista",
             addNode: "A\xF1adir nodo",
             back: "Atr\xE1s",
             close: "Cerrar",
             createEdgeError: "No se puede conectar una arista a un grupo.",
             del: "Eliminar selecci\xF3n",
@@ -4170,15 +4170,15 @@
             edgeDescription: "Haga clic en un nodo y arrastre la arista hacia otro nodo para conectarlos.",
             edit: "Editar",
             editClusterError: "No es posible editar grupos.",
             editEdge: "Editar arista",
             editEdgeDescription: "Haga clic en un punto de control y arrastrelo a un nodo para conectarlo.",
             editNode: "Editar nodo"
         },
-        ma = {
+        la = {
             addDescription: "Clicca per aggiungere un nuovo nodo",
             addEdge: "Aggiungi un vertice",
             addNode: "Aggiungi un nodo",
             back: "Indietro",
             close: "Chiudere",
             createEdgeError: "Non si possono collegare vertici ad un cluster",
             del: "Cancella la selezione",
@@ -4186,15 +4186,15 @@
             edgeDescription: "Clicca su un nodo e trascinalo ad un altro nodo per connetterli.",
             edit: "Modifica",
             editClusterError: "I clusters non possono essere modificati.",
             editEdge: "Modifica il vertice",
             editEdgeDescription: "Clicca sui Punti di controllo e trascinali ad un nodo per connetterli.",
             editNode: "Modifica il nodo"
         },
-        ya = {
+        ca = {
             addDescription: "Klik op een leeg gebied om een nieuwe node te maken.",
             addEdge: "Link toevoegen",
             addNode: "Node toevoegen",
             back: "Terug",
             close: "Sluiten",
             createEdgeError: "Kan geen link maken naar een cluster.",
             del: "Selectie verwijderen",
@@ -4202,15 +4202,15 @@
             edgeDescription: "Klik op een node en sleep de link naar een andere node om ze te verbinden.",
             edit: "Wijzigen",
             editClusterError: "Clusters kunnen niet worden aangepast.",
             editEdge: "Link wijzigen",
             editEdgeDescription: "Klik op de verbindingspunten en sleep ze naar een node om daarmee te verbinden.",
             editNode: "Node wijzigen"
         },
-        ba = {
+        ua = {
             addDescription: "Clique em um espa\xE7o em branco para adicionar um novo n\xF3",
             addEdge: "Adicionar aresta",
             addNode: "Adicionar n\xF3",
             back: "Voltar",
             close: "Fechar",
             createEdgeError: "N\xE3o foi poss\xEDvel linkar arestas a um cluster.",
             del: "Remover selecionado",
@@ -4218,15 +4218,15 @@
             edgeDescription: "Clique em um n\xF3 e arraste a aresta at\xE9 outro n\xF3 para conect\xE1-los",
             edit: "Editar",
             editClusterError: "Clusters n\xE3o puderam ser editados.",
             editEdge: "Editar aresta",
             editEdgeDescription: "Clique nos pontos de controle e os arraste para um n\xF3 para conect\xE1-los",
             editNode: "Editar n\xF3"
         },
-        va = {
+        fa = {
             addDescription: "\u041A\u043B\u0438\u043A\u043D\u0438\u0442\u0435 \u0432 \u0441\u0432\u043E\u0431\u043E\u0434\u043D\u043E\u0435 \u043C\u0435\u0441\u0442\u043E, \u0447\u0442\u043E\u0431\u044B \u0434\u043E\u0431\u0430\u0432\u0438\u0442\u044C \u043D\u043E\u0432\u044B\u0439 \u0443\u0437\u0435\u043B.",
             addEdge: "\u0414\u043E\u0431\u0430\u0432\u0438\u0442\u044C \u0440\u0435\u0431\u0440\u043E",
             addNode: "\u0414\u043E\u0431\u0430\u0432\u0438\u0442\u044C \u0443\u0437\u0435\u043B",
             back: "\u041D\u0430\u0437\u0430\u0434",
             close: "\u0417\u0430\u043A\u0440\u044B\u0432\u0430\u0442\u044C",
             createEdgeError: "\u041D\u0435\u0432\u043E\u0437\u043C\u043E\u0436\u043D\u043E \u0441\u043E\u0435\u0434\u0438\u043D\u0438\u0442\u044C \u0440\u0435\u0431\u0440\u0430 \u0432 \u043A\u043B\u0430\u0441\u0442\u0435\u0440.",
             del: "\u0423\u0434\u0430\u043B\u0438\u0442\u044C \u0432\u044B\u0431\u0440\u0430\u043D\u043D\u043E\u0435",
@@ -4234,15 +4234,15 @@
             edgeDescription: "\u041A\u043B\u0438\u043A\u043D\u0438\u0442\u0435 \u043D\u0430 \u0443\u0437\u0435\u043B \u0438 \u043F\u0440\u043E\u0442\u044F\u043D\u0438\u0442\u0435 \u0440\u0435\u0431\u0440\u043E \u043A \u0434\u0440\u0443\u0433\u043E\u043C\u0443 \u0443\u0437\u043B\u0443, \u0447\u0442\u043E\u0431\u044B \u0441\u043E\u0435\u0434\u0438\u043D\u0438\u0442\u044C \u0438\u0445.",
             edit: "\u0420\u0435\u0434\u0430\u043A\u0442\u0438\u0440\u043E\u0432\u0430\u0442\u044C",
             editClusterError: "\u041A\u043B\u0430\u0441\u0442\u0435\u0440\u044B \u043D\u0435\u0434\u043E\u0441\u0442\u0443\u043F\u043D\u044B \u0434\u043B\u044F \u0440\u0435\u0434\u0430\u043A\u0442\u0438\u0440\u043E\u0432\u0430\u043D\u0438\u044F.",
             editEdge: "\u0420\u0435\u0434\u0430\u043A\u0442\u0438\u0440\u043E\u0432\u0430\u0442\u044C \u0440\u0435\u0431\u0440\u043E",
             editEdgeDescription: "\u041A\u043B\u0438\u043A\u043D\u0438\u0442\u0435 \u043D\u0430 \u043A\u043E\u043D\u0442\u0440\u043E\u043B\u044C\u043D\u044B\u0435 \u0442\u043E\u0447\u043A\u0438 \u0438 \u043F\u0435\u0440\u0435\u0442\u0430\u0449\u0438\u0442\u0435 \u0438\u0445 \u0432 \u0443\u0437\u0435\u043B, \u0447\u0442\u043E\u0431\u044B \u043F\u043E\u0434\u043A\u043B\u044E\u0447\u0438\u0442\u044C\u0441\u044F \u043A \u043D\u0435\u043C\u0443.",
             editNode: "\u0420\u0435\u0434\u0430\u043A\u0442\u0438\u0440\u043E\u0432\u0430\u0442\u044C \u0443\u0437\u0435\u043B"
         },
-        wa = {
+        pa = {
             addDescription: "\u5355\u51FB\u7A7A\u767D\u5904\u653E\u7F6E\u65B0\u8282\u70B9\u3002",
             addEdge: "\u6DFB\u52A0\u8FDE\u63A5\u7EBF",
             addNode: "\u6DFB\u52A0\u8282\u70B9",
             back: "\u8FD4\u56DE",
             close: "\u95DC\u9589",
             createEdgeError: "\u65E0\u6CD5\u5C06\u8FDE\u63A5\u7EBF\u8FDE\u63A5\u5230\u7FA4\u96C6\u3002",
             del: "\u5220\u9664\u9009\u5B9A",
@@ -4250,15 +4250,15 @@
             edgeDescription: "\u5355\u51FB\u67D0\u4E2A\u8282\u70B9\u5E76\u5C06\u8BE5\u8FDE\u63A5\u7EBF\u62D6\u52A8\u5230\u53E6\u4E00\u4E2A\u8282\u70B9\u4EE5\u8FDE\u63A5\u5B83\u4EEC\u3002",
             edit: "\u7F16\u8F91",
             editClusterError: "\u65E0\u6CD5\u7F16\u8F91\u7FA4\u96C6\u3002",
             editEdge: "\u7F16\u8F91\u8FDE\u63A5\u7EBF",
             editEdgeDescription: "\u5355\u51FB\u63A7\u5236\u8282\u70B9\u5E76\u5C06\u5B83\u4EEC\u62D6\u5230\u8282\u70B9\u4E0A\u8FDE\u63A5\u3002",
             editNode: "\u7F16\u8F91\u8282\u70B9"
         },
-        _a = {
+        ga = {
             addDescription: "K\u043B\u0456\u043A\u043D\u0456\u0442\u044C \u043D\u0430 \u0432\u0456\u043B\u044C\u043D\u0435 \u043C\u0456\u0441\u0446\u0435, \u0449\u043E\u0431 \u0434\u043E\u0434\u0430\u0442\u0438 \u043D\u043E\u0432\u0438\u0439 \u0432\u0443\u0437\u043E\u043B.",
             addEdge: "\u0414\u043E\u0434\u0430\u0442\u0438 \u043A\u0440\u0430\u0439",
             addNode: "\u0414\u043E\u0434\u0430\u0442\u0438 \u0432\u0443\u0437\u043E\u043B",
             back: "\u041D\u0430\u0437\u0430\u0434",
             close: "\u0417\u0430\u043A\u0440\u0438\u0442\u0438",
             createEdgeError: "\u041D\u0435 \u043C\u043E\u0436\u043B\u0438\u0432\u043E \u043E\u0431'\u0454\u0434\u043D\u0430\u0442\u0438 \u043A\u0440\u0430\u0457 \u0432 \u0433\u0440\u0443\u043F\u0443.",
             del: "\u0412\u0438\u0434\u0430\u043B\u0438\u0442\u0438 \u043E\u0431\u0440\u0430\u043D\u0435",
@@ -4266,15 +4266,15 @@
             edgeDescription: "\u041A\u043B\u0456\u043A\u043D\u0456\u0442\u044C \u043D\u0430 \u0432\u0443\u0437\u043E\u043B \u0456 \u043F\u0435\u0440\u0435\u0442\u044F\u0433\u043D\u0456\u0442\u044C \u043A\u0440\u0430\u0439 \u0434\u043E \u0456\u043D\u0448\u043E\u0433\u043E \u0432\u0443\u0437\u043B\u0430, \u0449\u043E\u0431 \u0457\u0445 \u0437'\u0454\u0434\u043D\u0430\u0442\u0438.",
             edit: "\u0420\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u0442\u0438",
             editClusterError: "\u0413\u0440\u0443\u043F\u0438 \u043D\u0435\u0434\u043E\u0441\u0442\u0443\u043F\u043D\u0456 \u0434\u043B\u044F \u0440\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u043D\u043D\u044F.",
             editEdge: "\u0420\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u0442\u0438 \u043A\u0440\u0430\u0439",
             editEdgeDescription: "\u041A\u043B\u0456\u043A\u043D\u0456\u0442\u044C \u043D\u0430 \u043A\u043E\u043D\u0442\u0440\u043E\u043B\u044C\u043D\u0456 \u0442\u043E\u0447\u043A\u0438 \u0456 \u043F\u0435\u0440\u0435\u0442\u044F\u0433\u043D\u0456\u0442\u044C \u0457\u0445 \u0443 \u0432\u0443\u0437\u043E\u043B, \u0449\u043E\u0431 \u043F\u0456\u0434\u043A\u043B\u044E\u0447\u0438\u0442\u0438\u0441\u044F \u0434\u043E \u043D\u044C\u043E\u0433\u043E.",
             editNode: "\u0420\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u0442\u0438 \u0432\u0443\u0437\u043E\u043B"
         },
-        Ea = {
+        ma = {
             addDescription: "Cliquez dans un endroit vide pour placer un n\u0153ud.",
             addEdge: "Ajouter un lien",
             addNode: "Ajouter un n\u0153ud",
             back: "Retour",
             close: "Fermer",
             createEdgeError: "Impossible de cr\xE9er un lien vers un cluster.",
             del: "Effacer la s\xE9lection",
@@ -4282,15 +4282,15 @@
             edgeDescription: "Cliquez sur un n\u0153ud et glissez le lien vers un autre n\u0153ud pour les connecter.",
             edit: "\xC9diter",
             editClusterError: "Les clusters ne peuvent pas \xEAtre \xE9dit\xE9s.",
             editEdge: "\xC9diter le lien",
             editEdgeDescription: "Cliquez sur les points de contr\xF4le et glissez-les pour connecter un n\u0153ud.",
             editNode: "\xC9diter le n\u0153ud"
         },
-        xa = {
+        ya = {
             addDescription: "Kluknut\xEDm do pr\xE1zdn\xE9ho prostoru m\u016F\u017Eete p\u0159idat nov\xFD vrchol.",
             addEdge: "P\u0159idat hranu",
             addNode: "P\u0159idat vrchol",
             back: "Zp\u011Bt",
             close: "Zav\u0159\xEDt",
             createEdgeError: "Nelze p\u0159ipojit hranu ke shluku.",
             del: "Smazat v\xFDb\u011Br",
@@ -4298,30 +4298,30 @@
             edgeDescription: "P\u0159eta\u017Een\xEDm z jednoho vrcholu do druh\xE9ho m\u016F\u017Eete spojit tyto vrcholy novou hranou.",
             edit: "Upravit",
             editClusterError: "Nelze upravovat shluky.",
             editEdge: "Upravit hranu",
             editEdgeDescription: "P\u0159eta\u017Een\xEDm kontroln\xEDho vrcholu hrany ji m\u016F\u017Eete p\u0159ipojit k jin\xE9mu vrcholu.",
             editNode: "Upravit vrchol"
         },
-        Ca = Object.freeze({
+        ba = Object.freeze({
             __proto__: null,
-            en: fa,
-            de: pa,
-            es: ga,
-            it: ma,
-            nl: ya,
-            pt: ba,
-            ru: va,
-            cn: wa,
-            uk: _a,
-            fr: Ea,
-            cs: xa
+            cn: pa,
+            cs: ya,
+            de: da,
+            en: aa,
+            es: ha,
+            fr: ma,
+            it: la,
+            nl: ca,
+            pt: ua,
+            ru: fa,
+            uk: ga
         });
 
-    function Ta(n, e) {
+    function va(n, e) {
         try {
             let [t, i] = e.split(/[-_ /]/, 2), s = t != null ? t.toLowerCase() : null, o = i != null ? i.toUpperCase() : null;
             if (s && o) {
                 let r = s + "-" + o;
                 if (Object.prototype.hasOwnProperty.call(n, r)) return r;
                 console.warn(`Unknown variant ${o} of language ${s}.`)
             }
@@ -4792,15 +4792,15 @@
                 return {
                     width: this.width,
                     height: this.height,
                     lines: e
                 }
             }
         },
-        ka = {
+        wa = {
             "<b>": /<b>/,
             "<i>": /<i>/,
             "<code>": /<code>/,
             "</b>": /<\/b>/,
             "</i>": /<\/i>/,
             "</code>": /<\/code>/,
             "*": /\*/,
@@ -4856,15 +4856,15 @@
             replace(e, t) {
                 return this.match(e) ? (this.add(t), this.position += length - 1, !0) : !1
             }
             prepareRegExp(e) {
                 let t, i;
                 if (e instanceof RegExp) i = e, t = 1;
                 else {
-                    let s = ka[e];
+                    let s = wa[e];
                     s !== void 0 ? i = s : i = new RegExp(e), t = e.length
                 }
                 return [i, t]
             }
         },
         ko = class {
             constructor(e, t, i, s) {
@@ -5288,15 +5288,15 @@
                     r = 14;
                 return s === 0 && (s = r, o = r), {
                     width: s,
                     height: o
                 }
             }
         },
-        So = class extends De {
+        _a = class extends De {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.needsRefresh(t, i)) {
                     let s = this.getDimensionsFromLabel(e, t, i);
@@ -5383,15 +5383,15 @@
                     let d = this.labelModule.getTextSize(e, s, o);
                     d.lineCount >= 1 && (r += d.height / 2)
                 }
                 let a = i + r;
                 this.options.label && (this.labelOffset = r), this.labelModule.draw(e, t, a, s, o, "hanging")
             }
         },
-        Oo = class extends Gt {
+        Ea = class extends Gt {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.needsRefresh(t, i)) {
                     let s = this.getDimensionsFromLabel(e, t, i),
@@ -5405,15 +5405,15 @@
             updateBoundingBox(e, t) {
                 this.boundingBox.top = t - this.options.size, this.boundingBox.left = e - this.options.size, this.boundingBox.right = e + this.options.size, this.boundingBox.bottom = t + this.options.size
             }
             distanceToBorder(e) {
                 return e && this.resize(e), this.width * .5
             }
         },
-        Io = class extends Gt {
+        So = class extends Gt {
             constructor(e, t, i, s, o) {
                 super(e, t, i);
                 this.setImages(s, o)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.imageObj.src === void 0 || this.imageObj.width === void 0 || this.imageObj.height === void 0) {
                     let o = this.options.size * 2;
@@ -5446,30 +5446,30 @@
                 if (this.needsRefresh(t, i)) {
                     this.labelModule.getTextSize(e, t, i);
                     let a = 2 * s.size;
                     this.width = (o = this.customSizeWidth) != null ? o : a, this.height = (r = this.customSizeHeight) != null ? r : a, this.radius = .5 * this.width
                 }
             }
             _drawShape(e, t, i, s, o, r, a, d) {
-                return this.resize(e, r, a, d), this.left = s - this.width / 2, this.top = o - this.height / 2, this.initContextForDraw(e, d), ta(t)(e, s, o, d.size), this.performFill(e, d), this.options.icon !== void 0 && this.options.icon.code !== void 0 && (e.font = (r ? "bold " : "") + this.height / 2 + "px " + (this.options.icon.face || "FontAwesome"), e.fillStyle = this.options.icon.color || "black", e.textAlign = "center", e.textBaseline = "middle", e.fillText(this.options.icon.code, s, o)), {
+                return this.resize(e, r, a, d), this.left = s - this.width / 2, this.top = o - this.height / 2, this.initContextForDraw(e, d), Kr(t)(e, s, o, d.size), this.performFill(e, d), this.options.icon !== void 0 && this.options.icon.code !== void 0 && (e.font = (r ? "bold " : "") + this.height / 2 + "px " + (this.options.icon.face || "FontAwesome"), e.fillStyle = this.options.icon.color || "black", e.textAlign = "center", e.textBaseline = "middle", e.fillText(this.options.icon.code, s, o)), {
                     drawExternalLabel: () => {
                         if (this.options.label !== void 0) {
                             this.labelModule.calculateLabelSize(e, r, a, s, o, "hanging");
                             let h = o + .5 * this.height + .5 * this.labelModule.size.height;
                             this.labelModule.draw(e, s, h, r, a, "hanging")
                         }
                         this.updateBoundingBox(s, o)
                     }
                 }
             }
             updateBoundingBox(e, t) {
                 this.boundingBox.top = t - this.options.size, this.boundingBox.left = e - this.options.size, this.boundingBox.right = e + this.options.size, this.boundingBox.bottom = t + this.options.size, this.options.label !== void 0 && this.labelModule.size.width > 0 && (this.boundingBox.left = Math.min(this.boundingBox.left, this.labelModule.size.left), this.boundingBox.right = Math.max(this.boundingBox.right, this.labelModule.size.left + this.labelModule.size.width), this.boundingBox.bottom = Math.max(this.boundingBox.bottom, this.boundingBox.bottom + this.labelModule.size.height))
             }
         },
-        Po = class extends ke {
+        Oo = class extends ke {
             constructor(e, t, i, s) {
                 super(e, t, i, s);
                 this.ctxRenderer = s
             }
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o, r), this.left = t - this.width / 2, this.top = i - this.height / 2, e.save();
                 let a = this.ctxRenderer({
@@ -5492,15 +5492,15 @@
                 }
                 return a.nodeDimensions && (this.customSizeWidth = a.nodeDimensions.width, this.customSizeHeight = a.nodeDimensions.height), a
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Mo = class extends De {
+        Io = class extends De {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 if (this.needsRefresh(t, i)) {
                     let o = this.getDimensionsFromLabel(e, t, i).width + this.margin.right + this.margin.left;
@@ -5510,26 +5510,26 @@
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o), this.left = t - this.width / 2, this.top = i - this.height / 2, this.initContextForDraw(e, r), ao(e, t - this.width / 2, i - this.height / 2, this.width, this.height), this.performFill(e, r), this.updateBoundingBox(t, i, e, s, o), this.labelModule.draw(e, this.left + this.textSize.width / 2 + this.margin.left, this.top + this.textSize.height / 2 + this.margin.top, s, o)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Do = class extends ke {
+        xa = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "diamond", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Fo = class extends ke {
+        Po = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "circle", 2, t, i, s, o, r)
             }
             distanceToBorder(e) {
@@ -5554,15 +5554,15 @@
                 let i = this.width * .5,
                     s = this.height * .5,
                     o = Math.sin(t) * i,
                     r = Math.cos(t) * s;
                 return i * s / Math.sqrt(o * o + r * r)
             }
         },
-        No = class extends De {
+        Mo = class extends De {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 this.needsRefresh(t, i) && (this.iconSize = {
                     width: Number(this.options.icon.size),
@@ -5590,15 +5590,15 @@
                 let a = Number(this.options.icon.size);
                 this.options.icon.code !== void 0 ? (e.font = [this.options.icon.weight != null ? this.options.icon.weight : s ? "bold" : "", (this.options.icon.weight != null && s ? 5 : 0) + a + "px", this.options.icon.face].join(" "), e.fillStyle = this.options.icon.color || "black", e.textAlign = "center", e.textBaseline = "middle", this.enableShadow(e, r), e.fillText(this.options.icon.code, t, i), this.disableShadow(e, r)) : console.error("When using the icon shape, you need to define the code in the icon options object. This can be done per node or globally.")
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Bo = class extends Gt {
+        Ca = class extends Gt {
             constructor(e, t, i, s, o) {
                 super(e, t, i);
                 this.setImages(s, o)
             }
             resize(e, t = this.selected, i = this.hover) {
                 if (this.imageObj.src === void 0 || this.imageObj.width === void 0 || this.imageObj.height === void 0) {
                     let o = this.options.size * 2;
@@ -5625,74 +5625,74 @@
             updateBoundingBox(e, t) {
                 this.resize(), this.options.shapeProperties.coordinateOrigin === "top-left" ? (this.left = e, this.top = t) : (this.left = e - this.width / 2, this.top = t - this.height / 2), this.boundingBox.left = this.left, this.boundingBox.top = this.top, this.boundingBox.bottom = this.top + this.height, this.boundingBox.right = this.left + this.width, this.options.label !== void 0 && this.labelModule.size.width > 0 && (this.boundingBox.left = Math.min(this.boundingBox.left, this.labelModule.size.left), this.boundingBox.right = Math.max(this.boundingBox.right, this.labelModule.size.left + this.labelModule.size.width), this.boundingBox.bottom = Math.max(this.boundingBox.bottom, this.boundingBox.bottom + this.labelOffset))
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Ao = class extends ke {
+        Do = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "square", 2, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        zo = class extends ke {
+        Fo = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "hexagon", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Lo = class extends ke {
+        No = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "star", 4, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Ro = class extends De {
+        Bo = class extends De {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._setMargins(i)
             }
             resize(e, t, i) {
                 this.needsRefresh(t, i) && (this.textSize = this.labelModule.getTextSize(e, t, i), this.width = this.textSize.width + this.margin.right + this.margin.left, this.height = this.textSize.height + this.margin.top + this.margin.bottom, this.radius = .5 * this.width)
             }
             draw(e, t, i, s, o, r) {
                 this.resize(e, s, o), this.left = t - this.width / 2, this.top = i - this.height / 2, this.enableShadow(e, r), this.labelModule.draw(e, this.left + this.textSize.width / 2 + this.margin.left, this.top + this.textSize.height / 2 + this.margin.top, s, o), this.disableShadow(e, r), this.updateBoundingBox(t, i, e, s, o)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        Ho = class extends ke {
+        Ta = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "triangle", 3, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
                 return this._distanceToBorder(e, t)
             }
         },
-        jo = class extends ke {
+        Ao = class extends ke {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             draw(e, t, i, s, o, r) {
                 return this._drawShape(e, "triangleDown", 3, t, i, s, o, r)
             }
             distanceToBorder(e, t) {
@@ -5781,60 +5781,60 @@
                     i = [e, this.options, t, this.globalOptions, this.defaultOptions];
                 this.labelModule.update(this.options, i), this.labelModule.baseSize !== void 0 && (this.baseFontSize = this.labelModule.baseSize)
             }
             updateShape(e) {
                 if (e === this.options.shape && this.shape) this.shape.setOptions(this.options, this.imageObj, this.imageObjAlt);
                 else switch (this.options.shape) {
                     case "box":
-                        this.shape = new So(this.options, this.body, this.labelModule);
+                        this.shape = new _a(this.options, this.body, this.labelModule);
                         break;
                     case "circle":
-                        this.shape = new Oo(this.options, this.body, this.labelModule);
+                        this.shape = new Ea(this.options, this.body, this.labelModule);
                         break;
                     case "circularImage":
-                        this.shape = new Io(this.options, this.body, this.labelModule, this.imageObj, this.imageObjAlt);
+                        this.shape = new So(this.options, this.body, this.labelModule, this.imageObj, this.imageObjAlt);
                         break;
                     case "custom":
-                        this.shape = new Po(this.options, this.body, this.labelModule, this.options.ctxRenderer);
+                        this.shape = new Oo(this.options, this.body, this.labelModule, this.options.ctxRenderer);
                         break;
                     case "database":
-                        this.shape = new Mo(this.options, this.body, this.labelModule);
+                        this.shape = new Io(this.options, this.body, this.labelModule);
                         break;
                     case "diamond":
-                        this.shape = new Do(this.options, this.body, this.labelModule);
+                        this.shape = new xa(this.options, this.body, this.labelModule);
                         break;
                     case "dot":
-                        this.shape = new Fo(this.options, this.body, this.labelModule);
+                        this.shape = new Po(this.options, this.body, this.labelModule);
                         break;
                     case "ellipse":
                         this.shape = new Mi(this.options, this.body, this.labelModule);
                         break;
                     case "icon":
-                        this.shape = new No(this.options, this.body, this.labelModule);
+                        this.shape = new Mo(this.options, this.body, this.labelModule);
                         break;
                     case "image":
-                        this.shape = new Bo(this.options, this.body, this.labelModule, this.imageObj, this.imageObjAlt);
+                        this.shape = new Ca(this.options, this.body, this.labelModule, this.imageObj, this.imageObjAlt);
                         break;
                     case "square":
-                        this.shape = new Ao(this.options, this.body, this.labelModule);
+                        this.shape = new Do(this.options, this.body, this.labelModule);
                         break;
                     case "hexagon":
-                        this.shape = new zo(this.options, this.body, this.labelModule);
+                        this.shape = new Fo(this.options, this.body, this.labelModule);
                         break;
                     case "star":
-                        this.shape = new Lo(this.options, this.body, this.labelModule);
+                        this.shape = new No(this.options, this.body, this.labelModule);
                         break;
                     case "text":
-                        this.shape = new Ro(this.options, this.body, this.labelModule);
+                        this.shape = new Bo(this.options, this.body, this.labelModule);
                         break;
                     case "triangle":
-                        this.shape = new Ho(this.options, this.body, this.labelModule);
+                        this.shape = new Ta(this.options, this.body, this.labelModule);
                         break;
                     case "triangleDown":
-                        this.shape = new jo(this.options, this.body, this.labelModule);
+                        this.shape = new Ao(this.options, this.body, this.labelModule);
                         break;
                     default:
                         this.shape = new Mi(this.options, this.body, this.labelModule);
                         break
                 }
                 this.needsRefresh()
             }
@@ -5906,15 +5906,15 @@
             static checkMass(e, t) {
                 if (e.mass !== void 0 && e.mass <= 0) {
                     let i = "";
                     t !== void 0 && (i = " in node id: " + t), console.error("%cNegative or zero mass disallowed" + i + ", setting mass to 1.", _i), e.mass = 1
                 }
             }
         },
-        Wo = class {
+        zo = class {
             constructor(e, t, i, s) {
                 if (this.body = e, this.images = t, this.groups = i, this.layoutEngine = s, this.body.functions.createNode = this.create.bind(this), this.nodesListeners = {
                         add: (o, r) => {
                             this.add(r.items)
                         },
                         update: (o, r) => {
                             this.update(r.items, r.data, r.oldData)
@@ -6215,26 +6215,26 @@
             }
             static drawPath(e, t) {
                 e.beginPath(), e.moveTo(t[0].x, t[0].y);
                 for (let i = 1; i < t.length; ++i) e.lineTo(t[i].x, t[i].y);
                 e.closePath()
             }
         },
-        Vo = class extends G {
+        ka = class extends G {
             static draw(e, t) {
                 if (t.image) {
                     e.save(), e.translate(t.point.x, t.point.y), e.rotate(Math.PI / 2 + t.angle);
                     let i = t.imageWidth != null ? t.imageWidth : t.image.width,
                         s = t.imageHeight != null ? t.imageHeight : t.image.height;
                     t.image.drawImageAtPosition(e, 1, -i / 2, 0, i, s), e.restore()
                 }
                 return !1
             }
         },
-        qo = class extends G {
+        Lo = class extends G {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: 0
                 }, {
                     x: -1,
                     y: .3
@@ -6244,15 +6244,15 @@
                 }, {
                     x: -1,
                     y: -.3
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        Uo = class {
+        Ro = class {
             static draw(e, t) {
                 let i = [{
                     x: -1,
                     y: 0
                 }, {
                     x: 0,
                     y: .3
@@ -6262,80 +6262,80 @@
                 }, {
                     x: 0,
                     y: -.3
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        Yo = class {
+        Ho = class {
             static draw(e, t) {
                 let i = {
                     x: -.4,
                     y: 0
                 };
                 G.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
                 let s = Math.PI,
                     o = t.angle - s / 2,
                     r = t.angle + s / 2;
                 return e.beginPath(), e.arc(i.x, i.y, t.length * .4, o, r, !1), e.stroke(), !0
             }
         },
-        Xo = class {
+        jo = class {
             static draw(e, t) {
                 let i = {
                     x: -.3,
                     y: 0
                 };
                 G.transform(i, t), e.strokeStyle = e.fillStyle, e.fillStyle = "rgba(0, 0, 0, 0)";
                 let s = Math.PI,
                     o = t.angle + s / 2,
                     r = t.angle + 3 * s / 2;
                 return e.beginPath(), e.arc(i.x, i.y, t.length * .4, o, r, !1), e.stroke(), !0
             }
         },
-        Go = class {
+        Wo = class {
             static draw(e, t) {
                 let i = [{
                     x: .02,
                     y: 0
                 }, {
                     x: -1,
                     y: .3
                 }, {
                     x: -1,
                     y: -.3
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        Ko = class {
+        Vo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .3
                 }, {
                     x: 0,
                     y: -.3
                 }, {
                     x: -1,
                     y: 0
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        Zo = class {
+        qo = class {
             static draw(e, t) {
                 let i = {
                     x: -.4,
                     y: 0
                 };
                 return G.transform(i, t), Ci(e, i.x, i.y, t.length * .4), !0
             }
         },
-        Qo = class {
+        Uo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .5
                 }, {
                     x: 0,
                     y: -.5
@@ -6345,15 +6345,15 @@
                 }, {
                     x: -.15,
                     y: .5
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        $o = class {
+        Yo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: .3
                 }, {
                     x: 0,
                     y: -.3
@@ -6363,15 +6363,15 @@
                 }, {
                     x: -.6,
                     y: .3
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        Jo = class {
+        Xo = class {
             static draw(e, t) {
                 let i = [{
                     x: 0,
                     y: 0
                 }, {
                     x: -.5,
                     y: -.3
@@ -6381,15 +6381,15 @@
                 }, {
                     x: -.5,
                     y: .3
                 }];
                 return G.transform(i, t), G.drawPath(e, i), !0
             }
         },
-        en = class {
+        Go = class {
             static draw(e, t) {
                 let i = [{
                     x: -1,
                     y: .3
                 }, {
                     x: -.5,
                     y: 0
@@ -6404,38 +6404,38 @@
             }
         },
         Di = class {
             static draw(e, t) {
                 let i;
                 switch (t.type && (i = t.type.toLowerCase()), i) {
                     case "image":
-                        return Vo.draw(e, t);
+                        return ka.draw(e, t);
                     case "circle":
-                        return Zo.draw(e, t);
+                        return qo.draw(e, t);
                     case "box":
-                        return $o.draw(e, t);
+                        return Yo.draw(e, t);
                     case "crow":
-                        return Uo.draw(e, t);
+                        return Ro.draw(e, t);
                     case "curve":
-                        return Yo.draw(e, t);
+                        return Ho.draw(e, t);
                     case "diamond":
-                        return Jo.draw(e, t);
-                    case "inv_curve":
                         return Xo.draw(e, t);
+                    case "inv_curve":
+                        return jo.draw(e, t);
                     case "triangle":
-                        return Go.draw(e, t);
+                        return Wo.draw(e, t);
                     case "inv_triangle":
-                        return Ko.draw(e, t);
+                        return Vo.draw(e, t);
                     case "bar":
-                        return Qo.draw(e, t);
+                        return Uo.draw(e, t);
                     case "vee":
-                        return en.draw(e, t);
+                        return Go.draw(e, t);
                     case "arrow":
                     default:
-                        return qo.draw(e, t)
+                        return Lo.draw(e, t)
                 }
             }
         },
         Fi = class {
             constructor(e, t, i) {
                 this._body = t, this._labelModule = i, this.color = {}, this.colorDirty = !0, this.hoverWidth = 1.5, this.selectionWidth = 2, this.setOptions(e), this.fromPoint = this.from, this.toPoint = this.to
             }
@@ -6885,15 +6885,15 @@
                     o = Math.pow(1 - i, 2) * this.fromPoint.y + 2 * i * (1 - i) * t.y + Math.pow(i, 2) * this.toPoint.y;
                 return {
                     x: s,
                     y: o
                 }
             }
         },
-        tn = class extends Kt {
+        Ko = class extends Kt {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _getDistanceToBezierEdge2(e, t, i, s, o, r, a, d) {
                 let h = 1e9,
                     l = e,
                     c = t,
@@ -6908,15 +6908,15 @@
                         h = g < h ? g : h
                     }
                     l = C, c = f
                 }
                 return h
             }
         },
-        Ai = class extends tn {
+        Ai = class extends Ko {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _line(e, t, i) {
                 let s = i[0],
                     o = i[1];
                 this._bezierCurve(e, t, s, o)
@@ -7214,15 +7214,15 @@
             remove() {
                 this.cleanup(), this.disconnect(), delete this.body.edges[this.id]
             }
             endPointsValid() {
                 return this.body.nodes[this.fromId] !== void 0 && this.body.nodes[this.toId] !== void 0
             }
         },
-        sn = class {
+        Zo = class {
             constructor(e, t, i) {
                 this.body = e, this.images = t, this.groups = i, this.body.functions.createEdge = this.create.bind(this), this.edgesListeners = {
                     add: (s, o) => {
                         this.add(o.items)
                     },
                     update: (s, o) => {
                         this.update(o.items)
@@ -7630,15 +7630,15 @@
             _debug(e, t) {
                 this.barnesHutTree !== void 0 && (e.lineWidth = 1, this._drawBranch(this.barnesHutTree.root, e, t))
             }
             _drawBranch(e, t, i) {
                 i === void 0 && (i = "#FF0000"), e.childrenCount === 4 && (this._drawBranch(e.children.NW, t), this._drawBranch(e.children.NE, t), this._drawBranch(e.children.SE, t), this._drawBranch(e.children.SW, t)), t.strokeStyle = i, t.beginPath(), t.moveTo(e.range.minX, e.range.minY), t.lineTo(e.range.maxX, e.range.minY), t.stroke(), t.beginPath(), t.moveTo(e.range.maxX, e.range.minY), t.lineTo(e.range.maxX, e.range.maxY), t.stroke(), t.beginPath(), t.moveTo(e.range.maxX, e.range.maxY), t.lineTo(e.range.minX, e.range.maxY), t.stroke(), t.beginPath(), t.moveTo(e.range.minX, e.range.maxY), t.lineTo(e.range.minX, e.range.minY), t.stroke()
             }
         },
-        on = class {
+        Qo = class {
             constructor(e, t, i) {
                 this._rng = yt("REPULSION SOLVER"), this.body = e, this.physicsBody = t, this.setOptions(i)
             }
             setOptions(e) {
                 this.options = e
             }
             solve() {
@@ -7650,15 +7650,15 @@
                     b = 4 / 3;
                 for (let C = 0; C < l.length - 1; C++) {
                     a = h[l[C]];
                     for (let f = C + 1; f < l.length; f++) d = h[l[f]], e = d.x - a.x, t = d.y - a.y, i = Math.sqrt(e * e + t * t), i === 0 && (i = .1 * this._rng(), e = i), i < 2 * u && (i < .5 * u ? r = 1 : r = p * i + b, r = r / i, s = e * r, o = t * r, c[a.id].x -= s, c[a.id].y -= o, c[d.id].x += s, c[d.id].y += o)
                 }
             }
         },
-        nn = class {
+        $o = class {
             constructor(e, t, i) {
                 this.body = e, this.physicsBody = t, this.setOptions(i)
             }
             setOptions(e) {
                 this.options = e, this.overlapAvoidanceFactor = Math.max(0, Math.min(1, this.options.avoidOverlap || 0))
             }
             solve() {
@@ -7705,15 +7705,15 @@
                     r = Math.max(Math.sqrt(s * s + o * o), .01),
                     a = this.options.springConstant * (i - r) / r,
                     d = s * a,
                     h = o * a;
                 this.physicsBody.forces[e.id] !== void 0 && (this.physicsBody.forces[e.id].x += d, this.physicsBody.forces[e.id].y += h), this.physicsBody.forces[t.id] !== void 0 && (this.physicsBody.forces[t.id].x -= d, this.physicsBody.forces[t.id].y -= h)
             }
         },
-        rn = class {
+        Jo = class {
             constructor(e, t, i) {
                 this.body = e, this.physicsBody = t, this.setOptions(i)
             }
             setOptions(e) {
                 this.options = e
             }
             solve() {
@@ -7764,41 +7764,41 @@
                 }
             }
             _calculateForces(e, t, i, s, o) {
                 let r = e === 0 ? 0 : this.options.centralGravity / e;
                 s[o.id].x = t * r, s[o.id].y = i * r
             }
         },
-        an = class extends Li {
+        en = class extends Li {
             constructor(e, t, i) {
                 super(e, t, i);
                 this._rng = yt("FORCE ATLAS 2 BASED REPULSION SOLVER")
             }
             _calculateForces(e, t, i, s, o) {
                 e === 0 && (e = .1 * this._rng(), t = e), this.overlapAvoidanceFactor < 1 && s.shape.radius && (e = Math.max(.1 + this.overlapAvoidanceFactor * s.shape.radius, e - s.shape.radius));
                 let r = s.edges.length + 1,
                     a = this.options.gravitationalConstant * o.mass * s.options.mass * r / Math.pow(e, 2),
                     d = t * a,
                     h = i * a;
                 this.physicsBody.forces[s.id].x += d, this.physicsBody.forces[s.id].y += h
             }
         },
-        dn = class extends Ct {
+        tn = class extends Ct {
             constructor(e, t, i) {
                 super(e, t, i)
             }
             _calculateForces(e, t, i, s, o) {
                 if (e > 0) {
                     let r = o.edges.length + 1,
                         a = this.options.centralGravity * r * o.options.mass;
                     s[o.id].x = t * a, s[o.id].y = i * a
                 }
             }
         },
-        hn = class {
+        sn = class {
             constructor(e) {
                 this.body = e, this.physicsBody = {
                     physicsNodeIndices: [],
                     physicsEdgeIndices: [],
                     forces: {},
                     velocities: {}
                 }, this.physicsEnabled = !0, this.simulationInterval = 1e3 / 60, this.requiresTimeout = !0, this.previousStates = {}, this.referenceState = {}, this.freezeCache = {}, this.renderTimer = void 0, this.adaptiveTimestep = !1, this.adaptiveTimestepEnabled = !1, this.adaptiveCounter = 0, this.adaptiveInterval = 3, this.stabilized = !1, this.startedStabilization = !1, this.stabilizationIterations = 0, this.ready = !1, this.options = {}, this.defaultOptions = {
@@ -7884,15 +7884,15 @@
                     let t = this.options.wind;
                     t && ((typeof t.x != "number" || Number.isNaN(t.x)) && (t.x = 0), (typeof t.y != "number" || Number.isNaN(t.y)) && (t.y = 0)), this.timestep = this.options.timestep
                 }
                 this.init()
             }
             init() {
                 let e;
-                this.options.solver === "forceAtlas2Based" ? (e = this.options.forceAtlas2Based, this.nodesSolver = new an(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new dn(this.body, this.physicsBody, e)) : this.options.solver === "repulsion" ? (e = this.options.repulsion, this.nodesSolver = new on(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)) : this.options.solver === "hierarchicalRepulsion" ? (e = this.options.hierarchicalRepulsion, this.nodesSolver = new nn(this.body, this.physicsBody, e), this.edgesSolver = new rn(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)) : (e = this.options.barnesHut, this.nodesSolver = new Li(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)), this.modelOptions = e
+                this.options.solver === "forceAtlas2Based" ? (e = this.options.forceAtlas2Based, this.nodesSolver = new en(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new tn(this.body, this.physicsBody, e)) : this.options.solver === "repulsion" ? (e = this.options.repulsion, this.nodesSolver = new Qo(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)) : this.options.solver === "hierarchicalRepulsion" ? (e = this.options.hierarchicalRepulsion, this.nodesSolver = new $o(this.body, this.physicsBody, e), this.edgesSolver = new Jo(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)) : (e = this.options.barnesHut, this.nodesSolver = new Li(this.body, this.physicsBody, e), this.edgesSolver = new Zt(this.body, this.physicsBody, e), this.gravitySolver = new Ct(this.body, this.physicsBody, e)), this.modelOptions = e
             }
             initPhysics() {
                 this.physicsEnabled === !0 && this.options.enabled === !0 ? this.options.stabilization.enabled === !0 ? this.stabilize() : (this.stabilized = !1, this.ready = !0, this.body.emitter.emit("fit", {}, this.layoutFailed), this.startSimulation()) : (this.ready = !0, this.body.emitter.emit("fit"))
             }
             startSimulation() {
                 this.physicsEnabled === !0 && this.options.enabled === !0 ? (this.stabilized = !1, this.adaptiveTimestep = !1, this.body.emitter.emit("_resizeNodes"), this.viewFunction === void 0 && (this.viewFunction = this.simulationStep.bind(this), this.body.emitter.on("initRedraw", this.viewFunction), this.body.emitter.emit("_startRendering"))) : this.body.emitter.emit("_redraw")
             }
@@ -8098,15 +8098,15 @@
                 }
             }
             static cloneOptions(e, t) {
                 let i = {};
                 return t === void 0 || t === "node" ? (j(i, e.options, !0), i.x = e.x, i.y = e.y, i.amountOfConnections = e.edges.length) : j(i, e.options, !0), i
             }
         },
-        ln = class extends U {
+        on = class extends U {
             constructor(e, t, i, s, o, r) {
                 super(e, t, i, s, o, r);
                 this.isCluster = !0, this.containedNodes = {}, this.containedEdges = {}
             }
             _openChildCluster(e) {
                 let t = this.body.nodes[e];
                 if (this.containedNodes[e] === void 0) throw new Error("node with id: " + e + " not in current cluster");
@@ -8123,15 +8123,15 @@
                         o !== -1 && (A(i.clusteringEdgeReplacingIds, r => {
                             s.clusteringEdgeReplacingIds.push(r), this.body.edges[r].edgeReplacedById = s.id
                         }), s.clusteringEdgeReplacingIds.splice(o, 1))
                     })
                 }), t.edges = []
             }
         },
-        cn = class {
+        nn = class {
             constructor(e) {
                 this.body = e, this.clusteredNodes = {}, this.clusteredEdges = {}, this.options = {}, this.defaultOptions = {}, Object.assign(this.options, this.defaultOptions), this.body.emitter.on("_resetData", () => {
                     this.clusteredNodes = {}, this.clusteredEdges = {}
                 })
             }
             clusterByHubsize(e, t) {
                 e === void 0 ? e = this._getHubSize() : typeof e == "object" && (t = this._checkOptions(e), e = this._getHubSize());
@@ -8299,15 +8299,15 @@
                         } if (r = i.processProperties(r, l, c), !r) throw new Error("The processProperties function does not return properties!")
                 }
                 r.id === void 0 && (r.id = "cluster:" + Ce());
                 let a = r.id;
                 r.label === void 0 && (r.label = "cluster");
                 let d;
                 r.x === void 0 && (d = this._getClusterPosition(e), r.x = d.x), r.y === void 0 && (d === void 0 && (d = this._getClusterPosition(e)), r.y = d.y), r.id = a;
-                let h = this.body.functions.createNode(r, ln);
+                let h = this.body.functions.createNode(r, on);
                 h.containedNodes = e, h.containedEdges = t, h.clusterEdgeProperties = i.clusterEdgeProperties, this.body.nodes[r.id] = h, this._clusterEdges(e, t, r, i.clusterEdgeProperties), r.id = void 0, s === !0 && this.body.emitter.emit("_dataChanged")
             }
             _backupEdgeOptions(e) {
                 this.clusteredEdges[e.id] === void 0 && (this.clusteredEdges[e.id] = {
                     physics: e.options.physics
                 })
             }
@@ -8618,15 +8618,15 @@
 
     function Sa() {
         let n;
         window !== void 0 && (n = window.requestAnimationFrame || window.mozRequestAnimationFrame || window.webkitRequestAnimationFrame || window.msRequestAnimationFrame), n === void 0 ? window.requestAnimationFrame = function(e) {
             e()
         } : window.requestAnimationFrame = n
     }
-    var un = class {
+    var rn = class {
         constructor(e, t) {
             Sa(), this.body = e, this.canvas = t, this.redrawRequested = !1, this.renderTimer = void 0, this.requiresTimeout = !0, this.renderingActive = !1, this.renderRequests = 0, this.allowRedraw = !0, this.dragging = !1, this.zooming = !1, this.options = {}, this.defaultOptions = {
                 hideEdgesOnDrag: !1,
                 hideEdgesOnZoom: !1,
                 hideNodesOnDrag: !1
             }, Object.assign(this.options, this.defaultOptions), this._determineBrowserMethod(), this.bindEventListeners()
         }
@@ -8789,20 +8789,20 @@
 
     function Qt(n, e) {
         e.inputHandler = function(t) {
             t.isFirst && e(t)
         }, n.on("hammer.input", e.inputHandler)
     }
 
-    function fn(n, e) {
+    function an(n, e) {
         return e.inputHandler = function(t) {
             t.isFinal && e(t)
         }, n.on("hammer.input", e.inputHandler)
     }
-    var pn = class {
+    var dn = class {
         constructor(e) {
             this.body = e, this.pixelRatio = 1, this.cameraState = {}, this.initialized = !1, this.canvasViewCenter = {}, this._cleanupCallbacks = [], this.options = {}, this.defaultOptions = {
                 autoResize: !0,
                 height: "100%",
                 width: "100%"
             }, Object.assign(this.options, this.defaultOptions), this.bindEventListeners()
         }
@@ -8918,15 +8918,15 @@
                 this.body.eventListeners.onPinch(e)
             }), this.frame.canvas.addEventListener("wheel", e => {
                 this.body.eventListeners.onMouseWheel(e)
             }), this.frame.canvas.addEventListener("mousemove", e => {
                 this.body.eventListeners.onMouseMove(e)
             }), this.frame.canvas.addEventListener("contextmenu", e => {
                 this.body.eventListeners.onContext(e)
-            }), this.hammerFrame = new Ue(this.frame), fn(this.hammerFrame, e => {
+            }), this.hammerFrame = new Ue(this.frame), an(this.hammerFrame, e => {
                 this.body.eventListeners.onRelease(e)
             })
         }
         setSize(e = this.options.width, t = this.options.height) {
             e = this._prepareValue(e), t = this._prepareValue(t);
             let i = !1,
                 s = this.frame.canvas.width,
@@ -9000,15 +9000,15 @@
             maxZoomLevel: 1
         }, n != null ? n : {});
         if (!Array.isArray(t.nodes)) throw new TypeError("Nodes has to be an array of ids.");
         if (t.nodes.length === 0 && (t.nodes = e), !(typeof t.minZoomLevel == "number" && t.minZoomLevel > 0)) throw new TypeError("Min zoom level has to be a number higher than zero.");
         if (!(typeof t.maxZoomLevel == "number" && t.minZoomLevel <= t.maxZoomLevel)) throw new TypeError("Max zoom level has to be a number higher than min zoom level.");
         return t
     }
-    var gn = class {
+    var hn = class {
             constructor(e, t) {
                 this.body = e, this.canvas = t, this.animationSpeed = 1 / this.renderRefreshRate, this.animationEasingFunction = "easeInOutQuint", this.easingTime = 0, this.sourceScale = 0, this.targetScale = 0, this.sourceTranslation = 0, this.targetTranslation = 0, this.lockedOnNodeId = void 0, this.lockedOnNodeOffset = void 0, this.touchTime = 0, this.viewFunction = void 0, this.body.emitter.on("fit", this.fit.bind(this)), this.body.emitter.on("animationFinished", () => {
                     this.body.emitter.emit("_stopRendering")
                 }), this.body.emitter.on("unlockNode", this.releaseNode.bind(this))
             }
             setOptions(e = {}) {
                 this.options = e
@@ -9140,15 +9140,15 @@
             getViewPosition() {
                 return this.canvas.DOMtoCanvas({
                     x: .5 * this.canvas.frame.canvas.clientWidth,
                     y: .5 * this.canvas.frame.canvas.clientHeight
                 })
             }
         },
-        mn = class {
+        ln = class {
             constructor(e, t) {
                 this.body = e, this.canvas = t, this.iconsCreated = !1, this.navigationHammers = [], this.boundFunctions = {}, this.touchTime = 0, this.activated = !1, this.body.emitter.on("activate", () => {
                     this.activated = !0, this.configureKeyboardBindings()
                 }), this.body.emitter.on("deactivate", () => {
                     this.activated = !1, this.configureKeyboardBindings()
                 }), this.body.emitter.on("destroy", () => {
                     this.keycharm !== void 0 && this.keycharm.destroy()
@@ -9174,15 +9174,15 @@
                 this.navigationDOM.wrapper = document.createElement("div"), this.navigationDOM.wrapper.className = "vis-navigation", this.canvas.frame.appendChild(this.navigationDOM.wrapper);
                 for (let s = 0; s < e.length; s++) {
                     this.navigationDOM[e[s]] = document.createElement("div"), this.navigationDOM[e[s]].className = "vis-button vis-" + e[s], this.navigationDOM.wrapper.appendChild(this.navigationDOM[e[s]]);
                     let o = new Ue(this.navigationDOM[e[s]]);
                     t[s] === "_fit" ? Qt(o, this._fit.bind(this)) : Qt(o, this.bindToRedraw.bind(this, t[s])), this.navigationHammers.push(o)
                 }
                 let i = new Ue(this.canvas.frame);
-                fn(i, () => {
+                an(i, () => {
                     this._stopMovement()
                 }), this.navigationHammers.push(i), this.iconsCreated = !0
             }
             bindToRedraw(e) {
                 this.boundFunctions[e] === void 0 && (this.boundFunctions[e] = this[e].bind(this), this.body.emitter.on("initRedraw", this.boundFunctions[e]), this.body.emitter.emit("_startRendering"))
             }
             unbindFromRedraw(e) {
@@ -9295,17 +9295,17 @@
                 }, "keyup"), this.keycharm.bind("pageup", () => {
                     this.unbindFromRedraw("_zoomIn")
                 }, "keyup"), this.keycharm.bind("pagedown", () => {
                     this.unbindFromRedraw("_zoomOut")
                 }, "keyup")))
             }
         },
-        yn = class {
+        cn = class {
             constructor(e, t, i) {
-                this.body = e, this.canvas = t, this.selectionHandler = i, this.navigationHandler = new mn(e, t), this.body.eventListeners.onTap = this.onTap.bind(this), this.body.eventListeners.onTouch = this.onTouch.bind(this), this.body.eventListeners.onDoubleTap = this.onDoubleTap.bind(this), this.body.eventListeners.onHold = this.onHold.bind(this), this.body.eventListeners.onDragStart = this.onDragStart.bind(this), this.body.eventListeners.onDrag = this.onDrag.bind(this), this.body.eventListeners.onDragEnd = this.onDragEnd.bind(this), this.body.eventListeners.onMouseWheel = this.onMouseWheel.bind(this), this.body.eventListeners.onPinch = this.onPinch.bind(this), this.body.eventListeners.onMouseMove = this.onMouseMove.bind(this), this.body.eventListeners.onRelease = this.onRelease.bind(this), this.body.eventListeners.onContext = this.onContext.bind(this), this.touchTime = 0, this.drag = {}, this.pinch = {}, this.popup = void 0, this.popupObj = void 0, this.popupTimer = void 0, this.body.functions.getPointer = this.getPointer.bind(this), this.options = {}, this.defaultOptions = {
+                this.body = e, this.canvas = t, this.selectionHandler = i, this.navigationHandler = new ln(e, t), this.body.eventListeners.onTap = this.onTap.bind(this), this.body.eventListeners.onTouch = this.onTouch.bind(this), this.body.eventListeners.onDoubleTap = this.onDoubleTap.bind(this), this.body.eventListeners.onHold = this.onHold.bind(this), this.body.eventListeners.onDragStart = this.onDragStart.bind(this), this.body.eventListeners.onDrag = this.onDrag.bind(this), this.body.eventListeners.onDragEnd = this.onDragEnd.bind(this), this.body.eventListeners.onMouseWheel = this.onMouseWheel.bind(this), this.body.eventListeners.onPinch = this.onPinch.bind(this), this.body.eventListeners.onMouseMove = this.onMouseMove.bind(this), this.body.eventListeners.onRelease = this.onRelease.bind(this), this.body.eventListeners.onContext = this.onContext.bind(this), this.touchTime = 0, this.drag = {}, this.pinch = {}, this.popup = void 0, this.popupObj = void 0, this.popupTimer = void 0, this.body.functions.getPointer = this.getPointer.bind(this), this.options = {}, this.defaultOptions = {
                     dragNodes: !0,
                     dragView: !0,
                     hover: !1,
                     keyboard: {
                         enabled: !1,
                         speed: {
                             x: 10,
@@ -9392,16 +9392,15 @@
                     this.body.selectionBox.position.start = {
                         x: this.canvas._XconvertDOMtoCanvas(i.x),
                         y: this.canvas._YconvertDOMtoCanvas(i.y)
                     }, this.body.selectionBox.position.end = {
                         x: this.canvas._XconvertDOMtoCanvas(i.x),
                         y: this.canvas._YconvertDOMtoCanvas(i.y)
                     }
-                }
-                if (t !== void 0 && this.options.dragNodes === !0) {
+                } else if (t !== void 0 && this.options.dragNodes === !0) {
                     this.drag.nodeId = t.id, t.isSelected() === !1 && this.selectionHandler.setSelection({
                         nodes: [t.id]
                     }), this.selectionHandler.generateClickEvent("dragStart", e, this.drag.pointer);
                     for (let i of this.selectionHandler.getSelectedNodes()) {
                         let s = {
                             id: i.id,
                             node: i,
@@ -9582,15 +9581,15 @@
         if (i === "m") throw new TypeError("Private method is not writable");
         if (i === "a" && !s) throw new TypeError("Private accessor was defined without a setter");
         if (typeof e == "function" ? n !== e || !s : !e.has(n)) throw new TypeError("Cannot write private member to an object whose class did not declare it");
         return i === "a" ? s.call(n, t) : s ? s.value = t : e.set(n, t), t
     }
     var Xe, ce, Fe, Ne, $t;
 
-    function bn(n, e) {
+    function un(n, e) {
         let t = new Set;
         for (let i of e) n.has(i) || t.add(i);
         return t
     }
     var Hi = class {
         constructor() {
             Xe.set(this, new Set), ce.set(this, new Set)
@@ -9608,30 +9607,30 @@
             q(this, ce, "f").clear()
         }
         getSelection() {
             return [...q(this, ce, "f")]
         }
         getChanges() {
             return {
-                added: [...bn(q(this, Xe, "f"), q(this, ce, "f"))],
-                deleted: [...bn(q(this, ce, "f"), q(this, Xe, "f"))],
+                added: [...un(q(this, Xe, "f"), q(this, ce, "f"))],
+                deleted: [...un(q(this, ce, "f"), q(this, Xe, "f"))],
                 previous: [...new Set(q(this, Xe, "f"))],
                 current: [...new Set(q(this, ce, "f"))]
             }
         }
         commit() {
             let e = this.getChanges();
             Ri(this, Xe, q(this, ce, "f"), "f"), Ri(this, ce, new Set(q(this, Xe, "f")), "f");
             for (let t of e.added) t.select();
             for (let t of e.deleted) t.unselect();
             return e
         }
     };
     Xe = new WeakMap, ce = new WeakMap;
-    var vn = class {
+    var fn = class {
         constructor(e = () => {}) {
             Fe.set(this, new Hi), Ne.set(this, new Hi), $t.set(this, void 0), Ri(this, $t, e, "f")
         }
         get sizeNodes() {
             return q(this, Fe, "f").size
         }
         get sizeEdges() {
@@ -9663,17 +9662,17 @@
                 nodes: q(this, Fe, "f").commit(),
                 edges: q(this, Ne, "f").commit()
             };
             return q(this, $t, "f").call(this, t, ...e), t
         }
     };
     Fe = new WeakMap, Ne = new WeakMap, $t = new WeakMap;
-    var wn = class {
+    var pn = class {
             constructor(e, t) {
-                this.body = e, this.canvas = t, this._selectionAccumulator = new vn, this.hoverObj = {
+                this.body = e, this.canvas = t, this._selectionAccumulator = new fn, this.hoverObj = {
                     nodes: {},
                     edges: {}
                 }, this.options = {}, this.defaultOptions = {
                     multiselect: !1,
                     selectable: !0,
                     selectConnectedEdges: !0,
                     hoverConnectedEdges: !0
@@ -9928,15 +9927,15 @@
             fix(e, t) {
                 this.fake_use(e, t), this.abstract()
             }
             shift(e, t) {
                 this.fake_use(e, t), this.abstract()
             }
         },
-        _n = class extends ji {
+        gn = class extends ji {
             constructor(e) {
                 super();
                 this.layout = e
             }
             curveType() {
                 return "horizontal"
             }
@@ -9961,15 +9960,15 @@
             fix(e, t) {
                 e.y = this.layout.options.hierarchical.levelSeparation * t, e.options.fixed.y = !0
             }
             shift(e, t) {
                 this.layout.body.nodes[e].x += t
             }
         },
-        En = class extends ji {
+        mn = class extends ji {
             constructor(e) {
                 super();
                 this.layout = e
             }
             curveType() {
                 return "vertical"
             }
@@ -10009,22 +10008,22 @@
             let s = i.from.id,
                 o = i.to.id;
             e[s] == null && (e[s] = 0), (e[o] == null || e[s] >= e[o]) && (e[o] = e[s] + 1)
         }), e
     }
 
     function Pa(n) {
-        return xn(e => e.edges.filter(t => n.has(t.toId)).every(t => t.to === e), (e, t) => t > e, "from", n)
+        return yn(e => e.edges.filter(t => n.has(t.toId)).every(t => t.to === e), (e, t) => t > e, "from", n)
     }
 
     function Ma(n) {
-        return xn(e => e.edges.filter(t => n.has(t.toId)).every(t => t.from === e), (e, t) => t < e, "to", n)
+        return yn(e => e.edges.filter(t => n.has(t.toId)).every(t => t.from === e), (e, t) => t < e, "to", n)
     }
 
-    function xn(n, e, t, i) {
+    function yn(n, e, t, i) {
         let s = Object.create(null),
             o = [...i.values()].reduce((d, h) => d + 1 + h.edges.length, 0),
             r = t + "Id",
             a = t === "to" ? 1 : -1;
         for (let [d, h] of i) {
             if (!i.has(d) || !n(h)) continue;
             s[d] = 0;
@@ -10040,15 +10039,15 @@
                         (f == null || e(p, f)) && (s[C] = p, l.push(b[t]))
                     }), c > o) return Ia(i, s);
                 ++c
             }
         }
         return s
     }
-    var Cn = class {
+    var bn = class {
             constructor() {
                 this.childrenReference = {}, this.parentReference = {}, this.trees = {}, this.distributionOrdering = {}, this.levels = {}, this.distributionIndex = {}, this.isTree = !1, this.treeIndex = -1
             }
             addRelation(e, t) {
                 this.childrenReference[e] === void 0 && (this.childrenReference[e] = []), this.childrenReference[e].push(t), this.parentReference[t] === void 0 && (this.parentReference[t] = []), this.parentReference[t].push(e)
             }
             checkIfTree() {
@@ -10127,15 +10126,15 @@
                 for (let o in s)
                     if (s[o] === e) {
                         i = !0;
                         break
                     } i || (this.distributionOrdering[t].push(e), this.distributionIndex[e.id] = this.distributionOrdering[t].length - 1)
             }
         },
-        Tn = class {
+        vn = class {
             constructor(e) {
                 this.body = e, this._resetRNG(Math.random() + ":" + Date.now()), this.setPhysics = !1, this.options = {}, this.optionsBackup = {
                     physics: {}
                 }, this.defaultOptions = {
                     randomSeed: void 0,
                     improvedLayout: !0,
                     clusterThreshold: 150,
@@ -10311,15 +10310,15 @@
             getSeed() {
                 return this.initialRandomSeed
             }
             setupHierarchicalLayout() {
                 if (this.options.hierarchical.enabled === !0 && this.body.nodeIndices.length > 0) {
                     let e, t, i = !1,
                         s = !1;
-                    this.lastNodeOnLevel = {}, this.hierarchical = new Cn;
+                    this.lastNodeOnLevel = {}, this.hierarchical = new bn;
                     for (t in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, t) && (e = this.body.nodes[t], e.options.level !== void 0 ? (i = !0, this.hierarchical.levels[t] = e.options.level) : s = !0);
                     if (s === !0 && i === !0) throw new Error("To use the hierarchical layout, nodes require either no predefined levels or levels have to be defined for all nodes."); {
                         if (s === !0) {
                             let r = this.options.hierarchical.sortMethod;
                             r === "hubsize" ? this._determineLevelsByHubsize() : r === "directed" ? this._determineLevelsDirected() : r === "custom" && this._determineLevelsCustomCallback()
                         }
                         for (let r in this.body.nodes) Object.prototype.hasOwnProperty.call(this.body.nodes, r) && this.hierarchical.ensureLevel(r);
@@ -10438,16 +10437,16 @@
                             N = (B, F) => {
                                 let D = this.direction.getPosition(g),
                                     H = {};
                                 for (let Y = 0; Y < B; Y++) {
                                     let ue = w(D, F),
                                         Ke = k(D, F),
                                         ot = 40,
-                                        Nn = Math.max(-ot, Math.min(ot, Math.round(ue / Ke)));
-                                    if (D = D - Nn, H[D] !== void 0) break;
+                                        On = Math.max(-ot, Math.min(ot, Math.round(ue / Ke)));
+                                    if (D = D - On, H[D] !== void 0) break;
                                     H[D] = Y
                                 }
                                 return D
                             },
                             W = B => {
                                 let F = this.direction.getPosition(g);
                                 if (t[g.id] === void 0) {
@@ -10733,15 +10732,15 @@
                             foundParent: null,
                             withChild: a
                         }
                     };
                 return s(i, e), o(i, t)
             }
             setDirectionStrategy() {
-                this.options.hierarchical.direction === "UD" || this.options.hierarchical.direction === "DU" ? this.direction = new _n(this) : this.direction = new En(this)
+                this.options.hierarchical.direction === "UD" || this.options.hierarchical.direction === "DU" ? this.direction = new gn(this) : this.direction = new mn(this)
             }
             _getCenterPosition(e) {
                 let t = 1e9,
                     i = -1e9;
                 for (let s = 0; s < e.length; s++) {
                     let o;
                     if (e[s].id !== void 0) o = e[s];
@@ -10751,15 +10750,15 @@
                     }
                     let r = this.direction.getPosition(o);
                     t = Math.min(t, r), i = Math.max(i, r)
                 }
                 return .5 * (t + i)
             }
         },
-        kn = class {
+        wn = class {
             constructor(e, t, i, s) {
                 this.body = e, this.canvas = t, this.selectionHandler = i, this.interactionHandler = s, this.editMode = !1, this.manipulationDiv = void 0, this.editModeDiv = void 0, this.closeDiv = void 0, this._domEventListenerCleanupQueue = [], this.temporaryUIFunctions = {}, this.temporaryEventFunctions = [], this.touchTime = 0, this.temporaryIds = {
                     nodes: [],
                     edges: []
                 }, this.guiEnabled = !1, this.inMode = !1, this.selectedControlNode = void 0, this.options = {}, this.defaultOptions = {
                     enabled: !1,
                     initiallyActive: !1,
@@ -11155,15 +11154,15 @@
             }
         },
         O = "string",
         S = "boolean",
         y = "number",
         Tt = "array",
         P = "object",
-        Sn = "dom",
+        _n = "dom",
         Da = "any",
         Wi = ["arrow", "bar", "box", "circle", "crow", "curve", "diamond", "image", "inv_curve", "inv_triangle", "triangle", "vee"],
         Vi = {
             borderWidth: {
                 number: y
             },
             borderWidthSelected: {
@@ -11558,15 +11557,15 @@
                 }
             },
             size: {
                 number: y
             },
             title: {
                 string: O,
-                dom: Sn,
+                dom: _n,
                 undefined: "undefined"
             },
             value: {
                 number: y,
                 undefined: "undefined"
             },
             widthConstraint: {
@@ -11600,15 +11599,15 @@
                 filter: {
                     boolean: S,
                     string: O,
                     array: Tt,
                     function: "function"
                 },
                 container: {
-                    dom: Sn
+                    dom: _n
                 },
                 showButton: {
                     boolean: S
                 },
                 __type__: {
                     object: P,
                     boolean: S,
@@ -12384,15 +12383,15 @@
             width: {
                 string: O
             },
             __type__: {
                 object: P
             }
         },
-        On = {
+        En = {
             nodes: {
                 borderWidth: [1, 0, 10, 1],
                 borderWidthSelected: [2, 0, 10, 1],
                 color: {
                     border: ["color", "#2B7CE9"],
                     background: ["color", "#97C2FC"],
                     highlight: {
@@ -12609,16 +12608,16 @@
                 timestep: [.5, .01, 1, .01],
                 wind: {
                     x: [0, -10, 10, .1],
                     y: [0, -10, 10, .1]
                 }
             }
         },
-        Na = (n, e, t) => !!(n.includes("physics") && On.physics.solver.includes(e) && t.physics.solver !== e && e !== "wind");
-    var In = class {
+        Na = (n, e, t) => !!(n.includes("physics") && En.physics.solver.includes(e) && t.physics.solver !== e && e !== "wind");
+    var xn = class {
             constructor() {}
             getDistances(e, t, i) {
                 let s = {},
                     o = e.edges;
                 for (let a = 0; a < t.length; a++) {
                     let d = t[a],
                         h = {};
@@ -12643,17 +12642,17 @@
                             u[b] = f, C[c] = f
                         }
                     }
                 }
                 return s
             }
         },
-        Pn = class {
+        Cn = class {
             constructor(e, t, i) {
-                this.body = e, this.springLength = t, this.springConstant = i, this.distanceSolver = new In
+                this.body = e, this.springLength = t, this.springConstant = i, this.distanceSolver = new xn
             }
             setOptions(e) {
                 e && (e.springLength && (this.springLength = e.springLength), e.springConstant && (this.springConstant = e.springConstant))
             }
             solve(e, t, i = !1) {
                 let s = this.distanceSolver.getDistances(this.body, e, t);
                 this._createL_matrix(s), this._createK_matrix(s), this._createE_matrix();
@@ -12792,15 +12791,15 @@
             }
         };
 
     function I(n, e, t) {
         if (!(this instanceof I)) throw new SyntaxError("Constructor must be called with the new operator");
         this.options = {}, this.defaultOptions = {
             locale: "en",
-            locales: Ca,
+            locales: ba,
             clickToUse: !1
         }, Object.assign(this.options, this.defaultOptions), this.body = {
             container: n,
             nodes: {},
             nodeIndices: [],
             edges: {},
             edgeIndices: [],
@@ -12850,19 +12849,19 @@
                     },
                     end: {
                         x: 0,
                         y: 0
                     }
                 }
             }
-        }, this.bindEventListeners(), this.images = new Eo(() => this.body.emitter.emit("_requestRedraw")), this.groups = new xo, this.canvas = new pn(this.body), this.selectionHandler = new wn(this.body, this.canvas), this.interactionHandler = new yn(this.body, this.canvas, this.selectionHandler), this.view = new gn(this.body, this.canvas), this.renderer = new un(this.body, this.canvas), this.physics = new hn(this.body), this.layoutEngine = new Tn(this.body), this.clustering = new cn(this.body), this.manipulation = new kn(this.body, this.canvas, this.selectionHandler, this.interactionHandler), this.nodesHandler = new Wo(this.body, this.images, this.groups, this.layoutEngine), this.edgesHandler = new sn(this.body, this.images, this.groups), this.body.modules.kamadaKawai = new Pn(this.body, 150, .05), this.body.modules.clustering = this.clustering, this.canvas._create(), this.setOptions(t), this.setData(e)
+        }, this.bindEventListeners(), this.images = new Eo(() => this.body.emitter.emit("_requestRedraw")), this.groups = new xo, this.canvas = new dn(this.body), this.selectionHandler = new pn(this.body, this.canvas), this.interactionHandler = new cn(this.body, this.canvas, this.selectionHandler), this.view = new hn(this.body, this.canvas), this.renderer = new rn(this.body, this.canvas), this.physics = new sn(this.body), this.layoutEngine = new vn(this.body), this.clustering = new nn(this.body), this.manipulation = new wn(this.body, this.canvas, this.selectionHandler, this.interactionHandler), this.nodesHandler = new zo(this.body, this.images, this.groups, this.layoutEngine), this.edgesHandler = new Zo(this.body, this.images, this.groups), this.body.modules.kamadaKawai = new Cn(this.body, 150, .05), this.body.modules.clustering = this.clustering, this.canvas._create(), this.setOptions(t), this.setData(e)
     }(0, no.default)(I.prototype);
     I.prototype.setOptions = function(n) {
         if (n === null && (n = void 0), n !== void 0) {
-            if (Qs.validate(n, Fa) === !0 && console.error("%cErrors have been found in the supplied options object.", _i), qe(["locale", "locales", "clickToUse"], this.options, n), n.locale !== void 0 && (n.locale = Ta(n.locales || this.options.locales, n.locale)), n = this.layoutEngine.setOptions(n.layout, n), this.canvas.setOptions(n), this.groups.setOptions(n.groups), this.nodesHandler.setOptions(n.nodes), this.edgesHandler.setOptions(n.edges), this.physics.setOptions(n.physics), this.manipulation.setOptions(n.manipulation, n, this.options), this.interactionHandler.setOptions(n.interaction), this.renderer.setOptions(n.interaction), this.selectionHandler.setOptions(n.interaction), n.groups !== void 0 && this.body.emitter.emit("refreshNodes"), "configure" in n && (this.configurator || (this.configurator = new Ks(this, this.body.container, On, this.canvas.pixelRatio, Na)), this.configurator.setOptions(n.configure)), this.configurator && this.configurator.options.enabled === !0) {
+            if (Qs.validate(n, Fa) === !0 && console.error("%cErrors have been found in the supplied options object.", _i), qe(["locale", "locales", "clickToUse"], this.options, n), n.locale !== void 0 && (n.locale = va(n.locales || this.options.locales, n.locale)), n = this.layoutEngine.setOptions(n.layout, n), this.canvas.setOptions(n), this.groups.setOptions(n.groups), this.nodesHandler.setOptions(n.nodes), this.edgesHandler.setOptions(n.edges), this.physics.setOptions(n.physics), this.manipulation.setOptions(n.manipulation, n, this.options), this.interactionHandler.setOptions(n.interaction), this.renderer.setOptions(n.interaction), this.selectionHandler.setOptions(n.interaction), n.groups !== void 0 && this.body.emitter.emit("refreshNodes"), "configure" in n && (this.configurator || (this.configurator = new Ks(this, this.body.container, En, this.canvas.pixelRatio, Na)), this.configurator.setOptions(n.configure)), this.configurator && this.configurator.options.enabled === !0) {
                 let i = {
                     nodes: {},
                     edges: {},
                     layout: {},
                     interaction: {},
                     manipulation: {},
                     physics: {},
@@ -12896,20 +12895,20 @@
             this.clustering._updateState(), this._updateVisibleIndices(), this._updateValueRange(this.body.nodes), this._updateValueRange(this.body.edges), this.body.emitter.emit("startSimulation"), this.body.emitter.emit("_requestRedraw")
         })
     };
     I.prototype.setData = function(n) {
         if (this.body.emitter.emit("resetPhysics"), this.body.emitter.emit("_resetData"), this.selectionHandler.unselectAll(), n && n.dot && (n.nodes || n.edges)) throw new SyntaxError('Data must contain either parameter "dot" or  parameter pair "nodes" and "edges", but not both.');
         if (this.setOptions(n && n.options), n && n.dot) {
             console.warn("The dot property has been deprecated. Please use the static convertDot method to convert DOT into vis.network format and use the normal data format with nodes and edges. This converter is used like this: var data = vis.network.convertDot(dotString);");
-            let e = ca(n.dot);
+            let e = na(n.dot);
             this.setData(e);
             return
         } else if (n && n.gephi) {
             console.warn("The gephi property has been deprecated. Please use the static convertGephi method to convert gephi into vis.network format and use the normal data format with nodes and edges. This converter is used like this: var data = vis.network.convertGephi(gephiJson);");
-            let e = ua(n.gephi);
+            let e = ra(n.gephi);
             this.setData(e);
             return
         } else this.nodesHandler.setData(n && n.nodes, !0), this.edgesHandler.setData(n && n.edges, !0);
         this.body.emitter.emit("_dataChanged"), this.body.emitter.emit("_dataLoaded"), this.body.emitter.emit("initPhysics")
     };
     I.prototype.destroy = function() {
         this.body.emitter.emit("destroy"), this.body.emitter.off(), this.off(), delete this.groups, delete this.canvas, delete this.selectionHandler, delete this.interactionHandler, delete this.view, delete this.renderer, delete this.physics, delete this.layoutEngine, delete this.clustering, delete this.manipulation, delete this.nodesHandler, delete this.edgesHandler, delete this.configurator, delete this.images;
@@ -13084,15 +13083,15 @@
     I.prototype.releaseNode = function() {
         return this.view.releaseNode.apply(this.view, arguments)
     };
     I.prototype.getOptionsFromConfigurator = function() {
         let n = {};
         return this.configurator && (n = this.configurator.getOptions.apply(this.configurator)), n
     };
-    var Mn = n => {
+    var Tn = n => {
         if (!document.cookie) return;
         let e = null,
             t = document.cookie.split(";");
         for (let i = 0; i < t.length; i++) {
             let s = t[i].trim();
             if (s.substring(0, n.length + 1) === n + "=") {
                 e = decodeURIComponent(s.substring(n.length + 1));
@@ -13127,36 +13126,36 @@
                     enabled: !0
                 }
             },
             physics: {
                 solver: "forceAtlas2Based"
             }
         },
-        Ba = Mn("csrftoken"),
+        Ba = Tn("csrftoken"),
         Ge = null,
-        Dn = document.querySelector("#visgraph"),
-        Fn = document.querySelector("#id_save_coords");
+        kn = document.querySelector("#visgraph"),
+        Sn = document.querySelector("#id_save_coords");
     (function() {
         if (!topologyData) return;
 
         function e(s) {
             let o = document.createElement("div");
             return o.innerHTML = s, o
         }
         let t = new Te(topologyData.nodes.map(s => Be(de({}, s), {
                 title: e(s.title)
             }))),
             i = new Te(topologyData.edges.map(s => Be(de({}, s), {
                 title: e(s.title)
             })));
-        Ge = new I(Dn, {
+        Ge = new I(kn, {
             nodes: t,
             edges: i
         }, qi), Ge.fit(), Ge.on("dragEnd", s => {
-            Fn != null && (!Fn.checked || Promise.allSettled(Object.entries(Ge.getPositions(s.nodes)).map(a => Xi(this, [a], function*([o, r]) {
+            Sn != null && (!Sn.checked || Promise.allSettled(Object.entries(Ge.getPositions(s.nodes)).map(a => Xi(this, [a], function*([o, r]) {
                 let d = yield fetch("/api/plugins/netbox_topology_views/save-coords/save_coords/", {
                     method: "PATCH",
                     headers: {
                         "X-CSRFToken": Ba,
                         Accept: "application/json",
                         "Content-Type": "application/json"
                     },
@@ -13179,15 +13178,15 @@
     var Aa = "image/png",
         za = document.querySelector("#btnDownloadImage");
     za.addEventListener("click", n => {
         La()
     });
 
     function La() {
-        let n = Dn.querySelector("canvas"),
+        let n = kn.querySelector("canvas"),
             e = document.createElement("a"),
             t = n.toDataURL(Aa);
         e.href = t, e.download = "topology", document.body.appendChild(e), e.click(), document.body.removeChild(e)
     }
     var Ra = new MutationObserver(n => n.forEach(e => {
         if (!Ge || e.type !== "attributes" || e.attributeName !== "data-netbox-color-mode" || !(e.target instanceof HTMLElement)) return;
         let {
@@ -13196,42 +13195,28 @@
         qi.nodes.font.color = t === "dark" ? "#fff" : "#000", Ge.setOptions(qi)
     }));
     Ra.observe(document.documentElement, {
         attributes: !0,
         attributeFilter: ["data-netbox-color-mode"]
     });
 })();
-/*! *****************************************************************************
-Copyright (c) Microsoft Corporation.
-
-Permission to use, copy, modify, and/or distribute this software for any
-purpose with or without fee is hereby granted.
-
-THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
-AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
-INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
-LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
-OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
-PERFORMANCE OF THIS SOFTWARE.
-***************************************************************************** */
 /*! Hammer.JS - v2.0.17-rc - 2019-12-16
  * http://naver.github.io/egjs
  *
  * Forked By Naver egjs
  * Copyright (c) hammerjs
  * Licensed under the MIT license */
 /**
  * vis-data
  * http://visjs.org/
  *
  * Manage unstructured data using DataSet. Add, update, and remove data, and listen for changes in the data.
  *
- * @version 7.1.4
- * @date    2022-03-15T15:23:59.245Z
+ * @version 7.1.6
+ * @date    2023-03-22T11:39:37.256Z
  *
  * @copyright (c) 2011-2017 Almende B.V, http://almende.com
  * @copyright (c) 2017-2019 visjs contributors, https://github.com/visjs
  *
  * @license
  * vis.js is dual licensed under both
  *
@@ -13247,16 +13232,16 @@
  */
 /**
  * vis-network
  * https://visjs.github.io/vis-network/
  *
  * A dynamic, browser-based visualization library.
  *
- * @version 9.1.2
- * @date    2022-03-28T20:13:51.046Z
+ * @version 9.1.6
+ * @date    2023-03-23T21:31:19.223Z
  *
  * @copyright (c) 2011-2017 Almende B.V, http://almende.com
  * @copyright (c) 2017-2019 visjs contributors, https://github.com/visjs
  *
  * @license
  * vis.js is dual licensed under both
  *
```

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/index.html` & `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/index.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/urls.py` & `netbox-topology-views-3.4.0/netbox_topology_views/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/utils.py` & `netbox-topology-views-3.4.0/netbox_topology_views/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views/views.py` & `netbox-topology-views-3.4.0/netbox_topology_views/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,35 +60,35 @@
 
 def create_node(
     device: Union[Device, Circuit, PowerPanel, PowerFeed], save_coords: bool
 ):
     node = {}
     node_content = ""
     if isinstance(device, Circuit):
-        dev_name = f"Circuit {device.cid}"
+        dev_name = device.cid
         node["id"] = f"c{device.pk}"
 
         if device.provider is not None:
             node_content += (
                 f"<tr><th>Provider: </th><td>{device.provider.name}</td></tr>"
             )
         if device.type is not None:
             node_content += f"<tr><th>Type: </th><td>{device.type.name}</td></tr>"
     elif isinstance(device, PowerPanel):
-        dev_name = f"Power Panel {device.pk}"
+        dev_name = device.name
         node["id"] = f"p{device.pk}"
 
         if device.site is not None:
             node_content += f"<tr><th>Site: </th><td>{device.site.name}</td></tr>"
         if device.location is not None:
             node_content += (
                 f"<tr><th>Location: </th><td>{device.location.name}</td></tr>"
             )
     elif isinstance(device, PowerFeed):
-        dev_name = f"Power Feed {device.pk}"
+        dev_name = device.name
         node["id"] = f"f{device.pk}"
 
         if device.power_panel is not None:
             node_content += (
                 f"<tr><th>Power Panel: </th><td>{device.power_panel.name}</td></tr>"
             )
         if device.type is not None:
@@ -100,15 +100,15 @@
         if device.amperage is not None:
             node_content += f"<tr><th>Amperage: </th><td>{device.amperage}</td></tr>"
         if device.voltage is not None:
             node_content += f"<tr><th>Voltage: </th><td>{device.voltage}</td></tr>"
     else:
         dev_name = device.name
         if dev_name is None:
-            dev_name = "device name unknown"
+            dev_name = device.device_type.get_full_name
 
         if device.device_type is not None:
             node_content += (
                 f"<tr><th>Type: </th><td>{device.device_type.model}</td></tr>"
             )
         if device.device_role.name is not None:
             node_content += (
@@ -212,15 +212,14 @@
         edge["dashes"] = [5, 5, 3, 3]
         title = "Power Connection"
 
     elif interface is not None:
         title = "Interface Connection"
         edge["width"] = 3
         edge["dashes"] = [1, 10, 1, 10]
-        edge["arrows"] = {"to": {"enabled": True, "scaleFactor": 0.5}, "from": {"enabled": True, "scaleFactor": 0.5}}
         edge["color"] = '#f1c232'
         edge["href"] = interface.get_absolute_url() + "trace"
         
     edge[
         "title"
     ] = f"{title} between<br>{cable_a_dev_name} [{cable_a_name}]<br>{cable_b_dev_name} [{cable_b_name}]"
 
@@ -803,8 +802,8 @@
         return render(
             request,
             "netbox_topology_views/individual_options.html",
             {
                 "form": form,
                 "object": queryset,
             },
-        )
+        )
```

### Comparing `netbox-topology-views-3.3.0/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.4.0/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.3.0
+Version: 3.4.0
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -57,14 +57,15 @@
 python3 manage.py collectstatic --no-input
 ```
 
 ### Versions
 
 | netbox version | netbox-topology-views version |
 | -------------- | ----------------------------- |
+| >= 3.5.0       | >= v3.4.X                     |
 | >= 3.4.0       | >= v3.X.X                     |
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
```

### Comparing `netbox-topology-views-3.3.0/setup.py` & `netbox-topology-views-3.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-topology-views",
-    version="3.3.0",
+    version="3.4.0",
     description="An NetBox plugin to create Topology maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattieserver/netbox-topology-views",
     author="Mattijs Vanhaverbeke",
     license="Apache 2.0",
     install_requires=[],
```

