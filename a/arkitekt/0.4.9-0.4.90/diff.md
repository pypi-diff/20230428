# Comparing `tmp/arkitekt-0.4.9.tar.gz` & `tmp/arkitekt-0.4.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitekt-0.4.9.tar", max compression
+gzip compressed data, was "arkitekt-0.4.90.tar", max compression
```

## Comparing `arkitekt-0.4.9.tar` & `arkitekt-0.4.90.tar`

### file list

```diff
@@ -1,45 +1,59 @@
--rw-r--r--   0        0        0      172 2022-11-18 16:48:57.590265 arkitekt-0.4.9/arkitekt/__init__.py
--rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.9/arkitekt/apps/__init__.py
--rw-r--r--   0        0        0      226 2022-11-21 14:11:14.252912 arkitekt-0.4.9/arkitekt/apps/connected.py
--rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.9/arkitekt/apps/default.py
--rw-r--r--   0        0        0      491 2022-10-21 15:31:51.631173 arkitekt-0.4.9/arkitekt/apps/fakts.py
--rw-r--r--   0        0        0     1961 2022-11-23 15:26:31.884045 arkitekt-0.4.9/arkitekt/apps/fluss.py
--rw-r--r--   0        0        0      392 2022-11-20 15:05:46.740463 arkitekt-0.4.9/arkitekt/apps/herre.py
--rw-r--r--   0        0        0     2852 2022-10-22 16:34:02.510574 arkitekt-0.4.9/arkitekt/apps/mikro.py
--rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.9/arkitekt/apps/rekuest.py
--rw-r--r--   0        0        0     1033 2022-11-21 14:09:49.928729 arkitekt-0.4.9/arkitekt/apps/unlok.py
--rw-r--r--   0        0        0      145 2022-11-21 14:40:42.512278 arkitekt-0.4.9/arkitekt/arkitekt.yaml
--rw-r--r--   0        0        0     4532 2023-01-16 09:35:17.399369 arkitekt-0.4.9/arkitekt/builders.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.9/arkitekt/cli/__init__.py
--rw-r--r--   0        0        0        1 2022-08-25 10:31:18.676462 arkitekt-0.4.9/arkitekt/cli/dev/__init__.py
--rw-r--r--   0        0        0     5297 2022-11-21 17:03:39.266945 arkitekt-0.4.9/arkitekt/cli/dev/autostage.py
--rw-r--r--   0        0        0     5598 2022-12-16 13:08:08.548295 arkitekt-0.4.9/arkitekt/cli/gen.py
--rw-r--r--   0        0        0        0 2022-11-21 16:10:19.141644 arkitekt-0.4.9/arkitekt/cli/logic/__init__.py
--rw-r--r--   0        0        0     2078 2022-11-23 10:45:21.435773 arkitekt-0.4.9/arkitekt/cli/logic/build.py
--rw-r--r--   0        0        0     2587 2022-11-21 16:49:29.702180 arkitekt-0.4.9/arkitekt/cli/logic/connect.py
--rw-r--r--   0        0        0     1395 2022-11-21 17:45:32.573934 arkitekt-0.4.9/arkitekt/cli/logic/dev.py
--rw-r--r--   0        0        0     4128 2022-11-21 17:34:00.265095 arkitekt-0.4.9/arkitekt/cli/logic/initialize.py
--rw-r--r--   0        0        0     1574 2022-11-21 17:44:37.901866 arkitekt-0.4.9/arkitekt/cli/logic/run.py
--rw-r--r--   0        0        0    15571 2022-11-21 17:45:40.305944 arkitekt-0.4.9/arkitekt/cli/main.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.680462 arkitekt-0.4.9/arkitekt/cli/prod/__init__.py
--rw-r--r--   0        0        0     1808 2022-10-21 12:39:18.573000 arkitekt-0.4.9/arkitekt/cli/prod/check.py
--rw-r--r--   0        0        0     1595 2022-11-04 14:10:31.707126 arkitekt-0.4.9/arkitekt/cli/prod/dump.py
--rw-r--r--   0        0        0     1537 2022-11-21 16:57:49.530568 arkitekt-0.4.9/arkitekt/cli/prod/run.py
--rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.9/arkitekt/healthz.py
--rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.9/arkitekt/qt/__init__.py
--rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.9/arkitekt/qt/assets/dark/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.9/arkitekt/qt/assets/dark/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.9/arkitekt/qt/assets/dark/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.9/arkitekt/qt/assets/dark/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.9/arkitekt/qt/assets/dark/red pulse.gif
--rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.9/arkitekt/qt/assets/light/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.9/arkitekt/qt/assets/light/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.9/arkitekt/qt/assets/light/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.9/arkitekt/qt/assets/light/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.9/arkitekt/qt/assets/light/red pulse.gif
--rw-r--r--   0        0        0     7526 2022-11-18 15:46:06.230272 arkitekt-0.4.9/arkitekt/qt/magic_bar.py
--rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.9/arkitekt/qt/utils.py
--rw-r--r--   0        0        0     2752 2022-10-04 16:14:25.218176 arkitekt-0.4.9/arkitekt/utils.py
--rw-r--r--   0        0        0     1209 2023-01-18 14:53:21.289659 arkitekt-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 arkitekt-0.4.9/setup.py
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 arkitekt-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.90/arkitekt/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.90/arkitekt/apps/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.90/arkitekt/apps/connected.py
+-rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.90/arkitekt/apps/default.py
+-rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/apps/fakts.py
+-rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/apps/fluss.py
+-rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/apps/herre.py
+-rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.90/arkitekt/apps/mikro.py
+-rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.90/arkitekt/apps/rekuest.py
+-rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.90/arkitekt/apps/unlok.py
+-rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.90/arkitekt/builders.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.90/arkitekt/cli/__init__.py
+-rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.90/arkitekt/cli/build.py
+-rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.90/arkitekt/cli/configs/introspect.yaml
+-rw-r--r--   0        0        0    11054 2023-03-09 14:32:34.036965 arkitekt-0.4.90/arkitekt/cli/configs/latest.yaml
+-rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.90/arkitekt/cli/configs/minimal.yaml
+-rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.90/arkitekt/cli/deploy.py
+-rw-r--r--   0        0        0     7096 2023-04-21 13:20:29.188573 arkitekt-0.4.90/arkitekt/cli/dev.py
+-rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/cli/gen.py
+-rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.90/arkitekt/cli/init.py
+-rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.90/arkitekt/cli/inspect.py
+-rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.90/arkitekt/cli/main.py
+-rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.90/arkitekt/cli/run.py
+-rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/cli/scan.py
+-rw-r--r--   0        0        0    23235 2023-03-09 13:31:49.692385 arkitekt-0.4.90/arkitekt/cli/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0     5187 2023-03-09 13:31:49.692385 arkitekt-0.4.90/arkitekt/cli/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0   100011 2023-03-09 13:31:49.692385 arkitekt-0.4.90/arkitekt/cli/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0    50701 2023-03-09 13:31:49.692385 arkitekt-0.4.90/arkitekt/cli/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     8943 2023-03-09 13:31:49.696385 arkitekt-0.4.90/arkitekt/cli/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.90/arkitekt/cli/templates/simple.py
+-rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.90/arkitekt/cli/types.py
+-rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.90/arkitekt/cli/ui.py
+-rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.90/arkitekt/cli/utils.py
+-rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/deployers/port.py
+-rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.90/arkitekt/healthz.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.90/arkitekt/qt/__init__.py
+-rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.90/arkitekt/qt/assets/dark/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.90/arkitekt/qt/assets/dark/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.90/arkitekt/qt/assets/dark/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.90/arkitekt/qt/assets/dark/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.90/arkitekt/qt/assets/dark/red pulse.gif
+-rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.90/arkitekt/qt/assets/light/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.90/arkitekt/qt/assets/light/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.90/arkitekt/qt/assets/light/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.90/arkitekt/qt/assets/light/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.90/arkitekt/qt/assets/light/red pulse.gif
+-rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.90/arkitekt/qt/magic_bar.py
+-rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.90/arkitekt/qt/utils.py
+-rw-r--r--   0        0        0    23235 2023-03-09 13:18:29.782260 arkitekt-0.4.90/arkitekt/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0     5187 2023-03-09 13:18:29.814260 arkitekt-0.4.90/arkitekt/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0        0 2023-03-09 13:15:58.729965 arkitekt-0.4.90/arkitekt/schemas/latest/mikro.graphql
+-rw-r--r--   0        0        0   100011 2023-03-09 13:18:29.466260 arkitekt-0.4.90/arkitekt/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0        0 2023-03-09 13:16:05.513978 arkitekt-0.4.90/arkitekt/schemas/latest/rekuest.graphql
+-rw-r--r--   0        0        0    50701 2023-03-09 13:18:29.570260 arkitekt-0.4.90/arkitekt/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     8943 2023-03-09 13:18:29.854260 arkitekt-0.4.90/arkitekt/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.90/arkitekt/tqdm.py
+-rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.90/arkitekt/utils.py
+-rw-r--r--   0        0        0     2001 2023-04-28 13:05:17.058458 arkitekt-0.4.90/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.90/PKG-INFO
```

### Comparing `arkitekt-0.4.9/arkitekt/apps/default.py` & `arkitekt-0.4.90/arkitekt/apps/default.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/apps/fluss.py` & `arkitekt-0.4.90/arkitekt/apps/fluss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from arkitekt.apps.herre import HerreApp
 from pydantic import Field
 from fluss.fluss import Fluss
 from fluss.rath import FlussLinkComposition, FlussRath
