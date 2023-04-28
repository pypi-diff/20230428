# Comparing `tmp/arkitekt-0.4.91.tar.gz` & `tmp/arkitekt-0.4.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitekt-0.4.91.tar", max compression
+gzip compressed data, was "arkitekt-0.4.92.tar", max compression
```

## Comparing `arkitekt-0.4.91.tar` & `arkitekt-0.4.92.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.91/arkitekt/__init__.py
--rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.91/arkitekt/apps/__init__.py
--rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.91/arkitekt/apps/connected.py
--rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.91/arkitekt/apps/default.py
--rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/apps/fakts.py
--rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/apps/fluss.py
--rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/apps/herre.py
--rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.91/arkitekt/apps/mikro.py
--rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.91/arkitekt/apps/rekuest.py
--rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.91/arkitekt/apps/unlok.py
--rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.91/arkitekt/builders.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.91/arkitekt/cli/__init__.py
--rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.91/arkitekt/cli/build.py
--rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.91/arkitekt/cli/configs/introspect.yaml
--rw-r--r--   0        0        0    11054 2023-03-09 14:32:34.036965 arkitekt-0.4.91/arkitekt/cli/configs/latest.yaml
--rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.91/arkitekt/cli/configs/minimal.yaml
--rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.91/arkitekt/cli/deploy.py
--rw-r--r--   0        0        0     7187 2023-04-28 13:34:10.406830 arkitekt-0.4.91/arkitekt/cli/dev.py
--rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/cli/gen.py
--rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.91/arkitekt/cli/init.py
--rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.91/arkitekt/cli/inspect.py
--rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.91/arkitekt/cli/main.py
--rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.91/arkitekt/cli/run.py
--rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/cli/scan.py
--rw-r--r--   0        0        0    23235 2023-03-09 13:31:49.692385 arkitekt-0.4.91/arkitekt/cli/schemas/latest/fluss.schema.graphql
--rw-r--r--   0        0        0     5187 2023-03-09 13:31:49.692385 arkitekt-0.4.91/arkitekt/cli/schemas/latest/kuay.schema.graphql
--rw-r--r--   0        0        0   100011 2023-03-09 13:31:49.692385 arkitekt-0.4.91/arkitekt/cli/schemas/latest/mikro.schema.graphql
--rw-r--r--   0        0        0    50701 2023-03-09 13:31:49.692385 arkitekt-0.4.91/arkitekt/cli/schemas/latest/rekuest.schema.graphql
--rw-r--r--   0        0        0     8943 2023-03-09 13:31:49.696385 arkitekt-0.4.91/arkitekt/cli/schemas/latest/unlok.schema.graphql
--rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.91/arkitekt/cli/templates/simple.py
--rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.91/arkitekt/cli/types.py
--rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.91/arkitekt/cli/ui.py
--rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.91/arkitekt/cli/utils.py
--rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/deployers/port.py
--rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.91/arkitekt/healthz.py
--rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.91/arkitekt/qt/__init__.py
--rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.91/arkitekt/qt/assets/dark/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.91/arkitekt/qt/assets/dark/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.91/arkitekt/qt/assets/dark/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.91/arkitekt/qt/assets/dark/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.91/arkitekt/qt/assets/dark/red pulse.gif
--rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.91/arkitekt/qt/assets/light/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.91/arkitekt/qt/assets/light/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.91/arkitekt/qt/assets/light/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.91/arkitekt/qt/assets/light/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.91/arkitekt/qt/assets/light/red pulse.gif
--rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.91/arkitekt/qt/magic_bar.py
--rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.91/arkitekt/qt/utils.py
--rw-r--r--   0        0        0    23235 2023-03-09 13:18:29.782260 arkitekt-0.4.91/arkitekt/schemas/latest/fluss.schema.graphql
--rw-r--r--   0        0        0     5187 2023-03-09 13:18:29.814260 arkitekt-0.4.91/arkitekt/schemas/latest/kuay.schema.graphql
--rw-r--r--   0        0        0        0 2023-03-09 13:15:58.729965 arkitekt-0.4.91/arkitekt/schemas/latest/mikro.graphql
--rw-r--r--   0        0        0   100011 2023-03-09 13:18:29.466260 arkitekt-0.4.91/arkitekt/schemas/latest/mikro.schema.graphql
--rw-r--r--   0        0        0        0 2023-03-09 13:16:05.513978 arkitekt-0.4.91/arkitekt/schemas/latest/rekuest.graphql
--rw-r--r--   0        0        0    50701 2023-03-09 13:18:29.570260 arkitekt-0.4.91/arkitekt/schemas/latest/rekuest.schema.graphql
--rw-r--r--   0        0        0     8943 2023-03-09 13:18:29.854260 arkitekt-0.4.91/arkitekt/schemas/latest/unlok.schema.graphql
--rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.91/arkitekt/tqdm.py
--rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.91/arkitekt/utils.py
--rw-r--r--   0        0        0     2001 2023-04-28 13:34:13.250839 arkitekt-0.4.91/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.91/PKG-INFO
+-rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.92/arkitekt/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.92/arkitekt/apps/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.92/arkitekt/apps/connected.py
+-rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.92/arkitekt/apps/default.py
+-rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/apps/fakts.py
+-rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/apps/fluss.py
+-rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/apps/herre.py
+-rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.92/arkitekt/apps/mikro.py
+-rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.92/arkitekt/apps/rekuest.py
+-rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.92/arkitekt/apps/unlok.py
+-rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.92/arkitekt/builders.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.92/arkitekt/cli/__init__.py
+-rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.92/arkitekt/cli/build.py
+-rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.92/arkitekt/cli/configs/introspect.yaml
+-rw-r--r--   0        0        0    11054 2023-03-09 14:32:34.036965 arkitekt-0.4.92/arkitekt/cli/configs/latest.yaml
+-rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.92/arkitekt/cli/configs/minimal.yaml
+-rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.92/arkitekt/cli/deploy.py
+-rw-r--r--   0        0        0     7187 2023-04-28 13:34:41.530924 arkitekt-0.4.92/arkitekt/cli/dev.py
+-rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/cli/gen.py
+-rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.92/arkitekt/cli/init.py
+-rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.92/arkitekt/cli/inspect.py
+-rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.92/arkitekt/cli/main.py
+-rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.92/arkitekt/cli/run.py
+-rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/cli/scan.py
+-rw-r--r--   0        0        0    23235 2023-03-09 13:31:49.692385 arkitekt-0.4.92/arkitekt/cli/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0     5187 2023-03-09 13:31:49.692385 arkitekt-0.4.92/arkitekt/cli/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0   100011 2023-03-09 13:31:49.692385 arkitekt-0.4.92/arkitekt/cli/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0    50701 2023-03-09 13:31:49.692385 arkitekt-0.4.92/arkitekt/cli/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     8943 2023-03-09 13:31:49.696385 arkitekt-0.4.92/arkitekt/cli/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.92/arkitekt/cli/templates/simple.py
+-rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.92/arkitekt/cli/types.py
+-rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.92/arkitekt/cli/ui.py
+-rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.92/arkitekt/cli/utils.py
+-rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/deployers/port.py
+-rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.92/arkitekt/healthz.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.92/arkitekt/qt/__init__.py
+-rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.92/arkitekt/qt/assets/dark/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.92/arkitekt/qt/assets/dark/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.92/arkitekt/qt/assets/dark/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.92/arkitekt/qt/assets/dark/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.92/arkitekt/qt/assets/dark/red pulse.gif
+-rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.92/arkitekt/qt/assets/light/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.92/arkitekt/qt/assets/light/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.92/arkitekt/qt/assets/light/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.92/arkitekt/qt/assets/light/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.92/arkitekt/qt/assets/light/red pulse.gif
+-rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.92/arkitekt/qt/magic_bar.py
+-rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.92/arkitekt/qt/utils.py
+-rw-r--r--   0        0        0    23235 2023-03-09 13:18:29.782260 arkitekt-0.4.92/arkitekt/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0     5187 2023-03-09 13:18:29.814260 arkitekt-0.4.92/arkitekt/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0        0 2023-03-09 13:15:58.729965 arkitekt-0.4.92/arkitekt/schemas/latest/mikro.graphql
+-rw-r--r--   0        0        0   100011 2023-03-09 13:18:29.466260 arkitekt-0.4.92/arkitekt/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0        0 2023-03-09 13:16:05.513978 arkitekt-0.4.92/arkitekt/schemas/latest/rekuest.graphql
+-rw-r--r--   0        0        0    50701 2023-03-09 13:18:29.570260 arkitekt-0.4.92/arkitekt/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     8943 2023-03-09 13:18:29.854260 arkitekt-0.4.92/arkitekt/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.92/arkitekt/tqdm.py
+-rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.92/arkitekt/utils.py
+-rw-r--r--   0        0        0     2001 2023-04-28 13:34:54.310962 arkitekt-0.4.92/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.92/PKG-INFO
```

### Comparing `arkitekt-0.4.91/arkitekt/apps/connected.py` & `arkitekt-0.4.92/arkitekt/apps/connected.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/apps/default.py` & `arkitekt-0.4.92/arkitekt/apps/default.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/apps/fluss.py` & `arkitekt-0.4.92/arkitekt/apps/fluss.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/apps/mikro.py` & `arkitekt-0.4.92/arkitekt/apps/mikro.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/apps/rekuest.py` & `arkitekt-0.4.92/arkitekt/apps/rekuest.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/apps/unlok.py` & `arkitekt-0.4.92/arkitekt/apps/unlok.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/builders.py` & `arkitekt-0.4.92/arkitekt/builders.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/build.py` & `arkitekt-0.4.92/arkitekt/cli/build.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/configs/introspect.yaml` & `arkitekt-0.4.92/arkitekt/cli/configs/introspect.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/configs/latest.yaml` & `arkitekt-0.4.92/arkitekt/cli/configs/latest.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/configs/minimal.yaml` & `arkitekt-0.4.92/arkitekt/cli/configs/minimal.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/deploy.py` & `arkitekt-0.4.92/arkitekt/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/dev.py` & `arkitekt-0.4.92/arkitekt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/gen.py` & `arkitekt-0.4.92/arkitekt/cli/gen.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/init.py` & `arkitekt-0.4.92/arkitekt/cli/init.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/inspect.py` & `arkitekt-0.4.92/arkitekt/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/main.py` & `arkitekt-0.4.92/arkitekt/cli/main.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/run.py` & `arkitekt-0.4.92/arkitekt/cli/run.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/scan.py` & `arkitekt-0.4.92/arkitekt/cli/scan.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/schemas/latest/fluss.schema.graphql` & `arkitekt-0.4.92/arkitekt/cli/schemas/latest/fluss.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/schemas/latest/kuay.schema.graphql` & `arkitekt-0.4.92/arkitekt/cli/schemas/latest/kuay.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/schemas/latest/mikro.schema.graphql` & `arkitekt-0.4.92/arkitekt/cli/schemas/latest/mikro.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/schemas/latest/rekuest.schema.graphql` & `arkitekt-0.4.92/arkitekt/cli/schemas/latest/rekuest.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/schemas/latest/unlok.schema.graphql` & `arkitekt-0.4.92/arkitekt/cli/schemas/latest/unlok.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/types.py` & `arkitekt-0.4.92/arkitekt/cli/types.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/cli/ui.py` & `arkitekt-0.4.92/arkitekt/cli/ui.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/healthz.py` & `arkitekt-0.4.92/arkitekt/healthz.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/dark/gear.png` & `arkitekt-0.4.92/arkitekt/qt/assets/dark/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/dark/green pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/dark/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/dark/orange pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/dark/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/dark/pink pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/dark/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/dark/red pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/dark/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/light/gear.png` & `arkitekt-0.4.92/arkitekt/qt/assets/light/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/light/green pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/light/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/light/orange pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/light/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/light/pink pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/light/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/assets/light/red pulse.gif` & `arkitekt-0.4.92/arkitekt/qt/assets/light/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/qt/magic_bar.py` & `arkitekt-0.4.92/arkitekt/qt/magic_bar.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/schemas/latest/fluss.schema.graphql` & `arkitekt-0.4.92/arkitekt/schemas/latest/fluss.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/schemas/latest/kuay.schema.graphql` & `arkitekt-0.4.92/arkitekt/schemas/latest/kuay.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/schemas/latest/mikro.schema.graphql` & `arkitekt-0.4.92/arkitekt/schemas/latest/mikro.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/schemas/latest/rekuest.schema.graphql` & `arkitekt-0.4.92/arkitekt/schemas/latest/rekuest.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/schemas/latest/unlok.schema.graphql` & `arkitekt-0.4.92/arkitekt/schemas/latest/unlok.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/tqdm.py` & `arkitekt-0.4.92/arkitekt/tqdm.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/arkitekt/utils.py` & `arkitekt-0.4.92/arkitekt/utils.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.91/pyproject.toml` & `arkitekt-0.4.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arkitekt"
-version = "0.4.91"
+version = "0.4.92"
 description = "client for the arkitekt platform"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "arkitekt" }]
 
 [tool.poetry.dependencies]
 python = "^3.8, <=3.12"
```

### Comparing `arkitekt-0.4.91/PKG-INFO` & `arkitekt-0.4.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkitekt
-Version: 0.4.91
+Version: 0.4.92
 Summary: client for the arkitekt platform
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```
