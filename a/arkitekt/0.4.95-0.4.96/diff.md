# Comparing `tmp/arkitekt-0.4.95.tar.gz` & `tmp/arkitekt-0.4.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitekt-0.4.95.tar", max compression
+gzip compressed data, was "arkitekt-0.4.96.tar", max compression
```

## Comparing `arkitekt-0.4.95.tar` & `arkitekt-0.4.96.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.95/arkitekt/__init__.py
--rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.95/arkitekt/apps/__init__.py
--rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.95/arkitekt/apps/connected.py
--rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.95/arkitekt/apps/default.py
--rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/apps/fakts.py
--rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/apps/fluss.py
--rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/apps/herre.py
--rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.95/arkitekt/apps/mikro.py
--rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.95/arkitekt/apps/rekuest.py
--rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.95/arkitekt/apps/unlok.py
--rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.95/arkitekt/builders.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.95/arkitekt/cli/__init__.py
--rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.95/arkitekt/cli/build.py
--rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.95/arkitekt/cli/configs/introspect.yaml
--rw-r--r--   0        0        0    11676 2023-04-28 14:07:07.025792 arkitekt-0.4.95/arkitekt/cli/configs/latest.yaml
--rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.95/arkitekt/cli/configs/minimal.yaml
--rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.95/arkitekt/cli/deploy.py
--rw-r--r--   0        0        0     7187 2023-04-28 13:34:41.530924 arkitekt-0.4.95/arkitekt/cli/dev.py
--rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/cli/gen.py
--rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.95/arkitekt/cli/init.py
--rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.95/arkitekt/cli/inspect.py
--rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.95/arkitekt/cli/main.py
--rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.95/arkitekt/cli/run.py
--rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/cli/scan.py
--rw-r--r--   0        0        0    24496 2023-04-28 14:09:38.190295 arkitekt-0.4.95/arkitekt/cli/schemas/latest/fluss.schema.graphql
--rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.442296 arkitekt-0.4.95/arkitekt/cli/schemas/latest/gucker.schema.graphql
--rw-r--r--   0        0        0     4905 2023-04-28 14:09:38.226296 arkitekt-0.4.95/arkitekt/cli/schemas/latest/kuay.schema.graphql
--rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.022295 arkitekt-0.4.95/arkitekt/cli/schemas/latest/mikro.schema.graphql
--rw-r--r--   0        0        0    51282 2023-04-28 14:09:38.118295 arkitekt-0.4.95/arkitekt/cli/schemas/latest/rekuest.schema.graphql
--rw-r--r--   0        0        0    10014 2023-04-28 14:09:38.270296 arkitekt-0.4.95/arkitekt/cli/schemas/latest/unlok.schema.graphql
--rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.95/arkitekt/cli/templates/simple.py
--rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.95/arkitekt/cli/types.py
--rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.95/arkitekt/cli/ui.py
--rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.95/arkitekt/cli/utils.py
--rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/deployers/port.py
--rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.95/arkitekt/healthz.py
--rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.95/arkitekt/qt/__init__.py
--rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.95/arkitekt/qt/assets/dark/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.95/arkitekt/qt/assets/dark/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.95/arkitekt/qt/assets/dark/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.95/arkitekt/qt/assets/dark/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.95/arkitekt/qt/assets/dark/red pulse.gif
--rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.95/arkitekt/qt/assets/light/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.95/arkitekt/qt/assets/light/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.95/arkitekt/qt/assets/light/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.95/arkitekt/qt/assets/light/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.95/arkitekt/qt/assets/light/red pulse.gif
--rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.95/arkitekt/qt/magic_bar.py
--rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.95/arkitekt/qt/utils.py
--rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.95/arkitekt/tqdm.py
--rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.95/arkitekt/utils.py
--rw-r--r--   0        0        0     2001 2023-04-28 14:09:42.058308 arkitekt-0.4.95/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.95/PKG-INFO
+-rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.96/arkitekt/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.96/arkitekt/apps/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.96/arkitekt/apps/connected.py
+-rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.96/arkitekt/apps/default.py
+-rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/apps/fakts.py
+-rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/apps/fluss.py
+-rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/apps/herre.py
+-rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.96/arkitekt/apps/mikro.py
+-rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.96/arkitekt/apps/rekuest.py
+-rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.96/arkitekt/apps/unlok.py
+-rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.96/arkitekt/builders.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.96/arkitekt/cli/__init__.py
+-rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.96/arkitekt/cli/build.py
+-rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.96/arkitekt/cli/configs/introspect.yaml
+-rw-r--r--   0        0        0    11706 2023-04-28 14:16:38.131941 arkitekt-0.4.96/arkitekt/cli/configs/latest.yaml
+-rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.96/arkitekt/cli/configs/minimal.yaml
+-rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.96/arkitekt/cli/deploy.py
+-rw-r--r--   0        0        0     7187 2023-04-28 13:34:41.530924 arkitekt-0.4.96/arkitekt/cli/dev.py
+-rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/cli/gen.py
+-rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.96/arkitekt/cli/init.py
+-rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.96/arkitekt/cli/inspect.py
+-rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.96/arkitekt/cli/main.py
+-rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.96/arkitekt/cli/run.py
+-rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/cli/scan.py
+-rw-r--r--   0        0        0    24496 2023-04-28 14:09:38.190295 arkitekt-0.4.96/arkitekt/cli/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.442296 arkitekt-0.4.96/arkitekt/cli/schemas/latest/gucker.schema.graphql
+-rw-r--r--   0        0        0     4905 2023-04-28 14:09:38.226296 arkitekt-0.4.96/arkitekt/cli/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.022295 arkitekt-0.4.96/arkitekt/cli/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0    51282 2023-04-28 14:09:38.118295 arkitekt-0.4.96/arkitekt/cli/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0    10014 2023-04-28 14:09:38.270296 arkitekt-0.4.96/arkitekt/cli/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.96/arkitekt/cli/templates/simple.py
+-rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.96/arkitekt/cli/types.py
+-rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.96/arkitekt/cli/ui.py
+-rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.96/arkitekt/cli/utils.py
+-rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/deployers/port.py
+-rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.96/arkitekt/healthz.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.96/arkitekt/qt/__init__.py
+-rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.96/arkitekt/qt/assets/dark/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.96/arkitekt/qt/assets/dark/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.96/arkitekt/qt/assets/dark/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.96/arkitekt/qt/assets/dark/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.96/arkitekt/qt/assets/dark/red pulse.gif
+-rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.96/arkitekt/qt/assets/light/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.96/arkitekt/qt/assets/light/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.96/arkitekt/qt/assets/light/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.96/arkitekt/qt/assets/light/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.96/arkitekt/qt/assets/light/red pulse.gif
+-rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.96/arkitekt/qt/magic_bar.py
+-rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.96/arkitekt/qt/utils.py
+-rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.96/arkitekt/tqdm.py
+-rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.96/arkitekt/utils.py
+-rw-r--r--   0        0        0     2001 2023-04-28 14:16:40.123951 arkitekt-0.4.96/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.96/PKG-INFO
```

### Comparing `arkitekt-0.4.95/arkitekt/apps/connected.py` & `arkitekt-0.4.96/arkitekt/apps/connected.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/apps/default.py` & `arkitekt-0.4.96/arkitekt/apps/default.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/apps/fluss.py` & `arkitekt-0.4.96/arkitekt/apps/fluss.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/apps/mikro.py` & `arkitekt-0.4.96/arkitekt/apps/mikro.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/apps/rekuest.py` & `arkitekt-0.4.96/arkitekt/apps/rekuest.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/apps/unlok.py` & `arkitekt-0.4.96/arkitekt/apps/unlok.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/builders.py` & `arkitekt-0.4.96/arkitekt/builders.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/build.py` & `arkitekt-0.4.96/arkitekt/cli/build.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/configs/introspect.yaml` & `arkitekt-0.4.96/arkitekt/cli/configs/introspect.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/configs/latest.yaml` & `arkitekt-0.4.96/arkitekt/cli/configs/latest.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 projects:
   mikro:
     schema: .arkitekt/schemas/mikro.schema.graphql
     documents: graphql/mikro/*/**.graphql
     extensions:
       turms:
-        out_dir: mikro/api
+        generated_name: mikro.py
         exclude_typenames: true
         freeze:
           enabled: true
         options:
           enabled: true
           use_enum_values: true
           extra: "forbid"
@@ -91,15 +91,15 @@
           InputVector:
             - mikro.traits.Vectorizable
   rekuest:
     schema: .arkitekt/schemas/rekuest.schema.graphql
     documents: graphql/rekuest/*/**.graphql
     extensions:
       turms:
