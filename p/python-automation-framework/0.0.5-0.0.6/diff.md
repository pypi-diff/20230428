# Comparing `tmp/python-automation-framework-0.0.5.tar.gz` & `tmp/python-automation-framework-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.5.tar", last modified: Fri Apr 28 06:54:29 2023, max compression
+gzip compressed data, was "python-automation-framework-0.0.6.tar", last modified: Fri Apr 28 17:18:05 2023, max compression
```

## Comparing `python-automation-framework-0.0.5.tar` & `python-automation-framework-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.671743 python-automation-framework-0.0.5/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3106 2023-04-28 06:54:29.671571 python-automation-framework-0.0.5/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     2856 2023-04-28 06:45:27.000000 python-automation-framework-0.0.5/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.668954 python-automation-framework-0.0.5/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.5/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.5/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2283 2023-04-28 06:10:19.000000 python-automation-framework-0.0.5/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.5/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.5/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.5/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.5/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.5/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.5/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.5/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.5/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.5/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    12665 2023-04-28 06:51:28.000000 python-automation-framework-0.0.5/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6570 2023-04-27 13:27:22.000000 python-automation-framework-0.0.5/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.669851 python-automation-framework-0.0.5/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3106 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 06:54:29.000000 python-automation-framework-0.0.5/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 06:54:29.671788 python-automation-framework-0.0.5/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 06:54:24.000000 python-automation-framework-0.0.5/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 06:54:29.671373 python-automation-framework-0.0.5/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1060 2023-04-28 06:09:33.000000 python-automation-framework-0.0.5/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.5/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1292 2023-04-27 18:53:01.000000 python-automation-framework-0.0.5/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.5/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.5/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6986 2023-04-28 06:51:10.000000 python-automation-framework-0.0.5/test/test_uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.5/test/test_webdriver.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 17:18:05.808081 python-automation-framework-0.0.6/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3099 2023-04-28 17:18:05.807944 python-automation-framework-0.0.6/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2849 2023-04-28 07:57:13.000000 python-automation-framework-0.0.6/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 17:18:05.806164 python-automation-framework-0.0.6/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5741 2023-04-27 19:14:21.000000 python-automation-framework-0.0.6/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2567 2023-04-27 06:43:23.000000 python-automation-framework-0.0.6/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2283 2023-04-28 06:10:19.000000 python-automation-framework-0.0.6/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      309 2023-04-25 06:43:36.000000 python-automation-framework-0.0.6/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2430 2023-04-26 13:34:30.000000 python-automation-framework-0.0.6/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.6/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.6/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2544 2023-04-27 19:06:53.000000 python-automation-framework-0.0.6/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4249 2023-04-27 19:41:20.000000 python-automation-framework-0.0.6/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2737 2023-04-27 09:49:20.000000 python-automation-framework-0.0.6/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2476 2023-04-25 06:48:40.000000 python-automation-framework-0.0.6/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-04-19 09:45:36.000000 python-automation-framework-0.0.6/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    12781 2023-04-28 08:23:52.000000 python-automation-framework-0.0.6/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6580 2023-04-28 08:22:20.000000 python-automation-framework-0.0.6/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 17:18:05.806890 python-automation-framework-0.0.6/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3099 2023-04-28 17:18:05.000000 python-automation-framework-0.0.6/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      631 2023-04-28 17:18:05.000000 python-automation-framework-0.0.6/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-04-28 17:18:05.000000 python-automation-framework-0.0.6/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-04-28 17:18:05.000000 python-automation-framework-0.0.6/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-04-28 17:18:05.000000 python-automation-framework-0.0.6/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-04-28 17:18:05.808115 python-automation-framework-0.0.6/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-04-28 17:18:00.000000 python-automation-framework-0.0.6/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-04-28 17:18:05.807791 python-automation-framework-0.0.6/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1060 2023-04-28 06:09:33.000000 python-automation-framework-0.0.6/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      569 2023-04-19 16:18:15.000000 python-automation-framework-0.0.6/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1869 2023-04-28 08:20:26.000000 python-automation-framework-0.0.6/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1440 2023-04-27 19:24:35.000000 python-automation-framework-0.0.6/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1673 2023-04-27 19:37:23.000000 python-automation-framework-0.0.6/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6901 2023-04-28 08:14:15.000000 python-automation-framework-0.0.6/test/test_uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      844 2023-04-27 19:22:39.000000 python-automation-framework-0.0.6/test/test_webdriver.py
```

### Comparing `python-automation-framework-0.0.5/PKG-INFO` & `python-automation-framework-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
@@ -62,15 +62,15 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- Frames/ShadowRoot support
+- ShadowRoot support
 - Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
