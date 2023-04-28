# Comparing `tmp/TkUI-0.1.0.tar.gz` & `tmp/TkUI-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TkUI-0.1.0.tar", last modified: Thu Apr 27 05:52:53 2023, max compression
+gzip compressed data, was "dist\TkUI-0.2.0.tar", last modified: Fri Apr 28 01:47:29 2023, max compression
```

## Comparing `TkUI-0.1.0.tar` & `TkUI-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:53.027639 TkUI-0.1.0/
--rw-rw-rw-   0        0        0      405 2023-04-27 05:52:53.025606 TkUI-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-04-27 05:52:12.000000 TkUI-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:53.009440 TkUI-0.1.0/TkUI.egg-info/
--rw-rw-rw-   0        0        0      405 2023-04-27 05:52:52.000000 TkUI-0.1.0/TkUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-27 05:52:52.000000 TkUI-0.1.0/TkUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 05:52:52.000000 TkUI-0.1.0/TkUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 05:52:52.000000 TkUI-0.1.0/TkUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 05:52:53.027639 TkUI-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      580 2023-04-27 05:52:49.000000 TkUI-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:52:53.022652 TkUI-0.1.0/tkui/
--rw-rw-rw-   0        0        0       15 2023-04-27 05:49:18.000000 TkUI-0.1.0/tkui/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-27 03:40:57.000000 TkUI-0.1.0/tkui/base.py
--rw-rw-rw-   0        0        0     2559 2023-04-27 03:40:57.000000 TkUI-0.1.0/tkui/layout.py
--rw-rw-rw-   0        0        0      854 2023-04-27 02:13:36.000000 TkUI-0.1.0/tkui/tkui.py
--rw-rw-rw-   0        0        0      517 2023-04-27 02:51:31.000000 TkUI-0.1.0/tkui/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:47:29.274207 TkUI-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-27 06:30:40.000000 TkUI-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      505 2023-04-28 01:47:29.273210 TkUI-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-04-27 06:25:08.000000 TkUI-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 01:47:29.243708 TkUI-0.2.0/TkUI.egg-info/
+-rw-rw-rw-   0        0        0      505 2023-04-28 01:47:28.000000 TkUI-0.2.0/TkUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-28 01:47:29.000000 TkUI-0.2.0/TkUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 01:47:28.000000 TkUI-0.2.0/TkUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-28 01:47:28.000000 TkUI-0.2.0/TkUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 01:47:29.274207 TkUI-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-04-28 01:47:05.000000 TkUI-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 01:47:29.270216 TkUI-0.2.0/tkui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:31:01.000000 TkUI-0.2.0/tkui/__init__.py
+-rw-rw-rw-   0        0        0     3120 2023-04-28 01:30:34.000000 TkUI-0.2.0/tkui/base.py
+-rw-rw-rw-   0        0        0     5688 2023-04-27 09:29:47.000000 TkUI-0.2.0/tkui/layout.py
+-rw-rw-rw-   0        0        0      789 2023-04-28 01:30:25.000000 TkUI-0.2.0/tkui/tkui.py
+-rw-rw-rw-   0        0        0     1111 2023-04-27 07:06:08.000000 TkUI-0.2.0/tkui/utils.py
```

### Comparing `TkUI-0.1.0/setup.py` & `TkUI-0.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TkUI",
-    version="0.1.0",
+    version="0.2.0",
     author="iamxcd",
     author_email="iamxcd@gmail.com",
     description="TkUI,是基于tkinter的Canvas模块开发的,具有现代化风格的UI库",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/iamxcd/tk-ui",
     packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3"
-    ],
+    classifiers=[]
 )
```

### Comparing `TkUI-0.1.0/tkui/tkui.py` & `TkUI-0.2.0/tkui/tkui.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,13 +16,12 @@
         self.widgets.append(widget)
         return self
 
     def __reset(self, evt: Event):
         """
         窗口大小重置,更新子组件
         """
-        w_rate = evt.width / self.size[0]
-        h_rate = evt.height / self.size[1]
-        self.size = (evt.width, evt.height)
         self.delete(ALL)
         for widget in self.widgets:
-            widget.zoom(w_rate, h_rate)
+            widget.zoom(self.size, (evt.width, evt.height))
+
+        self.size = (evt.width, evt.height)
```