-from rath.contrib.fakts.links.httpx import FaktsHttpXLink
 from rath.links.split import SplitLink
 from rath.contrib.fakts.links.aiohttp import FaktsAIOHttpLink
 from rath.contrib.fakts.links.websocket import FaktsWebsocketLink
 from rath.contrib.herre.links.auth import HerreAuthLink
 from graphql import OperationType
-from .connected import ConnectedApp
 from .rekuest import RekuestApp
 from .unlok import UnlokApp
 from arkitekt.healthz import FaktsHealthz
 
 
 class ArkitektFluss(Fluss):
     rath: FlussRath = Field(
         default_factory=lambda: FlussRath(
             link=FlussLinkComposition(
                 auth=HerreAuthLink(),
                 split=SplitLink(
-                    left=FaktsHttpXLink(fakts_group="fluss"),
+                    left=FaktsAIOHttpLink(fakts_group="fluss"),
                     right=FaktsWebsocketLink(fakts_group="fluss"),
                     split=lambda o: o.node.operation != OperationType.SUBSCRIPTION,
                 ),
             )
         )
     )
     healthz: FaktsHealthz = Field(
```

### Comparing `arkitekt-0.4.9/arkitekt/apps/mikro.py` & `arkitekt-0.4.90/arkitekt/apps/mikro.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     right=FaktsWebsocketLink(fakts_group="mikro"),
                     split=lambda o: o.node.operation != OperationType.SUBSCRIPTION,
                 ),
             )
         )
     )
     datalayer: DataLayer = Field(
-        default_factory=lambda: FaktsDataLayer(fakts_group="mikro.datalayer")
+        default_factory=lambda: FaktsDataLayer(fakts_group="minio")
     )
     healthz: FaktsHealthz = Field(
         default_factory=lambda: FaktsHealthz(fakts_group="mikro")
     )
 
 
 class MikroApp(HerreApp):