```

### Comparing `python-automation-framework-0.0.5/README.md` & `python-automation-framework-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- Frames/ShadowRoot support
+- ShadowRoot support
 - Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
```

### Comparing `python-automation-framework-0.0.5/paf/assertion.py` & `python-automation-framework-0.0.6/paf/assertion.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/common.py` & `python-automation-framework-0.0.6/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/component.py` & `python-automation-framework-0.0.6/paf/component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/control.py` & `python-automation-framework-0.0.6/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/javascript.py` & `python-automation-framework-0.0.6/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/locator.py` & `python-automation-framework-0.0.6/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/manager.py` & `python-automation-framework-0.0.6/paf/manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/page.py` & `python-automation-framework-0.0.6/paf/page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/request.py` & `python-automation-framework-0.0.6/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/paf/uielement.py` & `python-automation-framework-0.0.6/paf/uielement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 from abc import abstractmethod, ABC
 from datetime import datetime
 from pathlib import Path
-from typing import Callable, Type, TypeVar, List, Generic, Iterable, Iterator
+from typing import Type, TypeVar, List, Generic, Iterable, Iterator
 
 import inject
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.by import By as SeleniumBy
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.color import Color
@@ -147,42 +147,51 @@
 
     def __relative_selector(self, by: By):
         if by.by == SeleniumBy.XPATH:
             return by.value.replace("/", "./", 0)
         else:
             return by.value
 
+    def _filter_web_elements(self, web_elements: List[WebElement]):
+        if self._by.get_filter():
+            return list(filter(self._by.get_filter(), web_elements))
+        else:
+            return web_elements
+
     def _find_web_elements(self, consumer: Mapper[List[WebElement], R]) -> R:
         if self._ui_element:
             def _handle(web_element: WebElement):
                 value = self.__relative_selector(self._by)
-                web_elements = web_element.find_elements(self._by.by, value)
-                return consumer(web_elements)
+
+                is_frame = web_element.tag_name.lower() in ("frame", "iframe")
+                if is_frame:
+                    self._webdriver.switch_to.frame(web_element)
+                    web_elements = self._webdriver.find_elements(self._by.by, value)
+                else:
+                    web_elements = web_element.find_elements(self._by.by, value)
+
+                return consumer(self._filter_web_elements(web_elements))
 
             return self._ui_element.find_web_element(_handle)
         elif self._webdriver:
-            # Switch to default content
+            self._webdriver.switch_to.default_content()
             web_elements = self._webdriver.find_elements(self._by.by, self._by.value)
-            return consumer(web_elements)
+            return consumer(self._filter_web_elements(web_elements))
         else:
             raise Exception("UiElement initialized without WebDriver nor UiElement")
 
     def find_web_element(self, mapper: Mapper[WebElement, R]) -> R:
         def _handle(web_elements: List[WebElement]):
-            if self._by.get_filter():
-                web_elements = list(filter(self._by.get_filter(), web_elements))
-
             count = len(web_elements)
 
             if self._by.is_unique and count != 1:
                 raise Exception(f"Not unique")
             elif count > self._index:
