# Comparing `tmp/hpr_scratcher-0.6.0.tar.gz` & `tmp/hpr_scratcher-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpr_scratcher-0.6.0.tar", max compression
+gzip compressed data, was "hpr_scratcher-0.6.1.tar", max compression
```

## Comparing `hpr_scratcher-0.6.0.tar` & `hpr_scratcher-0.6.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3147 2023-04-22 13:17:50.013907 hpr_scratcher-0.6.0/README.md
--rwxr-xr-x   0        0        0    15800 2023-04-21 19:41:03.866374 hpr_scratcher-0.6.0/hpr_scratcher/__init__.py
--rw-r--r--   0        0        0      479 2023-04-22 13:16:59.162457 hpr_scratcher-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 hpr_scratcher-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3272 2023-04-27 20:07:42.825670 hpr_scratcher-0.6.1/README.md
+-rwxr-xr-x   0        0        0    15874 2023-04-28 19:57:53.478166 hpr_scratcher-0.6.1/hpr_scratcher/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-28 19:58:23.284235 hpr_scratcher-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 hpr_scratcher-0.6.1/PKG-INFO
```

### Comparing `hpr_scratcher-0.6.0/README.md` & `hpr_scratcher-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+If you like to write your own extensions or get more features, you may want to check out https://github.com/fdev31/pyprland
+
 # Installation
 
 ```
 pip install hpr-scratcher
 ```
 
 _OR_
```

### Comparing `hpr_scratcher-0.6.0/hpr_scratcher/__init__.py` & `hpr_scratcher-0.6.1/hpr_scratcher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,32 +304,34 @@
         client_height = client["size"][1]
         margin_x = int((mon_width - client_width) / 2) + mon_x
         await hyprctl(
             f"movewindowpixel exact {margin_x} {mon_y + mon_height - client_height - margin},{client_uid}"
         )
 
     async def _animation_fromleft(self, monitor, client, client_uid, margin):
+        mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_height = monitor["height"]
 
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
 
-        await hyprctl(f"movewindowpixel exact {margin} {margin_y},{client_uid}")
+        await hyprctl(f"movewindowpixel exact {margin + mon_x} {margin_y},{client_uid}")
 
     async def _animation_fromright(self, monitor, client, client_uid, margin):
+        mon_x = monitor["x"]
         mon_y = monitor["y"]
         mon_width = monitor["width"]
         mon_height = monitor["height"]
 
         client_width = client["size"][0]
         client_height = client["size"][1]
         margin_y = int((mon_height - client_height) / 2) + mon_y
         await hyprctl(
-            f"movewindowpixel exact {mon_width - client_width - margin} {margin_y},{client_uid}"
+            f"movewindowpixel exact {mon_width - client_width - margin + mon_x} {margin_y},{client_uid}"
         )
 
     async def run_show(self, uid, force=False):
         uid = uid.strip()
         item = self.scratches.get(uid)
 
         if not item:
```

### Comparing `hpr_scratcher-0.6.0/PKG-INFO` & `hpr_scratcher-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: hpr-scratcher
-Version: 0.6.0
+Version: 0.6.1
 Summary: A scratchpad manager for hyprland
 Home-page: https://github.com/hyprland-community/hpr-scratcher
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
+If you like to write your own extensions or get more features, you may want to check out https://github.com/fdev31/pyprland
+
 # Installation
 
 ```
 pip install hpr-scratcher
 ```
 
 _OR_
```