```

### Comparing `arkitekt-0.4.9/arkitekt/apps/rekuest.py` & `arkitekt-0.4.90/arkitekt/apps/rekuest.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/apps/unlok.py` & `arkitekt-0.4.90/arkitekt/apps/unlok.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 from unlok import Unlok
 from unlok.rath import UnlokRath, UnlokLinkComposition
 from pydantic import Field
 from rath.links.split import SplitLink
 from rath.contrib.fakts.links.aiohttp import FaktsAIOHttpLink
 from rath.contrib.fakts.links.websocket import FaktsWebsocketLink
 from rath.contrib.herre.links.auth import HerreAuthLink
-from mikro.contrib.fakts.datalayer import FaktsDataLayer
 from graphql import OperationType
 
 
 class ArkitektUnlok(Unlok):
     rath: UnlokRath = Field(
         default_factory=lambda: UnlokRath(
             link=UnlokLinkComposition(
                 auth=HerreAuthLink(),
-                split=SplitLink(
-                    left=FaktsAIOHttpLink(fakts_group="herre"),
-                    right=FaktsWebsocketLink(fakts_group="herre"),
-                    split=lambda o: o.node.operation != OperationType.SUBSCRIPTION,
-                ),
+                split=FaktsAIOHttpLink(fakts_group="lok"),
             )
         )
     )
 
 
 class UnlokApp(HerreApp):
     """Lok App"""