-                # Switch to frame
-                return mapper(web_elements[self._index])
-                # Switch to default content
+                web_element = web_elements[self._index]
+                return mapper(web_element)
             else:
                 raise Exception(f"Not found")
 
         return self._find_web_elements(_handle)
 
     def _action_sequence(self, consumer: Consumer[WebElement]):
         control = inject.instance(Control)
@@ -274,18 +283,14 @@
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         return f"UiElement({self._by.__str__()})[{self._index}]"
 
-    # @property
-    # def list(self) -> "UiElementList":
-    #     return UiElementList(self)
-
     def scroll_into_view(self, offset: Point = Point()):
         self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, offset))
 
     def scroll_to_top(self, offset: Point = Point()):
         self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, offset))
 
     def _count_elements(self):
@@ -327,32 +332,24 @@
         self,
         ui_element: UiElement,
         raise_exception: bool = True,
     ):
         self._ui_element = ui_element
         self._raise = raise_exception
 
-    def _find_failsafe(self, mapper: Callable[[WebElement], any]):
-        try:
-            return self._ui_element.find_web_element(mapper)
-        except Exception as e:
-            pass
-
-        return None
-
     def _create_property_assertion(
         self,
         assertion_class: Type[A],
         mapper: Mapper[WebElement, any],
         property_name: str
     ) -> A:
         return assertion_class(
             parent=None,
             actual=lambda: self._ui_element.find_web_element(mapper),
-            subject=lambda: f"{self._ui_element.name_path}.{property_name} {Format.param(self._find_failsafe(mapper))}",
+            subject=lambda: f"{self._ui_element.name_path}.{property_name} {Format.param(self._ui_element.find_web_element(mapper))}",
             raise_exception=self._raise,
         )
 
     @property
     def text(self):
         def _map(web_element: WebElement):
             return web_element.text
```

### Comparing `python-automation-framework-0.0.5/paf/xpath.py` & `python-automation-framework-0.0.6/paf/xpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from paf.locator import By
 
 
 class XPath:
 
     def __init__(self, selector: str, position: int = None):
         self._selector = selector
-        if position and position == 0:
+        if position is not None and position == 0:
             position = 1
         self._pos = position
         self._root: XPath = None
         self._parent: XPath = None
         self._sub: XPath = None
         self._encloses: List[XPath] = []
         self._attributes: List[str] = []
@@ -82,16 +82,14 @@
         selector = XPath._normalize_selector(selector)
         xpath = XPath(XPath._translate_sub_selection(selector), position)
         xpath._root = self._root
         self._parent._sub = xpath
         xpath._parent = xpath
         return xpath
 
-
-
     def following(self, selector: any, position: int = None):
         selector = XPath._normalize_selector(selector)
         selector = XPath._translate_sibling(selector)
         return self.select(f"/following{selector}", position)
 
     def preceding(self, selector: any, position: int = None):
         selector = XPath._normalize_selector(selector)
```

### Comparing `python-automation-framework-0.0.5/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.0.6/python_automation_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 # PAF - Python Automation Framework
 
@@ -62,15 +62,15 @@
 - [Components](doc/components.md)
 - [Managing WebDrivers](doc/webdriver.md)
 - [Execution controlling](doc/control.md)
 
 ### Missing features (todos)
 
 - Rect assertions
-- Frames/ShadowRoot support
+- ShadowRoot support
 - Drag & Drop over frames
 
 ## Environment variables
 
 * `PAF_BROWSER_SETTING=chrome:90`: Sets the requested browser name and it's version.
 * `PAF_WINDOW_SIZE=1920x1080`: Sets the browsers default window size.
 * `PAF_SCREENSHOTS_DIR=screenshots`: Sets the screenshots' directory.
