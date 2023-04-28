# Comparing `tmp/vents-0.0.1.tar.gz` & `tmp/vents-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.0.1.tar", last modified: Fri Feb 10 13:10:06 2023, max compression
+gzip compressed data, was "vents-0.0.2.tar", last modified: Thu Apr 27 16:39:01 2023, max compression
```

## Comparing `vents-0.0.1.tar` & `vents-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,50 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-02-10 13:10:06.322650 vents-0.0.1/
--rw-r--r--   0 mourad     (501) staff       (20)      675 2023-02-10 13:10:06.322522 vents-0.0.1/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)       38 2023-02-10 13:10:06.322697 vents-0.0.1/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     1421 2023-02-10 13:10:03.000000 vents-0.0.1/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-02-10 13:10:06.322359 vents-0.0.1/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)      675 2023-02-10 13:10:06.000000 vents-0.0.1/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)      124 2023-02-10 13:10:06.000000 vents-0.0.1/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-02-10 13:10:06.000000 vents-0.0.1/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-02-10 13:10:06.000000 vents-0.0.1/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.265958 vents-0.0.2/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-27 16:30:14.000000 vents-0.0.2/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-27 16:39:01.266049 vents-0.0.2/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-27 16:39:01.266568 vents-0.0.2/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-27 16:32:25.000000 vents-0.0.2/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.260172 vents-0.0.2/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5095 2023-04-27 16:30:14.000000 vents-0.0.2/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.262034 vents-0.0.2/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      326 2023-04-27 16:30:14.000000 vents-0.0.2/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1897 2023-04-27 16:30:14.000000 vents-0.0.2/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-27 16:30:14.000000 vents-0.0.2/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-27 16:30:14.000000 vents-0.0.2/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-27 16:30:14.000000 vents-0.0.2/vents/connections/k8s_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-27 16:30:14.000000 vents-0.0.2/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.263702 vents-0.0.2/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-27 16:30:14.000000 vents-0.0.2/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-27 16:38:25.000000 vents-0.0.2/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.264216 vents-0.0.2/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.264722 vents-0.0.2/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5745 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     6695 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.265277 vents-0.0.2/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3517 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1084 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)      564 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.265806 vents-0.0.2/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4681 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2647 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-27 16:30:14.000000 vents-0.0.2/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-27 16:30:14.000000 vents-0.0.2/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-27 16:30:14.000000 vents-0.0.2/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-27 16:39:01.261099 vents-0.0.2/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-27 16:39:01.000000 vents-0.0.2/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1118 2023-04-27 16:39:01.000000 vents-0.0.2/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-27 16:39:01.000000 vents-0.0.2/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       12 2023-04-27 16:39:01.000000 vents-0.0.2/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-27 16:39:01.000000 vents-0.0.2/vents.egg-info/top_level.txt
```