```

### Comparing `arkitekt-0.4.9/arkitekt/cli/gen.py` & `arkitekt-0.4.90/arkitekt/cli/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     ChildPortFragment,
     PortKind,
     ReturnPortFragment,
     retrieveall
 )
     
 
-from black import format_str, FileMode
 import ast
 import re
 import inflection
 from arkitekt import easy
 
 def clean(varStr):
     return re.sub("\W|^(?=\d)", "_", varStr)
@@ -130,15 +129,15 @@
     args: List[ArgPortFragment]
 ):
 
     pos_args = []
     kw_values = []
 
     for arg in args:
-        annotation = get_arg_annotation(arg)
+        get_arg_annotation(arg)
         if arg.default:
             kw_values.append(ast.Constant(value=arg.default))
 
     return ast.arguments(
         args=pos_args,
         posonlyargs=[],
         kwonlyargs=[],
```

### Comparing `arkitekt-0.4.9/arkitekt/healthz.py` & `arkitekt-0.4.90/arkitekt/healthz.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/dark/gear.png` & `arkitekt-0.4.90/arkitekt/qt/assets/dark/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/dark/green pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/dark/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/dark/orange pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/dark/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/dark/pink pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/dark/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/dark/red pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/dark/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/light/gear.png` & `arkitekt-0.4.90/arkitekt/qt/assets/light/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/light/green pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/light/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/light/orange pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/light/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/light/pink pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/light/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/assets/light/red pulse.gif` & `arkitekt-0.4.90/arkitekt/qt/assets/light/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.9/arkitekt/qt/magic_bar.py` & `arkitekt-0.4.90/arkitekt/qt/magic_bar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 from enum import Enum
 from qtpy import QtWidgets, QtGui, QtCore
 from koil.qt import QtRunner
-from arkitekt.apps.rekuest import RekuestApp
+from arkitekt import Arkitekt
 from .utils import get_image_path
 
 
 class Profile(QtWidgets.QDialog):
+    updated = QtCore.Signal()
+
     def __init__(
         self,
-        app: RekuestApp,
+        app: Arkitekt,
         bar: "MagicBar",
         *args,
         dark_mode: bool = False,
         **kwargs,
-    ):
+    ) -> None:
         super(Profile, self).__init__(*args, parent=bar, **kwargs)
         self.app = app
         self.bar = bar
 
+
+        self.settings = QtCore.QSettings("arkitekt", f"{self.app.identifier}:{self.app.version}")
+
         self.setWindowTitle("Profile")
         self.layout = QtWidgets.QVBoxLayout()
         self.setLayout(self.layout)
 
         self.logout_button = QtWidgets.QPushButton("Logout")
         self.logout_button.clicked.connect(lambda: self.bar.logout_task.run())
 
         self.unkonfigure_button = QtWidgets.QPushButton("Unkonfirug")
         self.unkonfigure_button.clicked.connect(
             lambda: self.bar.configure_task.run(force_refresh=True)
         )
 