-        out_dir: rekuest/api
+        generated_name: rekuest.py
         always_resolve_interfaces: True
         exclude_typenames: true
         freeze:
           enabled: true
         options:
           enabled: true
           use_enum_values: true
@@ -171,15 +171,15 @@
           ReturnWidgetInput:
             - rekuest.traits.ports.ReturnWidgetInputTrait
   fluss:
     schema: .arkitekt/schemas/fluss.schema.graphql
     documents: graphql/fluss/*/**.graphql
     extensions:
       turms:
-        out_dir: fluss/api
+        generated_name: fluss.py
         exclude_typenames: true
         freeze:
           enabled: true
         options:
           enabled: true
           use_enum_values: true
           extra: "forbid"
@@ -236,15 +236,15 @@
           StreamItemChild:
             - fluss.traits.MockableTrait
   kuay:
     schema: .arkitekt/schemas/kuay.schema.graphql
     documents: graphql/kuay/*/**.graphql
     extensions:
       turms:
-        out_dir: kuay/api
+        generated_name: kuay.py
         exclude_typenames: true
         freeze:
           enabled: true
         options:
           enabled: true
           use_enum_values: true
           extra: "forbid"
@@ -289,15 +289,15 @@
           Any: typing.Any
           ID: rath.scalars.ID
   unlok:
     schema: .arkitekt/schemas/unlok.schema.graphql
     documents: graphql/unlok/*/**.graphql
     extensions:
       turms:
-        out_dir: unlok/api
+        generated_name: unlok.py
         exclude_typenames: true
         freeze:
           enabled: true
         options:
           enabled: true
           use_enum_values: true
           extra: "forbid"
```

### Comparing `arkitekt-0.4.95/arkitekt/cli/configs/minimal.yaml` & `arkitekt-0.4.96/arkitekt/cli/configs/minimal.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/deploy.py` & `arkitekt-0.4.96/arkitekt/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/dev.py` & `arkitekt-0.4.96/arkitekt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/gen.py` & `arkitekt-0.4.96/arkitekt/cli/gen.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/init.py` & `arkitekt-0.4.96/arkitekt/cli/init.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/inspect.py` & `arkitekt-0.4.96/arkitekt/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/main.py` & `arkitekt-0.4.96/arkitekt/cli/main.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/run.py` & `arkitekt-0.4.96/arkitekt/cli/run.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/scan.py` & `arkitekt-0.4.96/arkitekt/cli/scan.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/fluss.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/fluss.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/gucker.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/gucker.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/kuay.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/kuay.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/mikro.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/mikro.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/rekuest.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/rekuest.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/schemas/latest/unlok.schema.graphql` & `arkitekt-0.4.96/arkitekt/cli/schemas/latest/unlok.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/types.py` & `arkitekt-0.4.96/arkitekt/cli/types.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/cli/ui.py` & `arkitekt-0.4.96/arkitekt/cli/ui.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/healthz.py` & `arkitekt-0.4.96/arkitekt/healthz.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/dark/gear.png` & `arkitekt-0.4.96/arkitekt/qt/assets/dark/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/dark/green pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/dark/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/dark/orange pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/dark/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/dark/pink pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/dark/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/dark/red pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/dark/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/light/gear.png` & `arkitekt-0.4.96/arkitekt/qt/assets/light/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/light/green pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/light/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/light/orange pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/light/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/light/pink pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/light/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/assets/light/red pulse.gif` & `arkitekt-0.4.96/arkitekt/qt/assets/light/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/qt/magic_bar.py` & `arkitekt-0.4.96/arkitekt/qt/magic_bar.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/tqdm.py` & `arkitekt-0.4.96/arkitekt/tqdm.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/arkitekt/utils.py` & `arkitekt-0.4.96/arkitekt/utils.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.95/pyproject.toml` & `arkitekt-0.4.96/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arkitekt"
-version = "0.4.95"
+version = "0.4.96"
 description = "client for the arkitekt platform"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "arkitekt" }]
 
 [tool.poetry.dependencies]
 python = "^3.8, <=3.12"
```

### Comparing `arkitekt-0.4.95/PKG-INFO` & `arkitekt-0.4.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkitekt
-Version: 0.4.95
+Version: 0.4.96
 Summary: client for the arkitekt platform
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