```

### Comparing `python-automation-framework-0.0.5/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.0.6/python_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/setup.py` & `python-automation-framework-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.5/test/test_component.py` & `python-automation-framework-0.0.6/test/test_component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/test/test_javascript.py` & `python-automation-framework-0.0.6/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/test/test_locator.py` & `python-automation-framework-0.0.6/test/test_locator.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 def test_deep_selection():
     assert str(XPath.at("button").attribute("data-qa").present.encloses("span").text.be("Klick mich")) == "//button[@data-qa and descendant::span[.//text()='Klick mich']]"
 
 
 def test_XPath_with_XPath():
     assert str(XPath.at("body").encloses(XPath.at("div"))) == "//body[descendant::div]"
 
+
 def test_XPath_with_By():
     assert str(XPath.at("body").encloses(By.tag_name("div"))) == "//body[descendant::div]"
 
+
 def test_select_sibling():
     assert str(XPath.at("body").select("dd").text.be("Title").following("/dt")) == "//body//dd[.//text()='Title']/following-sibling::dt"
+    assert str(XPath.at("body").select("dd").text.be("Title").following("dt")) == "//body//dd[.//text()='Title']/following::dt"
+    assert str(XPath.at("body").select("dd").text.be("Title").preceding("/dt")) == "//body//dd[.//text()='Title']/preceding-sibling::dt"
+    assert str(XPath.at("body").select("dd").text.be("Title").preceding("dt")) == "//body//dd[.//text()='Title']/preceding::dt"
 
 
 def test_class_selection():
     assert str(XPath.at("body").select("nav").classes("container")) == "//body//nav[contains(concat(' ', normalize-space(@class), ' '), ' container ')]"
+
+
+def test_position():
+    assert str(XPath.at("body", 1)) == "//body[1]"
+    assert str(XPath.at("body", 0)) == "//body[1]"
+    assert str(XPath.at("body", -1)) == "//body[last()]"
```

### Comparing `python-automation-framework-0.0.5/test/test_page.py` & `python-automation-framework-0.0.6/test/test_page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/test/test_request.py` & `python-automation-framework-0.0.6/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.5/test/test_uielement.py` & `python-automation-framework-0.0.6/test/test_uielement.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inject
+import pytest
 from selenium.webdriver.support.color import Color
 
 from paf.control import Control
 from paf.locator import By
 from paf.manager import WebDriverManager
 from paf.page import PageFactory, FinderPage
 from paf.xpath import XPath
@@ -12,16 +13,21 @@
 
 
 def setup_module():
     global page_factory
     page_factory = inject.instance(PageFactory)
 
 
-def test_finder_page():
+@pytest.fixture
+def finder():
     finder = page_factory.create_page(FinderPage, create_webdriver())