+        self.go_all_the_way_button = QtWidgets.QPushButton("One click provide")
+        self.go_all_the_way_button.setCheckable(True)
+        self.go_all_the_way_button.setChecked(self.go_all_the_way_down)
+        self.go_all_the_way_button.clicked.connect(self.on_go_all_the_way_clicked)
+
+
         self.layout.addWidget(self.logout_button)
         self.layout.addWidget(self.unkonfigure_button)
+        self.layout.addWidget(self.go_all_the_way_button)
+
+
+    def on_go_all_the_way_clicked(self, checked: bool) -> None:
+        self.settings.setValue("go_all_the_way_down", checked)
+        self.updated.emit()
+
+    @property
+    def go_all_the_way_down(self) -> bool:
+        return self.settings.value("go_all_the_way_down", False, bool)
 
 
 class AppState(str, Enum):
     READY = "ready"
     DOWN = "down"
     UP = "up"
 
@@ -44,29 +65,39 @@
     UNKONFIGURED = "unkonfigured"
     UNLOGGED = "unlogged"
     UNPROVIDED = "unprovided"
     PROVIDING = "providing"
 
 
 class MagicBar(QtWidgets.QWidget):
+    CONNECT_LABEL = "Connect"
+
+
+    app_state_changed = QtCore.Signal()
     app_up = QtCore.Signal()
     app_down = QtCore.Signal()
     app_error = QtCore.Signal()
     state = AppState.DOWN
     process_state = ProcessState.UNKONFIGURED
 
-    def __init__(self, app: RekuestApp, dark_mode: bool = False) -> None:
+
+    def __init__(self, app: Arkitekt, dark_mode: bool = False) -> None:
         super().__init__()
         self.app = app
+
+
         # assert isinstance(
         #     self.app.koil, QtPedanticKoil
         # ), f"Koil should be Qt Koil but is {type(self.app.koil)}"
         self.dark_mode = dark_mode
 
+
+
         self.profile = Profile(app, self, dark_mode=dark_mode)
+        self.profile.updated.connect(self.on_profile_updated)
 
         self.configure_task = QtRunner(self.app.fakts.aload)
         self.configure_task.errored.connect(self.configure_errored)
         self.configure_task.returned.connect(self.set_unlogined)
 
         self.login_task = QtRunner(self.app.herre.alogin)
         self.login_task.errored.connect(self.login_errored)
@@ -76,15 +107,15 @@
         self.logout_task.errored.connect(self.task_errored)
         self.logout_task.returned.connect(self.set_unlogined)
 
         self.provide_task: QtRunner = QtRunner(self.app.rekuest.agent.aprovide)
         self.provide_task.errored.connect(self.provide_errored)
         self.provide_task.returned.connect(self.set_unprovided)
 
-        self.magicb = QtWidgets.QPushButton("Connect")
+        self.magicb = QtWidgets.QPushButton(MagicBar.CONNECT_LABEL)
         self.magicb.setMinimumHeight(30)
         self.magicb.setMaximumHeight(30)
 
         self.configure_future = None
         self.login_future = None
         self.provide_future = None
 
@@ -101,32 +132,49 @@
         self.gearb.clicked.connect(self.gear_button_clicked)
 
         self.layout.addWidget(self.magicb)
         self.layout.addWidget(self.gearb)
         self.setLayout(self.layout)
 
         self.set_unkonfigured()
+        self.on_profile_updated()
+
+    def on_profile_updated(self):
+        if self.profile.go_all_the_way_down:
+            self.set_unprovided()
+        
+    def show_error(self, ex: Exception):
+        dialog = QtWidgets.QDialog()
+        dialog.setWindowTitle("Error")
+        layout = QtWidgets.QVBoxLayout()
+        dialog.setLayout(layout)
+        label = QtWidgets.QLabel(str(ex))
+        layout.addWidget(label)
+        dialog.exec_()
 
     def task_errored(self, ex: Exception):
         raise ex
 
     def configure_errored(self, ex: Exception):
         self.set_unkonfigured()
-        raise ex
+        self.show_error(ex)
+
 
     def login_errored(self, ex: Exception):
         self.set_unlogined()
         raise ex
+        self.show_error(ex)
 
     def provide_errored(self, ex: Exception):
         self.set_unprovided()
         raise ex
+        self.show_error(ex)
 
     def on_configured(self):
-        set.set
+        self.magicb.setText("Login")
 
     def on_login(self):
         self.magicb.setText("Provide")
 
     def on_provided(self):
         self.magicb.setText("Provide ended")
 
@@ -147,76 +195,82 @@
         self.magicb_movie.setScaledSize(QtCore.QSize(30, 30))
         self.magicb_movie.start()
 
     def set_unkonfigured(self):
         self.state = AppState.DOWN
         self.process_state = ProcessState.UNKONFIGURED
         self.app_down.emit()
+        self.app_state_changed.emit()
         self.set_button_movie("pink pulse.gif")
         self.profile.unkonfigure_button.setDisabled(True)
         self.profile.logout_button.setDisabled(True)
         self.magicb.setDisabled(False)
         self.magicb.setText("Konfigure App")
 
     def set_unlogined(self):
         self.state = AppState.DOWN
         self.process_state = ProcessState.UNLOGGED
         self.app_down.emit()
+
+        self.app_state_changed.emit()
         self.set_button_movie("orange pulse.gif")
         self.profile.unkonfigure_button.setDisabled(False)
         self.profile.logout_button.setDisabled(True)
         self.magicb.setDisabled(False)
         self.magicb.setText("Login")
 
     def set_unprovided(self):
         self.state = AppState.UP
         self.process_state = ProcessState.UNPROVIDED
         self.app_up.emit()
+
+        self.app_state_changed.emit()
         self.set_button_movie("green pulse.gif")
         self.profile.unkonfigure_button.setDisabled(False)
         self.profile.logout_button.setDisabled(False)
         self.magicb.setDisabled(False)
         self.magicb.setText("Provide")
 
     def set_providing(self):
         self.state = AppState.UP
         self.process_state = ProcessState.PROVIDING
         self.app_up.emit()
+
+        self.app_state_changed.emit()
         self.set_button_movie("red pulse.gif")
         self.profile.unkonfigure_button.setDisabled(False)
         self.profile.logout_button.setDisabled(False)
         self.magicb.setDisabled(False)
         self.magicb.setText("Cancel Provide..")
 
     def magic_button_clicked(self):
-        if self.process_state == ProcessState.UNKONFIGURED:
+        if self.process_state == ProcessState.UNKONFIGURED and not self.profile.go_all_the_way_down:
             if not self.configure_future or self.configure_future.done():
                 self.configure_future = self.configure_task.run()
                 self.magicb.setText("Cancel Configuration")
                 return
             if not self.configure_future.done():
                 self.configure_future.cancel()
                 self.set_unkonfigured()
                 return
 
-        if self.process_state == ProcessState.UNLOGGED:
+        if self.process_state == ProcessState.UNLOGGED and not self.profile.go_all_the_way_down:
             if not self.login_future or self.login_future.done():
                 self.login_future = self.login_task.run()
                 self.magicb.setText("Cancel Login")
                 return
             if not self.login_future.done():
                 self.login_future.cancel()
                 self.magicb.setText("Login")
                 self.set_unlogined()
                 return
 
-        if self.process_state == ProcessState.UNPROVIDED:
+        if self.process_state != ProcessState.PROVIDING or self.profile.go_all_the_way_down:
             if not self.provide_future or self.provide_future.done():
                 self.provide_future = self.provide_task.run()
                 self.set_providing()
                 return
 
-        if self.process_state == ProcessState.PROVIDING:
-            if not self.provide_future.done():
-                self.provide_future.cancel()
-                self.set_unprovided()
-                return
+        if not self.provide_future.done():
+            self.provide_future.cancel()
+            self.set_unprovided()
+            return
```