+    yield finder
+
+
+def test_finder_page(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     assert p.name_path == 'UiElement(By.id(para1))[0]'
     assert p.name == p.name_path
 
 
@@ -31,16 +37,15 @@
 #
 #     p = finder.find(By.id("para1"))
 #     rect = p._get_bounds()
 #     assert isinstance(rect, Rect)
 #     assert rect.width == 962
 #     assert rect.height == 27
 
-def test_text_assertions():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_text_assertions(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find("#para1")
 
     p.expect.tag_name.be("p")
 
     text = p.expect.text
@@ -58,47 +63,32 @@
     length.greater_equal_than(10).be(True)
     length.lower_than(20).be(True)
     length.lower_equal_than(30).be(True)
     length.between(18, 20).be(True)
     length.not_be(30)
 
 
-def test_wait():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_wait(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find("#para1")
 
     assert p.wait_for.tag_name.be("p") is True
     assert p.wait_for.tag_name.be("b") is False
 
 
-# def test_displayed():
-#     finder = page_factory.create_page(FinderPage, create_webdriver())
-#     finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
-#
-#     ok = finder.find("#dialog-ok")
-#     btn = finder.find("#fakealert")
-#
-#     ok.expect.displayed.be(False)
-#     btn.click()
-#     ok.expect.displayed.be(True)
-
-
-def test_highlight():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_highlight(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 
     p = finder.find(By.id("para1"))
     p.highlight(color=Color.from_string("#0f0"))
     p.expect.css("outline").be("rgb(0, 255, 0) solid 5px")
 
 
-def test_scroll_until_visible():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_scroll_until_visible(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
 
     p = finder.find(By.id("pre1").unique)
     p.expect.visible.be(False)
     p.scroll_into_view()
     p.expect.visible.be(True)
     p.expect.fully_visible.be(True)
@@ -106,16 +96,15 @@
     first = finder.find("#p1")
     first.expect.visible.be(False)
     first.scroll_to_top()
     first.expect.visible.be(True)
     p.expect.visible.be(False)
 
 
-def test_find_sub_elements_list():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_find_sub_elements_list(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
 
     # Sub elements
     div = finder.find("#div1")
     p = div.find("p")
     p.expect.attribute("name").be("pName1")
 
@@ -129,16 +118,15 @@
     p.last.expect.attribute("name").be("pName41")
 
     for item in p:
         item.expect.attribute("name").be("pName1")
         break
 
 
-def test_form():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_form(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/basic-html-form-test.html")
 
     checkbox = finder.find(XPath.at("input").name("checkboxes[]").attribute("value").be("cb3"))
     checkbox.expect.selected.be(True)
 
     textarea = finder.find(By.name("comments"))
     textarea.expect.value.be("Comments...")
@@ -149,35 +137,32 @@
     username.expect.enabled.be(True)
     username.send_keys("My Name")
     username.expect.value.be("My Name")
     username.clear()
     username.expect.value.be("")
 
 
-def test_screenshot():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_screenshot(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/find-by-playground-test.html")
     p = finder.find(By.id("pre1").unique)
     path = p.take_screenshot()
     assert path
 
 
-def test_retry():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_retry(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/key-click-display-test.html")
     btn = finder.find(By.id("button").unique)
     clicks = finder.find(XPath.at("div").id("events").select("p"))
 
     control = inject.instance(Control)
     btn.click()
     control.retry(lambda: clicks.expect.count.be(3), lambda: btn.click(), wait_after_fail=0, count=3)
 
 
-def test_actions():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_actions(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/events/javascript-events.html")
 
     click_btn = finder.find("#onclick")
     click_status = finder.find("#onclickstatus")
     click_status.expect.displayed.be(False)
     click_btn.click()
     click_status.expect.displayed.be(True)
@@ -197,20 +182,41 @@
     double_click_btn = finder.find("#ondoubleclick")
     double_click_status = finder.find("#ondoubleclickstatus")
     double_click_status.expect.displayed.be(False)
     double_click_btn.double_click()
     double_click_status.expect.displayed.be(True)
 
 
-def test_drag_and_drop():
-    finder = page_factory.create_page(FinderPage, create_webdriver())
+def test_drag_and_drop(finder: FinderPage):
     finder.open("https://testpages.herokuapp.com/styled/drag-drop-javascript.html")
 
     drag = finder.find(".drag.left")
     drop = finder.find("#droppable1")
     drop.expect.text.be("Drop here")
     drag.drag_and_drop_to(drop)
     drop.expect.text.be("Dropped!")
 
 
+def test_frames(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/frames/frames-test.html")
+    left = finder.find(By.name("left"))
+    left.expect.tag_name.be("frame")
+    left.find("li").expect.count.be(30)
+    left.expect.tag_name.be("frame")
+
+    top = finder.find(By.name("top"))
+    exp = top.find(By.class_name("explanation"))
+    exp.expect.text.starts_with("This page").be(True)
+
+
+def test_locate_displayed(finder: FinderPage):
+    finder.open("https://testpages.herokuapp.com/styled/alerts/fake-alert-test.html")
+    ok = finder.find(By.id("dialog-ok").displayed)
+    btn = finder.find("#fakealert")
+
+    ok.expect.count.be(0)
+    btn.click()
+    ok.expect.count.be(1)
+
+
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.5/test/test_webdriver.py` & `python-automation-framework-0.0.6/test/test_webdriver.py`

 * *Files identical despite different names*

